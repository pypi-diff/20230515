# Comparing `tmp/dvc-render-0.4.0.tar.gz` & `tmp/dvc-render-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-render-0.4.0.tar", last modified: Fri Apr 21 19:43:43 2023, max compression
+gzip compressed data, was "dvc-render-0.5.0.tar", last modified: Mon May 15 17:37:03 2023, max compression
```

## Comparing `dvc-render-0.4.0.tar` & `dvc-render-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.249693 dvc-render-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.241693 dvc-render-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.241693 dvc-render-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-21 19:43:15.000000 dvc-render-0.4.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-21 19:43:15.000000 dvc-render-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-21 19:43:15.000000 dvc-render-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-21 19:43:43.249693 dvc-render-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-21 19:43:15.000000 dvc-render-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.241693 dvc-render-0.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.241693 dvc-render-0.4.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-21 19:43:15.000000 dvc-render-0.4.0/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-21 19:43:15.000000 dvc-render-0.4.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 19:43:15.000000 dvc-render-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-21 19:43:15.000000 dvc-render-0.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-21 19:43:15.000000 dvc-render-0.4.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-21 19:43:15.000000 dvc-render-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-21 19:43:43.249693 dvc-render-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.237693 dvc-render-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.245693 dvc-render-0.4.0/src/dvc_render/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/plotly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/vega.py
--rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/vega_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.245693 dvc-render-0.4.0/src/dvc_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:43:42.000000 dvc-render-0.4.0/src/dvc_render.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.249693 dvc-render-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_vega.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.766903 dvc-render-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-15 17:36:41.000000 dvc-render-0.5.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-15 17:36:41.000000 dvc-render-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-15 17:36:41.000000 dvc-render-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-15 17:37:03.766903 dvc-render-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-15 17:36:41.000000 dvc-render-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-15 17:36:41.000000 dvc-render-0.5.0/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 17:36:41.000000 dvc-render-0.5.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 17:36:41.000000 dvc-render-0.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-15 17:36:41.000000 dvc-render-0.5.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-15 17:36:41.000000 dvc-render-0.5.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-15 17:36:41.000000 dvc-render-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-15 17:37:03.766903 dvc-render-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.766903 dvc-render-0.5.0/src/dvc_render/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/vega.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23900 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/vega_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.766903 dvc-render-0.5.0/src/dvc_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.766903 dvc-render-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_vega.py
```

### Comparing `dvc-render-0.4.0/.cruft.json` & `dvc-render-0.5.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/.github/dependabot.yml` & `dvc-render-0.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/.github/workflows/docs.yml` & `dvc-render-0.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/.github/workflows/release.yml` & `dvc-render-0.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/.github/workflows/tests.yml` & `dvc-render-0.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/.gitignore` & `dvc-render-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/.pre-commit-config.yaml` & `dvc-render-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/CODE_OF_CONDUCT.rst` & `dvc-render-0.5.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/CONTRIBUTING.rst` & `dvc-render-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/LICENSE` & `dvc-render-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/PKG-INFO` & `dvc-render-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-render
-Version: 0.4.0
+Version: 0.5.0
 Summary: DVC render
 Home-page: https://github.com/iterative/dvc-render
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-render-0.4.0/README.rst` & `dvc-render-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/docs/assets/logo.svg` & `dvc-render-0.5.0/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/docs/gen_ref_pages.py` & `dvc-render-0.5.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/mkdocs.yml` & `dvc-render-0.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/noxfile.py` & `dvc-render-0.5.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/pyproject.toml` & `dvc-render-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/setup.cfg` & `dvc-render-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 package_dir = 
 	=src
 packages = find:
 
 [options.extras_require]
 table = 
 	tabulate>=0.8.7
+	flatten_dict<1,>=0.4.1
 markdown = 
 	%(table)s
 	matplotlib
 docs = 
 	mkdocs==1.3.1
 	mkdocs-gen-files==0.3.5
 	mkdocs-material==8.4.1
