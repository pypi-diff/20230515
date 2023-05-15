# Comparing `tmp/invocations-3.2.0.tar.gz` & `tmp/invocations-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpgwujf__9/dist/invocations-3.2.0.tar", last modified: Thu May 11 20:06:37 2023, max compression
+gzip compressed data, was "/tmp/tmplklofhdu/dist/invocations-3.3.0.tar", last modified: Mon May 15 21:53:08 2023, max compression
```

## Comparing `invocations-3.2.0.tar` & `invocations-3.3.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)     2091 2022-12-31 22:11:11.000000 invocations-3.2.0/docs/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)      189 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    13035 2023-05-11 20:06:36.000000 invocations-3.2.0/docs/changelog.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/autodoc.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/console.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      233 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/packaging.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       53 2022-03-18 00:56:41.000000 invocations-3.2.0/docs/api/ci.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/docs.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/environment.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       69 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/pytest.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2737 2023-04-28 15:16:14.000000 invocations-3.2.0/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-11 20:06:37.000000 invocations-3.2.0/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     2335 2021-12-23 21:30:39.000000 invocations-3.2.0/README.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-11 20:06:37.000000 invocations-3.2.0/setup.cfg
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations/
--rw-r--r--   0 jforcier  (1000) users      (100)     2491 2023-05-11 19:03:55.000000 invocations-3.2.0/invocations/checks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5009 2022-12-17 18:26:26.000000 invocations-3.2.0/invocations/pytest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1264 2021-12-23 21:30:39.000000 invocations-3.2.0/invocations/watch.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3866 2022-12-31 22:11:11.000000 invocations-3.2.0/invocations/ci.py
--rw-r--r--   0 jforcier  (1000) users      (100)      636 2022-06-17 16:03:46.000000 invocations-3.2.0/invocations/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6534 2023-04-12 22:47:06.000000 invocations-3.2.0/invocations/docs.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations/packaging/
--rw-r--r--   0 jforcier  (1000) users      (100)      296 2021-12-23 21:30:39.000000 invocations-3.2.0/invocations/packaging/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1069 2023-01-16 22:33:01.000000 invocations-3.2.0/invocations/packaging/semantic_version_monkey.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4399 2022-12-31 22:11:11.000000 invocations-3.2.0/invocations/packaging/vendorize.py
--rw-r--r--   0 jforcier  (1000) users      (100)    34493 2023-05-02 21:11:34.000000 invocations-3.2.0/invocations/packaging/release.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1942 2023-01-16 22:33:01.000000 invocations-3.2.0/invocations/console.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3194 2022-12-31 22:11:11.000000 invocations-3.2.0/invocations/autodoc.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-11 19:04:03.000000 invocations-3.2.0/invocations/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)      621 2022-09-08 19:21:52.000000 invocations-3.2.0/invocations/environment.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.2.0/invocations/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5910 2023-01-16 22:33:01.000000 invocations-3.2.0/invocations/testing.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-03-17 18:07:11.000000 invocations-3.2.0/LICENSE
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)       12 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     3271 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)      124 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/dependency_links.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/packaging/
--rw-r--r--   0 jforcier  (1000) users      (100)    50230 2023-05-02 21:11:45.000000 invocations-3.2.0/tests/packaging/release.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/packaging/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)      185 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/unreleased_1.x_features.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      261 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/no_unreleased_1.1_bugs.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      179 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/no_unreleased_1.x_features.rst
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/unreleased_1.1_bugs.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/
--rw-r--r--   0 jforcier  (1000) users      (100)       13 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/noversion.py
--rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/otherversion.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1890 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/console.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3873 2023-05-11 20:04:44.000000 invocations-3.2.0/tests/checks.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)      425 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/mytasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)      259 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/autodoc/_support/conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/docs/api.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/docs/index.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/
--rw-r--r--   0 jforcier  (1000) users      (100)     4418 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 jforcier  (1000) users      (100)      286 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/file.png
--rw-r--r--   0 jforcier  (1000) users      (100)     4758 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/language_data.js
--rw-r--r--   0 jforcier  (1000) users      (100)    18215 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/searchtools.js
--rw-r--r--   0 jforcier  (1000) users      (100)    89501 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/jquery.js
--rw-r--r--   0 jforcier  (1000) users      (100)    11230 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/alabaster.css
--rw-r--r--   0 jforcier  (1000) users      (100)    68420 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
--rw-r--r--   0 jforcier  (1000) users      (100)    19530 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/underscore.js
--rw-r--r--   0 jforcier  (1000) users      (100)     4712 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
--rw-r--r--   0 jforcier  (1000) users      (100)   288580 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js
--rw-r--r--   0 jforcier  (1000) users      (100)      415 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/documentation_options.js
--rw-r--r--   0 jforcier  (1000) users      (100)     5327 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/pygments.css
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/plus.png
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/minus.png
--rw-r--r--   0 jforcier  (1000) users      (100)     4472 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/doctools.js
--rw-r--r--   0 jforcier  (1000) users      (100)       42 2022-09-08 21:39:12.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/custom.css
--rw-r--r--   0 jforcier  (1000) users      (100)    14621 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/basic.css
--rw-r--r--   0 jforcier  (1000) users      (100)     3958 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/genindex.html
--rw-r--r--   0 jforcier  (1000) users      (100)     5187 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/api.html
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/
--rw-r--r--   0 jforcier  (1000) users      (100)     7645 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)     2657 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    14029 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_sources/
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_sources/api.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_sources/index.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     1375 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/searchindex.js
--rw-r--r--   0 jforcier  (1000) users      (100)     2861 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/search.html
--rw-r--r--   0 jforcier  (1000) users      (100)      230 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.buildinfo
--rw-r--r--   0 jforcier  (1000) users      (100)     3553 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/index.html
--rw-r--r--   0 jforcier  (1000) users      (100)      296 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/objects.inv
--rw-r--r--   0 jforcier  (1000) users      (100)     3108 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/py-modindex.html
--rw-r--r--   0 jforcier  (1000) users      (100)     2752 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/autodoc/base.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1116 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/environment.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1066 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2542 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/pytest_.py
--rw-r--r--   0 jforcier  (1000) users      (100)      295 2023-04-28 19:13:24.000000 invocations-3.2.0/dev-requirements.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      243 2022-03-18 00:56:41.000000 invocations-3.2.0/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/
+-rw-r--r--   0 jforcier  (1000) users      (100)      311 2023-05-15 21:31:04.000000 invocations-3.3.0/dev-requirements.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1890 2022-12-31 22:11:11.000000 invocations-3.3.0/tests/console.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/autodoc/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/autodoc/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)      425 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/autodoc/_support/mytasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      259 2022-12-31 22:11:11.000000 invocations-3.3.0/tests/autodoc/_support/conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/autodoc/_support/docs/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/
+-rw-r--r--   0 jforcier  (1000) users      (100)     5187 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/api.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     1375 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/searchindex.js
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/.doctrees/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2657 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)     7645 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    14029 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle
+-rw-r--r--   0 jforcier  (1000) users      (100)     3108 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/py-modindex.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     3958 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/genindex.html
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_sources/
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_sources/api.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_sources/index.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     2861 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/search.html
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)    68420 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
+-rw-r--r--   0 jforcier  (1000) users      (100)   288580 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    89501 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/jquery.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     4712 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
+-rw-r--r--   0 jforcier  (1000) users      (100)      286 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/file.png
+-rw-r--r--   0 jforcier  (1000) users      (100)     4418 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 jforcier  (1000) users      (100)       42 2022-09-08 21:39:12.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/custom.css
+-rw-r--r--   0 jforcier  (1000) users      (100)     4758 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/language_data.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     5327 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/pygments.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    18215 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/searchtools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    19530 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/underscore.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    11230 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/alabaster.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    14621 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/basic.css
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/plus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)      415 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/documentation_options.js
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/minus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)     4472 2022-12-22 02:25:27.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/doctools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     3553 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/index.html
+-rw-r--r--   0 jforcier  (1000) users      (100)      296 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/objects.inv
+-rw-r--r--   0 jforcier  (1000) users      (100)      230 2022-12-22 02:27:13.000000 invocations-3.3.0/tests/autodoc/_support/docs/_build/.buildinfo
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/autodoc/_support/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/autodoc/_support/docs/api.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2752 2022-12-31 22:11:11.000000 invocations-3.3.0/tests/autodoc/base.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3637 2023-05-15 21:50:31.000000 invocations-3.3.0/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2542 2022-12-31 22:11:11.000000 invocations-3.3.0/tests/pytest_.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/packaging/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/packaging/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)      179 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/no_unreleased_1.x_features.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      185 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/unreleased_1.x_features.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/unreleased_1.1_bugs.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/tests/packaging/_support/fakepackage/
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/fakepackage/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/fakepackage/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/fakepackage/otherversion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       13 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/fakepackage/noversion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      261 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/no_unreleased_1.1_bugs.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.3.0/tests/packaging/_support/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    49393 2023-05-15 21:50:31.000000 invocations-3.3.0/tests/packaging/release.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1116 2022-12-31 22:11:11.000000 invocations-3.3.0/tests/environment.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3873 2023-05-11 20:04:44.000000 invocations-3.3.0/tests/checks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-15 21:53:08.000000 invocations-3.3.0/setup.cfg
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)    13313 2023-05-15 21:50:31.000000 invocations-3.3.0/docs/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2091 2022-12-31 22:11:11.000000 invocations-3.3.0/docs/conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)       53 2022-03-18 00:56:41.000000 invocations-3.3.0/docs/api/ci.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2021-12-23 21:30:39.000000 invocations-3.3.0/docs/api/environment.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-12-23 21:30:39.000000 invocations-3.3.0/docs/api/docs.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.3.0/docs/api/autodoc.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       69 2021-12-23 21:30:39.000000 invocations-3.3.0/docs/api/pytest.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.3.0/docs/api/console.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      233 2021-12-23 21:30:39.000000 invocations-3.3.0/docs/api/packaging.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      189 2021-12-23 21:30:39.000000 invocations-3.3.0/docs/index.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/invocations/
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.3.0/invocations/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5009 2022-12-17 18:26:26.000000 invocations-3.3.0/invocations/pytest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1942 2023-01-16 22:33:01.000000 invocations-3.3.0/invocations/console.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2491 2023-05-11 19:03:55.000000 invocations-3.3.0/invocations/checks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-15 21:50:31.000000 invocations-3.3.0/invocations/_version.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/invocations/packaging/
+-rw-r--r--   0 jforcier  (1000) users      (100)    35312 2023-05-15 21:48:34.000000 invocations-3.3.0/invocations/packaging/release.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1069 2023-01-16 22:33:01.000000 invocations-3.3.0/invocations/packaging/semantic_version_monkey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4399 2022-12-31 22:11:11.000000 invocations-3.3.0/invocations/packaging/vendorize.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      296 2021-12-23 21:30:39.000000 invocations-3.3.0/invocations/packaging/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5910 2023-01-16 22:33:01.000000 invocations-3.3.0/invocations/testing.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6534 2023-04-12 22:47:06.000000 invocations-3.3.0/invocations/docs.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1264 2021-12-23 21:30:39.000000 invocations-3.3.0/invocations/watch.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      621 2022-09-08 19:21:52.000000 invocations-3.3.0/invocations/environment.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      636 2022-06-17 16:03:46.000000 invocations-3.3.0/invocations/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3866 2022-12-31 22:11:11.000000 invocations-3.3.0/invocations/ci.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3194 2022-12-31 22:11:11.000000 invocations-3.3.0/invocations/autodoc.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 21:53:08.000000 invocations-3.3.0/invocations.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-15 21:53:08.000000 invocations-3.3.0/invocations.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      124 2023-05-15 21:53:08.000000 invocations-3.3.0/invocations.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       12 2023-05-15 21:53:08.000000 invocations-3.3.0/invocations.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-15 21:53:08.000000 invocations-3.3.0/invocations.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)     3271 2023-05-15 21:53:08.000000 invocations-3.3.0/invocations.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      243 2022-03-18 00:56:41.000000 invocations-3.3.0/MANIFEST.in
+-rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-15 21:53:08.000000 invocations-3.3.0/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)     2335 2021-12-23 21:30:39.000000 invocations-3.3.0/README.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2737 2023-04-28 15:16:14.000000 invocations-3.3.0/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-03-17 18:07:11.000000 invocations-3.3.0/LICENSE
```

### Comparing `invocations-3.2.0/docs/conf.py` & `invocations-3.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/docs/changelog.rst` & `invocations-3.3.0/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+- :release:`3.3.0 <2023-05-12>`
+- :feature:`-` Add mypy type-checking variant of the recently added import
+  test, in ``packaging.release.test_install``. This helps prove packages
+  exposing ``py.typed`` in their source tree are including it in their
+  distributions correctly.
 - :release:`3.2.0 <2023-05-11>`
 - :feature:`-` Minor enhancements to the ``checks`` module:
 
     - ``blacken`` now has a ``format`` alias (and will likely reverse the real
       name and the alias in 4.0)
     - Added ``lint`` task which currently just runs ``flake8``, will likely
       learn how to be configurable later.
