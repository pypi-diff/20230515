# Comparing `tmp/wildcard.hps-1.4.1.tar.gz` & `tmp/wildcard.hps-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wildcard.hps-1.4.1.tar", last modified: Thu May 11 14:10:53 2023, max compression
+gzip compressed data, was "wildcard.hps-1.4.2.tar", last modified: Mon May 15 15:49:54 2023, max compression
```

## Comparing `wildcard.hps-1.4.1.tar` & `wildcard.hps-1.4.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.681055 wildcard.hps-1.4.1/
--rw-r--r--   0 joel       (501) staff       (20)     1196 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/CHANGES.md
--rw-r--r--   0 joel       (501) staff       (20)      521 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/DEVELOP.rst
--rw-r--r--   0 joel       (501) staff       (20)    17987 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/LICENSE.GPL
--rw-r--r--   0 joel       (501) staff       (20)      229 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/MANIFEST.in
--rw-r--r--   0 joel       (501) staff       (20)      330 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/Makefile
--rw-r--r--   0 joel       (501) staff       (20)     9255 2023-05-11 14:10:53.681127 wildcard.hps-1.4.1/PKG-INFO
--rw-r--r--   0 joel       (501) staff       (20)     6870 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/README.md
--rw-r--r--   0 joel       (501) staff       (20)       27 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/constraints.txt
--rw-r--r--   0 joel       (501) staff       (20)      105 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/constraints_plone50.txt
--rw-r--r--   0 joel       (501) staff       (20)      101 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/constraints_plone51.txt
--rw-r--r--   0 joel       (501) staff       (20)       50 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/requirements.txt
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.674718 wildcard.hps-1.4.1/scripts/
--rw-r--r--   0 joel       (501) staff       (20)     4362 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/scripts/populate.py
--rw-r--r--   0 joel       (501) staff       (20)      321 2023-05-11 14:10:53.681437 wildcard.hps-1.4.1/setup.cfg
--rw-r--r--   0 joel       (501) staff       (20)     2393 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/setup.py
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.672046 wildcard.hps-1.4.1/src/
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.674862 wildcard.hps-1.4.1/src/wildcard/
--rw-r--r--   0 joel       (501) staff       (20)       80 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/__init__.py
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.678293 wildcard.hps-1.4.1/src/wildcard/hps/
--rw-r--r--   0 joel       (501) staff       (20)      120 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/__init__.py
--rw-r--r--   0 joel       (501) staff       (20)      757 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/brain.py
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.679342 wildcard.hps-1.4.1/src/wildcard/hps/browser/
--rw-r--r--   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/browser/__init__.py
--rw-r--r--   0 joel       (501) staff       (20)     1334 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/browser/configure.zcml
--rw-r--r--   0 joel       (501) staff       (20)     2910 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/browser/controlpanel.py
--rw-r--r--   0 joel       (501) staff       (20)     2788 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/browser/controlpanel_layout.pt
--rw-r--r--   0 joel       (501) staff       (20)      217 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/browser/search.py
--rw-r--r--   0 joel       (501) staff       (20)     1282 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/browser/utilviews.py
--rw-r--r--   0 joel       (501) staff       (20)     3832 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/configure.zcml
--rw-r--r--   0 joel       (501) staff       (20)    11217 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/hook.py
--rw-r--r--   0 joel       (501) staff       (20)    12458 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/indexes.py
--rw-r--r--   0 joel       (501) staff       (20)      914 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/interfaces.py
--rw-r--r--   0 joel       (501) staff       (20)     2706 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/mapping.py
--rw-r--r--   0 joel       (501) staff       (20)    17669 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/opensearch.py
--rw-r--r--   0 joel       (501) staff       (20)     2531 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/patches.py
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.672415 wildcard.hps-1.4.1/src/wildcard/hps/profiles/
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.680065 wildcard.hps-1.4.1/src/wildcard/hps/profiles/default/
--rw-r--r--   0 joel       (501) staff       (20)      117 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/profiles/default/browserlayer.xml
--rw-r--r--   0 joel       (501) staff       (20)      422 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/profiles/default/controlpanel.xml
--rw-r--r--   0 joel       (501) staff       (20)       78 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/profiles/default/metadata.xml
--rw-r--r--   0 joel       (501) staff       (20)      118 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/profiles/default/registry.xml
--rw-r--r--   0 joel       (501) staff       (20)     2712 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/query.py
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.680405 wildcard.hps-1.4.1/src/wildcard/hps/scripts/
--rw-r--r--   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/scripts/__init__.py
--rw-r--r--   0 joel       (501) staff       (20)     8595 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/scripts/reindex.py
--rw-r--r--   0 joel       (501) staff       (20)     5185 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/testing.py
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.680901 wildcard.hps-1.4.1/src/wildcard/hps/tests/
--rw-r--r--   0 joel       (501) staff       (20)     2082 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/tests/__init__.py
--rw-r--r--   0 joel       (501) staff       (20)     3575 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/tests/test_catalog.py
--rw-r--r--   0 joel       (501) staff       (20)     9166 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/tests/test_search.py
--rw-r--r--   0 joel       (501) staff       (20)     1989 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard/hps/utils.py
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-11 14:10:53.676400 wildcard.hps-1.4.1/src/wildcard.hps.egg-info/
--rw-r--r--   0 joel       (501) staff       (20)     9255 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard.hps.egg-info/PKG-INFO
--rw-r--r--   0 joel       (501) staff       (20)     1506 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard.hps.egg-info/SOURCES.txt
--rw-r--r--   0 joel       (501) staff       (20)        1 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard.hps.egg-info/dependency_links.txt
--rw-r--r--   0 joel       (501) staff       (20)      217 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard.hps.egg-info/entry_points.txt
--rw-r--r--   0 joel       (501) staff       (20)        9 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard.hps.egg-info/namespace_packages.txt
--rw-r--r--   0 joel       (501) staff       (20)        1 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard.hps.egg-info/not-zip-safe
--rw-r--r--   0 joel       (501) staff       (20)      169 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard.hps.egg-info/requires.txt
--rw-r--r--   0 joel       (501) staff       (20)        9 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/src/wildcard.hps.egg-info/top_level.txt
--rw-r--r--   0 joel       (501) staff       (20)     3488 2023-05-11 14:10:53.000000 wildcard.hps-1.4.1/tox.ini
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.377081 wildcard.hps-1.4.2/
+-rw-r--r--   0 joel       (501) staff       (20)     1348 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/CHANGES.md
+-rw-r--r--   0 joel       (501) staff       (20)      521 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/DEVELOP.rst
+-rw-r--r--   0 joel       (501) staff       (20)    17987 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/LICENSE.GPL
+-rw-r--r--   0 joel       (501) staff       (20)      229 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/MANIFEST.in
+-rw-r--r--   0 joel       (501) staff       (20)      330 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/Makefile
+-rw-r--r--   0 joel       (501) staff       (20)     9407 2023-05-15 15:49:54.377224 wildcard.hps-1.4.2/PKG-INFO
+-rw-r--r--   0 joel       (501) staff       (20)     6870 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/README.md
+-rw-r--r--   0 joel       (501) staff       (20)       27 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/constraints.txt
+-rw-r--r--   0 joel       (501) staff       (20)      105 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/constraints_plone50.txt
+-rw-r--r--   0 joel       (501) staff       (20)      101 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/constraints_plone51.txt
+-rw-r--r--   0 joel       (501) staff       (20)       50 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/requirements.txt
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.370235 wildcard.hps-1.4.2/scripts/
+-rw-r--r--   0 joel       (501) staff       (20)     4362 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/scripts/populate.py
+-rw-r--r--   0 joel       (501) staff       (20)      321 2023-05-15 15:49:54.377633 wildcard.hps-1.4.2/setup.cfg
+-rw-r--r--   0 joel       (501) staff       (20)     2393 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/setup.py
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.366226 wildcard.hps-1.4.2/src/
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.370386 wildcard.hps-1.4.2/src/wildcard/
+-rw-r--r--   0 joel       (501) staff       (20)       80 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/__init__.py
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.374317 wildcard.hps-1.4.2/src/wildcard/hps/
+-rw-r--r--   0 joel       (501) staff       (20)      120 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/__init__.py
+-rw-r--r--   0 joel       (501) staff       (20)      757 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/brain.py
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.375333 wildcard.hps-1.4.2/src/wildcard/hps/browser/
+-rw-r--r--   0 joel       (501) staff       (20)        0 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/browser/__init__.py
+-rw-r--r--   0 joel       (501) staff       (20)     1334 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/browser/configure.zcml
+-rw-r--r--   0 joel       (501) staff       (20)     2910 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/browser/controlpanel.py
+-rw-r--r--   0 joel       (501) staff       (20)     2788 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/browser/controlpanel_layout.pt
+-rw-r--r--   0 joel       (501) staff       (20)      217 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/browser/search.py
+-rw-r--r--   0 joel       (501) staff       (20)     1282 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/browser/utilviews.py
+-rw-r--r--   0 joel       (501) staff       (20)     3832 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/configure.zcml
+-rw-r--r--   0 joel       (501) staff       (20)    10990 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/hook.py
+-rw-r--r--   0 joel       (501) staff       (20)    12458 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/indexes.py
+-rw-r--r--   0 joel       (501) staff       (20)      914 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/interfaces.py
+-rw-r--r--   0 joel       (501) staff       (20)     2706 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/mapping.py
+-rw-r--r--   0 joel       (501) staff       (20)    17669 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/opensearch.py
+-rw-r--r--   0 joel       (501) staff       (20)     2531 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/patches.py
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.366691 wildcard.hps-1.4.2/src/wildcard/hps/profiles/
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.376032 wildcard.hps-1.4.2/src/wildcard/hps/profiles/default/
+-rw-r--r--   0 joel       (501) staff       (20)      117 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/profiles/default/browserlayer.xml
+-rw-r--r--   0 joel       (501) staff       (20)      422 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/profiles/default/controlpanel.xml
+-rw-r--r--   0 joel       (501) staff       (20)       78 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/profiles/default/metadata.xml
+-rw-r--r--   0 joel       (501) staff       (20)      118 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/profiles/default/registry.xml
+-rw-r--r--   0 joel       (501) staff       (20)     2712 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/query.py
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.376370 wildcard.hps-1.4.2/src/wildcard/hps/scripts/
+-rw-r--r--   0 joel       (501) staff       (20)        0 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/scripts/__init__.py
+-rw-r--r--   0 joel       (501) staff       (20)     8595 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/scripts/reindex.py
+-rw-r--r--   0 joel       (501) staff       (20)     5185 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/testing.py
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.376907 wildcard.hps-1.4.2/src/wildcard/hps/tests/
+-rw-r--r--   0 joel       (501) staff       (20)     2082 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/tests/__init__.py
+-rw-r--r--   0 joel       (501) staff       (20)     3575 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/tests/test_catalog.py
+-rw-r--r--   0 joel       (501) staff       (20)     9166 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/tests/test_search.py
+-rw-r--r--   0 joel       (501) staff       (20)     1989 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/src/wildcard/hps/utils.py
+drwxr-xr-x   0 joel       (501) staff       (20)        0 2023-05-15 15:49:54.371908 wildcard.hps-1.4.2/src/wildcard.hps.egg-info/
+-rw-r--r--   0 joel       (501) staff       (20)     9407 2023-05-15 15:49:54.000000 wildcard.hps-1.4.2/src/wildcard.hps.egg-info/PKG-INFO
+-rw-r--r--   0 joel       (501) staff       (20)     1506 2023-05-15 15:49:54.000000 wildcard.hps-1.4.2/src/wildcard.hps.egg-info/SOURCES.txt
+-rw-r--r--   0 joel       (501) staff       (20)        1 2023-05-15 15:49:54.000000 wildcard.hps-1.4.2/src/wildcard.hps.egg-info/dependency_links.txt
+-rw-r--r--   0 joel       (501) staff       (20)      217 2023-05-15 15:49:54.000000 wildcard.hps-1.4.2/src/wildcard.hps.egg-info/entry_points.txt
+-rw-r--r--   0 joel       (501) staff       (20)        9 2023-05-15 15:49:54.000000 wildcard.hps-1.4.2/src/wildcard.hps.egg-info/namespace_packages.txt
+-rw-r--r--   0 joel       (501) staff       (20)        1 2023-05-15 15:49:54.000000 wildcard.hps-1.4.2/src/wildcard.hps.egg-info/not-zip-safe
+-rw-r--r--   0 joel       (501) staff       (20)      169 2023-05-15 15:49:54.000000 wildcard.hps-1.4.2/src/wildcard.hps.egg-info/requires.txt
+-rw-r--r--   0 joel       (501) staff       (20)        9 2023-05-15 15:49:54.000000 wildcard.hps-1.4.2/src/wildcard.hps.egg-info/top_level.txt
+-rw-r--r--   0 joel       (501) staff       (20)     3488 2023-05-15 15:49:53.000000 wildcard.hps-1.4.2/tox.ini
```

### Comparing `wildcard.hps-1.4.1/CHANGES.md` & `wildcard.hps-1.4.2/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+1.4.2 (2023-05-15)
+------------------
+
+- abstract unicode handling code for hook when getting index data, and handle
+  tuples, lists, and dict values
+
+
 1.4.1 (2023-05-11)
 ------------------
 
 - handle unicode error and fix bug in hook when getting index data
 
 
 1.4.0 (2022-11-04)
