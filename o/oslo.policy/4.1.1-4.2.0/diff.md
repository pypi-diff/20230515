# Comparing `tmp/oslo.policy-4.1.1.tar.gz` & `tmp/oslo.policy-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.policy-4.1.1.tar", last modified: Tue Feb 21 17:37:31 2023, max compression
+gzip compressed data, was "oslo.policy-4.2.0.tar", last modified: Mon May 15 08:53:37 2023, max compression
```

## Comparing `oslo.policy-4.1.1.tar` & `oslo.policy-4.2.0.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.283450 oslo.policy-4.1.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5376 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23365 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2023-02-21 17:37:31.283450 oslo.policy-4.1.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.263451 oslo.policy-4.1.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.263451 oslo.policy-4.1.1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.263451 oslo.policy-4.1.1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8793 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/admin/policy-json-file.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9315 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/admin/policy-yaml-file.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.267451 oslo.policy-4.1.1/doc/source/cli/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.267451 oslo.policy-4.1.1/doc/source/cli/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/common/convert-opts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/common/default-opts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/common/enforcer-opts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/common/generator-opts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/common/rule-opts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/oslopolicy-checker.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2667 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/oslopolicy-convert-json-to-yaml.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1185 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/oslopolicy-list-redundant.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/oslopolicy-policy-generator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/oslopolicy-sample-generator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/cli/oslopolicy-validator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3502 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.267451 oslo.policy-4.1.1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.267451 oslo.policy-4.1.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.267451 oslo.policy-4.1.1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.267451 oslo.policy-4.1.1/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.267451 oslo.policy-4.1.1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/user/plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2366 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/user/sphinxpolicygen.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23236 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.271451 oslo.policy-4.1.1/oslo.policy.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/oslo.policy.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4893 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/oslo.policy.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/oslo.policy.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/oslo.policy.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/oslo.policy.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/oslo.policy.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/oslo.policy.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-02-21 17:37:31.000000 oslo.policy-4.1.1/oslo.policy.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.271451 oslo.policy-4.1.1/oslo_policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/_cache_handler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9916 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4330 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/_external.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10377 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/_parser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2200 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25684 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/generator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.259451 oslo.policy-4.1.1/oslo_policy/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.259451 oslo.policy-4.1.1/oslo_policy/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.271451 oslo.policy-4.1.1/oslo_policy/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6214 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/locale/en_GB/LC_MESSAGES/oslo_policy.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6389 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62696 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4385 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5231 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/sphinxext.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3735 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/sphinxpolicygen.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.275451 oslo.policy-4.1.1/oslo_policy/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2317 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2981 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_cache_handler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16004 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14037 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_external.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2151 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41454 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_generator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20853 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_parser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    85821 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8488 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3801 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_sphinxext.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3519 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/test_sphinxpolicygen.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11244 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/tests/token_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/oslo_policy/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.259451 oslo.policy-4.1.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.279451 oslo.policy-4.1.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/Fix-map-system-scope-for-creds-dict-e4cbec2f7495f22e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/Pass-target-dict-to-oslopolicy-checker-87185d40aec413ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/add-deprecated-metadata-to-DeprecatedRule-79d2e8a3f5d11743.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/add-policy-convert-json-to-yaml-tool-3c93604aee79f58a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/add-policy-upgrade-command-a65bc4f760e5d8b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/add-scope-types-to-sphinxext-cacd845c4575e965.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/add-sphinxpolicygen-39e2f8fa24930b0c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/add_custom_rule_check_plugins-3c15c2c7ca5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/add_reno-3b4ae0789e9c45b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/bug-1779172-c1323c0f647bc44c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/bug-1880959-8f1370a59759d40d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/bug-1913718-f1b46bbff3231d98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/bug-1943584-fc74f9205039883c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/deprecate-policy-file-json-format-e1921f15b5d00287.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/drop-python27-support-9aa06224812cc352.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/enforce-scope-checks-always-when-rule-has-scope_types-8f983cdf70766e4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/enforce_new_defaults-6ae17d8b8d166a2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/enforce_scope_types-1e92f6a34e4173ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/expand-cli-docs-02c2f13adbe251c0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/fix-bug-1914095-fa71d81c9639ba94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/fix-deprecated-rule-handling-c6fe321fce6293a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/fix-passing-exclude-deprecated-param-317745d23022e544.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/fix-rendering-for-deprecated-rules-d465292e4155f483.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/list-redundant-deprecation-warnings-f84a06133efdaedd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/oslo-policy-descriptive-support-3ee688c5fa48d751.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/policy-check-performance-fbad83c7a4afd7d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/notes/policy-file-validator-906d5cff864a2d51.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.283450 oslo.policy-4.1.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.283450 oslo.policy-4.1.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.283450 oslo.policy-4.1.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8741 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.259451 oslo.policy-4.1.1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.259451 oslo.policy-4.1.1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.283450 oslo.policy-4.1.1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7465 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.259451 oslo.policy-4.1.1/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.283450 oslo.policy-4.1.1/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:37:31.283450 oslo.policy-4.1.1/sample_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5008 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/sample_data/auth_v3_token_admin.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5014 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/sample_data/auth_v3_token_member.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5028 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/sample_data/auth_v3_token_system_admin.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-02-21 17:37:31.283450 oslo.policy-4.1.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1489 2023-02-21 17:37:06.000000 oslo.policy-4.1.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.074841 oslo.policy-4.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5412 2023-05-15 08:53:36.000000 oslo.policy-4.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23612 2023-05-15 08:53:36.000000 oslo.policy-4.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1988 2023-05-15 08:53:37.074841 oslo.policy-4.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.050836 oslo.policy-4.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.050836 oslo.policy-4.2.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.050836 oslo.policy-4.2.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8793 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/admin/policy-json-file.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9315 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/admin/policy-yaml-file.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.054837 oslo.policy-4.2.0/doc/source/cli/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.054837 oslo.policy-4.2.0/doc/source/cli/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/common/convert-opts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/common/default-opts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/common/enforcer-opts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/common/generator-opts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/common/rule-opts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/oslopolicy-checker.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2667 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/oslopolicy-convert-json-to-yaml.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1185 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/oslopolicy-list-redundant.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/oslopolicy-policy-generator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/oslopolicy-sample-generator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/cli/oslopolicy-validator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3502 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.054837 oslo.policy-4.2.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.054837 oslo.policy-4.2.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.054837 oslo.policy-4.2.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.054837 oslo.policy-4.2.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.054837 oslo.policy-4.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/user/plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2366 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/user/sphinxpolicygen.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23236 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.058838 oslo.policy-4.2.0/oslo.policy.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1988 2023-05-15 08:53:36.000000 oslo.policy-4.2.0/oslo.policy.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4924 2023-05-15 08:53:37.000000 oslo.policy-4.2.0/oslo.policy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:53:36.000000 oslo.policy-4.2.0/oslo.policy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-05-15 08:53:36.000000 oslo.policy-4.2.0/oslo.policy.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:53:36.000000 oslo.policy-4.2.0/oslo.policy.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-15 08:53:36.000000 oslo.policy-4.2.0/oslo.policy.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-15 08:53:36.000000 oslo.policy-4.2.0/oslo.policy.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-05-15 08:53:36.000000 oslo.policy-4.2.0/oslo.policy.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.058838 oslo.policy-4.2.0/oslo_policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/_cache_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9916 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4330 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/_external.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10377 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/_parser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2200 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25684 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/generator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.046835 oslo.policy-4.2.0/oslo_policy/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.046835 oslo.policy-4.2.0/oslo_policy/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.062838 oslo.policy-4.2.0/oslo_policy/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6214 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/locale/en_GB/LC_MESSAGES/oslo_policy.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6389 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62737 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4385 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5231 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/sphinxext.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3735 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/sphinxpolicygen.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.062838 oslo.policy-4.2.0/oslo_policy/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2317 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2981 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_cache_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16004 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14037 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_external.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2151 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41454 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20853 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_parser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    85821 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8488 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3801 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_sphinxext.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3519 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/test_sphinxpolicygen.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11244 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/tests/token_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/oslo_policy/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.046835 oslo.policy-4.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.070840 oslo.policy-4.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/Fix-map-system-scope-for-creds-dict-e4cbec2f7495f22e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/Pass-target-dict-to-oslopolicy-checker-87185d40aec413ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/add-deprecated-metadata-to-DeprecatedRule-79d2e8a3f5d11743.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/add-policy-convert-json-to-yaml-tool-3c93604aee79f58a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/add-policy-upgrade-command-a65bc4f760e5d8b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/add-scope-types-to-sphinxext-cacd845c4575e965.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/add-sphinxpolicygen-39e2f8fa24930b0c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/add_custom_rule_check_plugins-3c15c2c7ca5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/add_reno-3b4ae0789e9c45b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/bug-1779172-c1323c0f647bc44c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/bug-1880959-8f1370a59759d40d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/bug-1913718-f1b46bbff3231d98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/bug-1943584-fc74f9205039883c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/deprecate-policy-file-json-format-e1921f15b5d00287.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/drop-python27-support-9aa06224812cc352.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/enforce-scope-checks-always-when-rule-has-scope_types-8f983cdf70766e4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/enforce_new_defaults-6ae17d8b8d166a2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/enforce_scope_types-1e92f6a34e4173ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/expand-cli-docs-02c2f13adbe251c0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/fix-bug-1914095-fa71d81c9639ba94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/fix-deprecated-rule-handling-c6fe321fce6293a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/fix-passing-exclude-deprecated-param-317745d23022e544.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/fix-rendering-for-deprecated-rules-d465292e4155f483.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/list-redundant-deprecation-warnings-f84a06133efdaedd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/oslo-policy-descriptive-support-3ee688c5fa48d751.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/policy-check-performance-fbad83c7a4afd7d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/notes/policy-file-validator-906d5cff864a2d51.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.074841 oslo.policy-4.2.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.074841 oslo.policy-4.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.074841 oslo.policy-4.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8741 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.046835 oslo.policy-4.2.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.046835 oslo.policy-4.2.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.074841 oslo.policy-4.2.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7465 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.046835 oslo.policy-4.2.0/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.074841 oslo.policy-4.2.0/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:53:37.074841 oslo.policy-4.2.0/sample_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5008 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/sample_data/auth_v3_token_admin.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5014 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/sample_data/auth_v3_token_member.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5028 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/sample_data/auth_v3_token_system_admin.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2023-05-15 08:53:37.074841 oslo.policy-4.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1489 2023-05-15 08:52:40.000000 oslo.policy-4.2.0/tox.ini
```

### Comparing `oslo.policy-4.1.1/.pre-commit-config.yaml` & `oslo.policy-4.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/AUTHORS` & `oslo.policy-4.2.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 Edan David <edand@mellanox.com>
 Eric Brown <browne@vmware.com>
 Eric Windisch <eric@cloudscaling.com>
 Flaper Fesp <flaper87@gmail.com>
 Flavio Percoco <flaper87@gmail.com>
 Florent Flament <florent.flament-ext@cloudwatt.com>
 Gary Kotton <gkotton@redhat.com>
