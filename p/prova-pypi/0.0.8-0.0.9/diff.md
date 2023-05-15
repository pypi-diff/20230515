# Comparing `tmp/prova_pypi-0.0.8.tar.gz` & `tmp/prova_pypi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prova_pypi-0.0.8.tar", last modified: Mon May 15 11:02:51 2023, max compression
+gzip compressed data, was "prova_pypi-0.0.9.tar", last modified: Mon May 15 11:10:43 2023, max compression
```

## Comparing `prova_pypi-0.0.8.tar` & `prova_pypi-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 11:02:51.853904 prova_pypi-0.0.8/
--rw-rw-r--   0 gio       (1000) gio       (1000)      308 2023-05-15 11:02:51.853904 prova_pypi-0.0.8/PKG-INFO
--rw-rw-r--   0 gio       (1000) gio       (1000)       19 2023-05-11 20:08:08.000000 prova_pypi-0.0.8/README.md
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 11:02:51.853904 prova_pypi-0.0.8/prova_pypi/
--rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-11 20:08:08.000000 prova_pypi-0.0.8/prova_pypi/__init__.py
--rw-rw-r--   0 gio       (1000) gio       (1000)        0 2023-05-11 20:08:08.000000 prova_pypi-0.0.8/prova_pypi/prova.py
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 11:02:51.853904 prova_pypi-0.0.8/prova_pypi/utils/
--rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-11 20:08:08.000000 prova_pypi-0.0.8/prova_pypi/utils/__init__.py
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 11:02:51.853904 prova_pypi-0.0.8/prova_pypi.egg-info/
--rw-rw-r--   0 gio       (1000) gio       (1000)      308 2023-05-15 11:02:51.000000 prova_pypi-0.0.8/prova_pypi.egg-info/PKG-INFO
--rw-rw-r--   0 gio       (1000) gio       (1000)      226 2023-05-15 11:02:51.000000 prova_pypi-0.0.8/prova_pypi.egg-info/SOURCES.txt
--rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-15 11:02:51.000000 prova_pypi-0.0.8/prova_pypi.egg-info/dependency_links.txt
--rw-rw-r--   0 gio       (1000) gio       (1000)       11 2023-05-15 11:02:51.000000 prova_pypi-0.0.8/prova_pypi.egg-info/top_level.txt
--rw-rw-r--   0 gio       (1000) gio       (1000)       38 2023-05-15 11:02:51.853904 prova_pypi-0.0.8/setup.cfg
--rw-rw-r--   0 gio       (1000) gio       (1000)      427 2023-05-15 11:02:47.000000 prova_pypi-0.0.8/setup.py
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 11:10:43.406460 prova_pypi-0.0.9/
+-rw-rw-r--   0 gio       (1000) gio       (1000)      308 2023-05-15 11:10:43.406460 prova_pypi-0.0.9/PKG-INFO
+-rw-rw-r--   0 gio       (1000) gio       (1000)       19 2023-05-11 20:08:08.000000 prova_pypi-0.0.9/README.md
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 11:10:43.406460 prova_pypi-0.0.9/prova_pypi/
+-rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-11 20:08:08.000000 prova_pypi-0.0.9/prova_pypi/__init__.py
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 11:10:43.406460 prova_pypi-0.0.9/prova_pypi/model/
+-rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-15 11:10:41.000000 prova_pypi-0.0.9/prova_pypi/model/__init__.py
+-rw-rw-r--   0 gio       (1000) gio       (1000)        0 2023-05-11 20:08:08.000000 prova_pypi-0.0.9/prova_pypi/prova.py
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 11:10:43.406460 prova_pypi-0.0.9/prova_pypi/utils/
+-rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-11 20:08:08.000000 prova_pypi-0.0.9/prova_pypi/utils/__init__.py
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-15 11:10:43.406460 prova_pypi-0.0.9/prova_pypi.egg-info/
+-rw-rw-r--   0 gio       (1000) gio       (1000)      308 2023-05-15 11:10:43.000000 prova_pypi-0.0.9/prova_pypi.egg-info/PKG-INFO
+-rw-rw-r--   0 gio       (1000) gio       (1000)      255 2023-05-15 11:10:43.000000 prova_pypi-0.0.9/prova_pypi.egg-info/SOURCES.txt
+-rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-15 11:10:43.000000 prova_pypi-0.0.9/prova_pypi.egg-info/dependency_links.txt
+-rw-rw-r--   0 gio       (1000) gio       (1000)       11 2023-05-15 11:10:43.000000 prova_pypi-0.0.9/prova_pypi.egg-info/top_level.txt
+-rw-rw-r--   0 gio       (1000) gio       (1000)       38 2023-05-15 11:10:43.406460 prova_pypi-0.0.9/setup.cfg
+-rw-rw-r--   0 gio       (1000) gio       (1000)      427 2023-05-15 11:10:41.000000 prova_pypi-0.0.9/setup.py
```

