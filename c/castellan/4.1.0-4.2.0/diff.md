# Comparing `tmp/castellan-4.1.0.tar.gz` & `tmp/castellan-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castellan-4.1.0.tar", last modified: Fri Feb 10 16:08:47 2023, max compression
+gzip compressed data, was "castellan-4.2.0.tar", last modified: Mon May 15 08:45:16 2023, max compression
```

## Comparing `castellan-4.1.0.tar` & `castellan-4.2.0.tar`

### file list

```diff
@@ -1,168 +1,170 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.481918 castellan-4.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-02-10 16:08:07.000000 castellan-4.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-02-10 16:08:07.000000 castellan-4.1.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-02-10 16:08:07.000000 castellan-4.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-02-10 16:08:07.000000 castellan-4.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1995 2023-02-10 16:08:07.000000 castellan-4.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3403 2023-02-10 16:08:47.000000 castellan-4.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1996 2023-02-10 16:08:07.000000 castellan-4.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12663 2023-02-10 16:08:47.000000 castellan-4.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2023-02-10 16:08:07.000000 castellan-4.1.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-10 16:08:07.000000 castellan-4.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1618 2023-02-10 16:08:47.481918 castellan-4.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2023-02-10 16:08:07.000000 castellan-4.1.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-02-10 16:08:07.000000 castellan-4.1.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.469918 castellan-4.1.0/castellan/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4971 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/_config_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.469918 castellan-4.1.0/castellan/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.469918 castellan-4.1.0/castellan/common/credentials/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/credentials/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/credentials/credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5483 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/credentials/keystone_password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4330 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/credentials/keystone_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1688 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/credentials/password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/credentials/token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2593 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.469918 castellan-4.1.0/castellan/common/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5743 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/managed_object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/opaque_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/passphrase.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2056 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/private_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2093 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/public_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2067 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/symmetric_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/objects/x_509.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7966 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.473918 castellan-4.1.0/castellan/key_manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2113 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/key_manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30228 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/key_manager/barbican_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5978 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/key_manager/key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2893 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/key_manager/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/key_manager/not_implemented_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14199 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/key_manager/vault_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7935 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/options.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.473918 castellan-4.1.0/castellan/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.473918 castellan-4.1.0/castellan/tests/contrib/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       66 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/contrib/gate_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1081 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/contrib/post_test_hook.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.473918 castellan-4.1.0/castellan/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2426 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/functional/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.473918 castellan-4.1.0/castellan/tests/functional/key_manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/functional/key_manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6877 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/functional/key_manager/test_barbican_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9787 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/functional/key_manager/test_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6201 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/functional/key_manager/test_vault_key_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.473918 castellan-4.1.0/castellan/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.473918 castellan-4.1.0/castellan/tests/unit/credentials/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/credentials/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16252 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/credentials/test_keystone_password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10091 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/credentials/test_keystone_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/credentials/test_password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/credentials/test_token.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.473918 castellan-4.1.0/castellan/tests/unit/key_manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/key_manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/key_manager/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9050 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/key_manager/mock_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26545 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/key_manager/test_barbican_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1616 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/key_manager/test_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5061 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/key_manager/test_migration_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9613 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/key_manager/test_mock_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1983 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/key_manager/test_not_implemented_key_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2626 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/key_manager/test_vault_key_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/castellan/tests/unit/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3504 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/objects/test_opaque.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3547 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/objects/test_passphrase.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5794 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/objects/test_private_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5779 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/objects/test_public_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5739 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/objects/test_symmetric_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3670 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/objects/test_x_509.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3948 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/test_config_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/test_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7149 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16264 2023-02-10 16:08:07.000000 castellan-4.1.0/castellan/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.469918 castellan-4.1.0/castellan.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1618 2023-02-10 16:08:47.000000 castellan-4.1.0/castellan.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5231 2023-02-10 16:08:47.000000 castellan-4.1.0/castellan.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:08:47.000000 castellan-4.1.0/castellan.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2023-02-10 16:08:47.000000 castellan-4.1.0/castellan.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:08:47.000000 castellan-4.1.0/castellan.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-10 16:08:47.000000 castellan-4.1.0/castellan.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-02-10 16:08:47.000000 castellan-4.1.0/castellan.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-02-10 16:08:47.000000 castellan-4.1.0/castellan.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-02-10 16:08:07.000000 castellan-4.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/doc/source/_extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-02-10 16:08:07.000000 castellan-4.1.0/doc/source/_extra/.htaccess
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2023-02-10 16:08:07.000000 castellan-4.1.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2023-02-10 16:08:07.000000 castellan-4.1.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-02-10 16:08:07.000000 castellan-4.1.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3500 2023-02-10 16:08:07.000000 castellan-4.1.0/doc/source/contributor/testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-02-10 16:08:07.000000 castellan-4.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-02-10 16:08:07.000000 castellan-4.1.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10896 2023-02-10 16:08:07.000000 castellan-4.1.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.465918 castellan-4.1.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/etc/castellan/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-02-10 16:08:07.000000 castellan-4.1.0/etc/castellan/functional-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-02-10 16:08:07.000000 castellan-4.1.0/etc/castellan/sample-config-generator.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.465918 castellan-4.1.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/playbooks/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-02-10 16:08:07.000000 castellan-4.1.0/playbooks/devstack/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-02-10 16:08:07.000000 castellan-4.1.0/playbooks/devstack/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-02-10 16:08:07.000000 castellan-4.1.0/playbooks/devstack/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.465918 castellan-4.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.477918 castellan-4.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/add-to-dict-and-from-dict-conversions-to-managed-objects-95a9f0fdbd371a87.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/add-vault-provider-29a4c19fe67ab51f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/barbican-service-user-11ebbfcd33dace9d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/bug-1876102-7c7288fb6e90b11d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/deprecate-auth-endpoint-b91a3e67b5c7263f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/fix-vault-create-key-b4340a3067cbd93c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/fix-vault-flaky-kv-api-version-b0cd9d62a39d2907.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/implements-keymanager-option-discovery-13a46c1dfc036a3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/support-legacy-fixed-key-id-9fa897b547111610.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/use-barbican-endpoint-type-config-option-e583d30930cc22ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/use-barbican-region-name-config-option-31bec809292302b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/vault-approle-support-5ea04daea07a152f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/vault-kv-mountpoint-919eb547764a0c74.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/notes/vault-namespaces-7d334e7407396df9.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.481918 castellan-4.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.481918 castellan-4.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.481918 castellan-4.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8863 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-10 16:08:07.000000 castellan-4.1.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2023-02-10 16:08:07.000000 castellan-4.1.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2023-02-10 16:08:47.481918 castellan-4.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-10 16:08:07.000000 castellan-4.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2023-02-10 16:08:07.000000 castellan-4.1.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:47.481918 castellan-4.1.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      852 2023-02-10 16:08:07.000000 castellan-4.1.0/tools/setup-vault-env.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2023-02-10 16:08:07.000000 castellan-4.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.481426 castellan-4.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-05-15 08:44:53.000000 castellan-4.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-15 08:44:53.000000 castellan-4.2.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-05-15 08:44:53.000000 castellan-4.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-05-15 08:44:53.000000 castellan-4.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1993 2023-05-15 08:44:53.000000 castellan-4.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3515 2023-05-15 08:45:16.000000 castellan-4.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1996 2023-05-15 08:44:53.000000 castellan-4.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13065 2023-05-15 08:45:16.000000 castellan-4.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2023-05-15 08:44:53.000000 castellan-4.2.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-15 08:44:53.000000 castellan-4.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2023-05-15 08:45:16.481426 castellan-4.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2023-05-15 08:44:53.000000 castellan-4.2.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-05-15 08:44:53.000000 castellan-4.2.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.457426 castellan-4.2.0/castellan/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4971 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/_config_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.461426 castellan-4.2.0/castellan/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.461426 castellan-4.2.0/castellan/common/credentials/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/credentials/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/credentials/credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5483 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/credentials/keystone_password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4330 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/credentials/keystone_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1688 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/credentials/password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/credentials/token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2593 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.461426 castellan-4.2.0/castellan/common/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5743 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/managed_object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/opaque_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/passphrase.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2056 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/private_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2093 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/public_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2067 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/symmetric_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/objects/x_509.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7966 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.465426 castellan-4.2.0/castellan/key_manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2113 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/key_manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32712 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/key_manager/barbican_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7723 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/key_manager/key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2893 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/key_manager/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2059 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/key_manager/not_implemented_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14950 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/key_manager/vault_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8182 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/options.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.465426 castellan-4.2.0/castellan/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.465426 castellan-4.2.0/castellan/tests/contrib/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       66 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/contrib/gate_hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1081 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/contrib/post_test_hook.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.465426 castellan-4.2.0/castellan/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2426 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/functional/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.465426 castellan-4.2.0/castellan/tests/functional/key_manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/functional/key_manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18965 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/functional/key_manager/test_barbican_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9787 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/functional/key_manager/test_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6201 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/functional/key_manager/test_vault_key_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.465426 castellan-4.2.0/castellan/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.469426 castellan-4.2.0/castellan/tests/unit/credentials/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/credentials/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16252 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/credentials/test_keystone_password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10091 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/credentials/test_keystone_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/credentials/test_password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/credentials/test_token.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.469426 castellan-4.2.0/castellan/tests/unit/key_manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/key_manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/key_manager/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9758 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/key_manager/mock_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40614 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/key_manager/test_barbican_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1616 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/key_manager/test_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5061 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/key_manager/test_migration_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9613 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/key_manager/test_mock_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1983 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/key_manager/test_not_implemented_key_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2626 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/key_manager/test_vault_key_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.469426 castellan-4.2.0/castellan/tests/unit/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3504 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/objects/test_opaque.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3547 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/objects/test_passphrase.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5794 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/objects/test_private_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5779 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/objects/test_public_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5739 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/objects/test_symmetric_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3670 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/objects/test_x_509.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3948 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/test_config_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/test_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7149 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16264 2023-05-15 08:44:53.000000 castellan-4.2.0/castellan/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.461426 castellan-4.2.0/castellan.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2023-05-15 08:45:16.000000 castellan-4.2.0/castellan.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5320 2023-05-15 08:45:16.000000 castellan-4.2.0/castellan.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:45:16.000000 castellan-4.2.0/castellan.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2023-05-15 08:45:16.000000 castellan-4.2.0/castellan.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:45:16.000000 castellan-4.2.0/castellan.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-15 08:45:16.000000 castellan-4.2.0/castellan.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-15 08:45:16.000000 castellan-4.2.0/castellan.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-05-15 08:45:16.000000 castellan-4.2.0/castellan.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.469426 castellan-4.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-15 08:44:53.000000 castellan-4.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.469426 castellan-4.2.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.469426 castellan-4.2.0/doc/source/_extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-15 08:44:53.000000 castellan-4.2.0/doc/source/_extra/.htaccess
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2023-05-15 08:44:53.000000 castellan-4.2.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.473426 castellan-4.2.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2023-05-15 08:44:53.000000 castellan-4.2.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-05-15 08:44:53.000000 castellan-4.2.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3500 2023-05-15 08:44:53.000000 castellan-4.2.0/doc/source/contributor/testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-05-15 08:44:53.000000 castellan-4.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.473426 castellan-4.2.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-15 08:44:53.000000 castellan-4.2.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.473426 castellan-4.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12174 2023-05-15 08:44:53.000000 castellan-4.2.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.453426 castellan-4.2.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.473426 castellan-4.2.0/etc/castellan/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-15 08:44:53.000000 castellan-4.2.0/etc/castellan/functional-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-05-15 08:44:53.000000 castellan-4.2.0/etc/castellan/sample-config-generator.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.453426 castellan-4.2.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.473426 castellan-4.2.0/playbooks/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-05-15 08:44:53.000000 castellan-4.2.0/playbooks/devstack/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-05-15 08:44:53.000000 castellan-4.2.0/playbooks/devstack/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-05-15 08:44:53.000000 castellan-4.2.0/playbooks/devstack/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.453426 castellan-4.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.477426 castellan-4.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/add-to-dict-and-from-dict-conversions-to-managed-objects-95a9f0fdbd371a87.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/add-vault-provider-29a4c19fe67ab51f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/barbican-service-user-11ebbfcd33dace9d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/bug-1876102-7c7288fb6e90b11d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/deprecate-auth-endpoint-b91a3e67b5c7263f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/fix-vault-create-key-b4340a3067cbd93c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/fix-vault-flaky-kv-api-version-b0cd9d62a39d2907.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/implements-keymanager-option-discovery-13a46c1dfc036a3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/secret-consumers-0253330a65b6638b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/support-legacy-fixed-key-id-9fa897b547111610.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/use-barbican-endpoint-type-config-option-e583d30930cc22ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/use-barbican-region-name-config-option-31bec809292302b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/vault-approle-support-5ea04daea07a152f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/vault-kv-mountpoint-919eb547764a0c74.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/notes/vault-namespaces-7d334e7407396df9.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.477426 castellan-4.2.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.477426 castellan-4.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.477426 castellan-4.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8863 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-15 08:44:53.000000 castellan-4.2.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2023-05-15 08:44:53.000000 castellan-4.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2023-05-15 08:45:16.481426 castellan-4.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-15 08:44:53.000000 castellan-4.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2023-05-15 08:44:53.000000 castellan-4.2.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:45:16.477426 castellan-4.2.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      852 2023-05-15 08:44:53.000000 castellan-4.2.0/tools/setup-vault-env.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2023-05-15 08:44:53.000000 castellan-4.2.0/tox.ini
```

### Comparing `castellan-4.1.0/.pre-commit-config.yaml` & `castellan-4.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/.zuul.yaml` & `castellan-4.2.0/.zuul.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 - job:
     name: castellan-functional-vault
