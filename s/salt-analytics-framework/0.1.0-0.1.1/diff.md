# Comparing `tmp/salt-analytics-framework-0.1.0.tar.gz` & `tmp/salt-analytics-framework-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Apr 28 21:37:58 2023, max compression
+gzip compressed data, last modified: Mon May 15 13:23:45 2023, max compression
```

## Comparing `salt-analytics-framework-0.1.0.tar` & `salt-analytics-framework-0.1.1.tar`

### file list

```diff
@@ -1,157 +1,159 @@
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.bandit
--rw-r--r--   0 root         (0) root         (0)      684 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/
--rw-r--r--   0 root         (0) root         (0)      229 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/actionlint.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/actions/setup-actionlint/
--rw-r--r--   0 root         (0) root         (0)      892 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/actions/setup-actionlint/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      995 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     7134 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     7030 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     4609 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/check-changelog-entries.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/copyright-headers.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 root         (0) root         (0)      579 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/sort-pylint-spelling-words.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pylint-spelling-words
--rw-r--r--   0 root         (0) root         (0)    19414 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      427 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     5256 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2487 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     9283 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3046 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1861 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/changelog/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/changelog/_template.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/_static/.gitkeep
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/all.rst
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6553 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/contents.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/modules.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.collect.rst
--rw-r--r--   0 root         (0) root         (0)      557 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.forward.rst
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.process.rst
--rw-r--r--   0 root         (0) root         (0)      861 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.rst
--rw-r--r--   0 root         (0) root         (0)      346 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.saltext.engines.rst
--rw-r--r--   0 root         (0) root         (0)      202 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.saltext.rst
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.utils.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    23817 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/docs-auto.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)     3170 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      198 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/beacons.py
--rw-r--r--   0 root         (0) root         (0)     5145 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/logs.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/noop.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/salt_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1560 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/disk.py
--rw-r--r--   0 root         (0) root         (0)      834 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/noop.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/test.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/manager.py
--rw-r--r--   0 root         (0) root         (0)     9649 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/models.py
--rw-r--r--   0 root         (0) root         (0)     5687 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)      845 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/noop.py
--rw-r--r--   0 root         (0) root         (0)     3095 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/regex_mask.py
--rw-r--r--   0 root         (0) root         (0)     4590 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/shannon_mask.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/engines/analytics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/utils/dt.py
--rw-r--r--   0 root         (0) root         (0)     5726 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/utils/eventbus.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3046 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3573 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      382 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      584 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/forwarders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/forwarders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2303 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/forwarders/test_concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/test_disabled_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/test_enabled_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_memusage.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/test_logs.py
--rw-r--r--   0 root         (0) root         (0)     3388 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/test_logs_with_parse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_arg.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_collatz.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_config_get.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/engines/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/process/test_regex_mask.py
--rw-r--r--   0 root         (0) root         (0)     5436 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/process/test_shannon_mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/salt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/salt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/salt/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/salt/engines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tools/
--rw-r--r--   0 root         (0) root         (0)      290 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tools/pre_commit.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tools/pre_commit.py~
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.bandit
+-rw-r--r--   0 root         (0) root         (0)      684 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/actionlint.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/actions/setup-actionlint/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/actions/setup-actionlint/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)    10391 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3571 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/check-changelog-entries.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/copyright-headers.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/make-autodocs.py
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/sort-pylint-spelling-words.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pylint-spelling-words
+-rw-r--r--   0 root         (0) root         (0)      967 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     9283 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/changelog/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/changelog/_template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/_static/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/all.rst
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/contents.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/modules.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.collect.rst
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.forward.rst
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.process.rst
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.rst
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.saltext.engines.rst
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.saltext.rst
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.utils.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    20016 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     4759 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/docs-auto.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/tools.txt
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/
+-rw-r--r--   0 root         (0) root         (0)      914 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/beacons.py
+-rw-r--r--   0 root         (0) root         (0)     5240 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/logs.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/salt_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/disk.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/test.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/manager.py
+-rw-r--r--   0 root         (0) root         (0)    10262 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/models.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/noop.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/regex_mask.pyi
+-rw-r--r--   0 root         (0) root         (0)     4442 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/shannon_mask.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/engines/analytics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/utils/dt.py
+-rw-r--r--   0 root         (0) root         (0)     5556 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/utils/eventbus.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3614 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      586 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/forwarders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/forwarders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/forwarders/test_concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/test_disabled_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/test_enabled_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_memusage.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/test_logs.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/test_logs_with_parse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_collatz.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_config_get.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/engines/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/process/test_regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)     5436 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/process/test_shannon_mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/salt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/salt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/salt/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/salt/engines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/.ruff.toml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/ci.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/pre_commit.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/pre_commit.py~
```

### Comparing `salt-analytics-framework-0.1.0/.coveragerc` & `salt-analytics-framework-0.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/.github/actions/setup-actionlint/action.yml` & `salt-analytics-framework-0.1.1/.github/actions/setup-actionlint/action.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/.gitignore` & `salt-analytics-framework-0.1.1/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -132,7 +132,10 @@
 .vim/
 
 # Ignore the setuptools_scm auto-generated version module
 src/saf/version.py
 
 # Ignore CI generated artifacts
 artifacts/
+
+# Ignore neovim backup files
+*~
```

### Comparing `salt-analytics-framework-0.1.0/.pre-commit-hooks/check-changelog-entries.py` & `salt-analytics-framework-0.1.1/.pre-commit-hooks/check-changelog-entries.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/.pre-commit-hooks/check-cli-examples.py` & `salt-analytics-framework-0.1.1/.pre-commit-hooks/check-cli-examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 CODE_ROOT = pathlib.Path(__file__).resolve().parent.parent
 EXECUTION_MODULES_PATH = CODE_ROOT / "src" / " saf" / "modules"
 
 
 def check_cli_examples(files):
     """
-    Check that every function on every execution module provides a CLI example
+    Check that every function on every execution module provides a CLI example.
     """
     errors = 0
     for file in files:
         path = pathlib.Path(file).resolve()
         try:
             relpath = path.relative_to(EXECUTION_MODULES_PATH)
             if str(relpath.parent) != ".":
```

### Comparing `salt-analytics-framework-0.1.0/.pre-commit-hooks/copyright-headers.py` & `salt-analytics-framework-0.1.1/.pre-commit-hooks/copyright-headers.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/.pre-commit-hooks/make-autodocs.py` & `salt-analytics-framework-0.1.1/.pre-commit-hooks/make-autodocs.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 #
 # pylint: disable=invalid-name,missing-module-docstring,missing-function-docstring
 import argparse
 import pathlib
 import sys
 import traceback
 
-
 CODE_ROOT = pathlib.Path(__file__).resolve().parent.parent
 SRC_DIR = CODE_ROOT / "src" / "salt-analytics-framework"
 DOC_DIR = CODE_ROOT / "docs"
 
 DOCS_BY_KIND = {}
```

### Comparing `salt-analytics-framework-0.1.0/.pre-commit-hooks/sort-pylint-spelling-words.py` & `salt-analytics-framework-0.1.1/.pre-commit-hooks/sort-pylint-spelling-words.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/.pylint-spelling-words` & `salt-analytics-framework-0.1.1/.pylint-spelling-words`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/CODE_OF_CONDUCT.md` & `salt-analytics-framework-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/CONTRIBUTING.md` & `salt-analytics-framework-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/LICENSE` & `salt-analytics-framework-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/NOTICE` & `salt-analytics-framework-0.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/PKG-INFO` & `salt-analytics-framework-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
```

### Comparing `salt-analytics-framework-0.1.0/README.rst` & `salt-analytics-framework-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/changelog/_template.rst` & `salt-analytics-framework-0.1.1/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/docs/Makefile` & `salt-analytics-framework-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/docs/conf.py` & `salt-analytics-framework-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/docs/index.rst` & `salt-analytics-framework-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/docs/make.bat` & `salt-analytics-framework-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/docs/ref/saf.collect.rst` & `salt-analytics-framework-0.1.1/docs/ref/saf.collect.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/docs/ref/saf.forward.rst` & `salt-analytics-framework-0.1.1/docs/ref/saf.forward.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/docs/ref/saf.process.rst` & `salt-analytics-framework-0.1.1/docs/ref/saf.process.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/docs/ref/saf.rst` & `salt-analytics-framework-0.1.1/docs/ref/saf.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/noxfile.py` & `salt-analytics-framework-0.1.1/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
-#
-# pylint: disable=protected-access
 from __future__ import annotations
 
+import contextlib
 import datetime
 import gzip
 import json
 import os
 import pathlib
 import shutil
 import sys
 import tarfile
 import tempfile
 from pathlib import Path
 
 import nox
 from nox.command import CommandFailed
-from nox.virtualenv import VirtualEnv
 
 # Nox options
 #  Reuse existing virtualenvs
 nox.options.reuse_existing_virtualenvs = True
 #  Don't fail on missing interpreters
 nox.options.error_on_missing_interpreters = False
 
 # Python versions to test against
 PYTHON_VERSIONS = ("3", "3.7", "3.8", "3.9", "3.10")
 # Be verbose when running under a CI context
