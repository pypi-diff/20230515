# Comparing `tmp/slap_cli-1.9.0.tar.gz` & `tmp/slap_cli-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slap_cli-1.9.0.tar", max compression
+gzip compressed data, was "slap_cli-1.9.1.tar", max compression
```

## Comparing `slap_cli-1.9.0.tar` & `slap_cli-1.9.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1002 2023-01-29 11:43:11.729548 slap_cli-1.9.0/LICENSE
--rw-r--r--   0        0        0     4974 2023-05-15 14:36:16.731931 slap_cli-1.9.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-05-15 14:36:16.731931 slap_cli-1.9.0/src/slap/__init__.py
--rw-r--r--   0        0        0      122 2023-05-15 14:08:15.856560 slap_cli-1.9.0/src/slap/__main__.py
--rw-r--r--   0        0        0    12122 2023-05-15 14:33:48.748284 slap_cli-1.9.0/src/slap/application.py
--rw-r--r--   0        0        0     9163 2023-02-09 13:39:04.453992 slap_cli-1.9.0/src/slap/changelog.py
--rw-r--r--   0        0        0     3353 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/check.py
--rw-r--r--   0        0        0     2520 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/configuration.py
--rw-r--r--   0        0        0     5337 2023-05-15 13:54:26.739024 slap_cli-1.9.0/src/slap/ext/application/add.py
--rw-r--r--   0        0        0    27292 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/ext/application/changelog.py
--rw-r--r--   0        0        0     6330 2023-05-15 14:28:58.852972 slap_cli-1.9.0/src/slap/ext/application/check.py
--rw-r--r--   0        0        0     3177 2023-05-15 14:02:47.957819 slap_cli-1.9.0/src/slap/ext/application/info.py
--rw-r--r--   0        0        0     4783 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/ext/application/init.py
--rw-r--r--   0        0        0    14309 2023-05-15 14:29:33.968869 slap_cli-1.9.0/src/slap/ext/application/install.py
--rw-r--r--   0        0        0     5982 2023-05-15 14:16:35.467350 slap_cli-1.9.0/src/slap/ext/application/link.py
--rw-r--r--   0        0        0     4230 2023-05-15 14:29:48.828826 slap_cli-1.9.0/src/slap/ext/application/publish.py
--rw-r--r--   0        0        0    21667 2023-05-15 14:33:39.328295 slap_cli-1.9.0/src/slap/ext/application/release.py
--rw-r--r--   0        0        0     3243 2023-05-15 14:30:47.388698 slap_cli-1.9.0/src/slap/ext/application/report.py
--rw-r--r--   0        0        0     3543 2023-05-15 14:30:52.064701 slap_cli-1.9.0/src/slap/ext/application/run.py
--rw-r--r--   0        0        0     7789 2023-05-15 14:29:06.756949 slap_cli-1.9.0/src/slap/ext/application/test.py
--rw-r--r--   0        0        0    19880 2023-05-15 14:20:06.182817 slap_cli-1.9.0/src/slap/ext/application/venv.py
--rw-r--r--   0        0        0     2075 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/checks/changelog.py
--rw-r--r--   0        0        0     2215 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/checks/general.py
--rw-r--r--   0        0        0     6060 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/checks/poetry.py
--rw-r--r--   0        0        0     2815 2023-05-15 14:08:26.480527 slap_cli-1.9.0/src/slap/ext/checks/release.py
--rw-r--r--   0        0        0     8491 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/project_handlers/base.py
--rw-r--r--   0        0        0     3799 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/project_handlers/flit.py
--rw-r--r--   0        0        0     6462 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/ext/project_handlers/poetry.py
--rw-r--r--   0        0        0     5751 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/project_handlers/setuptools.py
--rw-r--r--   0        0        0     1208 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/release/changelog.py
--rw-r--r--   0        0        0     2046 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/release/source_code_version.py
--rw-r--r--   0        0        0    16205 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/ext/repository_ci/github_actions.py
--rw-r--r--   0        0        0     4065 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/repository_handlers/default.py
--rw-r--r--   0        0        0     4479 2023-02-20 12:50:15.737708 slap_cli-1.9.0/src/slap/ext/repository_hosts/github.py
--rw-r--r--   0        0        0     1357 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/ext/version_incrementing_rule.py
--rw-r--r--   0        0        0    10869 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/install/installer.py
--rw-r--r--   0        0        0     8308 2023-05-15 13:52:59.875225 slap_cli-1.9.0/src/slap/plugins.py
--rw-r--r--   0        0        0     8676 2023-05-15 13:41:13.461567 slap_cli-1.9.0/src/slap/project.py
--rw-r--r--   0        0        0        0 2023-01-29 11:43:11.729548 slap_cli-1.9.0/src/slap/py.typed
--rw-r--r--   0        0        0    14965 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/python/dependency.py
--rw-r--r--   0        0        0     9711 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/python/environment.py
--rw-r--r--   0        0        0     6833 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/python/pep508.py
--rw-r--r--   0        0        0     2535 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/release.py
--rw-r--r--   0        0        0     5544 2023-05-15 14:20:02.546826 slap_cli-1.9.0/src/slap/repository.py
--rw-r--r--   0        0        0     1091 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/github/.github/workflows/changelog.yaml
--rw-r--r--   0        0        0      972 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/github/.github/workflows/python.yaml
--rw-r--r--   0        0        0      246 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/.flake8
--rw-r--r--   0        0        0       78 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/.gitignore
--rw-r--r--   0        0        0        0 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/LICENSE
--rw-r--r--   0        0        0        9 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/README.md
--rw-r--r--   0        0        0     1451 2023-05-15 13:23:04.316661 slap_cli-1.9.0/src/slap/templates/poetry/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 13:23:04.320661 slap_cli-1.9.0/src/slap/templates/poetry/src/{path}/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 13:23:04.320661 slap_cli-1.9.0/src/slap/templates/poetry/src/{path}/py.typed
--rw-r--r--   0        0        0       67 2023-05-15 13:23:04.320661 slap_cli-1.9.0/src/slap/templates/poetry/tests/test_import.py
--rw-r--r--   0        0        0     1847 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/cleo.py
--rw-r--r--   0        0        0     4309 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/external/licenses.py
--rw-r--r--   0        0        0     2172 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/external/pypi_classifiers.py
--rw-r--r--   0        0        0      418 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/pygments.py
--rw-r--r--   0        0        0     2113 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/toml_file.py
--rw-r--r--   0        0        0     7363 2023-01-29 11:43:11.733548 slap_cli-1.9.0/src/slap/util/vcs.py
--rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 slap_cli-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-01-29 11:43:11.729548 slap_cli-1.9.1/LICENSE
+-rw-r--r--   0        0        0     4981 2023-05-15 15:07:19.658323 slap_cli-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-05-15 15:07:19.658323 slap_cli-1.9.1/src/slap/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-15 14:08:15.856560 slap_cli-1.9.1/src/slap/__main__.py
+-rw-r--r--   0        0        0    12198 2023-05-15 15:00:04.087369 slap_cli-1.9.1/src/slap/application.py
+-rw-r--r--   0        0        0     9163 2023-02-09 13:39:04.453992 slap_cli-1.9.1/src/slap/changelog.py
+-rw-r--r--   0        0        0     3353 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/check.py
+-rw-r--r--   0        0        0     2533 2023-05-15 15:02:36.078985 slap_cli-1.9.1/src/slap/configuration.py
+-rw-r--r--   0        0        0     5337 2023-05-15 13:54:26.739024 slap_cli-1.9.1/src/slap/ext/application/add.py
+-rw-r--r--   0        0        0    27292 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/ext/application/changelog.py
+-rw-r--r--   0        0        0     6330 2023-05-15 14:28:58.852972 slap_cli-1.9.1/src/slap/ext/application/check.py
+-rw-r--r--   0        0        0     3177 2023-05-15 14:02:47.957819 slap_cli-1.9.1/src/slap/ext/application/info.py
+-rw-r--r--   0        0        0     4783 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/ext/application/init.py
+-rw-r--r--   0        0        0    14309 2023-05-15 14:29:33.968869 slap_cli-1.9.1/src/slap/ext/application/install.py
+-rw-r--r--   0        0        0     5982 2023-05-15 14:16:35.467350 slap_cli-1.9.1/src/slap/ext/application/link.py
+-rw-r--r--   0        0        0     4230 2023-05-15 14:29:48.828826 slap_cli-1.9.1/src/slap/ext/application/publish.py
+-rw-r--r--   0        0        0    21667 2023-05-15 14:33:39.328295 slap_cli-1.9.1/src/slap/ext/application/release.py
+-rw-r--r--   0        0        0     3243 2023-05-15 14:30:47.388698 slap_cli-1.9.1/src/slap/ext/application/report.py
+-rw-r--r--   0        0        0     3555 2023-05-15 14:59:30.475460 slap_cli-1.9.1/src/slap/ext/application/run.py
+-rw-r--r--   0        0        0     7789 2023-05-15 14:29:06.756949 slap_cli-1.9.1/src/slap/ext/application/test.py
+-rw-r--r--   0        0        0    19880 2023-05-15 14:20:06.182817 slap_cli-1.9.1/src/slap/ext/application/venv.py
+-rw-r--r--   0        0        0     2075 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/checks/changelog.py
+-rw-r--r--   0        0        0     2215 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/checks/general.py
+-rw-r--r--   0        0        0     6060 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/checks/poetry.py
+-rw-r--r--   0        0        0     2815 2023-05-15 14:08:26.480527 slap_cli-1.9.1/src/slap/ext/checks/release.py
+-rw-r--r--   0        0        0     8491 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/project_handlers/base.py
+-rw-r--r--   0        0        0     3799 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/project_handlers/flit.py
+-rw-r--r--   0        0        0     6462 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/ext/project_handlers/poetry.py
+-rw-r--r--   0        0        0     5751 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/project_handlers/setuptools.py
+-rw-r--r--   0        0        0     1208 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/release/changelog.py
+-rw-r--r--   0        0        0     2046 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/release/source_code_version.py
+-rw-r--r--   0        0        0    16205 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/ext/repository_ci/github_actions.py
+-rw-r--r--   0        0        0     4065 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/repository_handlers/default.py
+-rw-r--r--   0        0        0     4479 2023-02-20 12:50:15.737708 slap_cli-1.9.1/src/slap/ext/repository_hosts/github.py
+-rw-r--r--   0        0        0     1357 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/ext/version_incrementing_rule.py
+-rw-r--r--   0        0        0    10869 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/install/installer.py
+-rw-r--r--   0        0        0     8308 2023-05-15 13:52:59.875225 slap_cli-1.9.1/src/slap/plugins.py
+-rw-r--r--   0        0        0     8623 2023-05-15 15:05:38.122588 slap_cli-1.9.1/src/slap/project.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:43:11.729548 slap_cli-1.9.1/src/slap/py.typed
+-rw-r--r--   0        0        0    14965 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/python/dependency.py
+-rw-r--r--   0        0        0     9711 2023-01-29 11:43:11.733548 slap_cli-1.9.1/src/slap/python/environment.py
+-rw-r--r--   0        0        0     6833 2023-01-29 11:43:11.733548 slap_cli-1.9.1/src/slap/python/pep508.py
+-rw-r--r--   0        0        0     2535 2023-01-29 11:43:11.733548 slap_cli-1.9.1/src/slap/release.py
+-rw-r--r--   0        0        0     5629 2023-05-15 15:05:54.734548 slap_cli-1.9.1/src/slap/repository.py
+-rw-r--r--   0        0        0     1091 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/templates/github/.github/workflows/changelog.yaml
+-rw-r--r--   0        0        0      972 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/templates/github/.github/workflows/python.yaml
+-rw-r--r--   0        0        0      246 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/templates/poetry/.flake8
+-rw-r--r--   0        0        0       78 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/templates/poetry/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/templates/poetry/LICENSE
+-rw-r--r--   0        0        0        9 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/templates/poetry/README.md
+-rw-r--r--   0        0        0     1451 2023-05-15 13:23:04.316661 slap_cli-1.9.1/src/slap/templates/poetry/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 13:23:04.320661 slap_cli-1.9.1/src/slap/templates/poetry/src/{path}/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:23:04.320661 slap_cli-1.9.1/src/slap/templates/poetry/src/{path}/py.typed
+-rw-r--r--   0        0        0       67 2023-05-15 13:23:04.320661 slap_cli-1.9.1/src/slap/templates/poetry/tests/test_import.py
+-rw-r--r--   0        0        0     1847 2023-01-29 11:43:11.733548 slap_cli-1.9.1/src/slap/util/cleo.py
+-rw-r--r--   0        0        0     4309 2023-01-29 11:43:11.733548 slap_cli-1.9.1/src/slap/util/external/licenses.py
+-rw-r--r--   0        0        0     2172 2023-01-29 11:43:11.733548 slap_cli-1.9.1/src/slap/util/external/pypi_classifiers.py
+-rw-r--r--   0        0        0      418 2023-01-29 11:43:11.733548 slap_cli-1.9.1/src/slap/util/pygments.py
+-rw-r--r--   0        0        0     2113 2023-01-29 11:43:11.733548 slap_cli-1.9.1/src/slap/util/toml_file.py
+-rw-r--r--   0        0        0     7363 2023-01-29 11:43:11.733548 slap_cli-1.9.1/src/slap/util/vcs.py
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 slap_cli-1.9.1/PKG-INFO
```

### Comparing `slap_cli-1.9.0/LICENSE` & `slap_cli-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/pyproject.toml` & `slap_cli-1.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "slap-cli"
-version = "1.9.0"
+version = "1.9.1"
 description = "Slap is a command-line utility for developing Python applications."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 packages = [{ include = "slap", from = "src" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
@@ -113,15 +113,15 @@
 [tool.poetry.plugins."slap.plugins.repository_host"]
 github = "slap.ext.repository_hosts.github:GithubRepositoryHost"
 
 [tool.slap]
 typed = true
 
 [tool.slap.test]
-mypy   = "dmypy run src -- --namespace-packages --exclude src/slap/templates"
+mypy   = "dmypy run src"
 pytest = "pytest tests/ -vv"
 check  = "slap check"
 isort  = "isort src/ tests/ --check-only"
 black  = "black src/ tests/ --check"
 flake8 = "flake8 src/ tests/"
 
 [tool.slap.run]
@@ -134,14 +134,16 @@
 pretty = true
 warn_redundant_casts = true
 #warn_unused_ignores = true
 warn_no_return = true
 warn_unreachable = true
 show_error_context = true
 show_error_codes = true
+namespace_packages = true
+exclude = "src/slap/templates/.*"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 line_length = 120
```

### Comparing `slap_cli-1.9.0/src/slap/application.py` & `slap_cli-1.9.1/src/slap/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,19 +208,19 @@
         for project in self.repository.projects():
             path = project.directory.resolve()
             if path == cwd:
                 return project
 
         return None
 
-    def configurations(self) -> list[Configuration]:
+    def configurations(self, targets_only: bool = False) -> list[Configuration]:
         """Return a list of all configuration objects, i.e. all projects and eventually the #Repository, unless one
         project is from the same directory as the repository."""
 
-        result: list[Configuration] = list(self.repository.projects())
+        result: list[Configuration] = list(self.get_target_projects() if targets_only else self.repository.projects())
         if self.repository.directory not in tuple(p.directory for p in self.repository.projects()):
             result.insert(0, self.repository)
         return result
 
     def load_plugins(self) -> None:
         """Loads all application plugins (see #ApplicationPlugin) and activates them.
```

### Comparing `slap_cli-1.9.0/src/slap/changelog.py` & `slap_cli-1.9.1/src/slap/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/check.py` & `slap_cli-1.9.1/src/slap/check.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/configuration.py` & `slap_cli-1.9.1/src/slap/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Configuration:
     """Represents the configuration stored in a directory, which is either read from `slap.toml` or `pyproject.toml`."""
 
+    id: str
+
     #: The directory of the project. This is the directory where the `slap.toml` or `pyproject.toml` configuration
     #: would usually reside in, but the existence of neither is absolutely required.
     directory: Path
 
     #: Points to the `pyproject.toml` file in the project and can be used to conveniently check for its existence
     #: or to access its contents.
     pyproject_toml: TomlFile
```

### Comparing `slap_cli-1.9.0/src/slap/ext/application/add.py` & `slap_cli-1.9.1/src/slap/ext/application/add.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/changelog.py` & `slap_cli-1.9.1/src/slap/ext/application/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/check.py` & `slap_cli-1.9.1/src/slap/ext/application/check.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/info.py` & `slap_cli-1.9.1/src/slap/ext/application/info.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/init.py` & `slap_cli-1.9.1/src/slap/ext/application/init.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/install.py` & `slap_cli-1.9.1/src/slap/ext/application/install.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/link.py` & `slap_cli-1.9.1/src/slap/ext/application/link.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/publish.py` & `slap_cli-1.9.1/src/slap/ext/application/publish.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/release.py` & `slap_cli-1.9.1/src/slap/ext/application/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/report.py` & `slap_cli-1.9.1/src/slap/ext/application/report.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/run.py` & `slap_cli-1.9.1/src/slap/ext/application/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         command: list[str] = self.argument("args")
         if main_project and command[0] in self.config:
             command_string = self.config[command[0]] + " " + _join_args(command[1:])
             commands_to_execute[main_project.id if main_project else "/"] = command_string
             working_dirs[main_project.id if main_project else "/"] = Path.cwd()
         elif not main_project:
-            for project in self.app.get_target_projects():
+            for project in self.app.configurations(targets_only=True):
                 config = project.raw_config().get("run", {})
                 if command[0] in config:
                     command_string = config[command[0]] + " " + _join_args(command[1:])
                     commands_to_execute[project.id] = command_string
                     working_dirs[project.id] = project.directory
 
         if not commands_to_execute:
```

### Comparing `slap_cli-1.9.0/src/slap/ext/application/test.py` & `slap_cli-1.9.1/src/slap/ext/application/test.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/application/venv.py` & `slap_cli-1.9.1/src/slap/ext/application/venv.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/checks/changelog.py` & `slap_cli-1.9.1/src/slap/ext/checks/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/checks/general.py` & `slap_cli-1.9.1/src/slap/ext/checks/general.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/checks/poetry.py` & `slap_cli-1.9.1/src/slap/ext/checks/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/checks/release.py` & `slap_cli-1.9.1/src/slap/ext/checks/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/project_handlers/base.py` & `slap_cli-1.9.1/src/slap/ext/project_handlers/base.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/project_handlers/flit.py` & `slap_cli-1.9.1/src/slap/ext/project_handlers/flit.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/project_handlers/poetry.py` & `slap_cli-1.9.1/src/slap/ext/project_handlers/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/project_handlers/setuptools.py` & `slap_cli-1.9.1/src/slap/ext/project_handlers/setuptools.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/release/changelog.py` & `slap_cli-1.9.1/src/slap/ext/release/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/release/source_code_version.py` & `slap_cli-1.9.1/src/slap/ext/release/source_code_version.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/repository_ci/github_actions.py` & `slap_cli-1.9.1/src/slap/ext/repository_ci/github_actions.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/repository_handlers/default.py` & `slap_cli-1.9.1/src/slap/ext/repository_handlers/default.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/repository_hosts/github.py` & `slap_cli-1.9.1/src/slap/ext/repository_hosts/github.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/ext/version_incrementing_rule.py` & `slap_cli-1.9.1/src/slap/ext/version_incrementing_rule.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/install/installer.py` & `slap_cli-1.9.1/src/slap/install/installer.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/plugins.py` & `slap_cli-1.9.1/src/slap/plugins.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/project.py` & `slap_cli-1.9.1/src/slap/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,21 +200,17 @@
         assert isinstance(dependency, Dependency), type(dependency)
         self.handler().add_dependency(self, dependency, where)
         # TODO(@NiklasRosenstein): Use a method to flush the cache of Once when it is available in `nr.utils`.
         self.raw_config.get(True)
         self.dependencies.get(True)
 
     @property
-    def id(self) -> str:
+    def id(self) -> str:  # type: ignore[override]
         return self.dist_name() or self.directory.resolve().name
 
-    @id.setter
-    def id(self, value: str) -> None:
-        self._id = value
-
     @property
     def is_python_project(self) -> bool:
         return self.pyproject_toml.exists()
 
     @property
     def shared_venv(self) -> bool:
         """
```

### Comparing `slap_cli-1.9.0/src/slap/python/dependency.py` & `slap_cli-1.9.1/src/slap/python/dependency.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/python/environment.py` & `slap_cli-1.9.1/src/slap/python/environment.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/python/pep508.py` & `slap_cli-1.9.1/src/slap/python/pep508.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/release.py` & `slap_cli-1.9.1/src/slap/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/repository.py` & `slap_cli-1.9.1/src/slap/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,18 @@
         super().__init__(directory)
         self._handler = Once(self._get_repository_handler)
         self.projects = Once(self._get_projects)
         self.vcs = Once(self._get_vcs)
         self.host = Once(self._get_repository_host)
 
     @property
+    def id(self) -> str:  # type: ignore[override]
+        return "/"
+
+    @property
     def is_monorepo(self) -> bool:
         if len(self.projects()) > 1 or (len(self.projects()) == 1 and self.projects()[0].directory != self.directory):
             return True
         return False
 
     @property
     def use_shared_venv(self) -> bool:
```

### Comparing `slap_cli-1.9.0/src/slap/templates/github/.github/workflows/changelog.yaml` & `slap_cli-1.9.1/src/slap/templates/github/.github/workflows/changelog.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/templates/github/.github/workflows/python.yaml` & `slap_cli-1.9.1/src/slap/templates/github/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/templates/poetry/pyproject.toml` & `slap_cli-1.9.1/src/slap/templates/poetry/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/util/cleo.py` & `slap_cli-1.9.1/src/slap/util/cleo.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/util/external/licenses.py` & `slap_cli-1.9.1/src/slap/util/external/licenses.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/util/external/pypi_classifiers.py` & `slap_cli-1.9.1/src/slap/util/external/pypi_classifiers.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/util/toml_file.py` & `slap_cli-1.9.1/src/slap/util/toml_file.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/src/slap/util/vcs.py` & `slap_cli-1.9.1/src/slap/util/vcs.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.0/PKG-INFO` & `slap_cli-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slap-cli
-Version: 1.9.0
+Version: 1.9.1
 Summary: Slap is a command-line utility for developing Python applications.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

