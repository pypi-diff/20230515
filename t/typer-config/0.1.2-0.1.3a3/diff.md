# Comparing `tmp/typer_config-0.1.2.tar.gz` & `tmp/typer_config-0.1.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.1.2.tar", max compression
+gzip compressed data, was "typer_config-0.1.3a3.tar", max compression
```

## Comparing `typer_config-0.1.2.tar` & `typer_config-0.1.3a3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-01 23:14:04.009855 typer_config-0.1.2/LICENSE
--rw-r--r--   0        0        0     3693 2023-05-01 23:14:04.009855 typer_config-0.1.2/README.md
--rw-r--r--   0        0        0      784 2023-05-01 23:14:04.009855 typer_config-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1328 2023-05-01 23:14:04.009855 typer_config-0.1.2/typer_config/__init__.py
--rw-r--r--   0        0        0     1869 2023-05-01 23:14:04.009855 typer_config-0.1.2/typer_config/loaders.py
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 typer_config-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/LICENSE
+-rw-r--r--   0        0        0     1044 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/README.md
+-rw-r--r--   0        0        0     1010 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/pyproject.toml
+-rw-r--r--   0        0        0     1434 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/typer_config/__init__.py
+-rw-r--r--   0        0        0     1081 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/typer_config/_typing.py
+-rw-r--r--   0        0        0     3714 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/typer_config/loaders.py
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 typer_config-0.1.3a3/PKG-INFO
```

### Comparing `typer_config-0.1.2/LICENSE` & `typer_config-0.1.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.2/pyproject.toml` & `typer_config-0.1.3a3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.1.2"
+version = "0.1.3a3"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 keywords = ["typer"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-typer = "^0.8.0"
+typer = "^0"
 toml = {version = "^0.10.2", optional = true}
 pyyaml = {version = "^6.0", optional = true}
 
 [tool.poetry.extras]
 toml = ["toml"]
 yaml = ["pyyaml"]
 all = ["toml", "pyyaml"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.263"
 pylint = "^2.17.3"
 black = "^23.3.0"
 isort = "^5.12.0"
 pytest = "^7.3.1"
+mypy = "^1.2.0"
+types-toml = "^0.10.8.6"
+types-pyyaml = "^6.0.12.9"
+coverage = "^7.2.5"
+
+[tool.poetry.group.docs.dependencies]
+mkdocs-material = "^9.1.9"
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+mike = "^1.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

