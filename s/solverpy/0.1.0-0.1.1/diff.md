# Comparing `tmp/solverpy-0.1.0.tar.gz` & `tmp/solverpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solverpy-0.1.0.tar", last modified: Mon Apr 24 20:06:03 2023, max compression
+gzip compressed data, was "solverpy-0.1.1.tar", last modified: Sun May 14 23:23:00 2023, max compression
```

## Comparing `solverpy-0.1.0.tar` & `solverpy-0.1.1.tar`

### file list

```diff
@@ -1,107 +1,93 @@
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.888682 solverpy-0.1.0/
--rw-r--r--   0 yan       (1000) yan       (1000)    35149 2023-04-24 19:19:27.000000 solverpy-0.1.0/LICENSE
--rw-r--r--   0 yan       (1000) yan       (1000)      594 2023-04-24 20:06:03.888682 solverpy-0.1.0/PKG-INFO
--rw-rw-r--   0 yan       (1000) yan       (1000)      656 2023-04-24 20:05:30.000000 solverpy-0.1.0/pyproject.toml
--rw-r--r--   0 yan       (1000) yan       (1000)       38 2023-04-24 20:06:03.888682 solverpy-0.1.0/setup.cfg
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.866682 solverpy-0.1.0/src/
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.870682 solverpy-0.1.0/src/solverpy/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/__init__.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.872682 solverpy-0.1.0/src/solverpy/benchmark/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2021-03-19 15:15:57.000000 solverpy-0.1.0/src/solverpy/benchmark/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1656 2022-06-17 01:16:35.000000 solverpy-0.1.0/src/solverpy/benchmark/evals.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.872682 solverpy-0.1.0/src/solverpy/path/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/path/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      867 2023-02-03 23:16:56.000000 solverpy-0.1.0/src/solverpy/path/bids.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      351 2022-06-11 16:24:04.000000 solverpy-0.1.0/src/solverpy/path/sids.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.874682 solverpy-0.1.0/src/solverpy/solver/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/__init__.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.876682 solverpy-0.1.0/src/solverpy/solver/__old__/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/__old__/__init__.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.877682 solverpy-0.1.0/src/solverpy/solver/__old__/atp/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/__old__/atp/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1534 2022-06-16 20:12:31.000000 solverpy-0.1.0/src/solverpy/solver/__old__/atp/eprover.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      852 2022-06-16 20:13:16.000000 solverpy-0.1.0/src/solverpy/solver/__old__/atp/lash.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1065 2022-06-16 20:13:06.000000 solverpy-0.1.0/src/solverpy/solver/__old__/atp/vampire.py
--rw-r--r--   0 yan       (1000) yan       (1000)     2034 2023-02-01 20:47:41.000000 solverpy-0.1.0/src/solverpy/solver/__old__/cachedsolver.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.878682 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/__init__.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.879682 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/db/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/db/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      273 2022-06-14 14:30:32.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/db/bid.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1617 2022-06-16 23:03:10.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/db/jsons.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1158 2022-06-16 02:05:46.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/db/outputs.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      236 2022-06-14 14:30:19.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/db/sid.py
--rw-rw-r--   0 yan       (1000) yan       (1000)       81 2022-06-14 14:03:17.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/plugin.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      248 2022-06-14 14:49:54.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/provider.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.879682 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/shell/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/shell/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      810 2023-02-01 22:59:49.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/shell/limits.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      685 2022-06-16 22:44:32.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/shell/time.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      390 2022-06-14 15:18:03.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/shell/timeout.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.880682 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/status/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/status/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      365 2022-06-14 15:20:53.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/status/smt.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      361 2022-06-14 15:21:01.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/status/tptp.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      203 2022-06-14 13:54:32.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/translator.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      234 2023-02-01 21:05:26.000000 solverpy-0.1.0/src/solverpy/solver/__old__/plugins/updater.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      555 2022-06-15 23:51:28.000000 solverpy-0.1.0/src/solverpy/solver/__old__/process.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     2246 2023-02-01 19:29:57.000000 solverpy-0.1.0/src/solverpy/solver/__old__/shellsolver.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.880682 solverpy-0.1.0/src/solverpy/solver/__old__/smt/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/__old__/smt/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1571 2022-06-16 20:15:32.000000 solverpy-0.1.0/src/solverpy/solver/__old__/smt/bitwuzla.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      717 2022-06-14 14:58:32.000000 solverpy-0.1.0/src/solverpy/solver/__old__/smt/z3.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      618 2022-06-17 00:35:41.000000 solverpy-0.1.0/src/solverpy/solver/__old__/smtsolver.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1650 2023-02-01 20:55:44.000000 solverpy-0.1.0/src/solverpy/solver/__old__/solver.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1165 2022-06-17 00:35:26.000000 solverpy-0.1.0/src/solverpy/solver/__old__/tptpsolver.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.881682 solverpy-0.1.0/src/solverpy/solver/atp/
--rw-rw-r--   0 yan       (1000) yan       (1000)     1468 2023-02-02 10:05:22.000000 solverpy-0.1.0/src/solverpy/solver/atp/eprover.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      777 2023-02-02 19:38:28.000000 solverpy-0.1.0/src/solverpy/solver/atp/lash.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      998 2023-02-02 10:12:21.000000 solverpy-0.1.0/src/solverpy/solver/atp/vampire.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.882682 solverpy-0.1.0/src/solverpy/solver/plugins/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/plugins/__init__.py
--rw-r--r--   0 yan       (1000) yan       (1000)     1655 2023-02-04 01:00:07.000000 solverpy-0.1.0/src/solverpy/solver/plugins/cachedprovider.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.884682 solverpy-0.1.0/src/solverpy/solver/plugins/db/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/plugins/db/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      273 2022-06-14 14:30:32.000000 solverpy-0.1.0/src/solverpy/solver/plugins/db/bid.py
--rw-r--r--   0 yan       (1000) yan       (1000)      816 2023-02-03 23:27:06.000000 solverpy-0.1.0/src/solverpy/solver/plugins/db/errors.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      583 2023-02-04 00:21:34.000000 solverpy-0.1.0/src/solverpy/solver/plugins/db/jsons.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1131 2023-02-04 01:12:40.000000 solverpy-0.1.0/src/solverpy/solver/plugins/db/outputs.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      236 2022-06-14 14:30:19.000000 solverpy-0.1.0/src/solverpy/solver/plugins/db/sid.py
--rw-r--r--   0 yan       (1000) yan       (1000)      877 2023-02-04 01:09:43.000000 solverpy-0.1.0/src/solverpy/solver/plugins/db/solved.py
--rw-r--r--   0 yan       (1000) yan       (1000)      950 2023-02-04 01:14:49.000000 solverpy-0.1.0/src/solverpy/solver/plugins/db/status.py
--rw-r--r--   0 yan       (1000) yan       (1000)      578 2023-02-04 00:23:23.000000 solverpy-0.1.0/src/solverpy/solver/plugins/db/yamls.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      241 2023-02-01 23:22:48.000000 solverpy-0.1.0/src/solverpy/solver/plugins/decorator.py
--rw-rw-r--   0 yan       (1000) yan       (1000)       81 2022-06-14 14:03:17.000000 solverpy-0.1.0/src/solverpy/solver/plugins/plugin.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      248 2022-06-14 14:49:54.000000 solverpy-0.1.0/src/solverpy/solver/plugins/provider.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.885682 solverpy-0.1.0/src/solverpy/solver/plugins/shell/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/plugins/shell/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      854 2023-02-02 10:23:06.000000 solverpy-0.1.0/src/solverpy/solver/plugins/shell/limits.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      703 2023-02-02 09:33:40.000000 solverpy-0.1.0/src/solverpy/solver/plugins/shell/time.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      403 2023-02-01 23:30:09.000000 solverpy-0.1.0/src/solverpy/solver/plugins/shell/timeout.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.885682 solverpy-0.1.0/src/solverpy/solver/plugins/status/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/solver/plugins/status/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      382 2023-02-02 09:33:52.000000 solverpy-0.1.0/src/solverpy/solver/plugins/status/smt.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      378 2023-02-02 09:34:15.000000 solverpy-0.1.0/src/solverpy/solver/plugins/status/tptp.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      203 2022-06-14 13:54:32.000000 solverpy-0.1.0/src/solverpy/solver/plugins/translator.py
--rw-r--r--   0 yan       (1000) yan       (1000)     1639 2023-02-04 01:11:07.000000 solverpy-0.1.0/src/solverpy/solver/pluginsolver.py
--rw-r--r--   0 yan       (1000) yan       (1000)     1051 2023-02-03 22:52:56.000000 solverpy-0.1.0/src/solverpy/solver/shellsolver.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.886682 solverpy-0.1.0/src/solverpy/solver/smt/
--rw-rw-r--   0 yan       (1000) yan       (1000)     1467 2023-02-02 10:37:13.000000 solverpy-0.1.0/src/solverpy/solver/smt/bitwuzla.py
--rw-r--r--   0 yan       (1000) yan       (1000)     1389 2023-02-02 10:55:25.000000 solverpy-0.1.0/src/solverpy/solver/smt/cvc5.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      650 2023-02-02 10:16:17.000000 solverpy-0.1.0/src/solverpy/solver/smt/z3.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      764 2023-02-02 10:27:48.000000 solverpy-0.1.0/src/solverpy/solver/smtsolver.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      648 2023-02-02 00:01:31.000000 solverpy-0.1.0/src/solverpy/solver/solver.py
--rw-r--r--   0 yan       (1000) yan       (1000)     1234 2023-02-03 22:18:32.000000 solverpy-0.1.0/src/solverpy/solver/timedsolver.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1206 2023-02-02 19:48:34.000000 solverpy-0.1.0/src/solverpy/solver/tptpsolver.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.887682 solverpy-0.1.0/src/solverpy/tools/
--rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.0/src/solverpy/tools/__init__.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1191 2023-02-01 18:54:17.000000 solverpy-0.1.0/src/solverpy/tools/bars.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1097 2022-06-15 20:23:23.000000 solverpy-0.1.0/src/solverpy/tools/human.py
--rw-rw-r--   0 yan       (1000) yan       (1000)     1377 2023-03-02 18:14:23.000000 solverpy-0.1.0/src/solverpy/tools/par.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      555 2022-06-15 23:51:28.000000 solverpy-0.1.0/src/solverpy/tools/patterns.py
--rw-rw-r--   0 yan       (1000) yan       (1000)      280 2022-06-14 14:21:15.000000 solverpy-0.1.0/src/solverpy/tools/timeme.py
-drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-04-24 20:06:03.871682 solverpy-0.1.0/src/solverpy.egg-info/
--rw-rw-r--   0 yan       (1000) yan       (1000)      594 2023-04-24 20:06:03.000000 solverpy-0.1.0/src/solverpy.egg-info/PKG-INFO
--rw-rw-r--   0 yan       (1000) yan       (1000)     3295 2023-04-24 20:06:03.000000 solverpy-0.1.0/src/solverpy.egg-info/SOURCES.txt
--rw-rw-r--   0 yan       (1000) yan       (1000)        1 2023-04-24 20:06:03.000000 solverpy-0.1.0/src/solverpy.egg-info/dependency_links.txt
--rw-rw-r--   0 yan       (1000) yan       (1000)        9 2023-04-24 20:06:03.000000 solverpy-0.1.0/src/solverpy.egg-info/top_level.txt
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.331608 solverpy-0.1.1/
+-rw-r--r--   0 yan       (1000) yan       (1000)    35149 2023-04-24 19:19:27.000000 solverpy-0.1.1/LICENSE
+-rw-r--r--   0 yan       (1000) yan       (1000)      594 2023-05-14 23:23:00.331608 solverpy-0.1.1/PKG-INFO
+-rw-rw-r--   0 yan       (1000) yan       (1000)      762 2023-05-14 23:02:16.000000 solverpy-0.1.1/pyproject.toml
+-rw-r--r--   0 yan       (1000) yan       (1000)       38 2023-05-14 23:23:00.331608 solverpy-0.1.1/setup.cfg
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.312608 solverpy-0.1.1/src/
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.317608 solverpy-0.1.1/src/_dust/
+-rw-r--r--   0 yan       (1000) yan       (1000)     1505 2023-05-12 23:27:56.000000 solverpy-0.1.1/src/_dust/bars.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     2070 2023-05-06 21:16:45.000000 solverpy-0.1.1/src/_dust/evals.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     1601 2023-05-06 21:17:57.000000 solverpy-0.1.1/src/_dust/par.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.318608 solverpy-0.1.1/src/solverpy/
+-rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.1/src/solverpy/__init__.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.319608 solverpy-0.1.1/src/solverpy/benchmark/
+-rw-rw-r--   0 yan       (1000) yan       (1000)        0 2021-03-19 15:15:57.000000 solverpy-0.1.1/src/solverpy/benchmark/__init__.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.319608 solverpy-0.1.1/src/solverpy/benchmark/db/
+-rw-r--r--   0 yan       (1000) yan       (1000)        0 2023-05-13 18:55:30.000000 solverpy-0.1.1/src/solverpy/benchmark/db/__init__.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.320608 solverpy-0.1.1/src/solverpy/benchmark/db/_old/
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.320608 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/
+-rw-r--r--   0 yan       (1000) yan       (1000)     1663 2023-04-27 01:01:11.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/cachedprovider.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.321608 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/
+-rw-r--r--   0 yan       (1000) yan       (1000)      826 2023-04-27 02:06:54.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/errors.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      619 2023-04-27 02:07:02.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/jsons.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     1141 2023-04-27 02:07:09.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/outputs.py
+-rw-r--r--   0 yan       (1000) yan       (1000)      890 2023-04-27 02:07:22.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/solved.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1002 2023-04-27 02:07:29.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/status.py
+-rw-r--r--   0 yan       (1000) yan       (1000)      568 2023-04-27 02:07:35.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/yamls.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      322 2023-04-27 00:38:15.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/provider.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1825 2023-05-01 22:15:48.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/pluginsolver.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1234 2023-05-14 19:54:36.000000 solverpy-0.1.1/src/solverpy/benchmark/db/_old/timedsolver.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1771 2023-05-14 20:32:41.000000 solverpy-0.1.1/src/solverpy/benchmark/db/db.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1994 2023-05-14 21:53:18.000000 solverpy-0.1.1/src/solverpy/benchmark/db/jsons.py
+-rw-r--r--   0 yan       (1000) yan       (1000)      218 2023-05-13 23:01:41.000000 solverpy-0.1.1/src/solverpy/benchmark/db/provider.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     3819 2023-05-14 22:25:23.000000 solverpy-0.1.1/src/solverpy/benchmark/launcher.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.322608 solverpy-0.1.1/src/solverpy/benchmark/path/
+-rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.1/src/solverpy/benchmark/path/__init__.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      944 2023-05-13 21:20:54.000000 solverpy-0.1.1/src/solverpy/benchmark/path/bids.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     1350 2023-04-27 18:22:05.000000 solverpy-0.1.1/src/solverpy/benchmark/path/sids.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.323608 solverpy-0.1.1/src/solverpy/solver/
+-rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.1/src/solverpy/solver/__init__.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.323608 solverpy-0.1.1/src/solverpy/solver/atp/
+-rw-rw-r--   0 yan       (1000) yan       (1000)      106 2023-04-26 20:42:52.000000 solverpy-0.1.1/src/solverpy/solver/atp/__init__.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     1468 2023-02-02 10:05:22.000000 solverpy-0.1.1/src/solverpy/solver/atp/eprover.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      777 2023-02-02 19:38:28.000000 solverpy-0.1.1/src/solverpy/solver/atp/lash.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      998 2023-02-02 10:12:21.000000 solverpy-0.1.1/src/solverpy/solver/atp/vampire.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.324608 solverpy-0.1.1/src/solverpy/solver/plugins/
+-rw-rw-r--   0 yan       (1000) yan       (1000)      292 2023-05-13 21:26:18.000000 solverpy-0.1.1/src/solverpy/solver/plugins/__init__.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.325608 solverpy-0.1.1/src/solverpy/solver/plugins/db/
+-rw-rw-r--   0 yan       (1000) yan       (1000)       65 2023-05-01 22:35:52.000000 solverpy-0.1.1/src/solverpy/solver/plugins/db/__init__.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      283 2023-04-27 02:06:45.000000 solverpy-0.1.1/src/solverpy/solver/plugins/db/bid.py
+-rw-r--r--   0 yan       (1000) yan       (1000)      457 2023-05-13 21:31:03.000000 solverpy-0.1.1/src/solverpy/solver/plugins/db/errors.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      758 2023-05-13 21:31:25.000000 solverpy-0.1.1/src/solverpy/solver/plugins/db/outputs.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      378 2023-04-28 19:54:54.000000 solverpy-0.1.1/src/solverpy/solver/plugins/db/sid.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      317 2023-05-14 19:06:25.000000 solverpy-0.1.1/src/solverpy/solver/plugins/decorator.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)       81 2023-04-26 20:49:03.000000 solverpy-0.1.1/src/solverpy/solver/plugins/plugin.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.326608 solverpy-0.1.1/src/solverpy/solver/plugins/shell/
+-rw-rw-r--   0 yan       (1000) yan       (1000)      115 2023-04-26 20:32:31.000000 solverpy-0.1.1/src/solverpy/solver/plugins/shell/__init__.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      913 2023-05-14 20:09:38.000000 solverpy-0.1.1/src/solverpy/solver/plugins/shell/limits.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      773 2023-05-14 22:42:59.000000 solverpy-0.1.1/src/solverpy/solver/plugins/shell/time.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      403 2023-02-01 23:30:09.000000 solverpy-0.1.1/src/solverpy/solver/plugins/shell/timeout.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.326608 solverpy-0.1.1/src/solverpy/solver/plugins/status/
+-rw-rw-r--   0 yan       (1000) yan       (1000)       68 2023-04-26 20:39:19.000000 solverpy-0.1.1/src/solverpy/solver/plugins/status/__init__.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      492 2023-04-26 22:55:41.000000 solverpy-0.1.1/src/solverpy/solver/plugins/status/smt.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      488 2023-05-14 19:47:57.000000 solverpy-0.1.1/src/solverpy/solver/plugins/status/tptp.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      203 2022-06-14 13:54:32.000000 solverpy-0.1.1/src/solverpy/solver/plugins/translator.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1461 2023-05-13 21:02:09.000000 solverpy-0.1.1/src/solverpy/solver/pluginsolver.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1311 2023-05-13 21:02:46.000000 solverpy-0.1.1/src/solverpy/solver/shellsolver.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.327608 solverpy-0.1.1/src/solverpy/solver/smt/
+-rw-rw-r--   0 yan       (1000) yan       (1000)      106 2023-04-26 20:43:44.000000 solverpy-0.1.1/src/solverpy/solver/smt/__init__.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     1467 2023-02-02 10:37:13.000000 solverpy-0.1.1/src/solverpy/solver/smt/bitwuzla.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1718 2023-05-14 20:18:15.000000 solverpy-0.1.1/src/solverpy/solver/smt/cvc5.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      650 2023-02-02 10:16:17.000000 solverpy-0.1.1/src/solverpy/solver/smt/z3.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      780 2023-05-14 19:18:53.000000 solverpy-0.1.1/src/solverpy/solver/smtsolver.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     1071 2023-05-14 19:11:23.000000 solverpy-0.1.1/src/solverpy/solver/solver.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     1082 2023-05-14 19:20:00.000000 solverpy-0.1.1/src/solverpy/solver/tptpsolver.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.328608 solverpy-0.1.1/src/solverpy/task/
+-rw-r--r--   0 yan       (1000) yan       (1000)        0 2023-05-11 22:07:53.000000 solverpy-0.1.1/src/solverpy/task/__init__.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     2232 2023-05-13 21:23:31.000000 solverpy-0.1.1/src/solverpy/task/bar.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1336 2023-05-14 21:03:43.000000 solverpy-0.1.1/src/solverpy/task/launcher.py
+-rw-r--r--   0 yan       (1000) yan       (1000)      472 2023-05-12 21:43:54.000000 solverpy-0.1.1/src/solverpy/task/shelltask.py
+-rw-r--r--   0 yan       (1000) yan       (1000)      577 2023-05-13 19:13:20.000000 solverpy-0.1.1/src/solverpy/task/solvertask.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1011 2023-05-13 16:17:21.000000 solverpy-0.1.1/src/solverpy/task/task.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.330608 solverpy-0.1.1/src/solverpy/tools/
+-rw-rw-r--   0 yan       (1000) yan       (1000)        0 2022-06-15 19:11:03.000000 solverpy-0.1.1/src/solverpy/tools/__init__.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)     1387 2023-05-13 14:22:28.000000 solverpy-0.1.1/src/solverpy/tools/human.py
+-rw-r--r--   0 yan       (1000) yan       (1000)     1601 2023-05-13 19:54:23.000000 solverpy-0.1.1/src/solverpy/tools/log.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      555 2022-06-15 23:51:28.000000 solverpy-0.1.1/src/solverpy/tools/patterns.py
+-rw-rw-r--   0 yan       (1000) yan       (1000)      280 2022-06-14 14:21:15.000000 solverpy-0.1.1/src/solverpy/tools/timeme.py
+drwxr-xr-x   0 yan       (1000) yan       (1000)        0 2023-05-14 23:23:00.318608 solverpy-0.1.1/src/solverpy.egg-info/
+-rw-rw-r--   0 yan       (1000) yan       (1000)      594 2023-05-14 23:23:00.000000 solverpy-0.1.1/src/solverpy.egg-info/PKG-INFO
+-rw-rw-r--   0 yan       (1000) yan       (1000)     2580 2023-05-14 23:23:00.000000 solverpy-0.1.1/src/solverpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yan       (1000) yan       (1000)        1 2023-05-14 23:23:00.000000 solverpy-0.1.1/src/solverpy.egg-info/dependency_links.txt
+-rw-r--r--   0 yan       (1000) yan       (1000)       12 2023-05-14 23:23:00.000000 solverpy-0.1.1/src/solverpy.egg-info/requires.txt
+-rw-rw-r--   0 yan       (1000) yan       (1000)       15 2023-05-14 23:23:00.000000 solverpy-0.1.1/src/solverpy.egg-info/top_level.txt
```

### Comparing `solverpy-0.1.0/LICENSE` & `solverpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solverpy-0.1.0/PKG-INFO` & `solverpy-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solverpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python inteface for Automated Reasoning (AR) solvers, provers, and checkers.
 Project-URL: Homepage, https://github.com/cbboyan/solverpy
 Project-URL: Bug Tracker, https://github.com/cbboyan/solverpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `solverpy-0.1.0/pyproject.toml` & `solverpy-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools","setuptools-git-versioning<2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "solverpy"
