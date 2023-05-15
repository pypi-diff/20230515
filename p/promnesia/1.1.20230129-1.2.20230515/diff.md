# Comparing `tmp/promnesia-1.1.20230129.tar.gz` & `tmp/promnesia-1.2.20230515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promnesia-1.1.20230129.tar", last modified: Mon Jan 30 00:00:17 2023, max compression
+gzip compressed data, was "promnesia-1.2.20230515.tar", last modified: Mon May 15 20:09:06 2023, max compression
```

## Comparing `promnesia-1.1.20230129.tar` & `promnesia-1.2.20230515.tar`

### file list

```diff
@@ -1,228 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.873986 promnesia-1.1.20230129/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/.ci/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.ci/end2end_tests.Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/.ci/fake-systemd/
--rwxr-xr-x   0 runner    (1001) docker     (123)      847 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.ci/fake-systemd/systemctl
--rwxr-xr-x   0 runner    (1001) docker     (123)      727 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.ci/github-ci-compat
--rwxr-xr-x   0 runner    (1001) docker     (123)     2090 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.ci/release
--rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.ci/run
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.849986 promnesia-1.1.20230129/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/CHANGELOG.org
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24818 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/README.org
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/ci/
--rwxr-xr-x   0 runner    (1001) docker     (123)      160 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/ci/run-github-locally
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.857986 promnesia-1.1.20230129/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/doc/DEVELOPMENT.org
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/doc/GUIDE.org
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/doc/PRIVACY.org
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/doc/SOURCES.org
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/doc/TROUBLESHOOTING.org
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/doc/addons-mozilla-org.org
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/doc/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.857986 promnesia-1.1.20230129/docker/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/docker/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.857986 promnesia-1.1.20230129/docker/docker_files/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/docker/docker_files/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/docker/docker_files/Dockerfile-indexer
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/docker/docker_files/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/docker/docker_files/indexer-config.py.example
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/docker/docker_files/indexer-entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/docker/get-some-data.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/docker/init.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/docker/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.857986 promnesia-1.1.20230129/extension/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.857986 promnesia-1.1.20230129/extension/.ci/
--rwxr-xr-x   0 runner    (1001) docker     (123)      279 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/.ci/build
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/.flowconfig
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/MANUAL-TESTS.org
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/TODO.org
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.857986 promnesia-1.1.20230129/extension/__mocks__/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/__mocks__/dom-form-serializer.js
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/babel.config.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     3688 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/build
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.857986 promnesia-1.1.20230129/extension/flow-typed/
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/flow-typed/webextension-polyfill.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.857986 promnesia-1.1.20230129/extension/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/images/generate
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/images/ic_blacklisted_48.png
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/images/ic_blue_48.png
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/images/ic_boring_48.png
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/images/ic_error.png
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/images/ic_not_visited_48.png
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/images/ic_relatives_48.png
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/images/ic_visited_48.png
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/images/source_48.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/jest.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.857986 promnesia-1.1.20230129/extension/old/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/old/patcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.861986 promnesia-1.1.20230129/extension/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    35592 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/background.js
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/common.js
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/display.js
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/filterlist.js
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/normalise.js
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/notifications.js
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/options.js
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/options_page.css
--rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/options_page.html
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/options_page.js
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/search.js
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/selenium_bridge.js
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/showvisited.css
--rw-r--r--   0 runner    (1001) docker     (123)    21487 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/showvisited.js
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/sidebar-outer.css
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/sidebar.js
--rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/sources.js
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/toastify.css
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/src/toastify.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.861986 promnesia-1.1.20230129/extension/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/tests/common.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/tests/defensify.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/tests/integration.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/tests/test.html
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/extension/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.861986 promnesia-1.1.20230129/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      547 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/scripts/backup-phone-history.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3609 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/scripts/browser_history.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/scripts/promnesia
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 00:00:17.873986 promnesia-1.1.20230129/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.861986 promnesia-1.1.20230129/src/promnesia/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24638 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/cannon.py
--rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4635 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/kjson.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5857 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.865986 promnesia-1.1.20230129/src/promnesia/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/misc/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/misc/config_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/misc/install_server.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/read_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.865986 promnesia-1.1.20230129/src/promnesia/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/auto_logseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/auto_obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/fbmessenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/filetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/guess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/hackernews.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/hpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/instapaper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/org.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/plaintext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/roamresearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/shellcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/smscalls.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/stackexchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/takeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/takeout_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/viber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/website.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/src/promnesia/sources/zulip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.865986 promnesia-1.1.20230129/src/promnesia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-30 00:00:17.000000 promnesia-1.1.20230129/src/promnesia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-01-30 00:00:17.000000 promnesia-1.1.20230129/src/promnesia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 00:00:17.000000 promnesia-1.1.20230129/src/promnesia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-30 00:00:17.000000 promnesia-1.1.20230129/src/promnesia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 00:00:17.000000 promnesia-1.1.20230129/src/promnesia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-30 00:00:17.000000 promnesia-1.1.20230129/src/promnesia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-30 00:00:17.000000 promnesia-1.1.20230129/src/promnesia.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/browser_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/cannon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/config_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1623 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/convert_screencast.py
--rw-r--r--   0 runner    (1001) docker     (123)    19225 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/demos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44687 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/end2end_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/indexer_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/install_and_run
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/server_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/test_auto_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/test_org_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/test_traverse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/auto/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/auto/orgs/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/auto/orgs/file.org
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/auto/orgs/file2.org
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/auto/orgs/file3.org
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/auto/orgs/file4.org
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/auto/pocket.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/custom/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/custom/file2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/tests/testdata/logseq-graph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/logseq-graph/logseq/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/logseq-graph/logseq/config.edn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/logseq-graph/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/logseq-graph/pages/Note.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/normalise/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/normalise/ff.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/obsidian-vault/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/obsidian-vault/.obsidian/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/obsidian-vault/.obsidian/app.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/obsidian-vault/Note.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/tests/testdata/takeout/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/tests/testdata/takeout/Takeout/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.853986 promnesia-1.1.20230129/tests/testdata/takeout/Takeout/My Activity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/takeout/Takeout/My Activity/Chrome/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/takeout/Takeout/My Activity/Chrome/MyActivity.html
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/takeout-20150518T000000Z.zip
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/traverse/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/traverse/ignoreme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/traverse/ignoreme2/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/traverse/ignoreme2/notrealignored.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/traverse/imhere.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 00:00:17.869986 promnesia-1.1.20230129/tests/testdata/traverse/imhere2/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/traverse/imhere2/real.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/testdata/weird.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tests/webdriver_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-01-29 23:59:45.000000 promnesia-1.1.20230129/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/.ci/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.ci/end2end_tests.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/.ci/fake-systemd/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      847 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.ci/fake-systemd/systemctl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      727 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.ci/github-ci-compat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2090 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.ci/release
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.ci/run
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.190185 promnesia-1.2.20230515/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/CHANGELOG.org
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/README.org
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      160 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/ci/run-github-locally
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/doc/DEVELOPMENT.org
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/doc/GUIDE.org
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/doc/PRIVACY.org
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/doc/SOURCES.org
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/doc/TROUBLESHOOTING.org
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/doc/addons-mozilla-org.org
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/doc/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/docker/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/docker/docker_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/docker/docker_files/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/docker/docker_files/Dockerfile-indexer
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/docker/docker_files/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/docker/docker_files/indexer-config.py.example
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/docker/docker_files/indexer-entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/docker/get-some-data.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/docker/init.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/docker/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.198185 promnesia-1.2.20230515/extension/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.198185 promnesia-1.2.20230515/extension/.ci/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      279 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/.ci/build
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/.flowconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/MANUAL-TESTS.org
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/TODO.org
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.198185 promnesia-1.2.20230515/extension/__mocks__/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/__mocks__/dom-form-serializer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/babel.config.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/build
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.198185 promnesia-1.2.20230515/extension/flow-typed/
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/flow-typed/webextension-polyfill.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.198185 promnesia-1.2.20230515/extension/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/images/generate
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/images/ic_blacklisted_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/images/ic_blue_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/images/ic_boring_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/images/ic_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/images/ic_not_visited_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/images/ic_relatives_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/images/ic_visited_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/images/source_48.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/jest.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.198185 promnesia-1.2.20230515/extension/old/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/old/patcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)   824354 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.202185 promnesia-1.2.20230515/extension/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36598 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/background.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/common.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/display.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/filterlist.js
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/normalise.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/notifications.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/options_page.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/options_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/options_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/selenium_bridge.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/showvisited.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/showvisited.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/sidebar-outer.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24755 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/sidebar.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/sources.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/toastify.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/src/toastify.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.202185 promnesia-1.2.20230515/extension/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/tests/common.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/tests/defensify.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/tests/integration.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/tests/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/extension/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.202185 promnesia-1.2.20230515/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      547 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/scripts/backup-phone-history.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3609 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/scripts/browser_history.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/scripts/promnesia
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.190185 promnesia-1.2.20230515/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.206185 promnesia-1.2.20230515/src/promnesia/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24638 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/cannon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4635 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/kjson.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5874 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.206185 promnesia-1.2.20230515/src/promnesia/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/misc/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/misc/config_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/misc/install_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/read_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.210185 promnesia-1.2.20230515/src/promnesia/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/auto_logseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/auto_obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/browser_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/fbmessenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/filetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/guess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/hackernews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/hpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/instapaper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/plaintext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/roamresearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/shellcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/smscalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/stackexchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/takeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/takeout_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/telegram_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/viber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/website.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sources/zulip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/src/promnesia/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.206185 promnesia-1.2.20230515/src/promnesia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 20:09:05.000000 promnesia-1.2.20230515/src/promnesia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-15 20:09:06.000000 promnesia-1.2.20230515/src/promnesia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:09:05.000000 promnesia-1.2.20230515/src/promnesia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 20:09:05.000000 promnesia-1.2.20230515/src/promnesia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:09:05.000000 promnesia-1.2.20230515/src/promnesia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-15 20:09:05.000000 promnesia-1.2.20230515/src/promnesia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 20:09:05.000000 promnesia-1.2.20230515/src/promnesia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.210185 promnesia-1.2.20230515/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/browser_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/cannon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/config_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1623 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/convert_screencast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19225 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/demos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47184 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/end2end_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/indexer_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/install_and_run
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/server_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/test_auto_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/test_org_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/test_traverse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.210185 promnesia-1.2.20230515/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.210185 promnesia-1.2.20230515/tests/testdata/auto/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.210185 promnesia-1.2.20230515/tests/testdata/auto/orgs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/auto/orgs/file.org
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/auto/orgs/file2.org
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/auto/orgs/file3.org
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/auto/orgs/file4.org
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/auto/pocket.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/custom/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/custom/file2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.190185 promnesia-1.2.20230515/tests/testdata/logseq-graph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/logseq-graph/logseq/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/logseq-graph/logseq/config.edn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/logseq-graph/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/logseq-graph/pages/Note.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/normalise/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/normalise/ff.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/obsidian-vault/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/obsidian-vault/.obsidian/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/obsidian-vault/.obsidian/app.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/obsidian-vault/Note.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.190185 promnesia-1.2.20230515/tests/testdata/takeout/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/tests/testdata/takeout/Takeout/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.194185 promnesia-1.2.20230515/tests/testdata/takeout/Takeout/My Activity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/takeout/Takeout/My Activity/Chrome/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/takeout/Takeout/My Activity/Chrome/MyActivity.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/takeout-20150518T000000Z.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/traverse/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/traverse/ignoreme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/traverse/ignoreme2/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/traverse/ignoreme2/notrealignored.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/traverse/imhere.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:09:06.214185 promnesia-1.2.20230515/tests/testdata/traverse/imhere2/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/traverse/imhere2/real.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/testdata/weird.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tests/webdriver_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-15 20:08:31.000000 promnesia-1.2.20230515/tox.ini
```

### Comparing `promnesia-1.1.20230129/.ci/fake-systemd/systemctl` & `promnesia-1.2.20230515/.ci/fake-systemd/systemctl`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/.ci/github-ci-compat` & `promnesia-1.2.20230515/.ci/github-ci-compat`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/.ci/release` & `promnesia-1.2.20230515/.ci/release`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/.ci/run` & `promnesia-1.2.20230515/.ci/run`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/.circleci/config.yml` & `promnesia-1.2.20230515/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/.dockerignore` & `promnesia-1.2.20230515/.dockerignore`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/.github/workflows/main.yml` & `promnesia-1.2.20230515/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -14,27 +14,23 @@
 jobs:
   build:
     strategy:
       # useful to quickly debug all versions, otherwise a bit wasteful
       # fail-fast: false
       matrix:
         platform: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
         exclude: [
-            # windows runners are pretty scarce, so let's only run one of them..
-            # also 3.7 on windows is a bit broken due to the WindowsPath bug
-            {platform: windows-latest, python-version: '3.7'},
+            # windows runners are pretty scarce, so let's only run lowest and highest python version
             {platform: windows-latest, python-version: '3.9'},
-            # 3.11 on windows has this bug, lxml setup fails
-            #https://bugs.launchpad.net/lxml/+bug/1977998
-            {platform: windows-latest, python-version: '3.11'},
+            {platform: windows-latest, python-version: '3.10'},
 
-            # perhaps no need to run all macos versions -- it's a bit too slow and ubuntu covers python quirks well
-            {platform: macos-latest  , python-version: '3.8' },
+            # same, macos is a bit too slow and ubuntu covers python quirks well
             {platform: macos-latest  , python-version: '3.9' },
+            {platform: macos-latest  , python-version: '3.10' },
         ]
 
     runs-on: ${{ matrix.platform }}
 
     #continue-on-error: ${{ matrix.platform == 'windows-latest' }}
 
     steps:
```

### Comparing `promnesia-1.1.20230129/.gitignore` & `promnesia-1.2.20230515/.gitignore`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/CHANGELOG.org` & `promnesia-1.2.20230515/CHANGELOG.org`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/LICENSE` & `promnesia-1.2.20230515/LICENSE`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/README.org` & `promnesia-1.2.20230515/README.org`

 * *Files 2% similar despite different names*

```diff
@@ -402,15 +402,15 @@
 See [[file:doc/GUIDE.org#FAQ]]
 
 * Support
 The best support for me would be if you contribute to this or my other projects. Code, ideas of feedback -- everything is appreciated.
 
 I don't need money, but I understand it's often easier to give away than time, so here are some of projects that I donate to:
 
-- [[https://orgmode.org/worg/donate.html][org-mode]]
+- [[https://liberapay.com/org-mode][org-mode]]
 - [[https://archive.org/donate][Internet Archive]]
 - [[https://web.hypothes.is/donate][Hypothes.is]]
 - [[https://github.com/hlissner/doom-emacs#contribute][Doom Emacs]]
 
 * More links
 - [[file:doc/TROUBLESHOOTING.org][Troubleshooting guide]]
 - [[file:doc/SOURCES.org][Documentation on the sources]]
```

### Comparing `promnesia-1.1.20230129/doc/DEVELOPMENT.org` & `promnesia-1.2.20230515/doc/DEVELOPMENT.org`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 * Build extension
 
    : cd extension
    : npm install # (if necessary)
    : ./build --firefox # you can also use --chrome
    :         --lint    # [optional], run webext linter
    :         --release # [optional], build in the release mode (with optimizations)
