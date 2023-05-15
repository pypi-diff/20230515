# Comparing `tmp/tox-ansible-2.0.2.tar.gz` & `tmp/tox-ansible-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-ansible-2.0.2.tar", last modified: Wed May 10 20:29:37 2023, max compression
+gzip compressed data, was "tox-ansible-2.0.3.tar", last modified: Mon May 15 18:57:08 2023, max compression
```

## Comparing `tox-ansible-2.0.2.tar` & `tox-ansible-2.0.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.818992 tox-ansible-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.810992 tox-ansible-2.0.2/.config/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.config/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.810992 tox-ansible-2.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.810992 tox-ansible-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.github/workflows/run.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-10 20:29:37.818992 tox-ansible-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.814992 tox-ansible-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/docs/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/docs/integration.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/docs/sanity.ini
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/docs/tox-ansible.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/docs/unit.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:29:37.818992 tox-ansible-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.806992 tox-ansible-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.814992 tox-ansible-2.0.2/src/tox_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/src/tox_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 20:29:37.000000 tox-ansible-2.0.2/src/tox_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/src/tox_ansible/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.814992 tox-ansible-2.0.2/src/tox_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-10 20:29:37.000000 tox-ansible-2.0.2/src/tox_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 20:29:37.000000 tox-ansible-2.0.2/src/tox_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:29:37.000000 tox-ansible-2.0.2/src/tox_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 20:29:37.000000 tox-ansible-2.0.2/src/tox_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-10 20:29:37.000000 tox-ansible-2.0.2/src/tox_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 20:29:37.000000 tox-ansible-2.0.2/src/tox_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.814992 tox-ansible-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.806992 tox-ansible-2.0.2/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.806992 tox-ansible-2.0.2/tests/fixtures/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.814992 tox-ansible-2.0.2/tests/fixtures/integration/test_basic/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tests/fixtures/integration/test_basic/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tests/fixtures/integration/test_basic/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.818992 tox-ansible-2.0.2/tests/fixtures/integration/test_user_provided/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tests/fixtures/integration/test_user_provided/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tests/fixtures/integration/test_user_provided/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:29:37.818992 tox-ansible-2.0.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tests/integration/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tests/integration/test_user_provided.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-10 20:29:19.000000 tox-ansible-2.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.560289 tox-ansible-2.0.3/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.config/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.564288 tox-ansible-2.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.568288 tox-ansible-2.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/workflows/run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.568288 tox-ansible-2.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/integration.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/sanity.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/tox-ansible.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/unit.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.552288 tox-ansible-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.572289 tox-ansible-2.0.3/src/tox_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/src/tox_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/src/tox_ansible/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.576289 tox-ansible-2.0.3/src/tox_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.576289 tox-ansible-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.552288 tox-ansible-2.0.3/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.552288 tox-ansible-2.0.3/tests/fixtures/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.576289 tox-ansible-2.0.3/tests/fixtures/integration/test_basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/fixtures/integration/test_basic/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/fixtures/integration/test_basic/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/tests/fixtures/integration/test_user_provided/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/fixtures/integration/test_user_provided/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/fixtures/integration/test_user_provided/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/integration/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/integration/test_user_provided.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tox.ini
```

### Comparing `tox-ansible-2.0.2/.flake8` & `tox-ansible-2.0.3/.flake8`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/.github/workflows/release.yml` & `tox-ansible-2.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/.github/workflows/run.yml` & `tox-ansible-2.0.3/.github/workflows/run.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/.github/workflows/tox.yml` & `tox-ansible-2.0.3/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/.gitignore` & `tox-ansible-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/.pre-commit-config.yaml` & `tox-ansible-2.0.3/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   - repo: https://github.com/Lucas-C/pre-commit-hooks.git
     rev: v1.5.1
     hooks:
       - id: remove-tabs
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         always_run: true
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
@@ -41,15 +41,15 @@
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: "1.3.0"
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.263"
+    rev: "v0.0.267"
     hooks:
       - id: ruff
         args:
           - "--exit-non-zero-on-fix"
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
     rev: v6.31.0
@@ -75,15 +75,15 @@
           - --output-format=colorized
         additional_dependencies:
           - pytest
           - tox
           - pyyaml
 
   - repo: https://github.com/pre-commit/mirrors-mypy.git
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         additional_dependencies:
           - pytest
           - tox
           - types-PyYAML
         args:
```

### Comparing `tox-ansible-2.0.2/LICENSE` & `tox-ansible-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/PKG-INFO` & `tox-ansible-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.2
+Version: 2.0.3
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tox-ansible-2.0.2/README.md` & `tox-ansible-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/cspell.config.yaml` & `tox-ansible-2.0.3/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/docs/galaxy.yml` & `tox-ansible-2.0.3/docs/galaxy.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/docs/integration.ini` & `tox-ansible-2.0.3/docs/integration.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/docs/sanity.ini` & `tox-ansible-2.0.3/docs/sanity.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/docs/unit.ini` & `tox-ansible-2.0.3/docs/unit.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/pyproject.toml` & `tox-ansible-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/requirements.txt` & `tox-ansible-2.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/src/tox_ansible/plugin.py` & `tox-ansible-2.0.3/src/tox_ansible/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     "rsync",
     "mkdir",
     "cd",
     "echo",
 ]
 ENV_LIST = """
 {integration, sanity, unit}-py3.8-{2.9, 2.12, 2.13}
-{integration, sanity, unit}-py3.9-{2.12, 2.13, 2.14, milestone, devel}
-{integration, sanity, unit}-py3.10-{2.12, 2.13, 2.14, milestone, devel}
-{integration, sanity, unit}-py3.11-{2.14, milestone, devel}
+{integration, sanity, unit}-py3.9-{2.12, 2.13, 2.14, 2.15, milestone, devel}
+{integration, sanity, unit}-py3.10-{2.12, 2.13, 2.14, 2.15, milestone, devel}
+{integration, sanity, unit}-py3.11-{2.14, 2.15, milestone, devel}
 """
 TOX_WORK_DIR = Path()
 OUR_DEPS = [
     "pytest",
     "pytest-xdist",
     "pytest-ansible",
 ]
```

### Comparing `tox-ansible-2.0.2/src/tox_ansible.egg-info/PKG-INFO` & `tox-ansible-2.0.3/src/tox_ansible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.2
+Version: 2.0.3
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tox-ansible-2.0.2/src/tox_ansible.egg-info/SOURCES.txt` & `tox-ansible-2.0.3/src/tox_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/tests/conftest.py` & `tox-ansible-2.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/tests/integration/test_basic.py` & `tox-ansible-2.0.3/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/tests/integration/test_user_provided.py` & `tox-ansible-2.0.3/tests/integration/test_user_provided.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.2/tox.ini` & `tox-ansible-2.0.3/tox.ini`

 * *Files identical despite different names*

