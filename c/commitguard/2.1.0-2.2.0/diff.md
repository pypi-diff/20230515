# Comparing `tmp/commitguard-2.1.0.tar.gz` & `tmp/commitguard-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitguard-2.1.0.tar", max compression
+gzip compressed data, was "commitguard-2.2.0.tar", max compression
```

## Comparing `commitguard-2.1.0.tar` & `commitguard-2.2.0.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0     1070 2023-05-15 12:54:01.168308 commitguard-2.1.0/LICENSE
--rw-r--r--   0        0        0     1198 2023-05-15 12:54:01.168308 commitguard-2.1.0/README.md
--rw-r--r--   0        0        0      127 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/__init__.py
--rw-r--r--   0        0        0      376 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/api/__init__.py
--rw-r--r--   0        0        0    12058 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/api/git.py
--rw-r--r--   0        0        0     1087 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/api/path.py
--rw-r--r--   0        0        0     2654 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/cli/__init__.py
--rw-r--r--   0        0        0     1869 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/cli/activate.py
--rw-r--r--   0        0        0     4669 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/cli/check.py
--rw-r--r--   0        0        0     4020 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/cli/plugins.py
--rw-r--r--   0        0        0     4823 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/config.py
--rw-r--r--   0        0        0       99 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/errors.py
--rw-r--r--   0        0        0      113 2023-05-15 12:54:01.168308 commitguard-2.1.0/commitguard/extension/__init__.py
--rw-r--r--   0        0        0     4021 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/extension/rich.py
--rw-r--r--   0        0        0     7106 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/extension/terminal.py
--rw-r--r--   0        0        0     8973 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/helper.py
--rw-r--r--   0        0        0     2765 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/hooks.py
--rw-r--r--   0        0        0       41 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/precommit/__init__.py
--rw-r--r--   0        0        0     6618 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/precommit/run.py
--rwxr-xr-x   0        0        0      354 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/precommit/template
--rw-r--r--   0        0        0        0 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/py.typed
--rw-r--r--   0        0        0     2087 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/settings.py
--rw-r--r--   0        0        0     1824 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/template.py
--rw-r--r--   0        0        0     2474 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/terminal.py
--rw-r--r--   0        0        0     2617 2023-05-15 12:54:01.172308 commitguard-2.1.0/commitguard/utils.py
--rw-r--r--   0        0        0    41668 2023-05-15 12:54:01.172308 commitguard-2.1.0/poetry.lock
--rw-r--r--   0        0        0       31 2023-05-15 12:54:01.172308 commitguard-2.1.0/poetry.toml
--rw-r--r--   0        0        0     3203 2023-05-15 12:54:01.172308 commitguard-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4063 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/api/__init__.py
--rw-r--r--   0        0        0      754 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/api/git/__init__.py
--rw-r--r--   0        0        0     1334 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/api/git/test_diff.py
--rw-r--r--   0        0        0     6538 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/api/git/test_stash.py
--rw-r--r--   0        0        0    11763 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/api/git/test_status.py
--rw-r--r--   0        0        0     2785 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/api/test_path.py
--rw-r--r--   0        0        0      987 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/api/test_terminal.py
--rw-r--r--   0        0        0        0 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/cli/__init__.py
--rw-r--r--   0        0        0     3993 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/cli/test_activate.py
--rw-r--r--   0        0        0    16467 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/cli/test_check.py
--rw-r--r--   0        0        0     6497 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/cli/test_plugins.py
--rw-r--r--   0        0        0        0 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/precommit/__init__.py
--rw-r--r--   0        0        0     1753 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/precommit/test_run.py
--rw-r--r--   0        0        0      869 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/pyproject.test1.toml
--rw-r--r--   0        0        0      145 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/pyproject.test2.toml
--rw-r--r--   0        0        0        0 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/terminal/__init__.py
--rw-r--r--   0        0        0     5893 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0     7081 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/test_config.py
--rw-r--r--   0        0        0     7369 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/test_hooks.py
--rw-r--r--   0        0        0     4875 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/test_settings.py
--rw-r--r--   0        0        0     3100 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/test_template.py
--rw-r--r--   0        0        0     2807 2023-05-15 12:54:01.172308 commitguard-2.1.0/tests/test_terminal.py
--rw-r--r--   0        0        0     7832 2023-05-15 12:54:01.176308 commitguard-2.1.0/tests/test_utils.py
--rw-r--r--   0        0        0       95 2023-05-15 12:54:01.176308 commitguard-2.1.0/tests/test_version.py
--rw-r--r--   0        0        0     2874 1970-01-01 00:00:00.000000 commitguard-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-15 13:29:22.709958 commitguard-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1198 2023-05-15 13:29:22.709958 commitguard-2.2.0/README.md
+-rw-r--r--   0        0        0      127 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/__init__.py
+-rw-r--r--   0        0        0      376 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/api/__init__.py
+-rw-r--r--   0        0        0    12058 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/api/git.py
+-rw-r--r--   0        0        0     1087 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/api/path.py
+-rw-r--r--   0        0        0     2654 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/cli/__init__.py
+-rw-r--r--   0        0        0     1869 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/cli/activate.py
+-rw-r--r--   0        0        0     4669 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/cli/check.py
+-rw-r--r--   0        0        0     4020 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/cli/plugins.py
+-rw-r--r--   0        0        0     4823 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/config.py
+-rw-r--r--   0        0        0       99 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/errors.py
+-rw-r--r--   0        0        0      113 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/extension/__init__.py
+-rw-r--r--   0        0        0     4021 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/extension/rich.py
+-rw-r--r--   0        0        0     7106 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/extension/terminal.py
+-rw-r--r--   0        0        0     8973 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/helper.py
+-rw-r--r--   0        0        0     2765 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/hooks.py
+-rw-r--r--   0        0        0       41 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/precommit/__init__.py
+-rw-r--r--   0        0        0     6618 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/precommit/run.py
+-rwxr-xr-x   0        0        0      354 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/precommit/template
+-rw-r--r--   0        0        0        0 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/py.typed
+-rw-r--r--   0        0        0     2087 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/settings.py
+-rw-r--r--   0        0        0     1824 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/template.py
+-rw-r--r--   0        0        0     2474 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/terminal.py
+-rw-r--r--   0        0        0     2617 2023-05-15 13:29:22.709958 commitguard-2.2.0/commitguard/utils.py
+-rw-r--r--   0        0        0    41668 2023-05-15 13:29:22.709958 commitguard-2.2.0/poetry.lock
+-rw-r--r--   0        0        0       31 2023-05-15 13:29:22.709958 commitguard-2.2.0/poetry.toml
+-rw-r--r--   0        0        0     3330 2023-05-15 13:29:22.709958 commitguard-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4063 2023-05-15 13:29:22.709958 commitguard-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:29:22.709958 commitguard-2.2.0/tests/api/__init__.py
+-rw-r--r--   0        0        0      754 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/api/git/__init__.py
+-rw-r--r--   0        0        0     1334 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/api/git/test_diff.py
+-rw-r--r--   0        0        0     6538 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/api/git/test_stash.py
+-rw-r--r--   0        0        0    11763 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/api/git/test_status.py
+-rw-r--r--   0        0        0     2785 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/api/test_path.py
+-rw-r--r--   0        0        0      987 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/api/test_terminal.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3993 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/cli/test_activate.py
+-rw-r--r--   0        0        0    16467 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/cli/test_check.py
+-rw-r--r--   0        0        0     6497 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/cli/test_plugins.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/precommit/__init__.py
+-rw-r--r--   0        0        0     1753 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/precommit/test_run.py
+-rw-r--r--   0        0        0      869 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/pyproject.test1.toml
+-rw-r--r--   0        0        0      145 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/pyproject.test2.toml
+-rw-r--r--   0        0        0        0 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     5893 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0     7081 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/test_config.py
+-rw-r--r--   0        0        0     7369 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/test_hooks.py
+-rw-r--r--   0        0        0     4875 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/test_settings.py
+-rw-r--r--   0        0        0     3100 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/test_template.py
+-rw-r--r--   0        0        0     2807 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/test_terminal.py
+-rw-r--r--   0        0        0     7832 2023-05-15 13:29:22.713958 commitguard-2.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2874 1970-01-01 00:00:00.000000 commitguard-2.2.0/PKG-INFO
```

### Comparing `commitguard-2.1.0/LICENSE` & `commitguard-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/README.md` & `commitguard-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/api/git.py` & `commitguard-2.2.0/commitguard/api/git.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/api/path.py` & `commitguard-2.2.0/commitguard/api/path.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/cli/__init__.py` & `commitguard-2.2.0/commitguard/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/cli/activate.py` & `commitguard-2.2.0/commitguard/cli/activate.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/cli/check.py` & `commitguard-2.2.0/commitguard/cli/check.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/cli/plugins.py` & `commitguard-2.2.0/commitguard/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/config.py` & `commitguard-2.2.0/commitguard/config.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/extension/rich.py` & `commitguard-2.2.0/commitguard/extension/rich.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/extension/terminal.py` & `commitguard-2.2.0/commitguard/extension/terminal.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/helper.py` & `commitguard-2.2.0/commitguard/helper.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/hooks.py` & `commitguard-2.2.0/commitguard/hooks.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/precommit/run.py` & `commitguard-2.2.0/commitguard/precommit/run.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/settings.py` & `commitguard-2.2.0/commitguard/settings.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/template.py` & `commitguard-2.2.0/commitguard/template.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/terminal.py` & `commitguard-2.2.0/commitguard/terminal.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/commitguard/utils.py` & `commitguard-2.2.0/commitguard/utils.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/poetry.lock` & `commitguard-2.2.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/pyproject.toml` & `commitguard-2.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "commitguard"
-version = "2.1.0"
+version = "2.2.0"
 description = "Library for managing and writing git hooks in Python using pyproject.toml for its settings ✨"
 authors = ["Yasser Tahiri <hello@yezz.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/yezz123/CommitGuard"
 repository = "https://github.com/yezz123/CommitGuard"
 
@@ -67,15 +67,21 @@
 commitguard = "commitguard.cli:main"
 
 [tool.black]
 line-length = 80
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.commitguard]
-pre-commit = []
+pre-commit = [
+  'hooks.plugins.isort',
+  'hooks.plugins.black',
+  'hooks.plugins.pylint',
+  'hooks.plugins.pytest',
+  'hooks.plugins.mypy',
+]
 mode = "poetry"
 
 [tool.isort]
 profile = "black"
 line_length = 80
 known_third_party = ["typing_extensions"]
