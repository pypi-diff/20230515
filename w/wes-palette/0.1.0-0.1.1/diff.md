# Comparing `tmp/wes_palette-0.1.0.tar.gz` & `tmp/wes_palette-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wes_palette-0.1.0.tar", last modified: Sun May 14 15:51:58 2023, max compression
+gzip compressed data, was "wes_palette-0.1.1.tar", last modified: Mon May 15 04:28:40 2023, max compression
```

## Comparing `wes_palette-0.1.0.tar` & `wes_palette-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,21 @@
-drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-14 15:51:58.585080 wes_palette-0.1.0/
--rw-r--r--   0 arauhr     (501) staff       (20)      311 2023-05-14 15:38:54.000000 wes_palette-0.1.0/.bumpversion.cfg
--rw-r--r--   0 arauhr     (501) staff       (20)     1315 2023-05-14 15:38:54.000000 wes_palette-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 arauhr     (501) staff       (20)     5202 2023-05-14 15:38:54.000000 wes_palette-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 arauhr     (501) staff       (20)        5 2023-05-14 15:38:54.000000 wes_palette-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 arauhr     (501) staff       (20)     1059 2023-05-14 15:38:54.000000 wes_palette-0.1.0/LICENSE
--rw-r--r--   0 arauhr     (501) staff       (20)      357 2023-05-14 15:38:54.000000 wes_palette-0.1.0/MANIFEST.in
--rw-r--r--   0 arauhr     (501) staff       (20)     2262 2023-05-14 15:38:54.000000 wes_palette-0.1.0/Makefile
--rw-r--r--   0 arauhr     (501) staff       (20)     3106 2023-05-14 15:51:58.584535 wes_palette-0.1.0/PKG-INFO
--rw-r--r--   0 arauhr     (501) staff       (20)     1047 2023-05-14 15:38:54.000000 wes_palette-0.1.0/README.md
--rw-r--r--   0 arauhr     (501) staff       (20)   401832 2023-05-14 15:38:54.000000 wes_palette-0.1.0/palettes.png
--rw-r--r--   0 arauhr     (501) staff       (20)     2181 2023-05-14 15:50:29.000000 wes_palette-0.1.0/pyproject.toml
--rw-r--r--   0 arauhr     (501) staff       (20)       38 2023-05-14 15:51:58.585266 wes_palette-0.1.0/setup.cfg
--rw-r--r--   0 arauhr     (501) staff       (20)       39 2023-05-14 15:38:54.000000 wes_palette-0.1.0/setup.py
-drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-14 15:51:58.579291 wes_palette-0.1.0/wes_palette/
--rw-r--r--   0 arauhr     (501) staff       (20)        0 2023-05-14 15:46:05.000000 wes_palette-0.1.0/wes_palette/__init__.py
--rw-r--r--   0 arauhr     (501) staff       (20)    22805 2023-05-14 15:38:54.000000 wes_palette-0.1.0/wes_palette/test.png
--rw-r--r--   0 arauhr     (501) staff       (20)     2023 2023-05-14 15:38:54.000000 wes_palette-0.1.0/wes_palette/test_all.py
--rw-r--r--   0 arauhr     (501) staff       (20)    22805 2023-05-14 15:38:54.000000 wes_palette-0.1.0/wes_palette/wes.png
--rw-r--r--   0 arauhr     (501) staff       (20)     4307 2023-05-14 15:38:54.000000 wes_palette-0.1.0/wes_palette/wes_palette.py
-drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-14 15:51:58.583549 wes_palette-0.1.0/wes_palette.egg-info/
--rw-r--r--   0 arauhr     (501) staff       (20)     3106 2023-05-14 15:51:58.000000 wes_palette-0.1.0/wes_palette.egg-info/PKG-INFO
--rw-r--r--   0 arauhr     (501) staff       (20)      441 2023-05-14 15:51:58.000000 wes_palette-0.1.0/wes_palette.egg-info/SOURCES.txt
--rw-r--r--   0 arauhr     (501) staff       (20)        1 2023-05-14 15:51:58.000000 wes_palette-0.1.0/wes_palette.egg-info/dependency_links.txt
--rw-r--r--   0 arauhr     (501) staff       (20)      156 2023-05-14 15:51:58.000000 wes_palette-0.1.0/wes_palette.egg-info/requires.txt
--rw-r--r--   0 arauhr     (501) staff       (20)       12 2023-05-14 15:51:58.000000 wes_palette-0.1.0/wes_palette.egg-info/top_level.txt
+drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 04:28:40.458668 wes_palette-0.1.1/
+-rw-r--r--   0 arauhr     (501) staff       (20)      311 2023-05-14 15:38:54.000000 wes_palette-0.1.1/.bumpversion.cfg
+-rw-r--r--   0 arauhr     (501) staff       (20)     1059 2023-05-14 15:38:54.000000 wes_palette-0.1.1/LICENSE
+-rw-r--r--   0 arauhr     (501) staff       (20)      357 2023-05-14 15:38:54.000000 wes_palette-0.1.1/MANIFEST.in
+-rw-r--r--   0 arauhr     (501) staff       (20)     2261 2023-05-14 21:46:02.000000 wes_palette-0.1.1/Makefile
+-rw-r--r--   0 arauhr     (501) staff       (20)     4270 2023-05-15 04:28:40.457902 wes_palette-0.1.1/PKG-INFO
+-rw-r--r--   0 arauhr     (501) staff       (20)     2211 2023-05-15 04:16:47.000000 wes_palette-0.1.1/README.md
+-rw-r--r--   0 arauhr     (501) staff       (20)     2181 2023-05-15 04:16:48.000000 wes_palette-0.1.1/pyproject.toml
+-rw-r--r--   0 arauhr     (501) staff       (20)       38 2023-05-15 04:28:40.458890 wes_palette-0.1.1/setup.cfg
+-rw-r--r--   0 arauhr     (501) staff       (20)       39 2023-05-14 15:38:54.000000 wes_palette-0.1.1/setup.py
+drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 04:28:40.450359 wes_palette-0.1.1/tests/
+-rw-r--r--   0 arauhr     (501) staff       (20)     2110 2023-05-14 17:21:26.000000 wes_palette-0.1.1/tests/test_all.py
+drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 04:28:40.452394 wes_palette-0.1.1/wes_palette/
+-rw-r--r--   0 arauhr     (501) staff       (20)        0 2023-05-14 15:46:05.000000 wes_palette-0.1.1/wes_palette/__init__.py
+-rw-r--r--   0 arauhr     (501) staff       (20)     4384 2023-05-14 17:21:26.000000 wes_palette-0.1.1/wes_palette/wes_palette.py
+drwxr-xr-x   0 arauhr     (501) staff       (20)        0 2023-05-15 04:28:40.456844 wes_palette-0.1.1/wes_palette.egg-info/
+-rw-r--r--   0 arauhr     (501) staff       (20)     4270 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/PKG-INFO
+-rw-r--r--   0 arauhr     (501) staff       (20)      322 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/SOURCES.txt
+-rw-r--r--   0 arauhr     (501) staff       (20)        1 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/dependency_links.txt
+-rw-r--r--   0 arauhr     (501) staff       (20)      156 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/requires.txt
+-rw-r--r--   0 arauhr     (501) staff       (20)       12 2023-05-15 04:28:40.000000 wes_palette-0.1.1/wes_palette.egg-info/top_level.txt
```

### Comparing `wes_palette-0.1.0/LICENSE` & `wes_palette-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wes_palette-0.1.0/Makefile` & `wes_palette-0.1.1/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 #########
 # BUILD #
 #########
 develop:  ## install dependencies and build library
