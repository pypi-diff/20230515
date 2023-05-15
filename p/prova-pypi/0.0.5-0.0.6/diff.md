# Comparing `tmp/prova_pypi-0.0.5.tar.gz` & `tmp/prova_pypi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prova_pypi-0.0.5.tar", last modified: Mon May 15 10:39:38 2023, max compression
+gzip compressed data, was "prova_pypi-0.0.6.tar", last modified: Mon May 15 10:43:54 2023, max compression
```

## Comparing `prova_pypi-0.0.5.tar` & `prova_pypi-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 10:39:38.811447 prova_pypi-0.0.5/
--rw-rw-r--   0 gio       (1000) gio       (1000)      308 2023-05-15 10:39:38.811447 prova_pypi-0.0.5/PKG-INFO
--rw-rw-r--   0 gio       (1000) gio       (1000)       19 2023-05-11 20:08:08.000000 prova_pypi-0.0.5/README.md
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 10:39:38.811447 prova_pypi-0.0.5/prova_pypi/
--rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-11 20:08:08.000000 prova_pypi-0.0.5/prova_pypi/__init__.py
--rw-rw-r--   0 gio       (1000) gio       (1000)        0 2023-05-11 20:08:08.000000 prova_pypi-0.0.5/prova_pypi/prova.py
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 10:39:38.811447 prova_pypi-0.0.5/prova_pypi.egg-info/
--rw-rw-r--   0 gio       (1000) gio       (1000)      308 2023-05-15 10:39:38.000000 prova_pypi-0.0.5/prova_pypi.egg-info/PKG-INFO
--rw-rw-r--   0 gio       (1000) gio       (1000)      197 2023-05-15 10:39:38.000000 prova_pypi-0.0.5/prova_pypi.egg-info/SOURCES.txt
--rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-15 10:39:38.000000 prova_pypi-0.0.5/prova_pypi.egg-info/dependency_links.txt
--rw-rw-r--   0 gio       (1000) gio       (1000)       11 2023-05-15 10:39:38.000000 prova_pypi-0.0.5/prova_pypi.egg-info/top_level.txt
--rw-rw-r--   0 gio       (1000) gio       (1000)       38 2023-05-15 10:39:38.811447 prova_pypi-0.0.5/setup.cfg
--rw-rw-r--   0 gio       (1000) gio       (1000)      410 2023-05-15 10:38:26.000000 prova_pypi-0.0.5/setup.py
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 10:43:54.068823 prova_pypi-0.0.6/
+-rw-rw-r--   0 gio       (1000) gio       (1000)      308 2023-05-15 10:43:54.068823 prova_pypi-0.0.6/PKG-INFO
+-rw-rw-r--   0 gio       (1000) gio       (1000)       19 2023-05-11 20:08:08.000000 prova_pypi-0.0.6/README.md
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 10:43:54.068823 prova_pypi-0.0.6/prova_pypi/
+-rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-11 20:08:08.000000 prova_pypi-0.0.6/prova_pypi/__init__.py
+-rw-rw-r--   0 gio       (1000) gio       (1000)        0 2023-05-11 20:08:08.000000 prova_pypi-0.0.6/prova_pypi/prova.py
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 10:43:54.068823 prova_pypi-0.0.6/prova_pypi.egg-info/
+-rw-rw-r--   0 gio       (1000) gio       (1000)      308 2023-05-15 10:43:54.000000 prova_pypi-0.0.6/prova_pypi.egg-info/PKG-INFO
+-rw-rw-r--   0 gio       (1000) gio       (1000)      197 2023-05-15 10:43:54.000000 prova_pypi-0.0.6/prova_pypi.egg-info/SOURCES.txt
+-rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-15 10:43:54.000000 prova_pypi-0.0.6/prova_pypi.egg-info/dependency_links.txt
+-rw-rw-r--   0 gio       (1000) gio       (1000)       11 2023-05-15 10:43:54.000000 prova_pypi-0.0.6/prova_pypi.egg-info/top_level.txt
+-rw-rw-r--   0 gio       (1000) gio       (1000)       38 2023-05-15 10:43:54.068823 prova_pypi-0.0.6/setup.cfg
+-rw-rw-r--   0 gio       (1000) gio       (1000)      427 2023-05-15 10:43:51.000000 prova_pypi-0.0.6/setup.py
```

