# Comparing `tmp/autumn8-1.0.5rc4.tar.gz` & `tmp/autumn8-1.0.5rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.5rc4.tar", last modified: Mon May 15 13:52:43 2023, max compression
+gzip compressed data, was "autumn8-1.0.5rc5.tar", last modified: Mon May 15 15:00:54 2023, max compression
```

## Comparing `autumn8-1.0.5rc4.tar` & `autumn8-1.0.5rc5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.466127 autumn8-1.0.5rc4/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-15 13:52:43.466127 autumn8-1.0.5rc4/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-15 13:51:44.000000 autumn8-1.0.5rc4/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.456127 autumn8-1.0.5rc4/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc4/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.456127 autumn8-1.0.5rc4/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc4/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc4/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.456127 autumn8-1.0.5rc4/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    13135 2023-05-15 13:48:17.000000 autumn8-1.0.5rc4/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16089 2023-05-15 12:34:48.000000 autumn8-1.0.5rc4/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc4/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4094 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.456127 autumn8-1.0.5rc4/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-15 13:48:59.000000 autumn8-1.0.5rc4/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.456127 autumn8-1.0.5rc4/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc4/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.466127 autumn8-1.0.5rc4/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc4/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc4/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc4/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc4/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc4/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.466127 autumn8-1.0.5rc4/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc4/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc4/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.466127 autumn8-1.0.5rc4/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.466127 autumn8-1.0.5rc4/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11804 2023-05-15 13:48:17.000000 autumn8-1.0.5rc4/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1446 2023-05-15 13:48:17.000000 autumn8-1.0.5rc4/autumn8/lib/api/user.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc4/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.456127 autumn8-1.0.5rc4/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-15 13:52:43.000000 autumn8-1.0.5rc4/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1436 2023-05-15 13:52:43.000000 autumn8-1.0.5rc4/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-15 13:52:43.000000 autumn8-1.0.5rc4/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-15 13:52:43.000000 autumn8-1.0.5rc4/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-15 13:52:43.000000 autumn8-1.0.5rc4/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-15 13:52:43.000000 autumn8-1.0.5rc4/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-15 13:52:43.466127 autumn8-1.0.5rc4/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 13:52:43.466127 autumn8-1.0.5rc4/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc4/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-15 13:51:44.000000 autumn8-1.0.5rc5/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    13237 2023-05-15 15:00:03.000000 autumn8-1.0.5rc5/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16089 2023-05-15 12:34:48.000000 autumn8-1.0.5rc5/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4094 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-15 15:00:22.000000 autumn8-1.0.5rc5/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc5/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc5/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc5/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc5/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc5/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11875 2023-05-15 15:00:03.000000 autumn8-1.0.5rc5/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-15 15:00:03.000000 autumn8-1.0.5rc5/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc5/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1436 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/tests/test_settings.py
```

### Comparing `autumn8-1.0.5rc4/PKG-INFO` & `autumn8-1.0.5rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc4
+Version: 1.0.5rc5
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc4/README.md` & `autumn8-1.0.5rc5/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/cli/analyze.py` & `autumn8-1.0.5rc5/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/cli/cli_environment.py` & `autumn8-1.0.5rc5/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/cli/commands/cloud.py` & `autumn8-1.0.5rc5/autumn8/cli/commands/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,15 @@
     quiet: bool,
     docker_image_name: str = "",
     docker_port: Optional[int] = None,
     docker_container_registry: Optional[
         str
     ] = DEFAULT_DOCKER_CONTAINER_REGISTRY,
     container_http_request_path: str = "",
