# Comparing `tmp/ksconf-0.11.2b1.tar.gz` & `tmp/ksconf-0.11.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksconf-0.11.2b1.tar", last modified: Sun May 14 02:47:58 2023, max compression
+gzip compressed data, was "ksconf-0.11.3b1.tar", last modified: Mon May 15 13:09:35 2023, max compression
```

## Comparing `ksconf-0.11.2b1.tar` & `ksconf-0.11.3b1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:58.007106 ksconf-0.11.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-14 02:47:58.007106 ksconf-0.11.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:57.999106 ksconf-0.11.2b1/ksconf/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-14 02:47:57.000000 ksconf-0.11.2b1/ksconf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:57.999106 ksconf-0.11.2b1/ksconf/app/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/app/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/app/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/app/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:57.999106 ksconf-0.11.2b1/ksconf/builder/
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/builder/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/builder/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/builder/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:58.003106 ksconf-0.11.2b1/ksconf/commands/
--rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/promote.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/restexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/restpublish.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/unarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/commands/xmlformat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:58.003106 ksconf-0.11.2b1/ksconf/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/conf/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/conf/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/conf/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/conf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:58.003106 ksconf-0.11.2b1/ksconf/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14340 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/setup_entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:58.007106 ksconf-0.11.2b1/ksconf/util/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/util/completers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/util/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/util/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/util/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:58.007106 ksconf-0.11.2b1/ksconf/vc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/vc/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/ksconf/xmlformat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:47:57.999106 ksconf-0.11.2b1/ksconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-14 02:47:57.000000 ksconf-0.11.2b1/ksconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-14 02:47:57.000000 ksconf-0.11.2b1/ksconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 02:47:57.000000 ksconf-0.11.2b1/ksconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-14 02:47:57.000000 ksconf-0.11.2b1/ksconf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 02:47:57.000000 ksconf-0.11.2b1/ksconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 02:47:57.000000 ksconf-0.11.2b1/ksconf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 02:47:42.000000 ksconf-0.11.2b1/ksconf.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-14 02:47:58.007106 ksconf-0.11.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-14 02:47:31.000000 ksconf-0.11.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.291230 ksconf-0.11.3b1/ksconf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/app/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/app/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/app/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/builder/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/builder/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/builder/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/promote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/restexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/restpublish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/unarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/xmlformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14340 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/setup_entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/completers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/vc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/vc/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/xmlformat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.291230 ksconf-0.11.3b1/ksconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:09:20.000000 ksconf-0.11.3b1/ksconf.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 13:09:35.299230 ksconf-0.11.3b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/setup.py
```

### Comparing `ksconf-0.11.2b1/LICENSE` & `ksconf-0.11.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/PKG-INFO` & `ksconf-0.11.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.11.2b1
+Version: 0.11.3b1
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.11.2b1/README.md` & `ksconf-0.11.3b1/README.md`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/__init__.py` & `ksconf-0.11.3b1/ksconf/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/__main__.py` & `ksconf-0.11.3b1/ksconf/__main__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/app/__init__.py` & `ksconf-0.11.3b1/ksconf/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/app/deploy.py` & `ksconf-0.11.3b1/ksconf/app/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,16 +181,16 @@
 
     @classmethod
     def from_manifest_transformation(
             cls,
             base: AppManifest,
             target: AppManifest) -> "DeploySequence":
         seq = cls()
-        if target is None:
-            return cls.from_manifest(base)
+        if base is None:
+            return cls.from_manifest(target)
         if base.name != target.name:
             raise ValueError(f"Manifest must have the same app name.  {base.name} != {target.name}")
         seq.add(DeployAction_SourceReference(target.source, target.hash))
         seq.add(DeployAction_SetAppName(target.name))
 
         base_files = {f.path: f for f in base.files}
         target_files = {f.path: f for f in target.files}
```

