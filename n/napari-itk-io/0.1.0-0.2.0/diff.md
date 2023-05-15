# Comparing `tmp/napari-itk-io-0.1.0.tar.gz` & `tmp/napari-itk-io-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-itk-io-0.1.0.tar", last modified: Thu Apr 29 04:38:00 2021, max compression
+gzip compressed data, was "napari-itk-io-0.2.0.tar", last modified: Mon Mar 28 13:57:40 2022, max compression
```

## Comparing `napari-itk-io-0.1.0.tar` & `napari-itk-io-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2021-04-29 04:38:00.769681 napari-itk-io-0.1.0/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2021-04-29 04:38:00.769681 napari-itk-io-0.1.0/.github/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2021-04-29 04:38:00.769681 napari-itk-io-0.1.0/.github/workflows/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3058 2021-04-28 22:28:39.000000 napari-itk-io-0.1.0/.github/workflows/test_and_deploy.yml
--rw-rw-r--   0 matt      (1000) matt      (1000)      947 2021-04-28 21:36:39.000000 napari-itk-io-0.1.0/.gitignore
--rw-rw-r--   0 matt      (1000) matt      (1000)    11358 2021-04-28 21:36:39.000000 napari-itk-io-0.1.0/LICENSE
--rw-rw-r--   0 matt      (1000) matt      (1000)      121 2021-04-28 21:36:39.000000 napari-itk-io-0.1.0/MANIFEST.in
--rw-rw-r--   0 matt      (1000) matt      (1000)     5065 2021-04-29 04:38:00.769681 napari-itk-io-0.1.0/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     3590 2021-04-29 04:27:15.000000 napari-itk-io-0.1.0/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2021-04-29 04:38:00.769681 napari-itk-io-0.1.0/napari_itk_io/
--rw-rw-r--   0 matt      (1000) matt      (1000)      201 2021-04-29 03:09:51.000000 napari-itk-io-0.1.0/napari_itk_io/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3986 2021-04-29 04:22:30.000000 napari-itk-io-0.1.0/napari_itk_io/_reader.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2021-04-29 04:38:00.769681 napari-itk-io-0.1.0/napari_itk_io/_tests/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2021-04-28 21:36:39.000000 napari-itk-io-0.1.0/napari_itk_io/_tests/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4646 2021-04-29 04:03:32.000000 napari-itk-io-0.1.0/napari_itk_io/_tests/test_reader.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       92 2021-04-28 21:36:39.000000 napari-itk-io-0.1.0/napari_itk_io/_tests/test_writer.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      142 2021-04-29 04:38:00.000000 napari-itk-io-0.1.0/napari_itk_io/_version.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      463 2021-04-28 21:36:39.000000 napari-itk-io-0.1.0/napari_itk_io/_writer.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2021-04-29 04:38:00.769681 napari-itk-io-0.1.0/napari_itk_io.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)     5065 2021-04-29 04:38:00.000000 napari-itk-io-0.1.0/napari_itk_io.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      543 2021-04-29 04:38:00.000000 napari-itk-io-0.1.0/napari_itk_io.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2021-04-29 04:38:00.000000 napari-itk-io-0.1.0/napari_itk_io.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       47 2021-04-29 04:38:00.000000 napari-itk-io-0.1.0/napari_itk_io.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       70 2021-04-29 04:38:00.000000 napari-itk-io-0.1.0/napari_itk_io.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2021-04-29 04:38:00.000000 napari-itk-io-0.1.0/napari_itk_io.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       70 2021-04-29 00:04:41.000000 napari-itk-io-0.1.0/requirements.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2021-04-29 04:38:00.769681 napari-itk-io-0.1.0/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     1817 2021-04-28 22:02:00.000000 napari-itk-io-0.1.0/setup.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      851 2021-04-28 21:36:39.000000 napari-itk-io-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:57:40.970102 napari-itk-io-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:57:40.966102 napari-itk-io-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:57:40.970102 napari-itk-io-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4614 2022-03-28 13:57:40.970102 napari-itk-io-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3736 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-03-28 13:57:40.970102 napari-itk-io-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:57:40.966102 napari-itk-io-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:57:40.970102 napari-itk-io-0.2.0/src/napari_itk_io/
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/src/napari_itk_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/src/napari_itk_io/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:57:40.970102 napari-itk-io-0.2.0/src/napari_itk_io/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/src/napari_itk_io/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4645 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/src/napari_itk_io/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/src/napari_itk_io/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-03-28 13:57:39.000000 napari-itk-io-0.2.0/src/napari_itk_io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/src/napari_itk_io/_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/src/napari_itk_io/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:57:40.970102 napari-itk-io-0.2.0/src/napari_itk_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4614 2022-03-28 13:57:40.000000 napari-itk-io-0.2.0/src/napari_itk_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-03-28 13:57:40.000000 napari-itk-io-0.2.0/src/napari_itk_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-28 13:57:40.000000 napari-itk-io-0.2.0/src/napari_itk_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-03-28 13:57:40.000000 napari-itk-io-0.2.0/src/napari_itk_io.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-03-28 13:57:40.000000 napari-itk-io-0.2.0/src/napari_itk_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-28 13:57:40.000000 napari-itk-io-0.2.0/src/napari_itk_io.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-03-28 13:57:17.000000 napari-itk-io-0.2.0/tox.ini
```

### Comparing `napari-itk-io-0.1.0/.github/workflows/test_and_deploy.yml` & `napari-itk-io-0.2.0/.github/workflows/test_and_deploy.yml`

 * *Files 16% similar despite different names*

```diff
@@ -2,74 +2,70 @@
 # For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
 
 name: tests
 
 on: 
   push:
     branches:
