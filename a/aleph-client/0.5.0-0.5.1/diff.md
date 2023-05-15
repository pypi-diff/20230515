# Comparing `tmp/aleph-client-0.5.0.tar.gz` & `tmp/aleph-client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-client-0.5.0.tar", last modified: Thu Oct  6 19:46:33 2022, max compression
+gzip compressed data, was "aleph-client-0.5.1.tar", last modified: Mon May 15 15:48:41 2023, max compression
```

## Comparing `aleph-client-0.5.0.tar` & `aleph-client-0.5.1.tar`

### file list

```diff
@@ -1,114 +1,122 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.767482 aleph-client-0.5.0/
--rw-r--r--   0 user      (1000) user      (1000)      595 2022-03-08 15:17:02.000000 aleph-client-0.5.0/.coveragerc
--rw-r--r--   0 user      (1000) user      (1000)       54 2022-10-06 18:52:45.000000 aleph-client-0.5.0/.dockerignore
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.744148 aleph-client-0.5.0/.github/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.747482 aleph-client-0.5.0/.github/workflows/
--rw-r--r--   0 user      (1000) user      (1000)     1079 2022-10-06 09:50:23.000000 aleph-client-0.5.0/.github/workflows/test-build.yml
--rw-r--r--   0 user      (1000) user      (1000)     1562 2022-08-01 12:41:10.000000 aleph-client-0.5.0/.github/workflows/test-pytest.yml
--rw-r--r--   0 user      (1000) user      (1000)      537 2022-08-18 10:38:10.000000 aleph-client-0.5.0/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)      159 2022-03-08 15:17:02.000000 aleph-client-0.5.0/AUTHORS.rst
--rw-r--r--   0 user      (1000) user      (1000)       82 2022-03-08 15:17:02.000000 aleph-client-0.5.0/CHANGELOG.rst
--rw-r--r--   0 user      (1000) user      (1000)     1083 2022-03-08 15:17:02.000000 aleph-client-0.5.0/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)     2262 2022-10-06 19:46:33.767482 aleph-client-0.5.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1558 2022-08-11 15:36:50.000000 aleph-client-0.5.0/README.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.747482 aleph-client-0.5.0/docker/
--rw-r--r--   0 user      (1000) user      (1000)     1130 2022-10-06 19:36:53.000000 aleph-client-0.5.0/docker/Dockerfile
--rw-r--r--   0 user      (1000) user      (1000)      879 2022-10-06 09:50:23.000000 aleph-client-0.5.0/docker/with-ipfs.dockerfile
--rwxr-xr-x   0 user      (1000) user      (1000)      346 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docker/with-ipfs.entrypoint.sh
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.750815 aleph-client-0.5.0/docs/
--rw-r--r--   0 user      (1000) user      (1000)     7618 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/Makefile
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.750815 aleph-client-0.5.0/docs/_static/
--rw-r--r--   0 user      (1000) user      (1000)       18 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/_static/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)     2774 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/_static/logo.svg
--rw-r--r--   0 user      (1000) user      (1000)       41 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/authors.rst
--rw-r--r--   0 user      (1000) user      (1000)       43 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/changelog.rst
--rw-r--r--   0 user      (1000) user      (1000)     9733 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/conf.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.750815 aleph-client-0.5.0/docs/content/
--rw-r--r--   0 user      (1000) user      (1000)     3241 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/content/account.rst
--rw-r--r--   0 user      (1000) user      (1000)     2347 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/content/aggregates.rst
--rw-r--r--   0 user      (1000) user      (1000)     1543 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/content/async_notes.rst
--rw-r--r--   0 user      (1000) user      (1000)     1924 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/content/cli.rst
--rw-r--r--   0 user      (1000) user      (1000)     2604 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/content/introduction.rst
--rw-r--r--   0 user      (1000) user      (1000)     1402 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/content/posts.rst
--rw-r--r--   0 user      (1000) user      (1000)     1159 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/content/programs.rst
--rw-r--r--   0 user      (1000) user      (1000)     1474 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/index.rst
--rw-r--r--   0 user      (1000) user      (1000)       67 2022-03-08 15:17:02.000000 aleph-client-0.5.0/docs/license.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.754148 aleph-client-0.5.0/examples/
--rw-r--r--   0 user      (1000) user      (1000)     2138 2022-03-08 15:17:02.000000 aleph-client-0.5.0/examples/httpgateway.py
--rw-r--r--   0 user      (1000) user      (1000)     1697 2022-03-08 15:17:02.000000 aleph-client-0.5.0/examples/metrics.py
--rw-r--r--   0 user      (1000) user      (1000)     4044 2022-03-08 15:17:02.000000 aleph-client-0.5.0/examples/mqtt.py
--rw-r--r--   0 user      (1000) user      (1000)     2979 2022-03-08 15:17:02.000000 aleph-client-0.5.0/examples/store.py
--rw-r--r--   0 user      (1000) user      (1000)      664 2022-08-23 10:09:56.000000 aleph-client-0.5.0/requirements.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.754148 aleph-client-0.5.0/scripts/
--rw-r--r--   0 user      (1000) user      (1000)      310 2022-08-01 12:41:10.000000 aleph-client-0.5.0/scripts/build-and-shell.sh
--rw-r--r--   0 user      (1000) user      (1000)      437 2022-08-01 12:41:10.000000 aleph-client-0.5.0/scripts/build-and-test.sh
--rw-r--r--   0 user      (1000) user      (1000)      392 2022-10-06 19:36:53.000000 aleph-client-0.5.0/scripts/build-to-publish.sh
--rw-r--r--   0 user      (1000) user      (1000)     1735 2022-10-06 19:46:33.767482 aleph-client-0.5.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      576 2022-03-08 15:17:02.000000 aleph-client-0.5.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.744148 aleph-client-0.5.0/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.757482 aleph-client-0.5.0/src/aleph_client/
--rw-r--r--   0 user      (1000) user      (1000)      345 2022-03-08 15:17:02.000000 aleph-client-0.5.0/src/aleph_client/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    17802 2022-10-06 18:24:39.000000 aleph-client-0.5.0/src/aleph_client/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     2234 2022-10-06 13:04:56.000000 aleph-client-0.5.0/src/aleph_client/account.py
--rw-r--r--   0 user      (1000) user      (1000)    24282 2022-10-06 18:24:39.000000 aleph-client-0.5.0/src/aleph_client/asynchronous.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.760815 aleph-client-0.5.0/src/aleph_client/chains/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-03-08 15:17:02.000000 aleph-client-0.5.0/src/aleph_client/chains/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2473 2022-10-06 09:50:23.000000 aleph-client-0.5.0/src/aleph_client/chains/common.py
--rw-r--r--   0 user      (1000) user      (1000)     2355 2022-10-06 09:58:52.000000 aleph-client-0.5.0/src/aleph_client/chains/cosmos.py
--rw-r--r--   0 user      (1000) user      (1000)     1165 2022-10-06 09:50:23.000000 aleph-client-0.5.0/src/aleph_client/chains/ethereum.py
--rw-r--r--   0 user      (1000) user      (1000)    10170 2022-08-11 15:31:14.000000 aleph-client-0.5.0/src/aleph_client/chains/nuls1.py
--rw-r--r--   0 user      (1000) user      (1000)     1713 2022-08-11 15:31:14.000000 aleph-client-0.5.0/src/aleph_client/chains/nuls2.py
--rw-r--r--   0 user      (1000) user      (1000)     2311 2022-10-06 09:50:23.000000 aleph-client-0.5.0/src/aleph_client/chains/remote.py
--rw-r--r--   0 user      (1000) user      (1000)     1989 2022-10-06 09:50:23.000000 aleph-client-0.5.0/src/aleph_client/chains/sol.py
--rw-r--r--   0 user      (1000) user      (1000)     1328 2022-10-06 09:58:52.000000 aleph-client-0.5.0/src/aleph_client/chains/substrate.py
--rw-r--r--   0 user      (1000) user      (1000)     1518 2022-10-06 09:50:23.000000 aleph-client-0.5.0/src/aleph_client/chains/tezos.py
--rw-r--r--   0 user      (1000) user      (1000)     1309 2022-10-06 09:50:23.000000 aleph-client-0.5.0/src/aleph_client/conf.py
--rw-r--r--   0 user      (1000) user      (1000)      357 2022-10-06 09:50:23.000000 aleph-client-0.5.0/src/aleph_client/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)      295 2022-08-01 13:41:44.000000 aleph-client-0.5.0/src/aleph_client/main.py
--rw-r--r--   0 user      (1000) user      (1000)      354 2022-10-06 18:24:39.000000 aleph-client-0.5.0/src/aleph_client/models.py
--rw-r--r--   0 user      (1000) user      (1000)     3831 2022-10-06 18:24:39.000000 aleph-client-0.5.0/src/aleph_client/synchronous.py
--rw-r--r--   0 user      (1000) user      (1000)      875 2022-10-06 09:50:23.000000 aleph-client-0.5.0/src/aleph_client/types.py
--rw-r--r--   0 user      (1000) user      (1000)     2178 2022-10-06 09:50:23.000000 aleph-client-0.5.0/src/aleph_client/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.760815 aleph-client-0.5.0/src/aleph_client/vm/
--rw-r--r--   0 user      (1000) user      (1000)       70 2022-03-08 15:17:02.000000 aleph-client-0.5.0/src/aleph_client/vm/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2339 2022-08-11 15:31:14.000000 aleph-client-0.5.0/src/aleph_client/vm/app.py
--rw-r--r--   0 user      (1000) user      (1000)     1997 2022-08-11 15:31:14.000000 aleph-client-0.5.0/src/aleph_client/vm/cache.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.757482 aleph-client-0.5.0/src/aleph_client.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2262 2022-10-06 19:46:33.000000 aleph-client-0.5.0/src/aleph_client.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2543 2022-10-06 19:46:33.000000 aleph-client-0.5.0/src/aleph_client.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-10-06 19:46:33.000000 aleph-client-0.5.0/src/aleph_client.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       53 2022-10-06 19:46:33.000000 aleph-client-0.5.0/src/aleph_client.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-03-09 08:44:06.000000 aleph-client-0.5.0/src/aleph_client.egg-info/not-zip-safe
--rw-r--r--   0 user      (1000) user      (1000)      447 2022-10-06 19:46:33.000000 aleph-client-0.5.0/src/aleph_client.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2022-10-06 19:46:33.000000 aleph-client-0.5.0/src/aleph_client.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.760815 aleph-client-0.5.0/tests/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.764148 aleph-client-0.5.0/tests/integration/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/integration/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      118 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/integration/config.py
--rw-r--r--   0 user      (1000) user      (1000)      583 2022-10-06 09:50:23.000000 aleph-client-0.5.0/tests/integration/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)     2435 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/integration/itest_aggregates.py
--rw-r--r--   0 user      (1000) user      (1000)     4042 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/integration/itest_forget.py
--rw-r--r--   0 user      (1000) user      (1000)     1949 2022-10-06 09:50:23.000000 aleph-client-0.5.0/tests/integration/itest_posts.py
--rw-r--r--   0 user      (1000) user      (1000)       35 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/integration/pytest.ini
--rw-r--r--   0 user      (1000) user      (1000)      608 2022-10-06 09:50:23.000000 aleph-client-0.5.0/tests/integration/test_utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.764148 aleph-client-0.5.0/tests/test_app/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/test_app/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.767482 aleph-client-0.5.0/tests/unit/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/unit/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      233 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/unit/conftest.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:46:33.767482 aleph-client-0.5.0/tests/unit/test_app/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/unit/test_app/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      293 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/unit/test_app/main.py
--rw-r--r--   0 user      (1000) user      (1000)     5580 2022-10-06 17:28:19.000000 aleph-client-0.5.0/tests/unit/test_asynchronous.py
--rw-r--r--   0 user      (1000) user      (1000)     1461 2022-10-06 09:58:52.000000 aleph-client-0.5.0/tests/unit/test_asynchronous_get.py
--rw-r--r--   0 user      (1000) user      (1000)     1416 2022-10-06 09:58:52.000000 aleph-client-0.5.0/tests/unit/test_chain_ethereum.py
--rw-r--r--   0 user      (1000) user      (1000)     1351 2022-10-06 09:58:52.000000 aleph-client-0.5.0/tests/unit/test_chain_nuls1.py
--rw-r--r--   0 user      (1000) user      (1000)     4290 2022-10-06 09:58:52.000000 aleph-client-0.5.0/tests/unit/test_chain_nuls1_compat.py
--rw-r--r--   0 user      (1000) user      (1000)     2152 2022-10-06 09:58:52.000000 aleph-client-0.5.0/tests/unit/test_chain_solana.py
--rw-r--r--   0 user      (1000) user      (1000)     1461 2022-10-06 09:58:52.000000 aleph-client-0.5.0/tests/unit/test_chain_tezos.py
--rw-r--r--   0 user      (1000) user      (1000)      157 2022-10-06 09:58:52.000000 aleph-client-0.5.0/tests/unit/test_chains.py
--rw-r--r--   0 user      (1000) user      (1000)       88 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/unit/test_init.py
--rw-r--r--   0 user      (1000) user      (1000)     2170 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/unit/test_remote_account.py
--rw-r--r--   0 user      (1000) user      (1000)      599 2022-10-06 09:50:23.000000 aleph-client-0.5.0/tests/unit/test_utils.py
--rw-r--r--   0 user      (1000) user      (1000)      678 2022-03-08 15:17:02.000000 aleph-client-0.5.0/tests/unit/test_vm_app.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.058332 aleph-client-0.5.1/
+-rw-r--r--   0 user      (1000) user      (1000)      595 2023-01-10 17:17:10.000000 aleph-client-0.5.1/.coveragerc
+-rw-r--r--   0 user      (1000) user      (1000)       54 2023-01-10 17:17:10.000000 aleph-client-0.5.1/.dockerignore
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.054332 aleph-client-0.5.1/.github/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.054332 aleph-client-0.5.1/.github/workflows/
+-rw-r--r--   0 user      (1000) user      (1000)     1079 2023-05-15 15:37:42.000000 aleph-client-0.5.1/.github/workflows/test-build.yml
+-rw-r--r--   0 user      (1000) user      (1000)     1562 2023-05-15 15:37:42.000000 aleph-client-0.5.1/.github/workflows/test-pytest.yml
+-rw-r--r--   0 user      (1000) user      (1000)      537 2023-01-10 17:17:10.000000 aleph-client-0.5.1/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)      159 2023-01-10 17:17:10.000000 aleph-client-0.5.1/AUTHORS.rst
+-rw-r--r--   0 user      (1000) user      (1000)       82 2023-01-10 17:17:10.000000 aleph-client-0.5.1/CHANGELOG.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1083 2023-01-10 17:17:10.000000 aleph-client-0.5.1/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)     2262 2023-05-15 15:48:41.058332 aleph-client-0.5.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1558 2023-01-10 17:17:10.000000 aleph-client-0.5.1/README.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.055332 aleph-client-0.5.1/docker/
+-rw-r--r--   0 user      (1000) user      (1000)     1136 2023-05-15 15:48:34.000000 aleph-client-0.5.1/docker/Dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)      879 2023-05-11 13:32:41.000000 aleph-client-0.5.1/docker/with-ipfs.dockerfile
+-rwxr-xr-x   0 user      (1000) user      (1000)      346 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docker/with-ipfs.entrypoint.sh
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.055332 aleph-client-0.5.1/docs/
+-rw-r--r--   0 user      (1000) user      (1000)     7618 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/Makefile
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.055332 aleph-client-0.5.1/docs/_static/
+-rw-r--r--   0 user      (1000) user      (1000)       18 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/_static/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)     2774 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/_static/logo.svg
+-rw-r--r--   0 user      (1000) user      (1000)       41 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/authors.rst
+-rw-r--r--   0 user      (1000) user      (1000)       43 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/changelog.rst
+-rw-r--r--   0 user      (1000) user      (1000)     9733 2023-05-15 15:37:42.000000 aleph-client-0.5.1/docs/conf.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.055332 aleph-client-0.5.1/docs/content/
+-rw-r--r--   0 user      (1000) user      (1000)     3241 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/content/account.rst
+-rw-r--r--   0 user      (1000) user      (1000)     2347 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/content/aggregates.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1543 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/content/async_notes.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1924 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/content/cli.rst
+-rw-r--r--   0 user      (1000) user      (1000)     2604 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/content/introduction.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1402 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/content/posts.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1159 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/content/programs.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1474 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/index.rst
+-rw-r--r--   0 user      (1000) user      (1000)       67 2023-01-10 17:17:10.000000 aleph-client-0.5.1/docs/license.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.055332 aleph-client-0.5.1/examples/
+-rw-r--r--   0 user      (1000) user      (1000)     2138 2023-05-15 15:37:42.000000 aleph-client-0.5.1/examples/httpgateway.py
+-rw-r--r--   0 user      (1000) user      (1000)     1697 2023-05-15 15:37:42.000000 aleph-client-0.5.1/examples/metrics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4044 2023-05-15 15:37:42.000000 aleph-client-0.5.1/examples/mqtt.py
+-rw-r--r--   0 user      (1000) user      (1000)     2979 2023-05-15 15:37:42.000000 aleph-client-0.5.1/examples/store.py
+-rw-r--r--   0 user      (1000) user      (1000)      664 2023-05-15 15:37:42.000000 aleph-client-0.5.1/requirements.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.056332 aleph-client-0.5.1/scripts/
+-rw-r--r--   0 user      (1000) user      (1000)      310 2023-01-10 17:17:10.000000 aleph-client-0.5.1/scripts/build-and-shell.sh
+-rw-r--r--   0 user      (1000) user      (1000)      437 2023-01-10 17:17:10.000000 aleph-client-0.5.1/scripts/build-and-test.sh
+-rw-r--r--   0 user      (1000) user      (1000)      392 2023-01-10 17:17:10.000000 aleph-client-0.5.1/scripts/build-to-publish.sh
+-rw-r--r--   0 user      (1000) user      (1000)     1749 2023-05-15 15:48:41.059332 aleph-client-0.5.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      576 2023-05-15 15:37:42.000000 aleph-client-0.5.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.054332 aleph-client-0.5.1/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.056332 aleph-client-0.5.1/src/aleph_client/
+-rw-r--r--   0 user      (1000) user      (1000)      345 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1253 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2234 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/account.py
+-rw-r--r--   0 user      (1000) user      (1000)    24970 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/asynchronous.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.057332 aleph-client-0.5.1/src/aleph_client/chains/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2473 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/common.py
+-rw-r--r--   0 user      (1000) user      (1000)     2355 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/cosmos.py
+-rw-r--r--   0 user      (1000) user      (1000)     1165 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/ethereum.py
+-rw-r--r--   0 user      (1000) user      (1000)    10170 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/nuls1.py
+-rw-r--r--   0 user      (1000) user      (1000)     1713 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/nuls2.py
+-rw-r--r--   0 user      (1000) user      (1000)     2311 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/remote.py
+-rw-r--r--   0 user      (1000) user      (1000)     1989 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/sol.py
+-rw-r--r--   0 user      (1000) user      (1000)     1328 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/substrate.py
+-rw-r--r--   0 user      (1000) user      (1000)     1518 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/chains/tezos.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.057332 aleph-client-0.5.1/src/aleph_client/commands/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:20:17.000000 aleph-client-0.5.1/src/aleph_client/commands/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1551 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/commands/aggregate.py
+-rw-r--r--   0 user      (1000) user      (1000)     3437 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/commands/files.py
+-rw-r--r--   0 user      (1000) user      (1000)      315 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/commands/help_strings.py
+-rw-r--r--   0 user      (1000) user      (1000)     6357 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/commands/message.py
+-rw-r--r--   0 user      (1000) user      (1000)    11367 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/commands/program.py
+-rw-r--r--   0 user      (1000) user      (1000)     2708 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/commands/utils.py
+-rw-r--r--   0 user      (1000) user      (1000)     1309 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/conf.py
+-rw-r--r--   0 user      (1000) user      (1000)      357 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)      295 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/main.py
+-rw-r--r--   0 user      (1000) user      (1000)      354 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/models.py
+-rw-r--r--   0 user      (1000) user      (1000)     3930 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/synchronous.py
+-rw-r--r--   0 user      (1000) user      (1000)      875 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/types.py
+-rw-r--r--   0 user      (1000) user      (1000)     2178 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.057332 aleph-client-0.5.1/src/aleph_client/vm/
+-rw-r--r--   0 user      (1000) user      (1000)       70 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/vm/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2359 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/vm/app.py
+-rw-r--r--   0 user      (1000) user      (1000)     1997 2023-05-15 15:37:42.000000 aleph-client-0.5.1/src/aleph_client/vm/cache.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.056332 aleph-client-0.5.1/src/aleph_client.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2262 2023-05-15 15:48:41.000000 aleph-client-0.5.1/src/aleph_client.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2806 2023-05-15 15:48:41.000000 aleph-client-0.5.1/src/aleph_client.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-15 15:48:41.000000 aleph-client-0.5.1/src/aleph_client.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       53 2023-05-15 15:48:41.000000 aleph-client-0.5.1/src/aleph_client.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-01-12 11:43:23.000000 aleph-client-0.5.1/src/aleph_client.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1000) user      (1000)      460 2023-05-15 15:48:41.000000 aleph-client-0.5.1/src/aleph_client.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2023-05-15 15:48:41.000000 aleph-client-0.5.1/src/aleph_client.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.057332 aleph-client-0.5.1/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:30:54.000000 aleph-client-0.5.1/tests/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.057332 aleph-client-0.5.1/tests/integration/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-10 17:17:10.000000 aleph-client-0.5.1/tests/integration/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      118 2023-01-10 17:17:10.000000 aleph-client-0.5.1/tests/integration/config.py
+-rw-r--r--   0 user      (1000) user      (1000)      583 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/integration/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)     2435 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/integration/itest_aggregates.py
+-rw-r--r--   0 user      (1000) user      (1000)     4042 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/integration/itest_forget.py
+-rw-r--r--   0 user      (1000) user      (1000)     1949 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/integration/itest_posts.py
+-rw-r--r--   0 user      (1000) user      (1000)       35 2023-01-10 17:17:10.000000 aleph-client-0.5.1/tests/integration/pytest.ini
+-rw-r--r--   0 user      (1000) user      (1000)      608 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/integration/test_utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.058332 aleph-client-0.5.1/tests/test_app/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/test_app/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.058332 aleph-client-0.5.1/tests/unit/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:30:54.000000 aleph-client-0.5.1/tests/unit/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      233 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/conftest.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 15:48:41.058332 aleph-client-0.5.1/tests/unit/test_app/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-10 17:17:10.000000 aleph-client-0.5.1/tests/unit/test_app/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      293 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_app/main.py
+-rw-r--r--   0 user      (1000) user      (1000)     5578 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_asynchronous.py
+-rw-r--r--   0 user      (1000) user      (1000)     1527 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_asynchronous_get.py
+-rw-r--r--   0 user      (1000) user      (1000)     1416 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_chain_ethereum.py
+-rw-r--r--   0 user      (1000) user      (1000)     1351 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_chain_nuls1.py
+-rw-r--r--   0 user      (1000) user      (1000)     4290 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_chain_nuls1_compat.py
+-rw-r--r--   0 user      (1000) user      (1000)     2152 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_chain_solana.py
+-rw-r--r--   0 user      (1000) user      (1000)     1461 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_chain_tezos.py
+-rw-r--r--   0 user      (1000) user      (1000)      157 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_chains.py
+-rw-r--r--   0 user      (1000) user      (1000)       88 2023-01-10 17:17:10.000000 aleph-client-0.5.1/tests/unit/test_init.py
+-rw-r--r--   0 user      (1000) user      (1000)     2170 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_remote_account.py
+-rw-r--r--   0 user      (1000) user      (1000)      599 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)      678 2023-05-15 15:37:42.000000 aleph-client-0.5.1/tests/unit/test_vm_app.py
```

### Comparing `aleph-client-0.5.0/.coveragerc` & `aleph-client-0.5.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/.github/workflows/test-build.yml` & `aleph-client-0.5.1/.github/workflows/test-build.yml`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/.github/workflows/test-pytest.yml` & `aleph-client-0.5.1/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/.gitignore` & `aleph-client-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/LICENSE.txt` & `aleph-client-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/PKG-INFO` & `aleph-client-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: Lightweight Python Client library for the Aleph.im network
 Home-page: https://github.com/aleph-im/aleph-client
 Author: Aleph.im Team
 Author-email: hello@aleph.im
 License: mit
 Project-URL: Documentation, https://aleph.im/
 Platform: any
```