+    # disabled, cause these are not working properly right now on a8f
     # docker_environment: Optional[Dict[str, str]] = None,
     # docker_entrypoint: Optional[str] = None,
     input: Union[Dict[str, str], List[str], str, None] = None,
 ):
     """
     Run an inference on a given Docker image by creating
     a temporary container and calling an HTTP request against it
@@ -318,19 +319,19 @@
             "docker-processing",
             query,
             container_http_request_path,
         )
         response: httpx.Response = await httpClient.post(
             url=url,
             json={
-                "input": input,
-                "container_name": docker_image_name,
+                "container_image_name": docker_image_name,
                 "container_registry": docker_container_registry,
-                "container_path": container_http_request_path,
-                "port": docker_port,
+                "container_port": docker_port,
+                "http_request_input": input,
+                "http_request_path": container_http_request_path,
             },
             timeout=None,
         )
 
         logger.info("Container responded with:")
         click.echo(response.text)
         response.raise_for_status()
```

### Comparing `autumn8-1.0.5rc4/autumn8/cli/commands/models.py` & `autumn8-1.0.5rc5/autumn8/cli/commands/models.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/cli/examples.py` & `autumn8-1.0.5rc5/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/cli/interactive.py` & `autumn8-1.0.5rc5/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/cli/main.py` & `autumn8-1.0.5rc5/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/cli/options.py` & `autumn8-1.0.5rc5/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/cli/pending_uploads.py` & `autumn8-1.0.5rc5/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/cli/validation.py` & `autumn8-1.0.5rc5/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/common/config/cloud_info.py` & `autumn8-1.0.5rc5/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/common/config/settings.py` & `autumn8-1.0.5rc5/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/common/config/supported_instances.py` & `autumn8-1.0.5rc5/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/common/types.py` & `autumn8-1.0.5rc5/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/env/__init__.py` & `autumn8-1.0.5rc5/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/examples/mnist.py` & `autumn8-1.0.5rc5/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/examples/model.py` & `autumn8-1.0.5rc5/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.5rc5/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.5rc5/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/lib/__init__.py` & `autumn8-1.0.5rc5/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/lib/api/cloud.py` & `autumn8-1.0.5rc5/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/lib/api/lab.py` & `autumn8-1.0.5rc5/autumn8/lib/api/lab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import io
 import json
+import os
 from threading import Lock
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
 import appdirs
 import boto3
 import httpx
 import requests
@@ -173,35 +174,38 @@
         auth=HTTPBasicAuth(*retrieve_api_creds()),
     )
 
     require_ok_response(response)
     return FileUploadPermissionsResponse(response.json())
 
 
-def get_s3_client_from_temporary_permissions(
+def get_s3_resource_from_temporary_permissions(
     environment: CliEnvironment, permissions: FileUploadPermissionsResponse
 ):
     credentials = permissions["credentials"]
-    S3 = boto3.resource(
-        "s3",
-        endpoint_url=environment.value.s3_host,
+
+    session = boto3.Session(
         aws_access_key_id=credentials["AccessKeyId"],
         aws_secret_access_key=credentials["SecretAccessKey"],
         aws_session_token=credentials["SessionToken"],
     )
 
-    return S3
+    s3 = session.resource(
+        "s3", endpoint_url=environment.value.s3_host, region_name="us-east-1"
+    )
+
+    return s3
 
 
 def normal_upload(
     environment: CliEnvironment,
     permissions: FileUploadPermissionsResponse,
     file,
 ):
-    S3 = get_s3_client_from_temporary_permissions(environment, permissions)
+    S3 = get_s3_resource_from_temporary_permissions(environment, permissions)
 
     object_key = permissions["object_key"]
     S3.Bucket(permissions["bucket_name"]).Object(object_key).upload_fileobj(
         file
     )
     return object_key
 
@@ -270,15 +274,15 @@
     # max total upload size is 100GB
     part_size_in_bytes = max(
         10 * 1024**2, total_bytes // 500
     )  # minimum part size on aws is 5MB, list part returns max 1000 parts
 
     # we have to use low-level API to be able to support
     # resumable uploads - https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpu-upload-object.html
-    s3_client = get_s3_client_from_temporary_permissions(
+    s3_client = get_s3_resource_from_temporary_permissions(
         environment, permissions
     ).meta.client
     s3_bucket_name = permissions["bucket_name"]
     compatible_s3_file_url = permissions["object_key"]
 
     if mpu_id != None:
         print(f"Resuming upload with id {mpu_id}")
```

### Comparing `autumn8-1.0.5rc4/autumn8/lib/api/user.py` & `autumn8-1.0.5rc5/autumn8/lib/api/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 
 
 def fetch_org_api_keys(environment: CliEnvironment, organization_id: int):
     user_id, api_key = retrieve_api_creds()
     autodl_host = environment.value.app_host
 
     response = requests.get(
-        # TODO: change url after prod gets updated
-        # user_api_url(environment, f"inference_api_keys"),
-        f"{autodl_host}/api/admin/api_keys",
+        user_api_url(environment, f"inference_api_keys"),
         params={"organization_id": organization_id},
         headers={"Content-Type": "application/json"},
         auth=HTTPBasicAuth(user_id, api_key),
     )
     require_ok_response(response)
     return response.json()["api_keys"]
```

### Comparing `autumn8-1.0.5rc4/autumn8/lib/api_creds.py` & `autumn8-1.0.5rc5/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/lib/asyncio.py` & `autumn8-1.0.5rc5/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/lib/http.py` & `autumn8-1.0.5rc5/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/lib/logging.py` & `autumn8-1.0.5rc5/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/lib/logging.yaml` & `autumn8-1.0.5rc5/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/lib/package_resolver.py` & `autumn8-1.0.5rc5/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8/lib/service.py` & `autumn8-1.0.5rc5/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.5rc5/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc4
+Version: 1.0.5rc5
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc4/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.5rc5/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/pyproject.toml` & `autumn8-1.0.5rc5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.5rc5/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc4/tests/test_settings.py` & `autumn8-1.0.5rc5/tests/test_settings.py`

 * *Files identical despite different names*