-      - master
       - main
+      - npe2
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
   pull_request:
     branches:
-      - master
       - main
+      - npe2
   workflow_dispatch:
 
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
-        platform: [ubuntu-latest, macos-latest]
-        python-version: [3.7, 3.8, 3.9]
+        platform: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: [3.8, 3.9, '3.10']
 
     steps:
       - uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
-      # these libraries, along with pytest-xvfb (added in the `deps` in tox.ini),
-      # enable testing on Qt on linux
-      - name: Install Linux libraries
-        if: runner.os == 'Linux'
-        run: |
-          sudo apt-get install -y libdbus-1-3 libxkbcommon-x11-0 libxcb-icccm4 \
-            libxcb-image0 libxcb-keysyms1 libxcb-randr0 libxcb-render-util0 \
-            libxcb-xinerama0 libxcb-xinput0 libxcb-xfixes0
+      # these libraries enable testing on Qt on linux
+      - uses: tlambert03/setup-qt-libs@v1
 
       # strategy borrowed from vispy for installing opengl libs on windows
       - name: Install Windows OpenGL
         if: runner.os == 'Windows'
         run: |
-          git clone --depth 1 git://github.com/pyvista/gl-ci-helpers.git
+          git clone --depth 1 https://github.com/pyvista/gl-ci-helpers.git
           powershell gl-ci-helpers/appveyor/install_opengl.ps1
 
       # note: if you need dependencies from conda, considering using
       # setup-miniconda: https://github.com/conda-incubator/setup-miniconda
       # and
       # tox-conda: https://github.com/tox-dev/tox-conda
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install setuptools tox tox-gh-actions
+          python -m pip install setuptools tox tox-gh-actions
 
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
-        run: tox
+        uses: GabrielBB/xvfb-action@v1
+        with:
+          run: python -m tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
-        uses: codecov/codecov-action@v1
+        uses: codecov/codecov-action@v2
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your 
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
@@ -79,16 +75,17 @@
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -U setuptools setuptools_scm wheel twine
+          pip install -U setuptools setuptools_scm wheel twine build
       - name: Build and publish
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
         run: |
           git tag
