# Comparing `tmp/dvc-studio-client-0.9.0.tar.gz` & `tmp/dvc-studio-client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-studio-client-0.9.0.tar", last modified: Thu May  4 14:50:32 2023, max compression
+gzip compressed data, was "dvc-studio-client-0.9.1.tar", last modified: Mon May 15 19:13:15 2023, max compression
```

## Comparing `dvc-studio-client-0.9.0.tar` & `dvc-studio-client-0.9.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.575607 dvc-studio-client-0.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.575607 dvc-studio-client-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/leaked-secrets-scan.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.575607 dvc-studio-client-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/src/dvc_studio_client/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/post_live_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/src/dvc_studio_client/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 14:50:32.000000 dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:50:32.579607 dvc-studio-client-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-04 14:50:18.000000 dvc-studio-client-0.9.0/tests/test_post_live_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/leaked-secrets-scan.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/src/dvc_studio_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/post_live_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/tests/test_post_live_metrics.py
```

### Comparing `dvc-studio-client-0.9.0/.cruft.json` & `dvc-studio-client-0.9.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/.github/dependabot.yml` & `dvc-studio-client-0.9.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/.github/workflows/docs.yml` & `dvc-studio-client-0.9.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/.github/workflows/leaked-secrets-scan.yaml` & `dvc-studio-client-0.9.1/.github/workflows/leaked-secrets-scan.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -12,13 +12,13 @@
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: TruffleHog OSS
-        uses: trufflesecurity/trufflehog@40868952497a035edd4833fad140a903b5cb4fe5
+        uses: trufflesecurity/trufflehog@4c04bbbe851403f27d0c60ef85f57ce8cb674dcc
         with:
           path: ./
           base: ${{ github.event.repository.default_branch }}
           head: HEAD
           extra_args: --debug --only-verified
```

### Comparing `dvc-studio-client-0.9.0/.github/workflows/pre-commit.yml` & `dvc-studio-client-0.9.1/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/.github/workflows/release.yml` & `dvc-studio-client-0.9.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/.github/workflows/tests.yml` & `dvc-studio-client-0.9.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/.gitignore` & `dvc-studio-client-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/.pre-commit-config.yaml` & `dvc-studio-client-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/CODE_OF_CONDUCT.rst` & `dvc-studio-client-0.9.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/CONTRIBUTING.rst` & `dvc-studio-client-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/LICENSE` & `dvc-studio-client-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/PKG-INFO` & `dvc-studio-client-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/dvc-studio-client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.9.0/README.rst` & `dvc-studio-client-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/docs/assets/logo.svg` & `dvc-studio-client-0.9.1/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/docs/gen_ref_pages.py` & `dvc-studio-client-0.9.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/mkdocs.yml` & `dvc-studio-client-0.9.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/pyproject.toml` & `dvc-studio-client-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/setup.cfg` & `dvc-studio-client-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/src/dvc_studio_client/schema.py` & `dvc-studio-client-0.9.1/src/dvc_studio_client/schema.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/PKG-INFO` & `dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/dvc-studio-client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.9.0/src/dvc_studio_client.egg-info/SOURCES.txt` & `dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.0/tests/test_post_live_metrics.py` & `dvc-studio-client-0.9.1/tests/test_post_live_metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,52 +2,156 @@
 import os
 
 import pytest
 from dulwich.porcelain import clone, init
 from requests import RequestException
 
 from dvc_studio_client.env import (
+    DVC_STUDIO_OFFLINE,
+    DVC_STUDIO_REPO_URL,
     DVC_STUDIO_TOKEN,
     DVC_STUDIO_URL,
     STUDIO_REPO_URL,
     STUDIO_TOKEN,
 )
 from dvc_studio_client.post_live_metrics import (
+    STUDIO_URL,
     _get_remote_url,
-    get_studio_token_and_repo_url,
+    get_studio_config,
     post_live_metrics,
 )
 
 
 def test_get_url(monkeypatch, tmp_path_factory):
     source = os.fspath(tmp_path_factory.mktemp("source"))
     target = os.fspath(tmp_path_factory.mktemp("target"))
     with init(source), clone(source, target):
         monkeypatch.chdir(target)
         assert _get_remote_url() == source
 
 
