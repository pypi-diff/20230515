# Comparing `tmp/plone.app.caching-3.1.0.tar.gz` & `tmp/plone.app.caching-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.caching-3.1.0.tar", last modified: Wed Apr 26 21:46:53 2023, max compression
+gzip compressed data, was "plone.app.caching-3.1.1.tar", last modified: Mon May 15 06:53:09 2023, max compression
```

## Comparing `plone.app.caching-3.1.0.tar` & `plone.app.caching-3.1.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.923525 plone.app.caching-3.1.0/
--rw-r--r--   0 maurits    (501) staff       (20)    15150 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/CHANGES.md
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    19213 2023-04-26 21:46:53.923672 plone.app.caching-3.1.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3056 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.903506 plone.app.caching-3.1.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      674 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      308 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/docs/changelog_template.jinja
--rw-r--r--   0 maurits    (501) staff       (20)      230 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/lint-requirements.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.903795 plone.app.caching-3.1.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.906554 plone.app.caching-3.1.0/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.909945 plone.app.caching-3.1.0/plone/app/caching/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.913079 plone.app.caching-3.1.0/plone/app/caching/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    41005 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)    21546 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)      656 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/edit.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9575 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     5523 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/import.pt
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/plone.app.caching.gif
--rw-r--r--   0 maurits    (501) staff       (20)     6307 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/purge.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4622 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/browser/ramcache.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4468 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/caching.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3021 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3867 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/lastmodified.py
--rw-r--r--   0 maurits    (501) staff       (20)     3985 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/lookup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.914815 plone.app.caching-3.1.0/plone/app/caching/operations/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2783 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    13297 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/default.py
--rw-r--r--   0 maurits    (501) staff       (20)     7731 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/etags.py
--rw-r--r--   0 maurits    (501) staff       (20)     1725 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/ramcache.py
--rw-r--r--   0 maurits    (501) staff       (20)    24136 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/operations/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.899882 plone.app.caching-3.1.0/plone/app/caching/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.915773 plone.app.caching-3.1.0/plone/app/caching/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      594 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       13 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/plone.app.caching.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.917553 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/
--rw-r--r--   0 maurits    (501) staff       (20)     1934 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/basesettings.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2318 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/generic.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2137 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/moderate.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2486 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/strong.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/terse.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1792 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/weak.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.899559 plone.app.caching-3.1.0/plone/app/caching/profiles/v2/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.917846 plone.app.caching-3.1.0/plone/app/caching/profiles/v2/registry/
--rw-r--r--   0 maurits    (501) staff       (20)     2414 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/v2/registry/terse.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.918139 plone.app.caching-3.1.0/plone/app/caching/profiles/with-caching-proxy/
--rw-r--r--   0 maurits    (501) staff       (20)     4971 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/with-caching-proxy/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.918432 plone.app.caching-3.1.0/plone/app/caching/profiles/without-caching-proxy/
--rw-r--r--   0 maurits    (501) staff       (20)     4581 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles/without-caching-proxy/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1504 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     8396 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/purge.py
--rw-r--r--   0 maurits    (501) staff       (20)     1038 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2171 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.922695 plone.app.caching-3.1.0/plone/app/caching/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      668 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.923285 plone.app.caching-3.1.0/plone/app/caching/tests/data/
--rw-r--r--   0 maurits    (501) staff       (20)     9819 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/data/plone-app-caching.jpg
--rw-r--r--   0 maurits    (501) staff       (20)      189 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/data/testfile.csv
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test.css
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test.gif
--rw-r--r--   0 maurits    (501) staff       (20)    11871 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_etags.py
--rw-r--r--   0 maurits    (501) staff       (20)     9866 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_integration.py
--rw-r--r--   0 maurits    (501) staff       (20)     7101 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_lastmodified.py
--rw-r--r--   0 maurits    (501) staff       (20)    10537 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_lookup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2992 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_default.py
--rw-r--r--   0 maurits    (501) staff       (20)     6912 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_parameters.py
--rw-r--r--   0 maurits    (501) staff       (20)    55900 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    25538 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_profile_with_caching_proxy.py
--rw-r--r--   0 maurits    (501) staff       (20)    22468 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_profile_without_caching_proxy.py
--rw-r--r--   0 maurits    (501) staff       (20)    13490 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_purge.py
--rw-r--r--   0 maurits    (501) staff       (20)     5674 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2123 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone/app/caching/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:46:53.906258 plone.app.caching-3.1.0/plone.app.caching.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    19213 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2887 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      695 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/plone.app.caching.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1136 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       13 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)      326 2023-04-26 21:46:53.924218 plone.app.caching-3.1.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2775 2023-04-26 21:46:53.000000 plone.app.caching-3.1.0/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.701716 plone.app.caching-3.1.1/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15406 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/CHANGES.md
+-rw-r--r--   0 gil       (1000) gil       (1000)      162 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    19469 2023-05-15 06:53:09.701716 plone.app.caching-3.1.1/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     3056 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/README.md
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.694715 plone.app.caching-3.1.1/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      674 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/docs/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      308 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/docs/changelog_template.jinja
+-rw-r--r--   0 gil       (1000) gil       (1000)      230 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/lint-requirements.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.694715 plone.app.caching-3.1.1/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.695716 plone.app.caching-3.1.1/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.696715 plone.app.caching-3.1.1/plone/app/caching/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.697715 plone.app.caching-3.1.1/plone/app/caching/browser/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1119 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)    41005 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/controlpanel.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)    21546 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/controlpanel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      656 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/edit.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     9575 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/edit.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5523 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/import.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      155 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/plone.app.caching.gif
+-rw-r--r--   0 gil       (1000) gil       (1000)     6307 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/purge.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     4622 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/browser/ramcache.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     4468 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/caching.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1751 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     3021 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3867 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/lastmodified.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3985 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/lookup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.698716 plone.app.caching-3.1.1/plone/app/caching/operations/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/operations/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2783 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/operations/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)    13297 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/operations/default.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7731 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/operations/etags.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1725 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/operations/ramcache.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    24136 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/operations/utils.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.692716 plone.app.caching-3.1.1/plone/app/caching/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.698716 plone.app.caching-3.1.1/plone/app/caching/profiles/default/
+-rw-r--r--   0 gil       (1000) gil       (1000)      594 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/default/controlpanel.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      184 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/default/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)       13 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/default/plone.app.caching.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.699715 plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1934 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/basesettings.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2318 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/generic.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2137 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/moderate.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2486 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/strong.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2414 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/terse.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1792 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/weak.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.692716 plone.app.caching-3.1.1/plone/app/caching/profiles/v2/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.699715 plone.app.caching-3.1.1/plone/app/caching/profiles/v2/registry/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2414 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/v2/registry/terse.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.699715 plone.app.caching-3.1.1/plone/app/caching/profiles/with-caching-proxy/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4971 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/with-caching-proxy/registry.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.699715 plone.app.caching-3.1.1/plone/app/caching/profiles/without-caching-proxy/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4581 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles/without-caching-proxy/registry.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1504 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/profiles.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     8396 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/purge.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1038 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/setuphandlers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2171 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.701716 plone.app.caching-3.1.1/plone/app/caching/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)      668 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.701716 plone.app.caching-3.1.1/plone/app/caching/tests/data/
+-rw-r--r--   0 gil       (1000) gil       (1000)     9819 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/data/plone-app-caching.jpg
+-rw-r--r--   0 gil       (1000) gil       (1000)      189 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/data/testfile.csv
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test.css
+-rw-r--r--   0 gil       (1000) gil       (1000)      155 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test.gif
+-rw-r--r--   0 gil       (1000) gil       (1000)    11871 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_etags.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9866 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_integration.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7101 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_lastmodified.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    10537 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_lookup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2992 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_operation_default.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6912 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_operation_parameters.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    55900 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_operation_utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    25538 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_profile_with_caching_proxy.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    22468 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_profile_without_caching_proxy.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    13490 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_purge.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5674 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/tests/test_utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2123 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone/app/caching/utils.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 06:53:09.695716 plone.app.caching-3.1.1/plone.app.caching.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    19469 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone.app.caching.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     2887 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone.app.caching.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone.app.caching.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       40 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone.app.caching.egg-info/entry_points.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone.app.caching.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone.app.caching.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      695 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone.app.caching.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/plone.app.caching.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1136 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)       13 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/requirements.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      326 2023-05-15 06:53:09.702715 plone.app.caching-3.1.1/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     2775 2023-05-15 06:53:09.000000 plone.app.caching-3.1.1/setup.py
```

### Comparing `plone.app.caching-3.1.0/CHANGES.md` & `plone.app.caching-3.1.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,25 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 3.1.1 (2023-05-15)
+
+
+### Tests
+
+- Changed hardcoded test date to June instead of May to temporarily fix a testing error.
+  See `issue 127 <https://github.com/plone/plone.app.caching/issues/127>`_.
+  Needs a proper fix within a month.
+  [maurits] #127
+
+
 ## 3.1.0 (2023-04-26)
 
 
 ### New features:
 
 - Update the resourceRegistries ETag to use the config registry modification time.
   This time is set since Plone 6.0.4.