### Comparing `aleph-client-0.5.0/README.rst` & `aleph-client-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docker/Dockerfile` & `aleph-client-0.5.1/docker/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
 RUN pip install --upgrade 'aleph-message~=0.2.3' eth_account pynacl base58
-RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi requests
+RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-client/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-client
 
 RUN pip install -e .[testing,ethereum,solana]
```

### Comparing `aleph-client-0.5.0/docker/with-ipfs.dockerfile` & `aleph-client-0.5.1/docker/with-ipfs.dockerfile`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/Makefile` & `aleph-client-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/_static/logo.svg` & `aleph-client-0.5.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/conf.py` & `aleph-client-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/content/account.rst` & `aleph-client-0.5.1/docs/content/account.rst`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/content/aggregates.rst` & `aleph-client-0.5.1/docs/content/aggregates.rst`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/content/async_notes.rst` & `aleph-client-0.5.1/docs/content/async_notes.rst`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/content/cli.rst` & `aleph-client-0.5.1/docs/content/cli.rst`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/content/introduction.rst` & `aleph-client-0.5.1/docs/content/introduction.rst`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/content/posts.rst` & `aleph-client-0.5.1/docs/content/posts.rst`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/content/programs.rst` & `aleph-client-0.5.1/docs/content/programs.rst`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/docs/index.rst` & `aleph-client-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/examples/httpgateway.py` & `aleph-client-0.5.1/examples/httpgateway.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/examples/metrics.py` & `aleph-client-0.5.1/examples/metrics.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/examples/mqtt.py` & `aleph-client-0.5.1/examples/mqtt.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/examples/store.py` & `aleph-client-0.5.1/examples/store.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/requirements.txt` & `aleph-client-0.5.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/setup.cfg` & `aleph-client-0.5.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	coincurve
-	aiohttp>=3.8.0
+	aiohttp>=3.8.3
 	eciespy
 	typing_extensions
 	typer
 	aleph-message~=0.2.3
 	eth_account>=0.4.0
 	python-magic
 
