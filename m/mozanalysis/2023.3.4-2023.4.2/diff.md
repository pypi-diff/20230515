# Comparing `tmp/mozanalysis-2023.3.4.tar.gz` & `tmp/mozanalysis-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozanalysis-2023.3.4.tar", last modified: Mon Mar 27 17:52:13 2023, max compression
+gzip compressed data, was "mozanalysis-2023.4.2.tar", last modified: Thu Apr 20 18:37:51 2023, max compression
```

## Comparing `mozanalysis-2023.3.4.tar` & `mozanalysis-2023.4.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.194968 mozanalysis-2023.3.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.178968 mozanalysis-2023.3.4/.circleci/
--rw-r--r--   0 root         (0) root         (0)     4252 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)     1238 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)      985 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)      691 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)    16725 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      293 2023-03-27 17:52:13.194968 mozanalysis-2023.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2349 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.178968 mozanalysis-2023.3.4/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.182968 mozanalysis-2023.3.4/docs/_ext/
--rw-r--r--   0 root         (0) root         (0)      748 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/_ext/metrics_docstrings.py
--rw-r--r--   0 root         (0) root         (0)      138 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/about.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.182968 mozanalysis-2023.3.4/docs/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.182968 mozanalysis-2023.3.4/docs/api/bayesian_stats/
--rw-r--r--   0 root         (0) root         (0)      182 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/bayesian_stats/bayesian_bootstrap.rst
--rw-r--r--   0 root         (0) root         (0)      146 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/bayesian_stats/binary.rst
--rw-r--r--   0 root         (0) root         (0)      167 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/bayesian_stats/survival_func.rst
--rw-r--r--   0 root         (0) root         (0)      125 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/bayesian_stats.rst
--rw-r--r--   0 root         (0) root         (0)       97 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/bq.rst
--rw-r--r--   0 root         (0) root         (0)      113 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/experiment.rst
--rw-r--r--   0 root         (0) root         (0)      107 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/exposure.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.182968 mozanalysis-2023.3.4/docs/api/frequentist_stats/
--rw-r--r--   0 root         (0) root         (0)      164 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/frequentist_stats/bootstrap.rst
--rw-r--r--   0 root         (0) root         (0)      170 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/frequentist_stats/sample_size.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.182968 mozanalysis-2023.3.4/docs/api/metrics/
--rw-r--r--   0 root         (0) root         (0)      129 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/metrics/desktop.rst
--rw-r--r--   0 root         (0) root         (0)      125 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/metrics/fenix.rst
--rw-r--r--   0 root         (0) root         (0)      142 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/metrics/firefox_ios.rst
--rw-r--r--   0 root         (0) root         (0)      107 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/metrics.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.186968 mozanalysis-2023.3.4/docs/api/segments/
--rw-r--r--   0 root         (0) root         (0)      132 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/segments/desktop.rst
--rw-r--r--   0 root         (0) root         (0)      109 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/segments.rst
--rw-r--r--   0 root         (0) root         (0)      105 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api/sizing.rst
--rw-r--r--   0 root         (0) root         (0)       89 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/api.rst
--rw-r--r--   0 root         (0) root         (0)     5735 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    15303 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/guide.rst
--rw-r--r--   0 root         (0) root         (0)      231 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      472 2023-03-27 17:52:13.198968 mozanalysis-2023.3.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1236 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.174968 mozanalysis-2023.3.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.186968 mozanalysis-2023.3.4/src/mozanalysis/
--rw-r--r--   0 root         (0) root         (0)     1250 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.186968 mozanalysis-2023.3.4/src/mozanalysis/bayesian_stats/
--rw-r--r--   0 root         (0) root         (0)     9418 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/bayesian_stats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11736 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     8547 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/bayesian_stats/binary.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/bayesian_stats/survival_func.py
--rw-r--r--   0 root         (0) root         (0)     3304 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/bq.py
--rw-r--r--   0 root         (0) root         (0)     4379 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/config.py
--rw-r--r--   0 root         (0) root         (0)    53241 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/experiment.py
--rw-r--r--   0 root         (0) root         (0)     3598 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/exposure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.190968 mozanalysis-2023.3.4/src/mozanalysis/frequentist_stats/
--rw-r--r--   0 root         (0) root         (0)      199 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/frequentist_stats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8527 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/frequentist_stats/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)    19654 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/frequentist_stats/sample_size.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.190968 mozanalysis-2023.3.4/src/mozanalysis/metrics/
--rw-r--r--   0 root         (0) root         (0)    15172 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/metrics/desktop.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/metrics/fenix.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/metrics/firefox_ios.py
--rw-r--r--   0 root         (0) root         (0)      841 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/metrics/focus_android.py
--rw-r--r--   0 root         (0) root         (0)      817 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/metrics/focus_ios.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/metrics/klar_android.py
--rw-r--r--   0 root         (0) root         (0)      811 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/metrics/klar_ios.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.190968 mozanalysis-2023.3.4/src/mozanalysis/segments/
--rw-r--r--   0 root         (0) root         (0)     7442 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/segments/__init__.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/segments/desktop.py
--rw-r--r--   0 root         (0) root         (0)    25023 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/sizing.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/src/mozanalysis/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.186968 mozanalysis-2023.3.4/src/mozanalysis.egg-info/
--rw-r--r--   0 root         (0) root         (0)      293 2023-03-27 17:52:13.000000 mozanalysis-2023.3.4/src/mozanalysis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2345 2023-03-27 17:52:13.000000 mozanalysis-2023.3.4/src/mozanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 17:52:13.000000 mozanalysis-2023.3.4/src/mozanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      248 2023-03-27 17:52:13.000000 mozanalysis-2023.3.4/src/mozanalysis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-27 17:52:13.000000 mozanalysis-2023.3.4/src/mozanalysis.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.194968 mozanalysis-2023.3.4/tests/
--rw-r--r--   0 root         (0) root         (0)      425 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.194968 mozanalysis-2023.3.4/tests/bayesian_stats/
--rw-r--r--   0 root         (0) root         (0)      199 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/bayesian_stats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7069 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/bayesian_stats/test_bayesian_bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/bayesian_stats/test_binary.py
--rw-r--r--   0 root         (0) root         (0)     5487 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/bayesian_stats/test_consistency.py
--rw-r--r--   0 root         (0) root         (0)     3359 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/bayesian_stats/test_init.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/bayesian_stats/test_survival_func.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.194968 mozanalysis-2023.3.4/tests/frequentist_stats/
--rw-r--r--   0 root         (0) root         (0)      199 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/frequentist_stats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6355 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/frequentist_stats/test_bootstrap.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/frequentist_stats/test_sample_size_calc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 17:52:13.194968 mozanalysis-2023.3.4/tests/helpers/
--rw-r--r--   0 root         (0) root         (0)      411 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/helpers/cheap_lint.py
--rw-r--r--   0 root         (0) root         (0)    24336 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1524 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/test_metric_libraries.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/test_segment_libraries.py
--rw-r--r--   0 root         (0) root         (0)     4427 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/test_sizing.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-03-27 17:52:00.000000 mozanalysis-2023.3.4/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.750877 mozanalysis-2023.4.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.738877 mozanalysis-2023.4.2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     4252 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      985 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)      691 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      293 2023-04-20 18:37:51.750877 mozanalysis-2023.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2349 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.742877 mozanalysis-2023.4.2/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.742877 mozanalysis-2023.4.2/docs/_ext/
+-rw-r--r--   0 root         (0) root         (0)      748 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/_ext/metrics_docstrings.py
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/about.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.742877 mozanalysis-2023.4.2/docs/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.742877 mozanalysis-2023.4.2/docs/api/bayesian_stats/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/bayesian_stats/bayesian_bootstrap.rst
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/bayesian_stats/binary.rst
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/bayesian_stats/survival_func.rst
+-rw-r--r--   0 root         (0) root         (0)      125 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/bayesian_stats.rst
+-rw-r--r--   0 root         (0) root         (0)       97 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/bq.rst
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/experiment.rst
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/exposure.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.742877 mozanalysis-2023.4.2/docs/api/frequentist_stats/
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/frequentist_stats/bootstrap.rst
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/frequentist_stats/sample_size.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.742877 mozanalysis-2023.4.2/docs/api/metrics/
+-rw-r--r--   0 root         (0) root         (0)      129 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/metrics/desktop.rst
+-rw-r--r--   0 root         (0) root         (0)      125 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/metrics/fenix.rst
+-rw-r--r--   0 root         (0) root         (0)      142 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/metrics/firefox_ios.rst
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/metrics.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.742877 mozanalysis-2023.4.2/docs/api/segments/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/segments/desktop.rst
+-rw-r--r--   0 root         (0) root         (0)      109 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/segments.rst
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api/sizing.rst
+-rw-r--r--   0 root         (0) root         (0)       89 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/api.rst
+-rw-r--r--   0 root         (0) root         (0)     5735 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)    15303 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/guide.rst
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      472 2023-04-20 18:37:51.750877 mozanalysis-2023.4.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1236 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.738877 mozanalysis-2023.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.742877 mozanalysis-2023.4.2/src/mozanalysis/
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.746877 mozanalysis-2023.4.2/src/mozanalysis/bayesian_stats/
+-rw-r--r--   0 root         (0) root         (0)     9418 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/bayesian_stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11736 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     8547 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/bayesian_stats/binary.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/bayesian_stats/survival_func.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/bq.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/config.py
+-rw-r--r--   0 root         (0) root         (0)    53241 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/exposure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.746877 mozanalysis-2023.4.2/src/mozanalysis/frequentist_stats/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/frequentist_stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8527 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/frequentist_stats/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)    19654 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/frequentist_stats/sample_size.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.746877 mozanalysis-2023.4.2/src/mozanalysis/metrics/
+-rw-r--r--   0 root         (0) root         (0)    15203 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/metrics/desktop.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/metrics/fenix.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/metrics/firefox_ios.py
+-rw-r--r--   0 root         (0) root         (0)      841 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/metrics/focus_android.py
+-rw-r--r--   0 root         (0) root         (0)      817 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/metrics/focus_ios.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/metrics/klar_android.py
+-rw-r--r--   0 root         (0) root         (0)      811 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/metrics/klar_ios.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.746877 mozanalysis-2023.4.2/src/mozanalysis/segments/
+-rw-r--r--   0 root         (0) root         (0)     7442 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/segments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/segments/desktop.py
+-rw-r--r--   0 root         (0) root         (0)    25023 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/sizing.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/src/mozanalysis/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.746877 mozanalysis-2023.4.2/src/mozanalysis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      293 2023-04-20 18:37:51.000000 mozanalysis-2023.4.2/src/mozanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-04-20 18:37:51.000000 mozanalysis-2023.4.2/src/mozanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 18:37:51.000000 mozanalysis-2023.4.2/src/mozanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      248 2023-04-20 18:37:51.000000 mozanalysis-2023.4.2/src/mozanalysis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-20 18:37:51.000000 mozanalysis-2023.4.2/src/mozanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.746877 mozanalysis-2023.4.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.750877 mozanalysis-2023.4.2/tests/bayesian_stats/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/bayesian_stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7069 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/bayesian_stats/test_bayesian_bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/bayesian_stats/test_binary.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/bayesian_stats/test_consistency.py
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/bayesian_stats/test_init.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/bayesian_stats/test_survival_func.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.750877 mozanalysis-2023.4.2/tests/frequentist_stats/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/frequentist_stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6355 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/frequentist_stats/test_bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/frequentist_stats/test_sample_size_calc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:37:51.750877 mozanalysis-2023.4.2/tests/helpers/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/helpers/cheap_lint.py
+-rw-r--r--   0 root         (0) root         (0)    24336 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/test_metric_libraries.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/test_segment_libraries.py
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/test_sizing.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-04-20 18:37:39.000000 mozanalysis-2023.4.2/tox.ini
```

### Comparing `mozanalysis-2023.3.4/.circleci/config.yml` & `mozanalysis-2023.4.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/.gitignore` & `mozanalysis-2023.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/CHANGELOG.rst` & `mozanalysis-2023.4.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/CODE_OF_CONDUCT.md` & `mozanalysis-2023.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/LICENSE` & `mozanalysis-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/README.md` & `mozanalysis-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/docs/_ext/metrics_docstrings.py` & `mozanalysis-2023.4.2/docs/_ext/metrics_docstrings.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/docs/conf.py` & `mozanalysis-2023.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/docs/guide.rst` & `mozanalysis-2023.4.2/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/setup.py` & `mozanalysis-2023.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/__init__.py` & `mozanalysis-2023.4.2/src/mozanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/bayesian_stats/__init__.py` & `mozanalysis-2023.4.2/src/mozanalysis/bayesian_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py` & `mozanalysis-2023.4.2/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/bayesian_stats/binary.py` & `mozanalysis-2023.4.2/src/mozanalysis/bayesian_stats/binary.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/bayesian_stats/survival_func.py` & `mozanalysis-2023.4.2/src/mozanalysis/bayesian_stats/survival_func.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/bq.py` & `mozanalysis-2023.4.2/src/mozanalysis/bq.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/config.py` & `mozanalysis-2023.4.2/src/mozanalysis/config.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/experiment.py` & `mozanalysis-2023.4.2/src/mozanalysis/experiment.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/exposure.py` & `mozanalysis-2023.4.2/src/mozanalysis/exposure.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/frequentist_stats/bootstrap.py` & `mozanalysis-2023.4.2/src/mozanalysis/frequentist_stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/frequentist_stats/sample_size.py` & `mozanalysis-2023.4.2/src/mozanalysis/frequentist_stats/sample_size.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/metrics/__init__.py` & `mozanalysis-2023.4.2/src/mozanalysis/metrics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 return self._from_expr.format()
             except Exception as e:
                 raise ValueError(
                     f"{self.name}: from_expr contains a dataset template but no value was provided."  # noqa:E501
                 ) from e
         from_expr = self._from_expr.format(dataset=effective_dataset)
 