+Ghanshyam <gmann@ghanshyammann.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Haiwei Xu <xu-haiwei@mxw.nes.nec.co.jp>
 He Jie Xu <hejie.xu@intel.com>
 He Jie Xu <xuhj@linux.vnet.ibm.com>
 Hervé Beraud <hberaud@redhat.com>
 Ian Cordasco <graffatcolmingov@gmail.com>
 Ian Cordasco <ian.cordasco@rackspace.com>
```

### Comparing `oslo.policy-4.1.1/CONTRIBUTING.rst` & `oslo.policy-4.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/ChangeLog` & `oslo.policy-4.2.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+4.2.0
+-----
+
+* Revert "Moves supported python runtimes from version 3.8 to 3.10"
+* Moves supported python runtimes from version 3.8 to 3.10
+* Fix deprecated rule logic if the rule was deleted in policy directory
+* Update master for stable/2023.1
+
 4.1.1
 -----
 
 * Fix py38 jobs by using focal rather than jammy
 
 4.1.0
 -----
```

### Comparing `oslo.policy-4.1.1/LICENSE` & `oslo.policy-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/PKG-INFO` & `oslo.policy-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.policy
-Version: 4.1.1
+Version: 4.2.0
 Summary: Oslo Policy library
 Home-page: https://docs.openstack.org/oslo.policy/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -40,10 +40,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
