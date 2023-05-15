# Comparing `tmp/gpt-review-0.9.0rc680.post1.tar.gz` & `tmp/gpt_review-0.9.0rc707.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.9.0rc680.post1.tar", last modified: Fri May 12 18:37:12 2023, max compression
+gzip compressed data, was "gpt_review-0.9.0rc707.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gpt-review-0.9.0rc680.post1.tar` & `gpt_review-0.9.0rc707.post1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      336 2023-05-12 18:36:57.179624 gpt-review-0.9.0rc680.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-12 18:36:57.179624 gpt-review-0.9.0rc680.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1995 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4200 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1862 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/README.md
--rw-r--r--   0        0        0     3561 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/action.yml
--rw-r--r--   0        0        0      307 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/azure.yaml.template
--rw-r--r--   0        0        0      218 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/config.summary.template.yml
--rw-r--r--   0        0        0      362 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/prompt.template.yml
--rw-r--r--   0        0        0     8500 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-12 18:37:12.499722 gpt-review-0.9.0rc680.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-12 18:37:12.499722 gpt-review-0.9.0rc680.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0     9454 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     3016 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5998 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     5981 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     3882 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0      788 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     8560 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      894 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0     2639 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/context.py
--rw-r--r--   0        0        0      924 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0       33 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/prompts/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/prompts/_prompt.py
--rw-r--r--   0        0        0      349 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/prompts/prompt_bug.yaml
--rw-r--r--   0        0        0      362 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/prompts/prompt_coverage.yaml
--rw-r--r--   0        0        0      327 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/src/gpt_review/prompts/prompt_summary.yaml
--rw-r--r--   0        0        0      218 2023-05-12 18:36:57.183625 gpt-review-0.9.0rc680.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     5421 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/mock.diff
--rw-r--r--   0        0        0      375 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/test_context.py
--rw-r--r--   0        0        0      612 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/test_git.py
--rw-r--r--   0        0        0     1443 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/test_github.py
--rw-r--r--   0        0        0     5388 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1467 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/test_report.py
--rw-r--r--   0        0        0      797 2023-05-12 18:36:57.187625 gpt-review-0.9.0rc680.post1/tests/test_review.py
--rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 gpt-review-0.9.0rc680.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1995 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4200 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1862 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.pypirc
+-rw-r--r--   0        0        0      450 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/action.yml
+-rw-r--r--   0        0        0      307 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/azure.yaml.template
+-rw-r--r--   0        0        0      218 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/config.summary.template.yml
+-rw-r--r--   0        0        0      362 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/prompt.template.yml
+-rw-r--r--   0        0        0     8500 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-15 17:55:15.908599 gpt_review-0.9.0rc707.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-15 17:55:15.908599 gpt_review-0.9.0rc707.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0     9453 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-15 17:55:09.632621 gpt_review-0.9.0rc707.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     3016 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5998 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     5981 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     3882 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0      788 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     8558 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      894 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0     2640 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/context.py
+-rw-r--r--   0        0        0      924 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      349 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/prompts/prompt_bug.yaml
+-rw-r--r--   0        0        0      362 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/prompts/prompt_coverage.yaml
+-rw-r--r--   0        0        0      327 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/src/gpt_review/prompts/prompt_summary.yaml
+-rw-r--r--   0        0        0      218 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     5421 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/mock.diff
+-rw-r--r--   0        0        0      375 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/test_context.py
+-rw-r--r--   0        0        0      612 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1443 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5388 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1467 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/test_report.py
+-rw-r--r--   0        0        0      797 2023-05-15 17:55:09.636621 gpt_review-0.9.0rc707.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 gpt_review-0.9.0rc707.post1/PKG-INFO
```

### Comparing `gpt-review-0.9.0rc680.post1/.devcontainer/devcontainer.json` & `gpt_review-0.9.0rc707.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt_review-0.9.0rc707.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.github/dependabot.yml` & `gpt_review-0.9.0rc707.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.github/pull_request_template.md` & `gpt_review-0.9.0rc707.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.github/workflows/codeql.yml` & `gpt_review-0.9.0rc707.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.github/workflows/dependency-review.yml` & `gpt_review-0.9.0rc707.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt_review-0.9.0rc707.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.github/workflows/python.yml` & `gpt_review-0.9.0rc707.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.github/workflows/test-action.yml` & `gpt_review-0.9.0rc707.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.gitignore` & `gpt_review-0.9.0rc707.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/.vscode/settings.json` & `gpt_review-0.9.0rc707.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/LICENSE` & `gpt_review-0.9.0rc707.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/README.md` & `gpt_review-0.9.0rc707.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/action.yml` & `gpt_review-0.9.0rc707.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/pyproject.toml` & `gpt_review-0.9.0rc707.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/_ask.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/_ask.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from typing import Dict, List, Optional
 
 from knack import CLICommandsLoader
 from knack.arguments import ArgumentsContext
 from knack.commands import CommandGroup
 from knack.util import CLIError
 
-
+import gpt_review.constants as C
 from gpt_review._command import GPTCommandGroup
 from gpt_review._llama_index import _query_index
 from gpt_review._openai import _call_gpt