### Comparing `ksconf-0.11.2b1/ksconf/app/facts.py` & `ksconf-0.11.3b1/ksconf/app/facts.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/app/manifest.py` & `ksconf-0.11.3b1/ksconf/app/manifest.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/archive.py` & `ksconf-0.11.3b1/ksconf/archive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/builder/__init__.py` & `ksconf-0.11.3b1/ksconf/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/builder/cache.py` & `ksconf-0.11.3b1/ksconf/builder/cache.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/builder/core.py` & `ksconf-0.11.3b1/ksconf/builder/core.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/builder/steps.py` & `ksconf-0.11.3b1/ksconf/builder/steps.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/cli.py` & `ksconf-0.11.3b1/ksconf/cli.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/combine.py` & `ksconf-0.11.3b1/ksconf/combine.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/__init__.py` & `ksconf-0.11.3b1/ksconf/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/check.py` & `ksconf-0.11.3b1/ksconf/commands/check.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/combine.py` & `ksconf-0.11.3b1/ksconf/commands/combine.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/diff.py` & `ksconf-0.11.3b1/ksconf/commands/diff.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/filter.py` & `ksconf-0.11.3b1/ksconf/commands/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/merge.py` & `ksconf-0.11.3b1/ksconf/commands/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/minimize.py` & `ksconf-0.11.3b1/ksconf/commands/minimize.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/package.py` & `ksconf-0.11.3b1/ksconf/commands/package.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/promote.py` & `ksconf-0.11.3b1/ksconf/commands/promote.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/restexport.py` & `ksconf-0.11.3b1/ksconf/commands/restexport.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/restpublish.py` & `ksconf-0.11.3b1/ksconf/commands/restpublish.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/snapshot.py` & `ksconf-0.11.3b1/ksconf/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/sort.py` & `ksconf-0.11.3b1/ksconf/commands/sort.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/unarchive.py` & `ksconf-0.11.3b1/ksconf/commands/unarchive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/commands/xmlformat.py` & `ksconf-0.11.3b1/ksconf/commands/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/compat.py` & `ksconf-0.11.3b1/ksconf/compat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/conf/delta.py` & `ksconf-0.11.3b1/ksconf/conf/delta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/conf/merge.py` & `ksconf-0.11.3b1/ksconf/conf/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/conf/meta.py` & `ksconf-0.11.3b1/ksconf/conf/meta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/conf/parser.py` & `ksconf-0.11.3b1/ksconf/conf/parser.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/consts.py` & `ksconf-0.11.3b1/ksconf/consts.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/filter.py` & `ksconf-0.11.3b1/ksconf/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/layer.py` & `ksconf-0.11.3b1/ksconf/layer.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/package.py` & `ksconf-0.11.3b1/ksconf/package.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/setup_entrypoints.py` & `ksconf-0.11.3b1/ksconf/setup_entrypoints.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/util/__init__.py` & `ksconf-0.11.3b1/ksconf/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/util/compare.py` & `ksconf-0.11.3b1/ksconf/util/compare.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/util/completers.py` & `ksconf-0.11.3b1/ksconf/util/completers.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/util/file.py` & `ksconf-0.11.3b1/ksconf/util/file.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/util/rest.py` & `ksconf-0.11.3b1/ksconf/util/rest.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/util/terminal.py` & `ksconf-0.11.3b1/ksconf/util/terminal.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/vc/git.py` & `ksconf-0.11.3b1/ksconf/vc/git.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf/xmlformat.py` & `ksconf-0.11.3b1/ksconf/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf.egg-info/PKG-INFO` & `ksconf-0.11.3b1/ksconf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.11.2b1
+Version: 0.11.3b1
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.11.2b1/ksconf.egg-info/SOURCES.txt` & `ksconf-0.11.3b1/ksconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/ksconf.egg-info/entry_points.txt` & `ksconf-0.11.3b1/ksconf.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.2b1/setup.py` & `ksconf-0.11.3b1/setup.py`

 * *Files identical despite different names*