-        if self.experiments_column_type is None:
+        if (self.experiments_column_type is None) or (experiment_slug is None):
             return from_expr
 
         else:
             return """(
                 SELECT *
                 FROM {from_expr} ds
                 WHERE {slug_expr}
```

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/metrics/desktop.py` & `mozanalysis-2023.4.2/src/mozanalysis/metrics/desktop.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/metrics/fenix.py` & `mozanalysis-2023.4.2/src/mozanalysis/metrics/fenix.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/metrics/firefox_ios.py` & `mozanalysis-2023.4.2/src/mozanalysis/metrics/firefox_ios.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/metrics/focus_android.py` & `mozanalysis-2023.4.2/src/mozanalysis/metrics/focus_android.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/metrics/focus_ios.py` & `mozanalysis-2023.4.2/src/mozanalysis/metrics/focus_ios.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/metrics/klar_android.py` & `mozanalysis-2023.4.2/src/mozanalysis/metrics/klar_android.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/metrics/klar_ios.py` & `mozanalysis-2023.4.2/src/mozanalysis/metrics/klar_ios.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/segments/__init__.py` & `mozanalysis-2023.4.2/src/mozanalysis/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/segments/desktop.py` & `mozanalysis-2023.4.2/src/mozanalysis/segments/desktop.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/sizing.py` & `mozanalysis-2023.4.2/src/mozanalysis/sizing.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis/utils.py` & `mozanalysis-2023.4.2/src/mozanalysis/utils.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/src/mozanalysis.egg-info/SOURCES.txt` & `mozanalysis-2023.4.2/src/mozanalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/bayesian_stats/test_bayesian_bootstrap.py` & `mozanalysis-2023.4.2/tests/bayesian_stats/test_bayesian_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/bayesian_stats/test_binary.py` & `mozanalysis-2023.4.2/tests/bayesian_stats/test_binary.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/bayesian_stats/test_consistency.py` & `mozanalysis-2023.4.2/tests/bayesian_stats/test_consistency.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/bayesian_stats/test_init.py` & `mozanalysis-2023.4.2/tests/bayesian_stats/test_init.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/bayesian_stats/test_survival_func.py` & `mozanalysis-2023.4.2/tests/bayesian_stats/test_survival_func.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/frequentist_stats/test_bootstrap.py` & `mozanalysis-2023.4.2/tests/frequentist_stats/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/frequentist_stats/test_sample_size_calc.py` & `mozanalysis-2023.4.2/tests/frequentist_stats/test_sample_size_calc.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/test_experiment.py` & `mozanalysis-2023.4.2/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/test_metric_libraries.py` & `mozanalysis-2023.4.2/tests/test_metric_libraries.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/test_metrics.py` & `mozanalysis-2023.4.2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/test_segment_libraries.py` & `mozanalysis-2023.4.2/tests/test_segment_libraries.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/test_sizing.py` & `mozanalysis-2023.4.2/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tests/test_utils.py` & `mozanalysis-2023.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2023.3.4/tox.ini` & `mozanalysis-2023.4.2/tox.ini`

 * *Files identical despite different names*

