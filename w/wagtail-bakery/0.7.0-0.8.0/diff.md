# Comparing `tmp/wagtail-bakery-0.7.0.tar.gz` & `tmp/wagtail-bakery-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-bakery-0.7.0.tar", last modified: Sat Mar 18 17:47:24 2023, max compression
+gzip compressed data, was "wagtail-bakery-0.8.0.tar", last modified: Mon May 15 07:28:33 2023, max compression
```

## Comparing `wagtail-bakery-0.7.0.tar` & `wagtail-bakery-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 loicteixeira   (501) staff       (20)        0 2023-03-18 17:47:24.447211 wagtail-bakery-0.7.0/
--rw-r--r--   0 loicteixeira   (501) staff       (20)     2499 2023-03-18 17:46:16.000000 wagtail-bakery-0.7.0/CHANGELOG.md
--rw-r--r--   0 loicteixeira   (501) staff       (20)     1073 2023-03-18 08:39:43.000000 wagtail-bakery-0.7.0/LICENSE
--rw-r--r--   0 loicteixeira   (501) staff       (20)      192 2023-03-18 08:39:43.000000 wagtail-bakery-0.7.0/MANIFEST.in
--rw-r--r--   0 loicteixeira   (501) staff       (20)     7681 2023-03-18 17:47:24.447279 wagtail-bakery-0.7.0/PKG-INFO
--rw-r--r--   0 loicteixeira   (501) staff       (20)     6583 2023-03-18 09:16:52.000000 wagtail-bakery-0.7.0/README.md
--rw-r--r--   0 loicteixeira   (501) staff       (20)      399 2023-03-18 17:47:24.447515 wagtail-bakery-0.7.0/setup.cfg
--rw-r--r--   0 loicteixeira   (501) staff       (20)     1711 2023-03-18 17:46:16.000000 wagtail-bakery-0.7.0/setup.py
-drwxr-xr-x   0 loicteixeira   (501) staff       (20)        0 2023-03-18 17:47:24.445477 wagtail-bakery-0.7.0/src/
-drwxr-xr-x   0 loicteixeira   (501) staff       (20)        0 2023-03-18 17:47:24.447100 wagtail-bakery-0.7.0/src/wagtail_bakery.egg-info/
--rw-r--r--   0 loicteixeira   (501) staff       (20)      296 2023-03-18 17:47:24.000000 wagtail-bakery-0.7.0/src/wagtail_bakery.egg-info/SOURCES.txt
-drwxr-xr-x   0 loicteixeira   (501) staff       (20)        0 2023-03-18 17:47:24.446714 wagtail-bakery-0.7.0/src/wagtailbakery/
--rw-r--r--   0 loicteixeira   (501) staff       (20)       65 2023-03-18 08:39:43.000000 wagtail-bakery-0.7.0/src/wagtailbakery/__init__.py
--rw-r--r--   0 loicteixeira   (501) staff       (20)     6212 2023-03-18 09:16:52.000000 wagtail-bakery-0.7.0/src/wagtailbakery/api_views.py
--rw-r--r--   0 loicteixeira   (501) staff       (20)      293 2023-03-18 08:39:43.000000 wagtail-bakery-0.7.0/src/wagtailbakery/apps.py
--rw-r--r--   0 loicteixeira   (501) staff       (20)      796 2023-03-18 08:39:43.000000 wagtail-bakery-0.7.0/src/wagtailbakery/models.py
--rw-r--r--   0 loicteixeira   (501) staff       (20)      697 2023-03-18 09:16:52.000000 wagtail-bakery-0.7.0/src/wagtailbakery/signal_handlers.py
-drwxr-xr-x   0 loicteixeira   (501) staff       (20)        0 2023-03-18 17:47:24.445567 wagtail-bakery-0.7.0/src/wagtailbakery/templates/
-drwxr-xr-x   0 loicteixeira   (501) staff       (20)        0 2023-03-18 17:47:24.446836 wagtail-bakery-0.7.0/src/wagtailbakery/templates/wagtailbakery/
--rw-r--r--   0 loicteixeira   (501) staff       (20)      330 2023-03-18 08:39:43.000000 wagtail-bakery-0.7.0/src/wagtailbakery/templates/wagtailbakery/redirect.html
--rw-r--r--   0 loicteixeira   (501) staff       (20)     4493 2023-03-18 10:41:43.000000 wagtail-bakery-0.7.0/src/wagtailbakery/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:28:33.224874 wagtail-bakery-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-05-15 07:28:33.224874 wagtail-bakery-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-15 07:28:33.224874 wagtail-bakery-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:28:33.220874 wagtail-bakery-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:28:33.224874 wagtail-bakery-0.8.0/src/wagtail_bakery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 07:28:33.000000 wagtail-bakery-0.8.0/src/wagtail_bakery.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:28:33.224874 wagtail-bakery-0.8.0/src/wagtailbakery/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/src/wagtailbakery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/src/wagtailbakery/api_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/src/wagtailbakery/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/src/wagtailbakery/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/src/wagtailbakery/signal_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:28:33.220874 wagtail-bakery-0.8.0/src/wagtailbakery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:28:33.224874 wagtail-bakery-0.8.0/src/wagtailbakery/templates/wagtailbakery/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/src/wagtailbakery/templates/wagtailbakery/redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-15 07:28:28.000000 wagtail-bakery-0.8.0/src/wagtailbakery/views.py
```

### Comparing `wagtail-bakery-0.7.0/CHANGELOG.md` & `wagtail-bakery-0.8.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
-## [Unreleased](https://github.com/wagtail-nest/wagtail-bakery/compare/0.7.0...HEAD)
+## [Unreleased](https://github.com/wagtail-nest/wagtail-bakery/compare/0.8.0...HEAD)
 
 Nothing yet
 