```

### Comparing `dvc-render-0.4.0/src/dvc_render/base.py` & `dvc-render-0.5.0/src/dvc_render/base.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/src/dvc_render/html.py` & `dvc-render-0.5.0/src/dvc_render/html.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/src/dvc_render/image.py` & `dvc-render-0.5.0/src/dvc_render/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,12 +51,12 @@
         return ""
 
     def generate_markdown(self, report_path=None) -> str:
         content = []
         for datapoint in self.datapoints:
             src = datapoint[self.SRC_FIELD]
             if src.startswith("data:image;base64"):
-                raise ValueError("`generate_markdown` doesn't support base64")
+                src = src.replace("data:image;base64", "data:image/png;base64")
             content.append(f"\n![{datapoint[self.TITLE_FIELD]}]({src})")
         if content:
             return "\n".join(content)
         return ""
```

### Comparing `dvc-render-0.4.0/src/dvc_render/markdown.py` & `dvc-render-0.5.0/src/dvc_render/markdown.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,27 +42,32 @@
         for placeholder, value in kwargs.items():
             self.template = self.template.replace("{" + placeholder + "}", value)
         return self.template
 
 
 def render_markdown(
     renderers: List["Renderer"],
-    output_file: "StrPath",
+    output_file: Optional["StrPath"] = None,
     template_path: Optional["StrPath"] = None,
 ) -> "StrPath":
     "User renderers to fill an Markdown template and write to path."
-    output_path = Path(output_file)
-    output_path.parent.mkdir(exist_ok=True)
+    output_path = None
+    if output_file:
+        output_path = Path(output_file)
+        output_path.parent.mkdir(exist_ok=True)
 
     page = None
     if template_path:
         with open(template_path, encoding="utf-8") as fobj:
             page = fobj.read()
 
     document = Markdown(page)
 
     for renderer in renderers:
         document.with_element(renderer.generate_markdown(report_path=output_path))
 
-    output_path.write_text(document.embed(), encoding="utf8")
+    if output_file and output_path:
+        output_path.write_text(document.embed(), encoding="utf8")
 
-    return output_file
+        return output_file
+
+    return document.embed()
```

### Comparing `dvc-render-0.4.0/src/dvc_render/plotly.py` & `dvc-render-0.5.0/src/dvc_render/plotly.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/src/dvc_render/table.py` & `dvc-render-0.5.0/src/dvc_render/table.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/src/dvc_render/vega.py` & `dvc-render-0.5.0/src/dvc_render/vega.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import base64
+import io
 import json
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 from warnings import warn
 
 from .base import Renderer
 from .utils import list_dict_to_dict_list
@@ -98,27 +100,39 @@
         try:
             from matplotlib import pyplot as plt
         except ImportError as e:
             raise ImportError("matplotlib is required for `generate_markdown`") from e
 
         data = list_dict_to_dict_list(self.datapoints)
         if data:
-            report_folder = Path(report_path).parent
-            output_file = report_folder / self.name
-            output_file = output_file.with_suffix(".png")
-            output_file.parent.mkdir(exist_ok=True, parents=True)
+            if report_path:
+                report_folder = Path(report_path).parent
+                output_file = report_folder / self.name
+                output_file = output_file.with_suffix(".png")
+                output_file.parent.mkdir(exist_ok=True, parents=True)
+            else:
+                output_file = io.BytesIO()  # type: ignore
 
             x = self.properties.get("x")
             y = self.properties.get("y")
             data[x] = list(map(float, data[x]))
             data[y] = list(map(float, data[y]))
 
-            plt.title(self.properties.get("title", output_file.stem))
+            plt.title(self.properties.get("title", Path(self.name).stem))
             plt.xlabel(self.properties.get("x_label", x))
             plt.ylabel(self.properties.get("y_label", y))
             plt.plot(x, y, data=data)
             plt.tight_layout()
             plt.savefig(output_file)
             plt.close()
 