```

### Comparing `plone.app.caching-3.1.0/PKG-INFO` & `plone.app.caching-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.caching
-Version: 3.1.0
+Version: 3.1.1
 Summary: Plone UI and default rules for plone.caching/z3c.caching
 Home-page: https://github.com/plone/plone.app.caching
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable
@@ -108,14 +108,25 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 3.1.1 (2023-05-15)
+
+
+### Tests
+
+- Changed hardcoded test date to June instead of May to temporarily fix a testing error.
+  See `issue 127 <https://github.com/plone/plone.app.caching/issues/127>`_.
+  Needs a proper fix within a month.
+  [maurits] #127
+
+
 ## 3.1.0 (2023-04-26)
 
 
 ### New features:
 
 - Update the resourceRegistries ETag to use the config registry modification time.
   This time is set since Plone 6.0.4.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plone.app.caching Version: 3.1.0 Summary: Plone UI
+Metadata-Version: 2.1 Name: plone.app.caching Version: 3.1.1 Summary: Plone UI
 and default rules for plone.caching/z3c.caching Home-page: https://github.com/
 plone/plone.app.caching Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Plone Classifier: Framework ::
 Plone :: 6.0 Classifier: Framework :: Plone :: Core Classifier: Framework ::
 Zope :: 5 Classifier: License :: OSI Approved :: GNU General Public License v2