-CI_RUN = (
-    os.environ.get("JENKINS_URL") or os.environ.get("CI") or os.environ.get("DRONE") is not None
-)
+CI_RUN = os.environ.get("CI") is not None
 PIP_INSTALL_SILENT = CI_RUN is False
 SKIP_REQUIREMENTS_INSTALL = "SKIP_REQUIREMENTS_INSTALL" in os.environ
 EXTRA_REQUIREMENTS_INSTALL = os.environ.get("EXTRA_REQUIREMENTS_INSTALL")
 
 COVERAGE_VERSION_REQUIREMENT = "coverage==6.2"
 SALT_REQUIREMENT = os.environ.get("SALT_REQUIREMENT") or "salt>=3005"
 if SALT_REQUIREMENT == "salt==master":
     SALT_REQUIREMENT = "git+https://github.com/saltstack/salt.git@master"
 
+REPO_ROOT = pathlib.Path(os.path.dirname(__file__)).resolve()
+ARTIFACTS_DIR = REPO_ROOT / "artifacts"
+IS_WINDOWS = sys.platform.lower().startswith("win")
+ONEDIR_ARTIFACT_PATH = ARTIFACTS_DIR / "salt"
+if IS_WINDOWS:
+    ONEDIR_PYTHON_PATH = ONEDIR_ARTIFACT_PATH / "Scripts" / "python.exe"
+else:
+    ONEDIR_PYTHON_PATH = ONEDIR_ARTIFACT_PATH / "bin" / "python3"
+
 # Prevent Python from writing bytecode
 os.environ["PYTHONDONTWRITEBYTECODE"] = "1"
 
 # Global Path Definitions
 REPO_ROOT = pathlib.Path(__file__).resolve().parent
 # Change current directory to REPO_ROOT
 os.chdir(str(REPO_ROOT))
@@ -62,15 +67,16 @@
 
 def _get_session_python_version_info(session):
     try:
         version_info = session._runner._real_python_version_info
     except AttributeError:
         session_py_version = session.run_always(
             "python",
-            "-c" 'import sys; sys.stdout.write("{}.{}.{}".format(*sys.version_info))',
+            "-c",
+            'import sys; sys.stdout.write("{}.{}.{}".format(*sys.version_info))',
             silent=True,
             log=False,
         )
         version_info = tuple(int(part) for part in session_py_version.split(".") if part.isdigit())
         session._runner._real_python_version_info = version_info
     return version_info
 
@@ -86,14 +92,15 @@
     session,
     *passed_requirements,
     install_coverage_requirements=True,
     install_test_requirements=True,
     install_source=False,
     install_salt=True,
     install_extras=None,
+    onedir=False,
 ):
     install_extras = install_extras or []
     if SKIP_REQUIREMENTS_INSTALL is False:
         # Always have the wheel package installed
         session.install("--progress-bar=off", "setuptools>=65.6.3,<66", silent=PIP_INSTALL_SILENT)
         session.install("--progress-bar=off", "wheel", silent=PIP_INSTALL_SILENT)
         if install_coverage_requirements:
@@ -108,36 +115,39 @@
                 "EXTRA_REQUIREMENTS_INSTALL='%s'",
                 EXTRA_REQUIREMENTS_INSTALL,
             )
             install_command = ["--progress-bar=off"]
             install_command += [req.strip() for req in EXTRA_REQUIREMENTS_INSTALL.split()]
             session.install(*install_command, silent=PIP_INSTALL_SILENT)
 
-        if install_salt:
+        if onedir is False and install_salt:
             session.install("--progress-bar=off", SALT_REQUIREMENT, silent=PIP_INSTALL_SILENT)
 
         if install_test_requirements:
             install_extras.append("tests")
 
         if passed_requirements:
             session.install("--progress-bar=off", *passed_requirements, silent=PIP_INSTALL_SILENT)
 
         if install_source:
             pkg = "."
             if install_extras:
                 pkg += f"[{','.join(install_extras)}]"
-            session.install("--progress-bar=off", "-e", pkg, silent=PIP_INSTALL_SILENT)
+            args = ["--progress-bar=off"]
+            if onedir is False:
+                args.append("-e")
+            args.append(pkg)
+            session.install(*args, silent=PIP_INSTALL_SILENT)
         elif install_extras:
             pkg = f".[{','.join(install_extras)}]"
             session.install("--progress-bar=off", pkg, silent=PIP_INSTALL_SILENT)
 
 
-@nox.session(python=PYTHON_VERSIONS)
-def tests(session):
-    _install_requirements(session, "jinja2<3.1", install_source=True)
+def _tests(session, onedir=False):
+    _install_requirements(session, install_source=True, onedir=onedir)
 
     sitecustomize_dir = session.run("salt-factories", "--coverage", silent=True, log=False)
     python_path_env_var = os.environ.get("PYTHONPATH") or None
     if python_path_env_var is None:
         python_path_env_var = sitecustomize_dir
     else:
         python_path_entries = python_path_env_var.split(os.pathsep)
@@ -150,14 +160,15 @@
         # The updated python path so that sitecustomize is importable
         "PYTHONPATH": python_path_env_var,
         # The full path to the .coverage data file. Makes sure we always write
         # them to the same directory
         "COVERAGE_FILE": str(COVERAGE_REPORT_DB),
         # Instruct sub processes to also run under coverage
         "COVERAGE_PROCESS_START": str(REPO_ROOT / ".coveragerc"),