```

### Comparing `oslo.policy-4.1.1/README.rst` & `oslo.policy-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/admin/policy-json-file.rst` & `oslo.policy-4.2.0/doc/source/admin/policy-json-file.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/admin/policy-yaml-file.rst` & `oslo.policy-4.2.0/doc/source/admin/policy-yaml-file.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/cli/common/default-opts.rst` & `oslo.policy-4.2.0/doc/source/cli/common/default-opts.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/cli/oslopolicy-checker.rst` & `oslo.policy-4.2.0/doc/source/cli/oslopolicy-checker.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/cli/oslopolicy-convert-json-to-yaml.rst` & `oslo.policy-4.2.0/doc/source/cli/oslopolicy-convert-json-to-yaml.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/cli/oslopolicy-list-redundant.rst` & `oslo.policy-4.2.0/doc/source/cli/oslopolicy-list-redundant.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/cli/oslopolicy-policy-generator.rst` & `oslo.policy-4.2.0/doc/source/cli/oslopolicy-policy-generator.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/cli/oslopolicy-sample-generator.rst` & `oslo.policy-4.2.0/doc/source/cli/oslopolicy-sample-generator.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/cli/oslopolicy-validator.rst` & `oslo.policy-4.2.0/doc/source/cli/oslopolicy-validator.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/conf.py` & `oslo.policy-4.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/index.rst` & `oslo.policy-4.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/user/plugins.rst` & `oslo.policy-4.2.0/doc/source/user/plugins.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/user/sphinxpolicygen.rst` & `oslo.policy-4.2.0/doc/source/user/sphinxpolicygen.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/doc/source/user/usage.rst` & `oslo.policy-4.2.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo.policy.egg-info/PKG-INFO` & `oslo.policy-4.2.0/oslo.policy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.policy
-Version: 4.1.1
+Version: 4.2.0
 Summary: Oslo Policy library
 Home-page: https://docs.openstack.org/oslo.policy/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -40,10 +40,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