```

### Comparing `invocations-3.2.0/setup.py` & `invocations-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/PKG-INFO` & `invocations-3.3.0/invocations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invocations
-Version: 3.2.0
+Version: 3.3.0
 Summary: Common/best-practice Invoke tasks and collections
 Home-page: https://invocations.readthedocs.io
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/pyinvoke/invocations
 Project-URL: Changelog, https://invocations.readthedocs.io/en/latest/changelog.html
```

### Comparing `invocations-3.2.0/README.rst` & `invocations-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/checks.py` & `invocations-3.3.0/invocations/checks.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/pytest.py` & `invocations-3.3.0/invocations/pytest.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/watch.py` & `invocations-3.3.0/invocations/watch.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/ci.py` & `invocations-3.3.0/invocations/ci.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/util.py` & `invocations-3.3.0/invocations/util.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/docs.py` & `invocations-3.3.0/invocations/docs.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/packaging/semantic_version_monkey.py` & `invocations-3.3.0/invocations/packaging/semantic_version_monkey.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/packaging/vendorize.py` & `invocations-3.3.0/invocations/packaging/vendorize.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/packaging/release.py` & `invocations-3.3.0/invocations/packaging/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,15 +778,17 @@
 
     Directory should either be a ``dist`` directory itself, or the parent of
     one.
 
     Uses the `venv` module to build temporary virtualenvs.
 
     :param bool verbose: Whether to print subprocess output.