-version = "0.1.0"
 description = "Python inteface for Automated Reasoning (AR) solvers, provers, and checkers."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
-dependencies = []
+dependencies = [
+  "PyYAML",
+  "tqdm"
+]
+dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/cbboyan/solverpy"
 "Bug Tracker" = "https://github.com/cbboyan/solverpy/issues"
 
+[tool.setuptools-git-versioning]
+enabled = true
+
+
```

### Comparing `solverpy-0.1.0/src/solverpy/benchmark/evals.py` & `solverpy-0.1.1/src/_dust/evals.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,70 @@
 import os
 
-from ..path import bids, sids
+from ..benchmark.path import bids, sids
 from ..tools import par, bars
 
 
 def prove1(solver, instance, strategy):
    result = solver.solve(instance, strategy)
    return (instance, result)
 
-def eval1(solver, bid, sid, cores=4, chunksize=1, **others):
+def eval1(solver, bid, sid, cores=4, chunksize=1, desc=None, taskdone=None, **others):
    ps = bids.problems(bid)
    args = [(solver, (bid, p), sid) for p in ps]
    results = {}
 
    def callback(res, bar):
       nonlocal solver, results
       ((bid,p), result) = res
       results[p] = result
       if not solver.valid(result):
          bar.update_errors()
       elif solver.solved(result):
          bar.update_solved()
       else:
          bar.update_failed()
