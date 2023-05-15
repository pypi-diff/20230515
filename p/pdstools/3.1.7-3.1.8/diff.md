# Comparing `tmp/pdstools-3.1.7.tar.gz` & `tmp/pdstools-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.1.7.tar", last modified: Wed Apr 26 09:20:18 2023, max compression
+gzip compressed data, was "pdstools-3.1.8.tar", last modified: Mon May 15 13:40:59 2023, max compression
```

## Comparing `pdstools-3.1.7.tar` & `pdstools-3.1.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 09:20:06.000000 pdstools-3.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-26 09:20:18.192341 pdstools-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-26 09:20:06.000000 pdstools-3.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.188341 pdstools-3.1.7/pdstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 09:20:06.000000 pdstools-3.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.188341 pdstools-3.1.7/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.188341 pdstools-3.1.7/python/pdstools/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.188341 pdstools-3.1.7/python/pdstools/adm/
--rw-r--r--   0 runner    (1001) docker     (123)    56177 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/adm/Tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/app/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/app/Home.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/app/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/app/pages/Health Check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/ih/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/ih/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/pega_io/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/pega_io/API.py
--rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/pega_io/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/pega_io/S3.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/plots/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/reports/
--rw-r--r--   0 runner    (1001) docker     (123)    39159 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/reports/HealthCheckModel.qmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/pega_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/polars_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/table_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/valuefinder/
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:20:18.192341 pdstools-3.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.787946 pdstools-3.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 13:40:47.000000 pdstools-3.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-15 13:40:59.787946 pdstools-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-15 13:40:47.000000 pdstools-3.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 13:40:59.000000 pdstools-3.1.8/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-15 13:40:47.000000 pdstools-3.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.775946 pdstools-3.1.8/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)    56265 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/app/pages/Health Check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.779945 pdstools-3.1.8/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.783946 pdstools-3.1.8/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.783946 pdstools-3.1.8/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.783946 pdstools-3.1.8/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    39159 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/reports/HealthCheckModel.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.787946 pdstools-3.1.8/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17946 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/table_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:59.787946 pdstools-3.1.8/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:40:47.000000 pdstools-3.1.8/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:40:59.787946 pdstools-3.1.8/setup.cfg
```

### Comparing `pdstools-3.1.7/LICENSE` & `pdstools-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/PKG-INFO` & `pdstools-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.7
+Version: 3.1.8
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.7 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.8 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.7/README.md` & `pdstools-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/pdstools.egg-info/PKG-INFO` & `pdstools-3.1.8/pdstools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.7
+Version: 3.1.8
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.7 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.8 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.7/pdstools.egg-info/SOURCES.txt` & `pdstools-3.1.8/pdstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/pyproject.toml` & `pdstools-3.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 requires-python = ">=3.8"
 
 [tool.setuptools.dynamic]
 version = {attr="pdstools.__version__"}
 
 [project.optional-dependencies]
 docs = ['sphinx','furo','sphinx-autoapi','nbsphinx','sphinx-copybutton','myst-parser']
-app = ['streamlit>=1.20', 'quarto', 'papermill', 'itables', 'pandas>=1.5.3', 'jinja2>=3.1']
+app = ['streamlit>=1.20', 'quarto', 'papermill', 'itables', 'pandas>=1.5.3', 'jinja2>=3.1', 'xlsxwriter>=3.0']
 
 [project.urls]
 "Homepage" = "https://github.com/pegasystems/pega-datascientist-tools"
 "Bug Tracker" = "https://github.com/pegasystems/pega-datascientist-tools/issues"
 "Wiki" = "https://github.com/pegasystems/pega-datascientist-tools/wiki"
 "Docs" = "https://pegasystems.github.io/pega-datascientist-tools/"
```

### Comparing `pdstools-3.1.7/python/pdstools/__init__.py` & `pdstools-3.1.8/python/pdstools/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Python pdstools"""
 
-__version__ = "3.1.7"
+__version__ = "3.1.8"
 
 from polars import enable_string_cache
 
 enable_string_cache(True)
 
 import sys
 from pathlib import Path
 
 from .adm.ADMDatamart import ADMDatamart
 from .adm.ADMTrees import ADMTrees, MultiTrees
-from .pega_io import getToken, readClientCredentialFile, readDSExport
+from .pega_io import getToken, readDSExport
 from .pega_io import File, API, S3
+from .pega_io.API import setupAzureOpenAI
 from .utils import cdh_utils, datasets, errors, hds_utils
 from .utils.cdh_utils import defaultPredictorCategorization
 from .utils.show_versions import show_versions
 from .utils.datasets import CDHSample, SampleTrees, SampleValueFinder
 from .utils.hds_utils import Config, DataAnonymization
 from .utils.table_definitions import PegaDefaultTables
 from .valuefinder.ValueFinder import ValueFinder
```

### Comparing `pdstools-3.1.7/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.1.8/python/pdstools/adm/ADMDatamart.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,17 +563,17 @@
         Parameters
         ----------
         col : Literal['ResponseCount', 'Positives']
             The column to calculate the diff for
         """
 
         return (
-            pl.col("SnapshotTime")
-            .where(pl.col(col).diff() != 0)
-            .max()
+            pl.when(pl.col(col).min() == pl.col(col).max())
+            .then(pl.max("SnapshotTime"))
+            .otherwise(pl.col("SnapshotTime").where(pl.col(col).diff() != 0).max())
             .over("ModelID")
             .alias(f"Last_{col}")
         )
 
     def _get_combined_data(
         self, last=True, strategy: Literal["eager", "lazy"] = "eager"
     ) -> any_frame:
```

### Comparing `pdstools-3.1.7/python/pdstools/adm/ADMTrees.py` & `pdstools-3.1.8/python/pdstools/adm/ADMTrees.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/adm/Tables.py` & `pdstools-3.1.8/python/pdstools/adm/Tables.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/app/cli.py` & `pdstools-3.1.8/python/pdstools/app/cli.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/app/pages/Health Check.py` & `pdstools-3.1.8/python/pdstools/app/pages/Health Check.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.1.8/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/ih/legacy_IH.py` & `pdstools-3.1.8/python/pdstools/ih/legacy_IH.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/pega_io/File.py` & `pdstools-3.1.8/python/pdstools/pega_io/File.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/pega_io/S3.py` & `pdstools-3.1.8/python/pdstools/pega_io/S3.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/plots/plot_base.py` & `pdstools-3.1.8/python/pdstools/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/plots/plots_plotly.py` & `pdstools-3.1.8/python/pdstools/plots/plots_plotly.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.1.8/python/pdstools/reports/HealthCheck.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/reports/HealthCheckModel.qmd` & `pdstools-3.1.8/python/pdstools/reports/HealthCheckModel.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/utils/cdh_utils.py` & `pdstools-3.1.8/python/pdstools/utils/cdh_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/utils/datasets.py` & `pdstools-3.1.8/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/utils/hds_utils.py` & `pdstools-3.1.8/python/pdstools/utils/hds_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         outcome_column: str = "Decision_Outcome",
         positive_outcomes: list = ["Accepted", "Clicked"],
         negative_outcomes: list = ["Rejected", "Impression"],
         special_predictors: list = [
             "Decision_DecisionTime",
             "Decision_OutcomeTime",
             "Decision_Rank",
-            "Decision_SubjectID",
         ],
         sample_percentage_schema_inferencing: float = 0.01,
     ):
         self._opts = {key: value for key, value in vars().items() if key != "self"}
 
         if config_file is not None:
             self.load_from_config_file(config_file)
@@ -254,15 +253,17 @@
                 """Files not found. Please check the `hds_folder` 
                 and check if there are `.json` files in there. 
                 If preferred, you can also supply a polars Dataframe or Lazyframe 
                 directly with the `df` argument."""
             )
         out = []
         for file in files:
-            out.append(pl.scan_ndjson(file).with_columns(filename=file))
+            out.append(
+                pl.scan_ndjson(file).with_columns(pl.lit(str(file)).alias("filename"))
+            )
 
         df = pl.concat(out, how="diagonal")
         return df
 
     def read_predictor_type_from_file(self, df: pl.LazyFrame):
         """Infer the types of the preditors from the data.
```

### Comparing `pdstools-3.1.7/python/pdstools/utils/pega_template.py` & `pdstools-3.1.8/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/utils/polars_ext.py` & `pdstools-3.1.8/python/pdstools/utils/polars_ext.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/utils/show_versions.py` & `pdstools-3.1.8/python/pdstools/utils/show_versions.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     ---Streamlit app dependencies---
     streamlit: 1.20.0
     quarto: 0.1.0
     papermill: 2.4.0
     itables: 1.5.1
     pandas: 1.5.3
     jinja2: 3.1.2
+    xlsxwriter: 3.0
     """
 
     # note: we import 'platform' here as a micro-optimisation for initial import
     import platform
 
     print("---Version info---")
     print(f"pdstools: {__version__}")
@@ -77,14 +78,15 @@
     opt_deps = [
         "streamlit",
         "quarto",
         "papermill",
         "itables",
         "pandas",
         "jinja2",
+        "xlsxwriter",
     ]
     return {name: _get_dependency_version(name) for name in opt_deps}
 
 
 def _get_dependency_version(dep_name: str) -> str:
     try:
         module = importlib.import_module(dep_name)
```

### Comparing `pdstools-3.1.7/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.1.8/python/pdstools/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/utils/table_definitions.py` & `pdstools-3.1.8/python/pdstools/utils/table_definitions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.7/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.1.8/python/pdstools/valuefinder/ValueFinder.py`

 * *Files identical despite different names*

