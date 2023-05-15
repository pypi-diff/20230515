# Comparing `tmp/wes_palette-0.1.1.tar.gz` & `tmp/wes_palette-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wes_palette-0.1.1.tar", last modified: Mon May 15 04:28:40 2023, max compression
+gzip compressed data, was "wes_palette-0.1.2.tar", last modified: Mon May 15 17:53:10 2023, max compression
```

## Comparing `wes_palette-0.1.1.tar` & `wes_palette-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,48 @@
-drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 04:28:40.458668 wes_palette-0.1.1/
--rw-r--r--   0 arauhr     (501) staff       (20)      311 2023-05-14 15:38:54.000000 wes_palette-0.1.1/.bumpversion.cfg
--rw-r--r--   0 arauhr     (501) staff       (20)     1059 2023-05-14 15:38:54.000000 wes_palette-0.1.1/LICENSE
--rw-r--r--   0 arauhr     (501) staff       (20)      357 2023-05-14 15:38:54.000000 wes_palette-0.1.1/MANIFEST.in
--rw-r--r--   0 arauhr     (501) staff       (20)     2261 2023-05-14 21:46:02.000000 wes_palette-0.1.1/Makefile
--rw-r--r--   0 arauhr     (501) staff       (20)     4270 2023-05-15 04:28:40.457902 wes_palette-0.1.1/PKG-INFO
--rw-r--r--   0 arauhr     (501) staff       (20)     2211 2023-05-15 04:16:47.000000 wes_palette-0.1.1/README.md
--rw-r--r--   0 arauhr     (501) staff       (20)     2181 2023-05-15 04:16:48.000000 wes_palette-0.1.1/pyproject.toml
--rw-r--r--   0 arauhr     (501) staff       (20)       38 2023-05-15 04:28:40.458890 wes_palette-0.1.1/setup.cfg
--rw-r--r--   0 arauhr     (501) staff       (20)       39 2023-05-14 15:38:54.000000 wes_palette-0.1.1/setup.py
-drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 04:28:40.450359 wes_palette-0.1.1/tests/
--rw-r--r--   0 arauhr     (501) staff       (20)     2110 2023-05-14 17:21:26.000000 wes_palette-0.1.1/tests/test_all.py
-drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 04:28:40.452394 wes_palette-0.1.1/wes_palette/
--rw-r--r--   0 arauhr     (501) staff       (20)        0 2023-05-14 15:46:05.000000 wes_palette-0.1.1/wes_palette/__init__.py
--rw-r--r--   0 arauhr     (501) staff       (20)     4384 2023-05-14 17:21:26.000000 wes_palette-0.1.1/wes_palette/wes_palette.py
-drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 04:28:40.456844 wes_palette-0.1.1/wes_palette.egg-info/
--rw-r--r--   0 arauhr     (501) staff       (20)     4270 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/PKG-INFO
--rw-r--r--   0 arauhr     (501) staff       (20)      322 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/SOURCES.txt
--rw-r--r--   0 arauhr     (501) staff       (20)        1 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/dependency_links.txt
--rw-r--r--   0 arauhr     (501) staff       (20)      156 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/requires.txt
--rw-r--r--   0 arauhr     (501) staff       (20)       12 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/top_level.txt
+drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 17:53:10.809594 wes_palette-0.1.2/
+-rw-r--r--   0 arauhr     (501) staff       (20)      311 2023-05-15 16:11:26.000000 wes_palette-0.1.2/.bumpversion.cfg
+-rw-r--r--   0 arauhr     (501) staff       (20)     1423 2023-05-15 16:11:26.000000 wes_palette-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 arauhr     (501) staff       (20)     5202 2023-05-15 16:11:26.000000 wes_palette-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 arauhr     (501) staff       (20)      403 2023-05-15 16:11:26.000000 wes_palette-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 arauhr     (501) staff       (20)     1059 2023-05-15 16:11:26.000000 wes_palette-0.1.2/LICENSE
+-rw-r--r--   0 arauhr     (501) staff       (20)      430 2023-05-15 16:11:26.000000 wes_palette-0.1.2/MANIFEST.in
+-rw-r--r--   0 arauhr     (501) staff       (20)     2261 2023-05-15 16:11:26.000000 wes_palette-0.1.2/Makefile
+-rw-r--r--   0 arauhr     (501) staff       (20)     4265 2023-05-15 17:53:10.808883 wes_palette-0.1.2/PKG-INFO
+-rw-r--r--   0 arauhr     (501) staff       (20)     2206 2023-05-15 17:32:29.000000 wes_palette-0.1.2/README.md
+drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 17:53:10.796105 wes_palette-0.1.2/docs/
+-rw-r--r--   0 arauhr     (501) staff       (20)     5202 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/code_of_conduct.md
+-rw-r--r--   0 arauhr     (501) staff       (20)      403 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/contributing.md
+-rw-r--r--   0 arauhr     (501) staff       (20)    74152 2023-05-15 17:21:11.000000 wes_palette-0.1.2/docs/displot.png
+-rw-r--r--   0 arauhr     (501) staff       (20)   431265 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/examplegraph1.png
+-rw-r--r--   0 arauhr     (501) staff       (20)   446182 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/examplegraph2.png
+-rw-r--r--   0 arauhr     (501) staff       (20)   411704 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/examplegraph3.png
+-rw-r--r--   0 arauhr     (501) staff       (20)     1944 2023-05-15 17:21:11.000000 wes_palette-0.1.2/docs/examples.md
+-rw-r--r--   0 arauhr     (501) staff       (20)   431265 2023-05-15 17:21:11.000000 wes_palette-0.1.2/docs/heatmap.png
+-rw-r--r--   0 arauhr     (501) staff       (20)      536 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/index.md
+-rw-r--r--   0 arauhr     (501) staff       (20)       46 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/installation.md
+-rw-r--r--   0 arauhr     (501) staff       (20)     1059 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/license.md
+-rw-r--r--   0 arauhr     (501) staff       (20)     2211 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/overview.md
+-rw-r--r--   0 arauhr     (501) staff       (20)   384513 2023-05-15 17:21:11.000000 wes_palette-0.1.2/docs/pairplot.png
+-rw-r--r--   0 arauhr     (501) staff       (20)   401832 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/palettes.png
+-rw-r--r--   0 arauhr     (501) staff       (20)      207 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/reference.md
+-rw-r--r--   0 arauhr     (501) staff       (20)      513 2023-05-15 16:11:26.000000 wes_palette-0.1.2/docs/requirements.txt
+-rw-r--r--   0 arauhr     (501) staff       (20)   431265 2023-05-15 17:32:29.000000 wes_palette-0.1.2/ex1.png
+-rw-r--r--   0 arauhr     (501) staff       (20)    74152 2023-05-15 17:32:29.000000 wes_palette-0.1.2/ex2.png
+-rw-r--r--   0 arauhr     (501) staff       (20)   384513 2023-05-15 17:32:29.000000 wes_palette-0.1.2/ex3.png
+-rw-r--r--   0 arauhr     (501) staff       (20)      695 2023-05-15 16:11:26.000000 wes_palette-0.1.2/mkdocs.yml
+-rw-r--r--   0 arauhr     (501) staff       (20)   401832 2023-05-14 15:38:54.000000 wes_palette-0.1.2/palettes.png
+-rw-r--r--   0 arauhr     (501) staff       (20)     2227 2023-05-15 17:52:52.000000 wes_palette-0.1.2/pyproject.toml
+-rw-r--r--   0 arauhr     (501) staff       (20)       38 2023-05-15 17:53:10.809749 wes_palette-0.1.2/setup.cfg
+-rw-r--r--   0 arauhr     (501) staff       (20)       39 2023-05-15 16:11:26.000000 wes_palette-0.1.2/setup.py
+drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 17:53:10.799695 wes_palette-0.1.2/tests/
+-rw-r--r--   0 arauhr     (501) staff       (20)    22805 2023-05-15 17:14:37.000000 wes_palette-0.1.2/tests/test.png
+-rw-r--r--   0 arauhr     (501) staff       (20)     2110 2023-05-15 16:11:26.000000 wes_palette-0.1.2/tests/test_all.py
+-rw-r--r--   0 arauhr     (501) staff       (20)    22805 2023-05-15 16:11:26.000000 wes_palette-0.1.2/tests/wes.png
+drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 17:53:10.802285 wes_palette-0.1.2/wes_palette/
+-rw-r--r--   0 arauhr     (501) staff       (20)      207 2023-05-15 17:31:13.000000 wes_palette-0.1.2/wes_palette/__init__.py
+-rw-r--r--   0 arauhr     (501) staff       (20)     6353 2023-05-15 17:16:55.000000 wes_palette-0.1.2/wes_palette/wes_palette.py
+drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 17:53:10.807730 wes_palette-0.1.2/wes_palette.egg-info/
+-rw-r--r--   0 arauhr     (501) staff       (20)     4265 2023-05-15 17:53:10.000000 wes_palette-0.1.2/wes_palette.egg-info/PKG-INFO
+-rw-r--r--   0 arauhr     (501) staff       (20)      767 2023-05-15 17:53:10.000000 wes_palette-0.1.2/wes_palette.egg-info/SOURCES.txt
+-rw-r--r--   0 arauhr     (501) staff       (20)        1 2023-05-15 17:53:10.000000 wes_palette-0.1.2/wes_palette.egg-info/dependency_links.txt
+-rw-r--r--   0 arauhr     (501) staff       (20)      156 2023-05-15 17:53:10.000000 wes_palette-0.1.2/wes_palette.egg-info/requires.txt
+-rw-r--r--   0 arauhr     (501) staff       (20)       12 2023-05-15 17:53:10.000000 wes_palette-0.1.2/wes_palette.egg-info/top_level.txt
```

### Comparing `wes_palette-0.1.1/LICENSE` & `wes_palette-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wes_palette-0.1.1/Makefile` & `wes_palette-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `wes_palette-0.1.1/PKG-INFO` & `wes_palette-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wes_palette
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wes Anderson film color palette extension for matplotlib
 Author-email: AU <au2232@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 AU
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,17 +41,17 @@
 License-File: LICENSE
 
 ## wes-palette
 
 [![PyPI](https://img.shields.io/pypi/v/wes-palette)](https://pypi.org/project/wes-palette/)
 [![license](https://img.shields.io/github/license/au2232/wes-palette)](https://github.com/au2232/wes-palette/LICENSE)
 [![issues](https://img.shields.io/github/issues/au2232/wes-palette)](https://github.com/au2232/wes-palette/issues)
-[![build](https://img.shields.io/github/actions/workflow/status/au2232/wes_palette/build.yml)](https://github.com/au2232/wes_palette/actions/workflows/build.yml)
-[![docs](https://img.shields.io/github/actions/workflow/status/au2232/wes-palette/docs.yml?label=docs)](https://ew2664.github.io/wes-palette/)
-[![coverage](https://img.shields.io/codecov/c/github/au2232/wes_palette?token=5542beb1-1af8-4185-8340-fda0d36d528a)](https://coveralls.io/github/au2232/wes-palette)
+[![Build Status](https://github.com/au2232/wes_palette/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/au2232/wes_palette/actions?query=workflow%3A%22Build+Status%22)
+[![docs](https://img.shields.io/github/actions/workflow/status/au2232/wes-palette/mkdocs.yml?label=docs)](https://au2232.github.io/wes-palette/)
+[![coverage](https://img.shields.io/codecov/c/github/au2232/wes_palette?token=5542beb1-1af8-4185-8340-fda0d36d528a)](https://codecov.io/github/au2232/wes-palette)
 
 
 
 wes-palette is a Wes Anderson film color palettes for matplotlib based on [vapeplot](https://github.com/dantaki/vapeplot)
 
 ## Installation
 
@@ -99,17 +99,17 @@
 
     # Draw the heatmap with the mask and correct aspect ratio
     sns.heatmap(corr, mask=mask, cmap=cmap, vmax=.3, center=0,
             square=True, linewidths=.5, cbar_kws={"shrink": .5})
 
     plt.show()
     
-![example](examplegraph1.png)
-![example](examplegraph2.png)
-![example](examplegraph3.png)
+![example](ex1.png)
+![example](ex2.png)
+![example](ex3.png)
 
 ## Contributing
 
 See CONTRIBUTING.md
 
 ## License
```