-    :param bool skip_import: If True, don't try importing the installed module.
+    :param bool skip_import:
+        If True, don't try importing the installed module or checking it for
+        type hints.
     """
     # TODO: wants contextmanager or similar for only altering a setting within
     # a given scope or block - this may pollute subsequent subroutine calls
     if verbose:
         old_hide = c.config.run.hide
         c.config.run.hide = False
 
@@ -811,15 +813,28 @@
                 )
             )
             # Can we actually import it? (Will catch certain classes of
             # import-time-but-not-install-time explosions, eg busted dependency
             # specifications or imports).
             if not skip_import:
                 package = _find_package(c)
+                # Import, generally
                 c.run(f"{envbin / 'python'} -c 'import {package}'")
+                # Import, typecheck version (ie dependent package typechecking
+                # both itself and us). Assumes task is run from project root.
+                pytyped = Path(package) / "py.typed"
+                if pytyped.exists():
+                    # TODO: pin a specific mypy version?
+                    c.run(f"{envbin / 'pip'} install mypy")
+                    # Use some other dir (our cwd is probably the project root,
+                    # whose local $package dir may confuse mypy into a false
+                    # positive!)
+                    with tmpdir() as tmp2:
+                        mypy_check = f"{envbin / 'mypy'} -c 'import {package}'"
+                        c.run(f"cd {tmp2} && {mypy_check}")
 
     if verbose:
         c.config.run.hide = old_hide
 
 
 def get_archives(directory):
     # Obtain list of archive filenames, then ensure any wheels come first
```

### Comparing `invocations-3.2.0/invocations/console.py` & `invocations-3.3.0/invocations/console.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/autodoc.py` & `invocations-3.3.0/invocations/autodoc.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/environment.py` & `invocations-3.3.0/invocations/environment.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations/testing.py` & `invocations-3.3.0/invocations/testing.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/LICENSE` & `invocations-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations.egg-info/SOURCES.txt` & `invocations-3.3.0/invocations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/invocations.egg-info/PKG-INFO` & `invocations-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invocations
-Version: 3.2.0
+Version: 3.3.0
 Summary: Common/best-practice Invoke tasks and collections
 Home-page: https://invocations.readthedocs.io
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/pyinvoke/invocations
 Project-URL: Changelog, https://invocations.readthedocs.io/en/latest/changelog.html
```

### Comparing `invocations-3.2.0/tests/packaging/release.py` & `invocations-3.3.0/tests/packaging/release.py`

 * *Files 3% similar despite different names*

```diff
@@ -1198,78 +1198,62 @@
         def passed_to_upload(self, fakepub):
             c, mocks = fakepub
             publish(c, dry_run=True)
             assert mocks.upload.call_args[1]["dry_run"] is True
 
 
 class test_install_:
-    @patch("invocations.packaging.release.pip_version", "lmao")
-    @patch("invocations.packaging.release.get_archives")
-    @patch("invocations.util.mkdtemp")
-    @patch("invocations.util.rmtree", Mock("rmtree"))  # Just a neuter
-    @patch("venv.EnvBuilder")
-    @patch("invocations.packaging.release._find_package", lambda c: "foo")
-    def installs_all_archives_in_fresh_venv_with_matching_pip(
-        self, builder, mkdtemp, get_archives
-    ):
-        # Setup & run
-        c = MockContext(run=True, repeat=True)
-        mkdtemp.return_value = "tmpdir"
-        get_archives.return_value = ["foo.tgz", "foo.whl"]
+    def installs_all_archives_in_fresh_venv_with_matching_pip(self, install):
+        c = install
+        # Basic test, uses guts of fixture
         install_test_task(c, directory="whatever")
-        # Create factory
-        builder.assert_called_once_with(with_pip=True)
-        # Used helper to get artifacts
-        get_archives.assert_called_once_with("whatever")
-        # venv factory ran twice in some temp dir
-        builder.return_value.create.assert_has_calls(
-            [call("tmpdir"), call("tmpdir")]
-        )
-        pip_base = "tmpdir/bin/pip install --disable-pip-version-check"
-        c.run.assert_has_calls(
-            [
-                # Pip installed to same version as running interpreter's pip
-                call("tmpdir/bin/pip install pip==lmao"),
-                # Archives installed into venv
-                call("{} foo.tgz".format(pip_base)),
-                # Import attempt was made
-                call("tmpdir/bin/python -c 'import foo'"),
-                # And repeat
-                call("tmpdir/bin/pip install pip==lmao"),
-                call("{} foo.whl".format(pip_base)),
-                call("tmpdir/bin/python -c 'import foo'"),
-            ]
-        )
-
-    @patch("invocations.packaging.release.pip_version", "lmao")
-    @patch("invocations.packaging.release.get_archives")
-    @patch("invocations.util.mkdtemp")
-    @patch("invocations.util.rmtree", Mock("rmtree"))  # Just a neuter
-    @patch("invocations.packaging.release._find_package", lambda c: "foo")
-    def skips_import_test_when_asked_to(self, mkdtemp, get_archives):
-        # Setup & run
-        c = MockContext(run=True, repeat=True)
-        mkdtemp.return_value = "tmpdir"
-        get_archives.return_value = ["foo.tgz", "foo.whl"]
+        # Import attempt was made
+        c.run.assert_any_call("tmpdir/bin/python -c 'import foo'")
+
+    def skips_import_test_when_asked_to(self, install):
+        c = install
+        install_test_task(c, directory="whatever", skip_import=True)
+        # No import attempt
+        for unwanted in (call("tmpdir/bin/python -c 'import foo'"),):
+            assert unwanted not in c.run.mock_calls
+
+    def does_mypy_import_when_py_typed_present(self, install):
+        c = install
+        # Mock out the pathlib exists call as positive (default is negative)
+        c.set_exists(True)
+        install_test_task(c, directory="whatever")
+        # Mypy installed and executed
+        c.run.assert_any_call("tmpdir/bin/pip install mypy")
+        # NOTE: not actually the same 2 tmpdirs here but I'm already so sick of
+        # all these mocks, jeez
+        c.run.assert_any_call("cd tmpdir && tmpdir/bin/mypy -c 'import foo'")
+
+    def skips_mypy_import_when_no_py_typed(self, install):
+        c = install
+        # Mock out the pathlib exists call as explicitly false, why not
+        c.set_exists(False)
+        install_test_task(c, directory="whatever")
+        # Mypy NOT installed or executed
+        for unwanted in (
+            call("tmpdir/bin/pip install mypy"),
+            call("cd tmpdir && tmpdir/bin/mypy -c 'import foo'"),
+        ):
+            assert unwanted not in c.run.mock_calls
+
+    def skips_mypy_import_when_skipping_regular_import(self, install):
+        c = install
+        c.set_exists(True)
         install_test_task(c, directory="whatever", skip_import=True)
-        pip_base = "tmpdir/bin/pip install --disable-pip-version-check"
-        c.run.assert_has_calls(
-            [
-                # Pip installed to same version as running interpreter's pip
-                call("tmpdir/bin/pip install pip==lmao"),
-                # Archives installed into venv
-                call("{} foo.tgz".format(pip_base)),
-                # And repeat
-                call("tmpdir/bin/pip install pip==lmao"),
-                call("{} foo.whl".format(pip_base)),
-            ]
-        )
-        assert (
-            call("tmpdir/bin/python -c 'import foo'") not in c.run.mock_calls
-        )
+        # Mypy NOT installed or executed
+        for unwanted in (
+            call("tmpdir/bin/python -c 'import foo'"),
+            call("tmpdir/bin/pip install mypy"),
+            call("cd tmpdir && tmpdir/bin/mypy -c 'import foo'"),
+        ):
+            assert unwanted not in c.run.mock_calls
 
 
 class push_:
     def pushes_with_follow_tags(self):
         "git-pushes with --follow-tags"
         c = MockContext(run=True)
         push(c)
```

### Comparing `invocations-3.2.0/tests/console.py` & `invocations-3.3.0/tests/console.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/checks.py` & `invocations-3.3.0/tests/checks.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/language_data.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/searchtools.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/jquery.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/alabaster.css` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/underscore.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/pygments.css` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/doctools.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/basic.css` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/genindex.html` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/genindex.html`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/api.html` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/api.html`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/searchindex.js` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/searchindex.js`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/search.html` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/search.html`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/index.html` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/index.html`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/_support/docs/_build/py-modindex.html` & `invocations-3.3.0/tests/autodoc/_support/docs/_build/py-modindex.html`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/autodoc/base.py` & `invocations-3.3.0/tests/autodoc/base.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/environment.py` & `invocations-3.3.0/tests/environment.py`

 * *Files identical despite different names*

### Comparing `invocations-3.2.0/tests/pytest_.py` & `invocations-3.3.0/tests/pytest_.py`

 * *Files identical despite different names*

