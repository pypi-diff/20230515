# Comparing `tmp/a1rn-0.1.1.tar.gz` & `tmp/a1rn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\a1rn-0.1.1.tar", last modified: Mon May 15 09:20:24 2023, max compression
+gzip compressed data, was "dist\a1rn-0.1.2.tar", last modified: Mon May 15 09:27:49 2023, max compression
```

## Comparing `a1rn-0.1.1.tar` & `a1rn-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:20:24.000000 a1rn-0.1.1/
--rw-rw-rw-   0        0        0      368 2023-05-15 09:20:24.000000 a1rn-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-15 09:20:24.000000 a1rn-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      469 2023-05-15 09:17:50.000000 a1rn-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:20:24.000000 a1rn-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 09:20:24.000000 a1rn-0.1.1/src/a1rn.egg-info/
--rw-rw-rw-   0        0        0      368 2023-05-15 09:20:24.000000 a1rn-0.1.1/src/a1rn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-05-15 09:20:24.000000 a1rn-0.1.1/src/a1rn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:20:24.000000 a1rn-0.1.1/src/a1rn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:20:24.000000 a1rn-0.1.1/src/a1rn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 09:27:49.000000 a1rn-0.1.2/
+-rw-rw-rw-   0        0        0      368 2023-05-15 09:27:49.000000 a1rn-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-05-15 09:27:49.000000 a1rn-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      469 2023-05-15 09:27:18.000000 a1rn-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:27:49.000000 a1rn-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 09:27:49.000000 a1rn-0.1.2/src/a1rn.egg-info/
+-rw-rw-rw-   0        0        0      368 2023-05-15 09:27:49.000000 a1rn-0.1.2/src/a1rn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-05-15 09:27:49.000000 a1rn-0.1.2/src/a1rn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 09:27:49.000000 a1rn-0.1.2/src/a1rn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 09:27:49.000000 a1rn-0.1.2/src/a1rn.egg-info/top_level.txt
```