@@ -42,26 +42,27 @@
 	pytest-cov
 	pytest-asyncio
 	mypy
 	secp256k1
 	pynacl
 	base58
 	fastapi
+	httpx
 	requests
 	aleph-pytezos==0.1.0
 mqtt = 
 	aiomqtt
 	certifi
 	Click
 nuls2 = 
 	nuls2-python
 ethereum = 
 	eth_account>=0.4.0
 polkadot = 
-	substrate-interface
+	substrate-interface==1.3.4
 cosmos = 
 	cosmospy
 solana = 
 	pynacl
 	base58
 tezos = 
 	pynacl
```

### Comparing `aleph-client-0.5.0/setup.py` & `aleph-client-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/account.py` & `aleph-client-0.5.1/src/aleph_client/account.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/asynchronous.py` & `aleph-client-0.5.1/src/aleph_client/asynchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     StoreContent,
     PostMessage,
     Message,
     ForgetMessage,
     AlephMessage,
     AggregateMessage,
     StoreMessage,
-    ProgramMessage,
+    ProgramMessage, ItemType,
 )
 from pydantic import ValidationError
 
 from aleph_client.types import Account, StorageEnum, GenericMessage
 from .exceptions import MessageNotFoundError, MultipleMessagesError
 from .models import MessagesResponse
 from .utils import get_message_type_value
