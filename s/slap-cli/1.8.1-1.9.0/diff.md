# Comparing `tmp/slap_cli-1.8.1.tar.gz` & `tmp/slap_cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slap_cli-1.8.1.tar", max compression
+gzip compressed data, was "slap_cli-1.9.0.tar", max compression
```

## Comparing `slap_cli-1.8.1.tar` & `slap_cli-1.9.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1002 2023-05-13 10:33:37.160056 slap_cli-1.8.1/LICENSE
--rw-r--r--   0        0        0     4974 2023-05-13 19:14:08.329715 slap_cli-1.8.1/pyproject.toml
--rw-r--r--   0        0        0       98 2023-05-13 19:14:08.333715 slap_cli-1.8.1/src/slap/__init__.py
--rw-r--r--   0        0        0       82 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/__main__.py
--rw-r--r--   0        0        0    10314 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/application.py
--rw-r--r--   0        0        0     9163 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/changelog.py
--rw-r--r--   0        0        0     3353 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/check.py
--rw-r--r--   0        0        0     2520 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/configuration.py
--rw-r--r--   0        0        0     5337 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/add.py
--rw-r--r--   0        0        0    27292 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/changelog.py
--rw-r--r--   0        0        0     6202 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/check.py
--rw-r--r--   0        0        0     3049 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/info.py
--rw-r--r--   0        0        0     4783 2023-05-13 18:51:06.372905 slap_cli-1.8.1/src/slap/ext/application/init.py
--rw-r--r--   0        0        0    14043 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/install.py
--rw-r--r--   0        0        0     5930 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/link.py
--rw-r--r--   0        0        0     4102 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/publish.py
--rw-r--r--   0        0        0    21301 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/release.py
--rw-r--r--   0        0        0     3344 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/report.py
--rw-r--r--   0        0        0     3521 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/run.py
--rw-r--r--   0        0        0     7789 2023-05-13 10:33:37.164056 slap_cli-1.8.1/src/slap/ext/application/test.py
--rw-r--r--   0        0        0    19021 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/application/venv.py
--rw-r--r--   0        0        0     2075 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/checks/changelog.py
--rw-r--r--   0        0        0     2215 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/checks/general.py
--rw-r--r--   0        0        0     6060 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/checks/poetry.py
--rw-r--r--   0        0        0     2812 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/checks/release.py
--rw-r--r--   0        0        0     8491 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/project_handlers/base.py
--rw-r--r--   0        0        0     3799 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/project_handlers/flit.py
--rw-r--r--   0        0        0     6462 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/project_handlers/poetry.py
--rw-r--r--   0        0        0     5751 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/project_handlers/setuptools.py
--rw-r--r--   0        0        0     1208 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/release/changelog.py
--rw-r--r--   0        0        0     2046 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/release/source_code_version.py
--rw-r--r--   0        0        0    16205 2023-05-13 17:02:56.460903 slap_cli-1.8.1/src/slap/ext/repository_ci/github_actions.py
--rw-r--r--   0        0        0     4065 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/repository_handlers/default.py
--rw-r--r--   0        0        0     4479 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/repository_hosts/github.py
--rw-r--r--   0        0        0     1357 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/ext/version_incrementing_rule.py
--rw-r--r--   0        0        0    10869 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/install/installer.py
--rw-r--r--   0        0        0     8244 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/plugins.py
--rw-r--r--   0        0        0     7835 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/project.py
--rw-r--r--   0        0        0        0 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/py.typed
--rw-r--r--   0        0        0    14965 2023-05-13 18:23:43.419460 slap_cli-1.8.1/src/slap/python/dependency.py
--rw-r--r--   0        0        0     9711 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/python/environment.py
--rw-r--r--   0        0        0     6833 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/python/pep508.py
--rw-r--r--   0        0        0     2535 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/release.py
--rw-r--r--   0        0        0     5092 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/repository.py
--rw-r--r--   0        0        0     1091 2023-05-13 18:54:04.063864 slap_cli-1.8.1/src/slap/templates/github/.github/workflows/changelog.yaml
--rw-r--r--   0        0        0      972 2023-05-13 18:53:05.709519 slap_cli-1.8.1/src/slap/templates/github/.github/workflows/python.yaml
--rw-r--r--   0        0        0      246 2023-05-13 18:23:57.759054 slap_cli-1.8.1/src/slap/templates/poetry/.flake8
--rw-r--r--   0        0        0       78 2023-05-13 17:02:56.460903 slap_cli-1.8.1/src/slap/templates/poetry/.gitignore
--rw-r--r--   0        0        0        0 2023-05-13 17:02:56.460903 slap_cli-1.8.1/src/slap/templates/poetry/LICENSE
--rw-r--r--   0        0        0        9 2023-05-13 17:02:56.460903 slap_cli-1.8.1/src/slap/templates/poetry/README.md
--rw-r--r--   0        0        0     1451 2023-05-13 17:02:56.460903 slap_cli-1.8.1/src/slap/templates/poetry/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-13 17:02:56.460903 slap_cli-1.8.1/src/slap/templates/poetry/src/{path}/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 17:02:56.460903 slap_cli-1.8.1/src/slap/templates/poetry/src/{path}/py.typed
--rw-r--r--   0        0        0       67 2023-05-13 17:02:56.460903 slap_cli-1.8.1/src/slap/templates/poetry/tests/test_import.py
--rw-r--r--   0        0        0     1847 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/util/cleo.py
--rw-r--r--   0        0        0     4309 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/util/external/licenses.py
--rw-r--r--   0        0        0     2172 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/util/external/pypi_classifiers.py
--rw-r--r--   0        0        0      418 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/util/pygments.py
--rw-r--r--   0        0        0     2113 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/util/toml_file.py
--rw-r--r--   0        0        0     7363 2023-05-13 10:33:37.168056 slap_cli-1.8.1/src/slap/util/vcs.py
--rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 slap_cli-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-01-29 11:43:11.729548 slap_cli-1.9.0/LICENSE
+-rw-r--r--   0        0        0     4974 2023-05-15 14:36:16.731931 slap_cli-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-05-15 14:36:16.731931 slap_cli-1.9.0/src/slap/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-15 14:08:15.856560 slap_cli-1.9.0/src/slap/__main__.py
+-rw-r--r--   0        0        0    12122 2023-05-15 14:33:48.748284 slap_cli-1.9.0/src/slap/application.py
+-rw-r--r--   0        0        0     9163 2023-02-09 13:39:04.453992 slap_cli-1.9.0/src/slap/changelog.py
+-rw-r--r--   0        0        0     3353 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/check.py
+-rw-r--r--   0        0        0     2520 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/configuration.py
+-rw-r--r--   0        0        0     5337 2023-05-15 13:54:26.739024 slap_cli-1.9.0/src/slap/ext/application/add.py
+-rw-r--r--   0        0        0    27292 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/ext/application/changelog.py
+-rw-r--r--   0        0        0     6330 2023-05-15 14:28:58.852972 slap_cli-1.9.0/src/slap/ext/application/check.py
+-rw-r--r--   0        0        0     3177 2023-05-15 14:02:47.957819 slap_cli-1.9.0/src/slap/ext/application/info.py
+-rw-r--r--   0        0        0     4783 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/ext/application/init.py
+-rw-r--r--   0        0        0    14309 2023-05-15 14:29:33.968869 slap_cli-1.9.0/src/slap/ext/application/install.py
+-rw-r--r--   0        0        0     5982 2023-05-15 14:16:35.467350 slap_cli-1.9.0/src/slap/ext/application/link.py
+-rw-r--r--   0        0        0     4230 2023-05-15 14:29:48.828826 slap_cli-1.9.0/src/slap/ext/application/publish.py
+-rw-r--r--   0        0        0    21667 2023-05-15 14:33:39.328295 slap_cli-1.9.0/src/slap/ext/application/release.py
+-rw-r--r--   0        0        0     3243 2023-05-15 14:30:47.388698 slap_cli-1.9.0/src/slap/ext/application/report.py
+-rw-r--r--   0        0        0     3543 2023-05-15 14:30:52.064701 slap_cli-1.9.0/src/slap/ext/application/run.py
+-rw-r--r--   0        0        0     7789 2023-05-15 14:29:06.756949 slap_cli-1.9.0/src/slap/ext/application/test.py
+-rw-r--r--   0        0        0    19880 2023-05-15 14:20:06.182817 slap_cli-1.9.0/src/slap/ext/application/venv.py
+-rw-r--r--   0        0        0     2075 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/checks/changelog.py
+-rw-r--r--   0        0        0     2215 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/checks/general.py
+-rw-r--r--   0        0        0     6060 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/checks/poetry.py
+-rw-r--r--   0        0        0     2815 2023-05-15 14:08:26.480527 slap_cli-1.9.0/src/slap/ext/checks/release.py
+-rw-r--r--   0        0        0     8491 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/project_handlers/base.py
+-rw-r--r--   0        0        0     3799 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/project_handlers/flit.py
+-rw-r--r--   0        0        0     6462 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/ext/project_handlers/poetry.py
+-rw-r--r--   0        0        0     5751 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/project_handlers/setuptools.py
+-rw-r--r--   0        0        0     1208 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/release/changelog.py
+-rw-r--r--   0        0        0     2046 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/release/source_code_version.py
+-rw-r--r--   0        0        0    16205 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/ext/repository_ci/github_actions.py
+-rw-r--r--   0        0        0     4065 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/repository_handlers/default.py
+-rw-r--r--   0        0        0     4479 2023-02-20 12:50:15.737708 slap_cli-1.9.0/src/slap/ext/repository_hosts/github.py
+-rw-r--r--   0        0        0     1357 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/version_incrementing_rule.py
+-rw-r--r--   0        0        0    10869 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/install/installer.py
+-rw-r--r--   0        0        0     8308 2023-05-15 13:52:59.875225 slap_cli-1.9.0/src/slap/plugins.py
+-rw-r--r--   0        0        0     8676 2023-05-15 13:41:13.461567 slap_cli-1.9.0/src/slap/project.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/py.typed
+-rw-r--r--   0        0        0    14965 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/python/dependency.py
+-rw-r--r--   0        0        0     9711 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/python/environment.py
+-rw-r--r--   0        0        0     6833 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/python/pep508.py
+-rw-r--r--   0        0        0     2535 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/release.py
+-rw-r--r--   0        0        0     5544 2023-05-15 14:20:02.546826 slap_cli-1.9.0/src/slap/repository.py
+-rw-r--r--   0        0        0     1091 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/github/.github/workflows/changelog.yaml
+-rw-r--r--   0        0        0      972 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/github/.github/workflows/python.yaml
+-rw-r--r--   0        0        0      246 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/.flake8
+-rw-r--r--   0        0        0       78 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/LICENSE
+-rw-r--r--   0        0        0        9 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/README.md
+-rw-r--r--   0        0        0     1451 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 13:23:04.320661 slap_cli-1.9.0/src/slap/templates/poetry/src/{path}/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:23:04.320661 slap_cli-1.9.0/src/slap/templates/poetry/src/{path}/py.typed
+-rw-r--r--   0        0        0       67 2023-05-15 13:23:04.320661 slap_cli-1.9.0/src/slap/templates/poetry/tests/test_import.py
+-rw-r--r--   0        0        0     1847 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/cleo.py
+-rw-r--r--   0        0        0     4309 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/external/licenses.py
+-rw-r--r--   0        0        0     2172 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/external/pypi_classifiers.py
+-rw-r--r--   0        0        0      418 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/pygments.py
+-rw-r--r--   0        0        0     2113 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/toml_file.py
+-rw-r--r--   0        0        0     7363 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/vcs.py
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 slap_cli-1.9.0/PKG-INFO
```

### Comparing `slap_cli-1.8.1/LICENSE` & `slap_cli-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/pyproject.toml` & `slap_cli-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "slap-cli"
-version = "1.8.1"
+version = "1.9.0"
 description = "Slap is a command-line utility for developing Python applications."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 packages = [{ include = "slap", from = "src" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
```

### Comparing `slap_cli-1.8.1/src/slap/application.py` & `slap_cli-1.9.0/src/slap/application.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ With the application object we manage the CLI commands and other types of plugins as well as access to the Slap
 user and project configuration. """
 
 from __future__ import annotations
 
 import dataclasses
 import logging
+import subprocess as sp
 import textwrap
 import typing as t
 from pathlib import Path
 
 from cleo.application import Application as BaseCleoApplication  # type: ignore[import]
 from cleo.commands.command import Command as _BaseCommand  # type: ignore[import]
 from cleo.helpers import argument, option  # type: ignore[import]
@@ -181,18 +182,16 @@
         self.main_project = Once(self._get_main_project)
 
     @property
     def repository(self) -> Repository:
         """Return the Slap repository that is the subject of the current application. There may be command plugins
         that do not require the repository to function, so this property creates the repository lazily."""
 
-        from slap.repository import Repository
-
         if self._repository is None:
-            self._repository = Repository(self._directory)
+            self._repository = find_repository(self._directory)
 
         return self._repository
 
     def _get_application_configuration(self) -> ApplicationConfig:
         """Loads the application-level configuration."""
 
         from databind.core.settings import ExtraKeys
@@ -243,21 +242,70 @@
 
         logger.debug("Loading application plugins")
 
         for plugin_name, loader in iter_entrypoints(ApplicationPlugin):  # type: ignore[misc]
             if plugin_name in disable:
                 continue
             try:
-                plugin = loader()()
+                plugin = loader()(self)
             except Exception:
                 logger.exception("Could not load plugin <subj>%s</subj> due to an exception", plugin_name)
             else:
                 plugin_config = plugin.load_configuration(self)
                 plugin.activate(self, plugin_config)
 
     def _cleo_init(self, io: IO) -> None:
         self.load_plugins()
 
     def run(self) -> None:
         """Loads and activates application plugins and then invokes the CLI."""
 
         self.cleo.run()
+
+    def get_target_projects(self) -> list[Project]:
+        """
+        Returns the list of projects that should be dealt with when executing a command. When there is a main project,
+        only the main project will be returned. When in the repository root, all projects will be returned.
+        """
+
+        main = self.main_project()
+        if main:
+            return [main]
+        if self._directory == self.repository.directory:
+            return self.repository.projects()
+        return []
+
+
+def find_repository(directory: Path) -> Repository:
+    """
+    Finds the repository for the given directory. This will search for the closest parent directory that contains a
+    `slap.toml` configuration file. If no such file exists, but we're in a Git directory, and the given *directory*
+    is not the Git root directory, then a warning is printed and the *directory* is assumed to be the Slap repository
+    root.
+    """
+
+    from slap.repository import Repository
+
+    directory = directory.resolve()
+
+    try:
+        git_root = Path(sp.check_output(["git", "rev-parse", "--show-toplevel"]).decode().strip())
+    except sp.CalledProcessError:
+        git_root = None
+
+    if git_root is not None and git_root != directory:
+        directory.relative_to(git_root)  # Raises ValueError if not a sub directory
+
+        curdir = directory
+        while True:
+            if (curdir / "slap.toml").is_file():
+                return Repository(curdir)
+            if curdir == git_root:
+                break
+            curdir = curdir.parent
+
+        logger.warning(
+            "Could not find a <subj>slap.toml</subj> configuration file in the current directory or any of its "
+            "parents. Assuming that the current directory is the Slap repository root."
+        )
+
+    return Repository(directory)
```

### Comparing `slap_cli-1.8.1/src/slap/changelog.py` & `slap_cli-1.9.0/src/slap/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/check.py` & `slap_cli-1.9.0/src/slap/check.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/configuration.py` & `slap_cli-1.9.0/src/slap/configuration.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/application/add.py` & `slap_cli-1.9.0/src/slap/ext/application/add.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/application/changelog.py` & `slap_cli-1.9.0/src/slap/ext/application/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/application/check.py` & `slap_cli-1.9.0/src/slap/ext/application/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,23 @@
         option(
             "--warnings-as-errors",
             "w",
             description="Treat warnings as errors.",
         ),
     ]
 
+    def __init__(self, app: Application) -> None:
+        Command.__init__(self)
+        ApplicationPlugin.__init__(self, app)
+
     def load_configuration(self, app: "Application") -> dict[Project, CheckConfig]:
         import databind.json
 
         result = {}
-        for project in app.repository.projects():
+        for project in app.get_target_projects():
             config = databind.json.load(project.raw_config().get("check", {}), CheckConfig)
             result[project] = config
         return result
 
     def activate(self, app: "Application", config: dict[Project, CheckConfig]) -> None:
         self.app = app
         self.config = config
@@ -62,15 +66,15 @@
 
     def handle(self) -> int:
 
         counter: t.MutableMapping[CheckResult, int] = collections.defaultdict(int)
         if self.app.repository.is_monorepo:
             for check in self._run_application_checks():
                 counter[check.result] += 1
-        for project in self.app.repository.projects():
+        for project in self.app.get_target_projects():
             if not project.is_python_project:
                 continue
             for check in self._run_project_checks(project):
                 counter[check.result] += 1
 
         if self.option("warnings-as-errors") and counter.get(Check.WARNING, 0) > 0:
             exit_code = 1
@@ -143,15 +147,15 @@
             if self.app.repository.is_monorepo:
                 self.line(f"Checks for project <info>{project.id}</info>")
                 self.line("")
             self._print_checks(checks)
             self.line("")
 
     def _run_application_checks(self) -> t.Iterable[Check]:
-        plugin_names = {p for project in self.app.repository.projects() for p in self.config[project].plugins}
+        plugin_names = {p for project in self.app.get_target_projects() for p in self.config[project].plugins}
         checks = []
         for plugin_name in sorted(plugin_names):
             plugin = load_entrypoint(CheckPlugin, plugin_name)()
             try:
                 for check in sorted(plugin.get_application_checks(self.app), key=lambda c: c.name):
                     check.name = f"{plugin_name}:{check.name}"
                     yield check
```

### Comparing `slap_cli-1.8.1/src/slap/ext/application/info.py` & `slap_cli-1.9.0/src/slap/ext/application/info.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 class InfoCommandPlugin(Command, ApplicationPlugin):
     """Show info about the Slap application workspace and the loaded projects."""
 
     app: Application
     name = "info"
 
+    def __init__(self, app: Application) -> None:
+        Command.__init__(self)
+        ApplicationPlugin.__init__(self, app)
+
     def load_configuration(self, app: Application) -> None:
         return None
 
     def activate(self, app: Application, config: None) -> None:
         self.app = app
         app.cleo.add(self)
```

### Comparing `slap_cli-1.8.1/src/slap/ext/application/init.py` & `slap_cli-1.9.0/src/slap/ext/application/init.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/application/install.py` & `slap_cli-1.9.0/src/slap/ext/application/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -197,14 +197,15 @@
         # Get a list of the projects that need to be installed that also includes all the projects required through
         # interdependencies between the projects.
         projects_plus_dependencies = (
             Stream(projects)
             .map(lambda p: p.get_interdependencies(self.app.repository.projects(), recursive=True))
             .concat()
             .append(projects)
+            .distinct()
             .collect()
         )
 
         install_extras = self._get_extras_to_install()
         discovered_extras = {"dev"}  # Not discovering a 'dev' extra should not trigger a warning
         dependencies: list[Dependency] = []
 
@@ -281,15 +282,15 @@
 
         installer = PipInstaller(self)
         status_code = installer.install(dependencies, python_environment, options)
         if status_code != 0:
             return status_code
 
         if self.option("link"):
-            self.link_project(Path(self.option("from") or "."))
+            self._link_projects(projects_plus_dependencies)
 
         return 0
 
     def _validate_args(self) -> bool:
         """Validate combinations of command-line args and options."""
 
         for a, b in [("only-extras", "extras"), ("no-root", "link"), ("only-extras", "link")]:
@@ -308,14 +309,17 @@
             if not projects:
                 self.line_error(f'error: "{only_project}" does not point to a project', "error")
                 return []
             assert len(projects) == 1, projects
             return projects
 
         else:
+            main_project = self.app.main_project()
+            if main_project:
+                return [main_project]
             if not self.app.repository.projects:
                 self.line_error("error: no projects found")
                 return []
             return self.app.repository.get_projects_ordered()
 
     def _get_extras_to_install(self) -> set[str]:
         """Return a set of the extras that should be installed."""
@@ -339,18 +343,21 @@
             spec = IndexSpec.parse(extra)
             if spec.name in indexes.urls:
                 spec.url = spec.url or indexes.urls[spec.name]
             else:
                 logger.warning('passed an --index option for a source that does not exist (source: "%s")', spec.name)
             indexes.urls[spec.name] = spec.url_with_auth
 
+    def _link_projects(self, projects: list[Project]) -> None:
+        from slap.ext.application.link import link_repository
+
+        link_repository(self.io, projects, python=get_active_python_bin(self))
+
     # SymlinkHelper
 
     def get_dependencies_for_project(self, project: Path) -> list[Dependency]:
         # TODO (@NiklasRosenstein): Implement this method
         raise NotImplementedError
 
-    def link_project(self, project: Path) -> None:
-        from slap.ext.application.link import link_repository
-
-        app = Application(project)
-        link_repository(self.io, app.repository, python=get_active_python_bin(self))
+    def link_project(self, path: Path) -> None:
+        project = self.app.repository.get_project_by_directory(path)
+        self._link_projects([project])
```

### Comparing `slap_cli-1.8.1/src/slap/ext/application/link.py` & `slap_cli-1.9.0/src/slap/ext/application/link.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import textwrap
 import typing as t
 from pathlib import Path
 
 from slap.application import IO, Application, option
 from slap.ext.application.venv import VenvAwareCommand
 from slap.plugins import ApplicationPlugin
-from slap.repository import Repository
+from slap.project import Project
 
 from .install import get_active_python_bin, python_option, venv_check
 
 
 class LinkCommandPlugin(VenvAwareCommand, ApplicationPlugin):
     """
     Symlink your Python package with the help of Flit.
@@ -87,19 +87,24 @@
         result = super().handle()
         if result != 0:
             return result
 
         if not venv_check(self, "refusing to link"):
             return 1
 
-        link_repository(self.io, self.app.repository, self.option("dump-pyproject"), get_active_python_bin(self))
+        link_repository(
+            self.io,
+            self.app.repository.get_projects_ordered(),
+            self.option("dump-pyproject"),
+            get_active_python_bin(self),
+        )
         return 0
 
 
-def link_repository(io: IO, repository: Repository, dump_pyproject: bool = False, python: str | None = None) -> None:
+def link_repository(io: IO, projects: list[Project], dump_pyproject: bool = False, python: str | None = None) -> None:
 
     from flit.install import Installer  # type: ignore[import]
     from nr.util.fs import atomic_swap
 
     from slap.util.pygments import toml_highlight
 
     # We need to pass an absolute path to Python to make sure the scripts have an absolute shebang.
@@ -108,15 +113,15 @@
         raise Exception(f"Could not find Python executable from {python_bin!r}")
 
     # Without this set, the installer will complain about installing as the root user. If we want to
     # have a similar check in Slap, we must do it in the install command as well, otherwise you end
     # up installing as root but then just the linking step fails.
     os.environ["FLIT_ROOT_INSTALL"] = "1"
 
-    for project in repository.get_projects_ordered():
+    for project in projects:
         if not project.is_python_project:
             continue
 
         packages = project.packages()
         if not packages:
             continue
```

### Comparing `slap_cli-1.8.1/src/slap/ext/application/publish.py` & `slap_cli-1.9.0/src/slap/ext/application/publish.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,18 @@
         option("client-cert", flag=False),
         # option("verbose"),
         option("disable-progress-bar"),
         option("dry", "d"),
         option("build-directory", "b", flag=False),
     ]
 
+    def __init__(self, app: Application) -> None:
+        Command.__init__(self)
+        ApplicationPlugin.__init__(self, app)
+
     def load_configuration(self, app: Application) -> None:
         return None
 
     def activate(self, app: Application, config: None) -> None:
         self.app = app
         app.cleo.add(self)
 
@@ -79,15 +83,15 @@
             executable = self.option("python")
             if not executable:
                 isolated_env = stack.enter_context(build.env.IsolatedEnvBuilder())
                 executable = isolated_env.executable
             else:
                 isolated_env = None
 
-            for project in self.app.repository.projects():
+            for project in self.app.get_target_projects():
                 if isolated_env:
                     isolated_env.install(
                         list(flatten(PipInstaller.dependency_to_pip_arguments(x) for x in project.dependencies().build))
                     )
                 if not project.is_python_project:
                     continue
```

### Comparing `slap_cli-1.8.1/src/slap/ext/application/release.py` & `slap_cli-1.9.0/src/slap/ext/application/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,17 @@
 
     <b>Push to remote</b>
 
       <u>[Git]</u>: Using the <opt>--push, -p</opt> in combination with <opt>--tag, -t</opt> will push the new
       commit and tag to the remote Git repository immediately. You can specify the
       <opt>--remote, -r</opt> option to change the remote which will be pushed to (defaults
       to "origin").
+
+    Note that this command always operates across the entire repository, even when run from inside
+    the directory of a project of a mono-repository.
     """  # noqa: E501
 
     app: Application
     config: dict[Configuration, ReleaseConfig]
 
     name = "release"
     arguments = [
@@ -130,14 +133,18 @@
             "no-branch-check", None, "Do not validate the current Git branch matches the configured release branch."
         ),
         option("no-worktree-check", None, "Do not check the worktree state."),
     ]
 
     # TODO (@NiklasRosenstein): Support "git" rule for bumping versions
 
+    def __init__(self, app: Application) -> None:
+        Command.__init__(self)
+        ApplicationPlugin.__init__(self, app)
+
     def load_configuration(self, app: Application) -> dict[Configuration, ReleaseConfig]:
         import databind.json
 
         result = {}
         for project in t.cast(list[Configuration], [app.repository] + app.repository.projects()):  # type: ignore[operator]  # noqa: E501
             data = project.raw_config().get("release", {})
             result[project] = databind.json.load(data, ReleaseConfig)
@@ -430,15 +437,18 @@
             for plugin in self._load_plugins(project):
                 version_refs += plugin.get_version_refs(project)
 
         version_refs.sort(key=lambda r: r.file)
 
         for ref in version_refs:
             if ref.file == ref.file.absolute():
-                ref.file = ref.file.relative_to(Path.cwd())
+                try:
+                    ref.file = ref.file.relative_to(Path.cwd())
+                except ValueError:
+                    pass
 
         return version_refs
 
     def handle(self) -> int:
         """Entrypoint for the command."""
 
         from nr.util.git import Git
```

### Comparing `slap_cli-1.8.1/src/slap/ext/application/report.py` & `slap_cli-1.9.0/src/slap/ext/application/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,33 +25,29 @@
             "extras",
             description="A comma-separated list of extra dependencies to include.",
             flag=False,
         ),
         option("with-license-text", description="Include license text in the output."),
     ]
 
-    def __init__(self, app: Application) -> None:
-        super().__init__()
-        self.app = app
-
     def handle(self) -> int:
         import databind.json
         import tqdm  # type: ignore[import]
 
         from slap.python.environment import DistributionGraph, PythonEnvironment, build_distribution_graph
         from slap.python.pep508 import filter_dependencies
 
         result = super().handle()
         if result != 0:
             return result
 
         extras = set(filter(bool, map(str.strip, (self.option("extras") or "").split(","))))
 
         requirements: list[Dependency] = []
-        for project in self.app.repository.projects():
+        for project in self.app.get_target_projects():
             requirements += project.dependencies().run
             if "dev" in extras:
                 requirements += project.dependencies().dev
             for extra in extras:
                 requirements += project.dependencies().extra.get(extra, [])
 
         dists_cache: dict[str, pkg_resources.Distribution | None] = {}
```

### Comparing `slap_cli-1.8.1/src/slap/ext/application/run.py` & `slap_cli-1.9.0/src/slap/ext/application/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,29 +51,29 @@
             return result
 
         main_project = self.app.main_project()
         commands_to_execute = {}
         working_dirs = {}
 
         command: list[str] = self.argument("args")
-        if command[0] in self.config:
+        if main_project and command[0] in self.config:
             command_string = self.config[command[0]] + " " + _join_args(command[1:])
             commands_to_execute[main_project.id if main_project else "/"] = command_string
             working_dirs[main_project.id if main_project else "/"] = Path.cwd()
-        else:
-            for project in self.app.repository.projects():
+        elif not main_project:
+            for project in self.app.get_target_projects():
                 config = project.raw_config().get("run", {})
                 if command[0] in config:
                     command_string = config[command[0]] + " " + _join_args(command[1:])
                     commands_to_execute[project.id] = command_string
                     working_dirs[project.id] = project.directory
 
-            if not commands_to_execute:
-                commands_to_execute["$"] = _join_args(command)
-                working_dirs["$"] = Path.cwd()
+        if not commands_to_execute:
+            commands_to_execute["$"] = _join_args(command)
+            working_dirs["$"] = Path.cwd()
 
         if len(commands_to_execute) > 1:
             level = logging.WARNING
         else:
             level = logging.INFO
 
         results = {}
```

### Comparing `slap_cli-1.8.1/src/slap/ext/application/test.py` & `slap_cli-1.9.0/src/slap/ext/application/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
     # Hack to set a default value for the flag.
     next(opt for opt in options if opt.name == "no-line-prefix")._default = NotSet.Value  # type: ignore[assignment]
 
     def load_configuration(self, app: Application) -> None:
         self.app = app
         self.tests = []
-        for project in app.repository.projects():
+        for project in app.get_target_projects():
             for test_name, command in project.raw_config().get("test", {}).items():
                 self.tests.append(Test(project, test_name, command))
 
     def activate(self, app: Application, config: None) -> None:
         app.cleo.add(self)
 
     def _select_tests(self, name: str) -> set[Test]:
```

### Comparing `slap_cli-1.8.1/src/slap/ext/application/venv.py` & `slap_cli-1.9.0/src/slap/ext/application/venv.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,14 +96,33 @@
 
     def set_last_activated(self, venv_name: str) -> None:
         state = self._get_state()
         state["last_active_environment"] = venv_name
         self._set_state(state)
 
 
+def get_venv_manager(app: Application) -> VenvManager:
+    """
+    Returns the virtual environment manager for the given project.
+    """
+
+    project = app.main_project()
+    if project is not None:
+        if not project.shared_venv:
+            return VenvManager(project.directory / ".venvs")
+    return VenvManager(app.repository.directory / ".venvs")
+
+
+def get_venv_manager_global_or_local(use_global: bool, app: Application) -> VenvManager:
+    if use_global:
+        return VenvManager(GLOBAL_VENVS_DIRECTORY)
+    else:
+        return get_venv_manager(app)
+
+
 class VenvAwareCommand(Command):
     """Base class for commands that should be aware of the active local virtual environment. Before the
     command is executed, it will check if we're currently in a virtual environment. If not, it will activate
     the environment that is considered "active" by the Slap `venv` command."""
 
     requires_venv: t.ClassVar[bool] = True
 
@@ -121,29 +140,33 @@
             description="Use the specified Slap-managed virtual environment. This can be used to run a command "
             "in a seperate environment without activating or setting it as the current environment. Note that this "
             "option can not be used to run in a globally managed environment.",
             flag=False,
         ),
     ]
 
+    def __init__(self, app: Application) -> None:
+        super().__init__()
+        self.app = app
+
     def handle(self) -> int:
         if self.option("no-venv-check"):
             return 0
         venv = get_current_venv(os.environ)
         if (self.option("ignore-active-venv") or self.option("use-venv")) and venv:
             self.line(f"<info>(venv-aware) deactivating current virtual environment (<s>{venv.path}</s>)</info>")
             venv.deactivate(os.environ)
             venv = None
         if venv:
             self.io.error_output.write_line(
                 "<info>(venv-aware) a virtual environment is already activated "
                 f'(<s>{os.environ["VIRTUAL_ENV"]}</s>)</info>'
             )
         else:
-            manager = VenvManager()
+            manager = get_venv_manager(self.app)
             if self.option("use-venv"):
                 venv = manager.get(self.option("use-venv"))
                 if not venv.exists():
                     self.io.error_output.write_line(f'<error>environment <s>"{venv.name}"</s> does not exist</error>')
                     return 1
             else:
                 venv = manager.get_last_activated()
@@ -252,14 +275,18 @@
             description="The Python executable to use to create the virtual environment. If this is not specified, "
             "it defaults to <code>python</code> + the environment name if the environment name looks like a version "
             "number (contains numbers and dots). Otehrwise, it defaults to <code>python3</code>.",
             flag=False,
         ),
     ]
 
+    def __init__(self, app: Application) -> None:
+        super().__init__()
+        self.app = app
+
     def _validate_args(self) -> bool:
         for opt in ("activate", "create", "delete", "set", "exists"):
             if self.option("init-code") and self.option(opt):
                 self.line_error(
                     f"error: <opt>-i,--init-code</opt> is not compatible with <opt>-{opt[0]},--{opt}</opt>", "error"
                 )
                 return False
@@ -343,15 +370,15 @@
         if not self._validate_args():
             return 1
 
         shell = self.option("init-code")
         if shell:
             return self._get_init_code(shell)
 
-        manager = VenvManager(GLOBAL_VENVS_DIRECTORY if self.option("global") else Path(".venvs"))
+        manager = get_venv_manager_global_or_local(self.option("global"), self.app)
 
         if self.option("list"):
             self._list_environments(manager)
             return 0
 
         python = self._get_python_bin()
         venv = manager.get(self.argument("name")) if self.argument("name") else None
@@ -449,17 +476,21 @@
         option(
             "--force",
             "-f",
             description="Overwrite the link target if it already exists.",
         ),
     ]
 
+    def __init__(self, app: Application) -> None:
+        super().__init__()
+        self.app = app
+
     def handle(self) -> int:
         location = "global" if self.option("global") else "local"
-        manager = VenvManager(GLOBAL_VENVS_DIRECTORY if self.option("global") else Path(".venvs"))
+        manager = get_venv_manager_global_or_local(self.option("global"), self.app)
         venv = manager.get(self.argument("name"))
         if not venv.exists():
             self.line_error(f'error: {location} environment <s>"{venv.name}"</s> does not exist', "error")
             return 1
 
         program = venv.get_bin(self.argument("program"))
         if not program.is_file():
@@ -484,9 +515,9 @@
 
 
 class VenvPlugin(ApplicationPlugin):
     def load_configuration(self, app: Application) -> None:
         return None
 
     def activate(self, app: Application, config: None) -> None:
-        app.cleo.add(VenvCommand())
-        app.cleo.add(VenvLinkCommand())
+        app.cleo.add(VenvCommand(app))
+        app.cleo.add(VenvLinkCommand(app))
```

### Comparing `slap_cli-1.8.1/src/slap/ext/checks/changelog.py` & `slap_cli-1.9.0/src/slap/ext/checks/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/checks/general.py` & `slap_cli-1.9.0/src/slap/ext/checks/general.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/checks/poetry.py` & `slap_cli-1.9.0/src/slap/ext/checks/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/checks/release.py` & `slap_cli-1.9.0/src/slap/ext/checks/release.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         )
 
     @check("consistent-versions")
     def check_version_number_consistency(self, app: Application) -> tuple[CheckResult, str]:
         """Checks if the version numbers in the project source code, project configuration and any other instances
         that are detected by release plugins or in the `[tool.slap.release].references` option are consistent."""
 
-        releaser = ReleaseCommandPlugin()
+        releaser = ReleaseCommandPlugin(app)
         releaser.load_configuration(app)
 
         version_refs = releaser._get_version_refs()
         cardinality = len(set(r.value for r in version_refs))
 
         if cardinality == 0:
             result = Check.WARNING
```

### Comparing `slap_cli-1.8.1/src/slap/ext/project_handlers/base.py` & `slap_cli-1.9.0/src/slap/ext/project_handlers/base.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/project_handlers/flit.py` & `slap_cli-1.9.0/src/slap/ext/project_handlers/flit.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/project_handlers/poetry.py` & `slap_cli-1.9.0/src/slap/ext/project_handlers/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/project_handlers/setuptools.py` & `slap_cli-1.9.0/src/slap/ext/project_handlers/setuptools.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/release/changelog.py` & `slap_cli-1.9.0/src/slap/ext/release/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/release/source_code_version.py` & `slap_cli-1.9.0/src/slap/ext/release/source_code_version.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/repository_ci/github_actions.py` & `slap_cli-1.9.0/src/slap/ext/repository_ci/github_actions.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/repository_handlers/default.py` & `slap_cli-1.9.0/src/slap/ext/repository_handlers/default.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/repository_hosts/github.py` & `slap_cli-1.9.0/src/slap/ext/repository_hosts/github.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/ext/version_incrementing_rule.py` & `slap_cli-1.9.0/src/slap/ext/version_incrementing_rule.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/install/installer.py` & `slap_cli-1.9.0/src/slap/install/installer.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/plugins.py` & `slap_cli-1.9.0/src/slap/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 
 
 class ApplicationPlugin(t.Generic[T], abc.ABC):
     """A plugin that is activated on application load, usually used to register additional CLI commands."""
 
     ENTRYPOINT = "slap.plugins.application"
 
+    def __init__(self, app: Application) -> None:
+        pass
+
     @abc.abstractmethod
     def load_configuration(self, app: Application) -> T:
         """Load the configuration of the plugin. Usually, plugins will want to read the configuration from the Slap
         configuration, which is either loaded from `pyproject.toml` or `slap.toml`. Use #Application.raw_config
         to access the Slap configuration."""
 
     @abc.abstractmethod
```

### Comparing `slap_cli-1.8.1/src/slap/project.py` & `slap_cli-1.9.0/src/slap/project.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,14 +54,20 @@
     #: The source directory to use when relying on automatic package detection. If not set, the default project
     #: handler will search in `"src/"`` and then `"./"``.
     source_directory: t.Annotated[str | None, Alias("source-directory")] = None
 
     #: Whether the project source code is intended to be typed.
     typed: bool | None = None
 
+    #: Whether the virtual environment for this project should be shared with other projects in the same repository.
+    #: This means that the `.venvs` folder is not checked in the project's folder, but in the repository's folder.
+    #: This is useful for monorepos and by default will be inherit from the #Repository.use_shared_venv option. For
+    #: non-mono-repos, this doesn't have any effect.
+    shared_venv: bool | None = None
+
 
 class Project(Configuration):
     """Represents one Python project. Slap can work with multiple projects at the same time, for example if the same
     repository or source code project contains multiple individual Python projects. Every project has its own
     configuration, either loaded from `slap.toml` or `pyproject.toml`."""
 
     #: Reference to the Slap application object.
@@ -204,7 +210,19 @@
     @id.setter
     def id(self, value: str) -> None:
         self._id = value
 
     @property
     def is_python_project(self) -> bool:
         return self.pyproject_toml.exists()
+
+    @property
+    def shared_venv(self) -> bool:
+        """
+        If True, the project will share the venv with the other projects from the mono repository. This takes
+        precedence over #Repository.use_shared_venv.
+        """
+
+        shared_venv = self.config().shared_venv
+        if shared_venv is None:
+            shared_venv = self.repository.use_shared_venv
+        return shared_venv
```

### Comparing `slap_cli-1.8.1/src/slap/python/dependency.py` & `slap_cli-1.9.0/src/slap/python/dependency.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/python/environment.py` & `slap_cli-1.9.0/src/slap/python/environment.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/python/pep508.py` & `slap_cli-1.9.0/src/slap/python/pep508.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/release.py` & `slap_cli-1.9.0/src/slap/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/repository.py` & `slap_cli-1.9.0/src/slap/repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,14 +88,22 @@
 
     @property
     def is_monorepo(self) -> bool:
         if len(self.projects()) > 1 or (len(self.projects()) == 1 and self.projects()[0].directory != self.directory):
             return True
         return False
 
+    @property
+    def use_shared_venv(self) -> bool:
+        """
+        If True, the virtual environment between projects in the repository should be shared.
+        """
+
+        return True
+
     def _get_repository_handler(self) -> RepositoryHandlerPlugin | None:
         """Returns the handler for this repository."""
 
         from nr.util.plugins import load_entrypoint
 
         from slap.ext.repository_handlers.default import DefaultRepositoryHandler
         from slap.plugins import RepositoryHandlerPlugin
@@ -145,7 +153,13 @@
 
         return Optional(self._handler()).map(lambda h: h.get_vcs(self)).or_else(None)
 
     def _get_repository_host(self) -> RepositoryHost | None:
         from nr.util.optional import Optional
 
         return Optional(self._handler()).map(lambda h: h.get_repository_host(self)).or_else(None)
+
+    def get_project_by_directory(self, directory: Path) -> Project:
+        for project in self.projects():
+            if project.directory == directory:
+                return project
+        raise ValueError(f"no project found for directory {directory}")
```

### Comparing `slap_cli-1.8.1/src/slap/templates/github/.github/workflows/changelog.yaml` & `slap_cli-1.9.0/src/slap/templates/github/.github/workflows/changelog.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/templates/github/.github/workflows/python.yaml` & `slap_cli-1.9.0/src/slap/templates/github/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/templates/poetry/pyproject.toml` & `slap_cli-1.9.0/src/slap/templates/poetry/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/util/cleo.py` & `slap_cli-1.9.0/src/slap/util/cleo.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/util/external/licenses.py` & `slap_cli-1.9.0/src/slap/util/external/licenses.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/util/external/pypi_classifiers.py` & `slap_cli-1.9.0/src/slap/util/external/pypi_classifiers.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/util/toml_file.py` & `slap_cli-1.9.0/src/slap/util/toml_file.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/src/slap/util/vcs.py` & `slap_cli-1.9.0/src/slap/util/vcs.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.8.1/PKG-INFO` & `slap_cli-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: slap-cli
-Version: 1.8.1
+Version: 1.9.0
 Summary: Slap is a command-line utility for developing Python applications.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=4.0)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: build (>=0.8.0,<0.9.0)
 Requires-Dist: cleo (>=1.0.0a4)
 Requires-Dist: databind (>=2.0.0,<3.0.0)
 Requires-Dist: flit (>=3.6.0,<4.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
```