+## [0.8.0](https://github.com/wagtail-nest/wagtail-bakery/compare/0.7.0...0.8.0)
+
+### Added
+
+- Compatibility with Wagtail 5.0 and Django 4.2. [#86](https://github.com/wagtail-nest/wagtail-bakery/pull/86)
+- (Development) Update factory-boy to 3.x [#87](https://github.com/wagtail-nest/wagtail-bakery/pull/87)
+
 ## [0.7.0](https://github.com/wagtail-nest/wagtail-bakery/compare/0.6.0...0.7.0)
 
 ### Added
 
 - Compatibility with Python 3.11 and Wagtail 4.2. [#79](https://github.com/wagtail/wagtail-bakery/pull/79)
 
 ### Fixed
```

### Comparing `wagtail-bakery-0.7.0/LICENSE` & `wagtail-bakery-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-bakery-0.7.0/PKG-INFO` & `wagtail-bakery-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: wagtail-bakery
-Version: 0.7.0
+Version: 0.8.0
 Summary: A set of helpers for baking your Django Wagtail site out as flat files.
 Home-page: https://github.com/wagtail-nest/wagtail-bakery/
 Author: Rob Moorman and Wagtail Core Team
 Author-email: hello@wagtail.io
 License: MIT
 Project-URL: Source, https://github.com/wagtail-nest/wagtail-bakery/
 Project-URL: Issue tracker, https://github.com/wagtail-nest/wagtail-bakery/issues/
 Project-URL: Changelog, https://github.com/wagtail-nest/wagtail-bakery/blob/main/CHANGELOG.md
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -177,22 +178,27 @@
 Test as follow:
 
 - All supported Django/Wagtail combinations with the latest supported Python version.
 - The latest supported Django/Wagtail combination for the remaining Python versions.
 
 ### Releases
 
-1. Ensure you have the latest versions of `pip`, `setuptools` and `twine` installed in your virtual environment.
 1. Create a new branch (e.g. `release/1.1.3`) for the release of the new version.
 1. Update the version number in `setup.py` following [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 1. Update `CHANGELOG.md`.
 1. On GitHub, create a pull request and squash merge it.
-1. Checkout and pull the `main` branch locally.
-1. (Optional) If you need to verify anything, use `make publish-test` to upload to https://test.pypi.org and enter your PyPi _test_ credentials as needed.
-1. Use `make publish` and enter your PyPi credentials as needed.
+1. On GitHub, if this is a minor release bump (for example `1.1.0` or `1.2.0` but not `1.1.1`, `1.2.3`), create a `stable/1.1.x` branch from `main`.
+1. (Optional) Publish to TestPyPI if you need to verify anything:
+   1. Create and push a tag following the pattern `X.Y.Z.devN` (for example `1.1.3.dev1`).
+   1. Follow the action progress for the [Publish to TestPyPI](https://github.com/wagtail-nest/wagtail-bakery/actions/workflows/publish-test.yml) workflow.
+   1. Check the result on [TestPyPI: wagtail-bakery](https://test.pypi.org/project/wagtail-bakery/).
+1. Publish to PyPI:
+   1. Create and push a tag following [PEP 440 – Version Identification Specification](https://peps.python.org/pep-0440/) (for example `1.1.3` or `1.1.3rc1`), except for the `.devN` suffix used for testing (see _Publish to TestPyPI_ step above)
+   1. Follow the action progress for the [Publish to PyPI](https://github.com/wagtail-nest/wagtail-bakery/actions/workflows/publish.yml) workflow
+   1. Check the result on [PyPI: wagtail-bakery](https://pypi.org/project/wagtail-bakery/)
 1. On GitHub, create a release and a tag for the new version.
 
 ## Credits
 
 Thanks to [@mhnbcu](https://github.com/mhnbcu/wagtailbakery) for bringing this
 idea up initially, and [Django Bakery](https://github.com/datadesk/django-bakery)
 for providing the initial bakery package.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wagtail-bakery-0.7.0/README.md` & `wagtail-bakery-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -151,22 +151,27 @@
 Test as follow:
 
 - All supported Django/Wagtail combinations with the latest supported Python version.
 - The latest supported Django/Wagtail combination for the remaining Python versions.
 
 ### Releases
 
-1. Ensure you have the latest versions of `pip`, `setuptools` and `twine` installed in your virtual environment.
 1. Create a new branch (e.g. `release/1.1.3`) for the release of the new version.
 1. Update the version number in `setup.py` following [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 1. Update `CHANGELOG.md`.
 1. On GitHub, create a pull request and squash merge it.
-1. Checkout and pull the `main` branch locally.
-1. (Optional) If you need to verify anything, use `make publish-test` to upload to https://test.pypi.org and enter your PyPi _test_ credentials as needed.
-1. Use `make publish` and enter your PyPi credentials as needed.
+1. On GitHub, if this is a minor release bump (for example `1.1.0` or `1.2.0` but not `1.1.1`, `1.2.3`), create a `stable/1.1.x` branch from `main`.
+1. (Optional) Publish to TestPyPI if you need to verify anything:
+   1. Create and push a tag following the pattern `X.Y.Z.devN` (for example `1.1.3.dev1`).
+   1. Follow the action progress for the [Publish to TestPyPI](https://github.com/wagtail-nest/wagtail-bakery/actions/workflows/publish-test.yml) workflow.
+   1. Check the result on [TestPyPI: wagtail-bakery](https://test.pypi.org/project/wagtail-bakery/).
+1. Publish to PyPI:
+   1. Create and push a tag following [PEP 440 – Version Identification Specification](https://peps.python.org/pep-0440/) (for example `1.1.3` or `1.1.3rc1`), except for the `.devN` suffix used for testing (see _Publish to TestPyPI_ step above)
+   1. Follow the action progress for the [Publish to PyPI](https://github.com/wagtail-nest/wagtail-bakery/actions/workflows/publish.yml) workflow
+   1. Check the result on [PyPI: wagtail-bakery](https://pypi.org/project/wagtail-bakery/)
 1. On GitHub, create a release and a tag for the new version.
 
 ## Credits
 
 Thanks to [@mhnbcu](https://github.com/mhnbcu/wagtailbakery) for bringing this
 idea up initially, and [Django Bakery](https://github.com/datadesk/django-bakery)
 for providing the initial bakery package.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wagtail-bakery-0.7.0/setup.py` & `wagtail-bakery-0.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 install_requires = [
     'django-bakery~=0.13.1',
     'wagtail>=4.1',
 ]
 
 test_requires = [
-    'factory-boy<3',
+    'factory-boy',
     'flake8',
     'isort',
     'pytest',
     'pytest-cov',
     'pytest-django',
 ]
 
 setup(
     name='wagtail-bakery',
-    version='0.7.0',
+    version='0.8.0',
     description='A set of helpers for baking your Django Wagtail site out as flat files.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Rob Moorman and Wagtail Core Team',
     author_email='hello@wagtail.io',
     url="https://github.com/wagtail-nest/wagtail-bakery/",
     project_urls={
@@ -41,14 +41,15 @@
     license='MIT',
     classifiers=[
         'Environment :: Web Environment',
         'License :: OSI Approved :: MIT License',
         'Framework :: Django',
         'Framework :: Wagtail',
         'Framework :: Wagtail :: 4',
+        'Framework :: Wagtail :: 5',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
```

### Comparing `wagtail-bakery-0.7.0/src/wagtailbakery/api_views.py` & `wagtail-bakery-0.8.0/src/wagtailbakery/api_views.py`

 * *Files identical despite different names*

### Comparing `wagtail-bakery-0.7.0/src/wagtailbakery/models.py` & `wagtail-bakery-0.8.0/src/wagtailbakery/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-bakery-0.7.0/src/wagtailbakery/signal_handlers.py` & `wagtail-bakery-0.8.0/src/wagtailbakery/signal_handlers.py`

 * *Files identical despite different names*

### Comparing `wagtail-bakery-0.7.0/src/wagtailbakery/views.py` & `wagtail-bakery-0.8.0/src/wagtailbakery/views.py`

 * *Files identical despite different names*