-    parent: openstack-tox-py38
+    parent: openstack-tox-py310
     description: |
       Run tox functional-vault target
     required-projects:
       - name: openstack/castellan
     vars:
-      tox_envlist: functional-vault
+      tox_envlist: functional-vault-py310
 
 - job:
     name: castellan-functional-devstack
     parent: devstack
     description: |
       Run DevStack-based Castellan functional tests
     pre-run: playbooks/devstack/pre.yaml
@@ -55,11 +55,11 @@
     gate:
       jobs:
         - castellan-functional-vault
         - castellan-functional-devstack
         - barbican-tempest-plugin-simple-crypto-castellan-src
     templates:
       - check-requirements
-      - openstack-python3-antelope-jobs
+      - openstack-python3-jobs
       - periodic-stable-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
```

### Comparing `castellan-4.1.0/AUTHORS` & `castellan-4.2.0/AUTHORS`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 Douglas Mendizábal <mail@doug.gt>
 Dung Ha <dunght@vn.fujitsu.com>
 Ellen Batbouta <ellen.batbouta@oracle.com>
 Elod Illes <elod.illes@est.tech>
 Eric Harney <eharney@redhat.com>
 Fernando Diaz <diazjf@us.ibm.com>
 Flavio Percoco <flaper87@gmail.com>
+Ghanshyam <gmann@ghanshyammann.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Grzegorz Grasza <xek@redhat.com>
 Hervé Beraud <hberaud@redhat.com>
 Ian Wienand <iwienand@redhat.com>
 Ivan Kolodyazhny <e0ne@e0ne.info>
 James E. Blair <jeblair@redhat.com>
 James Page <james.page@ubuntu.com>
@@ -41,25 +42,27 @@
 Kaitlin Farr <kaitlin.farr@jhuapl.edu>
 Kiran_totad <kiran.totad@nectechnologies.in>
 Le Hou <houl7@chinaunicom.cn>
 LiZekun <2954674728@qq.com>
 Lingxian Kong <anlin.kong@gmail.com>
 Luigi Toscano <ltoscano@redhat.com>
 Mark Goddard <mark@stackhpc.com>
+Mauricio Harley <mharley@redhat.com>
 Michael McCune <msm@redhat.com>
 Moises Guimaraes de Medeiros <moguimar@redhat.com>
 Moisés Guimarães de Medeiros <moguimar@redhat.com>
 Monty Taylor <mordred@inaugust.com>
 Nguyen Van Trung <trungnv@vn.fujitsu.com>
 Niall Bunting <niall.bunting@hpe.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Paul Bourke <paul.bourke@oracle.com>
 Pavlo Shchelokovskyy <shchelokovskyy@gmail.com>
 Robert Clark <hyakuhei@gmail.com>
 Sam Morrison <sorrison@gmail.com>
+Scott Solkhon <scottsolkhon@gmail.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Steve Martinelli <s.martinelli@gmail.com>
 Sungjin Yook <sungyook@us.ibm.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Takashi Kajinami <tkajinam@redhat.com>
 Tim Kelsey <tim.kelsey@hp.com>
 Tom Cocozzello <tjcocozz@us.ibm.com>
```