-import gpt_review.constants as C
 from gpt_review.context import _load_azure_openai_context
 
 
 def validate_parameter_range(namespace) -> None:
     """
     Validate the following parameters:
     - max_tokens is in [1,4000]
```

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/_git.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/_git.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Basic Shell Commands for Git."""
 import logging
 import os
 from typing import Dict
 
+from git.repo import Repo
 from knack import CLICommandsLoader
 from knack.arguments import ArgumentsContext
 from knack.commands import CommandGroup
-from git.repo import Repo
 
 from gpt_review._command import GPTCommandGroup
 from gpt_review._review import _request_goal
 
 
 def _find_git_dir(path=".") -> str:
     """
```

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/_github.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/_github.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """GitHub API helpers."""
-import logging
 import json
+import logging
 import os
 from typing import Dict
 
 import requests
-from knack.arguments import ArgumentsContext
 from knack import CLICommandsLoader
+from knack.arguments import ArgumentsContext
 from knack.commands import CommandGroup
 
 from gpt_review._command import GPTCommandGroup
-from gpt_review._review import _summarize_files
 from gpt_review._repository import _RepositoryClient
+from gpt_review._review import _summarize_files
 
 
 class _GitHubClient(_RepositoryClient):
     """GitHub client."""
 
     @staticmethod
     def get_pr_diff(patch_repo=None, patch_pr=None, access_token=None) -> str:
```

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/_gpt_cli.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/_gpt_cli.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The GPT CLI configuration and utilities."""
-from collections import OrderedDict
 import os
 import sys
+from collections import OrderedDict
 
 from knack import CLI, CLICommandsLoader
 
 from gpt_review import __version__
 from gpt_review._ask import AskCommandGroup
 from gpt_review._git import GitCommandGroup
 from gpt_review._github import GitHubCommandGroup
```

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/_llama_index.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/_llama_index.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Wrapper for Llama Index."""
 import logging
 import os
 from typing import List, Optional
-from typing_extensions import override
 
 import openai
 from langchain.chat_models import AzureChatOpenAI
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.llms import AzureOpenAI
 from llama_index import (
     Document,
     GithubRepositoryReader,
     GPTVectorStoreIndex,
-    LLMPredictor,
     LangchainEmbedding,
+    LLMPredictor,
     ServiceContext,
     SimpleDirectoryReader,
     StorageContext,
     load_index_from_storage,
 )
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.storage.storage_context import DEFAULT_PERSIST_DIR
+from typing_extensions import override
 
 import gpt_review.constants as C
 from gpt_review.context import _load_azure_openai_context
 
 logger = logging.getLogger(__name__)
```

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/_openai.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/_repository.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/_review.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Basic functions for requesting review based goals from GPT-4."""
 import os
 from dataclasses import dataclass
 from typing import Dict
 
 import yaml
-
-from knack.arguments import ArgumentsContext
 from knack import CLICommandsLoader
+from knack.arguments import ArgumentsContext
 from knack.commands import CommandGroup
 
 from gpt_review._ask import _ask
 from gpt_review._command import GPTCommandGroup
 from gpt_review.prompts._prompt import load_bug_yaml, load_coverage_yaml, load_summary_yaml
 
-
 _CHECKS = {
     "SUMMARY_CHECKS": [
         {
             "flag": "SUMMARY_SUGGEST",
             "header": "Suggestions",
             "goal": "Any suggestions for improving the changes in this PR?",
         },
```

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/constants.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/context.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Context for the Azure OpenAI API and the models."""
 import os
 from dataclasses import dataclass
-from azure.identity import DefaultAzureCredential
-from azure.keyvault.secrets import SecretClient
+
 import openai
 import yaml
+from azure.identity import DefaultAzureCredential
+from azure.keyvault.secrets import SecretClient
 
 import gpt_review.constants as C
 
 DEFAULT_KEY_VAULT = "https://dciborow-openai.vault.azure.net/"
 
 
 @dataclass
```

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/main.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/src/gpt_review/prompts/_prompt.py` & `gpt_review-0.9.0rc707.post1/src/gpt_review/prompts/_prompt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Interface for a GPT Prompts."""
 import os
 import sys
-from pathlib import Path
 from dataclasses import dataclass
+from pathlib import Path
 
-from langchain.prompts import load_prompt, PromptTemplate
+from langchain.prompts import PromptTemplate, load_prompt
 
 import gpt_review.constants as C
 
 if sys.version_info[:2] <= (3, 10):
     from typing_extensions import Self
 else:
     from typing import Self
```

### Comparing `gpt-review-0.9.0rc680.post1/tests/conftest.py` & `gpt_review-0.9.0rc707.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/tests/mock.diff` & `gpt_review-0.9.0rc707.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/tests/test_git.py` & `gpt_review-0.9.0rc707.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/tests/test_github.py` & `gpt_review-0.9.0rc707.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/tests/test_gpt_cli.py` & `gpt_review-0.9.0rc707.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/tests/test_llama_index.py` & `gpt_review-0.9.0rc707.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/tests/test_openai.py` & `gpt_review-0.9.0rc707.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/tests/test_report.py` & `gpt_review-0.9.0rc707.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/tests/test_review.py` & `gpt_review-0.9.0rc707.post1/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.9.0rc680.post1/PKG-INFO` & `gpt_review-0.9.0rc707.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.9.0rc680.post1
+Version: 0.9.0rc707.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.9.0rc680.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.9.0rc707.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