-	python -m pip install -e .[develop]
+	python3 -m pip install -e .[develop]
 
 build:  ## build the python library
-	python setup.py build build_ext --inplace
+	python3 setup.py build build_ext --inplace
 
 install:  ## install library
-	python -m pip install .
+	python3 -m pip install .
 
 #########
 # LINTS #
 #########
 lint:  ## run static analysis with flake8
-	python -m black --check wes_palette setup.py
-	python -m flake8 wes_palette setup.py
+	python3 -m black --check wes_palette setup.py
+	python3 -m flake8 wes_palette setup.py
 
 # Alias
 lints: lint
 
 format:  ## run autoformatting with black
-	python -m black wes_palette/ setup.py
+	python3 -m black wes_palette/ setup.py
 
 # alias
 fix: format
 
 check:  ## check assets for packaging
 	check-manifest -v
 
 # Alias
 checks: check
 
 annotate:  ## run type checking
-	python -m mypy ./wes_palette
+	python3 -m mypy ./wes_palette
 
 #########
 # TESTS #
 #########
 test: ## clean and run unit tests
-	python -m pytest -v wes_palette/tests
+	python3 -m pytest -v tests
 
 coverage:  ## clean and run unit tests with coverage
-	python -m pytest -v wes_palette/tests --cov=example_project_python --cov-branch --cov-fail-under=75 --cov-report term-missing
+	python3 -m pytest -v wes_palette/tests --cov=example_project_python --cov-branch --cov-fail-under=75 --cov-report term-missing
 
 # Alias
 tests: test
 
 ###########
 # VERSION #
 ###########
