# Comparing `tmp/stitchtoon-1.1.0.tar.gz` & `tmp/stitchtoon-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stitchtoon-1.1.0.tar", last modified: Tue May  9 08:14:35 2023, max compression
+gzip compressed data, was "stitchtoon-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `stitchtoon-1.1.0.tar` & `stitchtoon-1.1.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      431 2023-05-07 16:26:35.828468 stitchtoon-1.1.0/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0      111 2023-04-28 22:49:08.769926 stitchtoon-1.1.0/.gitignore
--rwxr-xr-x   0        0        0     1073 2023-04-26 07:52:39.218719 stitchtoon-1.1.0/LICENSE
--rw-r--r--   0        0        0      603 2023-04-26 07:52:39.218719 stitchtoon-1.1.0/Makefile
--rwxr-xr-x   0        0        0      351 2023-05-08 09:18:19.986354 stitchtoon-1.1.0/Pipfile
--rw-r--r--   0        0        0    36902 2023-04-28 10:37:12.713234 stitchtoon-1.1.0/Pipfile.lock
--rwxr-xr-x   0        0        0     3019 2023-05-05 16:29:36.234698 stitchtoon-1.1.0/README.md
--rwxr-xr-x   0        0        0      121 2023-05-08 09:15:41.929690 stitchtoon-1.1.0/pre-commit.sh
--rwxr-xr-x   0        0        0     1178 2023-05-08 11:58:10.777055 stitchtoon-1.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      596 2023-05-07 16:33:56.675945 stitchtoon-1.1.0/requirements.txt
--rwxr-xr-x   0        0        0      768 2023-04-26 07:52:39.232059 stitchtoon-1.1.0/setup.cfg
--rwxr-xr-x   0        0        0      117 2023-04-26 07:52:39.278749 stitchtoon-1.1.0/setup.py
--rwxr-xr-x   0        0        0     1815 2023-05-08 11:57:59.100388 stitchtoon-1.1.0/src/stitchtoon/__init__.py
--rwxr-xr-x   0        0        0     6145 2023-05-08 11:57:16.073719 stitchtoon-1.1.0/src/stitchtoon/__main__.py
--rwxr-xr-x   0        0        0      219 2023-04-26 07:52:39.232059 stitchtoon-1.1.0/src/stitchtoon/detectors/__init__.py
--rwxr-xr-x   0        0        0      811 2023-05-08 11:39:48.371086 stitchtoon-1.1.0/src/stitchtoon/detectors/direct_slicing.py
--rwxr-xr-x   0        0        0     2136 2023-05-08 11:39:34.821086 stitchtoon-1.1.0/src/stitchtoon/detectors/pixel_comparison.py
--rwxr-xr-x   0        0        0      523 2023-04-26 21:46:22.055454 stitchtoon-1.1.0/src/stitchtoon/detectors/selector.py
--rwxr-xr-x   0        0        0      438 2023-05-08 09:17:36.506355 stitchtoon-1.1.0/src/stitchtoon/services/__init__.py
--rwxr-xr-x   0        0        0     1578 2023-05-08 08:58:56.639710 stitchtoon-1.1.0/src/stitchtoon/services/global_logger.py
--rwxr-xr-x   0        0        0     1826 2023-05-08 09:17:36.503021 stitchtoon-1.1.0/src/stitchtoon/services/image_directory.py
--rwxr-xr-x   0        0        0     3428 2023-05-08 08:58:56.629710 stitchtoon-1.1.0/src/stitchtoon/services/image_handler.py
--rwxr-xr-x   0        0        0     4256 2023-05-08 11:57:41.203721 stitchtoon-1.1.0/src/stitchtoon/services/image_manipulator.py
--rwxr-xr-x   0        0        0      746 2023-05-08 08:58:56.589710 stitchtoon-1.1.0/src/stitchtoon/services/postprocess_runner.py
--rwxr-xr-x   0        0        0     8269 2023-05-08 11:57:18.173720 stitchtoon-1.1.0/src/stitchtoon/services/process.py
--rw-r--r--   0        0        0     1009 2023-05-07 16:10:22.120819 stitchtoon-1.1.0/src/stitchtoon/services/progressbar.py
--rwxr-xr-x   0        0        0     3026 2023-05-08 09:17:36.483021 stitchtoon-1.1.0/src/stitchtoon/services/scanner.py
--rwxr-xr-x   0        0        0        0 2023-04-28 21:57:52.553321 stitchtoon-1.1.0/src/stitchtoon/utils/__init__.py
--rwxr-xr-x   0        0        0     1155 2023-05-08 11:40:02.797754 stitchtoon-1.1.0/src/stitchtoon/utils/constants.py
--rwxr-xr-x   0        0        0      134 2023-04-28 09:58:00.606614 stitchtoon-1.1.0/src/stitchtoon/utils/errors.py
--rwxr-xr-x   0        0        0      451 2023-04-26 07:52:39.262074 stitchtoon-1.1.0/src/stitchtoon/utils/funcs.py
--rwxr-xr-x   0        0        0      823 2023-04-28 10:55:05.359879 stitchtoon-1.1.0/stitchtoon.spec
--rw-r--r--   0        0        0        0 2023-04-26 07:52:39.272079 stitchtoon-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0   138180 2023-05-07 16:35:32.471442 stitchtoon-1.1.0/tests/test/data/01.jpeg
--rw-r--r--   0        0        0  1726886 2023-05-07 16:35:32.528109 stitchtoon-1.1.0/tests/test/data/01.webp
--rw-r--r--   0        0        0   141943 2023-05-07 16:35:32.488109 stitchtoon-1.1.0/tests/test/data/02.jpeg
--rw-r--r--   0        0        0   123745 2023-05-07 16:35:32.494776 stitchtoon-1.1.0/tests/test/data/03.jpeg
--rw-r--r--   0        0        0   142053 2023-05-07 16:35:32.498109 stitchtoon-1.1.0/tests/test/data/04.jpeg
--rw-r--r--   0        0        0     1117 2023-05-07 16:35:32.494776 stitchtoon-1.1.0/tests/test/test_manipulator.py
--rw-r--r--   0        0        0     1101 2023-05-07 16:35:32.494776 stitchtoon-1.1.0/tests/test/test_scan.py
--rw-r--r--   0        0        0      284 2023-04-28 22:41:33.483269 stitchtoon-1.1.0/tox.ini
--rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 stitchtoon-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      431 2023-05-07 16:26:35.000000 stitchtoon-1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      131 2023-05-15 03:14:37.433657 stitchtoon-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1091 2023-05-15 03:14:37.433657 stitchtoon-1.1.1/LICENSE
+-rw-r--r--   0        0        0      603 2023-04-26 07:52:39.000000 stitchtoon-1.1.1/Makefile
+-rw-r--r--   0        0        0      376 2023-05-15 03:14:37.434656 stitchtoon-1.1.1/Pipfile
+-rw-r--r--   0        0        0    36902 2023-04-28 10:37:12.000000 stitchtoon-1.1.1/Pipfile.lock
+-rw-r--r--   0        0        0     3099 2023-05-15 03:14:37.434656 stitchtoon-1.1.1/README.md
+-rw-r--r--   0        0        0       98 2023-05-11 11:01:07.250980 stitchtoon-1.1.1/TODO
+-rw-r--r--   0        0        0      128 2023-05-15 03:14:37.436654 stitchtoon-1.1.1/pre-commit.sh
+-rw-r--r--   0        0        0     1234 2023-05-15 03:27:37.039760 stitchtoon-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      613 2023-05-15 03:14:37.437654 stitchtoon-1.1.1/requirements.txt
+-rw-r--r--   0        0        0      817 2023-05-15 03:14:37.440158 stitchtoon-1.1.1/setup.cfg
+-rw-r--r--   0        0        0      125 2023-05-15 03:14:37.437654 stitchtoon-1.1.1/setup.py
+-rw-r--r--   0        0        0     1883 2023-05-15 03:21:20.328929 stitchtoon-1.1.1/src/stitchtoon/__init__.py
+-rw-r--r--   0        0        0     6364 2023-05-15 03:14:37.439653 stitchtoon-1.1.1/src/stitchtoon/__main__.py
+-rw-r--r--   0        0        0      224 2023-05-15 03:14:37.442169 stitchtoon-1.1.1/src/stitchtoon/detectors/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-15 03:14:37.441164 stitchtoon-1.1.1/src/stitchtoon/detectors/direct_slicing.py
+-rw-r--r--   0        0        0     2189 2023-05-15 03:14:37.443168 stitchtoon-1.1.1/src/stitchtoon/detectors/pixel_comparison.py
+-rw-r--r--   0        0        0      537 2023-05-15 03:14:37.442169 stitchtoon-1.1.1/src/stitchtoon/detectors/selector.py
+-rw-r--r--   0        0        0      457 2023-05-15 03:14:37.443168 stitchtoon-1.1.1/src/stitchtoon/services/__init__.py
+-rw-r--r--   0        0        0     1629 2023-05-15 03:14:37.446165 stitchtoon-1.1.1/src/stitchtoon/services/global_logger.py
+-rw-r--r--   0        0        0     2298 2023-05-15 03:14:37.445166 stitchtoon-1.1.1/src/stitchtoon/services/image_directory.py
+-rw-r--r--   0        0        0     3564 2023-05-15 03:14:37.445166 stitchtoon-1.1.1/src/stitchtoon/services/image_handler.py
+-rw-r--r--   0        0        0     4385 2023-05-15 03:14:37.448165 stitchtoon-1.1.1/src/stitchtoon/services/image_manipulator.py
+-rw-r--r--   0        0        0      773 2023-05-15 03:14:37.448165 stitchtoon-1.1.1/src/stitchtoon/services/postprocess_runner.py
+-rw-r--r--   0        0        0     8672 2023-05-15 03:14:37.448165 stitchtoon-1.1.1/src/stitchtoon/services/process.py
+-rw-r--r--   0        0        0     1009 2023-05-07 16:10:22.000000 stitchtoon-1.1.1/src/stitchtoon/services/progressbar.py
+-rw-r--r--   0        0        0     3148 2023-05-15 03:14:37.449671 stitchtoon-1.1.1/src/stitchtoon/services/scanner.py
+-rw-r--r--   0        0        0        0 2023-05-15 03:14:37.449671 stitchtoon-1.1.1/src/stitchtoon/utils/__init__.py
+-rw-r--r--   0        0        0     1267 2023-05-15 03:14:37.450700 stitchtoon-1.1.1/src/stitchtoon/utils/constants.py
+-rw-r--r--   0        0        0      144 2023-05-15 03:14:37.451704 stitchtoon-1.1.1/src/stitchtoon/utils/errors.py
+-rw-r--r--   0        0        0      470 2023-05-15 03:14:37.452703 stitchtoon-1.1.1/src/stitchtoon/utils/funcs.py
+-rw-r--r--   0        0        0      867 2023-05-15 03:14:37.452703 stitchtoon-1.1.1/stitchtoon.spec
+-rw-r--r--   0        0        0        0 2023-04-26 07:52:39.000000 stitchtoon-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0   138180 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/01.jpeg
+-rw-r--r--   0        0        0  1726886 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/01.webp
+-rw-r--r--   0        0        0   141943 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/02.jpeg
+-rw-r--r--   0        0        0   123745 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/03.jpeg
+-rw-r--r--   0        0        0   142053 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/04.jpeg
+-rw-r--r--   0        0        0     1117 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/test_manipulator.py
+-rw-r--r--   0        0        0     1101 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/test_scan.py
+-rw-r--r--   0        0        0      284 2023-04-28 22:41:33.000000 stitchtoon-1.1.1/tox.ini
+-rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 stitchtoon-1.1.1/PKG-INFO
```

### Comparing `stitchtoon-1.1.0/LICENSE` & `stitchtoon-1.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `stitchtoon-1.1.0/Makefile` & `stitchtoon-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/Pipfile.lock` & `stitchtoon-1.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/pyproject.toml` & `stitchtoon-1.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "stitchtoon"
-version = "1.1.0"
-authors = [
-  { name="Beshr Alghalil", email="beshrghalil@protonmail.com" },
-]
-description = "A powerful program for stitching and cutting webtoons/manhwa/manhua raws."
-readme = "README.md"
-requires-python = ">=3.8"
-keywords = ["manga", "webtoon", "stitch", "slice", "combin"]
-dependencies = [
-    "psd_tools",
-    'natsort',
-    'pillow',
-    'progress',
-]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/BishrGhalil/stitchtoon"
-"Bug Tracker" = "https://github.com/BishrGhalil/issues"
-
-[project.optional-dependencies]
-dev = [
-    "black",
-    "flake8",
-    "isort",
-    "tox",
-    "mypy",
-]
-test = [
-    "pytest",
-]
-
-[project.scripts]
-stitchtoon = "stitchtoon.__main__:main"
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-ensure_newline_before_comments = true
-line_length = 120
-
-[tool.pylint.format]
-max-line-length = "120"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "stitchtoon"
+version = "1.1.1"
+authors = [
+  { name="Beshr Alghalil", email="beshrghalil@protonmail.com" },
+]
+description = "A powerful program for stitching and cutting webtoons/manhwa/manhua raws."
+readme = "README.md"
+requires-python = ">=3.8"
+keywords = ["manga", "webtoon", "stitch", "slice", "combin"]
+dependencies = [
+    "psd_tools",
+    'natsort',
+    'pillow',
+    'progress',
+]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/BishrGhalil/stitchtoon"
+"Bug Tracker" = "https://github.com/BishrGhalil/issues"
+
+[project.optional-dependencies]
+dev = [
+    "black",
+    "flake8",
+    "isort",
+    "tox",
+    "mypy",
+]
+test = [
+    "pytest",
+]
+
+[project.scripts]
+stitchtoon = "stitchtoon.__main__:main"
+
+[tool.isort]
+profile = "black"
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+ensure_newline_before_comments = true
+line_length = 120
+
+[tool.pylint.format]
+max-line-length = "120"
```