```

### Comparing `commitguard-2.1.0/tests/__init__.py` & `commitguard-2.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/api/git/__init__.py` & `commitguard-2.2.0/tests/api/git/__init__.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/api/git/test_diff.py` & `commitguard-2.2.0/tests/api/git/test_diff.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/api/git/test_stash.py` & `commitguard-2.2.0/tests/api/git/test_stash.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/api/git/test_status.py` & `commitguard-2.2.0/tests/api/git/test_status.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/api/test_path.py` & `commitguard-2.2.0/tests/api/test_path.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/api/test_terminal.py` & `commitguard-2.2.0/tests/api/test_terminal.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/cli/test_activate.py` & `commitguard-2.2.0/tests/cli/test_activate.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/cli/test_check.py` & `commitguard-2.2.0/tests/cli/test_check.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/cli/test_plugins.py` & `commitguard-2.2.0/tests/cli/test_plugins.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/precommit/test_run.py` & `commitguard-2.2.0/tests/precommit/test_run.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/pyproject.test1.toml` & `commitguard-2.2.0/tests/pyproject.test1.toml`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/terminal/test_terminal.py` & `commitguard-2.2.0/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/test_config.py` & `commitguard-2.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/test_hooks.py` & `commitguard-2.2.0/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/test_settings.py` & `commitguard-2.2.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/test_template.py` & `commitguard-2.2.0/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/test_terminal.py` & `commitguard-2.2.0/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/tests/test_utils.py` & `commitguard-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `commitguard-2.1.0/PKG-INFO` & `commitguard-2.2.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitguard
-Version: 2.1.0
+Version: 2.2.0
 Summary: Library for managing and writing git hooks in Python using pyproject.toml for its settings ✨
 Home-page: https://github.com/yezz123/CommitGuard
 License: MIT
 Keywords: git,formatting,linting,hooks
 Author: Yasser Tahiri
 Author-email: hello@yezz.me
 Requires-Python: >=3.7.2,<4.0.0
```