@@ -62,18 +62,18 @@
 major:
 	bump2version major
 
 ########
 # DIST #
 ########
 dist-build:  # Build python dist
-	python setup.py sdist bdist_wheel
+	python3 setup.py sdist bdist_wheel
 
 dist-check:
-	python -m twine check dist/*
+	python3 -m twine check dist/*
 
 dist: clean build dist-build dist-check  ## Build dists
 
 publish:  # Upload python assets
 	echo "would usually run python -m twine upload dist/* --skip-existing"
 
 #########
```

### Comparing `wes_palette-0.1.0/pyproject.toml` & `wes_palette-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "wes_palette"
 authors = [{name = "AU", email = "au2232@columbia.edu"}]
 description="Wes Anderson film color palette extension for matplotlib"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `wes_palette-0.1.0/wes_palette/test_all.py` & `wes_palette-0.1.1/tests/test_all.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 from matplotlib import rcParams
 import matplotlib.pyplot as plt
 import cycler
 import matplotlib
 import numpy as np
 import wes_palette as wes
 
+
 def test_available(show=True):
-    #wes.available()
+    wes.available()
     if not show:
         return wes.palettes.keys()
     else:
         f, ax = plt.subplots(5, 2, figsize=(5, 8))
         for i, name in enumerate(wes.palettes.keys()):
             x, y = i // 2, i % 2
             cycle = wes.palettes[name]
             for j, c in enumerate(cycle):
                 ax[x, y].hlines(j, 0, 1, colors=c, linewidth=15)
             ax[x, y].set_ylim(-1, len(cycle))
             ax[x, y].set_title(name)
             wes.despine(ax[x, y], True)
-        plt.savefig('test.png')   
-        #plt.show()
+        plt.savefig('test.png')
+        # plt.show()
     assert wes.available() == plt.show()
 
+
 test_available()
 
+
 def test_check_key():
     palettes = {
-    "megasaki":["#aa82a7","#9d2f28","#deb867","#e3ced3","#948580","#110d0e"],
-    "budapest":["#4B0100","#900403","#4E1042","#806150","#C76B4F","#D8AA88"],
-    "kingdom":["#195B4E","#617337","#B1A16A","#E1D06E","#C99A6B","#B27B7F"],
-    "darjeeling":["#0D6CE8","#8ACAF0","#ABBBC7","#687075","#3B5657","#B45E3B"],
-    "tenenbaums":["#a7ba42","#95ccba","#ffdede","#fff0cb","#f2cc84"],
-    "tracy":["#eaa2b6","#e7cbaf","#e0bd59","#292176"],
-    "dispatch":["#1f5c89","#72a87c","#c0bc78","#ce784b"],
-    "darjeeling2":["#ffe959","#b5b867","#b7dbdb","#6ba08f","#345b8e"],
-    "fantasticfox":["#4baecb","#e4d405","#df8818","#b40c24","#272121"],
-    "mendls":["#3a0202","#a03558","#b25d55","#7896d7","#dc90b5","#e0e2f4"],
+        "megasaki": ["#aa82a7", "#9d2f28", "#deb867", "#e3ced3", "#948580", "#110d0e"],
+        "budapest": ["#4B0100", "#900403", "#4E1042", "#806150", "#C76B4F", "#D8AA88"],
+        "kingdom": ["#195B4E", "#617337", "#B1A16A", "#E1D06E", "#C99A6B", "#B27B7F"],
+        "darjeeling": ["#0D6CE8", "#8ACAF0", "#ABBBC7", "#687075", "#3B5657", "#B45E3B"],
+        "tenenbaums": ["#a7ba42", "#95ccba", "#ffdede", "#fff0cb", "#f2cc84"],
+        "tracy": ["#eaa2b6", "#e7cbaf", "#e0bd59", "#292176"],
+        "dispatch": ["#1f5c89", "#72a87c", "#c0bc78", "#ce784b"],
+        "darjeeling2": ["#ffe959", "#b5b867", "#b7dbdb", "#6ba08f", "#345b8e"],
+        "fantasticfox": ["#4baecb", "#e4d405", "#df8818", "#b40c24", "#272121"],
+        "mendls": ["#3a0202", "#a03558", "#b25d55", "#7896d7", "#dc90b5", "#e0e2f4"],
     }
     assert wes.palettes.keys() == palettes.keys()
-        
+
+
 test_check_key()
 
+
 def test_cmap():
     palname = 'megasaki'
     assert wes.cmap(palname) == matplotlib.colors.ListedColormap(wes.palettes[palname])
 
+
 test_cmap()
-  
+
+
 def test_palette(palname=None):
     assert wes.palette() == wes.palettes
 
-    #print(wes.palette())
-    #print(wes.palettes)
+    # print(wes.palette())
+    # print(wes.palettes)
+
 
 test_palette()
-  
+
+
 def test_reverse():
     assert wes.reverse('megasaki') == list(reversed(wes.palette('megasaki')))
 
+
 test_reverse()
-
```

### Comparing `wes_palette-0.1.0/wes_palette/wes_palette.py` & `wes_palette-0.1.1/wes_palette/wes_palette.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 import matplotlib.pyplot as plt
 import cycler
 import matplotlib
 import numpy as np
 
 
 palettes = {
-   # "":["#","#"],
-    "megasaki":["#aa82a7","#9d2f28","#deb867","#e3ced3","#948580","#110d0e"],
-    "budapest":["#4B0100","#900403","#4E1042","#806150","#C76B4F","#D8AA88"],
-    "kingdom":["#195B4E","#617337","#B1A16A","#E1D06E","#C99A6B","#B27B7F"],
-    "darjeeling":["#0D6CE8","#8ACAF0","#ABBBC7","#687075","#3B5657","#B45E3B"],
-    "tenenbaums":["#a7ba42","#95ccba","#ffdede","#fff0cb","#f2cc84"],
-    "tracy":["#eaa2b6","#e7cbaf","#e0bd59","#292176"],
-    "dispatch":["#1f5c89","#72a87c","#c0bc78","#ce784b"],
-    "darjeeling2":["#ffe959","#b5b867","#b7dbdb","#6ba08f","#345b8e"],
-    "fantasticfox":["#4baecb","#e4d405","#df8818","#b40c24","#272121"],
-    "mendls":["#3a0202","#a03558","#b25d55","#7896d7","#dc90b5","#e0e2f4"],
-
-    #"vaporwave": ["#94D0FF", "#8795E8", "#966bff", "#AD8CFF", "#C774E8", "#c774a9", "#FF6AD5", "#ff6a8b", "#ff8b8b", "#ffa58b", "#ffde8b", "#cdde8b", "#8bde8b", "#20de8b"],
-    #"cool": ["#FF6AD5", "#C774E8", "#AD8CFF", "#8795E8", "#94D0FF"],
-    #"crystal_pepsi": ["#FFCCFF", "#F1DAFF", "#E3E8FF", "#CCFFFF"],
-    #"mallsoft": ["#fbcff3", "#f7c0bb", "#acd0f4", "#8690ff", "#30bfdd", "#7fd4c1"],
-    #"jazzcup": ["#392682", "#7a3a9a", "#3f86bc", "#28ada8", "#83dde0"],
-    #"sunset": ["#661246", "#ae1357", "#f9247e", "#d7509f", "#f9897b"],
-    #"macplus": ["#1b4247", "#09979b", "#75d8d5", "#ffc0cb", "#fe7f9d", "#65323e"],
-    #"seapunk": ["#532e57", "#a997ab", "#7ec488", "#569874", "#296656"],
-    #"avanti": ["#FB4142", "#94376C", "#CE75AD", "#76BDCF", "#9DCFF0"]
+    # "":["#","#"],
+    "megasaki": ["#aa82a7", "#9d2f28", "#deb867", "#e3ced3", "#948580", "#110d0e"],
+    "budapest": ["#4B0100", "#900403", "#4E1042", "#806150", "#C76B4F", "#D8AA88"],
+    "kingdom": ["#195B4E", "#617337", "#B1A16A", "#E1D06E", "#C99A6B", "#B27B7F"],
+    "darjeeling": ["#0D6CE8", "#8ACAF0", "#ABBBC7", "#687075", "#3B5657", "#B45E3B"],
+    "tenenbaums": ["#a7ba42", "#95ccba", "#ffdede", "#fff0cb", "#f2cc84"],
+    "tracy": ["#eaa2b6", "#e7cbaf", "#e0bd59", "#292176"],
+    "dispatch": ["#1f5c89", "#72a87c", "#c0bc78", "#ce784b"],
+    "darjeeling2": ["#ffe959", "#b5b867", "#b7dbdb", "#6ba08f", "#345b8e"],
+    "fantasticfox": ["#4baecb", "#e4d405", "#df8818", "#b40c24", "#272121"],
+    "mendls": ["#3a0202", "#a03558", "#b25d55", "#7896d7", "#dc90b5", "#e0e2f4"],
+    # "vaporwave": ["#94D0FF", "#8795E8", "#966bff", "#AD8CFF", "#C774E8", "#c774a9", "#FF6AD5", "#ff6a8b", "#ff8b8b", "#ffa58b", "#ffde8b", "#cdde8b", "#8bde8b", "#20de8b"],
+    # "cool": ["#FF6AD5", "#C774E8", "#AD8CFF", "#8795E8", "#94D0FF"],
+    # "crystal_pepsi": ["#FFCCFF", "#F1DAFF", "#E3E8FF", "#CCFFFF"],
+    # "mallsoft": ["#fbcff3", "#f7c0bb", "#acd0f4", "#8690ff", "#30bfdd", "#7fd4c1"],
+    # "jazzcup": ["#392682", "#7a3a9a", "#3f86bc", "#28ada8", "#83dde0"],
+    # "sunset": ["#661246", "#ae1357", "#f9247e", "#d7509f", "#f9897b"],
+    # "macplus": ["#1b4247", "#09979b", "#75d8d5", "#ffc0cb", "#fe7f9d", "#65323e"],
+    # "seapunk": ["#532e57", "#a997ab", "#7ec488", "#569874", "#296656"],
+    # "avanti": ["#FB4142", "#94376C", "#CE75AD", "#76BDCF", "#9DCFF0"]
 }
 
 # avoid plotly import if not using
 plotly_palettes = {k: list(map(list, zip(np.linspace(0, 1, len(palettes[k])), palettes[k]))) for k in palettes}
 
+
 def available(show=True):
     if not show:
         return palettes.keys()
     else:
         f, ax = plt.subplots(5, 2, figsize=(5, 8))
         for i, name in enumerate(palettes.keys()):
             x, y = i // 2, i % 2
@@ -49,15 +49,17 @@
         plt.show()
 
 
 def check_key(palname):
     try:
         palettes[palname]
     except KeyError:
-        raise KeyError("{} not an accepted palette name. Check vapeplot.available() for available palettes".format(palname))
+        raise KeyError(
+            "{} not an accepted palette name. Check vapeplot.available() for available palettes".format(palname)
+        )
 
 
 def cmap(palname):
     check_key(palname)
     return matplotlib.colors.ListedColormap(palettes[palname])
 
 
@@ -88,16 +90,16 @@
 
 def reverse(palname):
     check_key(palname)
     return list(reversed(palette(palname)))
 
 
 def set_palette(palname):
-        check_key(palname)
-        rcParams['axes.prop_cycle'] = cycler.cycler(color=palettes[palname])
+    check_key(palname)
+    rcParams['axes.prop_cycle'] = cycler.cycler(color=palettes[palname])
 
 
 def view_palette(*args):
     if len(args) > 1:
         f, ax = plt.subplots(1, len(args), figsize=(3 * len(args), 3))
         for i, name in enumerate(args):
             check_key(name)
```

### Comparing `wes_palette-0.1.0/wes_palette.egg-info/PKG-INFO` & `wes_palette-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,74 @@
-Metadata-Version: 2.1
-Name: wes-palette
-Version: 0.1.0
-Summary: Wes Anderson film color palette extension for matplotlib
-Author-email: AU <au2232@columbia.edu>
-License: MIT License
-        
-        Copyright (c) 2023 AU
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: repository, https://github.com/au2232/wes_palette
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
 ## wes-palette
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Issues](https://img.shields.io/github/issues/au2232/wes-palette)
 
 [![PyPI](https://img.shields.io/pypi/v/wes-palette)](https://pypi.org/project/wes-palette/)
 [![license](https://img.shields.io/github/license/au2232/wes-palette)](https://github.com/au2232/wes-palette/LICENSE)
 [![issues](https://img.shields.io/github/issues/au2232/wes-palette)](https://github.com/au2232/wes-palette/issues)
+[![build](https://img.shields.io/github/actions/workflow/status/au2232/wes_palette/build.yml)](https://github.com/au2232/wes_palette/actions/workflows/build.yml)
 [![docs](https://img.shields.io/github/actions/workflow/status/au2232/wes-palette/docs.yml?label=docs)](https://ew2664.github.io/wes-palette/)
-[![coverage](https://coveralls.io/repos/github/au2232/wes-palette/badge.svg)](https://coveralls.io/github/au2232/wes-palette)
+[![coverage](https://img.shields.io/codecov/c/github/au2232/wes_palette?token=5542beb1-1af8-4185-8340-fda0d36d528a)](https://coveralls.io/github/au2232/wes-palette)
+
+
 
 wes-palette is a Wes Anderson film color palettes for matplotlib based on [vapeplot](https://github.com/dantaki/vapeplot)
 
 ## Installation
-pip install wes-palette
+
+    pip install wes-palette
 
 ## Examples
 
 ![wes anderson palettes](palettes.png)
 
 ## Basic Usage
 
+Import the package
+  
+    import wes_palette as wes
+    
+Generate a custom diverging colormap
+
+    cmap = wes.cmap('budapest')
+    
+Create your graph with matplotlib and then display the plot:
+    
+    plt.show()
+
+## Example
+
+    # Create a visualization
+    sns.set_theme(style="white")
+
+    # Generate a large random dataset
+    rs = np.random.RandomState(33)
+    d = pd.DataFrame(data=rs.normal(size=(100, 26)),
+                 columns=list(ascii_letters[26:]))
+
+    # Compute the correlation matrix
+    corr = d.corr()
+
+    # Generate a mask for the upper tria#ngle
+    mask = np.triu(np.ones_like(corr, dtype=bool))
+
+    # Set up the matplotlib figure
+    f, ax = plt.subplots(figsize=(11, 9))
+
+    # Generate a custom diverging colormap
+    cmap = wes.cmap('dispatch')
+
+    # Draw the heatmap with the mask and correct aspect ratio
+    sns.heatmap(corr, mask=mask, cmap=cmap, vmax=.3, center=0,
+            square=True, linewidths=.5, cbar_kws={"shrink": .5})
+
+    plt.show()
+    
+![example](examplegraph1.png)
+![example](examplegraph2.png)
+![example](examplegraph3.png)
+
 ## Contributing
 
+See CONTRIBUTING.md
+
 ## License
+
+Protected under MIT Liscense.
```