-            return f"\n![{self.name}]({output_file.relative_to(report_folder)})"
+            if report_path:
+                return f"\n![{self.name}]({output_file.relative_to(report_folder)})"
+
+            base64_str = base64.b64encode(
+                output_file.getvalue()  # type: ignore
+            ).decode()
+            src = f"data:image/png;base64,{base64_str}"
+
+            return f"\n![{self.name}]({src})"
+
         return ""
```

### Comparing `dvc-render-0.4.0/src/dvc_render/vega_templates.py` & `dvc-render-0.5.0/src/dvc_render/vega_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -509,36 +509,80 @@
                         "title": Template.anchor("y_label"),
                         "scale": {"zero": False},
                     },
                     "color": {
                         "field": "rev",
                         "type": "nominal",
                     },
+                    "tooltip": [
+                        {
+                            "field": Template.anchor("x"),
+                            "title": Template.anchor("x_label"),
+                            "type": "quantitative",
+                        },
+                        {
+                            "field": Template.anchor("y"),
+                            "title": Template.anchor("y_label"),
+                            "type": "quantitative",
+                        },
+                    ],
                 },
                 "transform": [
                     {
                         "loess": Template.anchor("y"),
                         "on": Template.anchor("x"),
                         "groupby": ["rev", "filename", "field", "filename::field"],
                         "bandwidth": {"signal": "smooth"},
                     },
                 ],
             },
             {
+                "mark": {"type": "line", "opacity": 0.2},
+                "encoding": {
+                    "x": {
+                        "field": Template.anchor("x"),
+                        "type": "quantitative",
+                        "title": Template.anchor("x_label"),
+                    },
+                    "y": {
+                        "field": Template.anchor("y"),
+                        "type": "quantitative",
+                        "title": Template.anchor("y_label"),
+                        "scale": {"zero": False},
+                    },
+                    "color": {"field": "rev", "type": "nominal"},
+                    "tooltip": [
+                        {
+                            "field": Template.anchor("x"),
+                            "title": Template.anchor("x_label"),
+                            "type": "quantitative",
+                        },
+                        {
+                            "field": Template.anchor("y"),
+                            "title": Template.anchor("y_label"),
+                            "type": "quantitative",
+                        },
+                    ],
+                },
+            },
+            {
                 "mark": {
-                    "type": "point",
-                    "tooltip": {"content": "data"},
+                    "type": "circle",
+                    "size": 10,
+                    "tooltip": {"content": "encoding"},
                 },
                 "encoding": {
                     "x": {
+                        "aggregate": "max",
                         "field": Template.anchor("x"),
                         "type": "quantitative",
                         "title": Template.anchor("x_label"),
                     },
                     "y": {
+                        "aggregate": {"argmax": Template.anchor("x")},
                         "field": Template.anchor("y"),
                         "type": "quantitative",
                         "title": Template.anchor("y_label"),
                         "scale": {"zero": False},
                     },
                     "color": {"field": "rev", "type": "nominal"},
                 },
```

### Comparing `dvc-render-0.4.0/src/dvc_render.egg-info/PKG-INFO` & `dvc-render-0.5.0/src/dvc_render.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-render
-Version: 0.4.0
+Version: 0.5.0
 Summary: DVC render
 Home-page: https://github.com/iterative/dvc-render
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-render-0.4.0/src/dvc_render.egg-info/SOURCES.txt` & `dvc-render-0.5.0/src/dvc_render.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/src/dvc_render.egg-info/requires.txt` & `dvc-render-0.5.0/src/dvc_render.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 [dev]
 tabulate>=0.8.7
+flatten_dict<1,>=0.4.1
 matplotlib
 funcy>=1.17
 pytest==7.2.0
 pytest-sugar==0.9.5
 pytest-cov==3.0.0
 pytest-mock==3.8.2
 pylint==2.15.0
@@ -21,21 +22,24 @@
 mkdocs-gen-files==0.3.5
 mkdocs-material==8.4.1
 mkdocs-section-index==0.3.4
 mkdocstrings-python==0.7.1
 
 [markdown]
 tabulate>=0.8.7
+flatten_dict<1,>=0.4.1
 matplotlib
 
 [table]
 tabulate>=0.8.7
+flatten_dict<1,>=0.4.1
 
 [tests]
 tabulate>=0.8.7
+flatten_dict<1,>=0.4.1
 matplotlib
 funcy>=1.17
 pytest==7.2.0
 pytest-sugar==0.9.5
 pytest-cov==3.0.0
 pytest-mock==3.8.2
 pylint==2.15.0
```

### Comparing `dvc-render-0.4.0/tests/test_html.py` & `dvc-render-0.5.0/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/tests/test_image.py` & `dvc-render-0.5.0/tests/test_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,16 +59,17 @@
 def test_invalid_generate_markdown():
     datapoints = [
         {
             "rev": "workspace",
             "src": "data:image;base64,encoded_image",
         }
     ]
-    with pytest.raises(ValueError, match="`generate_markdown` doesn't support base64"):
-        ImageRenderer(datapoints, "file.jpg").generate_markdown()
+    md = ImageRenderer(datapoints, "file.jpg").generate_markdown()
+
+    assert "![workspace](data:image/png;base64,encoded_image)" in md
 
 
 @pytest.mark.parametrize(
     "html_path,img_path,expected_path",
     [
         (
             os.path.join("output", "path", "index.html"),
```

### Comparing `dvc-render-0.4.0/tests/test_markdown.py` & `dvc-render-0.5.0/tests/test_markdown.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import pytest
 
-from dvc_render.markdown import PAGE_MARKDOWN, Markdown, MissingPlaceholderError
+from dvc_render.markdown import (
+    PAGE_MARKDOWN,
+    Markdown,
+    MissingPlaceholderError,
+    render_markdown,
+)
 
 # pylint: disable=missing-function-docstring, R0801
 
 
 CUSTOM_PAGE_MARKDOWN = """# CUSTOM REPORT
 
 {renderers}
@@ -22,21 +27,30 @@
         (
             CUSTOM_PAGE_MARKDOWN,
             ["content"],
             CUSTOM_PAGE_MARKDOWN.format(renderers="content"),
         ),
     ],
 )
-def test_html(template, page_elements, expected_page):
+def test_markdown(template, page_elements, expected_page):
     page = Markdown(template)
     page.elements = page_elements
 
     result = page.embed()
 
     assert result == expected_page
 
 
 def test_no_placeholder():
     template = "# Missing Placeholder"
 
     with pytest.raises(MissingPlaceholderError):
         Markdown(template)
+
+
+def test_render_markdown_to_file(tmp_dir):
+    output_file = tmp_dir / "report"
+    assert output_file == render_markdown([], output_file)
+
+
+def test_render_markdown_no_file():
+    assert "# DVC Report" in render_markdown([])
```

### Comparing `dvc-render-0.4.0/tests/test_parallel_coordinates.py` & `dvc-render-0.5.0/tests/test_parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/tests/test_table.py` & `dvc-render-0.5.0/tests/test_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,7 +20,15 @@
         {"foo": 1, "bar": 2},
     ]
     md = TableRenderer(datapoints, "metrics.json").generate_markdown()
     assert "metrics.json\n\n" in md
     assert "|   foo |   bar |" in md
     assert "|-------|-------|" in md
     assert "|     1 |     2 |" in md
+
+
+def test_nested():
+    datapoints = [{"foo": {"bar": 1}}]
+    html = TableRenderer(datapoints, "metrics.json").generate_html()
+    assert "<p>metrics_json</p>" in html
+    assert '<tr><th style="text-align: right;">  foo.bar</th></tr>' in html
+    assert '<tr><td style="text-align: right;">        1</td></tr>' in html
```

### Comparing `dvc-render-0.4.0/tests/test_templates.py` & `dvc-render-0.5.0/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.4.0/tests/test_vega.py` & `dvc-render-0.5.0/tests/test_vega.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,20 @@
         {"first_val": 200, "second_val": 300, "val": 3},
     ]
 
     plot_content = VegaRenderer(datapoints, "foo").get_filled_template(as_string=False)
 
     assert plot_content["layer"][0]["mark"] == "line"
 
-    assert plot_content["layer"][1]["mark"] == {
-        "type": "point",
-        "tooltip": {"content": "data"},
+    assert plot_content["layer"][1]["mark"] == {"type": "line", "opacity": 0.2}
+
+    assert plot_content["layer"][2]["mark"] == {
+        "type": "circle",
+        "size": 10,
+        "tooltip": {"content": "encoding"},
     }
 
 
 def test_choose_axes():
     props = {"x": "first_val", "y": "second_val"}
     datapoints = [
         {"first_val": 100, "second_val": 100, "val": 2},
@@ -111,15 +114,17 @@
     renderer = VegaRenderer(datapoints, "foo", **props)
     with pytest.raises(NoFieldInDataError):
         renderer.get_filled_template()
     renderer.get_filled_template(strict=False)
 
 
 @pytest.mark.parametrize("name", ["foo", "foo/bar", "foo/bar.tsv"])
-def test_generate_markdown(tmp_dir, mocker, name):
+@pytest.mark.parametrize("to_file", [True, False])
+def test_generate_markdown(tmp_dir, mocker, name, to_file):
+    # pylint: disable-msg=too-many-locals
     import matplotlib.pyplot
 
     plot = mocker.spy(matplotlib.pyplot, "plot")
     title = mocker.spy(matplotlib.pyplot, "title")
     xlabel = mocker.spy(matplotlib.pyplot, "xlabel")
     ylabel = mocker.spy(matplotlib.pyplot, "ylabel")
     savefig = mocker.spy(matplotlib.pyplot, "savefig")
@@ -127,31 +132,38 @@
     props = {"x": "first_val", "y": "second_val", "title": "FOO"}
     datapoints = [
         {"first_val": 100.0, "second_val": 100.0, "val": 2.0},
         {"first_val": 200.0, "second_val": 300.0, "val": 3.0},
     ]
     renderer = VegaRenderer(datapoints, name, **props)
 
-    (tmp_dir / "output").mkdir()
-    renderer.generate_markdown(tmp_dir / "output" / "report.md")
+    if to_file:
+        report_folder = tmp_dir / "output"
+        report_folder.mkdir()
+        md = renderer.generate_markdown(tmp_dir / "output" / "report.md")
+        output_file = (tmp_dir / "output" / renderer.name).with_suffix(".png")
+        assert output_file.exists()
+        savefig.assert_called_with(output_file)
+        assert f"![{name}]({output_file.relative_to(report_folder)})" in md
+    else:
+        md = renderer.generate_markdown()
+        assert f"![{name}](data:image/png;base64," in md
 
-    assert (tmp_dir / "output" / renderer.name).with_suffix(".png").exists()
     plot.assert_called_with(
         "first_val",
         "second_val",
         data={
             "first_val": [100.0, 200.0],
             "second_val": [100.0, 300.0],
             "val": [2, 3],
         },
     )
     title.assert_called_with("FOO")
     xlabel.assert_called_with("first_val")
     ylabel.assert_called_with("second_val")
-    savefig.assert_called_with((tmp_dir / "output" / name).with_suffix(".png"))
 
 
 def test_unsupported_template():
     datapoints = [
         {"predicted": "B", "actual": "A"},
         {"predicted": "A", "actual": "A"},
     ]
```