-   :         --publish # [optional], release to the Chrome Web Store/Mozilla addons
+   :         --publish listed # [optional], release to the Chrome Web Store/Mozilla addons
 
    You'll find the result in =dist/=. After that, you can load it in your browser and develop.
 
    - on Firefox, the temporary loaded extensions only persist until the browser restart. Chrome doesn't have that issue.
    - on Firefox for Android, web extensions on Android are mostly broken at the moment, see [[https://discourse.mozilla.org/t/add-on-support-in-new-firefox-for-android/53488][here]] (unless you're using [[https://blog.mozilla.org/addons/2020/09/29/expanded-extension-support-in-firefox-for-android-nightly][Firefox Nightly]])
 
 * Run end-to-end tests
```

### Comparing `promnesia-1.1.20230129/doc/GUIDE.org` & `promnesia-1.2.20230515/doc/GUIDE.org`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/doc/PRIVACY.org` & `promnesia-1.2.20230515/doc/PRIVACY.org`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/doc/SOURCES.org` & `promnesia-1.2.20230515/doc/SOURCES.org`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 This file is an overview of available sources along with descriptions and some guidance.
 
+See [[#instructions][instructions]] below for additional information.
+
 * Extra dependencies
 Some sources require additional dependencies, which you can install if needed.
 
 #+begin_src python :dir .. :exports output :results output drawer
 print('\n') # fix github org-mode issue with drawers
 
 import setup
 for (name, description), vals in setup.DEPS_SOURCES.items():
     # fuck org-ruby. promnesia[name] should be in quotes, but then it doesn't render as code. ugh.
     # https://github.com/wallyqs/org-ruby/issues/45
+    vals = [v.split('>')[0] for v in vals]
+    if len(vals) == 0:
+        continue
     print(f"- ~pip3 install --user promnesia[{name}]~")
     print(f'   ')
-    vals = [v.split('>')[0] for v in vals]
     print(f'   {description}: {", ".join(vals)}')
 #+end_src
 
 #+RESULTS:
 :results:
 
 
@@ -31,90 +35,87 @@
    dependencies for sources.html: beautifulsoup4, lxml
 - ~pip3 install --user promnesia[markdown]~
 
    dependencies for sources.markdown: mistletoe
 - ~pip3 install --user promnesia[org]~
 
    dependencies for sources.org: orgparse
-- ~pip3 install --user promnesia[telegram]~
-
-   dependencies for sources.telegram: dataset
 :end:
 
 Alternatively, you can just install all of them in bulk: ~pip3 install --user promnesia[all]~.
 
 
 * Sources
 
 These are included with the current Promnesia distribution:
 
-#+begin_src python :python "with_my python3" :dir ../src :exports output :results output drawer
+#+begin_src python :dir ../src :exports output :results output drawer
 print('\n') # fix github org-mode issue with drawers
 
+import ast
 from pathlib import Path
-import pkgutil
-import importlib
-import inspect
+import os
 
 indent = lambda s: ''.join('  ' + l for l in s.splitlines(keepends=True))
 
 git_root = Path('.').absolute().parent
 
-from promnesia.common import Results
+src = git_root / 'src'
 
-import promnesia.sources as pkg
-for importer, name, ispkg in sorted(pkgutil.walk_packages(
-        path=pkg.__path__,
-        prefix=pkg.__name__+'.'
-), key=lambda x: x[1]):
-    if name in {
-            # TODO damn, these modules need depednencies...
-            'promnesia.sources.browser',
-            'promnesia.sources.markdown',
-            'promnesia.sources.org',
-            'promnesia.sources.plaintext',
+for f in sorted((src / 'promnesia/sources').rglob('*.py')):
+    mp = f.relative_to(src)
+    module_name = str(mp.with_suffix('')).replace(os.sep, '.')
+    if module_name in {
+            'promnesia.sources.browser_old',  # deprecated
+            'promnesia.sources.takeout_legacy',  # deprecated
+            'promnesia.sources.guess',
+            'promnesia.sources.demo',
     }:
         continue
-    m = importlib.import_module(name)
-    public = [(k, v) for k, v in inspect.getmembers(m) if not k.startswith('_')]
-    indexers = [(k, v) for k, v in public if getattr(v, '__annotations__', {}).get('return') == Results]
-    assert len(indexers) > 0, name
-    for k, i in indexers:
-        # print(inspect.signature(i))
-        link = '../' + str(Path(m.__file__).relative_to(git_root))
-        print(f'- [[file:{link}][{name}]]')
-        d = m.__doc__
-        if d is not None:
-            print(indent(d))
+    a: ast.Module = ast.parse(f.read_text())
+    has_index = False
+    for x in a.body:
+        if isinstance(x, ast.FunctionDef) and x.name == 'index':
+            has_index = True
+    if not has_index:
+        continue
+    link = '../' + str(f.relative_to(git_root))
+    print(f'- [[file:{link}][{module_name}]]')
+    doc = ast.get_docstring(a, clean=False)
+    if doc is not None:
+        print(indent(doc))
 #+end_src
 
 #+RESULTS:
 :results:
 
 
 - [[file:../src/promnesia/sources/auto.py][promnesia.sources.auto]]
 
   - discovers files recursively
   - guesses the format (orgmode/markdown/json/etc) by the extension/MIME type
   - can index most of plaintext files, including source code!
   - autodetects Obsidian vault and adds `obsidian://` app protocol support [[file:../src/promnesia/sources/obsidian.py][promnesia.sources.obsidian]]
   - autodetects Logseq graph and adds `logseq://` app protocol support [[file:../src/promnesia/sources/logseq.py][promnesia.sources.logseq]]
-  
+
+- [[file:../src/promnesia/sources/browser.py][promnesia.sources.browser]]
+
+  Uses [[https://github.com/karlicoss/HPI][HPI]] for visits from web browsers.
+
 - [[file:../src/promnesia/sources/fbmessenger.py][promnesia.sources.fbmessenger]]
 
   Uses [[https://github.com/karlicoss/HPI][HPI]] for the messages data.
 
 - [[file:../src/promnesia/sources/github.py][promnesia.sources.github]]
 
   Uses [[https://github.com/karlicoss/HPI][HPI]] github module
 
-- [[file:../src/promnesia/sources/guess.py][promnesia.sources.guess]]
-- [[file:../src/promnesia/sources/html.py][promnesia.sources.html]]
+- [[file:../src/promnesia/sources/hackernews.py][promnesia.sources.hackernews]]
 
-  Extracts links from HTML files
+  Uses [[https://github.com/karlicoss/HPI][HPI]] dogsheep module to import HackerNews items.
 
 - [[file:../src/promnesia/sources/hypothesis.py][promnesia.sources.hypothesis]]
 
   Uses HPI [[https://github.com/karlicoss/HPI/blob/master/doc/MODULES.org#myhypothesis][hypothesis]] module
 
 - [[file:../src/promnesia/sources/instapaper.py][promnesia.sources.instapaper]]
 
@@ -129,53 +130,113 @@
   Uses HPI [[https://github.com/karlicoss/HPI/blob/master/doc/MODULES.org#myreddit][reddit]] module
 
 - [[file:../src/promnesia/sources/roamresearch.py][promnesia.sources.roamresearch]]
 
   Uses [[https://github.com/karlicoss/HPI][HPI]] for Roam Research data
 
 - [[file:../src/promnesia/sources/rss.py][promnesia.sources.rss]]
+
+  Uses [[https://github.com/karlicoss/HPI][HPI]] for RSS data.
+
 - [[file:../src/promnesia/sources/shellcmd.py][promnesia.sources.shellcmd]]
 
+  Greps out URLs from an arbitrary shell command results.
+
+- [[file:../src/promnesia/sources/signal.py][promnesia.sources.signal]]
+
+  Collects visits from Signal Desktop's encrypted SQLIite db(s).
+
 - [[file:../src/promnesia/sources/smscalls.py][promnesia.sources.smscalls]]
 
   Uses [[https://github.com/karlicoss/HPI][HPI]] smscalls module
 
+- [[file:../src/promnesia/sources/stackexchange.py][promnesia.sources.stackexchange]]
+
+  Uses [[https://github.com/karlicoss/HPI][HPI]] for Stackexchange data.
+
 - [[file:../src/promnesia/sources/takeout.py][promnesia.sources.takeout]]
 
   Uses HPI [[https://github.com/karlicoss/HPI/blob/master/doc/MODULES.org#mygoogletakeoutpaths][google.takeout]] module
 
 - [[file:../src/promnesia/sources/telegram.py][promnesia.sources.telegram]]
 
   Uses [[https://github.com/fabianonline/telegram_backup#readme][telegram_backup]] database for messages data
 
-- [[file:../src/promnesia/sources/viber.py][promnesia.sources.viber]]
-
-  Uses all local SQLite files found in your Viber Desktop configurations:
-  usually in =~/.ViberPC/**/viber.db= (one directory for each telephone number).
-
-- [[file:../src/promnesia/sources/signal.py][promnesia.sources.signal]]
-
-  When path(s) given, uses the SQLite inside Signal-Desktop's configuration directory
-  (see the sources for more parameters & location of the db-file for each platform)
-
 - [[file:../src/promnesia/sources/twitter.py][promnesia.sources.twitter]]
 
   Uses [[https://github.com/karlicoss/HPI][HPI]] for Twitter data.
 
 - [[file:../src/promnesia/sources/vcs.py][promnesia.sources.vcs]]
 
   Clones & indexes Git repositories (via sources.auto)
 
+- [[file:../src/promnesia/sources/viber.py][promnesia.sources.viber]]
+
+  Collects visits from Viber desktop app (e.g. `~/.ViberPC/XYZ123/viber.db`)
+
 - [[file:../src/promnesia/sources/website.py][promnesia.sources.website]]
 
   Clones a website with wget and indexes via sources.auto
 
+- [[file:../src/promnesia/sources/zulip.py][promnesia.sources.zulip]]
+
+  Uses [[https://github.com/karlicoss/HPI][HPI]] for Zulip data.
+
 :end:
 
+* Instructions
+** browser
 
+The browser source here uses [[https://github.com/karlicoss/HPI][HPI]], which uses
+[[https://github.com/seanbreckenridge/browserexport][browserexport]] to
+save/parse browser history. Since browsers remove old history after your
+history database has grown to a certain size, this saves the raw database files to
+a directory you specify. =browserexport= supports many browsers, including any
+Chromium/Firefox based browsers (e.g. Brave, Vivaldi, Waterfox). For more
+instructions on backing up databases, see
+[[https://github.com/seanbreckenridge/browserexport#usage][here]], but as
+a quickstart, after setting up =HPI=, run:
+#+BEGIN_SRC sh
+hpi module install my.browser.export
+#+END_SRC
+
+Then, to save your browser history, run a command like:
+#+BEGIN_SRC sh
+browserexport save -b firefox --to ~/data/browser_history
+browserexport save -b chrome --to ~/data/browser_history
+browserexport save -b safari --to ~/data/browser_history
+#+END_SRC
+
+This will save your browser history to a directory, which you can then point
+HPI at, in your
+[[https://github.com/karlicoss/HPI/blob/master/doc/MODULES.org#mybrowser][HPI
+config]]:
+#+BEGIN_SRC python
+class browser:
+    class export:
+        # path[s]/glob to your backed up browser history sqlite files
+        export_path: Paths = "~/data/browsing/*.sqlite"
+
+    class active_browser:
+        # paths to sqlite database files which you use actively
+        # to read from. For example:
+        # from browserexport.browsers.all import Firefox
+        # export_path = Firefox.locate_database()
+        export_path: Paths
+#+END_SRC
+
+Finally, you can add the browser source to =promnesia=, in your =config.py=:
+#+BEGIN_SRC python
+from promnesia.sources import browser
+
+SOURCES = [
+    browser,
+    ...
+]
+#+END_SRC
 * Extending
 Adding your own data sources is very easy!
 One day I'll add some proper documentation, but the easiest at the moment is to use existing simple modules as a reference, for example:
 
 - [[https://github.com/karlicoss/promnesia/blob/master/src/promnesia/sources/pocket.py][pocket]], 25 lines of code
 - [[https://github.com/karlicoss/promnesia/blob/master/src/promnesia/sources/fbmessenger.py][fbmessenger]], 30 lines of code
```

### Comparing `promnesia-1.1.20230129/doc/TROUBLESHOOTING.org` & `promnesia-1.2.20230515/doc/TROUBLESHOOTING.org`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/doc/config.py` & `promnesia-1.2.20230515/doc/config.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/docker/docker_files/Dockerfile` & `promnesia-1.2.20230515/docker/docker_files/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 FROM python:3
 
 RUN mkdir /user_data \
-    mkdir /usr/src/promnisia
+    mkdir /usr/src/promnesia
 
 WORKDIR /usr/src/promnesia
 COPY src/ .
 COPY setup.py /usr/src/
 
 #RUN python /usr/src/setup.py #LookupError: setuptools-scm was unable to detect version for '/usr/src/promnesia'.
 
 RUN pip install --no-cache-dir more_itertools pytz sqlalchemy cachew \
                 appdirs urlextract python-magic \
-                tzlocal hug \
-                logzero HPI beautifulsoup4 lxml mistletoe orgparse dataset
+                tzlocal \
+                logzero HPI beautifulsoup4 lxml mistletoe orgparse dataset fastapi uvicorn
 
 ENV PPATH=/usr/src/promnesia:${PPATH}
 VOLUME /user_data
 
 EXPOSE 13131
 CMD ["python", "-m", "promnesia", "serve", "--db", "/user_data/promnesia.sqlite", "--port", "13131"]
```

### Comparing `promnesia-1.1.20230129/docker/docker_files/docker-compose.yaml` & `promnesia-1.2.20230515/docker/docker_files/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/docker/docker_files/indexer-config.py.example` & `promnesia-1.2.20230515/docker/docker_files/indexer-config.py.example`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/.eslintrc.js` & `promnesia-1.2.20230515/extension/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/TODO.org` & `promnesia-1.2.20230515/extension/TODO.org`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/babel.config.js` & `promnesia-1.2.20230515/extension/babel.config.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/build` & `promnesia-1.2.20230515/extension/build`

 * *Files 5% similar despite different names*

```diff
@@ -13,47 +13,47 @@
 
 
 TARGETS = [
     'chrome',
     'firefox',
 ]
 
-def main():
+def main() -> None:
     p = argparse.ArgumentParser()
     p.add_argument('--release', action='store_true', help="Use release flavor of build")
     p.add_argument('--watch'  , action='store_true')
     p.add_argument('--lint'   , action='store_true')
-    p.add_argument('--publish', action='store_true', help="Publish on chrome web store/addons.mozilla.org")
+    p.add_argument('--publish', choices=['listed', 'unlisted'], help="Publish on chrome web store/addons.mozilla.org")
 
     tg = p.add_mutually_exclusive_group(required=True)
     tg.add_argument('--target', type=str, choices=TARGETS)
     for b in TARGETS:
         tg.add_argument('--' + b, action='store_const', const=b, dest='target')
     args = p.parse_args()
     target = args.target
 
     assert target is not None
 
     base_ext_dir = Path(__file__).absolute().parent / 'dist'
     ext_dir = (base_ext_dir / target).resolve() # webext can't into symlinks
     # sadly no way to specify zip name in the regex..
     artifacts_dir = (base_ext_dir / 'artifacts' / target).resolve()
-    def webext(*args, **kwargs):
+    def webext(*args, **kwargs) -> None:
         check_call([
             'npm', 'run', 'web-ext',
             '--',
             '--source-dir'   , ext_dir,
             '--artifacts-dir', artifacts_dir,
             *args,
         ], **kwargs)
 
     env = {
         'TARGET' : target,
         'RELEASE': 'YES' if args.release else 'NO',
-        'PUBLISH': 'YES' if args.publish else 'NO',
+        'PUBLISH': 'YES' if args.publish is not None else 'NO',
         'EXT_ID' : IDS[target],
         **os.environ,
     }
 
     if args.watch:
         check_call([
             'npm', 'run', 'watch',
@@ -82,25 +82,27 @@
         return [
             '--artifacts-dir', str(artifacts_dir),
             '--api-key'      , API_KEY,
             '--api-secret'   , API_SECRET,
             '--id'           , IDS[target],
         ]
 
-    if args.publish:
+    if args.publish is not None:
+        assert args.lint
         assert args.release
         if 'firefox' in target:
             check_call([
                 'npm', 'run', 'release:amo',
                 '--',
-                '--channel', 'listed',
+                '--channel', args.publish,
                 '--source-dir', str(ext_dir),
                 *firefox_release_args(),
             ])
         elif target == 'chrome':
+            assert args.publish == 'listed'  # no notion of unlisted on chrome store?
             from chrome_dev_secrets import CLIENT_ID, CLIENT_SECRET, REFRESH_TOKEN
             check_call([
                 'npm', 'run', 'release:cws',
                 '--',
                 'upload',
                 # '--auto-publish',
                 '--source'        , str(ext_dir),
```

### Comparing `promnesia-1.1.20230129/extension/flow-typed/webextension-polyfill.js` & `promnesia-1.2.20230515/extension/flow-typed/webextension-polyfill.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -176,30 +176,39 @@
     onCompleted: browser$WebNavigationX,
     onCommitted: browser$WebNavigationX,
     onTabReplaced: browser$WebNavigationX,
     onCreatedNavigationTarget: browser$WebNavigationX,
     onDOMContentLoaded: browser$WebNavigationX,
 }
 
+type browser$contextMenus = {
+    removeAll(): Promise < void > ,
+    onClicked: {
+        ...chrome$Event,
+        addListener(callback: $contextMenus$OnClick): void
+    }
+}
 
 declare var browser: {
     bookmarks: browser$bookmarks,
     history: browser$history,
     storage: browser$storage,
     permissions: browser$permissions,
     tabs: browser$tabs,
     scripting: browser$scripting,
     runtime: browser$runtime,
     webNavigation: browser$webNavigation,
+    contextMenus: browser$contextMenus,
 }
 
 
 declare module "webextension-polyfill" {
     declare var bookmarks: browser$bookmarks;
     declare var history: browser$history;
     declare var storage: browser$storage;
     declare var permissions: browser$permissions;
     declare var tabs: browser$tabs;
     declare var scripting: browser$scripting;
     declare var runtime: browser$runtime;
     declare var webNavigation: browser$webNavigation;
+    declare var contextMenus: browser$contextMenus;
 }
```

### Comparing `promnesia-1.1.20230129/extension/images/generate` & `promnesia-1.2.20230515/extension/images/generate`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/images/ic_blacklisted_48.png` & `promnesia-1.2.20230515/extension/images/ic_blacklisted_48.png`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/images/ic_blue_48.png` & `promnesia-1.2.20230515/extension/images/ic_blue_48.png`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/images/ic_boring_48.png` & `promnesia-1.2.20230515/extension/images/ic_boring_48.png`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/images/ic_error.png` & `promnesia-1.2.20230515/extension/images/ic_error.png`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/images/ic_not_visited_48.png` & `promnesia-1.2.20230515/extension/images/ic_not_visited_48.png`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/images/ic_relatives_48.png` & `promnesia-1.2.20230515/extension/images/ic_relatives_48.png`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/images/ic_visited_48.png` & `promnesia-1.2.20230515/extension/images/ic_visited_48.png`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/images/source_48.svg` & `promnesia-1.2.20230515/extension/images/source_48.svg`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/jest.config.js` & `promnesia-1.2.20230515/extension/jest.config.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/old/patcher.js` & `promnesia-1.2.20230515/extension/old/patcher.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/package.json` & `promnesia-1.2.20230515/extension/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.922676282051282%*

 * *Differences: {"'dependencies'": "{'tippy.js': '^6.3.7'}",*

 * * "'devDependencies'": "{'@babel/core': '^7.21.8', '@babel/eslint-parser': '^7.21.8', "*

 * *                      "'@babel/preset-env': '^7.21.5', '@babel/preset-flow': '^7.21.4', "*

 * *                      "'chrome-webstore-upload-cli': '^2.2.0', 'eslint': '^8.40.0', 'flow-bin': "*

 * *                      "'^0.206.0', 'jest': '^29.5.0', 'jest-environment-jsdom': '^29.5.0', "*

 * *                      "'node-fetch': '^3.3.1', 'style-loader': '^3.3.2', 'web-ext': '^7.6.2', "*

 * *    […]*

```diff
@@ -7,43 +7,44 @@
         "url": "https://github.com/karlicoss/promnesia/issues"
     },
     "dependencies": {
         "@codemirror/lang-css": "^6.0.1",
         "@codemirror/lang-javascript": "^6.1.2",
         "anchorme": "github:karlicoss/anchorme.js#promnesia",
         "codemirror": "^6.0.1",
+        "tippy.js": "^6.3.7",
         "webext-options-sync": "^4.0.0"
     },
     "description": "Recall what you already visited, why and in which context",
     "devDependencies": {
-        "@babel/core": "^7.20.12",
-        "@babel/eslint-parser": "^7.19.1",
-        "@babel/preset-env": "^7.20.2",
-        "@babel/preset-flow": "^7.18.6",
+        "@babel/core": "^7.21.8",
+        "@babel/eslint-parser": "^7.21.8",
+        "@babel/preset-env": "^7.21.5",
+        "@babel/preset-flow": "^7.21.4",
         "babel-loader": "^9.1.2",
-        "chrome-webstore-upload-cli": "^2.1.0",
+        "chrome-webstore-upload-cli": "^2.2.0",
         "clean-webpack-plugin": "^4.0.0",
         "copy-webpack-plugin": "^11.0.0",
         "css-loader": "^6.7.3",
-        "eslint": "^8.31.0",
+        "eslint": "^8.40.0",
         "eslint-plugin-flowtype": "^8.0.3",
-        "flow-bin": "^0.196.3",
+        "flow-bin": "^0.206.0",
         "flow-interfaces-chrome": "^0.7.0",
-        "jest": "^29.3.1",
-        "jest-environment-jsdom": "^29.3.1",
+        "jest": "^29.5.0",
+        "jest-environment-jsdom": "^29.5.0",
         "jest-fetch-mock": "^3.0.3",
         "loader-utils": "^3.2.1",
-        "node-fetch": "^3.3.0",
-        "style-loader": "^3.3.1",
-        "web-ext": "^7.4.0",
-        "web-ext-submit": "^7.4.0",
+        "node-fetch": "^3.3.1",
+        "style-loader": "^3.3.2",
+        "web-ext": "^7.6.2",
+        "web-ext-submit": "^7.6.2",
         "webextension-polyfill": "^0.10.0",
-        "webpack": "^5.75.0",
-        "webpack-cli": "^5.0.1",
-        "webpack-dev-server": "^4.11.1",
+        "webpack": "^5.82.1",
+        "webpack-cli": "^5.1.1",
+        "webpack-dev-server": "^4.15.0",
         "webpack-extension-manifest-plugin": "^0.8.0"
     },
     "homepage": "https://github.com/karlicoss/promnesia#readme",
     "keywords": [
         "pkm",
         "history"
     ],
@@ -62,10 +63,10 @@
         "flow": "flow",
         "release:amo": "web-ext-submit",
         "release:cws": "chrome-webstore-upload",
         "test": "jest",
         "watch": "webpack --watch --progress",
         "web-ext": "web-ext"
     },
-    "version": "1.1.2",
-    "version_name": "released on 2022.05.24"
+    "version": "1.2.4",
+    "version_name": "released on 2023.05.13"
 }
```

### Comparing `promnesia-1.1.20230129/extension/src/api.js` & `promnesia-1.2.20230515/extension/src/api.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -108,30 +108,30 @@
         fake.apiVisits(count).map(v => unwrap(rawToVisit(v))),
     )
 }
 
 
 export const backend = {
     visits: async function(url: Url): Promise < Visits | Error > {
-        return await queryBackendCommon < JsonObject > ({
+        return await queryBackendCommon < VisitsResponse > ({
                 url: url
             }, 'visits')
             .then(rawToVisits)
             .catch((err: Error) => err)
         // todo not sure if this error handling should be here?
     },
     search: async function(url: Url): Promise < Visits | Error > {
-        return await queryBackendCommon < JsonObject > ({
+        return await queryBackendCommon < VisitsResponse > ({
                 url: url
             }, 'search')
             .then(rawToVisits)
             .catch((err: Error) => err)
     },
     searchAround: async function(utc_timestamp_s: number): Promise < Visits | Error > {
-        return await queryBackendCommon < JsonObject > ({
+        return await queryBackendCommon < VisitsResponse > ({
                 timestamp: utc_timestamp_s
             }, 'search_around')
             .then(rawToVisits)
             .catch((err: Error) => err)
     },
     visited: async function(urls: Array < Url > ): Promise < Array < ? Visit > | Error > {
         return await queryBackendCommon < VisitedBackendResponse > ({
@@ -180,15 +180,15 @@
 function rawToVisits(vis: VisitsResponse | Error): Visits | Error {
     if (vis instanceof Error) {
         // most likely, network error.. so handle it defensively
         return vis
     }
     // TODO filter errors? not sure.
     // TODO this could be more defensive too
-    const visits = vis['visits'].map(x => unwrap(rawToVisit(x)))
+    const visits: Array < Visit | Error > = vis['visits'].map(x => unwrap(rawToVisit(x)))
     return new Visits(
         vis['original_url'],
         vis['normalised_url'],
         visits
     )
 }
```

### Comparing `promnesia-1.1.20230129/extension/src/background.js` & `promnesia-1.2.20230515/extension/src/background.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -41,21 +41,23 @@
 
 
 // useful for debugging
 const UUID = uuid()
 console.info('[promnesia]: running background page with UUID %s', UUID)
 
 
+type Action = chrome$browserAction | chrome$pageAction
 
-function actions(): Array < chrome$browserAction | chrome$pageAction > {
+
+function actions(): Array < Action > {
     // eh, on mobile neither pageAction nor browserAction have setIcon
     // but we can use pageAction to show at least some (default) icon in some circumstances
 
     // https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Differences_between_desktop_and_Android#User_interface
-    const res = [chrome.browserAction]
+    const res: Array < Action > = [chrome.browserAction]
 
     // need to be defensive, it's only for mobile firefox
     if (chrome.pageAction) {
         res.push(chrome.pageAction)
     } else {
         // this is a bit backwards because we need to register callbacks synchronously
         // otherwise isn't not working well after background page unloads
@@ -738,14 +740,16 @@
         // sendResponse(visits);
         // return true; // this is important!! otherwise message will not be sent?
     } else if (method == Methods.SEARCH_VISITS_AROUND) {
         const utc_timestamp_s: number = msg.utc_timestamp_s
         await handleOpenSearch({
             utc_timestamp_s: utc_timestamp_s.toString()
         })
+    } else if (method == Methods.OPTIONS_UPDATED) {
+        updateContextMenus(msg.options)
     } else if (method == Methods.MARK_VISITED) {
         await defensify(handleToggleMarkVisited, 'handleToggleMarkVisited')()
     } else if (method == Methods.OPEN_SEARCH) {
         await handleOpenSearch()
     } else if (method == Methods.ZAPPER_EXCLUDELIST) {
         await AddToMarkVisitedExcludelist.handleZapperResult(msg)
     }
@@ -1022,15 +1026,16 @@
     callback: (_info, _tab) => handleOpenSearch(),
 }, {
     id: 'menu_toggles',
     title: 'Quick toggles',
     callback: null,
 }, ]
 
-type MenuToggle = MenuEntry & {
+type MenuToggle = {
+    ...MenuEntry,
     checker: (opts: Options) => boolean,
 }
 
 const TOGGLES: Array < MenuToggle > = [{
     parentId: 'menu_toggles', // meh
     id: 'menu_toggles_sidebar',
     title: 'Always show sidebar',
@@ -1046,101 +1051,137 @@
     parentId: 'menu_toggles', // meh
     id: 'menu_toggles_highlights',
     title: 'Always show highlights',
     checker: opts => opts.highlight_on,
     callback: Toggles.showHighlights,
 }, ]
 
-
-function initBackground() {
-    // NOTE: callback registering needs to be synchronous
-    // otherwise doesn't work well with background page suspension
-
-    // $FlowFixMe
-    chrome.runtime.onMessage.addListener(onMessageCallback)
-
-    registerActions()
-
-    // need to be defensive since commands API isn't available under mobile browser
-    if (chrome.commands) {
-        //  $FlowFixMe // err, complains at Promise but nevertheless works
-        chrome.commands.onCommand.addListener(onCommandCallback)
-    } else {
+function hasContextMenus() : boolean {
+    // need to be defensive since contextMenus API isn't available under mobile browser
+    if (browser.contextMenus == undefined) {
         isMobile().then(mobile => {
             if (!mobile) {
-                notifyError("error: chrome.commands should be available")
+                notifyError("error: chrome.contextMenus should be available")
             }
         })
+        return false
     }
+    return true
+}
 
-    // not sure why but context menus need to be created in onInstalled?
-    // https://stackoverflow.com/a/19578984/706389
-    chrome.runtime.onInstalled.addListener(() => {
-        // need to be defensive since contextMenus API isn't available under mobile browser
-        if (chrome.contextMenus == undefined) {
-            isMobile().then(mobile => {
-                if (!mobile) {
-                    notifyError("error: chrome.contextMenus should be available")
-                }
-            })
-            return
-        }
+
+function initContextMenus(): void {
+    if (!hasContextMenus()) {
+        return
+    }
+
+    /*
+    Normally, you'd create context menu in chrome.runtime.onInstalled, since browser remembers context menu items in between installs.
+    see https://stackoverflow.com/a/19578984/706389
+    So if you create context menus outside of onInstalled, it would try to create same menus twice and cause error.
+    However then we can't change its states (checked/unchecked in this case) in response to changing options.
+    If we add the call to update context menu outside of onInstalled, then it might have a race condition on first init, 
+    and will fail to set checks on non yet existing menu itmes.
+    So seems the easiest to just remove all menus and init them again :shrug:
+    */
+    browser.contextMenus.removeAll().then(() => {
         for (const {
                 id: id,
                 title: title,
                 parentId: parentId,
                 contexts: contexts
             }
             of MENUS) {
             chrome.contextMenus.create({
                 id: id,
                 parentId: parentId,
                 title: title,
                 contexts: contexts || DEFAULT_CONTEXTS,
             })
         }
-        // TODO crap -- we need to refresh these menus when options update??
-        // it's broken in prod though so can live without it for a bit
-        // also cover with a test
-        getOptions().then((opts) => {
-            for (const {
-                    id: id,
-                    title: title,
-                    parentId: parentId,
-                    checker: checker,
-                    contexts: contexts
-                }
-                of TOGGLES) {
-                chrome.contextMenus.create({
-                    id: id,
-                    parentId: parentId,
-                    title: title,
-                    contexts: contexts || DEFAULT_CONTEXTS,
-                    type: 'checkbox',
-                    checked: checker(opts),
-                })
+
+        for (const {
+                id: id,
+                title: title,
+                parentId: parentId,
+                contexts: contexts
             }
-        })
+            of TOGGLES) {
+            chrome.contextMenus.create({
+                id: id,
+                parentId: parentId,
+                title: title,
+                contexts: contexts || DEFAULT_CONTEXTS,
+                type: 'checkbox',
+            })
+        }
+        getOptions().then((opts) => updateContextMenus(opts))
+    })
 
-        const onMenuClickedCallback = defensify(async (info: MenuInfo, tab: chrome$Tab) => {
-            const mid = info.menuItemId
-            for (const m of [...MENUS, ...TOGGLES]) {
-                if (mid == m.id) {
-                    const cb = m.callback
-                    if (cb != null) {
-                        await cb(info, tab)
-                    }
-                    break
+    // need to keep these callbacks here, since onInstalled above isn't called when background page resumes
+    const onMenuClickedCallback = defensify(async (info: MenuInfo, tab: chrome$Tab) => {
+        const mid = info.menuItemId
+        for (const m of [...MENUS, ...TOGGLES]) {
+            if (mid == m.id) {
+                const cb = m.callback
+                if (cb != null) {
+                    await cb(info, tab)
                 }
+                break
             }
-        }, 'onMenuClicked');
+        }
+    }, 'onMenuClicked')
+
+    // seems that it's best to keep onClicked listenere here (instead of inside removeAll)
+    // otherwise it's not working in firefox
+    // $FlowFixMe[incompatible-call] flow complains presumably because of defensify
+    browser.contextMenus.onClicked.addListener(onMenuClickedCallback)
+}
+
+
+function updateContextMenus(opts: Options): void {
+    if (!hasContextMenus()) {
+        return
+    }
+    for (const {
+            id: id,
+            checker: checker
+        }
+        of TOGGLES) {
+        chrome.contextMenus.update(
+            id, {
+                checked: checker(opts)
+            },
+        )
+    }
+}
+
+
+function initBackground(): void {
+    // NOTE: callback registering needs to be synchronous
+    // otherwise doesn't work well with background page suspension
 
+    // $FlowFixMe
+    chrome.runtime.onMessage.addListener(onMessageCallback)
+
+    registerActions()
+
+    // need to be defensive since commands API isn't available under mobile browser
+    if (chrome.commands) {
         //  $FlowFixMe // err, complains at Promise but nevertheless works
-        chrome.contextMenus.onClicked.addListener(onMenuClickedCallback)
-    })
+        chrome.commands.onCommand.addListener(onCommandCallback)
+    } else {
+        isMobile().then(mobile => {
+            if (!mobile) {
+                notifyError("error: chrome.commands should be available")
+            }
+        })
+    }
+
+    initContextMenus()
 }
 
 
 chrome.runtime.onMessage.addListener((info: any, _: chrome$MessageSender) => {
     // see selenium_bridge.js
     if (info === 'selenium-bridge-activate') {
         handleToggleSidebar()
@@ -1153,13 +1194,10 @@
     }
 })
 
 initBackground()
 
 
 // for debugging
-/*
-browser.runtime.onSuspend.addListener(() => {
-    console.error("SUSPENDING BACKGROUND PAGE!!")
-    notifyError("SUSPENDING BACKGROUND!!")
-})
-*/
+// browser.runtime.onSuspend.addListener(() => {
+//     notifyError("SUSPENDING BACKGROUND!!")
+// })
```

### Comparing `promnesia-1.1.20230129/extension/src/common.js` & `promnesia-1.2.20230515/extension/src/common.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -147,15 +147,15 @@
         // NOTE: JSON.stringify will use this method
         toJObject(): any {
             const o = {}
             // $FlowFixMe[prop-missing]
             Object.assign(o, this)
             // $FlowFixMe[prop-missing]
             // $FlowFixMe[incompatible-use]
-            o.visits = o.visits.map(v => {
+            o.visits = o.visits.map((v: Visit | Error) => {
                 return (v instanceof Visit) ?
                     v.toJObject()
                     // $FlowFixMe
                     :
                     {
                         error: v.message,
                         stack: v.stack
@@ -199,14 +199,15 @@
 export const Methods = {
     GET_SIDEBAR_VISITS: 'getActiveTabVisitsForSidebar',
     BIND_SIDEBAR_VISITS: 'bindSidebarVisits',
     SEARCH_VISITS_AROUND: 'searchVisitsAround',
     MARK_VISITED: 'markVisited',
     OPEN_SEARCH: 'openSearch',
     SIDEBAR_TOGGLE: 'sidebarToggle',
+    OPTIONS_UPDATED: 'optionsUpdated',
     // TODO not used
     SIDEBAR_SHOW: 'sidebarShow',
     ZAPPER_EXCLUDELIST: 'zapperExcludelist',
 }
 
 export const Ids = {
     // visits container in sidebar/search (see sidebar.css)
@@ -253,15 +254,15 @@
 }
 
 
 // shit. if I type Json properly, then it requires too much isinstance checks...
 // https://github.com/facebook/flow/issues/4825
 
 export type JsonArray = Array < Json >
-    export type JsonObject = $Shape < {
+    export type JsonObject = Partial < {
         [string]: any
     } >
     export type Json = JsonArray | JsonObject
 
 
 export function getBrowser(): string {
     // https://stackoverflow.com/questions/12489546/getting-a-browsers-name-client-side
@@ -337,15 +338,15 @@
     // if it's not cached, it will make a real request
     // anso works offline (returns cached response with no errors)
     const cached_resp = await fetch_typed(url, {
         cache: 'force-cache'
     }).then(rejectIfHttpError)
     const expires = cached_resp.headers.get('expires')
     // not sure if it's possible not to have 'expires'
-    const stale_ms = new Date() - new Date(expires == null ? 0 : expires)
+    const stale_ms = new Date().getTime() - new Date(expires == null ? 0 : expires).getTime()
     const max_stale_ms = max_stale * 1000
     if (stale_ms < max_stale_ms) {
         return cached_resp
     } else {
         // do a regular request instead
         return fetch_typed(url).then(rejectIfHttpError)
     }
```

### Comparing `promnesia-1.1.20230129/extension/src/display.js` & `promnesia-1.2.20230515/extension/src/display.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/filterlist.js` & `promnesia-1.2.20230515/extension/src/filterlist.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/normalise.js` & `promnesia-1.2.20230515/extension/src/normalise.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/notifications.js` & `promnesia-1.2.20230515/extension/src/notifications.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/options.js` & `promnesia-1.2.20230515/extension/src/options.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,11 @@
 /* @flow */
 import {
-    getBrowser
+    getBrowser,
+    Methods
 } from './common'
 
 /* NOTE: options can only be renamed in-between store releases */
 /* maybe later will bother with migrations for consistent naming, but that would require tests first */
 
 // ugh. hacky way to support partial option setting...
 type Opt1 = {
@@ -297,28 +298,40 @@
     return {
         ...stored,
         ...devDefaults
     }
 }
 
 
+async function notifyOptionsUpdated(): Promise < void > {
+    const options = await getOptions() // meh
+    browser.runtime.sendMessage({
+        method: Methods.OPTIONS_UPDATED,
+        options: options
+    })
+}
+
+
 // TODO would be nice to accept a substructure of Options??
 export async function setOptions(opts: StoredOptions) {
     const os = await optSync()
     await os.set(opts)
+    notifyOptionsUpdated()
 }
 
 export async function setOption(opt: Opt1 | Opt2): Promise < void > {
     const os = await optSync()
     await os.set(opt)
+    notifyOptionsUpdated()
 }
 
 export async function resetOptions(): Promise < void > {
     const os = await optSync()
     await os.setAll({})
+    notifyOptionsUpdated()
 }
 
 type ToggleOptionRes = () => Promise < void >
     function toggleOption(toggle: (StoredOptions) => void): ToggleOptionRes {
         return async () => {
             const opts = await getStoredOptions()
             toggle(opts)
```

### Comparing `promnesia-1.1.20230129/extension/src/options_page.css` & `promnesia-1.2.20230515/extension/src/options_page.css`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/options_page.html` & `promnesia-1.2.20230515/extension/src/options_page.html`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/options_page.js` & `promnesia-1.2.20230515/extension/src/options_page.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/search.html` & `promnesia-1.2.20230515/extension/src/search.html`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/search.js` & `promnesia-1.2.20230515/extension/src/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -75,15 +75,15 @@
     clearResults();
 
     const errres = await cb
     if (errres instanceof Error) {
         throw errres // will be handled above
     }
     const [visits, errors] = errres.partition()
-    visits.sort((f, s) => (s.time - f.time));
+    visits.sort((f, s) => (s.time.getTime() - f.time.getTime()))
     // TODO ugh, should do it via sort predicate...
 
     if (with_ctx_first) {
         visits.sort((f, s) => (f.context === null ? 1 : 0) - (s.context === null ? 1 : 0));
     }
 
     const res = getResultsContainer();
@@ -177,15 +177,15 @@
 
 
 window.onload = async () => {
     const opts = await getOptions()
     addStyle(doc, opts.position_css);
 
     const url = new URL(window.location)
-    const params: SearchPageParams = Object.fromEntries(url.searchParams)
+    const params = ((Object.fromEntries(url.searchParams): any): SearchPageParams)
     if (Object.keys(params).length == 0) {
         return
     }
 
     const q_param = params['q']
     if (q_param != null) {
         getQuery().value = q_param
```

### Comparing `promnesia-1.1.20230129/extension/src/showvisited.css` & `promnesia-1.2.20230515/extension/src/showvisited.css`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,18 @@
-/* TODO non-selectable? should probably be from the parent.. */
-
 /* TODO use variables */
 
-/* the mark that shows near the link */
-.promnesia-visited-eye {
-
-    /* absolute relative to the parent wrapper that forces zero space */
-    position: absolute;
-
-    /* display slightly above the text */
-    bottom: 1em;
-}
-
-/* invisible area taking 25% of the link and lets you click and pin the popup */
-.promnesia-visited-toggler {
-    cursor: crosshair;
-}
-
-
 /* actual popup with the metadata */
 .promnesia-visited-popup {
-    outline: solid 1px;
+    display: block; /* otherwise border etc don't work? */
+    white-space: pre-wrap; /* keep whitespace intact */
+
     background: #e6e6e6fa; /* same color as in sidebar */
+    color: black; /* to prevent it inheriting white text colour in dark mode */
+
+    outline: solid 1px;
     padding: 2px;
     /* not sure about initial?? */
     font-weight: initial;
     font-size: initial;
 }
 
 .promnesia-visited-popup .promnesia-visited-popup-link {
@@ -38,33 +25,25 @@
 .promnesia-visited-popup .context {
     display: block;
     /* color: black; */
     background: lightyellow;
     margin: 2px;
 }
 
+/* TODO need to use these styles in tippy */
 .promnesia-visited-popup .datetime {
     display: inline-block;
     float: right;
     padding-left: 0.5em;
 }
 
-/* close buton within the popup */
-.promnesia-visited-popup-close {
-    display: inline-block;
-    min-width: 1.5em;
-    min-height: 1.5em;
-    text-align: center;
-    font-weight: bold;
-    float: right;
-    color: red;
-    cursor: pointer;
-}
 
-.promnesia-visited-popup-help {
-    display: inline-block;
-    min-width: 1.5em;
-    min-height: 1.5em;
-    text-align: center;
-    font-weight: bold;
-    float: right;
+/* TODO not really sure about !important...  */
+.promnesia-visited.promnesia-eye {
+    /* note: outline is defined in sidebar.css */
+    background-repeat: no-repeat !important; /* repeats by default */
+    background-position-x: right !important; /* left by default */
+
+    /* same as text size, we just want a small icon */
+    /* using rem to prevent it from scaling too much on navigation elements etc */
+    background-size: '1rem' !important;
 }
```

### Comparing `promnesia-1.1.20230129/extension/src/sidebar-outer.css` & `promnesia-1.2.20230515/extension/src/sidebar-outer.css`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/sidebar.css` & `promnesia-1.2.20230515/extension/src/sidebar.css`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 }
 
 .promnesia a {
     text-decoration: none;
 }
 
 a.promnesia-visited {
-    outline: 0.5em solid;
+    /* hmm without important isn't working on some sites, e.g. google.com search results */
+    outline: 0.5em solid !important;
 }
 
 #promnesia-sidebar {
     display: flex;
     flex-flow: column;
     height: 100%;
     margin: 0;
```

### Comparing `promnesia-1.1.20230129/extension/src/sidebar.js` & `promnesia-1.2.20230515/extension/src/sidebar.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,16 @@
     Methods,
     addStyle,
     Ids,
     uuid,
     getOrDefault
 } from './common'
 import type {
-    Second
+    Second,
+    Src
 } from './common'
 import {
     getOptions,
     USE_ORIGINAL_TZ,
     GROUP_CONSECUTIVE_SECONDS
 } from './options';
 import type {
@@ -214,17 +215,28 @@
 
     async ensureFrame(): Promise < HTMLIFrameElement > {
         const frame = this.getFrame();
         if (frame != null) {
             return frame;
         }
 
-        const sidebar = doc.createElement('iframe');this.body.appendChild(sidebar);
-        sidebar.src = '';
-
+        const sidebar = doc.createElement('iframe')
+        sidebar.style.display = 'none' // prevent flickering while iframe is being initialised
+        const isFirefox = window.navigator.userAgent.indexOf('Firefox') != -1
+        if (isFirefox) {
+            // under firefox, if src is set after appendChild, it ceases to be bfcache friendly for some reason
+            // i.e. sidebar doesn't persist back/fwd navigation
+            // however, it only reproduced under regular firefox -- doesn't matter under webdriver. odd
+            sidebar.src = ''
+            this.body.appendChild(sidebar)
+        } else {
+            // BUT: under chrome if src is set before appendChild, it just doesn't display anything?? ugh
+            this.body.appendChild(sidebar)
+            sidebar.src = ''
+        }
 
         // TODO ugh it's a bit ridiculous that because of single iframe I have to propagate async everywhere..
         const loadPromise = new Promise((resolve, /*reject*/ ) => {
             // TODO not sure if there is anything to reject?..
             sidebar.addEventListener('load', () => {
                 resolve();
             }, {
@@ -297,15 +309,15 @@
         lines.delete(matched)
         yield [matched, elem]
     }
 }
 
 // TODO potentially not very efficient; replace with something existing (Hypothesis??)
 function _highlight(text: string, idx: number, v: Visit) {
-    const lines = new Set()
+    const lines = new Set < string > ()
     for (const line of text.split('\n')) {
         let sline = line.trim()
         if (sline.length == 0) {
             continue // no need to log
         }
         sline = _sanitize(line)
         if (sline.length <= 3) {
@@ -335,14 +347,21 @@
         }
 
         if (target.classList.contains('toastify')) {
             // hacky.. to avoid a race condition when toast notification is shown
             continue
         }
 
+        if (target.classList.contains('promnesia-visited-popup-link')) {
+            // prevent highlight from being shown in tooltips
+            // hmm a bit crap, ideally would target promnesia-visited-popup
+            // but not sure how to get classes including parent classes??
+            continue
+        }
+
         // TODO why doesn't flow warn about this??
         // target.name === 'body'
         if (target === doc.body) {
             // meh, but otherwise too spammy
             console.debug('promnesia: body matched for highlight; skipping it')
             continue;
         }
@@ -447,31 +466,32 @@
         // keep 'relatives' in the bottom
         // TODO: this might slightly break local visits sorting, because they don't necessarily have proper normalisation
         const fr = f.normalised_url === normalised
         const sr = s.normalised_url === normalised
         if (fr != sr) {
             return (sr ? 1 : 0) - (fr ? 1 : 0);
         }
-        return s.time - f.time;
-    });
+        return s.time.getTime() - f.time.getTime()
+    })
 
     // move visits with contexts on top
     const with_ctx = [];
     const no_ctx = [];
     for (const v of visits) {
         if (v.context === null) {
             no_ctx.push(v);
         } else {
             with_ctx.push(v);
         }
     }
 
     // TODO instead, use checkboxes and get checked values
     // TODO not sure if should ignore things without contexts here... how to fit everything?
-    const all_tags = new Map();
+    const all_tags = new Map < Src,
+        number > ()
     for (const v of with_ctx) {
         for (const t of v.tags) {
             // $FlowFixMe
             const pv = (all_tags.has(t) ? all_tags.get(t) : 0) + 1;
             all_tags.set(t, pv);
         }
     }
@@ -557,15 +577,15 @@
 
     const delta_ms = GROUP_CONSECUTIVE_SECONDS * 1000;
 
     function* groups() {
         let group = [];
         for (const v of no_ctx) {
             const last = group.length == 0 ? v : group[group.length - 1];
-            const diff = last.time - v.time
+            const diff = last.time.getTime() - v.time.getTime()
             if (diff > delta_ms) {
                 if (group.length > 0) {
                     yield group;
                 }
                 group = []
             }
             group.push(v);
@@ -585,15 +605,15 @@
         const first = group[0];
         const last = group[group.length - 1];
         // eslint-disable-next-line no-unused-vars
         const [fdates, ftimes] = visit_date_time(first)
         const [ldates, ltimes] = visit_date_time(last)
         const dates = ldates;
         const times = ltimes == ftimes ? ltimes : ltimes + "-" + ftimes;
-        const tset = new Set();
+        const tset = new Set < Src > ();
         let total_dur: ? Second = null;
         for (const v of group) {
             if (v.duration !== null) {
                 if (total_dur === null) {
                     total_dur = 0;
                 }
                 // $FlowFixMe
@@ -658,23 +678,17 @@
     } else if (method == Methods.SIDEBAR_TOGGLE) {
         sidebar().then(s => s.toggle())
     }
     // todo do I need to return anything?
 }
 
 
-const doc_body = unwrap(document.body)
-
-
 // this is necessary because due to data races it's possible for sidebar.js to be injected twice in the page
-// NOTE: we can't use window. variables here, seems that their state isn't preserved under geckodriver
-// see https://github.com/mozilla/geckodriver/issues/2075
-// perhaps have a separate version for testing purposes only??
-if (doc_body.getAttribute('promnesia_haslistener') == null) {
-    doc_body.setAttribute('promnesia_haslistener', 'true')
+if (window.promnesia_haslistener == null) {
+    window.promnesia_haslistener = true
     console.debug(`[promnesia] [sidebar-${UUID}] registering callbacks`)
     chrome.runtime.onMessage.addListener(onMessageListener)
 } else {
     console.debug(`[promnesia] [sidebar-${UUID}] skipping callback registration, they are already present`)
 }
 
 // TODO make configurable? or resizable?
```

### Comparing `promnesia-1.1.20230129/extension/src/sources.js` & `promnesia-1.2.20230515/extension/src/sources.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -65,15 +65,15 @@
     for (const r of it) {
         const u = r.url
         const ts = r.lastVisitTime
         if (u == null || ts == null) {
             continue
         }
         const t = new Date(ts)
-        if (now - t <= delay) {
+        if (now.getDate() - t.getDate() <= delay) {
             continue // filter it out
         }
         yield new Visit(
             u,
             normalise_url(u),
             ((t: any): AwareDate),
             ((t: any): NaiveDate),
@@ -105,16 +105,16 @@
 
         // NOTE: this normalise won't necessarily be the same as backend's... not sure what we can do about it without sending visits?
         const nurl = normalise_url(url)
 
         // NOTE: visitTime returns UTC epoch,
         const times: Array < Date > = results
             .map(r => new Date(r['visitTime'] || 0.0))
-            .filter(dt => now - dt > delay)
-        const visits = times.map(t => new Visit(
+            .filter(dt => now.getTime() - dt.getTime() > delay)
+        const visits: Array < Visit | Error > = times.map(t => new Visit(
             url,
             nurl,
             ((t: any): AwareDate),
             ((t: any): NaiveDate), // there is no TZ info in history anyway, so not much else we can do
             [THIS_BROWSER_TAG],
         ))
         return new Visits(url, nurl, visits)
@@ -126,15 +126,15 @@
         if (android) {
             return new Visits(url, url, [])
         }
         const nurl = normalise_url(url)
         const results = await browser.history.search({
             text: url
         })
-        const visits = Array.from(search2visits(results))
+        const visits: Array < Visit | Error > = Array.from(search2visits(results))
         return new Visits(url, nurl, visits)
     },
     searchAround: async function(utc_timestamp_s: number): Promise < Visits | Error > {
         const durl = 'http://dummy.xyz'
         const ndurl = normalise_url(durl)
         const android = await isAndroid()
         if (android) {
@@ -151,15 +151,15 @@
             endTime: end,
             text: '',
             maxResults: opts.browserhistory_max_results,
         })
         // right. this only returns history items with lastVisitTime
         // (see https://developer.chrome.com/extensions/history#type-HistoryItem)
         // so we need another pass to collec the 'correct' visit times
-        const visits = []
+        const visits: Array < Visit | Error > = []
         for (const r of results) {
             const u = r.url
             if (u == null) {
                 continue
             }
             const nu = normalise_url(u)
             // eh. apparently URL is the only useful?
@@ -234,15 +234,15 @@
             }
         }
     }
 }
 
 
 // todo take in from_, to?
-function* bookmarks2visits(bit: Iterable < Bres > ) {
+function* bookmarks2visits(bit: Iterable < Bres > ): Iterator < Visit > {
     for (const {
             bm: r,
             nurl: nu,
             path: path
         }
         of bit) {
         const u = r.url
@@ -277,15 +277,15 @@
         if (await isAndroid()) {
             // https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs#bookmarks :(
             return new Visits(url, url, [])
         }
         const nurl = normalise_url(url)
         const root = (await browser.bookmarks.getTree())[0]
         const all = bookmarksContaining(nurl, root, null)
-        const visits = Array.from(bookmarks2visits(all))
+        const visits: Array < Visit | Error > = Array.from(bookmarks2visits(all))
         return new Visits(url, nurl, visits)
     },
 
     search: async function(url: Url): Promise < Visits | Error > {
         // for bookmarks, search means the same as visits because they all come with context
         return (await bookmarks.visits(url))
     },
@@ -299,26 +299,26 @@
         }
         const root = (await browser.bookmarks.getTree())[0]
         const all = bookmarksContaining('', root, null)
         // todo for the sake of optimization might be better to do this before building all the Visit objects..
         // same in visited method actually
         const back = new Date((utc_timestamp_s - DELTA_BACK_S) * 1000)
         const front = new Date((utc_timestamp_s + DELTA_FRONT_S) * 1000)
-        const visits = []
+        const visits: Array < Visit | Error > = []
         for (const v of bookmarks2visits(all)) {
             if (back <= v.time && v.time <= front) {
                 visits.push(v)
             }
         }
         return new Visits(durl, ndurl, visits)
     },
 
     visited: async function(urls: Array < Url > ): Promise < VisitedResult | Error > {
         if (await isAndroid()) {
-            const res = new Array(urls.length)
+            const res = new Array < ? Visit > (urls.length)
             res.fill(null)
             return res
         }
 
         const root = (await browser.bookmarks.getTree())[0]
         const all = bookmarksContaining('', root, null)
 
@@ -418,15 +418,15 @@
             return errors[0]
         }
         return new Error("No datasources?")
     }
 
     static async get(): Promise < MultiSource > {
         const opts = await getOptions()
-        const srcs = []
+        const srcs: Array < VisitsSource > = []
         if (opts.host != '') {
             srcs.push(backend)
         }
         if (opts.use_bookmarks) {
             srcs.push(bookmarks)
         }
         if (opts.use_browserhistory) {
```

### Comparing `promnesia-1.1.20230129/extension/src/toastify.css` & `promnesia-1.2.20230515/extension/src/toastify.css`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/src/toastify.js` & `promnesia-1.2.20230515/extension/src/toastify.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/tests/common.test.js` & `promnesia-1.2.20230515/extension/tests/common.test.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/tests/defensify.test.js` & `promnesia-1.2.20230515/extension/tests/defensify.test.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/tests/integration.test.js` & `promnesia-1.2.20230515/extension/tests/integration.test.js`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/tests/test.html` & `promnesia-1.2.20230515/extension/tests/test.html`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/extension/webpack.config.js` & `promnesia-1.2.20230515/extension/webpack.config.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -116,14 +116,15 @@
         "48": "images/ic_not_visited_48.png",
     },
     browser_action: action,
     permissions: permissions,
     options_ui: {},
     web_accessible_resources: [
         "sidebar.css", /* injected in the sidebar */
+        "*.js.map", // debugging symbols
     ],
 }
 
 // this is only needed during testing
 if (!publish) {
     manifestExtra.content_scripts = [{
         "matches": ["<all_urls>"],
@@ -222,14 +223,17 @@
             import: 'anchorme',
             library: {
                 name: 'promnesia_anchorme',
                 type: "window",
                 /* 'sets' library to window. variable... all the other types didn't work :( */
             },
         },
+        showvisited: {
+            import: path.join(__dirname, './src/showvisited'),
+        },
     },
     output: {
         // hmm. according to https://stackoverflow.com/a/64715069
         // settings publicPath: '' shouldn't be necessary anymore
         // but still without it getting "Automatic publicPath is not supported in this browser" when trying to open sidebar
         // whatever.
         publicPath: '',
@@ -279,17 +283,14 @@
                 // not sure if it's the right way, but I guess webpack can't guess otherwise
                 {
                     context: 'src',
                     from: 'toastify.js'
                 }, // TODO my version is tweaked, right?
                 {
                     context: 'src',
-                    from: 'showvisited.js'
-                }, {
-                    context: 'src',
                     from: 'selenium_bridge.js'
                 }, {
                     from: 'node_modules/webextension-polyfill/dist/browser-polyfill.js'
                 },
             ]
         }),
         new WebpackExtensionManifestPlugin({
```

### Comparing `promnesia-1.1.20230129/scripts/backup-phone-history.sh` & `promnesia-1.2.20230515/scripts/backup-phone-history.sh`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/scripts/browser_history.py` & `promnesia-1.2.20230515/scripts/browser_history.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/setup.py` & `promnesia-1.2.20230515/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         package_data={pkg: ['py.typed']},
 
         url='https://github.com/karlicoss/promnesia',
         author='Dmitrii Gerasimov',
         author_email='karlicoss@gmail.com',
         description='Enhancement of your browsing history',
 
-        python_requires='>=3.7',
+        python_requires='>=3.8',
         install_requires=[
             'appdirs', # for portable user directories detection
             'tzlocal',
             'more_itertools',
             'pytz',
             'sqlalchemy', # DB api
             'cachew>=0.8.0', # caching with type hints
@@ -48,14 +48,15 @@
             'testing': [
                  'pytest',
                  'pytest-timeout',
                  'pytest-xdist', # why??
 
                  'psutil',
 
+                 'requests<2.30.0',  # temporary, see https://github.com/psf/requests/issues/6443
                  'httpie',   # nicer http requests (replace with curl?)
                  'selenium', # browser automations
                  'click',    # confirmations for end2end test (might remove dependency)
 
                  'pyautogui', # for keyboard automation during end2end tests
             ],
             'linting': [
@@ -102,14 +103,14 @@
     ('markdown', 'dependencies for sources.markdown'): [
         'mistletoe',
     ],
     ('org'     , 'dependencies for sources.org'     ): [
         'orgparse>=0.3.0',
     ],
     ('telegram', 'dependencies for sources.telegram'): [
-        'dataset',
+        # used to depend on 'dataset', keeping for backwards compatibility
     ],
 }
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `promnesia-1.1.20230129/src/promnesia/__main__.py` & `promnesia-1.2.20230515/src/promnesia/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from __future__ import annotations
+
 import argparse
-import logging
+import ast
+import importlib
 import inspect
-import sys
-from typing import List, Tuple, Optional, Dict, Sequence, Iterable, Iterator, Union
 from pathlib import Path
-from datetime import datetime
-from .compat import check_call, register_argparse_extend_action_in_pre_py38
+import shutil
+from subprocess import run, check_call, Popen
+import sys
 from tempfile import TemporaryDirectory
+from typing import Callable, Sequence, Iterable, Iterator, Union
 
 
 from . import config
 from . import server
 from .misc import install_server
-from .common import PathIsh, logger, get_tmpdir, DbVisit, Res
+from .common import Extractor, PathIsh, logger, get_tmpdir, DbVisit, Res
 from .common import Source, get_system_tz, user_config_file, default_config_path
 from .dump import visits_to_sqlite
-from .extract import extract_visits, make_filter
+from .extract import extract_visits
 
 
 def iter_all_visits(sources_subset: Iterable[Union[str, int]]=()) -> Iterator[Res[DbVisit]]:
     cfg = config.get()
     output_dir = cfg.output_dir
     # not sure if belongs here??
     if not output_dir.exists():
@@ -32,15 +35,15 @@
 
     is_subset_sources = bool(sources_subset)
     if is_subset_sources:
         sources_subset = set(sources_subset)
 
     for i, source in enumerate(sources):
         # TODO why would it not be present??
-        name = getattr(source, "name", None)
+        name: str | None = getattr(source, "name", None)
         if name and is_subset_sources:
             matched = name in sources_subset or i in sources_subset
             if matched:
                 sources_subset -= {i, name}  # type: ignore
             else:
                 logger.debug("skipping '%s' not in --sources.", name)
                 continue
@@ -68,15 +71,15 @@
 
     if sources_subset:
         logger.warning("unknown --sources: %s", ", ".join(repr(i) for i in sources_subset))
 
 
 def _do_index(dry: bool=False, sources_subset: Iterable[Union[str, int]]=(), overwrite_db: bool=False) -> Iterable[Exception]:
     # also keep & return errors for further display
-    errors: List[Exception] = []
+    errors: list[Exception] = []
     def it() -> Iterable[Res[DbVisit]]:
         for v in iter_all_visits(sources_subset):
             if isinstance(v, Exception):
                 errors.append(v)
             yield v
 
     if dry:
@@ -107,48 +110,46 @@
         logger.error('%d errors, printing them out:', len(errors))
         for e in errors:
             logger.exception(e)
         logger.error('%d errors, exit code 1', len(errors))
         sys.exit(1)
 
 
-def demo_sources():
-    def lazy(name: str):
+def demo_sources() -> dict[str, Callable[[], Extractor]]:
+    def lazy(name: str) -> Callable[[], Extractor]:
         # helper to avoid failed imports etc, since people might be lacking necessary dependencies
-        def inner(*args, **kwargs):
+        def inner() -> Extractor:
             from . import sources
-            import importlib
-            module = importlib.import_module('promnesia.sources' + '.' + name)
+            module = importlib.import_module(f'promnesia.sources.{name}')
             return getattr(module, 'index')
         return inner
 
     res = {}
-    import ast
     import promnesia.sources
-    for p in promnesia.sources.__path__: # type: ignore[attr-defined] # should be present
+    path: list[str] = getattr(promnesia.sources, '__path__')  # should be present
+    for p in path:
         for x in sorted(Path(p).glob('*.py')):
             a = ast.parse(x.read_text())
             candidates = [c for c in a.body if getattr(c, 'name', None) == 'index']
             if len(candidates) > 0:
                 res[x.stem] = lazy(x.stem)
     return res
 
 
 def do_demo(
         *,
         index_as: str,
         params: Sequence[str],
-        port: Optional[str],
-        config_file: Optional[Path],
+        port: str | None,
+        config_file: Path | None,
         dry: bool=False,
         name: str='demo',
         sources_subset: Iterable[Union[str, int]]=(),
         overwrite_db: bool=False,
     ) -> None:
-    from pprint import pprint
     with TemporaryDirectory() as tdir:
         outdir = Path(tdir)
 
         if config_file is not None:
             config.load_from(config_file)
         else:
             idx = demo_sources()[index_as]()
@@ -181,15 +182,14 @@
             )
 
         if sys.stdin.isatty():
             input("Press any key when ready")
 
 
 def read_example_config() -> str:
-    import inspect
     from .misc import config_example
     return inspect.getsource(config_example)
 
 
 def config_create(args: argparse.Namespace) -> None:
     cfg = user_config_file()
     cfgdir = cfg.parent
@@ -210,26 +210,24 @@
         logger.info('OK')
     else:
         logger.error('CHECK FAILED')
         sys.exit(1)
 
 
 def _config_check(cfg: Path) -> Iterable[Exception]:
-    from .compat import run
-
     logger.info('config: %s', cfg)
 
-    def check(cmd) -> Iterable[Exception]:
+    def check(cmd: list[str | Path]) -> Iterable[Exception]:
         logger.debug(' '.join(map(str, cmd)))
         res = run(cmd)
         if res.returncode > 0:
             yield Exception()
 
     logger.info('Checking syntax...')
-    cmd = [sys.executable, '-m', 'compileall', cfg]
+    cmd: list[str | Path] = [sys.executable, '-m', 'compileall', cfg]
     yield from check(cmd)
 
     # todo not sure if should be more defensive than check_call here
     logger.info('Checking type safety...')
     try:
         import mypy
     except ImportError:
@@ -261,26 +259,24 @@
         logger.info(f'OK, database exists: {db}')
 
     cmd = ['sqlite3', str(db), 'select src, COUNT(*) from visits GROUP BY src']
     logger.info(f'Querying database summary: {cmd}')
     check_call(cmd)
 
     bro = 'sqlitebrowser'
-    import shutil
     if not shutil.which(bro):
         logger.error(f'Install {bro} to inspect the database!')
         sys.exit(1)
     cmd = [bro, str(db)]
     logger.debug(f'Running {cmd}')
-    from .compat import Popen
     Popen(cmd)
 
 
 def cli_doctor_server(args: argparse.Namespace) -> None:
-    port = args.port
+    port: str = args.port
     endpoint = f'http://localhost:{port}/status'
     cmd = ['curl', endpoint]
     logger.info(f'Running {cmd}')
     check_call(cmd)
     print() # curl doesn't add newline
     logger.info('You should see the database path and version above!')
 
@@ -292,20 +288,19 @@
         pass
     return s
 
 
 def main() -> None:
     # TODO longer, literate description?
 
-    def add_index_args(parser: argparse.ArgumentParser, default_config_path: Optional[PathIsh]=None) -> None:
+    def add_index_args(parser: argparse.ArgumentParser, default_config_path: PathIsh | None = None) -> None:
         """
         :param default_config_path:
             if not given, all :func:`demo_sources()` are run
         """
-        register_argparse_extend_action_in_pre_py38(parser)
         parser.add_argument('--config', type=Path, default=default_config_path, help='Config path')
         parser.add_argument('--dry', action='store_true', help="Dry run, won't touch the database, only print the results out")
         parser.add_argument(
             '--sources',
             required=False,
             action="extend",
             nargs="+",
@@ -374,53 +369,54 @@
     sdp.add_parser('database', help='Inspect database').set_defaults(func=cli_doctor_db)
     sdps = sdp.add_parser('server'  , help='Check server'    )
     sdps.set_defaults(func=cli_doctor_server)
     add_port_arg(sdps)
 
     args = p.parse_args()
 
+    mode: str | None = args.mode
     # TODO is there a way to print full help? i.e. for all subparsers
-    if args.mode is None:
+    if mode is None:
         print('ERROR: Please specify a mode', file=sys.stderr)
         p.print_help(sys.stderr)
         sys.exit(1)
 
     logger.info("CLI args: %s", args)
 
     # TODO maybe, it's better for server to compute intermediate representations?
     # the only downside is storage. dunno.
     # worst case -- could use database?
 
     with get_tmpdir() as tdir: # TODO??
-        if args.mode == 'index':
+        if mode == 'index':
             do_index(
                 config_file=args.config,
                 dry=args.dry,
                 sources_subset=args.sources,
                 overwrite_db=args.overwrite,
             )
-        elif args.mode == 'serve':
+        elif mode == 'serve':
             server.run(args)
-        elif args.mode == 'demo':
+        elif mode == 'demo':
             # TODO not sure if 'as' is that useful
             # something like Telegram/Takeout is too hard to setup to justify adhoc mode like this?
             do_demo(
                 index_as=getattr(args, 'as'),
                 params=args.params,
                 port=args.port,
                 config_file=args.config,
                 dry=args.dry,
                 name=args.name,
                 sources_subset=args.sources,
                 overwrite_db=args.overwrite,
                 )
-        elif args.mode == 'install-server': # todo rename to 'autostart' or something?
+        elif mode == 'install-server': # todo rename to 'autostart' or something?
             install_server.install(args)
-        elif args.mode == 'config':
+        elif mode == 'config':
             args.func(args)
-        elif args.mode == 'doctor':
+        elif mode == 'doctor':
             args.func(args)
         else:
-            raise AssertionError(f'unexpected mode {args.mode}')
+            raise AssertionError(f'unexpected mode {mode}')
 
 if __name__ == '__main__':
     main()
```

### Comparing `promnesia-1.1.20230129/src/promnesia/cannon.py` & `promnesia-1.2.20230515/src/promnesia/cannon.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/common.py` & `promnesia-1.2.20230515/src/promnesia/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from collections.abc import Sized
+from __future__ import annotations
+
 from contextlib import contextmanager
 from datetime import datetime, date
-import os
-from typing import NamedTuple, Set, Iterable, Dict, TypeVar, Callable, List, Optional, Union, Any, Collection, Sequence, Tuple, TypeVar, TYPE_CHECKING
-from pathlib import Path
+from functools import lru_cache
 from glob import glob
 import itertools
-from more_itertools import intersperse
 import logging
-from functools import lru_cache
+import os
+from pathlib import Path
 import shutil
+from subprocess import run, PIPE, Popen
 from timeit import default_timer as timer
 from types import ModuleType
+from typing import NamedTuple, Iterable, TypeVar, Callable, List, Optional, Union, TypeVar
 import warnings
 
+from more_itertools import intersperse
 import pytz
 
 from .cannon import canonify
 
 
 _is_windows = os.name == 'nt'
 
@@ -73,15 +75,14 @@
     # TODO need some uniform way of string conversion
     # but generally, it will be
     # (url|file)(linenumber|json_path|anchor)
 
 @lru_cache(1)
 def _detect_mime_handler() -> str:
     def exists(what: str) -> bool:
-        from .compat import run, PIPE
         try:
             r = run(f'xdg-mime query default x-scheme-handler/{what}'.split(), stdout=PIPE)
         except FileNotFoundError:
             warnings.warn("No xdg-mime on your OS! If you're on OSX, perhaps you can help me! https://github.com/karlicoss/open-in-editor/issues/1")
             return False
         if r.returncode > 0:
             warnings.warn('xdg-mime failed') # hopefully rest is in stderr
@@ -187,15 +188,15 @@
     return logger
 
 
 
 import tempfile
 # kinda singleton
 @lru_cache(1)
-def get_tmpdir() -> tempfile.TemporaryDirectory:
+def get_tmpdir() -> tempfile.TemporaryDirectory[str]:
     # todo use appdirs?
     tdir = tempfile.TemporaryDirectory(suffix="promnesia")
     return tdir
 
 # TODO use mypy literal?
 Syntax = str
 
@@ -487,15 +488,14 @@
             # Remove dirs specified in ignore (clone dirs() as we have to remove in place)
             for i, d in enumerate(list(dirs)):
                 if d in ignore:
                     del dirs[i]
             yield from (Path(r) / f for f in files if f not in ignore)
         return
 
-    from .compat import Popen, PIPE
     cmd = ['find', *find_args(root, follow=follow, ignore=ignore)]
     # try to use fd.. it cooperates well with gitignore etc, also faster than find
     for x in ('fd', 'fd-find', 'fdfind'): # has different names on different dists..
         if shutil.which(x):
             cmd = [x, *fdfind_args(root, follow=follow, ignore=ignore)]
             break
     else:
@@ -574,15 +574,23 @@
         return cfg.absolute()
     else:
         return user_config_file()
     # TODO need to test this..
 
 
 @contextmanager
-def measure(tag: str='', *, logger, unit: str='ms'):
+def measure(tag: str='', *, logger: logging.Logger, unit: str='ms'):
     before = timer()
     yield lambda: timer() - before
     after = timer()
     secs = after - before
     mult = {'s': 1, 'ms': 10**3, 'us': 10**6}[unit]
     xx = secs * mult
     logger.debug(f'[{tag}]: {xx:.1f}{unit} elapsed')
+
+
+def is_sqlite_db(x: Path) -> bool:
+    return x.is_file() and mime(x) in {
+        'application/x-sqlite3',
+        'application/vnd.sqlite3',
+        # TODO this mime can also match wal files/journals, not sure
+    }
```

### Comparing `promnesia-1.1.20230129/src/promnesia/compare.py` & `promnesia-1.2.20230515/src/promnesia/compare.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/config.py` & `promnesia-1.2.20230515/src/promnesia/config.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/dump.py` & `promnesia-1.2.20230515/src/promnesia/dump.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/extract.py` & `promnesia-1.2.20230515/src/promnesia/extract.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/kjson.py` & `promnesia-1.2.20230515/src/promnesia/kjson.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/logging.py` & `promnesia-1.2.20230515/src/promnesia/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/usr/bin/env python3
 '''
-Default logger is a bit, see 'test'/run this file for a demo
+Default logger is a bit meh, see 'test'/run this file for a demo
 '''
 
 def test() -> None:
     import logging
     import sys
     from typing import Callable
-    M: Callable[[str], None]  = lambda s: print(s, file=sys.stderr)
+
+    M: Callable[[str], None] = lambda s: print(s, file=sys.stderr)
 
     M("   Logging module's defaults are not great...'")
     l = logging.getLogger('test_logger')
     l.error("For example, this should be logged as error. But it's not even formatted properly, doesn't have logger name or level")
 
     M("   The reason is that you need to remember to call basicConfig() first")
     logging.basicConfig()
     l.error("OK, this is better. But the default format kinda sucks, I prefer having timestamps and the file/line number")
 
     M("")
     M("    With LazyLogger you get a reasonable logging format, colours and other neat things")
 
-    ll = LazyLogger('test') # No need for basicConfig!
+    ll = LazyLogger('test')  # No need for basicConfig!
     ll.info("default level is INFO")
     ll.debug(".. so this shouldn't be displayed")
     ll.warning("warnings are easy to spot!")
     ll.exception(RuntimeError("exceptions as well"))
 
 
 import logging
@@ -33,39 +34,38 @@
 import warnings
 
 Level = int
 LevelIsh = Optional[Union[Level, str]]
 
 
 def mklevel(level: LevelIsh) -> Level:
-    # todo do the same for Promnesia?
-    # glevel = os.environ.get('HPI_LOGS', None)
-    # if glevel is not None:
-    #     level = glevel
+    # todo put in some global file, like envvars.py
+    glevel = os.environ.get('PROMNESIA_LOGS', None)
+    if glevel is not None:
+        level = glevel
     if level is None:
         return logging.NOTSET
     if isinstance(level, int):
         return level
     return getattr(logging, level.upper())
 
 
 FORMAT = '{start}[%(levelname)-7s %(asctime)s %(name)s %(filename)s:%(lineno)d]{end} %(message)s'
 FORMAT_COLOR   = FORMAT.format(start='%(color)s', end='%(end_color)s')
 FORMAT_NOCOLOR = FORMAT.format(start='', end='')
 DATEFMT = '%Y-%m-%d %H:%M:%S'
 
-# NOTE: this is a bit experimental and temporary..
 COLLAPSE_DEBUG_LOGS = os.environ.get('COLLAPSE_DEBUG_LOGS', False)
 
 _init_done = 'lazylogger_init_done'
 
 def setup_logger(logger: logging.Logger, level: LevelIsh) -> None:
     lvl = mklevel(level)
     try:
-        import logzero # type: ignore[import]
+        import logzero  # type: ignore[import]
         formatter = logzero.LogFormatter(
             fmt=FORMAT_COLOR,
             datefmt=DATEFMT,
         )
         use_logzero = True
     except ModuleNotFoundError:
         warnings.warn("You might want to install 'logzero' for nice colored logs!")
@@ -79,24 +79,24 @@
         return
 
     h = CollapseDebugHandler() if COLLAPSE_DEBUG_LOGS else logging.StreamHandler()
     logger.setLevel(lvl)
     h.setLevel(lvl)
     h.setFormatter(formatter)
     logger.addHandler(h)
-    logger.propagate = False # ugh. otherwise it duplicates log messages
+    logger.propagate = False  # ugh. otherwise it duplicates log messages? not sure about it..
 
 
 class LazyLogger(logging.Logger):
     def __new__(cls, name: str, level: LevelIsh = 'INFO') -> 'LazyLogger':
         logger = logging.getLogger(name)
 
         # this is called prior to all _log calls so makes sense to do it here?
         def isEnabledFor_lazyinit(*args, logger=logger, orig=logger.isEnabledFor, **kwargs) -> bool:
-            if not getattr(logger, _init_done, False):
+            if not getattr(logger, _init_done, False):  # init once, if necessary
                 setup_logger(logger, level=level)
                 setattr(logger, _init_done, True)
                 logger.isEnabledFor = orig # restore the callback
             return orig(*args, **kwargs)
 
         # oh god.. otherwise might go into an inf loop
         if not hasattr(logger, _init_done):
@@ -141,15 +141,15 @@
             else:
                 if self.last:
                     self.stream.write('\n') # clean up after the last debug line
             self.last = cur
             import os
             columns, _ = os.get_terminal_size(0)
             # ugh. the columns thing is meh. dunno I guess ultimately need curses for that
-            # TODO also would be cool to have a terminal post-processor? kinda like tail but aware of logging keyworkds (INFO/DEBUG/etc)
+            # TODO also would be cool to have a terminal post-processor? kinda like tail but aware of logging keywords (INFO/DEBUG/etc)
             self.stream.write(msg + ' ' * max(0, columns - len(msg)) + ('' if cur else '\n'))
             self.flush()
         except:
             self.handleError(record)
 
 
 if __name__ == '__main__':
```

### Comparing `promnesia-1.1.20230129/src/promnesia/misc/install_server.py` & `promnesia-1.2.20230515/src/promnesia/misc/install_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 import argparse
 import os
 import sys
 import time
 from pathlib import Path
 import platform
 from subprocess import check_call, run
@@ -46,15 +48,15 @@
                 <key>KeepAlive</key>
                 <true/>
         </dict>
 </plist>
 '''
 
 
-def systemd(*args, method=check_call):
+def systemd(*args: str | Path, method=check_call) -> None:
     method([
         'systemctl', '--no-pager', '--user', *args,
     ])
 
 
 def install_systemd(name: str, out: Path, launcher: str, largs: List[str]) -> None:
     unit_name = name
```

### Comparing `promnesia-1.1.20230129/src/promnesia/read_db.py` & `promnesia-1.2.20230515/src/promnesia/read_db.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/server.py` & `promnesia-1.2.20230515/src/promnesia/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/python3
+from __future__ import annotations
+
 __package__ = 'promnesia'  # ugh. hacky way to make wsgi runner work properly...
 
 import argparse
 from dataclasses import dataclass
-import os
-import json
 from datetime import timedelta
-from pathlib import Path
-import logging
 from functools import lru_cache
-from typing import List, NamedTuple, Dict, Optional, Any, Tuple
+import json
+import logging
+import os
+from pathlib import Path
+from typing import List, NamedTuple, Dict, Optional, Any, Tuple, Protocol
 
 
 import pytz
 from pytz import BaseTzInfo
 
 import fastapi
 
 from sqlalchemy import MetaData, exists, literal, between, or_, and_, exc, select
 from sqlalchemy import Column, Table, func, types
 from sqlalchemy.sql.elements import ColumnElement
 from sqlalchemy.sql import text
 
 
 from .common import PathWithMtime, DbVisit, Url, setup_logger, default_output_dir, get_system_tz
-from .compat import Protocol
 from .cannon import canonify
 
 
 Json = Dict[str, Any]
 
 app = fastapi.FastAPI()
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/auto.py` & `promnesia-1.2.20230515/src/promnesia/sources/auto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 - discovers files recursively
 - guesses the format (orgmode/markdown/json/etc) by the extension/MIME type
+- can index most of plaintext files, including source code!
+- autodetects Obsidian vault and adds `obsidian://` app protocol support [[file:../src/promnesia/sources/obsidian.py][promnesia.sources.obsidian]]
+- autodetects Logseq graph and adds `logseq://` app protocol support [[file:../src/promnesia/sources/logseq.py][promnesia.sources.logseq]]
 """
 
 import csv
 from concurrent.futures import ProcessPoolExecutor as Pool
 from contextlib import nullcontext
 from datetime import datetime
 import itertools
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/browser.py` & `promnesia-1.2.20230515/src/promnesia/sources/browser_legacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,29 @@
 from pathlib import Path
 from urllib.parse import unquote
 import sqlite3
 from typing import List, Set
 
 import pytz
 
-from ..common import PathIsh, Results, Visit, Loc, get_logger, Second, mime
+from ..common import PathIsh, Results, Visit, Loc, logger, Second, is_sqlite_db
 from .. import config
 
 # todo mcachew?
 from cachew import cachew
 
-logger = get_logger()
-
 
 def index(p: PathIsh) -> Results:
     pp = Path(p)
     assert pp.exists(), pp # just in case of broken symlinks
 
-    # is_file check because it also returns dirs
-    # TODO hmm, not sure what I meant here -- which dirs? behind symlinks?
-    is_db = lambda x: x.is_file() and mime(x) in {
-        'application/x-sqlite3',
-        'application/vnd.sqlite3',
-        # TODO this mime can also match wal files/journals, not sure
-    }
-
     # todo warn if filtered out too many?
     # todo wonder how quickly mimes can be computed?
     # todo ugh, dunno, maybe this really belongs to hpi?? need get_files etc...
-    dbs = [p for p in sorted(pp.rglob('*')) if is_db(p)]
+    dbs = [p for p in sorted(pp.rglob('*')) if is_sqlite_db(p)]
 
     assert len(dbs) > 0, pp
     logger.info('processing %d databases', len(dbs))
     cname = str('_'.join(pp.parts[1:])) # meh
     yield from _index_dbs(dbs, cachew_name=cname)
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/demo.py` & `promnesia-1.2.20230515/src/promnesia/sources/demo.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/fbmessenger.py` & `promnesia-1.2.20230515/src/promnesia/sources/fbmessenger.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/filetypes.py` & `promnesia-1.2.20230515/src/promnesia/sources/filetypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     'text/x-makefile',
     'text/troff',
     'text/x-asm',
     'text/x-objective-c',
     'text/x-lisp',
     'text/vnd.graphviz',
     'text/x-diff',  # patch files
+    'text/x-php',
 
     # these didn't have a mime type, or were mistyped?
     'css',
     'el',
     'rs',
     'go',
     'hs',  # mistyped on osx
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/github.py` & `promnesia-1.2.20230515/src/promnesia/sources/github.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/guess.py` & `promnesia-1.2.20230515/src/promnesia/sources/guess.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/hackernews.py` & `promnesia-1.2.20230515/src/promnesia/sources/hackernews.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 '''
-Uses [[https://github.com/karlicoss/HPI][HPI]] dogsheep module to import
-Hacker News items.
+Uses [[https://github.com/karlicoss/HPI][HPI]] dogsheep module to import HackerNews items.
 '''
 
 import textwrap
 
 from promnesia.common import Visit, Loc, Results
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/html.py` & `promnesia-1.2.20230515/src/promnesia/sources/html.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/hypothesis.py` & `promnesia-1.2.20230515/src/promnesia/sources/hypothesis.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/instapaper.py` & `promnesia-1.2.20230515/src/promnesia/sources/instapaper.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/markdown.py` & `promnesia-1.2.20230515/src/promnesia/sources/markdown.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/org.py` & `promnesia-1.2.20230515/src/promnesia/sources/org.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/plaintext.py` & `promnesia-1.2.20230515/src/promnesia/sources/plaintext.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/pocket.py` & `promnesia-1.2.20230515/src/promnesia/sources/pocket.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/reddit.py` & `promnesia-1.2.20230515/src/promnesia/sources/reddit.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/roamresearch.py` & `promnesia-1.2.20230515/src/promnesia/sources/roamresearch.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/rss.py` & `promnesia-1.2.20230515/src/promnesia/sources/rss.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+'''
+Uses [[https://github.com/karlicoss/HPI][HPI]] for RSS data.
+'''
+
 from itertools import chain
 
 from ..common import Visit, Loc, extract_urls, Results, get_logger
 
 from datetime import datetime
 
 import pytz
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/shellcmd.py` & `promnesia-1.2.20230515/src/promnesia/sources/shellcmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+"""
+Greps out URLs from an arbitrary shell command results.
+"""
+
 from datetime import datetime
 import os
 import re
-from typing import Optional, Union, Sequence
+from subprocess import run, PIPE
+from typing import Union, Sequence
 import warnings
 
-from ..compat import run, PIPE
 from ..common import Visit, Loc, Results, extract_urls, file_mtime, get_system_tz, now_tz, _is_windows, PathIsh
 from .plaintext import _has_grep
 
 
 def index(command: Union[str, Sequence[PathIsh]]) -> Results:
     cmd: Sequence[PathIsh]
     cmds: str
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/signal.py` & `promnesia-1.2.20230515/src/promnesia/sources/signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
-Harvest visits from Signal Desktop's chiphered SQLIite db(s).
+Collects visits from Signal Desktop's encrypted SQLIite db(s).
+"""
 
-Functions get their defaults from module-data.
+# Functions get their defaults from module-data.
+#
+# * Open-ciphered-db adapted from:
+#   https://github.com/carderne/signal-export/commit/2284c8f4
+# * Copyright (c) 2019 Chris Arderne, 2020 Kostis Anagnostopoulos
 
-* Open-ciphered-db adapted from:
-  https://github.com/carderne/signal-export/commit/2284c8f4
-* Copyright (c) 2019 Chris Arderne, 2020 Kostis Anagnostopoulos
-"""
 
 import json
 import logging
 import platform
 import sqlite3
 import subprocess as sbp
 from contextlib import contextmanager
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/smscalls.py` & `promnesia-1.2.20230515/src/promnesia/sources/smscalls.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,26 @@
 
 def index() -> Results:
     from . import hpi
     from my.smscalls import messages
 
     for m in messages():
 
+        if isinstance(m, Exception):
+            yield m
+            continue
+
         urls = extract_urls(m.message)
         if len(urls) == 0:
             continue
 
-        loc = Loc(title=f"SMS with {m.who} ({m.phone_number})")
+        if m.who is None:
+            loc = Loc(title=f"SMS with {m.phone_number}")
+        else:
+            loc = Loc(title=f"SMS with {m.who} ({m.phone_number})")
 
         for u in urls:
             yield Visit(
                 url=u,
                 dt=m.dt,
                 context=m.message,
                 locator=loc,
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/stackexchange.py` & `promnesia-1.2.20230515/src/promnesia/sources/stackexchange.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/takeout_legacy.py` & `promnesia-1.2.20230515/src/promnesia/sources/takeout_legacy.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/telegram.py` & `promnesia-1.2.20230515/src/promnesia/sources/telegram_legacy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 '''
 Uses [[https://github.com/fabianonline/telegram_backup#readme][telegram_backup]] database for messages data
 '''
 
 from pathlib import Path
+import sqlite3
 from textwrap import dedent
-from typing import Optional, Union, TypeVar
+from typing import Union, TypeVar
 from urllib.parse import unquote # TODO mm, make it easier to rememember to use...
 
 from ..common import PathIsh, Visit, get_logger, Loc, extract_urls, from_epoch, Results, echain
-
-# TODO potentially, belongs to my. package
+from ..sqlite import sqlite_connection
 
 T = TypeVar("T")
 
 
 def unwrap(res: Union[T, Exception]) -> T:
     if isinstance(res, Exception):
         raise res
     else:
         return res
 
 
-# TODO move to common?
-def dataset_readonly(db: Path):
-    import dataset # type: ignore
-    # see https://github.com/pudo/dataset/issues/136#issuecomment-128693122
-    import sqlite3
-    creator = lambda: sqlite3.connect(f'file:{db}?immutable=1', uri=True)
-    return dataset.connect('sqlite:///' , engine_kwargs={'creator': creator})
-
-
 def index(database: PathIsh, *, http_only: bool=False) -> Results:
     """
     :param database:
         the path of the sqlite generated by the _telegram_backup_ java program
     :param http_only:
         when true, do not collect IP-addresses and `python.py` strings
     """
     logger = get_logger()
 
     path = Path(database)
-    assert path.is_file(), path # TODO could check is_file inside `dataset_readonly()`
+    assert path.is_file(), path
 
     def make_query(text_query: str) -> str:
         extra_criteria = "AND (M.has_media == 1 OR text LIKE '%http%')" if http_only else ""
         return dedent(
             f"""
             WITH entities AS (
             SELECT 'dialog' as type
@@ -61,48 +52,46 @@
                 , coalesce(name, id) as display_name FROM chats
             )
             SELECT src.display_name AS chatname
                 , src.handle       AS chat
                 , snd.display_name AS sender
                 , M.time           AS time
                 , {text_query}     AS text
-                , M.id             AS mid
+                , M.message_id     AS mid
             FROM messages AS M
                                                                                 /* chat types are 'dialog' (1-1), 'group' and 'supergroup' */
                                                                                 /* this is abit hacky way to handle all groups in one go */
             LEFT JOIN entities AS src    ON M.source_id = src.id AND src.type = (CASE M.source_type WHEN 'supergroup' THEN 'group' ELSE M.source_type END)
             LEFT JOIN entities AS snd    ON M.sender_id = snd.id AND snd.type = 'dialog'
             WHERE
                 M.message_type NOT IN ('service_message', 'empty_message')
                 {extra_criteria}
             ORDER BY time;
             """)
 
-    # TODO context manager?
-    with dataset_readonly(path) as db:
-
+    with sqlite_connection(path, immutable=True, row_factory='row') as db:
         # TODO yield error if chatname or chat or smth else is null?
-        for row in db.query(make_query('M.text')):
+        for row in db.execute(make_query('M.text')):
             try:
                 yield from _handle_row(row)
             except Exception as ex:
                 yield echain(RuntimeError(f'While handling {row}'), ex)
-                # , None, sys.exc_info()[2]
-                # TODO hmm. traceback isn't preserved; wonder if that's because it's too heavy to attach to every single exception object..
 
         # old (also 'stable') version doesn't have 'json' column yet...
-        if 'json' in db['messages'].columns:
-            for row in db.query(make_query("json_extract(json, '$.media.webpage.description')")):
+        messages_columns = [d[0] for d in db.execute('SELECT * FROM messages').description]
+        # todo hmm what is 'markup_json'??
+        if 'json' in messages_columns:
+            for row in db.execute(make_query("json_extract(json, '$.media.webpage.description')")):
                 try:
                     yield from _handle_row(row)
                 except Exception as ex:
                     yield echain(RuntimeError(f'While handling {row}'), ex)
 
 
-def _handle_row(row) -> Results:
+def _handle_row(row: sqlite3.Row) -> Results:
     text = row['text']
     if text is None:
         return
     urls = extract_urls(text)
     if len(urls) == 0:
         return
     dt            = from_epoch(row['time'])
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/twitter.py` & `promnesia-1.2.20230515/src/promnesia/sources/twitter.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/vcs.py` & `promnesia-1.2.20230515/src/promnesia/sources/vcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
 Clones & indexes Git repositories (via sources.auto)
 '''
 # TODO not sure if worth exposing... could be just handled by auto or something?)
 
 from pathlib import Path
 import re
+from subprocess import check_call
 from typing import Iterable
 
 from ..common import Extraction, PathIsh, get_tmpdir, slugify
-from ..compat import check_call
 
 
 def index(path: PathIsh, *args, **kwargs) -> Iterable[Extraction]:
     repo = str(path)
 
     # TODO this looks pretty horrible as a context name
     # perhaps pass context here since we know it should be github repo?
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/viber.py` & `promnesia-1.2.20230515/src/promnesia/sources/viber.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
-Adapted from `telegram.py` to read from `~/.ViberPC/XYZ123/viber.db`
+Collects visits from Viber desktop app (e.g. `~/.ViberPC/XYZ123/viber.db`)
 """
 
 import logging
 import textwrap
 from os import PathLike
 from pathlib import Path
+import sqlite3
 from typing import Iterable, Optional
 
 from ..common import Loc, PathIsh, Results, Visit, extract_urls, from_epoch, join_tags
+from ..sqlite import sqlite_connection
 
 
 logger = logging.getLogger(__name__)
 
 
 def index(
     db_path: PathIsh = "~/.ViberPC/*/viber.db",
@@ -33,25 +35,14 @@
     msgs_query = messages_query(http_only)
 
     for db_path in _get_files(db_path):
         assert db_path.is_file(), f"Is it a (Viber-desktop sqlite) file? {db_path}"
         yield from _harvest_db(db_path, msgs_query, locator_schema)
 
 
-# TODO move to common?
-def _dataset_readonly(db: Path):
-    # see https://github.com/pudo/dataset/issues/136#issuecomment-128693122
-    import sqlite3
-
-    import dataset  # type: ignore
-
-    creator = lambda: sqlite3.connect(f"file:{db}?immutable=1", uri=True)
-    return dataset.connect("sqlite:///", engine_kwargs={"creator": creator})
-
-
 def messages_query(http_only: Optional[bool]) -> str:
     """
     An SQL-query returning 1 row for each message
 
     A non-private method, to facilitate experimentation.
     """
     extra_criteria = "AND text LIKE '%http%'" if http_only else ""
@@ -114,15 +105,15 @@
             AND text IS NOT NULL
             {extra_criteria}
         ORDER BY time;
         """
     )
 
 
-def _handle_row(row: dict, db_path: PathLike, locator_schema: str) -> Results:
+def _handle_row(row: sqlite3.Row, db_path: PathLike, locator_schema: str) -> Results:
     text = row["text"]
     urls = extract_urls(text)
     if not urls:
         return
 
     dt = from_epoch(row["time"] // 1000)  # timestamps are stored x100 this db
     mid: str = row["mid"]
@@ -169,16 +160,16 @@
 def _harvest_db(db_path: PathIsh, msgs_query: str, locator_schema: str) -> Results:
     is_debug = logger.isEnabledFor(logging.DEBUG)
 
     # Note: for displaying maybe better not to expand/absolute,
     # but it's safer for debugging resolved.
     db_path = Path(db_path).resolve()
 
-    with _dataset_readonly(db_path) as db:
-        for row in db.query(msgs_query):
+    with sqlite_connection(db_path, immutable=True, row_factory='row') as db:
+        for row in db.execute(msgs_query):
             try:
                 yield from _handle_row(row, db_path, locator_schema)
             except Exception as ex:
                 # TODO: also insert errors in db
                 logger.warning(
                     "Cannot extract row: %s, due to: %s(%s)",
                     row,
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/website.py` & `promnesia-1.2.20230515/src/promnesia/sources/website.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 Clones a website with wget and indexes via sources.auto
 '''
 
 from pathlib import Path
 import re
-from ..compat import check_call, run
+from subprocess import run
 from typing import Iterable
 
 from ..common import Extraction, PathIsh, get_tmpdir, slugify, get_logger
 
 
 def index(path: PathIsh, *args, **kwargs) -> Iterable[Extraction]:
     logger = get_logger()
```

### Comparing `promnesia-1.1.20230129/src/promnesia/sources/zulip.py` & `promnesia-1.2.20230515/src/promnesia/sources/zulip.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/src/promnesia.egg-info/SOURCES.txt` & `promnesia-1.2.20230515/src/promnesia.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 extension/.eslintrc.js
 extension/.flowconfig
 extension/MANUAL-TESTS.org
 extension/TODO.org
 extension/babel.config.js
 extension/build
 extension/jest.config.js
+extension/package-lock.json
 extension/package.json
 extension/webpack.config.js
 extension/.ci/build
 extension/__mocks__/dom-form-serializer.js
 extension/flow-typed/webextension-polyfill.js
 extension/images/generate
 extension/images/ic_blacklisted_48.png
@@ -95,14 +96,15 @@
 src/promnesia/dump.py
 src/promnesia/extract.py
 src/promnesia/kjson.py
 src/promnesia/logging.py
 src/promnesia/py.typed
 src/promnesia/read_db.py
 src/promnesia/server.py
+src/promnesia/sqlite.py
 src/promnesia.egg-info/PKG-INFO
 src/promnesia.egg-info/SOURCES.txt
 src/promnesia.egg-info/dependency_links.txt
 src/promnesia.egg-info/entry_points.txt
 src/promnesia.egg-info/not-zip-safe
 src/promnesia.egg-info/requires.txt
 src/promnesia.egg-info/top_level.txt
@@ -110,14 +112,15 @@
 src/promnesia/misc/config_example.py
 src/promnesia/misc/install_server.py
 src/promnesia/sources/__init__.pyi
 src/promnesia/sources/auto.py
 src/promnesia/sources/auto_logseq.py
 src/promnesia/sources/auto_obsidian.py
 src/promnesia/sources/browser.py
+src/promnesia/sources/browser_legacy.py
 src/promnesia/sources/demo.py
 src/promnesia/sources/fbmessenger.py
 src/promnesia/sources/filetypes.py
 src/promnesia/sources/github.py
 src/promnesia/sources/guess.py
 src/promnesia/sources/hackernews.py
 src/promnesia/sources/hpi.py
@@ -134,14 +137,15 @@
 src/promnesia/sources/shellcmd.py
 src/promnesia/sources/signal.py
 src/promnesia/sources/smscalls.py
 src/promnesia/sources/stackexchange.py
 src/promnesia/sources/takeout.py
 src/promnesia/sources/takeout_legacy.py
 src/promnesia/sources/telegram.py
+src/promnesia/sources/telegram_legacy.py
 src/promnesia/sources/twitter.py
 src/promnesia/sources/vcs.py
 src/promnesia/sources/viber.py
 src/promnesia/sources/website.py
 src/promnesia/sources/zulip.py
 tests/browser_helper.py
 tests/cannon.py
```

### Comparing `promnesia-1.1.20230129/tests/browser_helper.py` & `promnesia-1.2.20230515/tests/browser_helper.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/cannon.py` & `promnesia-1.2.20230515/tests/cannon.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/cli.py` & `promnesia-1.2.20230515/tests/cli.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/common.py` & `promnesia-1.2.20230515/tests/common.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/config_tests.py` & `promnesia-1.2.20230515/tests/config_tests.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/convert_screencast.py` & `promnesia-1.2.20230515/tests/convert_screencast.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/demos.py` & `promnesia-1.2.20230515/tests/demos.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/end2end_test.py` & `promnesia-1.2.20230515/tests/end2end_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from datetime import datetime
 from tempfile import TemporaryDirectory
 import os
 import shutil
 from subprocess import check_call, check_output
 from time import sleep
-from typing import NamedTuple, Optional, Iterator, TypeVar, Callable, Sequence, Union
+from typing import NamedTuple, Optional, Iterator, TypeVar, Callable, Sequence, Union, Dict, Any
 
 import pytest # type: ignore
 
 if __name__ == '__main__':
     # TODO ugh need to figure out PATH
     # python3 -m pytest -s tests/server_test.py::test_query
     pytest.main(['-s', __file__])
@@ -22,14 +22,15 @@
 
 from selenium import webdriver
 from selenium.webdriver import Remote as Driver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.alert import Alert
+from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support.ui import WebDriverWait as Wait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import NoAlertPresentException, NoSuchFrameException, TimeoutException
 
 
 from common import under_ci, uses_x, has_x, local_http_server
 from integration_test import index_hypothesis, index_local_chrome, index_urls
@@ -110,14 +111,17 @@
 
 def _get_webdriver(tdir: Path, browser: Browser, extension: bool=True) -> Driver:
     addon = get_addon_path(kind=browser.dist)
     driver: Driver
     if browser.name == 'firefox':
         ff_options = webdriver.FirefoxOptions()
         ff_options.set_preference('profile', str(tdir))
+        # todo remove when webdriver is updated
+        # see https://github.com/mozilla/geckodriver/issues/2075
+        ff_options.set_preference('fission.autostart', True)
         ff_options.headless = browser.headless
         # use firefox from here to test https://www.mozilla.org/en-GB/firefox/developer/
         driver = webdriver.Firefox(options=ff_options)
         # todo pass firefox-dev binary?
         if extension:
             driver.install_addon(str(addon), temporary=True)
     elif browser.name == 'chrome':
@@ -131,15 +135,33 @@
             if 'UNDER_DOCKER' in os.environ:
                 # docker runs as root and chrome refuses to use headless in that case
                 cr_options.add_argument('--no-sandbox')
 
             # regular --headless doesn't support extensions for some reason
             cr_options.add_argument('--headless=new')
         cr_options.add_extension(str(ex))
-        driver = webdriver.Chrome(options=cr_options)
+
+        # right, so recent chrome/chromium have this regression https://bugs.chromium.org/p/chromedriver/issues/detail?id=4440
+        # which breaks tons of tests due to iframe use
+        use_custom_chromium = True
+        mexepath: Dict[str, Any] = {}
+        if use_custom_chromium:
+            # see setup in end2end_tests.Dockerfile
+            user_data_dir = tdir / 'udir'
+            user_data_dir.mkdir()
+            # seems necessary, otherwise it somehow falls back onto snap chromium and gets stuck?
+            cr_options.add_argument('--user-data-dir=' + str(user_data_dir))
+            # ugh. sadly somehow if you add these chrome dirs to PATH, it doesn't work it still tries to use system binary?
+
+            cr_options.binary_location = '/tmp/chrome/chrome-linux/chrome'
+            driver_path = Path('/tmp/chrome/chromedriver_linux64/chromedriver')
+            assert driver_path.exists()
+            mexepath['executable_path'] = str(driver_path)
+        driver = webdriver.Chrome(options=cr_options, **mexepath)
+        logger.info(f"using webdriver: {driver.capabilities['browserVersion']} {driver.capabilities['chrome']['chromedriverVersion']}")
     else:
         raise RuntimeError(f'Unexpected browser {browser}')
     return driver
 
 
 # TODO copy paste from grasp
 @contextmanager
@@ -407,27 +429,33 @@
     def filters(self) -> list[WebElement]:
         # TODO hmm this only works within sidebar frame context
         # but if we add with self.ctx() here, it seems unhappy with enterinng the context twice
         # do something about it later..
         outer = self.driver.find_element(By.ID, 'promnesia-sidebar-filters')
         return outer.find_elements(By.CLASS_NAME, 'src')
 
-
     @property
     def visits(self) -> list[WebElement]:
         return self.driver.find_elements(By.XPATH, '//*[@id="visits"]/li')
 
     def trigger_search(self) -> None:
         # this should be the window with extension
         cur_window_handles = self.driver.window_handles
         with self.ctx():
-            search_button = self.driver.find_element(By.ID, 'button-search')
-            search_button.click()
+            self.driver.find_element(By.ID, 'button-search').click()
             self.helper.wait_for_search_tab(cur_window_handles)
 
+    def trigger_mark_visited(self) -> None:
+        with self.ctx():
+            self.driver.find_element(By.ID, 'button-mark').click()
+
+    def trigger_close(self) -> None:
+        with self.ctx():
+            self.driver.find_element(By.ID, 'button-close').click()
+
 
 class OptionsPage(NamedTuple):
     driver: Driver
     helper: 'TestHelper'
 
     def set_position(self, settings: str) -> None:
         field = self.driver.find_element(By.XPATH, '//*[@id="position_css_id"]')
@@ -482,15 +510,14 @@
         self.open_page('search.html' + query)
 
         Wait(self.driver, timeout=10).until(
             EC.presence_of_element_located((By.ID, 'visits')),
         )
 
     def move_to(self, element) -> None:
-        from selenium.webdriver.common.action_chains import ActionChains
         ActionChains(self.driver).move_to_element(element).perform()
 
     def switch_to_sidebar(self, wait: Union[bool, int]=False, *, wait2: bool=True) -> None:
         raise RuntimeError('not used anymore, use with helper.sidebar instead!')
 
     @property
     def sidebar(self) -> Sidebar:
@@ -567,14 +594,15 @@
 - if running in headless mode, will automatically assume 'yes'.
   of course it's not very robust, but at least we're testing some codepaths then
 '''
 manual = Interactive() if has_x() else Headless()
 
 
 # TODO deprecate this in favor of run_server
+# still used in demos.py..
 @contextmanager
 def _test_helper(tmp_path: Path, indexer: Callable[[Path], None], test_url: Optional[str], browser: Browser, **kwargs) -> Iterator[TestHelper]:
     tdir = Path(tmp_path)
 
     indexer(tdir)
     with wserver(db=tdir / 'promnesia.sqlite') as srv, get_webdriver(browser=browser) as driver:
         port = srv.port
@@ -846,34 +874,36 @@
 
         manual.confirm('you should see search results, "anthrocidal" should be highlighted red')
         # FIXME test clicking search around in actual search page.. it didn't work, seemingly because of initBackground() handling??
 
 
 # TODO skip if not my hostname
 @uses_x
-@browsers(FF, CH)
+@browsers()
 def test_chrome_visits(tmp_path: Path, browser: Browser) -> None:
     pytest.skip('TODO hmm seems that this file is gone now? not sure if a good test anyway')
     test_url = "https://en.wikipedia.org/wiki/Amplituhedron"
     test_url = "https://en.wikipedia.org/wiki/Symplectic_vector_space"
-    with _test_helper(tmp_path, index_local_chrome, test_url, browser=browser) as helper:
+    with _test_helper(tmp_path, index_local_chrome, test_url, browser=browser) as helper:  # type: ignore
         trigger_command(helper.driver, Command.ACTIVATE)
         confirm("You shoud see chrome visits now; with time spent")
 
 
 @browsers()
 def test_show_visited_marks(tmp_path: Path, driver: Driver) -> None:
     visited = {
         'https://en.wikipedia.org/wiki/Special_linear_group': None,
         'http://en.wikipedia.org/wiki/Unitary_group'        : None,
         'en.wikipedia.org/wiki/Transpose'                   : None,
     }
     test_url = "https://en.wikipedia.org/wiki/Symplectic_group"
     with run_server(tmp_path=tmp_path, indexer=index_urls(visited), driver=driver, show_dots=False) as helper:
         driver.get(test_url)
+
+        sleep(2)  # hmm not sure why it's necessary, but often fails headless firefox otherwise
         helper.mark_visited()
         sleep(1)  # marks are async, wait till it marks
 
         slg = driver.find_elements(By.XPATH, '//a[contains(@href, "/wiki/Special_linear_group")]')
         assert len(slg) > 0
         for s in slg:
             assert 'promnesia-visited' in s.get_attribute('class')
@@ -955,22 +985,20 @@
         helper.search()
         # TODO actually search something?
         # TODO use current domain as default? or 'parent' url?
         confirm("You shoud see search prompt now, with focus on search field")
 
 
 @browsers()
-def test_new_background_tab(tmp_path: Path, browser: Browser) -> None:
+def test_new_background_tab(tmp_path: Path, driver: Driver) -> None:
     start_url = "http://www.e-flux.com/journal/53/59883/the-black-stack/"
     # bg_url_text = "El Proceso (The Process)"
     # TODO generate some fake data instead?
-    with _test_helper(
-            tmp_path, index_hypothesis, start_url, browser=browser,
-            notify_contexts=True,
-    ) as helper:
+    with run_server(tmp_path=tmp_path, indexer=index_hypothesis, driver=driver, notify_contexts=True) as helper:
+        driver.get(start_url)
         manual.confirm('you should see notification about contexts')
         page_logo = helper.driver.find_element(By.XPATH, '//a[@class="page-logo"]')
         page_logo.send_keys(Keys.CONTROL + Keys.ENTER) # ctrl+click -- opens the link in new background tab
         manual.confirm('you should not see any new notifications')
         # TODO switch to new tab?
         # TODO https://www.e-flux.com/journal/53/
 
@@ -1084,76 +1112,79 @@
 
         # check that still can interact with the sidebar
         helper.sidebar.close()
         confirm('green icon, sidebar is closed')
 
 
 @browsers()
-def test_unreachable(tmp_path: Path, browser: Browser) -> None:
+def test_unreachable(tmp_path: Path, driver: Driver) -> None:
+    pytest.skip("NOTE: broken at the moment because webNavigation.onCompleted isn't working for unreachable pages")
+
     url = 'https://somenonexist1ngurl.com'
     urls = {
         url: 'some context',
     }
-    with _test_helper(
-            tmp_path, index_urls(urls), 'about:blank', browser=browser,
+    indexer = index_urls(urls)
+    with run_server(
+            tmp_path=tmp_path, indexer=indexer, driver=driver,
             notify_contexts=True,
             verbose_errors=False,
     ) as helper:
         try:
-            helper.driver.get(url)
+            driver.get(url)
         except:
             # results in exception because it's unreachable
             pass
-        # TODO maybe in this case it could instead open the sidebar in a separate tab?
         manual.confirm('green icon, no errors, desktop notification with contexts')
 
 
 @browsers()
-def test_stress(tmp_path: Path, browser: Browser) -> None:
+def test_stress(tmp_path: Path, driver: Driver) -> None:
     url = 'https://www.reddit.com/'
     urls = [
         (f'{url}/subpath/{i}.html', f'context {i}' if i > 10000 else None) for i in range(50000)
     ]
-    with _test_helper(tmp_path, index_urls(urls), url, browser=browser) as helper:
-        if has_x():
-            helper.activate()
+    indexer = index_urls(urls)
+    with run_server(tmp_path=tmp_path, indexer=indexer, driver=driver) as helper:
+        driver.get(url)
 
+        helper.activate()
+
+        # todo I guess it's kinda tricky to test in headless webdriver
         manual.confirm('''
 Is performance reasonable?
 The sidebar should show up, and update gradually.
 You should be able to scroll the page, trigger tooltips, etc., without any lags.
 '''.strip())
 
     
-@browsers(FF, CH)
-def test_fuzz(tmp_path: Path, browser: Browser) -> None:
+@browsers()
+def test_fuzz(tmp_path: Path, driver: Driver) -> None:
     # TODO ugh. this still results in 'tab permissions' pages, but perhaps because of closed tabs?
     # dunno if it's worth fixing..
     urls = {
         'https://www.iana.org/domains/reserved': 'IANA',
         'iana.org/domains/reserved': 'IANA2',
     }
-    with _test_helper(
-            tmp_path,
-            index_urls(urls),
-            'https://example.com',
-            browser=browser,
-            notify_contexts=True,
-    ) as helper:
-        driver = helper.driver
+    indexer = index_urls(urls)
+    with run_server(tmp_path=tmp_path, indexer=indexer, driver=driver, notify_contexts=True) as helper:
+        driver.get('https://example.com')
         tabs = 30
         for _ in range(tabs):
             driver.find_element(By.TAG_NAME, 'a').send_keys(Keys.CONTROL + Keys.RETURN)
 
         sleep(5)
         for _ in range(tabs - 2):
             driver.close()
             sleep(0.1)
             driver.switch_to.window(driver.window_handles[0])
 
+        if is_headless(driver):
+            pytest.skip("Rest of this test uses send_key to restore tab and it's not working under headless webdriver :(")
+
         def cb():
             for _ in range(10):
                 send_key('Ctrl+Shift+t')  # restore tabs
                 sleep(0.1)
         trigger_callback(driver, cb)
         confirm("shouldn't result in 'unexpected error occured'; show only show single notification per page")
 
@@ -1193,14 +1224,40 @@
 # (anonymous) @ VM2056 notifications.js:49
 # VM2056 notifications.js:17 Uncaught (in promise) TypeError: Cannot read property 'create' of undefined
 #     at notify (VM2056 notifications.js:17)
 #     at notifyError (VM2056 notifications.js:41)
 
 
 @browsers()
+def test_showvisits_popup(tmp_path: Path, driver: Driver) -> None:
+    url = 'https://www.iana.org/'
+    indexer = index_urls([
+        ('https://www.iana.org/abuse', 'some comment'),
+    ])
+    with run_server(tmp_path=tmp_path, indexer=indexer, driver=driver, notify_contexts=True, show_dots=True) as helper:
+        driver.get(url)
+        # todo might need to wait until marks are shown?
+        link_with_popup = driver.find_elements(By.XPATH, '//a[@href = "/abuse"]')[0]
+
+        # wait till visited marks appear
+        Wait(driver, timeout=5).until(
+            EC.presence_of_element_located((By.CLASS_NAME, 'promnesia-visited')),
+        )
+        helper.move_to(link_with_popup)  # hover over visited mark
+        # meh, but might need some time to render..
+        popup = Wait(driver, timeout=5).until(
+            EC.presence_of_element_located((By.CLASS_NAME, 'context')),
+        )
+        sleep(3)  #  text might take some time to render too..
+        assert popup.text == 'some comment'
+
+        assert is_visible(driver, popup)
+
+
+@browsers()
 def test_multiple_page_updates(tmp_path: Path, driver: Driver) -> None:
     # on some pages, onUpdated is triggered multiple times (because of iframes or perhaps something else??)
     # which previously resulted in flickering sidebar/performance degradation etc, so it's a regression test against this
     # TODO would be nice to hook to the backend and check how many requests it had...
     url = 'https://github.com/karlicoss/promnesia/projects/1'
     indexer = index_urls([
         ('https://github.com/karlicoss/promnesia', 'some comment'),
@@ -1218,29 +1275,19 @@
             assert len(toasts) <= 1
             sleep(0.1)
         assert had_toast
 
         helper._sidebar.open()
         helper._sidebar.close()
 
-        xpath = '//a[@href = "https://github.com/karlicoss/promnesia"]'
+        xpath = '//a[@href = "/karlicoss/promnesia"]'
         links_to_mark = driver.find_elements(By.XPATH, xpath)
         assert len(links_to_mark) > 2  # sanity check
         for l in links_to_mark:
             assert 'promnesia-visited' in l.get_attribute('class')
             # TODO would be nice to test clicking on them...
 
-        # meh...
-        header_link = driver.find_elements(By.XPATH, '//a[text() = "promnesia" and @href = "/karlicoss/promnesia"]')[0]
-        # hmm a bit crap, but works!!
-        header_link.find_element(By.XPATH, './../..').find_element(By.CLASS_NAME, 'promnesia-visited-toggler').click()
-
-        popup = driver.find_element(By.CLASS_NAME, 'context')
-        assert popup.text == 'some comment'
-
-        assert is_visible(driver, popup)
-
 
 # TODO FIXME need to test racey conditions _while_ page is loading, results in this 'unexpected error occured'?
 
 
 # TODO shit, sometimes I have 'bindSidebarData is not defined'? with vebose errors on demo_how_did_i_get_here
```

### Comparing `promnesia-1.1.20230129/tests/imports.py` & `promnesia-1.2.20230515/tests/imports.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/indexer_test.py` & `promnesia-1.2.20230515/tests/indexer_test.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/install_and_run` & `promnesia-1.2.20230515/tests/install_and_run`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/integration_test.py` & `promnesia-1.2.20230515/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/record.py` & `promnesia-1.2.20230515/tests/record.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/server_test.py` & `promnesia-1.2.20230515/tests/server_test.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/test_auto_indexer.py` & `promnesia-1.2.20230515/tests/test_auto_indexer.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/test_misc.py` & `promnesia-1.2.20230515/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/test_org_indexer.py` & `promnesia-1.2.20230515/tests/test_org_indexer.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/test_traverse.py` & `promnesia-1.2.20230515/tests/test_traverse.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/testdata/auto/orgs/file.org` & `promnesia-1.2.20230515/tests/testdata/auto/orgs/file.org`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/testdata/auto/orgs/file3.org` & `promnesia-1.2.20230515/tests/testdata/auto/orgs/file3.org`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/testdata/auto/pocket.json` & `promnesia-1.2.20230515/tests/testdata/auto/pocket.json`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/testdata/normalise/ff.txt` & `promnesia-1.2.20230515/tests/testdata/normalise/ff.txt`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/testdata/takeout/Takeout/My Activity/Chrome/MyActivity.html` & `promnesia-1.2.20230515/tests/testdata/takeout/Takeout/My Activity/Chrome/MyActivity.html`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/testdata/takeout-20150518T000000Z.zip` & `promnesia-1.2.20230515/tests/testdata/takeout-20150518T000000Z.zip`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/testdata/test_config.py` & `promnesia-1.2.20230515/tests/testdata/test_config.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tests/webdriver_utils.py` & `promnesia-1.2.20230515/tests/webdriver_utils.py`

 * *Files identical despite different names*

### Comparing `promnesia-1.1.20230129/tox.ini` & `promnesia-1.2.20230515/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     hpi module install my.github.ghexport
     hpi module install my.hypothesis
     hpi module install my.instapaper
     hpi module install my.pocket
     hpi module install my.reddit
     hpi module install my.fbmessenger
     hpi module install my.google.takeout.parser
+    hpi module install my.browser.export
 
     {envpython} -m mypy --install-types --non-interactive \
                    -p promnesia.sources \
                    # txt report is a bit more convenient to view on CI
                    --txt-report  .coverage.mypy-misc \
                    --html-report .coverage.mypy-misc \
                    {posargs}
```