```

### Comparing `wildcard.hps-1.4.1/DEVELOP.rst` & `wildcard.hps-1.4.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/LICENSE.GPL` & `wildcard.hps-1.4.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/PKG-INFO` & `wildcard.hps-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildcard.hps
-Version: 1.4.1
+Version: 1.4.2
 Summary: opensearch integration with CastleCMS and Plone
 Home-page: https://github.com/castlecms/wildcard.hps
 Author: Wildcard Corp.
 Author-email: corporate@wildcardcorp.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/wildcard.hps
 Project-URL: Source, https://github.com/castlecms/wildcard.hps
@@ -195,14 +195,21 @@
 $ ./bin/test
 ```
 
 
 Changelog
 =========
 
+1.4.2 (2023-05-15)
+------------------
+
+- abstract unicode handling code for hook when getting index data, and handle
+  tuples, lists, and dict values
+
+
 1.4.1 (2023-05-11)
 ------------------
 
 - handle unicode error and fix bug in hook when getting index data
 
 
 1.4.0 (2022-11-04)
```

### Comparing `wildcard.hps-1.4.1/README.md` & `wildcard.hps-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/scripts/populate.py` & `wildcard.hps-1.4.2/scripts/populate.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/setup.py` & `wildcard.hps-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     open('README.md').read(),
     open('CHANGES.md').read(),
 ])
 
 
 setup(
     name='wildcard.hps',
-    version='1.4.1',
+    version='1.4.2',
     description="opensearch integration with CastleCMS and Plone",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Development Status :: 5 - Production/Stable",
```

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/brain.py` & `wildcard.hps-1.4.2/src/wildcard/hps/brain.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/browser/configure.zcml` & `wildcard.hps-1.4.2/src/wildcard/hps/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/browser/controlpanel.py` & `wildcard.hps-1.4.2/src/wildcard/hps/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/browser/controlpanel_layout.pt` & `wildcard.hps-1.4.2/src/wildcard/hps/browser/controlpanel_layout.pt`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/browser/utilviews.py` & `wildcard.hps-1.4.2/src/wildcard/hps/browser/utilviews.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/configure.zcml` & `wildcard.hps-1.4.2/src/wildcard/hps/configure.zcml`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/hook.py` & `wildcard.hps-1.4.2/src/wildcard/hps/hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,14 +145,48 @@
         else:
             wrapped_object = obj
     else:
         wrapped_object = obj
     return wrapped_object
 
 
+# Ignore errors in converting to unicode, so json.dumps
+# does not barf when we're trying to send data to opensearch.
+def fix_unicode_for_opensearch(value):
+    val = value
+
+    if not six.PY2 and isinstance(val, bytes):
+        val = val.decode('utf-8', 'ignore')
+    elif six.PY2 and isinstance(val, str):
+        val = six.text_type(val, 'utf-8', 'ignore')
+    elif six.PY2 and isinstance(val, unicode):
+        # we're already getting a unicode string, but maybe it's not good utf-8
+        # so encode it as a string, then use six to convert it back
+        # to an appropriate unicode string, and in the process ignore characters
+        # that would otherwise be a problem
+        val = six.text_type(val.encode('utf-8', 'ignore'), 'utf-8', 'ignore')
+    elif isinstance(val, tuple):
+        vallist = []
+        for v in val:
+            vallist.append(fix_unicode_for_opensearch(v))
+        val = tuple(vallist)
+    elif isinstance(val, list):
+        vallist = []
+        for v in val:
+            vallist.append(fix_unicode_for_opensearch(v))
+        val = vallist
+    elif isinstance(val, dict):
+        valdict = {}
+        for (key, v) in val.items():
+            valdict[key] = fix_unicode_for_opensearch(v)
+        val = valdict
+
+    return val
+
+
 def get_index_data(obj, hpscatalog):  # noqa: C901
     catalog = hpscatalog.catalogtool._catalog
 
     wrapped_object = get_wrapped_object(obj, hpscatalog)
     index_data = {}
     for index_name in catalog.indexes.keys():
         index = getIndex(catalog, index_name)
@@ -165,62 +199,38 @@
                     index_name,
                     traceback.format_exc()))
                 value = None
             if value in (None, 'None'):
                 # yes, we'll index null data...
                 value = None
 
-            # Ignore errors in converting to unicode, so json.dumps
-            # does not barf when we're trying to send data to opensearch.
-            if six.PY2:
-                if isinstance(value, str):
-                    value = six.text_type(value, 'utf-8', 'ignore')
-                elif isinstance(value, unicode):
-                    # we're already getting a unicode string, but maybe it's not good utf-8
-                    # so encode it as a string, then use six to convert it back
-                    # to an appropriate unicode string, and in the process ignore characters
-                    # that would otherwise be a problem
-                    value = six.text_type(value.encode('utf-8', 'ignore'), 'utf-8', 'ignore')
-            else:
-                if isinstance(value, bytes):
-                    value = value.decode('utf-8', 'ignore')
+            value = fix_unicode_for_opensearch(value)
 
             index_data[index_name] = value
 
     # in case these indexes are deleted
     # (to increase performance and improve ram usage)
     for name in getExternalOnlyIndexes():
         if name in index_data:
             continue
         indexer = queryMultiAdapter((obj, hpscatalog.catalogtool), IIndexer, name=name)
         if indexer is not None:
             try:
-                val = indexer()
-                if six.PY2:
-                    if isinstance(val, str):
-                        value = six.text_type(val, 'utf-8', 'ignore')
-                    elif isinstance(val, unicode):
-                        # we're already getting a unicode string, but maybe it's not good utf-8
-                        # so encode it as a string, then use six to convert it back
-                        # to an appropriate unicode string, and in the process ignore characters
-                        # that would otherwise be a problem
-                        value = six.text_type(val.encode('utf-8', 'ignore'), 'utf-8', 'ignore')
-                else:
-                    if isinstance(val, bytes):
-                        value = val.decode('utf-8', 'ignore')
+                val = fix_unicode_for_opensearch(indexer())
                 index_data[name] = val
             except Exception:
                 logger.error('Error indexing value: %s: %s\n%s' % (
                     '/'.join(obj.getPhysicalPath()),
                     name,
                     traceback.format_exc()))
         else:
             val = getattr(obj, name, None)
             if callable(val):
                 val = val()
+            val = fix_unicode_for_opensearch(val)
             index_data[name] = val
 
     for _, adapter in getAdapters((obj,), IAdditionalIndexDataProvider):
         index_data.update(adapter(hpscatalog, index_data))
 
     return index_data
```

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/indexes.py` & `wildcard.hps-1.4.2/src/wildcard/hps/indexes.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/interfaces.py` & `wildcard.hps-1.4.2/src/wildcard/hps/interfaces.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/mapping.py` & `wildcard.hps-1.4.2/src/wildcard/hps/mapping.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/opensearch.py` & `wildcard.hps-1.4.2/src/wildcard/hps/opensearch.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/patches.py` & `wildcard.hps-1.4.2/src/wildcard/hps/patches.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/query.py` & `wildcard.hps-1.4.2/src/wildcard/hps/query.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/scripts/reindex.py` & `wildcard.hps-1.4.2/src/wildcard/hps/scripts/reindex.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/testing.py` & `wildcard.hps-1.4.2/src/wildcard/hps/testing.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/tests/__init__.py` & `wildcard.hps-1.4.2/src/wildcard/hps/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/tests/test_catalog.py` & `wildcard.hps-1.4.2/src/wildcard/hps/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/tests/test_search.py` & `wildcard.hps-1.4.2/src/wildcard/hps/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard/hps/utils.py` & `wildcard.hps-1.4.2/src/wildcard/hps/utils.py`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/src/wildcard.hps.egg-info/PKG-INFO` & `wildcard.hps-1.4.2/src/wildcard.hps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildcard.hps
-Version: 1.4.1
+Version: 1.4.2
 Summary: opensearch integration with CastleCMS and Plone
 Home-page: https://github.com/castlecms/wildcard.hps
 Author: Wildcard Corp.
 Author-email: corporate@wildcardcorp.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/wildcard.hps
 Project-URL: Source, https://github.com/castlecms/wildcard.hps
@@ -195,14 +195,21 @@
 $ ./bin/test
 ```
 
 
 Changelog
 =========
 
+1.4.2 (2023-05-15)
+------------------
+
+- abstract unicode handling code for hook when getting index data, and handle
+  tuples, lists, and dict values
+
+
 1.4.1 (2023-05-11)
 ------------------
 
 - handle unicode error and fix bug in hook when getting index data
 
 
 1.4.0 (2022-11-04)
```

### Comparing `wildcard.hps-1.4.1/src/wildcard.hps.egg-info/SOURCES.txt` & `wildcard.hps-1.4.2/src/wildcard.hps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wildcard.hps-1.4.1/tox.ini` & `wildcard.hps-1.4.2/tox.ini`

 * *Files identical despite different names*