### Comparing `castellan-4.1.0/CONTRIBUTING.rst` & `castellan-4.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/ChangeLog` & `castellan-4.2.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 CHANGES
 =======
 
+4.2.0
+-----
+
+* Revert "Moves supported python runtimes from version 3.8 to 3.10"
+* Moves supported python runtimes from version 3.8 to 3.10
+* Update master for stable/2023.1
+* Add secret consumers documentation and release note
+* Add force parameter functional tests
+* Add secret consumers functional tests
+* Implement force parameter
+* Add secret consumers
+
 4.1.0
 -----
 
 * Initial change to add secret consumers
+* Add support for specifying Vault KV path
 * Fix tox4 error
 * Make tests more consistent
 * Add Python3 antelope unit tests
 * Update master for stable/zed
 
 4.0.0
 -----
```

### Comparing `castellan-4.1.0/HACKING.rst` & `castellan-4.2.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/LICENSE` & `castellan-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/PKG-INFO` & `castellan-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: castellan
-Version: 4.1.0
+Version: 4.2.0
 Summary: Generic Key Manager interface for OpenStack
 Home-page: https://docs.openstack.org/castellan/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =========
         Castellan
@@ -32,10 +32,11 @@
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

### Comparing `castellan-4.1.0/README.rst` & `castellan-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/__init__.py` & `castellan-4.2.0/castellan/__init__.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/_config_driver.py` & `castellan-4.2.0/castellan/_config_driver.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/credentials/credential.py` & `castellan-4.2.0/castellan/common/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/credentials/keystone_password.py` & `castellan-4.2.0/castellan/common/credentials/keystone_password.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/credentials/keystone_token.py` & `castellan-4.2.0/castellan/common/credentials/keystone_token.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/credentials/password.py` & `castellan-4.2.0/castellan/common/credentials/password.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/credentials/token.py` & `castellan-4.2.0/castellan/common/credentials/token.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/exception.py` & `castellan-4.2.0/castellan/common/exception.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/__init__.py` & `castellan-4.2.0/castellan/common/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/certificate.py` & `castellan-4.2.0/castellan/common/objects/certificate.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/key.py` & `castellan-4.2.0/castellan/common/objects/key.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/managed_object.py` & `castellan-4.2.0/castellan/common/objects/managed_object.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/opaque_data.py` & `castellan-4.2.0/castellan/common/objects/opaque_data.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/passphrase.py` & `castellan-4.2.0/castellan/common/objects/passphrase.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/private_key.py` & `castellan-4.2.0/castellan/common/objects/private_key.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/public_key.py` & `castellan-4.2.0/castellan/common/objects/public_key.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/symmetric_key.py` & `castellan-4.2.0/castellan/common/objects/symmetric_key.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/objects/x_509.py` & `castellan-4.2.0/castellan/common/objects/x_509.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/common/utils.py` & `castellan-4.2.0/castellan/common/utils.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/i18n.py` & `castellan-4.2.0/castellan/i18n.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/key_manager/__init__.py` & `castellan-4.2.0/castellan/key_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/key_manager/barbican_key_manager.py` & `castellan-4.2.0/castellan/key_manager/barbican_key_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 from castellan.common import exception
 from castellan.common.objects import key as key_base_class
 from castellan.common.objects import opaque_data as op_data
 from castellan.i18n import _
 from castellan.key_manager import key_manager
 
