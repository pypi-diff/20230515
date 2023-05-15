# Comparing `tmp/vgd_counterfactuals-0.1.1.tar.gz` & `tmp/vgd_counterfactuals-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgd_counterfactuals-0.1.1.tar", max compression
+gzip compressed data, was "vgd_counterfactuals-0.1.2.tar", max compression
```

## Comparing `vgd_counterfactuals-0.1.1.tar` & `vgd_counterfactuals-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.1/LICENSE
--rwxr-xr-x   0        0        0     6577 2023-05-10 10:47:16.579832 vgd_counterfactuals-0.1.1/README.rst
--rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.1/banner.png
--rwxr-xr-x   0        0        0     1514 2023-05-10 10:47:16.571832 vgd_counterfactuals-0.1.1/pyproject.toml
--rwxr-xr-x   0        0        0        5 2023-05-10 10:47:16.579832 vgd_counterfactuals-0.1.1/vgd_counterfactuals/VERSION
--rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.1/vgd_counterfactuals/__init__.py
--rw-r--r--   0        0        0     6867 2023-05-01 16:03:23.965909 vgd_counterfactuals-0.1.1/vgd_counterfactuals/base.py
--rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/cli.py
--rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/00_quickstart.py
--rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/01_visualization.py
--rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/README.rst
--rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/__init__.py
--rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
--rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
--rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
--rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
--rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
--rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
--rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
--rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
--rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
--rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
--rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
--rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
--rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
--rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
--rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
--rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
--rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
--rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
--rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
--rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
--rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
--rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
--rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
--rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
--rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
--rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
--rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/README.rst
--rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/results/README.rst
--rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/template_experiment.py
--rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/template_experiment_sub.py
--rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/__init__.py
--rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3752 2023-05-10 10:46:22.791428 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
--rw-r--r--   0        0        0     6040 2023-05-10 10:46:22.147423 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/molecules.py
--rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/smiles_one_step_changes.py
--rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/templates/article.tex.j2
--rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.1/vgd_counterfactuals/testing.py
--rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.1/vgd_counterfactuals/utils.py
--rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.1/vgd_counterfactuals/visualization.py
--rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     6577 2023-05-15 12:12:06.827871 vgd_counterfactuals-0.1.2/README.rst
+-rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.2/banner.png
+-rwxr-xr-x   0        0        0     1514 2023-05-15 12:12:06.815871 vgd_counterfactuals-0.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0        5 2023-05-15 12:12:06.827871 vgd_counterfactuals-0.1.2/vgd_counterfactuals/VERSION
+-rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.2/vgd_counterfactuals/__init__.py
+-rw-r--r--   0        0        0     6867 2023-05-01 16:03:23.965909 vgd_counterfactuals-0.1.2/vgd_counterfactuals/base.py
+-rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.2/vgd_counterfactuals/cli.py
+-rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/00_quickstart.py
+-rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/01_visualization.py
+-rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/__init__.py
+-rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
+-rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
+-rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
+-rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
+-rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
+-rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
+-rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
+-rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
+-rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
+-rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
+-rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
+-rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
+-rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
+-rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
+-rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
+-rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
+-rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
+-rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
+-rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
+-rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
+-rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
+-rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
+-rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
+-rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
+-rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
+-rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
+-rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.2/vgd_counterfactuals/experiments/README.rst
+-rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.2/vgd_counterfactuals/experiments/results/README.rst
+-rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.2/vgd_counterfactuals/experiments/template_experiment.py
+-rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.2/vgd_counterfactuals/experiments/template_experiment_sub.py
+-rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.2/vgd_counterfactuals/generate/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.2/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6697 2023-05-15 12:10:39.475247 vgd_counterfactuals-0.1.2/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
+-rw-r--r--   0        0        0     9534 2023-05-15 12:10:38.963244 vgd_counterfactuals-0.1.2/vgd_counterfactuals/generate/molecules.py
+-rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.2/vgd_counterfactuals/generate/smiles_one_step_changes.py
+-rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.2/vgd_counterfactuals/templates/article.tex.j2
+-rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.2/vgd_counterfactuals/testing.py
+-rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.2/vgd_counterfactuals/utils.py
+-rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.2/vgd_counterfactuals/visualization.py
+-rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.2/PKG-INFO
```

### Comparing `vgd_counterfactuals-0.1.1/LICENSE` & `vgd_counterfactuals-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/README.rst` & `vgd_counterfactuals-0.1.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.1-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.2-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

### Comparing `vgd_counterfactuals-0.1.1/banner.png` & `vgd_counterfactuals-0.1.2/banner.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/pyproject.toml` & `vgd_counterfactuals-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vgd_counterfactuals"
-version = "0.1.1"
+version = "0.1.2"
 description = "Counterfactual explanations for GNNs based on the visual graph dataset format"
 license = "MIT license"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural networks", "counterfactuals", "explainable AI"]
 packages = [
```

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/base.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/base.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/cli.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/cli.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/00_quickstart.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/00_quickstart.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/01_visualization.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/01_visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/code.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/code.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/README.rst` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/template_experiment.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/experiments/template_experiment.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/template_experiment_sub.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/experiments/template_experiment_sub.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/smiles_one_step_changes.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/generate/smiles_one_step_changes.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/templates/article.tex.j2` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/utils.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/utils.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/vgd_counterfactuals/visualization.py` & `vgd_counterfactuals-0.1.2/vgd_counterfactuals/visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.1/PKG-INFO` & `vgd_counterfactuals-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgd-counterfactuals
-Version: 0.1.1
+Version: 0.1.2
 Summary: Counterfactual explanations for GNNs based on the visual graph dataset format
 License: MIT
 Keywords: graph neural networks,counterfactuals,explainable AI
 Author: Jonas Teufel
 Author-email: jonseb1998@gmail.com
 Maintainer: Jonas Teufel
 Maintainer-email: jonseb1998@gmail.com
@@ -32,15 +32,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.1-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.2-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