-
-   bar = bars.solved(total=len(args), desc=sid)
+      if taskdone is not None:
+         taskdone()
+ 
+   desc = "%s @ %s" % (sid, bid) if not desc else desc
+   bar = bars.solved(total=len(args), desc=desc)
    par.apply(prove1, args, cores=cores, bar=bar, chunksize=chunksize, callback=callback)
    return results
 
-#def evals(prover, bids, sids, cores=4, **others):
-#   allres = {}
-#   ns = len(bids) * len(sids)
-#   ps = sum([len(problem.problems(bid)) for bid in bids]) * len(sids)
-#   logger.info("+ evaluating %s strategies on %d benchmarks" % (len(sids), len(bids)))
-#   logger.debug(log.data("- evaluation parameters:", dict(
-#      bids=bids, 
-#      sids=sids,
-#      cores=cores,
-#      prover=prover.name(),
-#      resources=prover.resources(),
-#      problems=human.humanint(ps),
-#      eta=human.humantime(ps*prover.timeout()/cores) if prover.timeout() else "unknown",
-#   )))
-#   
-#   n = 1
-#   label = "(%%3d/%d)" % ns
-#   for bid in bids:
-#      for sid in sids:
-#         result1 = eval1(prover, bid, sid, cores=cores, label=label%n, **others)
-#         n += 1
-#         result1 = {(bid,sid,p):result1[p] for p in result1}
-#         allres.update(result1)
-#   return allres
+def evals(solver=None, bidlist=None, sidlist=None, jobs=None, **others):
+   assert(jobs or (solver and bidlist and sidlist))
+
+   if not jobs:
+      jobs = [(solver,bid,sid) for bid in bidlist for sid in sidlist]
+   
+   def indent(desc, left=True):
+      nonlocal maxdesc
+      if left:
+         return (" " * (maxdesc-len(desc))) + desc
+      else:
+         return desc + (" " * (maxdesc-len(desc))) 
+
+   allres = {}
+   total = 0
+   maxdesc = 0
+   for (solver, bid, sid) in jobs:
+      total += len(bids.problems(bid))
+      desc = "%s @ %s" % (sid, bid)
+      maxdesc = max(maxdesc, len(desc))
+
+   desc = "Total: %s jobs, %s tasks" % (len(jobs), total)
+   maxdesc = max(maxdesc, len(desc))
+   totbar = bars.default(total, indent(desc, left=False))
+   try:
+      for (solver, bid, sid) in jobs:
+         desc = "%s @ %s" % (sid, bid)
+         result1 = eval1(solver, bid, sid, taskdone=lambda: totbar.update(1), desc=indent(desc), **others)
+         result1 = {(bid,sid,p):result1[p] for p in result1}
+         allres.update(result1)
+      totbar.close()
+   except KeyboardInterrupt as e:
+      totbar.close()
+      raise e
+   
+   return allres
```

### Comparing `solverpy-0.1.0/src/solverpy/path/bids.py` & `solverpy-0.1.1/src/solverpy/benchmark/path/bids.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,19 +17,22 @@
    if os.path.isfile(p_bid):
       p_bid = os.path.dirname(p_bid)
    return os.path.join(p_bid, problem).rstrip("/")
 
 def name(bid, limit=None):
    bid = bid.replace("/", "-")
    if limit:
-      bid = f"{bid}-{limit}"
+      bid = f"{bid}--{limit}"
    return bid
 
-def problems(bid):
+def problems(bid, cache={}):
+   if bid in cache:
+      return cache[bid]
    p_bid = bidpath(bid)
    if os.path.isfile(p_bid):
       probs = open(p_bid).read().strip().split("\n")
    else: # now os.path.isdir(p_bid) holds
       probs = [x for x in os.listdir(p_bid) \
          if os.path.isfile(os.path.join(p_bid,x))]
+   cache[bid] = probs
    return probs
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/__old__/atp/eprover.py` & `solverpy-0.1.1/src/solverpy/solver/atp/eprover.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 import re
 
 from ..tptpsolver import TptpSolver
 from ..plugins.shell.limits import Limits
-from .. import process
-from ...tools import human
+from ...tools import patterns, human
 
 E_BINARY = "eprover"
 
 E_STATIC = "-s -p -R --print-statistics --tstp-format"
 
-E_LIMITS = {
+E_BUILDER = {
    "T": lambda x: "--soft-cpu-limit=%s --cpu-limit=%s" % (x,int(x)+1),
    "P": "--processed-set-limit=%s",
    "C": "--processed-clauses-limit=%s",
    "G": "--generated-limit=%s"
 }
 
 E_PAT = re.compile(r"^#\s*(\S.*\S)\s*: (\S*)$", re.MULTILINE)
 
 E_TABLE = {
    "Processed clauses"                    : "Processed",
    "Generated clauses"                    : "Generated",
    "Proof object total steps"             : "ProofLen",
    "Removed by relevancy pruning/SinE"    : "Pruned",
    "Backward-subsumed"                    : "BackSub",
-   "Backward-rewritten"                   : "BackRw",
+   "Backward-rewritten"                   : "BackRew",
    "Paramodulations"                      : "Paramod",
    "Factorizations"                       : "Fact",
    "Equation resolutions"                 : "EqRes",
    "Clause-clause subsumption calls (NU)" : "Subsumes",
    "Termbank termtop insertions"          : "TermBank",
 }
 
 class E(TptpSolver):
 
-   def __init__(self, limit=None, binary=E_BINARY, static=E_STATIC, complete=True, plugins=[]):
+   def __init__(self, limit, binary=E_BINARY, static=E_STATIC, complete=True, plugins=[]):
       cmd = f"{binary} {static}"
-      limits = [Limits(limit, E_LIMITS)] if limit else []
-      TptpSolver.__init__(self, cmd, plugins+limits, complete, wait=2)
+      TptpSolver.__init__(self, cmd, limit, E_BUILDER, plugins, 2, complete)
 
    def process(self, output):
-      result = process.keyval(E_PAT, output, E_TABLE)
-      result = process.mapval(result, human.numeric)
+      result = patterns.keyval(E_PAT, output, E_TABLE)
+      result = patterns.mapval(result, human.numeric)
       return result
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/__old__/atp/vampire.py` & `solverpy-0.1.1/src/solverpy/solver/atp/vampire.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import re
 
 from ..tptpsolver import TptpSolver
 from ..plugins.shell.limits import Limits
-from .. import process
-from ...tools import human
+from ...tools import patterns, human
 
 
 V_BINARY = "vampire"
 
 V_STATIC = "--proof tptp -stat full --input_syntax tptp"
 
-V_LIMITS = {
+V_BUILDER = {
    "T": "--time_limit %ss",
    "M": "--memory_limit %s",
 }
 
 V_PAT = re.compile(r"^% (.*): ([0-9.]*).*$", re.MULTILINE)
 
 V_TABLE = {
@@ -25,17 +24,16 @@
    "Time elapsed"      : "Runtime",
    "Memory used [KB]"  : "Memory",
    "Split clauses"     : "Splits",
 }
 
 class Vampire(TptpSolver):
 
-   def __init__(self, limit=None, binary=V_BINARY, static=V_STATIC, complete=True, plugins=[]):
+   def __init__(self, limit, binary=V_BINARY, static=V_STATIC, complete=True, plugins=[]):
       cmd = f"{binary} {static}"
-      limits = [Limits(limit, V_LIMITS)] if limit else []
-      TptpSolver.__init__(self, cmd, plugins+limits, complete, wait=1)
+      TptpSolver.__init__(self, cmd, limit, V_BUILDER, plugins, 1, complete)
 
    def process(self, output):
-      result = process.keyval(V_PAT, output, V_TABLE)
-      result = process.mapval(result, human.numeric)
+      result = patterns.keyval(V_PAT, output, V_TABLE)
+      result = patterns.mapval(result, human.numeric)
       return result
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/__old__/plugins/db/jsons.py` & `solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/cachedprovider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 import os
-import json
-
-from ..provider import Provider
-from ....path import bids
 from multiprocessing import Manager
 
-DEFAULT_NAME = "00JSONS"
-DEFAULT_DIR = os.getenv("PYSOLVE_JSONS", DEFAULT_NAME)
+from .provider import Provider
 
-def path(bid, sid):
-   return os.path.join(
-      DEFAULT_DIR, 
-      bids.name(bid),
-      sid).rstrip("/") + ".json"
-
-class Jsons(Provider):
-  
-   def __init__(self, bid, sid):
-      self.bid = bid
-      self.sid = sid
+class CachedProvider(Provider):
+
+   def __init__(self):
+      self.bid = None
+      self.sid = None
       man = Manager()
-      self.cache = self.load() # thread-local copy / not synced
+      self.cache = None # thread-local copy / not synced 
       self.results = man.list() # shared list 
 
    def register(self, solver):
       solver.providers.append(self)
+      self.solver = solver
+
+   def reset(self, bid, sid):
+      self.flush()
+      self.bid = bid
+      self.sid = sid
+      self.cache = self.load()
    
    def query(self, instance, strategy):
       (bid, p) = instance
       if not self.check(bid, strategy):
-         raise Exception("Error: Query on invalid bid/sid in Jsons.query.")
+         raise Exception("Error: Query on invalid bid/sid in CachedProvider.")
       return self.cache[p] if p in self.cache else None
 
    def store(self, instance, strategy, output, result):
+      if not self.solver.valid(result):
+         return
       (bid, p) = instance
       if not self.check(bid, strategy):
-         raise Exception("Error: Store on invalid bid/sid in Jsons.store.")
+         raise Exception("Error: Store on invalid bid/sid in CachedProvider.")
       self.results.append((p, result))
 
    def check(self, bid, sid):
       return (self.bid == bid) and (self.sid == sid)
 
    def flush(self):
+      if (self.cache is None) or (self.bid is None) or (self.sid is None):
+         return
       self.cache.update(dict(self.results))
       while self.results:
          self.results.pop()
-      f = path(self.bid, self.sid)
+      f = self.cachepath()
       os.makedirs(os.path.dirname(f), exist_ok=True)
-      with open(f,"w") as fw:
-         json.dump(self.cache, fw, indent=3, sort_keys=True)
+      self.cachedump(f)
 
    def load(self):
-      f = path(self.bid, self.sid)
-      ret = json.load(open(f)) if os.path.isfile(f) else {}
-      return ret
+      f = self.cachepath()
+      return self.cacheload(f)
+
+   def cachedump(self, f):
+      raise NotImlementedError()
 
+   def cacheload(self, f):
+      raise NotImlementedError
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/__old__/plugins/db/outputs.py` & `solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/outputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import os
 
 from ..provider import Provider
-from ....path import bids
+from ....benchmark.path import bids
 
-DEFAULT_NAME = "00OUTPUTS"
-DEFAULT_DIR = os.getenv("PYSOLVE_OUTPUTS", DEFAULT_NAME)
-
-def path(bid, sid, limit, problem):
-   return os.path.join(
-      DEFAULT_DIR, 
-      bids.name(bid,limit),
-      sid,
-      problem).rstrip("/")
+NAME = "outputs"
 
 class Outputs(Provider):
    
+   def __init__(self):
+      self._path = bids.dbpath(NAME)
+   
    def register(self, solver):
       solver.providers.append(self)
       self.solver = solver
    
    def path(self, instance, strategy):
       (bid, problem) = instance
-      return path(bid, strategy, self.solver.limits.spec, problem) + ".out"
+      limit = self.solver.limits.limit
+      p = os.path.join(self._path, bids.name(bid,limit), strategy, problem)
+      return p
    
    def query(self, instance, strategy):
       f = self.path(instance, strategy)
       #print("QUERY", instance, strategy, f)
       if not os.path.isfile(f):
          return None
       output = open(f).read()
       result = self.solver.process(output)
-      self.solver.update(instance, strategy, output, result, store=False)
+      self.solver.update(instance, strategy, output, result)
       return result
 
    def store(self, instance, strategy, output, result):
+      if not output:
+         return
       #print("STORE", instance, strategy, result)
-      f = self.path(instance, strategy)
-      os.makedirs(os.path.dirname(f), exist_ok=True)
-      open(f,"w").write(output)
+      if self.solver.valid(result):
+         f = self.path(instance, strategy)
+         os.makedirs(os.path.dirname(f), exist_ok=True)
+         open(f,"w").write(output)
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/__old__/plugins/shell/limits.py` & `solverpy-0.1.1/src/solverpy/solver/plugins/shell/limits.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-from ..updater import Updater
+from ..decorator import Decorator
 
-def make(fun, arg):
+def build(fun, arg):
    return fun % arg if isinstance(fun, str) else fun(arg)
 
-class Limits(Updater):
+class Limits(Decorator):
 
-   def __init__(self, spec, limits):
-      lims = {x[0]:x[1:] for x in spec.split("-") if x}
+   def __init__(self, limit, builder):
+      lims = {x[0]:x[1:] for x in limit.split("-") if x}
       self.timeout = int(lims["T"]) if "T" in lims else None
       try:
-         lims = [make(limits[x],y) for (x,y) in lims.items() if limits[x]]
+         lims = [build(builder[x],y) for (x,y) in lims.items() if builder[x]]
       except:
-         raise Exception(f"pysolve: Invalid limit string: {spec}")
+         raise Exception(f"solverpy: Invalid limit string: {limit}")
       self.args = " ".join(lims)
-      self.spec = spec
-   
+      self.limit = limit
+
+   def __str__(self):
+      return self.limit
+
    def register(self, solver):
       super().register(solver)
-      solver.limits = self
-
-   def shell(self, cmd):
+      self._timeouts = solver.timeout
+   
+   def decorate(self, cmd):
       return f"{cmd} {self.args}" if self.args else cmd
-
+   
    def update(self, instance, strategy, output, result):
-      if self.timeout:
+      if result["status"] in self._timeouts:
          result["timeout"] = self.timeout
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/__old__/plugins/shell/time.py` & `solverpy-0.1.1/src/solverpy/solver/plugins/shell/time.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import re
 
-from ..updater import Updater
-from ... import process
+from ..decorator import Decorator
+from ....tools import patterns
 
 # real 0.01
 # user 0.01
 # sys 0.00
 
 TIME_CMD = "/usr/bin/env time -p"
 
 TIME_PAT = re.compile(r"^(real|user|sys) ([0-9.]*)$", re.MULTILINE)
 
 TIME_TABLE = {
-   "real": "REALTIME",
-   "user": "USERTIME",
-   "sys" : "SYSTIME",
+   "real": "realtime",
+   "user": "usertime",
+   "sys" : "systime",
 }
 
-class Time(Updater):
+class Time(Decorator):
 
    def __init__(self):
       self.prefix = TIME_CMD
 
-   def shell(self, cmd):
+   def decorate(self, cmd):
       return f"{self.prefix} {cmd}"
 
    def update(self, instance, strategy, output, result):
-      res = process.keyval(TIME_PAT, output, TIME_TABLE)
-      res = process.mapval(res, float)
-      result["RUNTIME"] = res["REALTIME"] - res["SYSTIME"]
-      result["USERTIME"] = res["USERTIME"]
+      res = patterns.keyval(TIME_PAT, output, TIME_TABLE)
+      res = patterns.mapval(res, float)
+      result.update(res)
+      result["runtime"] = res["realtime"] - res["systime"]
+      #result["realtime"] = res["realtime"]
+      #result["runtime"] = res["usertime"]
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/__old__/process.py` & `solverpy-0.1.1/src/solverpy/tools/patterns.py`

 * *Files identical despite different names*

### Comparing `solverpy-0.1.0/src/solverpy/solver/__old__/smt/bitwuzla.py` & `solverpy-0.1.1/src/solverpy/solver/smt/bitwuzla.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import re
 from ..smtsolver import SmtSolver
-from ..plugins.shell.limits import Limits
-from .. import process
-from ...tools import human
+from ...tools import patterns, human
 
 BWZ_BINARY = "bitwuzla"
 
 BWZ_STATIC = "-v"
 
-BWZ_LIMITS = {
+BWZ_BUILDER = {
    "T": "-t=%s",
 }
 
 BWZ_TABLE = {
    "variable substitutions"               : "SubstVar",
    "uninterpreted function substitutions" : "SubstUf",
    "embedded constraint substitutions"    : "SubstEc",
@@ -30,17 +28,16 @@
 BWZ_KEYS = "|".join(BWZ_TABLE.keys()).replace("(","[(]").replace(")","[)]")
 
 #BWZ_PAT = re.compile(r"^\[bitwuzla>core\]\s*(\d+) ([a-zA-Z ]*)\b", flags=re.MULTILINE)
 BWZ_PAT = re.compile(r"^\[bitwuzla>core\]\s*(\d+) (%s)" % BWZ_KEYS, flags=re.MULTILINE)
 
 class Bitwuzla(SmtSolver):
    
-   def __init__(self, limit=None, binary=BWZ_BINARY, static=BWZ_STATIC, plugins=[]):
+   def __init__(self, limit, binary=BWZ_BINARY, static=BWZ_STATIC, plugins=[]):
       cmd = f"{binary} {static}"
-      limits = [Limits(limit, BWZ_LIMITS)] if limit else []
-      SmtSolver.__init__(self, cmd, plugins+limits, wait=1)
+      SmtSolver.__init__(self, cmd, limit, BWZ_BUILDER, plugins, wait=1)
 
    def process(self, output):
-      result = process.valkey(BWZ_PAT, output, BWZ_TABLE)
-      result = process.mapval(result, human.numeric)
+      result = patterns.valkey(BWZ_PAT, output, BWZ_TABLE)
+      result = patterns.mapval(result, human.numeric)
       return result
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/__old__/solver.py` & `solverpy-0.1.1/src/solverpy/solver/pluginsolver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,48 @@
-import time
+import logging
+from .solver import Solver
 
-def updated(call):
-   def inner(self, instance, strategy):
-      result = self.query(instance, strategy)
-      if result: 
-         return result
-      # the original "call"
-      (output, result) = call(self, instance, strategy)
-      # 
-      self.update(instance, strategy, output, result)
-      if not self.valid(result):
-         print(f"Error: solverpy: FAILED evaluation of {strategy} on {instance}")
-      return result
-   return inner
-
-class Solver:
-
-   def __init__(self, plugins=[]):
-      self.providers = []
-      self.updaters = []
+logger = logging.getLogger(__name__)
+  
+class PluginSolver(Solver):
+
+   def __init__(self, plugins=[], name=None):
+      Solver.__init__(self, name=name)
+      self.decorators = []
       self.translators = []
       self.init(plugins)
 
-   @updated
    def solve(self, instance, strategy):
-      output = self.run(instance, strategy)
-      result = self.process(output)
-      return (output, result)
-
-   # abstract methods:
-
-   def run(self, instance, strategy):
-      raise NotImlementedError()
-
-   def process(self, output):
-      raise NotImlementedError()
-
-   def solved(self, result, limit=None):
-      raise NotImlementedError()
-
-   # plugins control:
-
+      (output, result) = super().solve(instance, strategy)
+      self.update(instance, strategy, output, result)
+      if not self.valid(result):
+         lines = output.split("\n")
+         if len(lines) > 3:
+            msg = f"{lines[2]}\n{lines[3]}" # command and first output line
+         else:
+            msg = output
+         logger.debug(f"failed solver run: {self}:{strategy} @ {instance}\n{msg}")
+      return result
+   
+   # plugins initization
    def init(self, plugins):
       for plugin in plugins:
          plugin.register(self)
-
-   def query(self, instance, strategy):
-      for plugin in self.providers:
-         result = plugin.query(instance, strategy)
-         if result: # TODO: and self.solved(result)
-            return result
-      return None
-
-   def store(self, instance, strategy, output, result):
-      for plugin in self.providers:
-         plugin.store(instance, strategy, output, result)
-
+   
+   # decorators
+   def decorate(self, cmd):
+      for plugin in self.decorators:
+         cmd = plugin.decorate(cmd)
+      return cmd
+   
    def update(self, instance, strategy, output, result):
-      for plugin in self.updaters:
+      for plugin in self.decorators:
          plugin.update(instance, strategy, output, result)
+      for plugin in self.decorators:
+         plugin.finished(instance, strategy, output, result)
+
+   # translators
+   def translate(self, instance, strategy):
+      for plugin in self.translators:
+         (instance, strategy) = plugin.translate(instance, strategy)
+      return (instance, strategy)
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/atp/lash.py` & `solverpy-0.1.1/src/solverpy/solver/atp/lash.py`

 * *Files identical despite different names*

### Comparing `solverpy-0.1.0/src/solverpy/solver/plugins/db/errors.py` & `solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from ..provider import Provider
-from ....path import bids
+from ....benchmark.path import bids
 
 NAME = "errors"
 
 class Errors(Provider):
    
    def __init__(self):
       self._path = bids.dbpath(NAME)
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/plugins/db/jsons.py` & `solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/jsons.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 import json
 
 from ..cachedprovider import CachedProvider
-from ....path import bids
+from ....benchmark.path import bids
 
 NAME = "results"
 
 class Jsons(CachedProvider):
   
-   def __init__(self, bid, sid):
-      CachedProvider.__init__(self, bid, sid)
+   def __init__(self):
+      CachedProvider.__init__(self)
 
    def cachepath(self):
+      assert(self.bid)
+      assert(self.sid)
       return os.path.join(
          bids.dbpath(NAME),
          bids.name(self.bid),
          self.sid).rstrip("/") + ".json"
 
    def cachedump(self, f):
       with open(f,"w") as fw:
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/plugins/db/outputs.py` & `solverpy-0.1.1/src/solverpy/benchmark/db/_old/pluginsolver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,64 @@
-import os
+from .solver import Solver
+  
+class PluginSolver(Solver):
 
-from ..provider import Provider
-from ....path import bids
+   def __init__(self, plugins=[]):
+      self.providers = []
+      self.decorators = []
+      self.translators = []
+      self.init(plugins)
 
-NAME = "outputs"
-
-class Outputs(Provider):
-   
-   def __init__(self):
-      self._path = bids.dbpath(NAME)
+   def solve(self, instance, strategy):
+      result = self.query(instance, strategy)
+      if not result: 
+         (output, result) = super().solve(instance, strategy)
+         self.update(instance, strategy, output, result)
+         self.store(instance, strategy, output, result)
+      else:
+         self.store(instance, strategy, None, result)
+      return result
    
-   def register(self, solver):
-      solver.providers.append(self)
-      self.solver = solver
+   def applicable(self, result):
+      return self.solved(result)
    
-   def path(self, instance, strategy):
-      (bid, problem) = instance
-      limit = self.solver.limits.limit
-      p = os.path.join(self._path, bids.name(bid,limit), strategy, problem)
-      return p
+   # plugins initization
+   def init(self, plugins):
+      for plugin in plugins:
+         plugin.register(self)
    
+   # providers
    def query(self, instance, strategy):
-      f = self.path(instance, strategy)
-      #print("QUERY", instance, strategy, f)
-      if not os.path.isfile(f):
-         return None
-      output = open(f).read()
-      result = self.solver.process(output)
-      self.solver.update(instance, strategy, output, result)
-      return result
+      for plugin in self.providers:
+         result = plugin.query(instance, strategy)
+         if result and self.applicable(result):
+            return result
+      return None
 
    def store(self, instance, strategy, output, result):
-      if not output:
-         return
-      #print("STORE", instance, strategy, result)
-      if self.solver.valid(result):
-         f = self.path(instance, strategy)
-         os.makedirs(os.path.dirname(f), exist_ok=True)
-         open(f,"w").write(output)
+      for plugin in self.providers:
+         plugin.store(instance, strategy, output, result)
+   
+   def flush(self):
+      for plugin in self.providers:
+         plugin.flush()
+
+   def reset(self, bid, sid):
+      for plugin in self.providers:
+         plugin.reset(bid, sid)
+
+   # decorators
+   def decorate(self, cmd):
+      for plugin in self.decorators:
+         cmd = plugin.decorate(cmd)
+      return cmd
+   
+   def update(self, instance, strategy, output, result):
+      for plugin in self.decorators:
+         plugin.update(instance, strategy, output, result)
+
+   # translators
+   def translate(self, instance, strategy):
+      for plugin in self.translators:
+         (instance, strategy) = plugin.translate(instance, strategy)
+      return (instance, strategy)
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/plugins/db/solved.py` & `solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/solved.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 
 from ..cachedprovider import CachedProvider
-from ....path import bids
+from ....benchmark.path import bids
 
 NAME = "solved"
 
 class Solved(CachedProvider):
    
-   def __init__(self, bid, sid):
-      CachedProvider.__init__(self, bid, sid)
+   def __init__(self):
+      CachedProvider.__init__(self)
    
    def query(self, instance, strategy):
       return None
 
    def cachepath(self):
+      assert(self.bid)
       return os.path.join(
          bids.dbpath(NAME),
          bids.name(self.bid, self.solver.limits.limit),
          self.sid).rstrip("/")
 
    def cachedump(self, f):
       solved = [p for (p,r) in self.cache.items()
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/plugins/db/status.py` & `solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 from ..cachedprovider import CachedProvider
-from ....path import bids
+from ....benchmark.path import bids
 
 NAME = "status"
 
 class Status(CachedProvider):
    
-   def __init__(self, bid, sid):
-      CachedProvider.__init__(self, bid, sid)
+   def __init__(self):
+      CachedProvider.__init__(self)
    
    def query(self, instance, strategy):
       return None
 
    def cachepath(self):
       return os.path.join(
          bids.dbpath(NAME),
@@ -25,11 +25,14 @@
       status.sort()
       status = "\n".join(status) + ("\n" if status else "")
       with open(f,"w") as fw: fw.write(status)
 
    def cacheload(self, f):
       if not os.path.isfile(f): 
          return {}
-      solved = open(f).read().strip().split("\n")
+      solved = open(f).read().strip()
+      if not solved:
+         return {}
+      solved = solved.split("\n")
       solved = dict(x.rsplit(":",1) for x in solved)
       return {x:dict(status=y) for (x,y) in solved.items()}
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/plugins/db/yamls.py` & `solverpy-0.1.1/src/solverpy/benchmark/db/_old/plugins/db/yamls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import yaml
 
 from ..cachedprovider import CachedProvider
-from ....path import bids
+from ....benchmark.path import bids
 
 NAME = "results"
 
 class Yamls(CachedProvider):
   
-   def __init__(self, bid, sid):
-      CachedProvider.__init__(self, bid, sid)
+   def __init__(self):
+      CachedProvider.__init__(self)
 
    def cachepath(self):
       return os.path.join(
          bids.dbpath(NAME),
          bids.name(self.bid),
          self.sid).rstrip("/") + ".yaml"
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/smt/cvc5.py` & `solverpy-0.1.1/src/solverpy/solver/smt/cvc5.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 import re
 from ..smtsolver import SmtSolver
 from ...tools import patterns, human
 
 CVC5_BINARY = "cvc5"
 
-CVC5_STATIC = "--produce-proofs --dump-instantiations --print-inst-full " +\
-              "--stats --stats-internal --track-relevant-literals"
+#CVC5_STATIC = "--produce-proofs --dump-instantiations --print-inst-full " +\
+#              "--stats --stats-internal --track-relevant-literals"
+
+CVC5_STATIC = "--stats --stats-internal"
 
 CVC5_BUILDER = {
    "T": lambda x: "--tlimit=%s" % (1000*int(x)),
    "R": lambda x: "--rlimit=%s" % x
 }
 
 CVC5_KEYS = [
    "driver::totalTime",
+   "global::totalTime",
    "resource::resourceUnitsUsed",
    "resource::steps::resource",
    "Instantiate::[^ ]*",
+   "QuantifiersEngine::[^ ]*",
    "SharedTermsDatabase::termsCount",
    "sat::conflicts",
    "sat::decisions",
    "sat::clauses_literals",
    "sat::propagations",
 ]
 
-CVC5_PAT = re.compile(r"^(%s) = (.*)$" % "|".join(CVC5_KEYS), flags=re.MULTILINE)
+CVC5_TIMEOUT = re.compile(r"cvc5 interrupted by (timeout)")
 
 class Cvc5(SmtSolver):
    
-   def __init__(self, limit, binary=CVC5_BINARY, static=CVC5_STATIC, plugins=[]):
+   def __init__(self, limit, binary=CVC5_BINARY, static=CVC5_STATIC, plugins=[], keys=CVC5_KEYS):
       cmd = f"{binary} {static}"
       SmtSolver.__init__(self, cmd, limit, CVC5_BUILDER, plugins, wait=1)
+      self.pattern = re.compile(r"^(%s) = (.*)$" % "|".join(keys), flags=re.MULTILINE)
    
    def process(self, output):
       
       def parseval(val):
          if val.startswith("{") and val.endswith("}"):
             val = val.strip(" {}")
             val = val.split(",")
             val = [x.split(":") for x in val]
             return {x.strip():human.numeric(y.strip()) for (x,y) in val}
          return human.numeric(val)
       
-      result = patterns.keyval(CVC5_PAT, output)
+      result = patterns.keyval(self.pattern, output)
       result = patterns.mapval(result, parseval)
+      timeouted = patterns.single(CVC5_TIMEOUT, output, None)
+      if timeouted:
+         result["status"] = timeouted # timeouted == "timeout"
       return result
```

### Comparing `solverpy-0.1.0/src/solverpy/solver/smt/z3.py` & `solverpy-0.1.1/src/solverpy/solver/smt/z3.py`

 * *Files identical despite different names*

### Comparing `solverpy-0.1.0/src/solverpy/solver/timedsolver.py` & `solverpy-0.1.1/src/solverpy/benchmark/db/_old/timedsolver.py`

 * *Files identical despite different names*

### Comparing `solverpy-0.1.0/src/solverpy/tools/bars.py` & `solverpy-0.1.1/src/_dust/bars.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from tqdm import tqdm
 
-BAR_DEFAULT = "{desc}: {percentage:.3f}%|{bar}| {n_fmt}/{total_fmt} [{elapsed}<{remaining}]{postfix}"
+BAR_DEFAULT = "{desc}: {percentage:6.3f}%|{bar}| {n_fmt}/{total_fmt} [{elapsed}<{remaining}]{postfix}"
 
-BAR_SOLVED = "{desc}: {percentage:.3f}%|{bar}| {n_fmt}/{total_fmt} +{solved}/-{failed}/!{errors}/?{solved_eta:.0f} [{elapsed}<{remaining}]{postfix}"
+BAR_SOLVED = "{desc}: {percentage:6.3f}%|{bar}| {n_fmt}/{total_fmt} +{solved}/-{failed}/!{errors}/?{solved_eta:.0f} [{elapsed}<{remaining}]{postfix}"
 
 class SolvedBar(tqdm):
 
    def __init__(self, *args, **kwargs):
       self._solved = 0
       self._failed = 0
       self._errors = 0
@@ -32,13 +32,17 @@
       self._failed += n
 
    def update_errors(self, n=1):
       self._errors += n
 
 #
 
-def default(total, desc):
-   return tqdm(total=total, desc=desc, bar_format=BAR_DEFAULT)
+def default(total, desc, *args, **kwargs):
+   return tqdm(total=total, desc=desc, bar_format=BAR_DEFAULT, ascii="┈─═━", colour="green", *args, **kwargs)
+
+def solved(total, desc, *args, **kwargs):
+   #return SolvedBar(total=total, desc=desc, ascii="░▒█")
+   return SolvedBar(total=total, desc=desc, ascii="┈─═━", colour="blue", *args, **kwargs)
+   #return SolvedBar(total=total, desc=desc, ascii="┈▏ ▎ ▍ ▌ ▋ ▊ ▉█", colour="blue")
+
 
-def solved(total, desc):
-   return SolvedBar(total=total, desc=desc)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `solverpy-0.1.0/src/solverpy/tools/par.py` & `solverpy-0.1.1/src/_dust/par.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,39 +10,47 @@
    results = runner.get(WAIT)
    pool.close()
    pool.join()
    return results
 
 def apply(fun, args, cores=4, chunksize=1, bar=None, callback=None):
    pool = Pool(cores)
-   m = Manager()
-   queue = m.Queue()
-   todo = len(args)
-   #if bar: bar = tqdm(total=todo, desc=bar ,bar_format=bar_format) #, ncols=80, ascii="ox") 
-   if isinstance(bar,str): bar = bars.default(todo, bar)
-   queuedata = callback is not None
-   args = [(fun,job,queue,queuedata) for job in args]
-   runner = pool.starmap_async(runjob, args, chunksize=chunksize)
-   while todo:
-      res = queue.get(WAIT)
-      if callback:
-         callback(res, bar)
-      todo -= 1
-      if bar: bar.update(1)
-   if bar: bar.close()
-   pool.close()
-   pool.join()
-   return None if queuedata else runner.get(WAIT)
+   try:
+      m = Manager()
+      queue = m.Queue()
+      todo = len(args)
+      #if bar: bar = tqdm(total=todo, desc=bar ,bar_format=bar_format) #, ncols=80, ascii="ox") 
+      if isinstance(bar,str): bar = bars.default(todo, bar)
+      queuedata = callback is not None
+      args = [(fun,job,queue,queuedata) for job in args]
+      runner = pool.starmap_async(runjob, args, chunksize=chunksize)
+      while todo:
+         res = queue.get(WAIT)
+         if callback:
+            callback(res, bar)
+         todo -= 1
+         if bar: bar.update(1)
+      if bar: bar.close()
+      pool.close()
+      pool.join()
+      return None if queuedata else runner.get(WAIT)
+   except KeyboardInterrupt as e:
+      if bar: bar.close()
+      pool.terminate()
+      raise e
 
 def runjob(fun, job, queue, queuedata):
    result = None
    try:
       result = fun(*job)
    except Exception as e:
       print(e)
       import traceback
       print("Error: "+traceback.format_exc())
       print(job)
+      return None
+   except KeyboardInterrupt:
+      return None
    # send the result throught the queue or return it
    queue.put(result if queuedata else "DONE")
    return None if queuedata else result
```

### Comparing `solverpy-0.1.0/src/solverpy.egg-info/PKG-INFO` & `solverpy-0.1.1/src/solverpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solverpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python inteface for Automated Reasoning (AR) solvers, provers, and checkers.
 Project-URL: Homepage, https://github.com/cbboyan/solverpy
 Project-URL: Bug Tracker, https://github.com/cbboyan/solverpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