-
 from barbicanclient import client as barbican_client_import
 from barbicanclient import exceptions as barbican_exceptions
 from oslo_utils import timeutils
 
 
 _barbican_opts = [
     cfg.StrOpt('barbican_endpoint',
@@ -156,15 +155,14 @@
         except Exception as e:
             LOG.error("Error creating Barbican client: %s", e)
             raise exception.KeyManagerError(reason=e)
 
         self._base_url = self._create_base_url(auth,
                                                sess,
                                                self._barbican_endpoint)
-
         return self._barbican_client
 
     def _get_keystone_auth(self, context):
         if context.__class__.__name__ == 'KeystonePassword':
             auth = identity.Password(
                 auth_url=context.auth_url,
                 username=context.username,
@@ -548,25 +546,28 @@
         # convert created ISO8601 in Barbican to POSIX
         if secret.created:
             time_stamp = timeutils.parse_isotime(
                 str(secret.created)).timetuple()
             created = calendar.timegm(time_stamp)
 
         if issubclass(secret_type, key_base_class.Key):
-            return secret_type(secret.algorithm,
-                               secret.bit_length,
-                               secret_data,
-                               secret.name,
-                               created,
-                               object_id)
+            return secret_type(algorithm=secret.algorithm,
+                               bit_length=secret.bit_length,
+                               key=secret_data,
+                               name=secret.name,
+                               created=created,
+                               id=object_id,
+                               consumers=secret.consumers)
         else:
+            # Opaque Data or Passphrase
             return secret_type(secret_data,
-                               secret.name,
-                               created,
-                               object_id)
+                               name=secret.name,
+                               created=created,
+                               id=object_id,
+                               consumers=secret.consumers)
 
     def _get_secret(self, context, object_id):
         """Returns the metadata of the secret.
 
         :param context: contains information of the user and the environment
                         for the request (castellan/context.py)
         :param object_id: UUID of the secret
@@ -614,38 +615,85 @@
             LOG.error("Error retrieving object: %s", e)
             if self._is_secret_not_found_error(e):
                 raise exception.ManagedObjectNotFoundError(
                     uuid=managed_object_id)
             else:
                 raise exception.KeyManagerError(reason=e)
 
-    def delete(self, context, managed_object_id):
+    def delete(self, context, managed_object_id, force=False):
         """Deletes the specified managed object.
 
         :param context: contains information of the user and the environment
                      for the request (castellan/context.py)
         :param managed_object_id: the UUID of the object to delete
+        :param force: specifies if the secret must be deleted even when they
+                     have consumers.
+        :raises ValueError: if the secret has consumers but no force parameter
+                     is provided or if force equals False.
         :raises KeyManagerError: if object deletion fails
         :raises ManagedObjectNotFoundError: if the object could not be found
         """
         barbican_client = self._get_barbican_client(context)
-
         try:
             secret_ref = self._create_secret_ref(managed_object_id)
-            barbican_client.secrets.delete(secret_ref)
+            barbican_client.secrets.delete(secret_ref, force)
         except (barbican_exceptions.HTTPAuthError,
                 barbican_exceptions.HTTPClientError,
                 barbican_exceptions.HTTPServerError) as e:
             LOG.error("Error deleting object: %s", e)
             if self._is_secret_not_found_error(e):
                 raise exception.ManagedObjectNotFoundError(
                     uuid=managed_object_id)
             else:
                 raise exception.KeyManagerError(reason=e)
 
+    def add_consumer(self, context, managed_object_id, consumer_data):
+        """Add a consumer to the specified managed object
+
+        :param context: contains information of the user and the environment
+                     for the request (castellan/context.py)
+        :param managed_object_id: the UUID of the object to update
+        :param consumer_data: dict containing consumer data
+        :raises KeyManagerError: if object deletion fails
+        :raises ManagedObjectNotFoundError: if the object could not be found
+        """
+
+        barbican_client = self._get_barbican_client(context)
+        try:
+            secret_ref = self._create_secret_ref(managed_object_id)
+            barbican_client.secrets.register_consumer(
+                secret_ref, **consumer_data)
+
+        except (barbican_exceptions.HTTPAuthError,
+                barbican_exceptions.HTTPClientError,
+                barbican_exceptions.HTTPServerError) as e:
+            LOG.error("Error adding consumer: %s", e)
+            if self._is_secret_not_found_error(e):
+                raise exception.ManagedObjectNotFoundError(
+                    uuid=managed_object_id)
+            else:
+                raise exception.KeyManagerError(reason=e)
+
+    def remove_consumer(self, context, managed_object_id, consumer_data):
+
+        barbican_client = self._get_barbican_client(context)
+        try:
+            secret_ref = self._create_secret_ref(managed_object_id)
+            barbican_client.secrets.remove_consumer(
+                secret_ref, **consumer_data)
+        except (barbican_exceptions.HTTPAuthError,
+                barbican_exceptions.HTTPClientError,
+                barbican_exceptions.HTTPServerError) as e:
+            LOG.error("Error removing consumer: %s", e)
+            if self._is_secret_not_found_error(e):
+                raise exception.ManagedObjectNotFoundError(
+                    uuid=managed_object_id)
+            else:
+                raise exception.KeyManagerError(reason=e)
+
     def list(self, context, object_type=None, metadata_only=False):
         """Retrieves a list of managed objects that match the criteria.
 
         If no search criteria is given, all objects are returned.
 
         :param context: contains information of the user and the environment
                      for the request (castellan/context.py)
```

### Comparing `castellan-4.1.0/castellan/key_manager/key_manager.py` & `castellan-4.2.0/castellan/key_manager/key_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -102,27 +102,65 @@
         UUIDs of objects that belong to other users by repeatedly calling
         this method. That is, objects that belong to other users should be
         considered "non-existent" and completely invisible.
         """
         pass
 
     @abc.abstractmethod
-    def delete(self, context, managed_object_id):
+    def delete(self, context, managed_object_id, force=False):
         """Deletes the specified managed object.
 
         Implementations should verify that the caller has permission to delete
         the managed object by checking the context object (context). A
         NotAuthorized exception should be raised if the caller lacks
         permission.
 
         If the specified object does not exist, then a KeyError should be
         raised. Implementations should preclude users from discerning the
         UUIDs of objects that belong to other users by repeatedly calling this
         method. That is, objects that belong to other users should be
         considered "non-existent" and completely invisible.
+
+        Implementations that block the deletion of secrets with consumers
+        without making the "force" parameter equals True should raise
+        an exception.
+        """
+        pass
+
+    @abc.abstractmethod
+    def add_consumer(self, context, managed_object_id, consumer_data):
+        """Add a consumer to a managed object.
+
+        Implementations should verify that the caller has permission to
+        add a consumer to the managed object by checking the context object
+        (context). A NotAuthorized exception should be raised if the caller
+        lacks permission.
+
+        If the specified object does not exist, then a KeyError should be
+        raised. Implementations should preclude users from discerning the
+        UUIDs of objects that belong to other users by repeatedly calling this
+        method. That is, objects that belong to other users should be
+        considered "non-existent" and completely invisible.
+        """
+        pass
+
+    @abc.abstractmethod
+    def remove_consumer(self, context, managed_object_id, consumer_data):
+        """Remove a consumer from a managed object.
+
+        Implementations should verify that the caller has permission to
+        remove a consumer to the managed object by checking the context object
+        (context). A NotAuthorized exception should be raised if the caller
+        lacks permission.
+
+        If the specified object does not exist, then a KeyError should be
+        raised. Implementations should preclude users from discerning the
+        UUIDs of objects that belong to other users by repeatedly calling this
+        method. That is, objects that belong to other users should be
+        considered "non-existent" and completely invisible.
         """
         pass
 
     def list(self, context, object_type=None, metadata_only=False):
         """Lists the managed objects given the criteria.
 
         Implementations should verify that the caller has permission to list
```

### Comparing `castellan-4.1.0/castellan/key_manager/migration.py` & `castellan-4.2.0/castellan/key_manager/migration.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/key_manager/not_implemented_key_manager.py` & `castellan-4.2.0/castellan/key_manager/not_implemented_key_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -44,9 +44,15 @@
 
     def get(self, context, managed_object_id, **kwargs):
         raise NotImplementedError()
 
     def list(self, context, object_type=None):
         raise NotImplementedError()
 
-    def delete(self, context, managed_object_id, **kwargs):
+    def delete(self, context, managed_object_id, force=False):
+        raise NotImplementedError()
+
+    def add_consumer(self, context, managed_object_id, consumer_data):
+        raise NotImplementedError()
+
+    def remove_consumer(self, context, managed_object_id, consumer_data):
         raise NotImplementedError()
```

### Comparing `castellan-4.1.0/castellan/key_manager/vault_key_manager.py` & `castellan-4.2.0/castellan/key_manager/vault_key_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,17 @@
                help='AppRole role_id for authentication with vault'),
     cfg.StrOpt('approle_secret_id',
                help='AppRole secret_id for authentication with vault'),
     cfg.StrOpt('kv_mountpoint',
                default=_DEFAULT_MOUNTPOINT,
                help='Mountpoint of KV store in Vault to use, for example: '
                     '{}'.format(_DEFAULT_MOUNTPOINT)),
+    cfg.StrOpt('kv_path',
+               help='Path relative to root of KV store in Vault to use.'
+               ),
     cfg.IntOpt('kv_version',
                default=_DEFAULT_VERSION,
                help='Version of KV store in Vault to use, for example: '
                     '{}'.format(_DEFAULT_VERSION)),
     cfg.StrOpt('vault_url',
                default=_DEFAULT_VAULT_URL,
                help='Use this endpoint to connect to Vault, for example: '
@@ -97,36 +100,37 @@
         self._root_token_id = self._conf.vault.root_token_id
         self._approle_role_id = self._conf.vault.approle_role_id
         self._approle_secret_id = self._conf.vault.approle_secret_id
         self._cached_approle_token_id = None
         self._approle_token_ttl = None
         self._approle_token_issue = None
         self._kv_mountpoint = self._conf.vault.kv_mountpoint
+        self._kv_path = self._conf.vault.kv_path
         self._kv_version = self._conf.vault.kv_version
         self._vault_url = self._conf.vault.vault_url
         self._namespace = self._conf.vault.namespace
         if self._vault_url.startswith("https://"):
             self._verify_server = self._conf.vault.ssl_ca_crt_file or True
         else:
             self._verify_server = False
 
     def _get_url(self):
         if not self._vault_url.endswith('/'):
             self._vault_url += '/'
         return self._vault_url
 
     def _get_resource_url(self, key_id=None):
-        return '{}v1/{}/{}{}'.format(
+        return '{}v1/{}/{}{}{}'.format(
             self._get_url(),
             self._kv_mountpoint,
 
             '' if self._kv_version == 1 else
             'data/' if key_id else
             'metadata/',  # no key_id is for listing and 'data/' doesn't works
-
+            (self._kv_path + '/') if self._kv_path else '',
             key_id if key_id else '?list=true')
 
     @property
     def _approle_token_id(self):
         if (all((self._approle_token_issue, self._approle_token_ttl)) and
                 timeutils.is_older_than(self._approle_token_issue,
                                         self._approle_token_ttl)):
@@ -339,26 +343,40 @@
                          key_id)
         else:
             return clazz(key,
                          record['name'],
                          record['created'],
                          key_id)
 
-    def delete(self, context, key_id):
-        """Represents deleting the key."""
+    def delete(self, context, key_id, force=False):
+        """Represents deleting the key.
+
+        The 'force' parameter is not used whatsoever and only kept to allow
+        consistency with the Barbican implementation.
+        """
 
         if not key_id:
             raise exception.KeyManagerError('key identifier not provided')
 
         resp = self._do_http_request(self._session.delete,
                                      self._get_resource_url(key_id))
 
         if resp.status_code == requests.codes['not_found']:
             raise exception.ManagedObjectNotFoundError(uuid=key_id)
 
+    def add_consumer(self, context, managed_object_id, consumer_data):
+        raise NotImplementedError(
+            "VaultKeyManager does not implement adding consumers"
+        )
+
+    def remove_consumer(self, context, managed_object_id, consumer_data):
+        raise NotImplementedError(
+            "VaultKeyManager does not implement deleting consumers"
+        )
+
     def list(self, context, object_type=None, metadata_only=False):
         """Lists the managed objects given the criteria."""
 
         if object_type and object_type not in self._secret_type_dict:
             msg = _("Invalid secret type: %s") % object_type
             raise exception.KeyManagerError(reason=msg)
```

### Comparing `castellan-4.1.0/castellan/options.py` & `castellan-4.2.0/castellan/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 def set_defaults(conf, backend=None, barbican_endpoint=None,
                  barbican_api_version=None, auth_endpoint=None,
                  retry_delay=None, number_of_retries=None, verify_ssl=None,
                  verify_ssl_path=None,
                  api_class=None, vault_root_token_id=None,
                  vault_approle_role_id=None, vault_approle_secret_id=None,
-                 vault_kv_mountpoint=None, vault_url=None,
+                 vault_kv_mountpoint=None, vault_kv_path=None, vault_url=None,
                  vault_ssl_ca_crt_file=None, vault_use_ssl=None,
                  vault_namespace=None,
                  barbican_endpoint_type=None,
                  vault_kv_version=None):
     """Set defaults for configuration values.
 
     Overrides the default options values.
@@ -57,14 +57,15 @@
     :param verify_ssl: Use this to specify if ssl should be verified.
     :param verify_ssl_path: Use this to specify the CA path.
     :param vault_root_token_id: Use this for the root token id for vault.
     :param vault_approle_role_id: Use this for the approle role_id for vault.
     :param vault_approle_secret_id: Use this for the approle secret_id
                                     for vault.
     :param vault_kv_mountpoint: Mountpoint of KV store in vault to use.
+    :param vault_kv_path: Path relative to root of KV store in Vault to use.
     :param vault_url: Use this for the url for vault.
     :param vault_use_ssl: Use this to force vault driver to use ssl.
     :param vault_ssl_ca_crt_file: Use this for the CA file for vault.
     :param vault_namespace: Namespace to use for all requests to Vault.
     :param barbican_endpoint_type: Use this to specify the type of URL.
     :                              Valid values are: public, internal or admin.
     :param vault_kv_version: Use this for the kv version for vault.
@@ -120,14 +121,17 @@
                              group=vkm._VAULT_OPT_GROUP)
         if vault_approle_secret_id is not None:
             conf.set_default('approle_secret_id', vault_approle_secret_id,
                              group=vkm._VAULT_OPT_GROUP)
         if vault_kv_mountpoint is not None:
             conf.set_default('kv_mountpoint', vault_kv_mountpoint,
                              group=vkm._VAULT_OPT_GROUP)
+        if vault_kv_path is not None:
+            conf.set_default('kv_path', vault_kv_path,
+                             group=vkm._VAULT_OPT_GROUP)
         if vault_url is not None:
             conf.set_default('vault_url', vault_url,
                              group=vkm._VAULT_OPT_GROUP)
         if vault_ssl_ca_crt_file is not None:
             conf.set_default('ssl_ca_crt_file', vault_ssl_ca_crt_file,
                              group=vkm._VAULT_OPT_GROUP)
         if vault_use_ssl is not None:
```

### Comparing `castellan-4.1.0/castellan/tests/base.py` & `castellan-4.2.0/castellan/tests/base.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/contrib/post_test_hook.sh` & `castellan-4.2.0/castellan/tests/contrib/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/functional/config.py` & `castellan-4.2.0/castellan/tests/functional/config.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/functional/key_manager/test_key_manager.py` & `castellan-4.2.0/castellan/tests/functional/key_manager/test_key_manager.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/functional/key_manager/test_vault_key_manager.py` & `castellan-4.2.0/castellan/tests/functional/key_manager/test_vault_key_manager.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/credentials/test_keystone_password.py` & `castellan-4.2.0/castellan/tests/unit/credentials/test_keystone_password.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/credentials/test_keystone_token.py` & `castellan-4.2.0/castellan/tests/unit/credentials/test_keystone_token.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/credentials/test_password.py` & `castellan-4.2.0/castellan/tests/unit/credentials/test_password.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/credentials/test_token.py` & `castellan-4.2.0/castellan/tests/unit/credentials/test_token.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/key_manager/fake.py` & `castellan-4.2.0/castellan/tests/unit/key_manager/fake.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/key_manager/mock_key_manager.py` & `castellan-4.2.0/castellan/tests/unit/key_manager/mock_key_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -195,14 +195,30 @@
         KeyError is raised if the UUID is invalid.
         """
         if context is None:
             raise exception.Forbidden()
 
         del self.keys[managed_object_id]
 
+    def add_consumer(self, context, managed_object_id, consumer_data):
+        if context is None:
+            raise exception.Forbidden()
+        if managed_object_id not in self.keys:
+            raise exception.ManagedObjectNotFoundError()
+        self.keys[managed_object_id].consumers.append(consumer_data)
+
+    def remove_consumer(self, context, managed_object_id, consumer_data):
+        if context is None:
+            raise exception.Forbidden()
+        if managed_object_id not in self.keys:
+            raise exception.ManagedObjectNotFoundError()
+        self.keys[managed_object_id].consumers = [
+            c for c in self.keys[managed_object_id].consumers
+            if c != consumer_data]
+
     def _generate_password(self, length, symbolgroups):
         """Generate a random password from the supplied symbol groups.
 
         At least one symbol from each group will be included. Unpredictable
         results if length is less than the number of symbol groups.
 
         Believed to be reasonably secure (with a reasonable password length!)
```

### Comparing `castellan-4.1.0/castellan/tests/unit/key_manager/test_key_manager.py` & `castellan-4.2.0/castellan/tests/unit/key_manager/test_key_manager.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/key_manager/test_migration_key_manager.py` & `castellan-4.2.0/castellan/tests/unit/key_manager/test_migration_key_manager.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/key_manager/test_mock_key_manager.py` & `castellan-4.2.0/castellan/tests/unit/key_manager/test_mock_key_manager.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/key_manager/test_not_implemented_key_manager.py` & `castellan-4.2.0/castellan/tests/unit/key_manager/test_not_implemented_key_manager.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/key_manager/test_vault_key_manager.py` & `castellan-4.2.0/castellan/tests/unit/key_manager/test_vault_key_manager.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/objects/__init__.py` & `castellan-4.2.0/castellan/tests/unit/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/objects/test_opaque.py` & `castellan-4.2.0/castellan/tests/unit/objects/test_opaque.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/objects/test_passphrase.py` & `castellan-4.2.0/castellan/tests/unit/objects/test_passphrase.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/objects/test_private_key.py` & `castellan-4.2.0/castellan/tests/unit/objects/test_private_key.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/objects/test_public_key.py` & `castellan-4.2.0/castellan/tests/unit/objects/test_public_key.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/objects/test_symmetric_key.py` & `castellan-4.2.0/castellan/tests/unit/objects/test_symmetric_key.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/objects/test_x_509.py` & `castellan-4.2.0/castellan/tests/unit/objects/test_x_509.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/test_config_driver.py` & `castellan-4.2.0/castellan/tests/unit/test_config_driver.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/test_options.py` & `castellan-4.2.0/castellan/tests/unit/test_options.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/unit/test_utils.py` & `castellan-4.2.0/castellan/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan/tests/utils.py` & `castellan-4.2.0/castellan/tests/utils.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/castellan.egg-info/PKG-INFO` & `castellan-4.2.0/castellan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: castellan
-Version: 4.1.0
+Version: 4.2.0
 Summary: Generic Key Manager interface for OpenStack
 Home-page: https://docs.openstack.org/castellan/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =========
         Castellan
@@ -32,10 +32,11 @@
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

### Comparing `castellan-4.1.0/castellan.egg-info/SOURCES.txt` & `castellan-4.2.0/castellan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -107,20 +107,22 @@
 releasenotes/notes/barbican-service-user-11ebbfcd33dace9d.yaml
 releasenotes/notes/bug-1876102-7c7288fb6e90b11d.yaml
 releasenotes/notes/deprecate-auth-endpoint-b91a3e67b5c7263f.yaml
 releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
 releasenotes/notes/fix-vault-create-key-b4340a3067cbd93c.yaml
 releasenotes/notes/fix-vault-flaky-kv-api-version-b0cd9d62a39d2907.yaml
 releasenotes/notes/implements-keymanager-option-discovery-13a46c1dfc036a3f.yaml
+releasenotes/notes/secret-consumers-0253330a65b6638b.yaml
 releasenotes/notes/support-legacy-fixed-key-id-9fa897b547111610.yaml
 releasenotes/notes/use-barbican-endpoint-type-config-option-e583d30930cc22ba.yaml
 releasenotes/notes/use-barbican-region-name-config-option-31bec809292302b8.yaml
 releasenotes/notes/vault-approle-support-5ea04daea07a152f.yaml
 releasenotes/notes/vault-kv-mountpoint-919eb547764a0c74.yaml
 releasenotes/notes/vault-namespaces-7d334e7407396df9.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
```

### Comparing `castellan-4.1.0/doc/source/conf.py` & `castellan-4.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/doc/source/contributor/testing.rst` & `castellan-4.2.0/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/doc/source/user/index.rst` & `castellan-4.2.0/doc/source/user/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -169,14 +169,55 @@
 
 Having finished our work with the key, we can now delete it from the key
 manager service. We once again instantiate a key manager, then we simply
 delete the key by using its identifier. Under normal conditions, this call
 will not return anything but may raise exceptions if there are communication,
 identification, or authorization issues.
 
+**Example. Secret consumers.**
+
+.. code:: python
+
+    import myapp
+    from castellan import key_manager
+
+    manager = key_manager.API()
+
+    # Listing consumers:
+    stored_secret = self.key_mgr.get(myapp.context(), stored_id)
+    consumer_list = stored_secret.consumers  # consumers is a list of dicts
+
+    # Adding consumers:
+    consumer = {'service': 'glance',
+	        'resource_type': 'image',
+                'resource_id': 'image_id'}
+    try:
+        manager.add_consumer(myapp.context(), stored_id, consumer)
+    except NotImplementedError:
+        pass  # backends like Vault don't support adding/removing consumers
+
+    # Remove the consumer before calling secret delete without the force flag:
+    try:
+	manager.remove_consumer(myapp.context(), stored_id, consumer)
+    except NotImplementedError:
+        pass
+    manager.delete(myapp.context(), stored_key_id)
+
+    # Alternatively, force delete a secret
+    manager.delete(myapp.context(), stored_key_id, force=True)
+
+After creating a secret, we can add consumers to it. Secrets with consumers
+cannot be deleted without using the force flag.
+
+.. note::
+
+  Secret consumers are currently only avaliable for the Barbican backend.
+  https://docs.openstack.org/barbican/latest/api/reference/secret_consumers.html
+
+
 Configuring castellan
 ~~~~~~~~~~~~~~~~~~~~~
 
 Castellan contains several options which control the key management
 service usage and the configuration of that service. It also contains
 functions to help configure the defaults and produce listings for use
 with the ``oslo-config-generator`` application.
```

### Comparing `castellan-4.1.0/releasenotes/notes/fix-vault-create-key-b4340a3067cbd93c.yaml` & `castellan-4.2.0/releasenotes/notes/fix-vault-create-key-b4340a3067cbd93c.yaml`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/releasenotes/notes/implements-keymanager-option-discovery-13a46c1dfc036a3f.yaml` & `castellan-4.2.0/releasenotes/notes/implements-keymanager-option-discovery-13a46c1dfc036a3f.yaml`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/releasenotes/source/conf.py` & `castellan-4.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/requirements.txt` & `castellan-4.2.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # The order of packages is significant, because pip processes them in the order
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
 
 pbr!=2.1.0,>=2.0.0 # Apache-2.0
 cryptography>=2.7 # BSD/Apache-2.0
-python-barbicanclient>=4.5.2 # Apache-2.0
+python-barbicanclient>=5.5.0 # Apache-2.0
 oslo.config>=6.4.0 # Apache-2.0
 oslo.context>=2.19.2 # Apache-2.0
 oslo.i18n>=3.15.3 # Apache-2.0
 oslo.log>=3.36.0 # Apache-2.0
 oslo.utils>=3.33.0 # Apache-2.0
 stevedore>=1.20.0 # Apache-2.0
 keystoneauth1>=3.4.0 # Apache-2.0
```

### Comparing `castellan-4.1.0/setup.cfg` & `castellan-4.2.0/setup.cfg`

 * *Files 9% similar despite different names*

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
 	castellan
```

### Comparing `castellan-4.1.0/setup.py` & `castellan-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/test-requirements.txt` & `castellan-4.2.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/tools/setup-vault-env.sh` & `castellan-4.2.0/tools/setup-vault-env.sh`

 * *Files identical despite different names*

### Comparing `castellan-4.1.0/tox.ini` & `castellan-4.2.0/tox.ini`

 * *Files identical despite different names*