@@ -45,17 +45,21 @@
 Interface). 3. Go to ``portal_setup``, and then to the Import tab. 4. Select
 the HTTP caching support profile, perhaps easiest by id: `profile-
 plone.app.caching:default`. 5. Click 'Import all steps'. ## Source Code
 Contributors, please read the document [Process for Plone core's development]
 (https://5.docs.plone.org/develop/coredev/docs/index.html) Sources are at the
 [Plone code repository hosted at Github ](https://github.com/plone/
 plone.app.caching). ## This project is supported by [Plone_Logo] ## License The
-project is licensed under GPLv2. # Changelog   ## 3.1.0 (2023-04-26) ### New
-features: - Update the resourceRegistries ETag to use the config registry
-modification time. This time is set since Plone 6.0.4. Fixes `issue 93
+project is licensed under GPLv2. # Changelog   ## 3.1.1 (2023-05-15) ### Tests
+- Changed hardcoded test date to June instead of May to temporarily fix a
+testing error. See `issue 127
+github.com/plone/plone.app.caching/issues/127>`_. Needs a proper fix within a
+month. [maurits] #127 ## 3.1.0 (2023-04-26) ### New features: - Update the
+resourceRegistries ETag to use the config registry modification time. This time
+is set since Plone 6.0.4. Fixes `issue 93
 ` in controlpanel. [petschki] (#112) - Revert changes to tests to work with the
 Zope security fix. We must have an empty byte, not text, otherwise it is an
 indication that we get a possibly wrong Content-Type in a 304 status. See `Zope
 issue 1089
 github.com/zopefoundation/Zope/issues/1089>`_. [maurits] (#1089) ## 3.0.1
 (2022-12-21) ### Bug fixes: - Fix tests to work with the Zope security fix.
 [maurits] (#106) ## 3.0.0 (2022-11-14) ### Bug fixes: - Add missing quotation
```

### Comparing `plone.app.caching-3.1.0/README.md` & `plone.app.caching-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/docs/LICENSE.GPL` & `plone.app.caching-3.1.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/docs/LICENSE.txt` & `plone.app.caching-3.1.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/browser/configure.zcml` & `plone.app.caching-3.1.1/plone/app/caching/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/browser/controlpanel.pt` & `plone.app.caching-3.1.1/plone/app/caching/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/browser/controlpanel.py` & `plone.app.caching-3.1.1/plone/app/caching/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/browser/edit.pt` & `plone.app.caching-3.1.1/plone/app/caching/browser/edit.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/browser/edit.py` & `plone.app.caching-3.1.1/plone/app/caching/browser/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/browser/import.pt` & `plone.app.caching-3.1.1/plone/app/caching/browser/import.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/browser/purge.pt` & `plone.app.caching-3.1.1/plone/app/caching/browser/purge.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/browser/ramcache.pt` & `plone.app.caching-3.1.1/plone/app/caching/browser/ramcache.pt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/caching.zcml` & `plone.app.caching-3.1.1/plone/app/caching/caching.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/configure.zcml` & `plone.app.caching-3.1.1/plone/app/caching/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/interfaces.py` & `plone.app.caching-3.1.1/plone/app/caching/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/lastmodified.py` & `plone.app.caching-3.1.1/plone/app/caching/lastmodified.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/lookup.py` & `plone.app.caching-3.1.1/plone/app/caching/lookup.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/operations/configure.zcml` & `plone.app.caching-3.1.1/plone/app/caching/operations/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/operations/default.py` & `plone.app.caching-3.1.1/plone/app/caching/operations/default.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/operations/etags.py` & `plone.app.caching-3.1.1/plone/app/caching/operations/etags.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/operations/ramcache.py` & `plone.app.caching-3.1.1/plone/app/caching/operations/ramcache.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/operations/utils.py` & `plone.app.caching-3.1.1/plone/app/caching/operations/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/default/controlpanel.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/basesettings.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/basesettings.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/generic.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/generic.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/moderate.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/moderate.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/strong.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/strong.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/terse.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/terse.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/default/registry/weak.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/default/registry/weak.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/v2/registry/terse.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/v2/registry/terse.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/with-caching-proxy/registry.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/with-caching-proxy/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles/without-caching-proxy/registry.xml` & `plone.app.caching-3.1.1/plone/app/caching/profiles/without-caching-proxy/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/profiles.zcml` & `plone.app.caching-3.1.1/plone/app/caching/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/purge.py` & `plone.app.caching-3.1.1/plone/app/caching/purge.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/setuphandlers.py` & `plone.app.caching-3.1.1/plone/app/caching/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/testing.py` & `plone.app.caching-3.1.1/plone/app/caching/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/__init__.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/data/plone-app-caching.jpg` & `plone.app.caching-3.1.1/plone/app/caching/tests/data/plone-app-caching.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_etags.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_etags.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_integration.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_lastmodified.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_lastmodified.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_lookup.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_default.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_operation_default.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_parameters.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_operation_parameters.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_operation_utils.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_operation_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_profile_with_caching_proxy.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_profile_with_caching_proxy.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_profile_without_caching_proxy.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_profile_without_caching_proxy.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_purge.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_purge.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone/app/caching/tests/test_utils.py` & `plone.app.caching-3.1.1/plone/app/caching/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 TEST_TIMEZONE = "Europe/Vienna"
 TEST_IMAGE = pkg_resources.resource_filename("plone.app.caching.tests", "test.gif")
 
 
 def stable_now():
     """Patch localized_now to allow stable results in tests."""
     tzinfo = pytz.timezone(TEST_TIMEZONE)
-    now = datetime(2013, 5, 5, 10, 0, 0).replace(microsecond=0)
+    now = datetime(2013, 6, 5, 10, 0, 0).replace(microsecond=0)
     now = tzinfo.localize(now)  # set tzinfo with correct DST offset
     return now
 
 
 def normalize_etag(value):
     split_value = value.split("|")
     # The last component is expected to be the resourceRegistries ETag,
```

### Comparing `plone.app.caching-3.1.0/plone/app/caching/utils.py` & `plone.app.caching-3.1.1/plone/app/caching/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone.app.caching.egg-info/PKG-INFO` & `plone.app.caching-3.1.1/plone.app.caching.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.caching
-Version: 3.1.0
+Version: 3.1.1
 Summary: Plone UI and default rules for plone.caching/z3c.caching
 Home-page: https://github.com/plone/plone.app.caching
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable
@@ -108,14 +108,25 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 3.1.1 (2023-05-15)
+
+
+### Tests
+
+- Changed hardcoded test date to June instead of May to temporarily fix a testing error.
+  See `issue 127 <https://github.com/plone/plone.app.caching/issues/127>`_.
+  Needs a proper fix within a month.
+  [maurits] #127
+
+
 ## 3.1.0 (2023-04-26)
 
 
 ### New features:
 
 - Update the resourceRegistries ETag to use the config registry modification time.
   This time is set since Plone 6.0.4.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plone.app.caching Version: 3.1.0 Summary: Plone UI
+Metadata-Version: 2.1 Name: plone.app.caching Version: 3.1.1 Summary: Plone UI
 and default rules for plone.caching/z3c.caching Home-page: https://github.com/
 plone/plone.app.caching Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: plone caching
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Plone Classifier: Framework ::
 Plone :: 6.0 Classifier: Framework :: Plone :: Core Classifier: Framework ::
 Zope :: 5 Classifier: License :: OSI Approved :: GNU General Public License v2
@@ -45,17 +45,21 @@
 Interface). 3. Go to ``portal_setup``, and then to the Import tab. 4. Select
 the HTTP caching support profile, perhaps easiest by id: `profile-
 plone.app.caching:default`. 5. Click 'Import all steps'. ## Source Code
 Contributors, please read the document [Process for Plone core's development]
 (https://5.docs.plone.org/develop/coredev/docs/index.html) Sources are at the
 [Plone code repository hosted at Github ](https://github.com/plone/
 plone.app.caching). ## This project is supported by [Plone_Logo] ## License The
-project is licensed under GPLv2. # Changelog   ## 3.1.0 (2023-04-26) ### New
-features: - Update the resourceRegistries ETag to use the config registry
-modification time. This time is set since Plone 6.0.4. Fixes `issue 93
+project is licensed under GPLv2. # Changelog   ## 3.1.1 (2023-05-15) ### Tests
+- Changed hardcoded test date to June instead of May to temporarily fix a
+testing error. See `issue 127
+github.com/plone/plone.app.caching/issues/127>`_. Needs a proper fix within a
+month. [maurits] #127 ## 3.1.0 (2023-04-26) ### New features: - Update the
+resourceRegistries ETag to use the config registry modification time. This time
+is set since Plone 6.0.4. Fixes `issue 93
 ` in controlpanel. [petschki] (#112) - Revert changes to tests to work with the
 Zope security fix. We must have an empty byte, not text, otherwise it is an
 indication that we get a possibly wrong Content-Type in a 304 status. See `Zope
 issue 1089
 github.com/zopefoundation/Zope/issues/1089>`_. [maurits] (#1089) ## 3.0.1
 (2022-12-21) ### Bug fixes: - Fix tests to work with the Zope security fix.
 [maurits] (#106) ## 3.0.0 (2022-11-14) ### Bug fixes: - Add missing quotation
```

### Comparing `plone.app.caching-3.1.0/plone.app.caching.egg-info/SOURCES.txt` & `plone.app.caching-3.1.1/plone.app.caching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/plone.app.caching.egg-info/requires.txt` & `plone.app.caching-3.1.1/plone.app.caching.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/pyproject.toml` & `plone.app.caching-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.caching-3.1.0/setup.py` & `plone.app.caching-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.1.0"
+version = "3.1.1"
 
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
```

