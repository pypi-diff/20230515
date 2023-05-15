# Comparing `tmp/colorsysx-0.1.tar.gz` & `tmp/colorsysx-0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorsysx-0.1.tar", last modified: Sat May 13 18:51:17 2023, max compression
+gzip compressed data, was "colorsysx-0.2a1.tar", last modified: Mon May 15 12:23:23 2023, max compression
```

## Comparing `colorsysx-0.1.tar` & `colorsysx-0.2a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      506 2023-05-13 17:41:09.960408 colorsysx-0.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       53 2023-05-11 22:49:25.520127 colorsysx-0.1/.gitignore
--rw-r--r--   0        0        0    32422 2023-05-11 09:15:26.337556 colorsysx-0.1/LICENSE
--rw-r--r--   0        0        0     1963 2023-05-13 18:44:55.089756 colorsysx-0.1/README.md
--rw-r--r--   0        0        0     1446 2023-05-13 18:48:36.475462 colorsysx-0.1/colorsysx/__init__.py
--rw-r--r--   0        0        0     5538 2023-05-13 16:33:15.954469 colorsysx-0.1/colorsysx/_glhs.py
--rw-r--r--   0        0        0     4279 2023-05-13 16:30:13.433488 colorsysx-0.1/colorsysx/_hcy.py
--rw-r--r--   0        0        0      379 2023-05-11 02:07:41.913560 colorsysx-0.1/colorsysx/_helpers.py
--rw-r--r--   0        0        0      741 2023-05-13 16:25:55.939388 colorsysx-0.1/colorsysx/_swizzle.py
--rw-r--r--   0        0        0     2760 2023-05-13 16:30:36.870102 colorsysx-0.1/colorsysx/_yuv.py
--rw-r--r--   0        0        0     1807 2023-05-13 00:51:20.967395 colorsysx-0.1/colorsysx/weights.py
--rw-r--r--   0        0        0      688 2023-05-13 18:47:24.806900 colorsysx-0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-13 01:06:47.992623 colorsysx-0.1/tests/__init__.py
--rw-r--r--   0        0        0      319 2023-05-13 01:01:00.825464 colorsysx-0.1/tests/context.py
--rw-r--r--   0        0        0     3703 2023-05-13 00:58:20.387916 colorsysx-0.1/tests/test_glhs.py
--rw-r--r--   0        0        0     2749 2023-05-13 00:50:11.754849 colorsysx-0.1/tests/test_hcy.py
--rw-r--r--   0        0        0      592 2023-05-13 16:25:28.626827 colorsysx-0.1/tests/test_swizzle.py
--rw-r--r--   0        0        0      799 2023-05-13 01:05:35.215977 colorsysx-0.1/tests/test_weights.py
--rw-r--r--   0        0        0     1673 2023-05-13 01:06:48.008623 colorsysx-0.1/tests/test_yuv.py
--rw-r--r--   0        0        0      845 2023-05-13 16:31:02.878793 colorsysx-0.1/tox.ini
--rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 colorsysx-0.1/PKG-INFO
+-rw-r--r--   0        0        0      506 2023-05-13 17:41:09.960408 colorsysx-0.2a1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       53 2023-05-11 22:49:25.520127 colorsysx-0.2a1/.gitignore
+-rw-r--r--   0        0        0    32422 2023-05-11 09:15:26.337556 colorsysx-0.2a1/LICENSE
+-rw-r--r--   0        0        0     3082 2023-05-15 12:22:59.382536 colorsysx-0.2a1/README.md
+-rw-r--r--   0        0        0     1448 2023-05-13 19:38:00.135300 colorsysx-0.2a1/colorsysx/__init__.py
+-rw-r--r--   0        0        0     5538 2023-05-15 12:22:59.386536 colorsysx-0.2a1/colorsysx/_glhs.py
+-rw-r--r--   0        0        0     4279 2023-05-15 12:22:59.386536 colorsysx-0.2a1/colorsysx/_hcy.py
+-rw-r--r--   0        0        0      379 2023-05-11 02:07:41.913560 colorsysx-0.2a1/colorsysx/_helpers.py
+-rw-r--r--   0        0        0      741 2023-05-13 16:25:55.939388 colorsysx-0.2a1/colorsysx/_swizzle.py
+-rw-r--r--   0        0        0     2760 2023-05-13 16:30:36.870102 colorsysx-0.2a1/colorsysx/_yuv.py
+-rw-r--r--   0        0        0     1807 2023-05-13 00:51:20.967395 colorsysx-0.2a1/colorsysx/weights.py
+-rw-r--r--   0        0        0      688 2023-05-13 18:47:24.806900 colorsysx-0.2a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-13 01:06:47.992623 colorsysx-0.2a1/tests/__init__.py
+-rw-r--r--   0        0        0      319 2023-05-13 01:01:00.825464 colorsysx-0.2a1/tests/context.py
+-rw-r--r--   0        0        0     3703 2023-05-15 12:22:59.386536 colorsysx-0.2a1/tests/test_glhs.py
+-rw-r--r--   0        0        0     2749 2023-05-15 12:22:59.386536 colorsysx-0.2a1/tests/test_hcy.py
+-rw-r--r--   0        0        0      592 2023-05-13 16:25:28.626827 colorsysx-0.2a1/tests/test_swizzle.py
+-rw-r--r--   0        0        0      799 2023-05-13 01:05:35.215977 colorsysx-0.2a1/tests/test_weights.py
+-rw-r--r--   0        0        0     1673 2023-05-13 01:06:48.008623 colorsysx-0.2a1/tests/test_yuv.py
+-rw-r--r--   0        0        0      865 2023-05-13 19:25:52.937780 colorsysx-0.2a1/tox.ini
+-rw-r--r--   0        0        0     3609 1970-01-01 00:00:00.000000 colorsysx-0.2a1/PKG-INFO
```

### Comparing `colorsysx-0.1/LICENSE` & `colorsysx-0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/colorsysx/__init__.py` & `colorsysx-0.2a1/colorsysx/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 See the corresponding module help texts for further details about each
 model. All of the colour spaces added by this package can be
 parameterized to tune them for different tasks. See the
 colorsysx.weights module for details.
 
 """
 
-__version__ = "0.1"
+__version__ = "0.2a1"
 
 # Imports::
 
 # Import just the functions,
 # people wanting weights can import .weights submodule.
 from ._yuv import rgb_to_yuv, yuv_to_rgb  # noqa: F401
 from ._hcy import rgb_to_hcy, hcy_to_rgb  # noqa: F401
```

### Comparing `colorsysx-0.1/colorsysx/_glhs.py` & `colorsysx-0.2a1/colorsysx/_glhs.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/colorsysx/_hcy.py` & `colorsysx-0.2a1/colorsysx/_hcy.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/colorsysx/_swizzle.py` & `colorsysx-0.2a1/colorsysx/_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/colorsysx/_yuv.py` & `colorsysx-0.2a1/colorsysx/_yuv.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/colorsysx/weights.py` & `colorsysx-0.2a1/colorsysx/weights.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/pyproject.toml` & `colorsysx-0.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/tests/test_glhs.py` & `colorsysx-0.2a1/tests/test_glhs.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/tests/test_hcy.py` & `colorsysx-0.2a1/tests/test_hcy.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/tests/test_swizzle.py` & `colorsysx-0.2a1/tests/test_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/tests/test_weights.py` & `colorsysx-0.2a1/tests/test_weights.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/tests/test_yuv.py` & `colorsysx-0.2a1/tests/test_yuv.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.1/tox.ini` & `colorsysx-0.2a1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -16,31 +16,32 @@
 # }}}
 # Test environments {{{
 
 [testenv]
 description = run tests using pytest
 deps =
     pytest >= 7,<8
-skip_install = True
 setenv =
     PYTHONDONTWRITEBYTECODE=1
 commands =
     {posargs:pytest --showlocals --doctest-modules -- tests}
 
 
 [testenv:linter]
 description = run the flake8 linter
 deps =
     flake8 >= 6,<7
+skip_install = True
 commands =
     {posargs:flake8 -- colorsysx tests}
 
 
 [testenv:pydoc]
 description = run pydoc on {posargs}
 deps =
 passenv = TERM
+skip_install = True
 commands =
     python -m pydoc {posargs}
 
 
 # }}}
```

### Comparing `colorsysx-0.1/PKG-INFO` & `colorsysx-0.2a1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: colorsysx
-Version: 0.1
+Version: 0.2a1
 Summary: Extra, human-relevant, colour spaces derived from RGB.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/achadwick/python-colorsysx/python-package.yml?branch=main)
+![PyPI](https://img.shields.io/pypi/v/colorsysx)
 ![GitHub](https://img.shields.io/github/license/achadwick/python-colorsysx)
+![GitHub issues](https://img.shields.io/github/issues/achadwick/python-colorsysx)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/achadwick/python-colorsysx/python-package.yml?branch=main)
 
 # colorsysX
 
 🎨👁️ _Extra, human-relevant, colour spaces derived from RGB_
 
 This package extends the standard Python library's `colorsys` module
 with a few additional, useful, colour spaces. The models of colour
@@ -36,14 +38,28 @@
 YUV's. It's particularly useful when manipulating colours to meet WCAG
 2.2 or draft 3.0 WCAG contrast criteria.
 
 [GLHS][3] is a generalization of the cylindrical coordinate spaces
 provided in `colorsysx` and `colorsys`. It can be parameterised to
 provide any of the other similar models.
 
+# For developers
+
+ColorsysX is library code, with no bundled scripts. Other projects are
+free to depend on it inthe normal way.
+
+## Installation
+
+To install the [latest version from PyPI][4], for example into your
+current Python virtual environment:
+
+```sh
+pip install colorsysx
+```
+
 ## Interface conventions
 
 ```python
 from colorsysx import rgb_to_hcy, hcy_to_rgb
 
 h, c, y = rgb_to_hcy(0.5, 0.7, 0.93)
 r, g, b = hcy_to_rgb(h, c, y)
@@ -56,11 +72,36 @@
     rgb_to_abc() → a, b, c
     abc_to_rgb() → r, g, b
 
 All inputs and outputs are tuples of 3 floats in the range [0.0, 1.0].
 Unlike `colorsysx`, the functions accept optional weighting parameters,
 which can be used to tune the colour model being used.
 
+## Testing and developing
+
+ColorsysX is developed on GitHub as [achadwick/python-colorsysx][5].
+Please report bugs via the [issue tracker][6] there.
+
+ColorsysX uses [tox][7] to run tests and manage utility Python
+environments. Examples:
+
+```sh
+# Run all standard tests in parallel on all available Pythons
+tox -p
+
+# Run the system version of Python interactively in a venv with
+# colorsysx available.
+tox -e py python
+```
+
+The build system is [flit][8], and the project is PEP 621 and PEP 517
+compliant.
+
 [1]: https://en.wikipedia.org/wiki/YUV#Related_color_models
 [2]: https://chilliant.com/rgb2hsv.html
 [3]: https://doi.org/10.1006/cgip.1993.1019
+[4]: https://pypi.org/project/colorsysx/
+[5]: https://github.com/achadwick/python-colorsysx
+[6]: https://github.com/achadwick/python-colorsysx/issues
+[7]: https://tox.wiki/
+[8]: https://flit.pypa.io
```

