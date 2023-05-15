# Comparing `tmp/commitguard-1.0.0.tar.gz` & `tmp/commitguard-2.0.0.tar.gz`

## Comparing `commitguard-1.0.0.tar` & `commitguard-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,64 @@
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 commitguard-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 commitguard-1.0.0/.github/CODEOWNERS
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 commitguard-1.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 commitguard-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 commitguard-1.0.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 commitguard-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 commitguard-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 commitguard-1.0.0/commitguard/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 commitguard-1.0.0/scripts/clean.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 commitguard-1.0.0/scripts/format.sh
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 commitguard-1.0.0/scripts/lint.sh
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 commitguard-1.0.0/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commitguard-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 commitguard-1.0.0/tests/test_version.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 commitguard-1.0.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 commitguard-1.0.0/LICENSE
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 commitguard-1.0.0/README.md
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 commitguard-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 commitguard-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 commitguard-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 commitguard-2.0.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 commitguard-2.0.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 commitguard-2.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 commitguard-2.0.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 commitguard-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 commitguard-2.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/__init__.py
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/config.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/errors.py
+-rw-r--r--   0        0        0     8961 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/helper.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/py.typed
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/settings.py
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/template.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/terminal.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/utils.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/api/__init__.py
+-rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/api/git.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/api/path.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/cli/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/cli/activate.py
+-rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/cli/check.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/cli/plugins.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/extension/__init__.py
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/extension/rich.py
+-rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/extension/terminal.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/precommit/__init__.py
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/precommit/run.py
+-rwxr-xr-x   0        0        0      354 2020-02-02 00:00:00.000000 commitguard-2.0.0/commitguard/precommit/template
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 commitguard-2.0.0/scripts/clean.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 commitguard-2.0.0/scripts/format.sh
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 commitguard-2.0.0/scripts/lint.sh
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 commitguard-2.0.0/scripts/test.sh
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/pyproject.test1.toml
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/pyproject.test2.toml
+-rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/test_config.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/test_hooks.py
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/test_settings.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/test_template.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/test_terminal.py
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/api/__init__.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/api/test_path.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/api/test_terminal.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/api/git/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/api/git/test_diff.py
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/api/git/test_stash.py
+-rw-r--r--   0        0        0    11403 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/api/git/test_status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/cli/test_activate.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/cli/test_check.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/cli/test_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/precommit/__init__.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/precommit/test_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 commitguard-2.0.0/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 commitguard-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 commitguard-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 commitguard-2.0.0/README.md
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 commitguard-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 commitguard-2.0.0/PKG-INFO
```

### Comparing `commitguard-1.0.0/.pre-commit-config.yaml` & `commitguard-2.0.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,11 @@
         - --keep-runtime-typing
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: v0.0.267
     hooks:
     -   id: ruff
         args:
         - --fix
--   repo: https://github.com/pycqa/isort
-    rev: 5.12.0
-    hooks:
-    -   id: isort
-        name: isort (python)
 -   repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     -   id: black
```

### Comparing `commitguard-1.0.0/.github/workflows/lint.yml` & `commitguard-2.0.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `commitguard-1.0.0/.github/workflows/release.yml` & `commitguard-2.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `commitguard-1.0.0/.github/workflows/test.yml` & `commitguard-2.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `commitguard-1.0.0/scripts/clean.sh` & `commitguard-2.0.0/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `commitguard-1.0.0/.gitignore` & `commitguard-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `commitguard-1.0.0/LICENSE` & `commitguard-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitguard-1.0.0/pyproject.toml` & `commitguard-2.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,40 +7,52 @@
 description = "Library for managing and writing git hooks in Python using pyproject.toml for its settings ✨"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 authors = [
     { name = "Yasser Tahiri", email = "hello@yezz.me" },
 ]
+keywords = [
+    "git",
+    "hooks",
+    "pre-commit",
+    "commit",
+]
 
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
-    "Framework :: Pydantic",
     "Environment :: Console",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Software Development :: Version Control :: Git",
     "Typing :: Typed",
 ]
 
 dependencies = [
     "typing-extensions >=3.7.4,<4.6.0",
-    "pydantic >=1.6.2,!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0",
-    "email-validator>=1.3.0",
+    "colorful >=0.5.4,<0.6.0",
+    "httpx[http2] >=0.24.0,<1.0.0",
+    "rich >=13.0.0,<20.0.0",
+    "tomlkit >=0.5.11",
 ]
 
 dynamic = ["version"]
 
+[project.scripts]
+cli-name = "commitguard.cli:main"
+
 [project.urls]
 Homepage = "https://github.com/yezz123/CommitGuard"
 Funding = 'https://github.com/sponsors/yezz123'
 
 [project.optional-dependencies]
 lint = [
     "pre-commit==3.3.1",
@@ -54,25 +66,25 @@
 ]
 docs = [
     "mkdocs >=1.1.2,<2.0.0",
     "mkdocs-material >=8.1.4,<10.0.0",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
     "mkdocs-mermaid2-plugin==0.6.0",
-    "markdown-include==0.8.0",
-    "pymdown-extensions==9.9.2",
+    "markdown-include==0.8.1",
+    "pymdown-extensions==9.11",
     "jinja2==3.1.2"
 ]
 
 [tool.hatch.version]
 path = "commitguard/__init__.py"
 
 [tool.isort]
 profile = "black"
-known_third_party = ["pydantic", "typing_extensions"]
+known_third_party = ["typing_extensions"]
 
 [tool.ruff]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
@@ -85,26 +97,19 @@
     "C901",  # too complex
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.isort]
-known-third-party = ["pydantic", "typing_extensions"]
+known-third-party = ["typing_extensions"]
 
 [tool.mypy]
-plugins = "pydantic.mypy"
-follow_imports = "silent"
-strict_optional = true
-warn_redundant_casts = true
-warn_unused_ignores = true
-disallow_any_generics = true
-check_untyped_defs = true
 ignore_missing_imports = true
-disallow_untyped_defs = true
+explicit_package_bases = true
 
 [[tool.mypy.overrides]]
 module = "commitguard.tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [tool.coverage.report]
@@ -121,7 +126,11 @@
 [tool.pytest]
 testpaths = "tests/"
 log_cli = "1"
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format= "%Y-%m-%d %H:%M:%S"
 asyncio_mode= "auto"
+
+[tool.commitguard]
+mode = "pythonpath"
+pre-commit = []
```

