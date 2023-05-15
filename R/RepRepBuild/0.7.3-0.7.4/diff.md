# Comparing `tmp/RepRepBuild-0.7.3.tar.gz` & `tmp/RepRepBuild-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.7.3.tar", last modified: Wed May 10 14:56:01 2023, max compression
+gzip compressed data, was "RepRepBuild-0.7.4.tar", last modified: Mon May 15 07:29:27 2023, max compression
```

## Comparing `RepRepBuild-0.7.3.tar` & `RepRepBuild-0.7.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.945506 RepRepBuild-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.937506 RepRepBuild-0.7.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.937506 RepRepBuild-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/HEADER
--rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-10 14:56:01.945506 RepRepBuild-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:56:01.945506 RepRepBuild-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.933506 RepRepBuild-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.941506 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.945506 RepRepBuild-0.7.3/src/reprepbuild/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/reprepbuild/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/articlezip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/latexdep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/pythonscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/HEADER
+-rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.927795 RepRepBuild-0.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/src/reprepbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/reprepbuild/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/articlezip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/latexdep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/zip.py
```

### Comparing `RepRepBuild-0.7.3/.github/workflows/pypi.yaml` & `RepRepBuild-0.7.4/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/.pre-commit-config.yaml` & `RepRepBuild-0.7.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/CHANGELOG.md` & `RepRepBuild-0.7.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.7.4] - 2023-05-15
+
+### Fixed
+
+- Make local imports of Python scripts work when executed through RepRepBuild.
+
 ## [0.7.3] - 2023-05-10
 
 ### Fixed
 
 - Also detect bare `results` folder without suffix.
 
 ## [0.7.2] - 2023-04-27
```

### Comparing `RepRepBuild-0.7.3/COPYING` & `RepRepBuild-0.7.4/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/HEADER` & `RepRepBuild-0.7.4/HEADER`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/PKG-INFO` & `RepRepBuild-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.3
+Version: 0.7.4
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.7.3/README.md` & `RepRepBuild-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/pyproject.toml` & `RepRepBuild-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.7.4/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.3
+Version: 0.7.4
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.7.3/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.7.4/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/__init__.py` & `RepRepBuild-0.7.4/src/reprepbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/__main__.py` & `RepRepBuild-0.7.4/src/reprepbuild/__main__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/articlezip.py` & `RepRepBuild-0.7.4/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/bibtex.py` & `RepRepBuild-0.7.4/src/reprepbuild/bibtex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/latex.py` & `RepRepBuild-0.7.4/src/reprepbuild/latex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/latexdep.py` & `RepRepBuild-0.7.4/src/reprepbuild/latexdep.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.7.4/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.7.4/src/reprepbuild/pythonscript.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/repeat.py` & `RepRepBuild-0.7.4/src/reprepbuild/repeat.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/utils.py` & `RepRepBuild-0.7.4/src/reprepbuild/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 A `dyndep` is more powerful and general, but also a bit more complicated to set up.
 """
 
 
 import importlib.util
 import os
 import re
+import sys
 
 __all__ = (
     "parse_inputs_fls",
     "write_dep",
     "write_dyndep",
     "import_python_path",
     "check_script_args",
@@ -116,21 +117,25 @@
             f.write(" | ")
             f.write(" ".join(imp_inputs))
         f.write("\n")
 
 
 def import_python_path(path):
     """Return a module by importing a Python file at a given path."""
+    cwd = os.getcwd()
+    sys.path.append(cwd)
     spec = importlib.util.spec_from_file_location("<pythonscript>", path)
     module = importlib.util.module_from_spec(spec)
     try:
         spec.loader.exec_module(module)
-    except Exception:
+    except ImportError:
         # Ignore the script if it cannot be imported correctly.
-        return None
+        module = None
+    finally:
+        sys.path.remove(cwd)
     return module
 
 
 def check_script_args(script_args):
     for script_arg in script_args:
         if isinstance(script_arg, str):
             if not re.match(r"^[a-zA-Z0-9_-]*$", script_arg):
```

### Comparing `RepRepBuild-0.7.3/src/reprepbuild/zip.py` & `RepRepBuild-0.7.4/src/reprepbuild/zip.py`

 * *Files identical despite different names*