```

### Comparing `oslo.policy-4.1.1/oslo.policy.egg-info/SOURCES.txt` & `oslo.policy-4.2.0/oslo.policy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 releasenotes/notes/fix-deprecated-rule-handling-c6fe321fce6293a9.yaml
 releasenotes/notes/fix-passing-exclude-deprecated-param-317745d23022e544.yaml
 releasenotes/notes/fix-rendering-for-deprecated-rules-d465292e4155f483.yaml
 releasenotes/notes/list-redundant-deprecation-warnings-f84a06133efdaedd.yaml
 releasenotes/notes/oslo-policy-descriptive-support-3ee688c5fa48d751.yaml
 releasenotes/notes/policy-check-performance-fbad83c7a4afd7d7.yaml
 releasenotes/notes/policy-file-validator-906d5cff864a2d51.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
```

### Comparing `oslo.policy-4.1.1/oslo.policy.egg-info/entry_points.txt` & `oslo.policy-4.2.0/oslo.policy.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/_cache_handler.py` & `oslo.policy-4.2.0/oslo_policy/_cache_handler.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/_checks.py` & `oslo.policy-4.2.0/oslo_policy/_checks.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/_external.py` & `oslo.policy-4.2.0/oslo_policy/_external.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/_i18n.py` & `oslo.policy-4.2.0/oslo_policy/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/_parser.py` & `oslo.policy-4.2.0/oslo_policy/_parser.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/fixture.py` & `oslo.policy-4.2.0/oslo_policy/fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/generator.py` & `oslo.policy-4.2.0/oslo_policy/generator.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/locale/en_GB/LC_MESSAGES/oslo_policy.po` & `oslo.policy-4.2.0/oslo_policy/locale/en_GB/LC_MESSAGES/oslo_policy.po`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/opts.py` & `oslo.policy-4.2.0/oslo_policy/opts.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/policy.py` & `oslo.policy-4.2.0/oslo_policy/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,14 +660,15 @@
                     if not policy_file_rules_changed and self.overwrite:
                         self._load_policy_file(path=self.policy_path,
                                                force_reload=True,
                                                overwrite=self.overwrite
                                                )
                 elif self.overwrite:
                     self.rules = Rules(default_rule=self.default_rule)
+                    self.file_rules = {}
                 for path in existing_policy_dirs:
                     self._walk_through_policy_directory(
                         path, self._load_policy_file, True, False)
 
             for default in self.registered_rules.values():
                 if default.deprecated_for_removal:
                     self._emit_deprecated_for_removal_warning(default)
```

