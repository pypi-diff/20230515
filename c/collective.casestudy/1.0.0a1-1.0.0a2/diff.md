# Comparing `tmp/collective.casestudy-1.0.0a1.tar.gz` & `tmp/collective.casestudy-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.casestudy-1.0.0a1.tar", last modified: Wed Dec  7 00:16:57 2022, max compression
+gzip compressed data, was "collective.casestudy-1.0.0a2.tar", last modified: Mon May 15 08:44:57 2023, max compression
```

## Comparing `collective.casestudy-1.0.0a1.tar` & `collective.casestudy-1.0.0a2.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.075061 collective.casestudy-1.0.0a1/
--rw-r--r--   0 ericof     (501) staff       (20)       66 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/CHANGELOG.md
--rw-r--r--   0 ericof     (501) staff       (20)       49 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/CONTRIBUTORS.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/LICENSE.md
--rw-r--r--   0 ericof     (501) staff       (20)       66 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     4535 2022-12-07 00:16:57.074913 collective.casestudy-1.0.0a1/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     3279 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/README.md
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.068669 collective.casestudy-1.0.0a1/docs/
--rw-r--r--   0 ericof     (501) staff       (20)     8072 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/docs/icon.svg
--rw-r--r--   0 ericof     (501) staff       (20)      800 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)       38 2022-12-07 00:16:57.075105 collective.casestudy-1.0.0a1/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2206 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.065954 collective.casestudy-1.0.0a1/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.068838 collective.casestudy-1.0.0a1/src/collective/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.070937 collective.casestudy-1.0.0a1/src/collective/casestudy/
--rw-r--r--   0 ericof     (501) staff       (20)      201 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.071402 collective.casestudy-1.0.0a1/src/collective/casestudy/browser/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/browser/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      667 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/browser/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1009 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/browser/controlpanel.py
--rw-r--r--   0 ericof     (501) staff       (20)      670 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.071686 collective.casestudy-1.0.0a1/src/collective/casestudy/content/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/content/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1096 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/content/case_study.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.072094 collective.casestudy-1.0.0a1/src/collective/casestudy/indexers/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/indexers/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      245 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/indexers/case_study.py
--rw-r--r--   0 ericof     (501) staff       (20)      271 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/indexers/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1013 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/interfaces.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.072381 collective.casestudy-1.0.0a1/src/collective/casestudy/locales/
--rw-r--r--   0 ericof     (501) staff       (20)     3133 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/locales/collective.casestudy.pot
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.066501 collective.casestudy-1.0.0a1/src/collective/casestudy/locales/pt_BR/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.072545 collective.casestudy-1.0.0a1/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     3438 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/collective.casestudy.po
--rw-r--r--   0 ericof     (501) staff       (20)     1946 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/locales/update.py
--rw-r--r--   0 ericof     (501) staff       (20)      287 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/permissions.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.066882 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.073253 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/
--rw-r--r--   0 ericof     (501) staff       (20)      169 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/browserlayer.xml
--rw-r--r--   0 ericof     (501) staff       (20)      503 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/catalog.xml
--rw-r--r--   0 ericof     (501) staff       (20)      458 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/controlpanel.xml
--rw-r--r--   0 ericof     (501) staff       (20)      107 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/metadata.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.073547 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/registry/
--rw-r--r--   0 ericof     (501) staff       (20)     1080 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/registry/main.xml
--rw-r--r--   0 ericof     (501) staff       (20)     2359 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/registry/querystring.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.073689 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/types/
--rw-r--r--   0 ericof     (501) staff       (20)     2866 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/types/CaseStudy.xml
--rw-r--r--   0 ericof     (501) staff       (20)      184 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/types.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.073828 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/uninstall/
--rw-r--r--   0 ericof     (501) staff       (20)      123 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 ericof     (501) staff       (20)      742 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/profiles.zcml
--rw-r--r--   0 ericof     (501) staff       (20)      671 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/testing.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.074071 collective.casestudy-1.0.0a1/src/collective/casestudy/upgrades/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/upgrades/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      140 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/upgrades/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.074698 collective.casestudy-1.0.0a1/src/collective/casestudy/vocabularies/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/vocabularies/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      435 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/vocabularies/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)      519 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/vocabularies/industries.py
--rw-r--r--   0 ericof     (501) staff       (20)      505 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/vocabularies/usages.py
--rw-r--r--   0 ericof     (501) staff       (20)      548 2022-12-07 00:16:56.000000 collective.casestudy-1.0.0a1/src/collective/casestudy/vocabularies/versions.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2022-12-07 00:16:57.069999 collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     4535 2022-12-07 00:16:57.000000 collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     2179 2022-12-07 00:16:57.000000 collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2022-12-07 00:16:57.000000 collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)      125 2022-12-07 00:16:57.000000 collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2022-12-07 00:16:57.000000 collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)      146 2022-12-07 00:16:57.000000 collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2022-12-07 00:16:57.000000 collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/top_level.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2022-12-07 00:16:57.000000 collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/zip-safe
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.334089 collective.casestudy-1.0.0a2/
+-rw-r--r--   0 ericof     (501) staff       (20)      174 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/CHANGELOG.md
+-rw-r--r--   0 ericof     (501) staff       (20)       49 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/CONTRIBUTORS.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/LICENSE.md
+-rw-r--r--   0 ericof     (501) staff       (20)       66 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     4643 2023-05-15 08:44:57.333955 collective.casestudy-1.0.0a2/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     3279 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/README.md
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.327446 collective.casestudy-1.0.0a2/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)     8072 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/docs/icon.svg
+-rw-r--r--   0 ericof     (501) staff       (20)      800 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-05-15 08:44:57.334130 collective.casestudy-1.0.0a2/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2207 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.325105 collective.casestudy-1.0.0a2/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.327590 collective.casestudy-1.0.0a2/src/collective/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.329677 collective.casestudy-1.0.0a2/src/collective/casestudy/
+-rw-r--r--   0 ericof     (501) staff       (20)      201 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.330149 collective.casestudy-1.0.0a2/src/collective/casestudy/browser/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/browser/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      667 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/browser/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1009 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/browser/controlpanel.py
+-rw-r--r--   0 ericof     (501) staff       (20)      670 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.330446 collective.casestudy-1.0.0a2/src/collective/casestudy/content/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/content/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1096 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/content/case_study.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.330846 collective.casestudy-1.0.0a2/src/collective/casestudy/indexers/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/indexers/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      245 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/indexers/case_study.py
+-rw-r--r--   0 ericof     (501) staff       (20)      271 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/indexers/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1013 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/interfaces.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.331118 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/
+-rw-r--r--   0 ericof     (501) staff       (20)     3133 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/collective.casestudy.pot
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.325623 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/es/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.331272 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/es/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)     3793 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/es/LC_MESSAGES/collective.casestudy.po
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.325752 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/pt_BR/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.331419 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)     3438 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/collective.casestudy.po
+-rw-r--r--   0 ericof     (501) staff       (20)     1946 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/update.py
+-rw-r--r--   0 ericof     (501) staff       (20)      287 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/permissions.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.326122 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.332185 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/
+-rw-r--r--   0 ericof     (501) staff       (20)      169 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/browserlayer.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      503 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/catalog.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      458 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/controlpanel.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      107 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/metadata.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.332457 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/registry/
+-rw-r--r--   0 ericof     (501) staff       (20)     1080 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/registry/main.xml
+-rw-r--r--   0 ericof     (501) staff       (20)     2359 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/registry/querystring.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.332619 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/types/
+-rw-r--r--   0 ericof     (501) staff       (20)     2866 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/types/CaseStudy.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      184 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/types.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.332779 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/uninstall/
+-rw-r--r--   0 ericof     (501) staff       (20)      123 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      742 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      671 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.333048 collective.casestudy-1.0.0a2/src/collective/casestudy/upgrades/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/upgrades/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      140 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/upgrades/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.333738 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      435 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      519 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/industries.py
+-rw-r--r--   0 ericof     (501) staff       (20)      505 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/usages.py
+-rw-r--r--   0 ericof     (501) staff       (20)      548 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/versions.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.328738 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)     4643 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     2251 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      125 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       11 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      147 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       11 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/top_level.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/zip-safe
```

### Comparing `collective.casestudy-1.0.0a1/LICENSE.md` & `collective.casestudy-1.0.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/PKG-INFO` & `collective.casestudy-1.0.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.casestudy
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Case Study content type for Plone.
 Home-page: https://github.com/collective/collective.casestudy
 Author: Plone Community
 Author-email: ericof@plone.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.casestudy
 Project-URL: Source, https://github.com/collective/collective.casestudy