-@pytest.mark.parametrize("var", [DVC_STUDIO_TOKEN, STUDIO_TOKEN])
-def test_studio_token_envvar(monkeypatch, var):
-    monkeypatch.setenv(var, "FOO_TOKEN")
-    monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
-    assert get_studio_token_and_repo_url() == ("FOO_TOKEN", "FOO_REPO_URL")
+@pytest.mark.parametrize(
+    "token,repo_url",
+    [(DVC_STUDIO_TOKEN, DVC_STUDIO_REPO_URL), (STUDIO_TOKEN, STUDIO_REPO_URL)],
+)
+def test_studio_config_envvar(monkeypatch, token, repo_url):
+    monkeypatch.setenv(token, "FOO_TOKEN")
+    monkeypatch.setenv(repo_url, "FOO_REPO_URL")
+    assert get_studio_config() == {
+        "token": "FOO_TOKEN",
+        "repo_url": "FOO_REPO_URL",
+        "url": STUDIO_URL,
+    }
+
+
+def test_studio_config_dvc_studio_config():
+    dvc_studio_config = {
+        "token": "FOO_TOKEN",
+        "repo_url": "FOO_REPO_URL",
+        "url": "FOO_URL",
+    }
+    expected = {
+        "token": "FOO_TOKEN",
+        "repo_url": "FOO_REPO_URL",
+        "url": "FOO_URL",
+    }
+    assert get_studio_config(dvc_studio_config=dvc_studio_config) == expected
+
+
+def test_studio_config_kwarg(monkeypatch):
+    expected = {
+        "token": "FOO_TOKEN",
+        "repo_url": "FOO_REPO_URL",
+        "url": "FOO_URL",
+    }
+    assert (
+        get_studio_config(
+            studio_token="FOO_TOKEN",
+            studio_repo_url="FOO_REPO_URL",
+            studio_url="FOO_URL",
+        )
+        == expected
+    )
+
+
+def test_studio_config_envvar_override(monkeypatch):
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_URL, "FOO_URL")
+    monkeypatch.setenv(DVC_STUDIO_REPO_URL, "FOO_REPO_URL")
+    dvc_studio_config = {
+        "token": "BAR_TOKEN",
+        "url": "BAR_URL",
+    }
+    expected = {
+        "token": "FOO_TOKEN",
+        "repo_url": "FOO_REPO_URL",
+        "url": "FOO_URL",
+    }
+    assert get_studio_config(dvc_studio_config=dvc_studio_config) == expected
+
+
+def test_studio_config_kwarg_override(monkeypatch):
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_REPO_URL, "FOO_REPO_URL")
+    monkeypatch.setenv(DVC_STUDIO_URL, "FOO_URL")
+    expected = {
+        "token": "BAR_TOKEN",
+        "repo_url": "BAR_REPO_URL",
+        "url": "BAR_URL",
+    }
+    assert (
+        get_studio_config(
+            studio_token="BAR_TOKEN",
+            studio_repo_url="BAR_REPO_URL",
+            studio_url="BAR_URL",
+        )
+        == expected
+    )
+
+
+@pytest.mark.parametrize(
+    "val",
+    ("1", "y", "yes", "true", True, 1),
+)
+def test_studio_config_offline(monkeypatch, val):
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_REPO_URL, "FOO_REPO_URL")
+
+    assert get_studio_config() != {}
+
+    assert get_studio_config(offline=val) == {}
+
+    monkeypatch.setenv(DVC_STUDIO_OFFLINE, val)
+    assert get_studio_config() == {}
+
+    monkeypatch.setenv(DVC_STUDIO_OFFLINE, val)
+    assert get_studio_config() == {}
+
+    assert get_studio_config(dvc_studio_config={"offline": True}) == {}
+
+
+def test_studio_config_infer_url(monkeypatch):
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_REPO_URL, "FOO_REPO_URL")
+
+    assert get_studio_config()["url"] == STUDIO_URL
 
 
 def test_post_live_metrics_skip_on_missing_token(caplog):
     with caplog.at_level(logging.DEBUG, logger="dvc_studio_client.post_live_metrics"):
         assert post_live_metrics("start", "current_rev", "fooname", "fooclient") is None
         assert caplog.records[0].message == (
             "DVC_STUDIO_TOKEN not found. Skipping `post_studio_live_metrics`"
         )
 
 
 def test_post_live_metrics_skip_on_schema_error(caplog, monkeypatch):
     monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
-    monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
+    monkeypatch.setenv(DVC_STUDIO_REPO_URL, "FOO_REPO_URL")
+    monkeypatch.setenv(DVC_STUDIO_URL, STUDIO_URL)
     with caplog.at_level(logging.DEBUG, logger="dvc_studio_client.post_live_metrics"):
         assert post_live_metrics("start", "bad_hash", "fooname", "fooclient") is None
         assert caplog.records[0].message == (
             "expected a length 40 commit sha for dictionary value @ "
             "data['baseline_sha']. Got 'bad_hash'"
         )
 
@@ -336,19 +440,18 @@
             "fooname",
             "fooclient",
         )
         is False
     )
 
 
-def test_get_studio_token_and_repo_url_skip_repo_url(monkeypatch):
+def test_get_studio_config_skip_repo_url(monkeypatch):
     monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
-    token, repo_url = get_studio_token_and_repo_url()
-    assert token is None
-    assert repo_url is None  # Skipped call to get_repo_url
+    config = get_studio_config()
+    assert config == {}  # Skipped call to get_repo_url
 
 
 def test_post_live_metrics_token_and_repo_url_args(mocker, monkeypatch):
     monkeypatch.setenv(DVC_STUDIO_URL, "https://0.0.0.0")
 
     mocked_response = mocker.MagicMock()
     mocked_response.status_code = 200
```