### Comparing `stitchtoon-1.1.0/requirements.txt` & `stitchtoon-1.1.1/requirements.txt`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
--i https://pypi.org/simple
-aggdraw==1.3.16 ; python_version >= '3.7'
-attrs==23.1.0 ; python_version >= '3.7'
-docopt==0.6.2
-imageio==2.28.0 ; python_version >= '3.7'
-lazy-loader==0.2 ; python_version >= '3.7'
-natsort==8.3.1
-networkx==3.1 ; python_version >= '3.8'
-numpy==1.24.3 ; python_version >= '3.8'
-packaging==23.1 ; python_version >= '3.7'
-pillow==9.5.0
-progress==1.6
-psd-tools==1.9.24
-pywavelets==1.4.1 ; python_version >= '3.8'
-scikit-image==0.20.0 ; python_version >= '3.8'
-scipy==1.10.1 ; python_version < '3.12' and python_version >= '3.8'
-tifffile==2023.4.12 ; python_version >= '3.8'
+-i https://pypi.org/simple
+aggdraw==1.3.16 ; python_version >= '3.7'
+attrs==23.1.0 ; python_version >= '3.7'
+docopt==0.6.2
+imageio==2.28.0 ; python_version >= '3.7'
+lazy-loader==0.2 ; python_version >= '3.7'
+natsort==8.3.1
+networkx==3.1 ; python_version >= '3.8'
+numpy==1.24.3 ; python_version >= '3.8'
+packaging==23.1 ; python_version >= '3.7'
+pillow==9.5.0
+progress==1.6
+psd-tools==1.9.24
+pywavelets==1.4.1 ; python_version >= '3.8'
+scikit-image==0.20.0 ; python_version >= '3.8'
+scipy==1.10.1 ; python_version < '3.12' and python_version >= '3.8'
+tifffile==2023.4.12 ; python_version >= '3.8'
```

### Comparing `stitchtoon-1.1.0/src/stitchtoon/__init__.py` & `stitchtoon-1.1.1/src/stitchtoon/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# This file is part of stitchtoon.
-# License: MIT, see the file "LICENSE" for details.
-"""Stitch Toon"""
-
-import os
-from sys import version_info
-
-
-# Version helper
-def version_helper():
-    if __release__:
-        version_string = "stitchtoon {0}".format(__version__)
-    else:
-        import subprocess
-
-        version_string = "stitchtoon-master {0}"
-        try:
-            with subprocess.Popen(
-                ["git", "describe"],
-                universal_newlines=True,
-                cwd=stitchtoon,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-            ) as git_describe:
-                (git_description, _) = git_describe.communicate()
-            version_string = version_string.format(git_description.strip("\n"))
-        except (OSError, subprocess.CalledProcessError, AttributeError):
-            version_string = version_string.format(__version__)
-    return version_string
-
-
-# Information
-__license__ = "MIT"
-__version__ = "1.1.0"
-__release__ = False
-__author__ = __maintainer__ = "Beshr Ghalil"
-__email__ = "beshrghalil@porotonmail.com"
-
-# Constants
-stitchtoon = os.path.dirname(__file__)
-DEFAULT_PAGER = "less"
-USAGE = "%prog [options] [path]"
-VERSION = version_helper()
-PY3 = version_info[0] >= 3
-
-args = None
-
-from .services.image_directory import Image
-from .services.image_directory import ImageDirectory
-from .services.process import process
-from .services.process import stitch
-from .services.progressbar import ProgressHandler
-from .services.scanner import is_supported_img
-from .services.scanner import scan
-from .services.scanner import scanimgdir
-from .services.scanner import walkimgdir
-
-__all__ = [
-    Image,
-    ImageDirectory,
-    scan,
-    scanimgdir,
-    walkimgdir,
-    process,
-    stitch,
-    is_supported_img,
-    ProgressHandler,
-]
+# This file is part of stitchtoon.
+# License: MIT, see the file "LICENSE" for details.
+"""Stitch Toon"""
+
+import os
+from sys import version_info
+
+
+# Version helper
+def version_helper():
+    if __release__:
+        version_string = "stitchtoon {0}".format(__version__)
+    else:
+        import subprocess
+
+        version_string = "stitchtoon-master {0}"
+        try:
+            with subprocess.Popen(
+                ["git", "describe"],
+                universal_newlines=True,
+                cwd=stitchtoon,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            ) as git_describe:
+                (git_description, _) = git_describe.communicate()
+            version_string = version_string.format(git_description.strip("\n"))
+        except (OSError, subprocess.CalledProcessError, AttributeError):
+            version_string = version_string.format(__version__)
+    return version_string
+
+
+# Information
+__license__ = "MIT"
+__version__ = "1.1.1"
+__release__ = False
+__author__ = __maintainer__ = "Beshr Ghalil"
+__email__ = "beshrghalil@porotonmail.com"
+
+# Constants
+stitchtoon = os.path.dirname(__file__)
+DEFAULT_PAGER = "less"
+USAGE = "%prog [options] [path]"
+VERSION = version_helper()
+PY3 = version_info[0] >= 3
+
+args = None
+
+from .services.image_directory import Image
+from .services.image_directory import ImageDirectory
+from .services.process import process
+from .services.process import stitch
+from .services.progressbar import ProgressHandler
+from .services.scanner import is_supported_img
+from .services.scanner import scan
+from .services.scanner import scanimgdir
+from .services.scanner import walkimgdir
+
+__all__ = [
+    Image,
+    ImageDirectory,
+    scan,
+    scanimgdir,
+    walkimgdir,
+    process,
+    stitch,
+    is_supported_img,
+    ProgressHandler,
+]
```

### Comparing `stitchtoon-1.1.0/src/stitchtoon/__main__.py` & `stitchtoon-1.1.1/src/stitchtoon/__main__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-import argparse
-import sys
-
-from stitchtoon import __version__
-from stitchtoon.services.global_logger import DEFAULT_LOG_LEVEL
-from stitchtoon.services.global_logger import get_logger
-from stitchtoon.services.process import process
-
-
-def positive_int(value):
-    if not value.isdigit() or int(value) <= 0:
-        raise argparse.ArgumentTypeError("Not a valid integer value")
-    return int(value)
-
-
-def log_level(value):
-    import logging
-
-    return {"debug": logging.DEBUG, "info": logging.INFO, "error": logging.ERROR}.get(
-        value, DEFAULT_LOG_LEVEL
-    )
-
-
-def size_format(value):
-    value = value.replace("x", "X")
-    size = value.split("X")
-    if len(size) > 2:
-        raise argparse.ArgumentTypeError(
-            "invalid size format. Supported formats `<height>X<width>` or `<height>` or `x<width>`. ex: `5000X760`"
-        )
-
-    elif len(size) == 1:
-        size.append("0")
-    elif len(size) == 0:
-        return (-1, -1)
-
-    for idx, s in enumerate(size):
-        if not s.isdigit():
-            raise argparse.ArgumentTypeError(
-                "invalid size format. Supported formats `<height>X<width>` or `<height>` or `x<width>`. ex: `5000X760`"
-            )
-        else:
-            size[idx] = int(s)
-    return size
-
-
-def get_args():
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-V", "--version", action="version", version=f"%(prog)s {__version__}"
-    )
-    parser.add_argument(
-        "-i",
-        "--input",
-        dest="input",
-        type=str,
-        required=True,
-        help="Sets the path of Input Folder",
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        dest="output",
-        type=str,
-        required=True,
-        help="Saves at specified output path",
-    )
-    parser.add_argument(
-        "-s",
-        "--size",
-        dest="size",
-        type=size_format,
-        required="-n" not in sys.argv and "--images-number" not in sys.argv,
-        help="Sets the value of the Rough Panel Height And Width, hXw",
-        default=(-1, -1),
-    )
-    parser.add_argument(
-        "-n",
-        "--images-number",
-        dest="images_number",
-        type=positive_int,
-        default=0,
-        required="-s" not in sys.argv and "--size" not in sys.argv,
-        help="Sets the value of the Rough Panel Height And Width, hXw",
-    )
-    parser.add_argument(
-        "-t",
-        "--type",
-        dest="output_format",
-        type=str,
-        default="jpg",
-        choices=["png", "jpeg", "jpg", "webp", "psb", "psd"],
-        help="Sets the type/format of the Output Image Files",
-    )
-    parser.add_argument("-r", "--recursive", dest="recursive", action="store_true")
-    parser.add_argument("-a", "--as-archive", dest="as_archive", action="store_true")
-    parser.add_argument(
-        "-p",
-        "--progress",
-        dest="show_progress",
-        action="store_true",
-        help="Shows a progress bar",
-        default=False,
-    )
-    advanced = parser.add_argument_group("Advanced")
-    advanced.add_argument(
-        "-w",
-        "--width-enforcement",
-        dest="width_enforcement",
-        type=str,
-        default="none",
-        choices=("none", "auto", "copywrite"),
-        help="Width Enforcement Technique, Default=None)",
-    )
-    advanced.add_argument(
-        "-d",
-        "--detection-type",
-        type=str,
-        dest="detection_type",
-        default="pixel",
-        choices=["none", "pixel"],
-        help="Sets the type of Slice Location Detection, Default=pixel (Pixel Comparison)",
-    )
-    advanced.add_argument(
-        "-e",
-        "--sensitivity",
-        dest="sensitivity",
-        type=int,
-        default=90,
-        choices=range(0, 101),
-        metavar="[0-100]",
-        help="Sets the Object Detection sensitivity Percentage, Default=90 (10 percent tolerance)",
-    )
-    advanced.add_argument(
-        "-q",
-        "--quality",
-        dest="lossy_quality",
-        type=int,
-        default=100,
-        choices=range(0, 101),
-        metavar="[1-100]",
-        help="Sets the quality of lossy file types like .jpg if used, Default=100 (100 percent)",
-    )
-    advanced.add_argument(
-        "-g",
-        "--ingorable_pixels",
-        dest="ignorable_pixels",
-        type=positive_int,
-        default=5,
-        help="Sets the value of Ignorable Border Pixels, Default=5 (5px)",
-    )
-    advanced.add_argument(
-        "-l",
-        "--line-steps",
-        dest="line_steps",
-        type=int,
-        default=5,
-        choices=range(1, 100),
-        metavar="[1-100]",
-        help="Sets the value of Scan Line Step, Default=5 (5px)",
-    )
-    general = parser.add_argument_group("General")
-    general.add_argument(
-        "--log-level",
-        dest="log_level",
-        default="error",
-        choices=["error", "debug", "info"],
-        help="Sets log level",
-    )
-    general.add_argument(
-        "--log-file",
-        dest="log_file",
-        default=sys.stdout,
-        help="Sets the log file, this supports providing datatime format.",
-    )
-    return parser.parse_args()
-
-
-def main():
-    kwargs = get_args()
-
-    global Logger
-    Logger = get_logger(
-        log_level=log_level(kwargs.log_level),
-        filename=kwargs.log_file,
-    )
-
-    stitch_params = {
-        "detection_type": kwargs.detection_type,
-        "sensitivity": kwargs.sensitivity,
-        "width_enforce": kwargs.width_enforcement,
-        "custom_width": kwargs.size[1],
-        "line_steps": kwargs.line_steps,
-        "ignorable_pixels": kwargs.ignorable_pixels,
-    }
-
-    try:
-        process(
-            input=kwargs.input,
-            output=kwargs.output,
-            split_height=kwargs.size[0],
-            images_number=kwargs.images_number,
-            output_format=kwargs.output_format,
-            recursive=kwargs.recursive,
-            as_archive=kwargs.as_archive,
-            lossy_quality=kwargs.lossy_quality,
-            show_progress=kwargs.show_progress,
-            params=stitch_params,
-        )
-    except Exception as e:
-        print(f"ERROR: {e}")
-        return 1
-
-    else:
-        return 0
-
-
-if __name__ == "__main__":
-    exit(main())
+import argparse
+import sys
+
+from stitchtoon import __version__
+from stitchtoon.services.global_logger import DEFAULT_LOG_LEVEL
+from stitchtoon.services.global_logger import get_logger
+from stitchtoon.services.process import process
+
+
+def positive_int(value):
+    if not value.isdigit() or int(value) <= 0:
+        raise argparse.ArgumentTypeError("Not a valid integer value")
+    return int(value)
+
+
+def log_level(value):
+    import logging
+
+    return {"debug": logging.DEBUG, "info": logging.INFO, "error": logging.ERROR}.get(
+        value, DEFAULT_LOG_LEVEL
+    )
+
+
+def size_format(value):
+    value = value.replace("x", "X")
+    size = value.split("X")
+    if len(size) > 2:
+        raise argparse.ArgumentTypeError(
+            "invalid size format. Supported formats `<height>X<width>` or `<height>` or `x<width>`. ex: `5000X760`"
+        )
+
+    elif len(size) == 1:
+        size.append("0")
+    elif len(size) == 0:
+        return (-1, -1)
+
+    for idx, s in enumerate(size):
+        if not s.isdigit():
+            raise argparse.ArgumentTypeError(
+                "invalid size format. Supported formats `<height>X<width>` or `<height>` or `x<width>`. ex: `5000X760`"
+            )
+        else:
+            size[idx] = int(s)
+    return size
+
+
+def get_args():
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-V", "--version", action="version", version=f"%(prog)s {__version__}"
+    )
+    parser.add_argument(
+        "-i",
+        "--input",
+        dest="input",
+        type=str,
+        required=True,
+        help="Sets the path of Input Folder",
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        dest="output",
+        type=str,
+        required=True,
+        help="Saves at specified output path",
+    )
+    parser.add_argument(
+        "-s",
+        "--size",
+        dest="size",
+        type=size_format,
+        required="-n" not in sys.argv and "--images-number" not in sys.argv,
+        help="Sets the value of the Rough Panel Height And Width, hXw",
+        default=(-1, -1),
+    )
+    parser.add_argument(
+        "-n",
+        "--images-number",
+        dest="images_number",
+        type=positive_int,
+        default=0,
+        required="-s" not in sys.argv and "--size" not in sys.argv,
+        help="Sets the value of the Rough Panel Height And Width, hXw",
+    )
+    parser.add_argument(
+        "-t",
+        "--type",
+        dest="output_format",
+        type=str,
+        default="jpg",
+        choices=["png", "jpeg", "jpg", "webp", "psb", "psd"],
+        help="Sets the type/format of the Output Image Files",
+    )
+    parser.add_argument("-r", "--recursive", dest="recursive", action="store_true")
+    parser.add_argument("-a", "--as-archive", dest="as_archive", action="store_true")
+    parser.add_argument(
+        "-p",
+        "--progress",
+        dest="show_progress",
+        action="store_true",
+        help="Shows a progress bar",
+        default=False,
+    )
+    advanced = parser.add_argument_group("Advanced")
+    advanced.add_argument(
+        "-w",
+        "--width-enforcement",
+        dest="width_enforcement",
+        type=str,
+        default="none",
+        choices=("none", "auto", "copywrite"),
+        help="Width Enforcement Technique, Default=None)",
+    )
+    advanced.add_argument(
+        "-d",
+        "--detection-type",
+        type=str,
+        dest="detection_type",
+        default="pixel",
+        choices=["none", "pixel"],
+        help="Sets the type of Slice Location Detection, Default=pixel (Pixel Comparison)",
+    )
+    advanced.add_argument(
+        "-e",
+        "--sensitivity",
+        dest="sensitivity",
+        type=int,
+        default=90,
+        choices=range(0, 101),
+        metavar="[0-100]",
+        help="Sets the Object Detection sensitivity Percentage, Default=90 (10 percent tolerance)",
+    )
+    advanced.add_argument(
+        "-q",
+        "--quality",
+        dest="lossy_quality",
+        type=int,
+        default=100,
+        choices=range(0, 101),
+        metavar="[1-100]",
+        help="Sets the quality of lossy file types like .jpg if used, Default=100 (100 percent)",
+    )
+    advanced.add_argument(
+        "-g",
+        "--ingorable_pixels",
+        dest="ignorable_pixels",
+        type=positive_int,
+        default=5,
+        help="Sets the value of Ignorable Border Pixels, Default=5 (5px)",
+    )
+    advanced.add_argument(
+        "-l",
+        "--line-steps",
+        dest="line_steps",
+        type=int,
+        default=5,
+        choices=range(1, 100),
+        metavar="[1-100]",
+        help="Sets the value of Scan Line Step, Default=5 (5px)",
+    )
+    general = parser.add_argument_group("General")
+    general.add_argument(
+        "--log-level",
+        dest="log_level",
+        default="error",
+        choices=["error", "debug", "info"],
+        help="Sets log level",
+    )
+    general.add_argument(
+        "--log-file",
+        dest="log_file",
+        default=sys.stdout,
+        help="Sets the log file, this supports providing datatime format.",
+    )
+    return parser.parse_args()
+
+
+def main():
+    kwargs = get_args()
+
+    global Logger
+    Logger = get_logger(
+        log_level=log_level(kwargs.log_level),
+        filename=kwargs.log_file,
+    )
+
+    stitch_params = {
+        "detection_type": kwargs.detection_type,
+        "sensitivity": kwargs.sensitivity,
+        "width_enforce": kwargs.width_enforcement,
+        "custom_width": kwargs.size[1],
+        "line_steps": kwargs.line_steps,
+        "ignorable_pixels": kwargs.ignorable_pixels,
+    }
+
+    try:
+        process(
+            input=kwargs.input,
+            output=kwargs.output,
+            split_height=kwargs.size[0],
+            images_number=kwargs.images_number,
+            output_format=kwargs.output_format,
+            recursive=kwargs.recursive,
+            as_archive=kwargs.as_archive,
+            lossy_quality=kwargs.lossy_quality,
+            show_progress=kwargs.show_progress,
+            params=stitch_params,
+        )
+    except Exception as e:
+        print(f"ERROR: {e}")
+        return 1
+
+    else:
+        return 0
+
+
+if __name__ == "__main__":
+    exit(main())
```

### Comparing `stitchtoon-1.1.0/src/stitchtoon/detectors/direct_slicing.py` & `stitchtoon-1.1.1/src/stitchtoon/detectors/direct_slicing.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from ..services.global_logger import logFunc
-from ..services.image_directory import Image
-from ..utils.constants import SMALLER_ALLOWD_HEIGHT
-
-
-class DirectSlicingDetector:
-    @logFunc(inclass=True)
-    def run(self, combined_img: Image, split_height: int, **kwargs) -> list[int]:
-        if split_height < SMALLER_ALLOWD_HEIGHT:
-            raise Exception("Height very small to slice")
-        # Changes from a pil image to an numpy pixel array
-        last_row = combined_img.height
-        # Initializes some variables
-        slice_locations = [0]
-        row = split_height
-        while row < last_row:
-            slice_locations.append(row)
-            row += split_height
-        if slice_locations[-1] != last_row - 1:
-            slice_locations.append(last_row - 1)
-        return slice_locations
+from ..services.global_logger import logFunc
+from ..services.image_directory import Image
+from ..utils.constants import SMALLER_ALLOWD_HEIGHT
+
+
+class DirectSlicingDetector:
+    @logFunc(inclass=True)
+    def run(self, combined_img: Image, split_height: int, **kwargs) -> list[int]:
+        if split_height < SMALLER_ALLOWD_HEIGHT:
+            raise Exception("Height very small to slice")
+        # Changes from a pil image to an numpy pixel array
+        last_row = combined_img.height
+        # Initializes some variables
+        slice_locations = [0]
+        row = split_height
+        while row < last_row:
+            slice_locations.append(row)
+            row += split_height
+        if slice_locations[-1] != last_row - 1:
+            slice_locations.append(last_row - 1)
+        return slice_locations
```

### Comparing `stitchtoon-1.1.0/src/stitchtoon/detectors/pixel_comparison.py` & `stitchtoon-1.1.1/src/stitchtoon/detectors/pixel_comparison.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import numpy as np
-
-from ..services.global_logger import logFunc
-from ..services.image_directory import Image
-from ..utils.constants import SMALLER_ALLOWD_HEIGHT
-
-
-class PixelComparisonDetector:
-    @logFunc(inclass=True)
-    def run(self, combined_img: Image, split_height: int, **kwargs) -> list[int]:
-        """Uses Neighbouring pixels comparison to detect ideal slice locations"""
-        if split_height < SMALLER_ALLOWD_HEIGHT:
-            raise Exception("Height very small to slice")
-        # Changes from a pil Image to an numpy pixel array
-        combined_img = np.array(combined_img.pil.convert("L"))
-        # Setting up rest of Detector Parameters
-        scan_step = kwargs.get("scan_step", 5)
-        ignorable_pixels = kwargs.get("ignorable_pixels", 0)
-        sensitivity = kwargs.get("sensitivity", 90)
-        threshold = int(255 * (1 - (sensitivity / 100)))
-        last_row = len(combined_img)
-        # Initializes some variables
-        slice_locations = [0]
-        row = split_height
-        move_up = True
-        # Detector Main Logic
-        while row < last_row:
-            row_pixels = combined_img[row]
-            can_slice = True
-            for index in range(
-                ignorable_pixels + 1, len(row_pixels) - ignorable_pixels
-            ):
-                prev_pixel = int(row_pixels[index - 1])
-                next_pixel = int(row_pixels[index])
-                value_diff = next_pixel - prev_pixel
-                if value_diff > threshold or value_diff < -threshold:
-                    can_slice = False
-                    break
-            if can_slice:
-                slice_locations.append(row)
-                row += split_height
-                move_up = True
-                continue
-            if row - slice_locations[-1] <= 0.4 * split_height:
-                row = slice_locations[-1] + split_height
-                move_up = False
-            if move_up:
-                row -= scan_step
-                continue
-            row += scan_step
-        if slice_locations[-1] != last_row - 1:
-            slice_locations.append(last_row - 1)
-        return slice_locations
+import numpy as np
+
+from ..services.global_logger import logFunc
+from ..services.image_directory import Image
+from ..utils.constants import SMALLER_ALLOWD_HEIGHT
+
+
+class PixelComparisonDetector:
+    @logFunc(inclass=True)
+    def run(self, combined_img: Image, split_height: int, **kwargs) -> list[int]:
+        """Uses Neighbouring pixels comparison to detect ideal slice locations"""
+        if split_height < SMALLER_ALLOWD_HEIGHT:
+            raise Exception("Height very small to slice")
+        # Changes from a pil Image to an numpy pixel array
+        combined_img = np.array(combined_img.pil.convert("L"))
+        # Setting up rest of Detector Parameters
+        scan_step = kwargs.get("scan_step", 5)
+        ignorable_pixels = kwargs.get("ignorable_pixels", 0)
+        sensitivity = kwargs.get("sensitivity", 90)
+        threshold = int(255 * (1 - (sensitivity / 100)))
+        last_row = len(combined_img)
+        # Initializes some variables
+        slice_locations = [0]
+        row = split_height
+        move_up = True
+        # Detector Main Logic
+        while row < last_row:
+            row_pixels = combined_img[row]
+            can_slice = True
+            for index in range(
+                ignorable_pixels + 1, len(row_pixels) - ignorable_pixels
+            ):
+                prev_pixel = int(row_pixels[index - 1])
+                next_pixel = int(row_pixels[index])
+                value_diff = next_pixel - prev_pixel
+                if value_diff > threshold or value_diff < -threshold:
+                    can_slice = False
+                    break
+            if can_slice:
+                slice_locations.append(row)
+                row += split_height
+                move_up = True
+                continue
+            if row - slice_locations[-1] <= 0.4 * split_height:
+                row = slice_locations[-1] + split_height
+                move_up = False
+            if move_up:
+                row -= scan_step
+                continue
+            row += scan_step
+        if slice_locations[-1] != last_row - 1:
+            slice_locations.append(last_row - 1)
+        return slice_locations
```

### Comparing `stitchtoon-1.1.0/src/stitchtoon/services/image_directory.py` & `stitchtoon-1.1.1/src/stitchtoon/services/image_directory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,82 @@
-from __future__ import annotations
-
-import os
-from dataclasses import dataclass
-from dataclasses import field
-
-from PIL import Image as pilImage
-from psd_tools import PSDImage
-
-from ..utils.constants import PHOTOSHOP_FILE_TYPES
-from ..utils.errors import ImageNotOpenedError
-
-
-@dataclass
-class Image:
-    path: os.PathLike
-    name: str
-    format: str = field(default=None)
-    pil: pilImage = field(default=None)
-
-    def save(self, fp: os.PathLike, format: str = None, quality: int = 90) -> None:
-        if not self.pil:
-            return
-        if not format:
-            format = self.format
-
-        if format in PHOTOSHOP_FILE_TYPES:
-            psd_obj = PSDImage.frompil(self.pil)
-            psd_obj.save(fp)
-            del psd_obj
-        else:
-            self.pil.save(fp, format=format, quality=quality)
-            self.pil.close()
-
-    def copy(self) -> Image:
-        return Image(path=self.path, format=self.format, name=self.name, pil=self.pil)
-
-    def topil(self) -> pilImage:
-        if not self.pil:
-            self.open()
-
-        return self.pil
-
-    def open(self) -> Image:
-        if self.pil:
-            return self
-        self.pil = pilImage.open(self.path)
-        return self
-
-    @property
-    def width(self) -> int:
-        self._raise_if_not_opened()
-        return self.pil.size[0]
-
-    @property
-    def height(self) -> int:
-        self._raise_if_not_opened()
-        return self.pil.size[1]
-
-    @property
-    def size(self) -> tuple[int, int]:
-        self._raise_if_not_opened()
-        return self.pil.size
-
-    def _raise_if_not_opened(self) -> None:
-        if not self.pil:
-            raise ImageNotOpenedError("Image is not opened yet")
-
-
-@dataclass
-class ImageDirectory:
-    path: os.PathLike
-    images: list[Image]
-    dirs: list[ImageDirectory] = field(default=None)
+from __future__ import annotations
+
+import os
+from dataclasses import dataclass
+from dataclasses import field
+
+from PIL import Image as pilImage
+from psd_tools import PSDImage
+
+from ..utils.constants import PHOTOSHOP_FILE_TYPES
+from ..utils.constants import SUPPORTS_TRANSPARENCY
+
+
+@dataclass
+class Image:
+    path: os.PathLike
+    name: str
+    format: str = field(default=None)
+    pil: pilImage = field(default=None)
+
+    def save(self, fp: os.PathLike, format: str = None, quality: int = 90) -> None:
+        if not self.pil:
+            self._raise_if_not_opened()
+        if not format:
+            format = self.format
+
+        if format in PHOTOSHOP_FILE_TYPES:
+            psd_obj = PSDImage.frompil(self.pil)
+            psd_obj.save(fp)
+            del psd_obj
+        else:
+            if self.pil.mode == "RGBA" and format.lower() not in SUPPORTS_TRANSPARENCY:
+                self.pil.load()
+                background = pilImage.new("RGB", self.size, (255, 255, 255))
+                background.paste(
+                    self.pil, mask=self.pil.split()[3]
+                )  # 3 is the alpha channel
+                self.pil = background
+
+            self.pil.save(fp, format=format, quality=quality)
+            self.pil.close()
+
+    def copy(self) -> Image:
+        return Image(path=self.path, format=self.format, name=self.name, pil=self.pil)
+
+    def topil(self) -> pilImage:
+        if not self.pil:
+            self.open()
+
+        return self.pil
+
+    def open(self) -> Image:
+        if self.pil:
+            return self
+        self.pil = pilImage.open(self.path)
+        return self
+
+    @property
+    def width(self) -> int:
+        self._raise_if_not_opened()
+        return self.pil.size[0]
+
+    @property
+    def height(self) -> int:
+        self._raise_if_not_opened()
+        return self.pil.size[1]
+
+    @property
+    def size(self) -> tuple[int, int]:
+        self._raise_if_not_opened()
+        return self.pil.size
+
+    def _raise_if_not_opened(self) -> None:
+        if not self.pil:
+            raise Exception("Image should be opened first")
+
+
+@dataclass
+class ImageDirectory:
+    path: os.PathLike
+    images: list[Image]
+    dirs: list[ImageDirectory] = field(default=None)
```

### Comparing `stitchtoon-1.1.0/src/stitchtoon/services/image_handler.py` & `stitchtoon-1.1.1/src/stitchtoon/services/image_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,106 @@
-from __future__ import annotations
-
-import io
-import os
-import os.path as osp
-import zipfile
-
-from PIL import Image as pilImage
-from psd_tools import PSDImage
-
-from ..utils.constants import PHOTOSHOP_FILE_TYPES
-from .global_logger import logFunc
-from .image_directory import Image
-from .progressbar import ProgressHandler
-
-
-class ImageHandler:
-    @logFunc(inclass=True)
-    def filename_handler(self, filename: str, format: str) -> str:
-        if not osp.splitext(filename)[1]:
-            filename = f"{filename}.{format}"
-        else:
-            filename = f"{osp.splitext(filename)[0]}.{format}"
-
-        return filename
-
-    # TODOO: Load images from ao zip/cbz archive.
-    @logFunc(inclass=True)
-    def load_zip(
-        self,
-        path: os.PathLike,
-        progress: ProgressHandler = ProgressHandler(),
-        increament: int = 0,
-    ) -> list[Image]:
-        pass
-
-    @logFunc(inclass=True)
-    def load(
-        self,
-        images: list[Image],
-        progress: ProgressHandler = ProgressHandler(),
-        increament: int = 0,
-    ) -> list[Image]:
-        """Loads all image files into a list of PIL image objects."""
-        images_len = len(images)
-        for idx, image in enumerate(images, 1):
-            if image.format not in PHOTOSHOP_FILE_TYPES:
-                image.pil = pilImage.open(image.path)
-            else:
-                psd = PSDImage.open(image.path)
-                image.pil = psd.topil()
-                del psd
-            progress.update(progress.value + increament, f"Loading {idx}/{images_len}")
-        return images
-
-    @logFunc(inclass=True)
-    def save_archive(
-        self,
-        output,
-        images: list[pilImage.Image],
-        img_format: str,
-        quality=100,
-        progress=ProgressHandler(),
-        increament=0,
-    ) -> os.PathLike:
-        if img_format in PHOTOSHOP_FILE_TYPES:
-            # FIXMEE: support archiving psd files
-            raise Exception("Can't make PSD archive")
-
-        zf = zipfile.ZipFile(output, mode="w")
-        images_len = len(images)
-        for idx, image in enumerate(images, 1):
-            img_byte_arr = io.BytesIO()
-            image.pil.save(img_byte_arr, img_format, quality=quality)
-            img_byte_arr = img_byte_arr.getvalue()
-            zf.writestr(self.filename_handler(f"{idx:02}", img_format), img_byte_arr)
-            progress.update(progress.value + increament, f"Archive {idx}/{images_len}")
-
-        return output
-
-    @logFunc(inclass=True)
-    def save_all(
-        self,
-        output: os.PathLike,
-        images: list[Image],
-        format: str = "png",
-        as_archive: bool = False,
-        quality: int = 100,
-        progress=ProgressHandler(),
-        increament: int = 0,
-    ) -> os.PathLike:
-        progress.update(progress.value, "Saving, Please wait...")
-        if as_archive:
-            os.makedirs(osp.dirname(output), exist_ok=True)
-            self.save_archive(output, images, format, quality, progress, increament)
-        else:
-            os.makedirs(output, exist_ok=True)
-            images_len = len(images)
-            for idx, img in enumerate(images, 1):
-                filename = self.filename_handler(f"{idx:02}", format)
-                img.save(osp.join(output, filename), format, quality)
-                progress.update(
-                    progress.value + increament, f"Saving {idx}/{images_len}"
-                )
-        return output
+from __future__ import annotations
+
+import io
+import os
+import os.path as osp
+import zipfile
+
+from PIL import Image as pilImage
+from psd_tools import PSDImage
+
+from ..utils.constants import PHOTOSHOP_FILE_TYPES
+from .global_logger import logFunc
+from .image_directory import Image
+from .progressbar import ProgressHandler
+
+
+class ImageHandler:
+    @logFunc(inclass=True)
+    def filename_handler(self, filename: str, format: str) -> str:
+        if not osp.splitext(filename)[1]:
+            filename = f"{filename}.{format}"
+        else:
+            filename = f"{osp.splitext(filename)[0]}.{format}"
+
+        return filename
+
+    # TODOO: Load images from a zip/cbz archive.
+    @logFunc(inclass=True)
+    def load_zip(
+        self,
+        path: os.PathLike,
+        progress: ProgressHandler = ProgressHandler(),
+        increament: int = 0,
+    ) -> list[Image]:
+        pass
+
+    @logFunc(inclass=True)
+    def load(
+        self,
+        images: list[Image],
+        progress: ProgressHandler = ProgressHandler(),
+        increament: int = 0,
+        transparent: bool = False,
+    ) -> list[Image]:
+        """Loads all image files into a list of PIL image objects."""
+        images_len = len(images)
+        for idx, image in enumerate(images, 1):
+            if image.format not in PHOTOSHOP_FILE_TYPES:
+                image.pil = pilImage.open(image.path)
+            else:
+                psd = PSDImage.open(image.path)
+                image.pil = psd.topil()
+                del psd
+            progress.update(progress.value + increament, f"Loading {idx}/{images_len}")
+        return images
+
+    @logFunc(inclass=True)
+    def save_archive(
+        self,
+        output,
+        images: list[pilImage.Image],
+        img_format: str,
+        quality=100,
+        progress=ProgressHandler(),
+        increament=0,
+    ) -> os.PathLike:
+        if img_format in PHOTOSHOP_FILE_TYPES:
+            # FIXMEE: support archiving psd files
+            raise Exception("Can't make PSD archive")
+
+        zf = zipfile.ZipFile(output, mode="w")
+        images_len = len(images)
+        for idx, image in enumerate(images, 1):
+            img_byte_arr = io.BytesIO()
+            image.save(img_byte_arr, img_format, quality=quality)
+            img_byte_arr = img_byte_arr.getvalue()
+            zf.writestr(self.filename_handler(f"{idx:02}", img_format), img_byte_arr)
+            progress.update(progress.value + increament, f"Archive {idx}/{images_len}")
+
+        return output
+
+    @logFunc(inclass=True)
+    def save_all(
+        self,
+        output: os.PathLike,
+        images: list[Image],
+        format: str = "png",
+        as_archive: bool = False,
+        quality: int = 100,
+        progress=ProgressHandler(),
+        increament: int = 0,
+    ) -> os.PathLike:
+        progress.update(progress.value, "Saving, Please wait...")
+        if as_archive:
+            os.makedirs(osp.dirname(output), exist_ok=True)
+            self.save_archive(output, images, format, quality, progress, increament)
+        else:
+            os.makedirs(output, exist_ok=True)
+            images_len = len(images)
+            for idx, img in enumerate(images, 1):
+                filename = self.filename_handler(f"{idx:02}", format)
+                img.save(osp.join(output, filename), format, quality)
+                progress.update(
+                    progress.value + increament, f"Saving {idx}/{images_len}"
+                )
+        return output
```

### Comparing `stitchtoon-1.1.0/src/stitchtoon/services/image_manipulator.py` & `stitchtoon-1.1.1/src/stitchtoon/services/image_manipulator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from PIL import Image as pilImage
-
-from ..utils.constants import WIDTH_ENFORCEMENT
-from ..utils.errors import SizeLimitError
-from .global_logger import logFunc
-from .image_directory import Image
-from .progressbar import ProgressHandler
-
-
-class ImageManipulator:
-    @logFunc
-    @staticmethod
-    def _resize_img(img: Image, new_img_width) -> Image:
-        if img.width == new_img_width:
-            return img
-        img_ratio = float(img.height / img.width)
-        new_img_height = int(img_ratio * new_img_width)
-        if new_img_height > 0:
-            img.pil = img.pil.resize(
-                (new_img_width, new_img_height), pilImage.Resampling.LANCZOS
-            )
-        return img
-
-    @logFunc(inclass=True)
-    @staticmethod
-    def resize(
-        img_objs: list[Image],
-        enforce_setting: WIDTH_ENFORCEMENT,
-        custom_width: int = 720,
-    ) -> list[Image]:
-        """Resizes all given images according to the set enforcement setting.
-
-        Args:
-            img_objs (list[Image])
-            enforce_setting WIDTH_ENFORCEMENT
-            custom_width (int, optional). Defaults to 720.
-
-        Returns:
-            list[Image]
-        """
-
-        if enforce_setting == WIDTH_ENFORCEMENT.NONE.value and not custom_width:
-            return img_objs
-
-        new_img_width = 0
-        if enforce_setting == WIDTH_ENFORCEMENT.COPYWRITE.value:
-            if len(img_objs) >= 2:
-                new_img_width = img_objs[1].width
-                ImageManipulator._resize_img(img_objs[0], new_img_width)
-            return img_objs
-
-        elif enforce_setting == WIDTH_ENFORCEMENT.AUTO.value:
-            widths, heights = zip(*(img.size for img in img_objs))
-            new_img_width = min(widths)
-
-        elif enforce_setting == WIDTH_ENFORCEMENT.FIXED.value or custom_width:
-            new_img_width = custom_width
-
-        for img in img_objs:
-            ImageManipulator._resize_img(img, new_img_width)
-
-        return img_objs
-
-    @logFunc(inclass=True)
-    @staticmethod
-    def combine(
-        img_objs: list[Image], progress: ProgressHandler = None, increament: int = 0
-    ) -> Image:
-        """Combines given image objs to a single vertically stacked single image obj.
-
-        Args:
-            img_objs (list[Image])
-            progress (_type_, optional)
-            increament (int, optional). Defaults to 0.
-
-        Returns:
-            Image
-        """
-
-        if not progress:
-            progress = ProgressHandler()
-        widths, heights = zip(*(img.size for img in img_objs))
-        combined_img_width = max(widths)
-        combined_img_height = sum(heights)
-        combined_img = pilImage.new("RGB", (combined_img_width, combined_img_height))
-        combine_offset = 0
-        images_len = len(img_objs)
-        for idx, img in enumerate(img_objs, 1):
-            combined_img.paste(img.pil, (0, combine_offset))
-            combine_offset += img.height
-            img.pil.close()
-            progress.update(progress.value + increament, f"Combined {idx}/{images_len}")
-
-        img = Image(
-            path=img_objs[0].path, format=img_objs[0].format, name=img_objs[0].name
-        )
-        img.pil = combined_img
-        progress.update(progress.value, "All combined")
-        return img
-
-    @logFunc(inclass=True)
-    @staticmethod
-    def slice(combined_img: Image, slice_locations: list[int]) -> list[Image]:
-        """Combines given combined img to into multiple img slices given the slice locations.
-
-        Args:
-            combined_img (Image)
-            slice_locations (list[int])
-
-        Returns:
-            list[Image]
-        """
-
-        max_width = combined_img.width
-        img_objs = []
-        for index in range(1, len(slice_locations)):
-            upper_limit = slice_locations[index - 1]
-            lower_limit = slice_locations[index]
-            slice_boundaries = (0, upper_limit, max_width, lower_limit)
-            try:
-                img_slice = combined_img.pil.crop(slice_boundaries)
-            except ValueError:
-                raise SizeLimitError("Images to small to slice")
-            img = combined_img.copy()
-            img.pil = img_slice
-            img_objs.append(img)
-        combined_img.pil.close()
-        return img_objs
+from PIL import Image as pilImage
+
+from ..utils.constants import WIDTH_ENFORCEMENT
+from ..utils.errors import SizeLimitError
+from .global_logger import logFunc
+from .image_directory import Image
+from .progressbar import ProgressHandler
+
+
+class ImageManipulator:
+    @logFunc
+    @staticmethod
+    def _resize_img(img: Image, new_img_width) -> Image:
+        if img.width == new_img_width:
+            return img
+        img_ratio = float(img.height / img.width)
+        new_img_height = int(img_ratio * new_img_width)
+        if new_img_height > 0:
+            img.pil = img.pil.resize(
+                (new_img_width, new_img_height), pilImage.Resampling.LANCZOS
+            )
+        return img
+
+    @logFunc(inclass=True)
+    @staticmethod
+    def resize(
+        img_objs: list[Image],
+        enforce_setting: WIDTH_ENFORCEMENT,
+        custom_width: int = 720,
+    ) -> list[Image]:
+        """Resizes all given images according to the set enforcement setting.
+
+        Args:
+            img_objs (list[Image])
+            enforce_setting WIDTH_ENFORCEMENT
+            custom_width (int, optional). Defaults to 720.
+
+        Returns:
+            list[Image]
+        """
+
+        if enforce_setting == WIDTH_ENFORCEMENT.NONE.value and not custom_width:
+            return img_objs
+
+        new_img_width = 0
+        if enforce_setting == WIDTH_ENFORCEMENT.COPYWRITE.value:
+            if len(img_objs) >= 2:
+                new_img_width = img_objs[1].width
+                ImageManipulator._resize_img(img_objs[0], new_img_width)
+            return img_objs
+
+        elif enforce_setting == WIDTH_ENFORCEMENT.AUTO.value:
+            widths, heights = zip(*(img.size for img in img_objs))
+            new_img_width = min(widths)
+
+        elif enforce_setting == WIDTH_ENFORCEMENT.FIXED.value or custom_width:
+            new_img_width = custom_width
+
+        for img in img_objs:
+            ImageManipulator._resize_img(img, new_img_width)
+
+        return img_objs
+
+    @logFunc(inclass=True)
+    @staticmethod
+    def combine(
+        img_objs: list[Image], progress: ProgressHandler = None, increament: int = 0
+    ) -> Image:
+        """Combines given image objs to a single vertically stacked single image obj.
+
+        Args:
+            img_objs (list[Image])
+            progress (_type_, optional)
+            increament (int, optional). Defaults to 0.
+
+        Returns:
+            Image
+        """
+
+        if not progress:
+            progress = ProgressHandler()
+        widths, heights = zip(*(img.size for img in img_objs))
+        combined_img_width = max(widths)
+        combined_img_height = sum(heights)
+        combined_img = pilImage.new("RGBA", (combined_img_width, combined_img_height))
+        combine_offset = 0
+        images_len = len(img_objs)
+        for idx, img in enumerate(img_objs, 1):
+            combined_img.paste(img.pil, (0, combine_offset))
+            combine_offset += img.height
+            img.pil.close()
+            progress.update(progress.value + increament, f"Combined {idx}/{images_len}")
+
+        img = Image(
+            path=img_objs[0].path, format=img_objs[0].format, name=img_objs[0].name
+        )
+        img.pil = combined_img
+        progress.update(progress.value, "All combined")
+        return img
+
+    @logFunc(inclass=True)
+    @staticmethod
+    def slice(combined_img: Image, slice_locations: list[int]) -> list[Image]:
+        """Combines given combined img to into multiple img slices given the slice locations.
+
+        Args:
+            combined_img (Image)
+            slice_locations (list[int])
+
+        Returns:
+            list[Image]
+        """
+
+        max_width = combined_img.width
+        img_objs = []
+        for index in range(1, len(slice_locations)):
+            upper_limit = slice_locations[index - 1]
+            lower_limit = slice_locations[index]
+            slice_boundaries = (0, upper_limit, max_width, lower_limit)
+            try:
+                img_slice = combined_img.pil.crop(slice_boundaries)
+            except ValueError:
+                raise SizeLimitError("Images to small to slice")
+            img = combined_img.copy()
+            img.pil = img_slice
+            img_objs.append(img)
+        combined_img.pil.close()
+        return img_objs
```

### Comparing `stitchtoon-1.1.0/src/stitchtoon/services/process.py` & `stitchtoon-1.1.1/src/stitchtoon/services/process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,248 +1,251 @@
-import gc
-import os.path as osp
-from os import PathLike
-
-from stitchtoon.detectors import select_detector
-from stitchtoon.services import ImageHandler
-from stitchtoon.services import ImageManipulator
-from stitchtoon.services import logFunc
-from stitchtoon.services import scan
-from stitchtoon.services.image_directory import Image
-from stitchtoon.services.progressbar import DefaultCliProgress
-from stitchtoon.services.progressbar import ProgressHandler
-from stitchtoon.utils.constants import DETECTION_TYPE
-from stitchtoon.utils.constants import FORMAT_NAME_MAPPER
-from stitchtoon.utils.constants import FORMAT_SIZE_MAPPER
-from stitchtoon.utils.constants import SIZE_LIMITS
-from stitchtoon.utils.constants import ProcessDefaults
-from stitchtoon.utils.constants import StitchDefaults
-from stitchtoon.utils.errors import EmptyImageDir
-from stitchtoon.utils.errors import SizeLimitError
-
-# Must have a sum of 100
-PROGRESS_PERCENTAGE = {
-    "scan": 10,
-    "stitch": 70,
-    "loading": 10,
-    "save": 10,
-}
-
-
-@logFunc()
-def process(
-    input: PathLike,
-    output: PathLike,
-    *,
-    split_height: int = 0,
-    images_number: int = 0,
-    output_format: str = ProcessDefaults.OUTPUT_FORMAT,
-    recursive: bool = ProcessDefaults.RECURSIVE,
-    as_archive: bool = ProcessDefaults.AS_ARCHIVE,
-    lossy_quality: int = ProcessDefaults.LOSSY_QUALITY,
-    show_progress: bool = ProcessDefaults.SHOW_PROGRESS,
-    progress: ProgressHandler = None,
-    params: dict[str, any],
-) -> None:
-    """stitch images in input and save them to output
-
-    Args:
-        input (PathLike)
-        output (PathLike)
-        split_height (int)
-        params (dict[str, any]): stitch params, see stitch function for more info.
-        output_format (str, optional): Defaults to ProcessDefaults.OUTPUT_FORMAT.
-        recursive (bool, optional): Defaults to ProcessDefaults.RECURSIVE.
-        as_archive (bool, optional): Defaults to ProcessDefaults.AS_ARCHIVE.
-        lossy_quality (int, optional): Defaults to ProcessDefaults.LOSSY_QUALITY.
-        show_progress (bool, optional): Defaults to ProcessDefaults.SHOW_PROGRESS.
-        progress (ProgressHandler, optional): progressbar handler. Defaults to None.
-
-    Raises:
-        FileNotFoundError: When input directory could not be found
-        EmptyImageDir: When input directory does not contain supported images
-        Exception: When output is not provided
-    """
-    handler = ImageHandler()
-    progress = progress or _get_progressbar(show_progress)
-
-    if not split_height and not images_number:
-        raise Exception(
-            "split_height and images_number are not provided, Must provide one of theme"
-        )
-
-    format = _get_format_for_size(
-        output_format, max(split_height, params.get("custom_width", 0))
-    )
-
-    if not osp.lexists(input):
-        raise FileNotFoundError(f"Could not found {input}")
-    if not output:
-        raise Exception("Output path is not provided")
-    working_dirs = scan(input, recursive)
-    if not working_dirs:
-        raise EmptyImageDir(
-            "Input directory does not contain supported images. Try again with batch mode."
-        )
-
-    progress.update(progress.value + PROGRESS_PERCENTAGE["scan"], "Stichting")
-    working_dirs_len = len(working_dirs)
-    for image_dir in working_dirs:
-        images_len = len(image_dir.images)
-        per_dir_percentage = PROGRESS_PERCENTAGE["loading"] / working_dirs_len
-        images = handler.load(
-            image_dir.images,
-            progress=progress,
-            increament=per_dir_percentage / images_len,
-        )
-        if not images:
-            continue
-
-        total_images_length = sum(image.height for image in images)
-        if images_number:
-            split_height = total_images_length / images_number
-            format = _get_format_for_size(format, split_height)
-            params["detection_type"] = DETECTION_TYPE.NO_DETECTION.value
-
-        per_dir_percentage = PROGRESS_PERCENTAGE["stitch"] / working_dirs_len
-        images = stitch(
-            images,
-            split_height,
-            progress=progress,
-            increament=per_dir_percentage / images_len,
-            **params,
-        )
-        images_len = len(images)
-        sub_output = output
-
-        if recursive:
-            sub_output = osp.join(output, osp.basename(image_dir.path))
-            if as_archive and osp.splitext(output)[1] != ".zip":
-                sub_output += ".zip"
-        else:
-            if as_archive and osp.splitext(output)[1] != ".zip":
-                sub_output = osp.join(output, f"{osp.basename(image_dir.path)}.zip")
-
-        per_dir_percentage = PROGRESS_PERCENTAGE["save"] / working_dirs_len
-        handler.save_all(
-            output=sub_output,
-            images=images,
-            format=format,
-            as_archive=as_archive,
-            quality=lossy_quality,
-            progress=progress,
-            increament=per_dir_percentage / images_len,
-        )
-    progress.update(100, "Completed")
-    progress.finish()
-    gc.collect()
-
-
-@logFunc()
-def stitch(
-    images: list[Image],
-    split_height: int,
-    *,
-    progress: ProgressHandler = None,
-    increament: int = StitchDefaults.INCREAMENT,
-    detection_type: str = StitchDefaults.DETECTION_TYPE,
-    sensitivity: int = StitchDefaults.SENSITIVITY,
-    width_enforce: str = StitchDefaults.WIDTH_ENFORCE,
-    custom_width: int = StitchDefaults.CUSTOM_WIDTH,
-    line_steps: int = StitchDefaults.LINE_STEPS,
-    ignorable_pixels: int = StitchDefaults.IGNORABLE_PIXELS,
-) -> list[Image]:
-    """Stitchs images to specified heigh
-
-    Args:
-        images (list[Image])
-        split_height (int)
-        progress (ProgressHandler, optional): progressbar handler. Defaults to None.
-        increament (int, optional): progressbar increament factor. Defaults to StitchDefaults.INCREAMENT.
-        detection_type (str, optional): Defaults to StitchDefaults.DETECTION_TYPE.
-        sensitivity (int, optional): Defaults to StitchDefaults.SENSITIVITY.
-        width_enforce (str, optional): Defaults to StitchDefaults.WIDTH_ENFORCE.
-        custom_width (int, optional): Defaults to StitchDefaults.CUSTOM_WIDTH.
-        line_steps (int, optional): Defaults to StitchDefaults.LINE_STEPS.
-        ignorable_pixels (int, optional): Defaults to StitchDefaults.IGNORABLE_PIXELS.
-
-    Returns:
-        list[Images]: stitched images
-    """
-    if not progress:
-        progress = _get_progressbar()
-    detector = select_detector(detection_type=detection_type)
-    images = ImageManipulator.resize(images, width_enforce, custom_width)
-    combined_img = ImageManipulator.combine(
-        images, progress=progress, increament=increament
-    )
-    slice_points = detector.run(
-        combined_img,
-        split_height,
-        sensitivity=sensitivity,
-        ignorable_pixels=ignorable_pixels,
-        scan_step=line_steps,
-    )
-    images = ImageManipulator.slice(combined_img, slice_points)
-
-    return images
-
-
-def _is_size_ok(format: str, size: int) -> bool:
-    """Checks if size excedes format size limit
-
-    Args:
-        format (str)
-        size (int)
-
-    Returns:
-        bool
-    """
-
-    if size > SIZE_LIMITS[format]:
-        return False
-
-    return True
-
-
-def _get_format_for_size(format: str, size: int) -> str:
-    """Gets the right format alternative for current size or raise
-
-    Args:
-        format (str)
-        size (int)
-
-    Raises:
-        SizeLimitError: Whene size is bigger than format size limit
-
-    Returns:
-        str: format
-    """
-
-    format = format.lower()
-    format = FORMAT_NAME_MAPPER.get(format, format)
-
-    if FORMAT_SIZE_MAPPER.get(format) and not _is_size_ok(format, size):
-        format = FORMAT_SIZE_MAPPER.get(format)
-
-    if not _is_size_ok(format, size):
-        raise SizeLimitError(
-            f"Image type {format} supports size up to {SIZE_LIMITS[format]}px only"
-        )
-    else:
-        return format
-
-
-def _get_progressbar(show: bool = False) -> ProgressHandler:
-    """Returns a progress bar handler
-
-    Args:
-        show (bool, optional): Shows a progress bar on the command line. Defaults to False.
-
-    Returns:
-        ProgressHandler
-    """
-
-    if show:
-        return DefaultCliProgress()
-    else:
-        return ProgressHandler()
+import gc
+import os.path as osp
+from os import PathLike
+
+from stitchtoon.detectors import select_detector
+from stitchtoon.services import ImageHandler
+from stitchtoon.services import ImageManipulator
+from stitchtoon.services import logFunc
+from stitchtoon.services import scan
+from stitchtoon.services.image_directory import Image
+from stitchtoon.services.progressbar import DefaultCliProgress
+from stitchtoon.services.progressbar import ProgressHandler
+from stitchtoon.utils.constants import DETECTION_TYPE
+from stitchtoon.utils.constants import FORMAT_NAME_MAPPER
+from stitchtoon.utils.constants import FORMAT_SIZE_MAPPER
+from stitchtoon.utils.constants import SIZE_LIMITS
+from stitchtoon.utils.constants import SUPPORTS_TRANSPARENCY
+from stitchtoon.utils.constants import ProcessDefaults
+from stitchtoon.utils.constants import StitchDefaults
+from stitchtoon.utils.errors import EmptyImageDir
+from stitchtoon.utils.errors import SizeLimitError
+
+# Must have a sum of 100
+PROGRESS_PERCENTAGE = {
+    "scan": 10,
+    "stitch": 70,
+    "loading": 10,
+    "save": 10,
+}
+
+
+@logFunc()
+def process(
+    input: PathLike,
+    output: PathLike,
+    *,
+    split_height: int = 0,
+    images_number: int = 0,
+    output_format: str = ProcessDefaults.OUTPUT_FORMAT,
+    recursive: bool = ProcessDefaults.RECURSIVE,
+    as_archive: bool = ProcessDefaults.AS_ARCHIVE,
+    lossy_quality: int = ProcessDefaults.LOSSY_QUALITY,
+    show_progress: bool = ProcessDefaults.SHOW_PROGRESS,
+    progress: ProgressHandler = None,
+    params: dict[str, any],
+) -> None:
+    """stitch images in input and save them to output
+
+    Args:
+        input (PathLike)
+        output (PathLike)
+        split_height (int)
+        params (dict[str, any]): stitch params, see stitch function for more info.
+        output_format (str, optional): Defaults to ProcessDefaults.OUTPUT_FORMAT.
+        recursive (bool, optional): Defaults to ProcessDefaults.RECURSIVE.
+        as_archive (bool, optional): Defaults to ProcessDefaults.AS_ARCHIVE.
+        lossy_quality (int, optional): Defaults to ProcessDefaults.LOSSY_QUALITY.
+        show_progress (bool, optional): Defaults to ProcessDefaults.SHOW_PROGRESS.
+        progress (ProgressHandler, optional): progressbar handler. Defaults to None.
+
+    Raises:
+        FileNotFoundError: When input directory could not be found
+        EmptyImageDir: When input directory does not contain supported images
+        Exception: When output is not provided
+    """
+    handler = ImageHandler()
+    progress = progress or _get_progressbar(show_progress)
+
+    if not split_height and not images_number:
+        raise Exception(
+            "split_height and images_number are not provided, Must provide one of theme"
+        )
+
+    format = _get_format_for_size(
+        output_format, max(split_height, params.get("custom_width", 0))
+    )
+
+    if not osp.lexists(input):
+        raise FileNotFoundError(f"Could not found {input}")
+    if not output:
+        raise Exception("Output path is not provided")
+    working_dirs = scan(input, recursive)
+    if not working_dirs:
+        raise EmptyImageDir(
+            "Input directory does not contain supported images. Try again with batch mode."
+        )
+
+    progress.update(progress.value + PROGRESS_PERCENTAGE["scan"], "Stichting")
+    working_dirs_len = len(working_dirs)
+    for image_dir in working_dirs:
+        images_len = len(image_dir.images)
+        per_dir_percentage = PROGRESS_PERCENTAGE["loading"] / working_dirs_len
+        transparent = format in SUPPORTS_TRANSPARENCY
+        images = handler.load(
+            image_dir.images,
+            progress=progress,
+            increament=per_dir_percentage / images_len,
+            transparent=transparent,
+        )
+        if not images:
+            continue
+
+        total_images_length = sum(image.height for image in images)
+        if images_number:
+            split_height = total_images_length / images_number
+            format = _get_format_for_size(format, split_height)
+            params["detection_type"] = DETECTION_TYPE.NO_DETECTION.value
+
+        per_dir_percentage = PROGRESS_PERCENTAGE["stitch"] / working_dirs_len
+        images = stitch(
+            images,
+            split_height,
+            progress=progress,
+            increament=per_dir_percentage / images_len,
+            **params,
+        )
+        images_len = len(images)
+        sub_output = output
+
+        if recursive:
+            sub_output = osp.join(output, osp.basename(image_dir.path))
+            if as_archive and osp.splitext(output)[1] != ".zip":
+                sub_output += ".zip"
+        else:
+            if as_archive and osp.splitext(output)[1] != ".zip":
+                sub_output = osp.join(output, f"{osp.basename(image_dir.path)}.zip")
+
+        per_dir_percentage = PROGRESS_PERCENTAGE["save"] / working_dirs_len
+        handler.save_all(
+            output=sub_output,
+            images=images,
+            format=format,
+            as_archive=as_archive,
+            quality=lossy_quality,
+            progress=progress,
+            increament=per_dir_percentage / images_len,
+        )
+    progress.update(100, "Completed")
+    progress.finish()
+    gc.collect()
+
+
+@logFunc()
+def stitch(
+    images: list[Image],
+    split_height: int,
+    *,
+    progress: ProgressHandler = None,
+    increament: int = StitchDefaults.INCREAMENT,
+    detection_type: str = StitchDefaults.DETECTION_TYPE,
+    sensitivity: int = StitchDefaults.SENSITIVITY,
+    width_enforce: str = StitchDefaults.WIDTH_ENFORCE,
+    custom_width: int = StitchDefaults.CUSTOM_WIDTH,
+    line_steps: int = StitchDefaults.LINE_STEPS,
+    ignorable_pixels: int = StitchDefaults.IGNORABLE_PIXELS,
+) -> list[Image]:
+    """Stitchs images to specified heigh
+
+    Args:
+        images (list[Image])
+        split_height (int)
+        progress (ProgressHandler, optional): progressbar handler. Defaults to None.
+        increament (int, optional): progressbar increament factor. Defaults to StitchDefaults.INCREAMENT.
+        detection_type (str, optional): Defaults to StitchDefaults.DETECTION_TYPE.
+        sensitivity (int, optional): Defaults to StitchDefaults.SENSITIVITY.
+        width_enforce (str, optional): Defaults to StitchDefaults.WIDTH_ENFORCE.
+        custom_width (int, optional): Defaults to StitchDefaults.CUSTOM_WIDTH.
+        line_steps (int, optional): Defaults to StitchDefaults.LINE_STEPS.
+        ignorable_pixels (int, optional): Defaults to StitchDefaults.IGNORABLE_PIXELS.
+
+    Returns:
+        list[Images]: stitched images
+    """
+    if not progress:
+        progress = _get_progressbar()
+    detector = select_detector(detection_type=detection_type)
+    images = ImageManipulator.resize(images, width_enforce, custom_width)
+    combined_img = ImageManipulator.combine(
+        images, progress=progress, increament=increament
+    )
+    slice_points = detector.run(
+        combined_img,
+        split_height,
+        sensitivity=sensitivity,
+        ignorable_pixels=ignorable_pixels,
+        scan_step=line_steps,
+    )
+    images = ImageManipulator.slice(combined_img, slice_points)
+
+    return images
+
+
+def _is_size_ok(format: str, size: int) -> bool:
+    """Checks if size excedes format size limit
+
+    Args:
+        format (str)
+        size (int)
+
+    Returns:
+        bool
+    """
+
+    if size > SIZE_LIMITS[format]:
+        return False
+
+    return True
+
+
+def _get_format_for_size(format: str, size: int) -> str:
+    """Gets the right format alternative for current size or raise
+
+    Args:
+        format (str)
+        size (int)
+
+    Raises:
+        SizeLimitError: Whene size is bigger than format size limit
+
+    Returns:
+        str: format
+    """
+
+    format = format.lower()
+    format = FORMAT_NAME_MAPPER.get(format, format)
+
+    if FORMAT_SIZE_MAPPER.get(format) and not _is_size_ok(format, size):
+        format = FORMAT_SIZE_MAPPER.get(format)
+
+    if not _is_size_ok(format, size):
+        raise SizeLimitError(
+            f"Image type {format} supports size up to {SIZE_LIMITS[format]}px only"
+        )
+    else:
+        return format
+
+
+def _get_progressbar(show: bool = False) -> ProgressHandler:
+    """Returns a progress bar handler
+
+    Args:
+        show (bool, optional): Shows a progress bar on the command line. Defaults to False.
+
+    Returns:
+        ProgressHandler
+    """
+
+    if show:
+        return DefaultCliProgress()
+    else:
+        return ProgressHandler()
```

### Comparing `stitchtoon-1.1.0/src/stitchtoon/services/progressbar.py` & `stitchtoon-1.1.1/src/stitchtoon/services/progressbar.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/src/stitchtoon/services/scanner.py` & `stitchtoon-1.1.1/src/stitchtoon/services/scanner.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from __future__ import annotations
-
-import os
-import os.path as osp
-from typing import Iterable
-
-from natsort import natsorted
-
-from ..utils.constants import SUPPORTED_IMG_TYPES
-from .global_logger import logFunc
-from .image_directory import Image
-from .image_directory import ImageDirectory
-
-
-@logFunc()
-def is_supported_img(*, format: str = None, filename: os.PathLike = None) -> bool:
-    """Checks if an image format is supported
-
-    Args:
-        format (str, optional): image format. Defaults to None.
-        filename (os.PathLike, optional): filename with image format extention. Defaults to None.
-
-    Returns:
-        bool
-    """
-
-    format = format or osp.splitext(filename)[1].lower()
-    format = format.strip(".")
-    if format in SUPPORTED_IMG_TYPES:
-        return True
-    return False
-
-
-@logFunc
-def get_format(filename: os.PathLike) -> str:
-    """Gets filename extention
-
-    Args:
-        filename (os.PathLike)
-
-    Returns:
-        str
-    """
-
-    return osp.splitext(filename)[1].lower().strip(".")
-
-
-@logFunc()
-def scanimgdir(input: os.PathLike, sort: bool = True) -> Iterable[ImageDirectory]:
-    """Scan a directory for supported images
-
-    Args:
-        input (os.PathLike): directory path
-        sort (bool, optional): natural sorting. Defaults to True.
-
-    Returns:
-        Iterable[ImageDirectory]
-    """
-
-    images = []
-    for ent in os.scandir(input):
-        if ent.is_file() and is_supported_img(filename=ent.name):
-            images.append(Image(ent.path, ent.name, format=get_format(ent.name)))
-
-    if not images:
-        return None
-    images = natsorted(images, key=lambda x: x.path)
-    image_dir = ImageDirectory(input, images)
-    return (image_dir,)
-
-
-@logFunc()
-def walkimgdir(input: os.PathLike, sort: bool = True) -> Iterable[ImageDirectory]:
-    """Recursivaly scan a directory for supported images
-
-    Args:
-        input (os.PathLike): directory path
-        sort (bool, optional): natural sorting. Defaults to True.
-
-    Returns:
-        Iterable[ImageDirectory]
-    """
-
-    images = []
-    dirspaths = []
-    dirs = []
-    for ent in os.scandir(input):
-        if ent.is_file() and is_supported_img(filename=ent.name):
-            images.append(Image(ent.path, ent.name, format=get_format(ent.name)))
-
-        elif ent.is_dir():
-            dirspaths.append(ent.path)
-
-    if images:
-        images = natsorted(images, key=lambda x: x.path)
-        dirs.append(ImageDirectory(input, images))
-
-    if dirspaths:
-        dirspaths = natsorted(dirspaths)
-
-    for dir in dirspaths:
-        res = walkimgdir(dir, sort)
-        if res:
-            dirs.extend(res)
-
-    return dirs
-
-
-@logFunc()
-def scan(input: os.PathLike, recursive: bool = True) -> Iterable[ImageDirectory]:
-    """scan a directory for supported images
-
-    Args:
-        input (os.PathLike)
-        recursive (bool, optional) Defaults to True.
-
-    Returns:
-        Iterable[ImageDirectory]
-    """
-
-    strategy = walkimgdir if recursive else scanimgdir
-    return strategy(osp.abspath(input))
+from __future__ import annotations
+
+import os
+import os.path as osp
+from typing import Iterable
+
+from natsort import natsorted
+
+from ..utils.constants import SUPPORTED_IMG_TYPES
+from .global_logger import logFunc
+from .image_directory import Image
+from .image_directory import ImageDirectory
+
+
+@logFunc()
+def is_supported_img(*, format: str = None, filename: os.PathLike = None) -> bool:
+    """Checks if an image format is supported
+
+    Args:
+        format (str, optional): image format. Defaults to None.
+        filename (os.PathLike, optional): filename with image format extention. Defaults to None.
+
+    Returns:
+        bool
+    """
+
+    format = format or osp.splitext(filename)[1].lower()
+    format = format.strip(".")
+    if format in SUPPORTED_IMG_TYPES:
+        return True
+    return False
+
+
+@logFunc
+def get_format(filename: os.PathLike) -> str:
+    """Gets filename extention
+
+    Args:
+        filename (os.PathLike)
+
+    Returns:
+        str
+    """
+
+    return osp.splitext(filename)[1].lower().strip(".")
+
+
+@logFunc()
+def scanimgdir(input: os.PathLike, sort: bool = True) -> Iterable[ImageDirectory]:
+    """Scan a directory for supported images
+
+    Args:
+        input (os.PathLike): directory path
+        sort (bool, optional): natural sorting. Defaults to True.
+
+    Returns:
+        Iterable[ImageDirectory]
+    """
+
+    images = []
+    for ent in os.scandir(input):
+        if ent.is_file() and is_supported_img(filename=ent.name):
+            images.append(Image(ent.path, ent.name, format=get_format(ent.name)))
+
+    if not images:
+        return None
+    images = natsorted(images, key=lambda x: x.path)
+    image_dir = ImageDirectory(input, images)
+    return (image_dir,)
+
+
+@logFunc()
+def walkimgdir(input: os.PathLike, sort: bool = True) -> Iterable[ImageDirectory]:
+    """Recursivaly scan a directory for supported images
+
+    Args:
+        input (os.PathLike): directory path
+        sort (bool, optional): natural sorting. Defaults to True.
+
+    Returns:
+        Iterable[ImageDirectory]
+    """
+
+    images = []
+    dirspaths = []
+    dirs = []
+    for ent in os.scandir(input):
+        if ent.is_file() and is_supported_img(filename=ent.name):
+            images.append(Image(ent.path, ent.name, format=get_format(ent.name)))
+
+        elif ent.is_dir():
+            dirspaths.append(ent.path)
+
+    if images:
+        images = natsorted(images, key=lambda x: x.path)
+        dirs.append(ImageDirectory(input, images))
+
+    if dirspaths:
+        dirspaths = natsorted(dirspaths)
+
+    for dir in dirspaths:
+        res = walkimgdir(dir, sort)
+        if res:
+            dirs.extend(res)
+
+    return dirs
+
+
+@logFunc()
+def scan(input: os.PathLike, recursive: bool = True) -> Iterable[ImageDirectory]:
+    """scan a directory for supported images
+
+    Args:
+        input (os.PathLike)
+        recursive (bool, optional) Defaults to True.
+
+    Returns:
+        Iterable[ImageDirectory]
+    """
+
+    strategy = walkimgdir if recursive else scanimgdir
+    return strategy(osp.abspath(input))
```

### Comparing `stitchtoon-1.1.0/tests/test/data/01.jpeg` & `stitchtoon-1.1.1/tests/test/data/01.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/tests/test/data/01.webp` & `stitchtoon-1.1.1/tests/test/data/01.webp`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/tests/test/data/02.jpeg` & `stitchtoon-1.1.1/tests/test/data/02.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/tests/test/data/03.jpeg` & `stitchtoon-1.1.1/tests/test/data/03.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/tests/test/data/04.jpeg` & `stitchtoon-1.1.1/tests/test/data/04.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/tests/test/test_manipulator.py` & `stitchtoon-1.1.1/tests/test/test_manipulator.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/tests/test/test_scan.py` & `stitchtoon-1.1.1/tests/test/test_scan.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.0/PKG-INFO` & `stitchtoon-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stitchtoon
-Version: 1.1.0
+Version: 1.1.1
 Summary: A powerful program for stitching and cutting webtoons/manhwa/manhua raws.
 Keywords: manga,webtoon,stitch,slice,combin
 Author-email: Beshr Alghalil <beshrghalil@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stitchtoon Version: 1.1.0 Summary: A powerful
+Metadata-Version: 2.1 Name: stitchtoon Version: 1.1.1 Summary: A powerful
 program for stitching and cutting webtoons/manhwa/manhua raws. Keywords:
 manga,webtoon,stitch,slice,combin Author-email: Beshr Alghalil
 protonmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Dist: psd_tools Requires-Dist: natsort Requires-Dist: pillow Requires-
 Dist: progress Requires-Dist: black ; extra == "dev" Requires-Dist: flake8 ;
```