@@ -119,12 +119,20 @@
 -------
 
 The project is licensed under the GPLv2.
 
 
 # Changelog
 
+1.0.0a2 (2023-05-15)
+
+- Added Spanish translation [macagua]
+
+- Use `pytest-plone` for testing.
+  [ericof]
+
+
 ## 1.0.0a1 (2022-12-06)
 
 - Initial release. [ericof]
```

### Comparing `collective.casestudy-1.0.0a1/README.md` & `collective.casestudy-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/docs/icon.svg` & `collective.casestudy-1.0.0a2/docs/icon.svg`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/pyproject.toml` & `collective.casestudy-1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/setup.py` & `collective.casestudy-1.0.0a2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGELOG.md").read_text()}\n
 """
 
 setup(
     name="collective.casestudy",
-    version="1.0.0a1",
+    version="1.0.0a2",
     description="Case Study content type for Plone.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -48,20 +48,20 @@
     install_requires=[
         "setuptools",
         "Plone",
         "plone.api",
     ],
     extras_require={
         "test": [
-            "gocept.pytestlayer",
             "zest.releaser[recommended]",
             "plone.app.testing>=7.0.0a3",
             "plone.restapi[test]",
             "pytest",
             "pytest-cov",
+            "pytest-plone>=0.2.0",
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     [console_scripts]
     update_locale = collective.casestudy.locales.update:update_locale
```

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/browser/configure.zcml` & `collective.casestudy-1.0.0a2/src/collective/casestudy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/browser/controlpanel.py` & `collective.casestudy-1.0.0a2/src/collective/casestudy/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/configure.zcml` & `collective.casestudy-1.0.0a2/src/collective/casestudy/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/content/case_study.py` & `collective.casestudy-1.0.0a2/src/collective/casestudy/content/case_study.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/interfaces.py` & `collective.casestudy-1.0.0a2/src/collective/casestudy/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/locales/collective.casestudy.pot` & `collective.casestudy-1.0.0a2/src/collective/casestudy/locales/collective.casestudy.pot`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/collective.casestudy.po` & `collective.casestudy-1.0.0a2/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/collective.casestudy.po`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/locales/update.py` & `collective.casestudy-1.0.0a2/src/collective/casestudy/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/registry/main.xml` & `collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/registry/main.xml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/registry/querystring.xml` & `collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/registry/querystring.xml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/profiles/default/types/CaseStudy.xml` & `collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/types/CaseStudy.xml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/profiles.zcml` & `collective.casestudy-1.0.0a2/src/collective/casestudy/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/testing.py` & `collective.casestudy-1.0.0a2/src/collective/casestudy/testing.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/vocabularies/industries.py` & `collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/industries.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective/casestudy/vocabularies/versions.py` & `collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/versions.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/PKG-INFO` & `collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.casestudy
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Case Study content type for Plone.
 Home-page: https://github.com/collective/collective.casestudy
 Author: Plone Community
 Author-email: ericof@plone.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.casestudy
 Project-URL: Source, https://github.com/collective/collective.casestudy
