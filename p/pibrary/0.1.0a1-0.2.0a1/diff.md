# Comparing `tmp/pibrary-0.1.0a1.tar.gz` & `tmp/pibrary-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibrary-0.1.0a1.tar", max compression
+gzip compressed data, was "pibrary-0.2.0a1.tar", max compression
```

## Comparing `pibrary-0.1.0a1.tar` & `pibrary-0.2.0a1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1074 2023-05-08 15:05:56.342612 pibrary-0.1.0a1/LICENSE
--rw-r--r--   0        0        0      111 2023-05-08 15:05:56.342783 pibrary-0.1.0a1/README.md
--rw-r--r--   0        0        0        0 2023-05-09 06:39:08.627636 pibrary-0.1.0a1/pibrary/__init__.py
--rw-r--r--   0        0        0     4446 2023-05-12 02:16:45.133836 pibrary-0.1.0a1/pibrary/file.py
--rw-r--r--   0        0        0      939 2023-05-08 15:05:56.343483 pibrary-0.1.0a1/pibrary/logger.py
--rw-r--r--   0        0        0      459 2023-05-13 03:01:21.992143 pibrary-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 pibrary-0.1.0a1/setup.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 pibrary-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-08 15:05:56.342612 pibrary-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0     1750 2023-05-15 03:36:38.146800 pibrary-0.2.0a1/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 06:39:08.627636 pibrary-0.2.0a1/pibrary/__init__.py
+-rw-r--r--   0        0        0     4446 2023-05-12 02:16:45.133836 pibrary-0.2.0a1/pibrary/file.py
+-rw-r--r--   0        0        0      939 2023-05-08 15:05:56.343483 pibrary-0.2.0a1/pibrary/logger.py
+-rw-r--r--   0        0        0     1435 2023-05-14 14:59:23.553176 pibrary-0.2.0a1/pibrary/string.py
+-rw-r--r--   0        0        0      487 2023-05-15 03:47:16.612269 pibrary-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2497 1970-01-01 00:00:00.000000 pibrary-0.2.0a1/setup.py
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 pibrary-0.2.0a1/PKG-INFO
```

### Comparing `pibrary-0.1.0a1/LICENSE` & `pibrary-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pibrary-0.1.0a1/pibrary/file.py` & `pibrary-0.2.0a1/pibrary/file.py`

 * *Files identical despite different names*

### Comparing `pibrary-0.1.0a1/pibrary/logger.py` & `pibrary-0.2.0a1/pibrary/logger.py`

 * *Files identical despite different names*

