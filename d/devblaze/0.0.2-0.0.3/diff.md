# Comparing `tmp/devblaze-0.0.2.tar.gz` & `tmp/devblaze-0.0.3.tar.gz`

## Comparing `devblaze-0.0.2.tar` & `devblaze-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,41 @@
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 devblaze-0.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devblaze-0.0.2/Makefile
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 devblaze-0.0.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/devblaze.iml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/2f88094502ec7f89
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/35fe71a4dd87ac17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/5eb4f5434501f633
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/609322798689986d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/75c6f13fc972def1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/7b71c0436bbfd443
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/99e45b1bd08c7e6a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/a71860a9be908f3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/aa0d0bc3ca67ba4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/d62bd5c9e0fb954f
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/__init__.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/textual_utils/__init__.py
--rw-r--r--   0        0        0     9770 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/textual_utils/screen.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/textual_utils/static/cookiecutter.css
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 devblaze-0.0.2/scripts/format.sh
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 devblaze-0.0.2/scripts/lint.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devblaze-0.0.2/scripts/test.sh
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 devblaze-0.0.2/tests/test_version.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 devblaze-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 devblaze-0.0.2/LICENSE
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 devblaze-0.0.2/README.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 devblaze-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 devblaze-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 devblaze-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devblaze-0.0.3/Makefile
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 devblaze-0.0.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/2f88094502ec7f89
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/35fe71a4dd87ac17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/5eb4f5434501f633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/609322798689986d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/75c6f13fc972def1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/7b71c0436bbfd443
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/99e45b1bd08c7e6a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/a71860a9be908f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/aa0d0bc3ca67ba4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.3/.ruff_cache/content/d62bd5c9e0fb954f
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/__init__.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/constants.py
+-rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/screen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/screens/__init__.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/screens/base_app.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/screens/code_browser.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/screens/error.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/screens/quit.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/screens/success.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/static/checkbox.css
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/static/code_browser.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/static/cookiecutter.css
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/static/modal.css
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/static/radio_set_changed.css
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devblaze-0.0.3/devblaze/textual_utils/static/test.css
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 devblaze-0.0.3/scripts/format.sh
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 devblaze-0.0.3/scripts/lint.sh
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devblaze-0.0.3/scripts/test.sh
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 devblaze-0.0.3/tests/test_version.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 devblaze-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 devblaze-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 devblaze-0.0.3/README.md
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 devblaze-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 devblaze-0.0.3/PKG-INFO
```

### Comparing `devblaze-0.0.2/CONTRIBUTING.md` & `devblaze-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.2/.github/PULL_REQUEST_TEMPLATE.md` & `devblaze-0.0.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.2/devblaze/main.py` & `devblaze-0.0.3/devblaze/main.py`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.2/.gitignore` & `devblaze-0.0.3/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -70,7 +70,8 @@
 /site
 .mypy_cache/
 .dmypy.json
 dmypy.json
 .pyre/
 .pytype/
 cython_debug/
+.idea/
```

### Comparing `devblaze-0.0.2/LICENSE` & `devblaze-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.2/README.md` & `devblaze-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.2/pyproject.toml` & `devblaze-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 ]
 dependencies = [
     "cookiecutter ==2.1.1",
     "textual ==0.24.1",
 ]
 dynamic = ["version"]
 
+[project.urls]
+homepage = "https://github.com/godd0t/devblaze"
+
 [project.license]
 file = "LICENSE"
 
 [project.scripts]
 devblaze = "devblaze.main:main"
 
 [project.optional-dependencies]
```

### Comparing `devblaze-0.0.2/PKG-INFO` & `devblaze-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: devblaze
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for creating and managing development and production environments.
+Project-URL: homepage, https://github.com/godd0t/devblaze
 License: MIT License
         
         Copyright (c) 2023 Lirim Shala
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