@@ -119,12 +119,20 @@
 -------
 
 The project is licensed under the GPLv2.
 
 
 # Changelog
 
+1.0.0a2 (2023-05-15)
+
+- Added Spanish translation [macagua]
+
+- Use `pytest-plone` for testing.
+  [ericof]
+
+
 ## 1.0.0a1 (2022-12-06)
 
 - Initial release. [ericof]
```

### Comparing `collective.casestudy-1.0.0a1/src/collective.casestudy.egg-info/SOURCES.txt` & `collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/collective/casestudy/content/__init__.py
 src/collective/casestudy/content/case_study.py
 src/collective/casestudy/indexers/__init__.py
 src/collective/casestudy/indexers/case_study.py
 src/collective/casestudy/indexers/configure.zcml
 src/collective/casestudy/locales/collective.casestudy.pot
 src/collective/casestudy/locales/update.py
+src/collective/casestudy/locales/es/LC_MESSAGES/collective.casestudy.po
 src/collective/casestudy/locales/pt_BR/LC_MESSAGES/collective.casestudy.po
 src/collective/casestudy/profiles/default/browserlayer.xml
 src/collective/casestudy/profiles/default/catalog.xml
 src/collective/casestudy/profiles/default/controlpanel.xml
 src/collective/casestudy/profiles/default/metadata.xml
 src/collective/casestudy/profiles/default/types.xml
 src/collective/casestudy/profiles/default/registry/main.xml
```