### Comparing `oslo.policy-4.1.1/oslo_policy/shell.py` & `oslo.policy-4.2.0/oslo_policy/shell.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/sphinxext.py` & `oslo.policy-4.2.0/oslo_policy/sphinxext.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/sphinxpolicygen.py` & `oslo.policy-4.2.0/oslo_policy/sphinxpolicygen.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/base.py` & `oslo.policy-4.2.0/oslo_policy/tests/base.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_cache_handler.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_cache_handler.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_checks.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_external.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_external.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_fixtures.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_generator.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_opts.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_opts.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_parser.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_policy.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_shell.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_sphinxext.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_sphinxext.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/test_sphinxpolicygen.py` & `oslo.policy-4.2.0/oslo_policy/tests/test_sphinxpolicygen.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/tests/token_fixture.py` & `oslo.policy-4.2.0/oslo_policy/tests/token_fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/oslo_policy/version.py` & `oslo.policy-4.2.0/oslo_policy/version.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/releasenotes/notes/bug-1779172-c1323c0f647bc44c.yaml` & `oslo.policy-4.2.0/releasenotes/notes/bug-1779172-c1323c0f647bc44c.yaml`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/releasenotes/notes/deprecate-policy-file-json-format-e1921f15b5d00287.yaml` & `oslo.policy-4.2.0/releasenotes/notes/deprecate-policy-file-json-format-e1921f15b5d00287.yaml`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/releasenotes/notes/enforce_new_defaults-6ae17d8b8d166a2c.yaml` & `oslo.policy-4.2.0/releasenotes/notes/enforce_new_defaults-6ae17d8b8d166a2c.yaml`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/releasenotes/notes/enforce_scope_types-1e92f6a34e4173ef.yaml` & `oslo.policy-4.2.0/releasenotes/notes/enforce_scope_types-1e92f6a34e4173ef.yaml`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/releasenotes/notes/fix-deprecated-rule-handling-c6fe321fce6293a9.yaml` & `oslo.policy-4.2.0/releasenotes/notes/fix-deprecated-rule-handling-c6fe321fce6293a9.yaml`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/releasenotes/notes/oslo-policy-descriptive-support-3ee688c5fa48d751.yaml` & `oslo.policy-4.2.0/releasenotes/notes/oslo-policy-descriptive-support-3ee688c5fa48d751.yaml`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/releasenotes/source/conf.py` & `oslo.policy-4.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.policy-4.2.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `oslo.policy-4.2.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/sample_data/auth_v3_token_admin.json` & `oslo.policy-4.2.0/sample_data/auth_v3_token_admin.json`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/sample_data/auth_v3_token_member.json` & `oslo.policy-4.2.0/sample_data/auth_v3_token_member.json`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/sample_data/auth_v3_token_system_admin.json` & `oslo.policy-4.2.0/sample_data/auth_v3_token_system_admin.json`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/setup.cfg` & `oslo.policy-4.2.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [files]
 packages = 
 	oslo_policy
```

### Comparing `oslo.policy-4.1.1/setup.py` & `oslo.policy-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.policy-4.1.1/tox.ini` & `oslo.policy-4.2.0/tox.ini`

 * *Files identical despite different names*