+        "ONEDIR_TESTRUN": "1" if onedir else "0",
     }
 
     session.run("coverage", "erase")
     args = [
         "--rootdir",
         str(REPO_ROOT),
         f"--log-file={RUNTESTS_LOGFILE.relative_to(REPO_ROOT)}",
@@ -190,226 +201,97 @@
                 continue
         else:
             args.append("tests/")
     try:
         session.run("coverage", "run", "-m", "pytest", *args, env=env)
     finally:
         # Always combine and generate the XML coverage report
-        try:
+        with contextlib.suppress(CommandFailed):
             session.run("coverage", "combine")
-        except CommandFailed:
-            # Sometimes some of the coverage files are corrupt which would
-            # trigger a CommandFailed exception
-            pass
-        # Generate report for salt code coverage
-        session.run(
-            "coverage",
-            "xml",
-            "-o",
-            str(COVERAGE_REPORT_PROJECT),
-            "--omit=tests/*",
-            "--include=src/saf/*",
-        )
-        # Generate report for tests code coverage
-        session.run(
-            "coverage",
-            "xml",
-            "-o",
-            str(COVERAGE_REPORT_TESTS),
-            "--omit=src/saf/*",
-            "--include=tests/*",
-        )
+
         try:
-            session.run("coverage", "report", "--show-missing", "--include=src/saf/*")
-            # If you also want to display the code coverage report on the CLI
-            # for the tests, comment the call above and uncomment the line below
-            # session.run(
-            #    "coverage", "report", "--show-missing",
-            #    "--include=src/saf/*,tests/*"
-            # )
-        finally:
-            # Move the coverage DB to artifacts/coverage in order for it to be archived by CI
-            if COVERAGE_REPORT_DB.exists():
-                shutil.move(str(COVERAGE_REPORT_DB), str(ARTIFACTS_DIR / COVERAGE_REPORT_DB.name))
+            # Generate report for salt code coverage
+            session.run(
+                "coverage",
+                "xml",
+                "-o",
+                str(COVERAGE_REPORT_PROJECT),
+                "--omit=tests/*",
+                "--include=src/saf/*",
+            )
+            # Generate report for tests code coverage
+            session.run(
+                "coverage",
+                "xml",
+                "-o",
+                str(COVERAGE_REPORT_TESTS),
+                "--omit=src/saf/*",
+                "--include=tests/*",
+            )
+            try:
+                session.run("coverage", "report", "--show-missing", "--include=src/saf/*")
+                # If you also want to display the code coverage report on the CLI
+                # for the tests, comment the call above and uncomment the line below
+                # session.run(
+                #    "coverage", "report", "--show-missing",
+                #    "--include=src/saf/*,tests/*"
+                # )
+            finally:
+                # Move the coverage DB to artifacts/coverage in order for it to be archived by CI
+                if COVERAGE_REPORT_DB.exists():
+                    shutil.move(
+                        str(COVERAGE_REPORT_DB), str(ARTIFACTS_DIR / COVERAGE_REPORT_DB.name)
+                    )
+        except CommandFailed as exc:
+            # Tracking code coverage is still not working that well
+            if onedir is False:
+                raise exc from None
+
+
+@nox.session(python=PYTHON_VERSIONS)
+def tests(session):
+    _tests(session, onedir=False)
+
+
+@nox.session(
+    python=str(ONEDIR_PYTHON_PATH),
+    name="tests-onedir",
+    venv_params=["--system-site-packages"],
+)
+def test_onedir(session):
+    if not ONEDIR_ARTIFACT_PATH.exists():
+        session.error(
+            "The salt onedir artifact, expected to be in '{}', was not found".format(
+                ONEDIR_ARTIFACT_PATH.relative_to(REPO_ROOT)
+            )
+        )
+
+    _tests(session, onedir=True)
 
 
 class Tee:
     """
     Python class to mimic linux tee behavior.
     """
 
-    def __init__(self, first, second):
+    def __init__(self, first, second) -> None:
         self._first = first
         self._second = second
 
     def write(self, buf):
         wrote = self._first.write(buf)
         self._first.flush()
         self._second.write(buf)
         self._second.flush()
         return wrote
 
     def fileno(self):
         return self._first.fileno()
 
 
-def _lint(session, rcfile, flags, paths, tee_output=True):
-    _install_requirements(
-        session,
-        install_salt=False,
-        install_coverage_requirements=False,
-        install_test_requirements=False,
-        install_extras=["dev", "tests"],
-    )
-
-    if tee_output:
-        session.run("pylint", "--version")
-        pylint_report_path = os.environ.get("PYLINT_REPORT")
-
-    cmd_args = ["pylint", f"--rcfile={rcfile}"] + list(flags) + list(paths)
-
-    src_path = str(REPO_ROOT / "src")
-    python_path_env_var = os.environ.get("PYTHONPATH") or None
-    if python_path_env_var is None:
-        python_path_env_var = src_path
-    else:
-        python_path_entries = python_path_env_var.split(os.pathsep)
-        if src_path in python_path_entries:
-            python_path_entries.remove(src_path)
-        python_path_entries.insert(0, src_path)
-        python_path_env_var = os.pathsep.join(python_path_entries)
-
-    env = {
-        # The updated python path so that the project is importable without installing it
-        "PYTHONPATH": python_path_env_var,
-        "PYTHONUNBUFFERED": "1",
-    }
-
-    cmd_kwargs = {"env": env}
-
-    if tee_output:
-        stdout = tempfile.TemporaryFile(mode="w+b")
-        cmd_kwargs["stdout"] = Tee(stdout, sys.__stdout__)
-
-    try:
-        session.run(*cmd_args, **cmd_kwargs)
-    finally:
-        if tee_output:
-            stdout.seek(0)
-            contents = stdout.read()
-            if contents:
-                contents = contents.decode("utf-8")
-                sys.stdout.write(contents)
-                sys.stdout.flush()
-                if pylint_report_path:
-                    # Write report
-                    with open(pylint_report_path, "w", encoding="utf-8") as wfh:
-                        wfh.write(contents)
-                    session.log("Report file written to %r", pylint_report_path)
-            stdout.close()
-
-
-def _lint_pre_commit(session, rcfile, flags, paths):
-    if "VIRTUAL_ENV" not in os.environ:
-        session.error(
-            "This should be running from within a virtualenv and "
-            "'VIRTUAL_ENV' was not found as an environment variable."
-        )
-    if "pre-commit" not in os.environ["VIRTUAL_ENV"]:
-        session.error(
-            "This should be running from within a pre-commit virtualenv and "
-            "'VIRTUAL_ENV'({}) does not appear to be a pre-commit virtualenv.".format(
-                os.environ["VIRTUAL_ENV"]
-            )
-        )
-
-    try:
-        session.run(
-            "pip",
-            "uninstall",
-            "-y",
-            "salt-analytics-framework",
-            silent=True,
-        )
-    except (CommandFailed, OSError):
-        pass
-
-    # Let's patch nox to make it run inside the pre-commit virtualenv
-    session._runner.venv = VirtualEnv(
-        os.environ["VIRTUAL_ENV"],
-        interpreter=session._runner.func.python,
-        reuse_existing=True,
-        venv=True,
-    )
-    _lint(session, rcfile, flags, paths, tee_output=False)
-
-
-@nox.session(python="3")
-def lint(session):
-    """
-    Run PyLint against the code and the test suite. Set PYLINT_REPORT to a path to capture output.
-    """
-    session.notify(f"lint-code-{session.python}")
-    session.notify(f"lint-tests-{session.python}")
-
-
-@nox.session(python="3", name="lint-code")
-def lint_code(session):
-    """
-    Run PyLint against the code. Set PYLINT_REPORT to a path to capture output.
-    """
-    flags = ["--disable=I"]
-    if session.posargs:
-        paths = session.posargs
-    else:
-        paths = ["setup.py", "noxfile.py", "src/"]
-    _lint(session, ".pylintrc", flags, paths)
-
-
-@nox.session(python="3", name="lint-tests")
-def lint_tests(session):
-    """
-    Run PyLint against the test suite. Set PYLINT_REPORT to a path to capture output.
-    """
-    flags = ["--disable=I,redefined-outer-name,no-member,unused-argument"]
-    if session.posargs:
-        paths = session.posargs
-    else:
-        paths = ["tests/"]
-    _lint(session, ".pylintrc", flags, paths)
-
-
-@nox.session(python=False, name="lint-code-pre-commit")
-def lint_code_pre_commit(session):
-    """
-    Run PyLint against the code. Set PYLINT_REPORT to a path to capture output.
-    """
-    flags = ["--disable=I"]
-    if session.posargs:
-        paths = session.posargs
-    else:
-        paths = ["setup.py", "noxfile.py", "src/"]
-    _lint_pre_commit(session, ".pylintrc", flags, paths)
-
-
-@nox.session(python=False, name="lint-tests-pre-commit")
-def lint_tests_pre_commit(session):
-    """
-    Run PyLint against the code and the test suite. Set PYLINT_REPORT to a path to capture output.
-    """
-    flags = [
-        "--disable=I,redefined-outer-name,missing-function-docstring,no-member,missing-module-docstring",
-    ]
-    if session.posargs:
-        paths = session.posargs
-    else:
-        paths = ["tests/"]
-    _lint_pre_commit(session, ".pylintrc", flags, paths)
-
-
 @nox.session(python="3")
 def docs(session):
     """
     Build Docs.
     """
     _install_requirements(
         session,
@@ -536,18 +418,17 @@
     _install_requirements(
         session,
         install_coverage_requirements=False,
         install_test_requirements=False,
         install_source=True,
         install_extras=["docs"],
     )
-    try:
+    with contextlib.suppress(FileNotFoundError):
         shutil.rmtree("docs/ref")
-    except FileNotFoundError:
-        pass
+
     session.run(
         "sphinx-apidoc",
         "--module-first",
         "-o",
         "docs/ref/",
         "src/",
         "src/saf/config/schemas",
@@ -628,15 +509,15 @@
 
 
 class Recompress:
     """
     Helper class to re-compress a ``.tag.gz`` file to make it reproducible.
     """
 
-    def __init__(self, mtime):
+    def __init__(self, mtime) -> None:
         self.mtime = int(mtime)
 
     def tar_reset(self, tarinfo):
         """
         Reset user, group, mtime, and mode to create reproducible tar.
         """
         tarinfo.uid = tarinfo.gid = 0
@@ -655,35 +536,33 @@
         Re-compress the passed path.
         """
         tempd = pathlib.Path(tempfile.mkdtemp()).resolve()
         d_src = tempd.joinpath("src")
         d_src.mkdir()
         d_tar = tempd.joinpath(targz.stem)
         d_targz = tempd.joinpath(targz.name)
-        with tarfile.open(d_tar, "w|") as wfile:
-            with tarfile.open(targz, "r:gz") as rfile:
-                rfile.extractall(d_src)  # nosec
-                extracted_dir = next(pathlib.Path(d_src).iterdir())
-                for name in sorted(extracted_dir.rglob("*")):
-                    wfile.add(
-                        str(name),
-                        filter=self.tar_reset,
-                        recursive=False,
-                        arcname=str(name.relative_to(d_src)),
-                    )
-
-        with open(d_tar, "rb") as rfh:
-            with gzip.GzipFile(
-                fileobj=open(d_targz, "wb"), mode="wb", filename="", mtime=self.mtime
-            ) as gzfile:
-                while True:
-                    chunk = rfh.read(1024)
-                    if not chunk:
-                        break
-                    gzfile.write(chunk)
+        with tarfile.open(d_tar, "w|") as wfile, tarfile.open(targz, "r:gz") as rfile:
+            rfile.extractall(d_src)  # nosec
+            extracted_dir = next(pathlib.Path(d_src).iterdir())
+            for name in sorted(extracted_dir.rglob("*")):
+                wfile.add(
+                    str(name),
+                    filter=self.tar_reset,
+                    recursive=False,
+                    arcname=str(name.relative_to(d_src)),
+                )
+
+        with open(d_tar, "rb") as rfh, gzip.GzipFile(
+            fileobj=open(d_targz, "wb"), mode="wb", filename="", mtime=self.mtime
+        ) as gzfile:
+            while True:
+                chunk = rfh.read(1024)
+                if not chunk:
+                    break
+                gzfile.write(chunk)
         targz.unlink()
         shutil.move(str(d_targz), str(targz))
 
 
 @nox.session(python="3")
 def build(session):
     """
```

### Comparing `salt-analytics-framework-0.1.0/setup.cfg` & `salt-analytics-framework-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/src/saf/__init__.py` & `salt-analytics-framework-0.1.1/src/saf/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 from __future__ import annotations
 
+import contextlib
 import pathlib
 
 PACKAGE_ROOT = pathlib.Path(__file__).resolve().parent
 try:
     from .version import __version__
 except ImportError:  # pragma: no cover
     __version__ = "0.0.0.not-installed"
     try:
-        from importlib.metadata import version
         from importlib.metadata import PackageNotFoundError
+        from importlib.metadata import version
 
-        try:
+        with contextlib.suppress(PackageNotFoundError):
             __version__ = version(__name__)
-        except PackageNotFoundError:
-            # package is not installed
-            pass
+
     except ImportError:
         try:
-            from pkg_resources import get_distribution
             from pkg_resources import DistributionNotFound
+            from pkg_resources import get_distribution
 
-            try:
+            with contextlib.suppress(DistributionNotFound):
                 __version__ = get_distribution(__name__).version
-            except DistributionNotFound:
-                # package is not installed
-                pass
+
         except ImportError:
             # pkg resources isn't even available?!
             pass
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/collect/beacons.py` & `salt-analytics-framework-0.1.1/src/saf/collect/beacons.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,31 +6,35 @@
 It listens to Salt's event bus for beacon events and generates
 analytics events based off of those.
 """
 from __future__ import annotations
 
 import logging
 from datetime import datetime
+from datetime import timezone
 from typing import Any
 from typing import AsyncIterator
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TypeVar
 from typing import Union
 
 from pydantic import validator
 
 from saf.models import CollectConfigBase
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
 from saf.models import SaltEvent
 from saf.utils import eventbus
 
 log = logging.getLogger(__name__)
 
+BCE = TypeVar("BCE", bound="BeaconCollectedEvent")
+
 
 class BeaconsConfig(CollectConfigBase):
     """
     Configuration schema for the beacons collect plugin.
     """
 
     beacons: List[str]
@@ -46,23 +50,23 @@
     stamp: datetime
     raw_data: Dict[str, Any]
 
     @staticmethod
     def _convert_stamp(stamp: str) -> datetime:
         _stamp: datetime
         try:
-            _stamp = datetime.fromisoformat(stamp)
+            _stamp = datetime.fromisoformat(stamp).replace(tzinfo=timezone.utc)
         except AttributeError:  # pragma: no cover
             # Python < 3.7
-            _stamp = datetime.strptime(stamp, "%Y-%m-%dT%H:%M:%S.%f")
+            _stamp = datetime.strptime(stamp, "%Y-%m-%dT%H:%M:%S.%f").replace(tzinfo=timezone.utc)
         return _stamp
 
     @validator("stamp")
     @classmethod
-    def _validate_stamp(cls, value: Union[str, datetime]) -> datetime:
+    def _validate_stamp(cls: Type[BCE], value: Union[str, datetime]) -> datetime:
         if isinstance(value, datetime):
             return value
         return BeaconCollectedEvent._convert_stamp(value)
 
 
 def get_config_schema() -> Type[BeaconsConfig]:
     """
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/collect/logs.py` & `salt-analytics-framework-0.1.1/src/saf/collect/logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,47 +14,51 @@
 from typing import AsyncIterator
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Pattern
 from typing import Tuple
 from typing import Type
+from typing import TypeVar
 from typing import Union
 
 from drain3 import TemplateMiner
 from drain3.template_miner_config import TemplateMinerConfig
 from pydantic.class_validators import validator
 from pydantic.main import BaseModel
 
 from saf.models import CollectConfigBase
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
 
-
 log = logging.getLogger(__name__)
 
 
+LCC = TypeVar("LCC", bound="LogCollectConfig")
+
+
 class LogCollectConfig(CollectConfigBase):
     """
     Configuration schema for the log collect plugin.
     """
 
     path: pathlib.Path
     log_format: Optional[str]
     parse_config: Optional[pathlib.Path]
     backfill: bool = True
     wait: float = 5
 
     @validator("parse_config")
     @classmethod
     def _ensure_log_format_for_parsing(
-        cls, value: pathlib.Path, values: Dict[str, Any]
+        cls: Type[LCC], value: pathlib.Path, values: Dict[str, Any]
     ) -> pathlib.Path:
         if value and not values["log_format"]:
-            raise ValueError("Parsing without specifying a log_format is not allowed!")
+            msg = "Parsing without specifying a log_format is not allowed!"
+            raise ValueError(msg)
         return value
 
 
 class DrainResult(BaseModel):
     """
     Wrapper around parsing results.
     """
@@ -106,15 +110,15 @@
 
 async def collect(*, ctx: PipelineRunContext[LogCollectConfig]) -> AsyncIterator[CollectedEvent]:
     """
     Method called to collect log events.
     """
     config = ctx.config
     try:
-        parsing = True if config.parse_config else False
+        parsing = bool(config.parse_config)
 
         if config.log_format:
             headers, format_regex = _generate_log_format_regex(config.log_format)
 
         if parsing:
             log.info("Logs collector will be parsing using config at %s", config.parse_config)
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/collect/noop.py` & `salt-analytics-framework-0.1.1/src/saf/collect/noop.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from typing import AsyncIterator
 from typing import Type
 
 from saf.models import CollectConfigBase
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
 
-
 log = logging.getLogger(__name__)
 
 
 class NoopConfig(CollectConfigBase):
     """
     Configuration schema for the noop collect plugin.
     """
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/collect/salt_exec.py` & `salt-analytics-framework-0.1.1/src/saf/collect/salt_exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 import salt.loader
 
 from saf.models import CollectConfigBase
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
 
-
 log = logging.getLogger(__name__)
 
 
 class SaltExecConfig(CollectConfigBase):
     """
     Configuration schema for the salt_exec collect plugin.
     """
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/forward/disk.py` & `salt-analytics-framework-0.1.1/src/saf/forward/disk.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/src/saf/forward/noop.py` & `salt-analytics-framework-0.1.1/src/saf/forward/noop.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 import logging
 from typing import Type
 
 from saf.models import CollectedEvent
 from saf.models import ForwardConfigBase
 from saf.models import PipelineRunContext
 
-
 log = logging.getLogger(__name__)
 
 
 def get_config_schema() -> Type[ForwardConfigBase]:
     """
     Get the noop plugin configuration schema.
     """
     return ForwardConfigBase
 
 
-async def forward(  # pylint: disable=unused-argument
+async def forward(
     *,
-    ctx: PipelineRunContext[ForwardConfigBase],
+    ctx: PipelineRunContext[ForwardConfigBase],  # noqa: ARG001
     event: CollectedEvent,
 ) -> None:
     """
     Method called to forward the event.
     """
     log.info("Forwarding: %s", event)
-    assert event
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/forward/test.py` & `salt-analytics-framework-0.1.1/src/saf/forward/test.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from typing import Optional
 from typing import Type
 
 from saf.models import CollectedEvent
 from saf.models import ForwardConfigBase
 from saf.models import PipelineRunContext
 
-
 log = logging.getLogger(__name__)
 
 
 class TestForwardConfig(ForwardConfigBase):
     """
     Test forwarder configuration.
     """
@@ -49,15 +48,14 @@
     event: CollectedEvent,
 ) -> None:
     """
     Method called to forward the event.
     """
     config = ctx.config
     log.info("Forwarding using %s: %s", config.name, event)
-    assert event
     if config.sleep > 0:
         await asyncio.sleep(config.sleep)
     if config.path:
         if config.message:
             if config.dump_event:
                 dump_text = json.dumps({config.message: event.dict()})
             else:
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/manager.py` & `salt-analytics-framework-0.1.1/src/saf/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,90 +4,96 @@
 Salt Analytics Framework Pipelines Manager.
 """
 from __future__ import annotations
 
 import asyncio
 import logging
 from asyncio import Task
+from typing import TYPE_CHECKING
+from typing import TypeVar
 
 import aiorun
 
-from saf.models import AnalyticsConfig
 from saf.pipeline import Pipeline
 
+if TYPE_CHECKING:
+    from saf.models import AnalyticsConfig
+
 log = logging.getLogger(__name__)
 
+MN = TypeVar("MN", bound="Manager")
+
 
 class Manager:
     """
     Pipelines Manager.
     """
 
-    def __init__(self, config: AnalyticsConfig):
+    def __init__(self: MN, config: AnalyticsConfig) -> None:
         self.config = config
         self.pipelines: dict[str, Pipeline] = {}
         for name, pipeline_config in config.pipelines.items():
             self.pipelines[name] = Pipeline(name, pipeline_config)
         self.pipeline_tasks: dict[str, Task] = {}  # type: ignore[type-arg]
         self.loop = asyncio.get_event_loop()
 
-    async def run(self) -> None:
+    async def run(self: MN) -> None:
         """
         Async entry point to run the pipelines.
         """
         await self.start_pipelines()
         try:
             while True:
                 try:
                     await asyncio.sleep(0.05)
                 except (KeyboardInterrupt, asyncio.CancelledError):
                     break
         finally:
             await aiorun.shutdown_waits_for(self.stop_pipelines())
 
-    async def await_stopped(self) -> None:
+    async def await_stopped(self: MN) -> None:
         """
         Wait until all pipelines have been stopped.
         """
         await self.stop_pipelines()
 
-    async def start_pipelines(self) -> None:
+    async def start_pipelines(self: MN) -> None:
         """
         Start the pipelines.
         """
         for name in self.pipelines:
             result = await self.start_pipeline(name)
             if result is not None:
                 log.warning(result)
 
-    async def stop_pipelines(self) -> None:
+    async def stop_pipelines(self: MN) -> None:
         """
         Stop the pipelines.
         """
         for name in list(self.pipeline_tasks):
             result = await self.stop_pipeline(name)
             if result is not None:
                 log.warning(result)
 
-    async def start_pipeline(self, name: str) -> str | None:
+    async def start_pipeline(self: MN, name: str) -> str | None:
         """
         Start a pipeline by name.
         """
         log.info("Starting pipeline %r", name)
         if name not in self.pipelines:
             return f"Cannot start unknown pipeline {name!r}"
         pipeline = self.pipelines[name]
         if pipeline.config.enabled is False:
             return f"Pipeline {name!r} is disabled, skipping start."
         if name in self.pipeline_tasks:
             return f"Pipeline {name!r} is already running"
         self.pipeline_tasks[name] = self.loop.create_task(pipeline.run())
         return None
 
-    async def stop_pipeline(self, name: str) -> str | None:
+    async def stop_pipeline(self: MN, name: str) -> str | None:
         """
         Stop a pipeline by name.
         """
         log.info("Stopping pipeline %r", name)
         if name not in self.pipeline_tasks:
             return f"Pipeline {name!r} is not running. Not stopping it."
         task = self.pipeline_tasks.pop(name)
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/models.py` & `salt-analytics-framework-0.1.1/src/saf/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,95 +3,109 @@
 """
 Salt Analytics Framework Models.
 """
 from __future__ import annotations
 
 import logging
 from datetime import datetime
-from types import ModuleType
+from datetime import timezone
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Dict
 from typing import Generic
 from typing import List
+from typing import Mapping
 from typing import Optional
+from typing import Type
 from typing import TypeVar
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import PrivateAttr
 from pydantic import validator
 from pydantic.generics import GenericModel
 
 from saf.plugins import PluginsList
 from saf.utils import dt
 
+if TYPE_CHECKING:
+    from types import ModuleType
 
 log = logging.getLogger(__name__)
 
 
 class NonMutableModel(BaseModel):
     """
     Base class for non mutable models.
     """
 
     class Config:
         allow_mutation = False
 
 
+NMC = TypeVar("NMC", bound="NonMutableConfig")
+
+
 class NonMutableConfig(BaseModel):
     """
     Base class for non-mutable configurations.
     """
 
     _parent: AnalyticsConfig = PrivateAttr()
 
     @property
-    def parent(self) -> AnalyticsConfig:
+    def parent(self: NMC) -> AnalyticsConfig:
         """
         Return the parent configuration schema.
         """
         return self._parent
 
     class Config:
         allow_mutation = False
         underscore_attrs_are_private = True
 
 
+PCMI = TypeVar("PCMI", bound="PluginConfigMixin")
+
+
 class PluginConfigMixin(NonMutableConfig):
     """
     Base class for plugin configuration schemas.
     """
 
     plugin: str
 
     _name: str = PrivateAttr()
 
     @property
-    def name(self) -> str:
+    def name(self: PCMI) -> str:
         """
         Return the plugin name as defined in the configuration file.
         """
         return self._name
 
     @property
-    def loaded_plugin(self) -> ModuleType:
+    def loaded_plugin(self: PCMI) -> ModuleType:
         """
         Return the plugin instance(module) for which this configuration refers to.
         """
         raise NotImplementedError
 
 
+CCB = TypeVar("CCB", bound="CollectConfigBase")
+
+
 class CollectConfigBase(PluginConfigMixin):
     """
     Base config schema for collect plugins.
     """
 
-    def __new__(  # pylint: disable=unused-argument
-        cls,
+    def __new__(
+        cls: Type[CCB],
         plugin: str,
         **kwargs: Dict[str, Any],
     ) -> CollectConfigBase:
         """
         Swap the ``cls`` to instantiate if necessary.
 
         If the targeted plugin provides a ``get_config_schema`` function, then this
@@ -110,28 +124,31 @@
                 )
         except KeyError:
             pass
         instance: CollectConfigBase = PluginConfigMixin.__new__(cls)
         return instance
 
     @property
-    def loaded_plugin(self) -> ModuleType:
+    def loaded_plugin(self: CCB) -> ModuleType:
         """
         Return the plugin instance(module) for which this configuration refers to.
         """
         return PluginsList.instance().collectors[self.plugin]
 
 
+PCB = TypeVar("PCB", bound="ProcessConfigBase")
+
+
 class ProcessConfigBase(PluginConfigMixin):
     """
     Base config schema for process plugins.
     """
 
-    def __new__(  # pylint: disable=unused-argument
-        cls,
+    def __new__(
+        cls: Type[PCB],
         plugin: str,
         **kwargs: Dict[str, Any],
     ) -> ProcessConfigBase:
         """
         Swap the ``cls`` to instantiate if necessary.
 
         If the targeted plugin provides a ``get_config_schema`` function, then this
@@ -150,28 +167,31 @@
                 )
         except KeyError:
             pass
         instance: ProcessConfigBase = PluginConfigMixin.__new__(cls)
         return instance
 
     @property
-    def loaded_plugin(self) -> ModuleType:
+    def loaded_plugin(self: PCB) -> ModuleType:
         """
         Return the plugin instance(module) for which this configuration refers to.
         """
         return PluginsList.instance().processors[self.plugin]
 
 
+FCB = TypeVar("FCB", bound="ForwardConfigBase")
+
+
 class ForwardConfigBase(PluginConfigMixin):
     """
     Base config schema for forward plugins.
     """
 
-    def __new__(  # pylint: disable=unused-argument
-        cls,
+    def __new__(
+        cls: Type[FCB],
         plugin: str,
         **kwargs: Dict[str, Any],
     ) -> ForwardConfigBase:
         """
         Swap the ``cls`` to instantiate if necessary.
 
         If the targeted plugin provides a ``get_config_schema`` function, then this
@@ -190,56 +210,64 @@
                 )
         except KeyError:
             pass
         instance: ForwardConfigBase = PluginConfigMixin.__new__(cls)
         return instance
 
     @property
-    def loaded_plugin(self) -> ModuleType:
+    def loaded_plugin(self: FCB) -> ModuleType:
         """
         Return the plugin instance(module) for which this configuration refers to.
         """
         return PluginsList.instance().forwarders[self.plugin]
 
 
+PC = TypeVar("PC", bound="PipelineConfig")
+
+
 class PipelineConfig(NonMutableConfig):
     """
     Base config schema for pipeline configuration.
     """
 
     collect: str
     process: List[str] = Field(default_factory=list)
     forward: List[str]
     enabled: bool = True
     concurrent_forwarders: bool = True
 
     _name: str = PrivateAttr()
 
     @property
-    def name(self) -> str:
+    def name(self: PC) -> str:
         """
         Return the pipeline name as defined in the configuration file.
         """
         return self._name
 
 
+AC = TypeVar("AC", bound="AnalyticsConfig")
+
+
 class AnalyticsConfig(BaseModel):
     """
     Salt Analytics Framework configuration.
     """
 
     collectors: Dict[str, CollectConfigBase]
     processors: Dict[str, ProcessConfigBase] = Field(default_factory=dict)
     forwarders: Dict[str, ForwardConfigBase]
     pipelines: Dict[str, PipelineConfig]
     salt_config: Dict[str, Any]
 
     @validator("pipelines", pre=True)
     @classmethod
-    def _validate_pipelines(cls, pipelines: Dict[str, Dict[str, Any]]) -> Dict[str, Dict[str, Any]]:
+    def _validate_pipelines(
+        cls: Type[AC], pipelines: Dict[str, Dict[str, Any]]
+    ) -> Dict[str, Dict[str, Any]]:
         for name, data in pipelines.items():
             collect = data["collect"]
             process = data.get("process")
             forward = data["forward"]
             if process is None:
                 process = []
             elif isinstance(process, str):
@@ -249,15 +277,15 @@
 
             pipelines[name]["collect"] = collect
             pipelines[name]["process"] = process
             pipelines[name]["forward"] = forward
             pipelines[name].setdefault("enabled", True)
         return pipelines
 
-    def _init_private_attributes(self) -> None:
+    def _init_private_attributes(self: AC) -> None:
         """
         Set the `_parent` attribute on child schemas.
         """
         super()._init_private_attributes()
         # Allow plugin configurations to access the full configuration, this instance
         for entry in (self.collectors, self.processors, self.forwarders, self.pipelines):
             if entry is None:
@@ -268,41 +296,44 @@
 
 
 class CollectedEvent(BaseModel):
     """
     Class representing each of the collected events.
     """
 
-    data: Dict[str, Any]
+    data: Mapping[str, Any]
     timestamp: Optional[datetime] = Field(default_factory=dt.utcnow)
 
 
+SE = TypeVar("SE", bound="SaltEvent")
+
+
 class SaltEvent(NonMutableModel):
     """
     Class representing an event from Salt's event bus.
     """
 
     tag: str
     stamp: datetime
     data: Dict[str, Any]
     raw_data: Dict[str, Any]
 
     @staticmethod
     def _convert_stamp(stamp: str) -> datetime:
         _stamp: datetime
         try:
-            _stamp = datetime.fromisoformat(stamp)
+            _stamp = datetime.fromisoformat(stamp).replace(tzinfo=timezone.utc)
         except AttributeError:  # pragma: no cover
             # Python < 3.7
-            _stamp = datetime.strptime(stamp, "%Y-%m-%dT%H:%M:%S.%f")
+            _stamp = datetime.strptime(stamp, "%Y-%m-%dT%H:%M:%S.%f").replace(tzinfo=timezone.utc)
         return _stamp
 
     @validator("stamp")
     @classmethod
-    def _validate_stamp(cls, value: Union[str, datetime]) -> datetime:
+    def _validate_stamp(cls: Type[SE], value: Union[str, datetime]) -> datetime:
         if isinstance(value, datetime):
             return value
         return SaltEvent._convert_stamp(value)
 
 
 PipelineRunContextConfigType = TypeVar("PipelineRunContextConfigType", bound=NonMutableConfig)
 
@@ -313,20 +344,20 @@
     """
 
     config: PipelineRunContextConfigType
     cache: Dict[str, Any] = Field(default_factory=dict)
     shared_cache: Dict[str, Any] = Field(default_factory=dict)
 
     @property
-    def pipeline_config(self) -> AnalyticsConfig:
+    def pipeline_config(self) -> AnalyticsConfig:  # noqa: ANN101
         """
         Return the analytics configuration.
         """
         return self.config.parent
 
     @property
-    def salt_config(self) -> Dict[str, Any]:
+    def salt_config(self) -> Dict[str, Any]:  # noqa: ANN101
         """
         Return the salt configuration.
         """
         config: Dict[str, Any] = self.config.parent.salt_config
         return config
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/pipeline.py` & `salt-analytics-framework-0.1.1/src/saf/pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,79 +3,84 @@
 """
 Salt Analytics Framework Pipeline.
 """
 from __future__ import annotations
 
 import asyncio
 import logging
-from types import ModuleType
+from typing import TYPE_CHECKING
 from typing import Any
+from typing import TypeVar
 
 import backoff
 
 from saf.models import CollectConfigBase
 from saf.models import CollectedEvent
 from saf.models import ForwardConfigBase
 from saf.models import PipelineConfig
 from saf.models import PipelineRunContext
 from saf.models import ProcessConfigBase
 
+if TYPE_CHECKING:
+    from types import ModuleType
+
 log = logging.getLogger(__name__)
 
 
 def _check_backoff_exception(exc: Exception) -> bool:
     if isinstance(exc, asyncio.CancelledError):
         return True
     return False
 
 
+P = TypeVar("P", bound="Pipeline")
+
+
 class Pipeline:
     """
     Salt Analytics Pipeline.
     """
 
-    def __init__(self, name: str, config: PipelineConfig):
+    def __init__(self: P, name: str, config: PipelineConfig) -> None:
         self.name = name
         self.config = config
         self.collect_config: CollectConfigBase = config.parent.collectors[config.collect]
         self.process_configs: list[ProcessConfigBase] = []
         for config_name in config.process:
             self.process_configs.append(config.parent.processors[config_name])
         self.forward_configs: list[ForwardConfigBase] = []
         for config_name in config.forward:
             self.forward_configs.append(config.parent.forwarders[config_name])
 
-    async def run(self) -> None:
+    async def run(self: P) -> None:
         """
         Run the pipeline.
         """
         log.info("Pipeline %r started", self.name)
         while True:
             try:
                 await self._run()
             except asyncio.CancelledError:
                 log.info("Pipeline %r canceled", self.name)
                 break
-            except Exception as exc:  # pylint: disable=broad-except
-                log.error(
-                    "Failed to start the pipeline %s due to an error: %s",
+            except Exception:
+                log.exception(
+                    "Failed to start the pipeline %s due to an error",
                     self.name,
-                    exc,
-                    exc_info=True,
                 )
                 break
 
     @backoff.on_exception(
         backoff.expo,
         Exception,
         jitter=backoff.full_jitter,
         max_tries=5,
         giveup=_check_backoff_exception,
     )
-    async def _run(self) -> None:
+    async def _run(self: P) -> None:
         shared_cache: dict[str, Any] = {}
         process_ctxs: dict[str, PipelineRunContext[ProcessConfigBase]] = {}
         forward_ctxs: dict[str, PipelineRunContext[ForwardConfigBase]] = {}
         collect_ctx: PipelineRunContext[CollectConfigBase] = PipelineRunContext.construct(
             config=self.collect_config,
             shared_cache=shared_cache,
         )
@@ -92,26 +97,24 @@
                     # We pass copies of the event so that, in case an exception occurs while
                     # the event is being processed, and the event has already been modified,
                     # the next processor to run will get an unmodified copy of the event, not
                     # the partially processed event
                     original_event = event.copy()
                     process_plugin = process_config.loaded_plugin
                     try:
-                        event = await process_plugin.process(
+                        event = await process_plugin.process(  # noqa: PLW2901
                             ctx=process_ctxs[process_config.name],
                             event=event,
                         )
-                    except Exception as exc:  # pylint: disable=broad-except
-                        log.error(
-                            "An exception occurred while processing the event: %s",
-                            exc,
-                            exc_info=True,
+                    except Exception:
+                        log.exception(
+                            "An exception occurred while processing the event",
                         )
                         # Restore the original event
-                        event = original_event
+                        event = original_event  # noqa: PLW2901
                 # Forward the event
                 coros = []
                 for forward_config in self.forward_configs:
                     if forward_config.name not in forward_ctxs:
                         forward_ctxs[forward_config.name] = PipelineRunContext.construct(
                             config=forward_config,
                             shared_cache=shared_cache,
@@ -131,18 +134,19 @@
                         await coro
         finally:
             shared_cache.clear()
             process_ctxs.clear()
             forward_ctxs.clear()
 
     async def _wrap_forwarder_plugin_call(
-        self, plugin: ModuleType, ctx: PipelineRunContext[ForwardConfigBase], event: CollectedEvent
+        self: P,
+        plugin: ModuleType,
+        ctx: PipelineRunContext[ForwardConfigBase],
+        event: CollectedEvent,
     ) -> None:
         try:
             await plugin.forward(ctx=ctx, event=event)
-        except Exception as exc:  # pylint: disable=broad-except
-            log.error(
-                "An exception occurred while forwarding the event through config %r: %s",
+        except Exception:
+            log.exception(
+                "An exception occurred while forwarding the event through config %r",
                 ctx.config,
-                exc,
-                exc_info=True,
             )
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/plugins.py` & `salt-analytics-framework-0.1.1/src/saf/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,37 +6,40 @@
 from __future__ import annotations
 
 import contextlib
 import logging
 import pathlib
 import types
 from typing import Generator
+from typing import TypeVar
 
 from salt.utils import entrypoints
 
 log = logging.getLogger(__name__)
 
 
 PACKAGE_ROOT = pathlib.Path(__file__).resolve().parent
 
+PLT = TypeVar("PLT", bound="PluginsList")
+
 
 class PluginsList:
     """
     Plugins manager.
     """
 
     _instance = None
 
-    def __init__(self) -> None:
+    def __init__(self: PLT) -> None:
         self.collectors: dict[str, types.ModuleType] = {}
         self.processors: dict[str, types.ModuleType] = {}
         self.forwarders: dict[str, types.ModuleType] = {}
         self.load_plugins()
 
-    def __repr__(self) -> str:
+    def __repr__(self: PLT) -> str:
         """
         Return a printable representation of the class instance.
         """
         return (
             f"<{self.__class__.__name__} collectors={list(self.collectors)} "
             f"processors={list(self.processors)} forwarders={list(self.forwarders)}>"
         )
@@ -48,15 +51,15 @@
 
         If it doesn't exist yet, a new instance is created and cached.
         """
         if PluginsList._instance is None:
             PluginsList._instance = PluginsList()
         return PluginsList._instance
 
-    def load_plugins(self) -> None:
+    def load_plugins(self: PLT) -> None:
         """
         Load the available salt analytics framework plugins.
         """
         for name, listing in (
             ("collect", self.collectors),
             ("process", self.processors),
             ("forward", self.forwarders),
@@ -74,17 +77,15 @@
 def catch_entry_points_exception(entry_point: str) -> Generator[types.SimpleNamespace, None, None]:
     """
     Context manager to catch exceptions while loading entry points.
     """
     context = types.SimpleNamespace(exception_caught=False)
     try:
         yield context
-    except Exception as exc:  # pylint: disable=broad-except
+    except Exception:
         context.exception_caught = True
         entry_point_details = entrypoints.name_and_version_from_entry_point(entry_point)
-        log.error(  # type: ignore[call-arg]
-            "Error processing Salt Analytics Framework Plugin %s(version: %s): %s",
+        log.exception(
+            "Error processing Salt Analytics Framework Plugin %s(version: %s)",
             entry_point_details.name,
             entry_point_details.version,
-            exc,
-            exc_info_on_loglevel=logging.DEBUG,
         )
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/process/noop.py` & `salt-analytics-framework-0.1.1/src/saf/process/noop.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 import logging
 from typing import Type
 
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
 from saf.models import ProcessConfigBase
 
-
 log = logging.getLogger(__name__)
 
 
 def get_config_schema() -> Type[ProcessConfigBase]:
     """
     Get the noop plugin configuration schema.
     """
     return ProcessConfigBase
 
 
-async def process(  # pylint: disable=unused-argument
+async def process(
     *,
-    ctx: PipelineRunContext[ProcessConfigBase],
+    ctx: PipelineRunContext[ProcessConfigBase],  # noqa: ARG001
     event: CollectedEvent,
 ) -> CollectedEvent:
     """
     Method called to process the event.
     """
     log.info("Processing: %s", event)
     return event
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/process/regex_mask.py` & `salt-analytics-framework-0.1.1/src/saf/process/regex_mask.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 import logging
 import re
 from typing import Any
 from typing import Dict
 from typing import Match
 from typing import Optional
 from typing import Type
+from typing import TypeVar
 
 from pydantic import Field
 
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
 from saf.models import ProcessConfigBase
 
-
 log = logging.getLogger(__name__)
 
+RegexProcessObject = TypeVar("RegexProcessObject")
+
 
 class RegexMaskProcessConfig(ProcessConfigBase):
     """
     Configuration schema for the regex mask processor plugin.
     """
 
     rules: Dict[str, str]
@@ -53,51 +55,54 @@
 
         If a mask_char was provided, use that with matching length.
         Otherwise, use the rule name surrounded by prefix and suffix.
         """
         if config.mask_char:
             matched_str = match.group(0)
             return config.mask_char * len(matched_str)
-        else:
-            return f"{config.mask_prefix}{rule_name}{config.mask_suffix}"
+        return f"{config.mask_prefix}{rule_name}{config.mask_suffix}"
 
     orig_str = event_piece
 
     try:
         for rule_name, pattern in config.rules.items():
             event_piece = re.sub(pattern, functools.partial(repl_fn, rule_name), event_piece)
-    except Exception as exc:  # pylint: disable=broad-except
-        log.error("Failed to mask value '%s' with message %s.  Skipping.", orig_str, exc)
+    except Exception:
+        log.exception("Failed to mask value '%s'", orig_str)
 
     return event_piece
 
 
-def _regex_process(obj: Any, config: RegexMaskProcessConfig) -> Any:
+def _regex_process(
+    obj: str | list[Any] | tuple[Any, ...] | set[Any] | Dict[str, Any],
+    config: RegexMaskProcessConfig,
+) -> str | list[Any] | tuple[Any, ...] | set[Any] | Dict[str, Any]:
     """
     Recursive method to iterate over dictionary and apply rules to all str values.
     """
-    # Iterate over all attributes of obj.  If string, do mask.  If dict, set, tuple, or list -> recurse.
+    # Iterate over all attributes of obj.
+    # If string, do mask.
+    # If dict, set, tuple, or list -> recurse.
     if isinstance(obj, str):
         return _regex_mask(obj, config)
-    elif isinstance(obj, (list, tuple, set)):
+    if isinstance(obj, (list, tuple, set)):
         klass = type(obj)
         return klass(_regex_process(i, config) for i in obj)
-    elif isinstance(obj, dict):
+    if isinstance(obj, dict):
         for key, value in obj.items():
             obj[key] = _regex_process(value, config)
     return obj
 
 
-async def process(  # pylint: disable=unused-argument
+async def process(
     *,
     ctx: PipelineRunContext[RegexMaskProcessConfig],
     event: CollectedEvent,
 ) -> CollectedEvent:
     """
     Method called to mask the data based on provided regex rules.
     """
     config = ctx.config
     log.info("Processing event in regex_mask: %s", event.json())
     event_dict = event.dict()
     processed_event_dict = _regex_process(event_dict, config)
-    processed_event = event.parse_obj(processed_event_dict)
-    return processed_event
+    return event.parse_obj(processed_event_dict)
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/process/shannon_mask.py` & `salt-analytics-framework-0.1.1/src/saf/process/shannon_mask.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from pydantic import Field
 
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
 from saf.models import ProcessConfigBase
 
-
 log = logging.getLogger(__name__)
 
 
 class ShannonMaskProcessConfig(ProcessConfigBase):
     """
     Configuration schema for the Shannon mask processor plugin.
     """
@@ -79,55 +78,53 @@
         The replacement function to be called on each match.
 
         If a mask_char was provided, use that with matching length.
         Otherwise, use the config.mask_str surrounded by prefix and suffix.
         """
         if config.mask_char:
             return config.mask_char * len(word)
-        else:
-            return f"{config.mask_prefix}{config.mask_str}{config.mask_suffix}"
+        return f"{config.mask_prefix}{config.mask_str}{config.mask_suffix}"
 
     orig_str = event_piece
 
     try:
         split_piece = event_piece.split(config.delimeter)
         for word in split_piece:
             if len(word) >= config.length_threshold:
                 h_norm = _calculate_normalized_shannon_index(word, config.alphabet)
                 if h_norm > config.h_threshold:
                     event_piece = event_piece.replace(word, repl_fn(word))
-    except Exception as exc:  # pylint: disable=broad-except
-        log.error("Failed to mask value '%s' with message %s.  Skipping.", orig_str, exc)
+    except Exception:
+        log.exception("Failed to mask value '%s'", orig_str)
 
     return event_piece
 
 
-def _shannon_process(obj: Any, config: ShannonMaskProcessConfig) -> Any:
+def _shannon_process(obj: Any, config: ShannonMaskProcessConfig) -> Any:  # noqa: ANN401
     """
     Recursive method to iterate over dictionary and apply rules to all str values.
     """
     # Iterate over all attributes of obj.  If string, do mask.  If dict, recurse.  Else, do nothing.
     if isinstance(obj, str):
         return _shannon_mask(obj, config)
-    elif isinstance(obj, (list, tuple, set)):
+    if isinstance(obj, (list, tuple, set)):
         klass = type(obj)
         return klass(_shannon_process(i, config) for i in obj)
-    elif isinstance(obj, dict):
+    if isinstance(obj, dict):
         for key, value in obj.items():
             obj[key] = _shannon_process(value, config)
     return obj
 
 
-async def process(  # pylint: disable=unused-argument
+async def process(
     *,
     ctx: PipelineRunContext[ShannonMaskProcessConfig],
     event: CollectedEvent,
 ) -> CollectedEvent:
     """
     Method called to mask the data based on normalized Shannon index values.
     """
     config = ctx.config
     log.info("Processing event in shannon_mask: %s", event.json())
     event_dict = event.dict()
     processed_event_dict = _shannon_process(event_dict, config)
-    processed_event = event.parse_obj(processed_event_dict)
-    return processed_event
+    return event.parse_obj(processed_event_dict)
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/saltext/engines/analytics.py` & `salt-analytics-framework-0.1.1/src/saf/saltext/engines/analytics.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 Salt engine module.
 """
 from __future__ import annotations
 
 import asyncio
 import logging
 import pathlib
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
-from typing import TYPE_CHECKING
 
 import aiorun
 from salt.utils import yaml
 
 from saf.manager import Manager
 from saf.models import AnalyticsConfig
```

### Comparing `salt-analytics-framework-0.1.0/src/saf/utils/eventbus.py` & `salt-analytics-framework-0.1.1/src/saf/utils/eventbus.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from __future__ import annotations
 
 import asyncio
 import copy
 import fnmatch
 import logging
 import queue
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import AsyncIterator
-from typing import TYPE_CHECKING
 
 import salt.utils.event
 
 from saf.models import SaltEvent
 
 if TYPE_CHECKING:
     from queue import Queue
@@ -39,20 +39,20 @@
         salt_event = SaltEvent(
             tag=event_data["tag"],
             stamp=event_raw_data["_stamp"],
             data=event_data["data"],
             raw_data=event_raw_data,
         )
         log.debug("Constructed SaltEvent: %s", salt_event)
-    except Exception as exc:  # pylint: disable=broad-except
-        log.error("Failed to construct a SaltEvent: %s", exc, exc_info=True)
+    except Exception:
+        log.exception("Failed to construct a SaltEvent")
     return salt_event
 
 
-def _process_events(
+def _process_events(  # noqa: C901
     opts: dict[str, Any],
     events_queue: Queue[SaltEvent],
     tags: set[str],
 ) -> None:
     """
     Collect events from Salt's event bus.
 
@@ -94,19 +94,17 @@
                                     beacon_event_data["data"],
                                 )
                                 salt_event = _construct_event(beacon_event_data)
                                 if salt_event:
                                     events_queue.put_nowait(salt_event)
                                 # We found a matching tag, stop iterating tags
                                 break
-                        except Exception as exc:  # pylint: disable=broad-except
-                            log.error(
-                                "Ran into an error while processing beacon events: %s",
-                                exc,
-                                exc_info=True,
+                        except Exception:
+                            log.exception(
+                                "Ran into an error while processing beacon events",
                             )
                 # No additional processing required, process to next event from the event bus
                 continue
 
             # Non special cased salt event tags
             for tag in tags:
                 if fnmatch.fnmatch(event_tag, tag):
@@ -117,15 +115,15 @@
                     # We found a matching tag, stop iterating tags
                     break
 
 
 async def _start_event_listener(
     *,
     opts: dict[str, Any],
-    events_queue: "Queue[SaltEvent]",
+    events_queue: Queue[SaltEvent],
     tags: set[str],
 ) -> None:
     # We don't want to mix asyncio and tornado loops,
     # so, we defer the salt event listening to a separate
     # thread.
     loop = asyncio.get_event_loop()
     await loop.run_in_executor(
```

### Comparing `salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/PKG-INFO` & `salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
```

### Comparing `salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/SOURCES.txt` & `salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 .bandit
 .coveragerc
 .dockerignore
 .gitignore
 .pre-commit-config.yaml
 .pylint-spelling-words
-.pylintrc
 CHANGELOG.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 NOTICE
 README.rst
 noxfile.py
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 .github/actionlint.yaml
 .github/actions/setup-actionlint/action.yml
-.github/workflows/release.yml
-.github/workflows/test.yml
+.github/workflows/ci.yml
 .pre-commit-hooks/check-changelog-entries.py
 .pre-commit-hooks/check-cli-examples.py
 .pre-commit-hooks/copyright-headers.py
 .pre-commit-hooks/make-autodocs.py
 .pre-commit-hooks/sort-pylint-spelling-words.py
 changelog/_template.rst
 docs/Makefile
@@ -46,14 +44,15 @@
 requirements/base.txt
 requirements/build.txt
 requirements/changelog.txt
 requirements/dev.txt
 requirements/docs-auto.txt
 requirements/docs.txt
 requirements/tests.txt
+requirements/tools.txt
 src/saf/__init__.py
 src/saf/manager.py
 src/saf/models.py
 src/saf/pipeline.py
 src/saf/plugins.py
 src/saf/py.typed
 src/saf/version.py
@@ -65,14 +64,15 @@
 src/saf/forward/__init__.py
 src/saf/forward/disk.py
 src/saf/forward/noop.py
 src/saf/forward/test.py
 src/saf/process/__init__.py
 src/saf/process/noop.py
 src/saf/process/regex_mask.py
+src/saf/process/regex_mask.pyi
 src/saf/process/shannon_mask.py
 src/saf/saltext/__init__.py
 src/saf/saltext/engines/__init__.py
 src/saf/saltext/engines/analytics.py
 src/saf/utils/__init__.py
 src/saf/utils/dt.py
 src/saf/utils/eventbus.py
@@ -113,10 +113,12 @@
 tests/integration/engines/test_engine.py
 tests/unit/__init__.py
 tests/unit/process/__init__.py
 tests/unit/process/test_regex_mask.py
 tests/unit/process/test_shannon_mask.py
 tests/unit/salt/__init__.py
 tests/unit/salt/engines/__init__.py
+tools/.ruff.toml
 tools/__init__.py
+tools/ci.py
 tools/pre_commit.py
 tools/pre_commit.py~
```

### Comparing `salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/requires.txt` & `salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -40,9 +40,9 @@
 autodoc_pydantic
 
 [docsauto]
 sphinx-autobuild
 
 [tests]
 pytest>=6.0.0
-pytest-salt-factories==0.911.0
+pytest-salt-factories==1.0.0rc21
 pytest-asyncio
```

### Comparing `salt-analytics-framework-0.1.0/tests/functional/conftest.py` & `salt-analytics-framework-0.1.1/tests/functional/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 from __future__ import annotations
 
 import asyncio
-from typing import Any
 from typing import TYPE_CHECKING
+from typing import Any
 
 import pytest
 import pytest_asyncio
 
 from saf.manager import Manager
 from saf.models import AnalyticsConfig
 
-
 if TYPE_CHECKING:
     try:
         from typing import AsyncGenerator
     except ImportError:
         from typing import AsyncGenerator
 
 try:
@@ -40,15 +39,15 @@
 
 @pytest.fixture
 def analytics_config(analytics_config_dict: dict[str, Any]):
     return AnalyticsConfig.parse_obj(analytics_config_dict)
 
 
 @asyncio_fixture
-async def manager(analytics_config: AnalyticsConfig) -> "AsyncGenerator[Manager, None]":
+async def manager(analytics_config: AnalyticsConfig) -> AsyncGenerator[Manager, None]:
     _manager = Manager(analytics_config)
     loop = asyncio.get_event_loop()
     task = loop.create_task(_run_manager(_manager))
     try:
         yield _manager
     finally:
         if not task.done():
```

### Comparing `salt-analytics-framework-0.1.0/tests/functional/forwarders/test_concurrency.py` & `salt-analytics-framework-0.1.1/tests/functional/forwarders/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/functional/manager/conftest.py` & `salt-analytics-framework-0.1.1/tests/functional/manager/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/functional/manager/test_disabled_pipeline.py` & `salt-analytics-framework-0.1.1/tests/functional/manager/test_disabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/functional/manager/test_enabled_pipeline.py` & `salt-analytics-framework-0.1.1/tests/functional/manager/test_enabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_memusage.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_memusage.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_multiple.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_multiple.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_status.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_status.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/logs/conftest.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/logs/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/logs/test_logs.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/logs/test_logs.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/logs/test_logs_with_parse.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/logs/test_logs_with_parse.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/conftest.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_arg.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_arg.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pathlib
 import time
 
 import pytest
 
 from saf.models import CollectedEvent
 
-
 log = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope="module")
 def analytics_config_contents(analytics_events_dump_directory) -> str:
     return """
     collectors:
```

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_collatz.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_collatz.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pathlib
 import time
 
 import pytest
 
 from saf.models import CollectedEvent
 
-
 log = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope="module")
 def analytics_config_contents(analytics_events_dump_directory) -> str:
     return """
     collectors:
```

### Comparing `salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_config_get.py` & `salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_config_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pathlib
 import time
 
 import pytest
 
 from saf.models import CollectedEvent
 
-
 log = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope="module")
 def analytics_config_contents(analytics_events_dump_directory) -> str:
     return """
     collectors:
```

### Comparing `salt-analytics-framework-0.1.0/tests/integration/conftest.py` & `salt-analytics-framework-0.1.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/integration/engines/test_engine.py` & `salt-analytics-framework-0.1.1/tests/integration/engines/test_engine.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.0/tests/unit/process/test_regex_mask.py` & `salt-analytics-framework-0.1.1/tests/unit/process/test_regex_mask.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 import copy
 from typing import Any
 
 import pytest
 
 from saf.models import CollectedEvent
-from saf.process.regex_mask import _regex_process
 from saf.process.regex_mask import RegexMaskProcessConfig
+from saf.process.regex_mask import _regex_process
 
 
 class SubclassedCollectedEvent(CollectedEvent):
     """
     A subclass of CollectedEvent to allow recursive testing of regex masker.
     """
```

### Comparing `salt-analytics-framework-0.1.0/tests/unit/process/test_shannon_mask.py` & `salt-analytics-framework-0.1.1/tests/unit/process/test_shannon_mask.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import copy
 from typing import Any
 
 import pytest
 
 from saf.models import CollectedEvent
+from saf.process.shannon_mask import ShannonMaskProcessConfig
 from saf.process.shannon_mask import _calculate_normalized_shannon_index
 from saf.process.shannon_mask import _shannon_process
-from saf.process.shannon_mask import ShannonMaskProcessConfig
 
 
 class SubclassedCollectedEvent(CollectedEvent):
     """
     A subclass of CollectedEvent to allow recursive testing of Shannon masker.
     """
```

### Comparing `salt-analytics-framework-0.1.0/tools/pre_commit.py` & `salt-analytics-framework-0.1.1/tools/pre_commit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 """
 # pylint: disable=resource-leakage,broad-except,3rd-party-module-not-gated
 from __future__ import annotations
 
 import logging
 import shutil
 
-from ptscripts import command_group
 from ptscripts import Context
+from ptscripts import command_group
 
 log = logging.getLogger(__name__)
 
 # Define the command group
 cgroup = command_group(name="pre-commit", help="Pre-Commit Related Commands", description=__doc__)
```

### Comparing `salt-analytics-framework-0.1.0/tools/pre_commit.py~` & `salt-analytics-framework-0.1.1/tools/pre_commit.py~`

 * *Files identical despite different names*