### Comparing `wes_palette-0.1.1/README.md` & `wes_palette-0.1.2/docs/overview.md`

 * *Files identical despite different names*

### Comparing `wes_palette-0.1.1/pyproject.toml` & `wes_palette-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "wes_palette"
 authors = [{name = "AU", email = "au2232@columbia.edu"}]
 description="Wes Anderson film color palette extension for matplotlib"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -46,14 +46,17 @@
     "mypy",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "twine",
     "wheel",
 ]
 
+[tool.setuptools]
+packages = ['wes_palette']
+
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
 
 [tool.check-manifest]
```

### Comparing `wes_palette-0.1.1/tests/test_all.py` & `wes_palette-0.1.2/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `wes_palette-0.1.1/wes_palette.egg-info/PKG-INFO` & `wes_palette-0.1.2/wes_palette.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wes-palette
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wes Anderson film color palette extension for matplotlib
 Author-email: AU <au2232@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 AU
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,17 +41,17 @@
 License-File: LICENSE
 
 ## wes-palette
 
 [![PyPI](https://img.shields.io/pypi/v/wes-palette)](https://pypi.org/project/wes-palette/)
 [![license](https://img.shields.io/github/license/au2232/wes-palette)](https://github.com/au2232/wes-palette/LICENSE)
 [![issues](https://img.shields.io/github/issues/au2232/wes-palette)](https://github.com/au2232/wes-palette/issues)
-[![build](https://img.shields.io/github/actions/workflow/status/au2232/wes_palette/build.yml)](https://github.com/au2232/wes_palette/actions/workflows/build.yml)
-[![docs](https://img.shields.io/github/actions/workflow/status/au2232/wes-palette/docs.yml?label=docs)](https://ew2664.github.io/wes-palette/)
-[![coverage](https://img.shields.io/codecov/c/github/au2232/wes_palette?token=5542beb1-1af8-4185-8340-fda0d36d528a)](https://coveralls.io/github/au2232/wes-palette)
+[![Build Status](https://github.com/au2232/wes_palette/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/au2232/wes_palette/actions?query=workflow%3A%22Build+Status%22)
+[![docs](https://img.shields.io/github/actions/workflow/status/au2232/wes-palette/mkdocs.yml?label=docs)](https://au2232.github.io/wes-palette/)
+[![coverage](https://img.shields.io/codecov/c/github/au2232/wes_palette?token=5542beb1-1af8-4185-8340-fda0d36d528a)](https://codecov.io/github/au2232/wes-palette)
 
 
 
 wes-palette is a Wes Anderson film color palettes for matplotlib based on [vapeplot](https://github.com/dantaki/vapeplot)
 
 ## Installation
 
@@ -99,17 +99,17 @@
 
     # Draw the heatmap with the mask and correct aspect ratio
     sns.heatmap(corr, mask=mask, cmap=cmap, vmax=.3, center=0,
             square=True, linewidths=.5, cbar_kws={"shrink": .5})
 
     plt.show()
     
-![example](examplegraph1.png)
-![example](examplegraph2.png)
-![example](examplegraph3.png)
+![example](ex1.png)
+![example](ex2.png)
+![example](ex3.png)
 
 ## Contributing
 
 See CONTRIBUTING.md
 
 ## License
```