@@ -60,47 +60,47 @@
 
 def get_fallback_session() -> ClientSession:
     thread_id = threading.get_native_id()
     return _get_fallback_session(thread_id=thread_id)
 
 
 async def ipfs_push(
-    content,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        content,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> str:
     session = session or get_fallback_session()
 
     url = f"{api_server}/api/v0/ipfs/add_json"
     logger.debug(f"Pushing to IPFS on {url}")
 
     async with session.post(url, json=content) as resp:
         resp.raise_for_status()
         return (await resp.json()).get("hash")
 
 
 async def storage_push(
-    content,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        content,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> str:
     session = session or get_fallback_session()
 
     url = f"{api_server}/api/v0/storage/add_json"
     logger.debug(f"Pushing to storage on {url}")
 
     async with session.post(url, json=content) as resp:
         resp.raise_for_status()
         return (await resp.json()).get("hash")
 
 
 async def ipfs_push_file(
-    file_content,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        file_content,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> str:
     session = session or get_fallback_session()
 
     data = aiohttp.FormData()
     data.add_field("file", file_content)
 
     url = f"{api_server}/api/v0/ipfs/add_file"
@@ -108,17 +108,17 @@
 
     async with session.post(url, data=data) as resp:
         resp.raise_for_status()
         return (await resp.json()).get("hash")
 
 
 async def storage_push_file(
-    file_content,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        file_content,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> str:
     session = session or get_fallback_session()
 
     data = aiohttp.FormData()
     data.add_field("file", file_content)
 
     url = f"{api_server}/api/v0/storage/add_file"
@@ -126,27 +126,27 @@
 
     async with session.post(url, data=data) as resp:
         resp.raise_for_status()
         return (await resp.json()).get("hash")
 
 
 async def broadcast(
-    message,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        message,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> None:
     """Broadcast a message on the Aleph network via pubsub for nodes to pick it up."""
     session = session or get_fallback_session()
 
     url = f"{api_server}/api/v0/ipfs/pubsub/pub"
     logger.debug(f"Posting message on {url}")
 
     async with session.post(
-        url,
-        json={"topic": "ALEPH-TEST", "data": json.dumps(message)},
+            url,
+            json={"topic": "ALEPH-TEST", "data": json.dumps(message)},
     ) as response:
         response.raise_for_status()
         result = await response.json()
         status = result.get("status")
         if status == "success":
             return
         elif status == "warning":
@@ -165,24 +165,24 @@
         else:
             raise ValueError(
                 f"Invalid response from server, status in missing or unknown: '{status}'"
             )
 
 
 async def create_post(
-    account: Account,
-    post_content,
-    post_type: str,
-    ref: Optional[str] = None,
-    address: Optional[str] = settings.ADDRESS_TO_USE,
-    channel: str = settings.DEFAULT_CHANNEL,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
-    inline: bool = True,
-    storage_engine: StorageEnum = StorageEnum.storage,
+        account: Account,
+        post_content,
+        post_type: str,
+        ref: Optional[str] = None,
+        address: Optional[str] = settings.ADDRESS_TO_USE,
+        channel: str = settings.DEFAULT_CHANNEL,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
+        inline: bool = True,
+        storage_engine: StorageEnum = StorageEnum.storage,
 ) -> PostMessage:
     address = address or account.get_address()
 
     content = PostContent(
         type=post_type,
         address=address,
         content=post_content,
@@ -199,22 +199,22 @@
         session=session,
         inline=inline,
         storage_engine=storage_engine,
     )
 
 
 async def create_aggregate(
-    account: Account,
-    key,
-    content,
-    address: Optional[str] = settings.ADDRESS_TO_USE,
-    channel: str = settings.DEFAULT_CHANNEL,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
-    inline: bool = True,
+        account: Account,
+        key,
+        content,
+        address: Optional[str] = settings.ADDRESS_TO_USE,
+        channel: str = settings.DEFAULT_CHANNEL,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
+        inline: bool = True,
 ) -> AggregateMessage:
     address = address or account.get_address()
 
     content_ = AggregateContent(
         key=key,
         address=address,
         content=content,
@@ -229,25 +229,25 @@
         api_server=api_server,
         session=session,
         inline=inline,
     )
 
 
 async def create_store(
-    account: Account,
-    address=settings.ADDRESS_TO_USE,
-    file_content: Optional[bytes] = None,
-    file_hash: Optional[str] = None,
-    guess_mime_type: bool = False,
-    ref: Optional[str] = None,
-    storage_engine=StorageEnum.storage,
-    extra_fields: Optional[dict] = None,
-    channel: str = settings.DEFAULT_CHANNEL,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        account: Account,
+        address=settings.ADDRESS_TO_USE,
+        file_content: Optional[bytes] = None,
+        file_hash: Optional[str] = None,
+        guess_mime_type: bool = False,
+        ref: Optional[str] = None,
+        storage_engine=StorageEnum.storage,
+        extra_fields: Optional[dict] = None,
+        channel: str = settings.DEFAULT_CHANNEL,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> StoreMessage:
     address = address or account.get_address()
     extra_fields = extra_fields or {}
 
     if file_hash is None:
         if file_content is None:
             raise ValueError("Please specify at least a file_content or a file_hash")
@@ -292,34 +292,33 @@
         api_server=api_server,
         session=session,
         inline=True,
     )
 
 
 async def create_program(
-    account: Account,
-    program_ref: str,
-    entrypoint: str,
-    runtime: str,
-    environment_variables: Optional[Dict[str, str]] = None,
-    storage_engine: StorageEnum = StorageEnum.storage,
-    channel: str = settings.DEFAULT_CHANNEL,
-    address: Optional[str] = settings.ADDRESS_TO_USE,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
-    memory: int = settings.DEFAULT_VM_MEMORY,
-    vcpus: int = settings.DEFAULT_VM_VCPUS,
-    timeout_seconds: float = settings.DEFAULT_VM_TIMEOUT,
-    persistent: bool = False,
-    encoding: Encoding = Encoding.zip,
-    volumes: List[Dict] = None,
-    subscriptions: Optional[List[Dict]] = None,
+        account: Account,
+        program_ref: str,
+        entrypoint: str,
+        runtime: str,
+        environment_variables: Optional[Dict[str, str]] = None,
+        storage_engine: StorageEnum = StorageEnum.storage,
+        channel: str = settings.DEFAULT_CHANNEL,
+        address: Optional[str] = settings.ADDRESS_TO_USE,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
+        memory: int = settings.DEFAULT_VM_MEMORY,
+        vcpus: int = settings.DEFAULT_VM_VCPUS,
+        timeout_seconds: float = settings.DEFAULT_VM_TIMEOUT,
+        persistent: bool = False,
+        encoding: Encoding = Encoding.zip,
+        volumes: Optional[List[Dict]] = None,
+        subscriptions: Optional[List[Dict]] = None,
 ) -> ProgramMessage:
     volumes = volumes if volumes is not None else []
-
     address = address or account.get_address()
 
     # TODO: Check that program_ref, runtime and data_ref exist
 
     ## Register the different ways to trigger a VM
     if subscriptions:
         # Trigger on HTTP calls and on Aleph message subscriptions.
@@ -386,22 +385,22 @@
         api_server=api_server,
         storage_engine=storage_engine,
         session=session,
     )
 
 
 async def forget(
-    account: Account,
-    hashes: List[str],
-    reason: Optional[str],
-    storage_engine: StorageEnum = StorageEnum.storage,
-    channel: str = settings.DEFAULT_CHANNEL,
-    address: Optional[str] = settings.ADDRESS_TO_USE,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        account: Account,
+        hashes: List[str],
+        reason: Optional[str],
+        storage_engine: StorageEnum = StorageEnum.storage,
+        channel: str = settings.DEFAULT_CHANNEL,
+        address: Optional[str] = settings.ADDRESS_TO_USE,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> ForgetMessage:
     address = address or account.get_address()
 
     content = ForgetContent(
         hashes=hashes,
         reason=reason,
         address=address,
@@ -417,120 +416,122 @@
         storage_engine=storage_engine,
         session=session,
         inline=True,
     )
 
 
 async def submit(
-    account: Account,
-    content: Dict,
-    message_type: MessageType,
-    channel: str = settings.DEFAULT_CHANNEL,
-    api_server: str = settings.API_HOST,
-    storage_engine: StorageEnum = StorageEnum.storage,
-    session: Optional[ClientSession] = None,
-    inline: bool = True,
+        account: Account,
+        content: Dict,
+        message_type: MessageType,
+        channel: str = settings.DEFAULT_CHANNEL,
+        api_server: str = settings.API_HOST,
+        storage_engine: StorageEnum = StorageEnum.storage,
+        session: Optional[ClientSession] = None,
+        inline: bool = True,
 ) -> AlephMessage:
     message: Dict[str, Any] = {
-        #'item_hash': ipfs_hash,
+        # 'item_hash': ipfs_hash,
         "chain": account.CHAIN,
         "channel": channel,
         "sender": account.get_address(),
         "type": message_type,
         "time": time.time(),
     }
 
     item_content: str = json.dumps(content, separators=(",", ":"))
 
     if inline and (len(item_content) < 50000):
         message["item_content"] = item_content
         h = hashlib.sha256()
         h.update(message["item_content"].encode("utf-8"))
         message["item_hash"] = h.hexdigest()
-        message["item_type"] = "inline"
+        message["item_type"] = ItemType.inline
     else:
         if storage_engine == StorageEnum.ipfs:
             message["item_hash"] = await ipfs_push(
                 content, session=session, api_server=api_server
             )
+            message["item_type"] = ItemType.ipfs
         else:  # storage
             assert storage_engine == StorageEnum.storage
             message["item_hash"] = await storage_push(
                 content, session=session, api_server=api_server
             )
+            message["item_type"] = ItemType.storage
 
     message = await account.sign_message(message)
     await broadcast(message, session=session, api_server=api_server)
 
     # let's add the content to the object so users can access it.
     message["content"] = content
 
     return Message(**message)
 
 
 async def fetch_aggregate(
-    address: str,
-    key: str,
-    limit: Optional[int] = 100,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        address: str,
+        key: str,
+        limit: Optional[int] = 100,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> Dict[str, Dict]:
     session = session or get_fallback_session()
 
     params: Dict[str, Any] = {"keys": key}
     if limit:
         params["limit"] = limit
 
     async with session.get(
-        f"{api_server}/api/v0/aggregates/{address}.json", params=params
+            f"{api_server}/api/v0/aggregates/{address}.json", params=params
     ) as resp:
         result = await resp.json()
         data = result.get("data", dict())
         return data.get(key)
 
 
 async def fetch_aggregates(
-    address: str,
-    keys: Optional[Iterable[str]] = None,
-    limit: Optional[int] = 100,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        address: str,
+        keys: Optional[Iterable[str]] = None,
+        limit: Optional[int] = 100,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> Dict[str, Dict]:
     session = session or get_fallback_session()
 
     keys_str = ",".join(keys) if keys else ""
     params: Dict[str, Any] = {}
     if keys_str:
         params["keys"] = keys_str
     if limit:
         params["limit"] = limit
 
     async with session.get(
-        f"{api_server}/api/v0/aggregates/{address}.json",
-        params=params,
+            f"{api_server}/api/v0/aggregates/{address}.json",
+            params=params,
     ) as resp:
         result = await resp.json()
         data = result.get("data", dict())
         return data
 
 
 async def get_posts(
-    pagination: int = 200,
-    page: int = 1,
-    types: Optional[Iterable[str]] = None,
-    refs: Optional[Iterable[str]] = None,
-    addresses: Optional[Iterable[str]] = None,
-    tags: Optional[Iterable[str]] = None,
-    hashes: Optional[Iterable[str]] = None,
-    channels: Optional[Iterable[str]] = None,
-    chains: Optional[Iterable[str]] = None,
-    start_date: Optional[Union[datetime, float]] = None,
-    end_date: Optional[Union[datetime, float]] = None,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        pagination: int = 200,
+        page: int = 1,
+        types: Optional[Iterable[str]] = None,
+        refs: Optional[Iterable[str]] = None,
+        addresses: Optional[Iterable[str]] = None,
+        tags: Optional[Iterable[str]] = None,
+        hashes: Optional[Iterable[str]] = None,
+        channels: Optional[Iterable[str]] = None,
+        chains: Optional[Iterable[str]] = None,
+        start_date: Optional[Union[datetime, float]] = None,
+        end_date: Optional[Union[datetime, float]] = None,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ):
     session = session or get_fallback_session()
 
     params: Dict[str, Any] = dict(pagination=pagination, page=page)
 
     if types is not None:
         params["types"] = ",".join(types)
@@ -558,31 +559,31 @@
 
     async with session.get(f"{api_server}/api/v0/posts.json", params=params) as resp:
         resp.raise_for_status()
         return await resp.json()
 
 
 async def get_messages(
-    pagination: int = 200,
-    page: int = 1,
-    message_type: Optional[MessageType] = None,
-    content_types: Optional[Iterable[str]] = None,
-    content_keys: Optional[Iterable[str]] = None,
-    refs: Optional[Iterable[str]] = None,
-    addresses: Optional[Iterable[str]] = None,
-    tags: Optional[Iterable[str]] = None,
-    hashes: Optional[Iterable[str]] = None,
-    channels: Optional[Iterable[str]] = None,
-    chains: Optional[Iterable[str]] = None,
-    start_date: Optional[Union[datetime, float]] = None,
-    end_date: Optional[Union[datetime, float]] = None,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
-    ignore_invalid_messages: bool = True,
-    invalid_messages_log_level: int = logging.NOTSET,
+        pagination: int = 200,
+        page: int = 1,
+        message_type: Optional[MessageType] = None,
+        content_types: Optional[Iterable[str]] = None,
+        content_keys: Optional[Iterable[str]] = None,
+        refs: Optional[Iterable[str]] = None,
+        addresses: Optional[Iterable[str]] = None,
+        tags: Optional[Iterable[str]] = None,
+        hashes: Optional[Iterable[str]] = None,
+        channels: Optional[Iterable[str]] = None,
+        chains: Optional[Iterable[str]] = None,
+        start_date: Optional[Union[datetime, float]] = None,
+        end_date: Optional[Union[datetime, float]] = None,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
+        ignore_invalid_messages: bool = True,
+        invalid_messages_log_level: int = logging.NOTSET,
 ) -> MessagesResponse:
     session = session or get_fallback_session()
 
     params: Dict[str, Any] = dict(pagination=pagination, page=page)
 
     if message_type is not None:
         params["msgType"] = message_type.value
@@ -643,19 +644,19 @@
             pagination_total=response_json["pagination_total"],
             pagination_per_page=response_json["pagination_per_page"],
             pagination_item=response_json["pagination_item"],
         )
 
 
 async def get_message(
-    item_hash: str,
-    message_type: Optional[Type[GenericMessage]] = None,
-    channel: Optional[str] = None,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        item_hash: str,
+        message_type: Optional[Type[GenericMessage]] = None,
+        channel: Optional[str] = None,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> GenericMessage:
     """Get a single message from its `item_hash`."""
     messages_response = await get_messages(
         hashes=[item_hash],
         session=session,
         channels=[channel] if channel else None,
         api_server=api_server,
@@ -674,26 +675,26 @@
                 f"The message type '{message.type}' "
                 f"does not match the expected type '{expected_type}'"
             )
     return message
 
 
 async def watch_messages(
-    message_type: Optional[MessageType] = None,
-    content_types: Optional[Iterable[str]] = None,
-    refs: Optional[Iterable[str]] = None,
-    addresses: Optional[Iterable[str]] = None,
-    tags: Optional[Iterable[str]] = None,
-    hashes: Optional[Iterable[str]] = None,
-    channels: Optional[Iterable[str]] = None,
-    chains: Optional[Iterable[str]] = None,
-    start_date: Optional[Union[datetime, float]] = None,
-    end_date: Optional[Union[datetime, float]] = None,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        message_type: Optional[MessageType] = None,
+        content_types: Optional[Iterable[str]] = None,
+        refs: Optional[Iterable[str]] = None,
+        addresses: Optional[Iterable[str]] = None,
+        tags: Optional[Iterable[str]] = None,
+        hashes: Optional[Iterable[str]] = None,
+        channels: Optional[Iterable[str]] = None,
+        chains: Optional[Iterable[str]] = None,
+        start_date: Optional[Union[datetime, float]] = None,
+        end_date: Optional[Union[datetime, float]] = None,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> AsyncIterable[AlephMessage]:
     """
     Iterate over current and future matching messages asynchronously.
     """
 
     session = session or get_fallback_session()
 
@@ -722,15 +723,15 @@
         params["startDate"] = start_date
     if end_date is not None:
         if not isinstance(end_date, float) and hasattr(start_date, "timestamp"):
             end_date = end_date.timestamp()
         params["endDate"] = end_date
 
     async with session.ws_connect(
-        f"{api_server}/api/ws0/messages", params=params
+            f"{api_server}/api/ws0/messages", params=params
     ) as ws:
         logger.debug("Websocket connected")
         async for msg in ws:
             if msg.type == aiohttp.WSMsgType.TEXT:
                 if msg.data == "close cmd":
                     await ws.close()
                     break
```

### Comparing `aleph-client-0.5.0/src/aleph_client/chains/common.py` & `aleph-client-0.5.1/src/aleph_client/chains/common.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/chains/cosmos.py` & `aleph-client-0.5.1/src/aleph_client/chains/cosmos.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/chains/ethereum.py` & `aleph-client-0.5.1/src/aleph_client/chains/ethereum.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/chains/nuls1.py` & `aleph-client-0.5.1/src/aleph_client/chains/nuls1.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/chains/nuls2.py` & `aleph-client-0.5.1/src/aleph_client/chains/nuls2.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/chains/remote.py` & `aleph-client-0.5.1/src/aleph_client/chains/remote.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/chains/sol.py` & `aleph-client-0.5.1/src/aleph_client/chains/sol.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/chains/substrate.py` & `aleph-client-0.5.1/src/aleph_client/chains/substrate.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/chains/tezos.py` & `aleph-client-0.5.1/src/aleph_client/chains/tezos.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/conf.py` & `aleph-client-0.5.1/src/aleph_client/conf.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/synchronous.py` & `aleph-client-0.5.1/src/aleph_client/synchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,47 +42,48 @@
 fetch_aggregate = wrap_async(asynchronous.fetch_aggregate)
 fetch_aggregates = wrap_async(asynchronous.fetch_aggregates)
 get_posts = wrap_async(asynchronous.get_posts)
 get_messages = wrap_async(asynchronous.get_messages)
 
 
 def get_message(
-    item_hash: str,
-    message_type: Optional[Type[GenericMessage]] = None,
-    channel: Optional[str] = None,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
+        item_hash: str,
+        message_type: Optional[Type[GenericMessage]] = None,
+        channel: Optional[str] = None,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
 ) -> GenericMessage:
     return wrap_async(asynchronous.get_message)(
         item_hash=item_hash,
         message_type=message_type,
         channel=channel,
         session=session,
         api_server=api_server,
     )
 
 
 def create_program(
-    account: Account,
-    program_ref: str,
-    entrypoint: str,
-    runtime: str,
-    environment_variables: Optional[Dict[str, str]] = None,
-    storage_engine: StorageEnum = StorageEnum.storage,
-    channel: str = settings.DEFAULT_CHANNEL,
-    address: Optional[str] = settings.ADDRESS_TO_USE,
-    session: Optional[ClientSession] = None,
-    api_server: str = settings.API_HOST,
-    memory: int = settings.DEFAULT_VM_MEMORY,
-    vcpus: int = settings.DEFAULT_VM_VCPUS,
-    timeout_seconds: float = settings.DEFAULT_VM_TIMEOUT,
-    persistent: bool = False,
-    encoding: Encoding = Encoding.zip,
-    volumes: List[Dict] = None,
-    subscriptions: Optional[List[Dict]] = None,
+        account: Account,
+        program_ref: str,
+        entrypoint: str,
+        runtime: str,
+        environment_variables: Optional[Dict[str, str]] = None,
+        storage_engine: StorageEnum = StorageEnum.storage,
+        channel: str = settings.DEFAULT_CHANNEL,
+        address: Optional[str] = settings.ADDRESS_TO_USE,
+        session: Optional[ClientSession] = None,
+        api_server: str = settings.API_HOST,
+        memory: int = settings.DEFAULT_VM_MEMORY,
+        vcpus: int = settings.DEFAULT_VM_VCPUS,
+        timeout_seconds: float = settings.DEFAULT_VM_TIMEOUT,
+        persistent: bool = False,
+        encoding: Encoding = Encoding.zip,
+        volumes: Optional[List[Dict]] = None,
+
+        subscriptions: Optional[List[Dict]] = None,
 ):
     return wrap_async(asynchronous.create_program)(
         account=account,
         program_ref=program_ref,
         entrypoint=entrypoint,
         environment_variables=environment_variables,
         runtime=runtime,
```

### Comparing `aleph-client-0.5.0/src/aleph_client/types.py` & `aleph-client-0.5.1/src/aleph_client/types.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/utils.py` & `aleph-client-0.5.1/src/aleph_client/utils.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client/vm/app.py` & `aleph-client-0.5.1/src/aleph_client/vm/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             return func
 
         return inner
 
     async def __call__(
         self,
         scope: Dict,
-        receive: Awaitable = None,
-        send: Callable[[Dict], Awaitable] = None,
+        receive: Optional[Awaitable] = None,
+        send: Optional[Callable[[Dict], Awaitable]] = None,
     ):
         if scope["type"] in ("http", "websocket"):
             if self.http_app:
                 await self.http_app(scope=scope, receive=receive, send=send)
             else:
                 raise ValueError("No HTTP app registered")
         elif scope["type"] == "aleph.message":
```

### Comparing `aleph-client-0.5.0/src/aleph_client/vm/cache.py` & `aleph-client-0.5.1/src/aleph_client/vm/cache.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/src/aleph_client.egg-info/PKG-INFO` & `aleph-client-0.5.1/src/aleph_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: Lightweight Python Client library for the Aleph.im network
 Home-page: https://github.com/aleph-im/aleph-client
 Author: Aleph.im Team
 Author-email: hello@aleph.im
 License: mit
 Project-URL: Documentation, https://aleph.im/
 Platform: any
```

### Comparing `aleph-client-0.5.0/src/aleph_client.egg-info/SOURCES.txt` & `aleph-client-0.5.1/src/aleph_client.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -59,14 +59,21 @@
 src/aleph_client/chains/ethereum.py
 src/aleph_client/chains/nuls1.py
 src/aleph_client/chains/nuls2.py
 src/aleph_client/chains/remote.py
 src/aleph_client/chains/sol.py
 src/aleph_client/chains/substrate.py
 src/aleph_client/chains/tezos.py
+src/aleph_client/commands/__init__.py
+src/aleph_client/commands/aggregate.py
+src/aleph_client/commands/files.py
+src/aleph_client/commands/help_strings.py
+src/aleph_client/commands/message.py
+src/aleph_client/commands/program.py
+src/aleph_client/commands/utils.py
 src/aleph_client/vm/__init__.py
 src/aleph_client/vm/app.py
 src/aleph_client/vm/cache.py
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/config.py
 tests/integration/conftest.py
```

### Comparing `aleph-client-0.5.0/tests/integration/conftest.py` & `aleph-client-0.5.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/integration/itest_aggregates.py` & `aleph-client-0.5.1/tests/integration/itest_aggregates.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/integration/itest_forget.py` & `aleph-client-0.5.1/tests/integration/itest_forget.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/integration/itest_posts.py` & `aleph-client-0.5.1/tests/integration/itest_posts.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/integration/test_utils.py` & `aleph-client-0.5.1/tests/integration/test_utils.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/unit/test_asynchronous.py` & `aleph-client-0.5.1/tests/unit/test_asynchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,26 @@
     PostMessage,
     AggregateMessage,
     StoreMessage,
     ProgramMessage,
     ForgetMessage,
 )
 
-from aleph_client.conf import settings
-from aleph_client.types import StorageEnum
-
 from aleph_client.asynchronous import (
     create_post,
     _get_fallback_session,
     create_aggregate,
     create_store,
     create_program,
     forget,
 )
 from aleph_client.chains.common import get_fallback_private_key
 from aleph_client.chains.ethereum import ETHAccount
+from aleph_client.conf import settings
+from aleph_client.types import StorageEnum
 
 
 def new_mock_session_with_post_success():
     mock_response = AsyncMock()
     mock_response.json.return_value = {"status": "success"}
 
     mock_post = AsyncMock()
@@ -111,15 +110,14 @@
 
     mock_session = new_mock_session_with_post_success()
 
     mock_ipfs_push_file = AsyncMock()
     mock_ipfs_push_file.return_value = "QmRTV3h1jLcACW4FRfdisokkQAk4E4qDhUzGpgdrd4JAFy"
 
     with patch("aleph_client.asynchronous.ipfs_push_file", mock_ipfs_push_file):
-
         await create_store(
             account=account,
             file_content=b"HELLO",
             # file_hash="abcde",
             channel="TEST",
             storage_engine=StorageEnum.ipfs,
             session=mock_session,
@@ -136,15 +134,14 @@
             api_server="https://example.org",
         )
 
     mock_storage_push_file = AsyncMock()
     mock_storage_push_file.return_value = "QmRTV3h1jLcACW4FRfdisokkQAk4E4qDhUzGpgdrd4JAFy"
 
     with patch("aleph_client.asynchronous.storage_push_file", mock_storage_push_file):
-
         new_post = await create_store(
             account=account,
             file_content=b"HELLO",
             channel="TEST",
             storage_engine=StorageEnum.storage,
             session=mock_session,
             api_server="https://example.org",
@@ -199,7 +196,8 @@
         channel="TEST",
         session=mock_session,
         api_server="https://example.org",
     )
 
     assert mock_session.post.called
     assert isinstance(new_post, ForgetMessage)
+
```

### Comparing `aleph-client-0.5.0/tests/unit/test_asynchronous_get.py` & `aleph-client-0.5.1/tests/unit/test_asynchronous_get.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 from aleph_message.models import MessageType, MessagesResponse
+import unittest
 
 from aleph_client.asynchronous import (
     get_messages,
     fetch_aggregates,
     fetch_aggregate,
     _get_fallback_session,
 )
@@ -53,7 +54,11 @@
         pagination=2,
     )
 
     messages = response.messages
     assert len(messages) > 1
     assert messages[0].type
     assert messages[0].sender
+
+
+if __name__ == '__main __':
+    unittest.main()
```

### Comparing `aleph-client-0.5.0/tests/unit/test_chain_ethereum.py` & `aleph-client-0.5.1/tests/unit/test_chain_ethereum.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/unit/test_chain_nuls1.py` & `aleph-client-0.5.1/tests/unit/test_chain_nuls1.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/unit/test_chain_nuls1_compat.py` & `aleph-client-0.5.1/tests/unit/test_chain_nuls1_compat.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/unit/test_chain_solana.py` & `aleph-client-0.5.1/tests/unit/test_chain_solana.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/unit/test_chain_tezos.py` & `aleph-client-0.5.1/tests/unit/test_chain_tezos.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/unit/test_remote_account.py` & `aleph-client-0.5.1/tests/unit/test_remote_account.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/unit/test_utils.py` & `aleph-client-0.5.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `aleph-client-0.5.0/tests/unit/test_vm_app.py` & `aleph-client-0.5.1/tests/unit/test_vm_app.py`

 * *Files identical despite different names*