-          python setup.py sdist bdist_wheel
+          python -m build .
           twine upload dist/*
+
```

### Comparing `napari-itk-io-0.1.0/.gitignore` & `napari-itk-io-0.2.0/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -62,18 +62,24 @@
 
 # MkDocs documentation
 /site/
 
 # PyBuilder
 target/
 
+# Pycharm and VSCode
+.idea/
+venv/
+.vscode/
+
 # IPython Notebook
 .ipynb_checkpoints
 
 # pyenv
 .python-version
 
 # OS
 .DS_Store
 
 # written by setuptools_scm
-*/_version.py
+**/_version.py
+
```

### Comparing `napari-itk-io-0.1.0/LICENSE` & `napari-itk-io-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-itk-io-0.1.0/README.md` & `napari-itk-io-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 [![License](https://img.shields.io/pypi/l/napari-itk-io.svg?color=green)](https://github.com/InsightSoftwareConsortium/napari-itk-io/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-itk-io.svg?color=green)](https://pypi.org/project/napari-itk-io)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-itk-io.svg?color=green)](https://python.org)
 [![tests](https://github.com/InsightSoftwareConsortium/napari-itk-io/workflows/tests/badge.svg)](https://github.com/InsightSoftwareConsortium/napari-itk-io/actions)
 [![codecov](https://codecov.io/gh/InsightSoftwareConsortium/napari-itk-io/branch/master/graph/badge.svg)](https://codecov.io/gh/InsightSoftwareConsortium/napari-itk-io)
 
-File IO with itk for napari.
+File IO with [itk](https://itk.org) for [napari](https://napari.org).
+
+Image metadata, e.g. the pixel spacing, origin, and metadata tags, are preserved and passed into napari.
 
 Supported image file formats:
 
 - [BioRad](http://www.bio-rad.com/)
 - [BMP](https://en.wikipedia.org/wiki/BMP_file_format)
 - [DICOM](http://dicom.nema.org/)
 - [DICOM Series](http://dicom.nema.org/)
@@ -67,8 +69,8 @@
 [Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [file an issue]: https://github.com/InsightSoftwareConsortium/napari-itk-io/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
+[PyPI]: https://pypi.org/
```

### Comparing `napari-itk-io-0.1.0/napari_itk_io/_reader.py` & `napari-itk-io-0.2.0/src/napari_itk_io/_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 This module provides itk-based file reading functionality in a reader plugin for napari.
 
 """
 from pathlib import Path
-import numpy as np
 import itk
 from itk_napari_conversion import image_layer_from_image
-from napari_plugin_engine import napari_hook_implementation
 
-@napari_hook_implementation
+
 def napari_get_reader(path):
     """An itk implementation of the napari_get_reader hook specification.
 
     Parameters
     ----------
     path : str or list of str
         Path to file, or list of paths.
```

### Comparing `napari-itk-io-0.1.0/napari_itk_io/_tests/test_reader.py` & `napari-itk-io-0.2.0/src/napari_itk_io/_tests/test_reader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -121,8 +121,8 @@
 
     # make sure it's the same as it started
     np.testing.assert_allclose(original_data, layer_data_tuple[0])
     np.testing.assert_allclose(np.array(origin)[::-1], layer_data_tuple[1]['translate'])
 
 def test_get_reader_pass():
     reader = napari_get_reader("fake.file")
-    assert reader is None
+    assert reader is None
```

### Comparing `napari-itk-io-0.1.0/tox.ini` & `napari-itk-io-0.2.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # For more information about tox, see https://tox.readthedocs.io/en/latest/
 [tox]
-envlist = py{37,38,39}-{linux,macos,windows}
+envlist = py{38,39,310}-{linux,macos,windows}
+isolated_build=true
 
 [gh-actions]
 python =
-    3.7: py37
     3.8: py38
     3.9: py39
+    3.10: py310
     
 [gh-actions:env]
 PLATFORM =
     ubuntu-latest: linux
     macos-latest: macos
     windows-latest: windows
 
@@ -24,15 +25,17 @@
     GITHUB_ACTIONS
     DISPLAY XAUTHORITY
     NUMPY_EXPERIMENTAL_ARRAY_FUNCTION
     PYVISTA_OFF_SCREEN
 deps = 
     pytest  # https://docs.pytest.org/en/latest/contents.html
     pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
-    pytest-xvfb ; sys_platform == 'linux'
     # you can remove these if you don't use them
     napari
-    magicgui
     pytest-qt
     qtpy
     pyqt5
+    numpy
+    itk-io
+    itk-napari-conversion
+
 commands = pytest -v --color=yes --cov=napari_itk_io --cov-report=xml
```

