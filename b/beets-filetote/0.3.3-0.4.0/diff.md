# Comparing `tmp/beets_filetote-0.3.3.tar.gz` & `tmp/beets_filetote-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets_filetote-0.3.3.tar", max compression
+gzip compressed data, was "beets_filetote-0.4.0.tar", max compression
```

## Comparing `beets_filetote-0.3.3.tar` & `beets_filetote-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1143 2023-01-08 21:55:13.026236 beets_filetote-0.3.3/LICENSE
--rw-r--r--   0        0        0     6180 2023-01-08 21:55:13.030236 beets_filetote-0.3.3/README.md
--rw-r--r--   0        0        0      144 2023-01-08 21:55:13.030236 beets_filetote-0.3.3/beetsplug/__init__.py
--rw-r--r--   0        0        0    15878 2023-01-08 21:55:13.030236 beets_filetote-0.3.3/beetsplug/filetote.py
--rw-r--r--   0        0        0     1338 2023-01-08 21:55:13.030236 beets_filetote-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     7165 1970-01-01 00:00:00.000000 beets_filetote-0.3.3/setup.py
--rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 beets_filetote-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1143 2023-05-14 23:05:36.351821 beets_filetote-0.4.0/LICENSE
+-rw-r--r--   0        0        0    13498 2023-05-14 23:05:36.351821 beets_filetote-0.4.0/README.md
+-rw-r--r--   0        0        0      144 2023-05-14 23:05:36.351821 beets_filetote-0.4.0/beetsplug/__init__.py
+-rw-r--r--   0        0        0    24392 2023-05-14 23:05:36.351821 beets_filetote-0.4.0/beetsplug/filetote.py
+-rw-r--r--   0        0        0     2571 2023-05-14 23:05:36.351821 beets_filetote-0.4.0/beetsplug/filetote_dataclasses.py
+-rw-r--r--   0        0        0     2314 2023-05-14 23:05:36.351821 beets_filetote-0.4.0/beetsplug/mapping_model.py
+-rw-r--r--   0        0        0     2010 2023-05-14 23:05:36.351821 beets_filetote-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    15120 1970-01-01 00:00:00.000000 beets_filetote-0.4.0/PKG-INFO
```

### Comparing `beets_filetote-0.3.3/LICENSE` & `beets_filetote-0.4.0/LICENSE`

 * *Files identical despite different names*

