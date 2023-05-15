# Comparing `tmp/typer_config-0.1.2.tar.gz` & `tmp/typer_config-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.1.2.tar", max compression
+gzip compressed data, was "typer_config-0.1.3.tar", max compression
```

## Comparing `typer_config-0.1.2.tar` & `typer_config-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-01 23:14:04.009855 typer_config-0.1.2/LICENSE
--rw-r--r--   0        0        0     3693 2023-05-01 23:14:04.009855 typer_config-0.1.2/README.md
--rw-r--r--   0        0        0      784 2023-05-01 23:14:04.009855 typer_config-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1328 2023-05-01 23:14:04.009855 typer_config-0.1.2/typer_config/__init__.py
--rw-r--r--   0        0        0     1869 2023-05-01 23:14:04.009855 typer_config-0.1.2/typer_config/loaders.py
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 typer_config-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-15 03:20:33.887810 typer_config-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1044 2023-05-15 03:20:33.887810 typer_config-0.1.3/README.md
+-rw-r--r--   0        0        0     2150 2023-05-15 03:20:33.887810 typer_config-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1621 2023-05-15 03:20:33.887810 typer_config-0.1.3/typer_config/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-15 03:20:33.887810 typer_config-0.1.3/typer_config/__typing.py
+-rw-r--r--   0        0        0     3758 2023-05-15 03:20:33.887810 typer_config-0.1.3/typer_config/loaders.py
+-rw-r--r--   0        0        0     2936 1970-01-01 00:00:00.000000 typer_config-0.1.3/PKG-INFO
```

### Comparing `typer_config-0.1.2/LICENSE` & `typer_config-0.1.3/LICENSE`

 * *Files identical despite different names*

