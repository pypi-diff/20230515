# Comparing `tmp/kube_copilot-0.1.7.tar.gz` & `tmp/kube_copilot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kube_copilot-0.1.7.tar", max compression
+gzip compressed data, was "kube_copilot-0.1.8.tar", max compression
```

## Comparing `kube_copilot-0.1.7.tar` & `kube_copilot-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-03-25 09:21:30.419382 kube_copilot-0.1.7/LICENSE
--rw-r--r--   0        0        0    13659 2023-03-29 13:15:38.920561 kube_copilot-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-03-25 09:21:38.259064 kube_copilot-0.1.7/kube_copilot/__init__.py
--rw-r--r--   0        0        0     3699 2023-03-30 03:12:54.950641 kube_copilot-0.1.7/kube_copilot/agent.py
--rw-r--r--   0        0        0     2616 2023-03-29 12:41:27.907090 kube_copilot-0.1.7/kube_copilot/cli.py
--rw-r--r--   0        0        0      671 2023-03-25 10:47:12.857795 kube_copilot-0.1.7/kube_copilot/llm.py
--rw-r--r--   0        0        0     3164 2023-03-29 13:04:38.734591 kube_copilot-0.1.7/kube_copilot/prompts.py
--rw-r--r--   0        0        0     2022 2023-03-30 03:11:54.460130 kube_copilot-0.1.7/kube_copilot/shell.py
--rw-r--r--   0        0        0      701 2023-04-21 04:55:03.325223 kube_copilot-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    14395 1970-01-01 00:00:00.000000 kube_copilot-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-25 09:21:30.419382 kube_copilot-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3727 2023-05-15 12:57:51.606979 kube_copilot-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 09:21:38.259064 kube_copilot-0.1.8/kube_copilot/__init__.py
+-rw-r--r--   0        0        0     2759 2023-05-15 12:57:51.607506 kube_copilot-0.1.8/kube_copilot/agent.py
+-rw-r--r--   0        0        0     2275 2023-05-15 12:57:51.607927 kube_copilot-0.1.8/kube_copilot/cli.py
+-rw-r--r--   0        0        0      671 2023-03-25 10:47:12.857795 kube_copilot-0.1.8/kube_copilot/llm.py
+-rw-r--r--   0        0        0     3166 2023-05-15 12:57:51.608488 kube_copilot-0.1.8/kube_copilot/prompts.py
+-rw-r--r--   0        0        0     2022 2023-03-30 03:11:54.460130 kube_copilot-0.1.8/kube_copilot/shell.py
+-rw-r--r--   0        0        0      747 2023-05-15 12:57:51.610774 kube_copilot-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 kube_copilot-0.1.8/PKG-INFO
```

### Comparing `kube_copilot-0.1.7/LICENSE` & `kube_copilot-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.7/kube_copilot/cli.py` & `kube_copilot-0.1.8/kube_copilot/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,82 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+import logging
+import sys
 import click
 from kube_copilot.llm import init_openai
 from kube_copilot.agent import CopilotLLM
 from kube_copilot.prompts import (
     get_prompt,
     get_diagnose_prompt,
     get_audit_prompt
 )
 
 
+logging.basicConfig(stream=sys.stdout, level=logging.CRITICAL)
+logging.getLogger().addHandler(logging.StreamHandler(stream=sys.stdout))
+
+
 cmd_options = [
-    click.option("--short", is_flag=True, default=False,
-                 help="Disable verbose information of copilot execution steps"),
-    click.option("--model", default="gpt-3.5-turbo",
-                 help="OpenAI model to use for copilot execution, default is gpt-3.5-turbo"),
-    click.option("--enable-terminal", is_flag=True, default=False,
-                 help="Enable Copilot to run programs within terminal. Enable with caution since Copilot may execute inappropriate commands"),
+    click.option("--verbose", is_flag=True, default=False,
+                 help="Enable verbose information of copilot execution steps"),
+    click.option("--model", default="gpt-4",
+                 help="OpenAI model to use for copilot execution, default is gpt-4"),
 ]
 
 
 def add_options(options):
     '''Add options to a command'''
     def _add_options(func):
         for option in reversed(options):
             func = option(func)
         return func
     return _add_options
 
 
-def get_llm_chain(verbose, model, enable_terminal):
+def get_llm_chain(verbose, model):
     '''Get Copilot LLM chain'''
     init_openai()
-    return CopilotLLM(verbose=verbose, model=model, enable_terminal=enable_terminal)
+    return CopilotLLM(verbose=verbose, model=model)
 
 
 @click.group()
 @click.version_option()
 def cli():
     '''Kubernetes Copilot powered by OpenAI'''
 
 
 @cli.command(help="execute operations based on prompt instructions")
 @click.argument('instructions')
 @add_options(cmd_options)
-def execute(instructions, short, model, enable_terminal):
+def execute(instructions, verbose, model):
     '''Execute operations based on prompt instructions'''
-    if click.confirm("Copilot may generate and execute inappropriate operations steps, are you sure to continue?"):
-        chain = get_llm_chain(not short, model, enable_terminal)
-        result = chain.run(get_prompt(instructions))
-        print(result)
+    chain = get_llm_chain(verbose, model)
+    result = chain.run(get_prompt(instructions))
+    print(result)
 
 
 @cli.command(help="diagnose problems for a Pod")
 @click.argument('pod')
 @click.argument('namespace', default="default")
 @add_options(cmd_options)
-def diagnose(namespace, pod, short, model, enable_terminal):
+def diagnose(namespace, pod, verbose, model):
     '''Diagnose problems for a Pod'''
-    chain = get_llm_chain(not short, model, enable_terminal)
+    chain = get_llm_chain(verbose, model)
     result = chain.run(get_diagnose_prompt(namespace, pod))
     print(result)
 
 
 @cli.command(help="audit security issues for a Pod")
 @click.argument('pod')
 @click.argument('namespace', default="default")
 @add_options(cmd_options)
-def audit(namespace, pod, short, model, enable_terminal):
+def audit(namespace, pod, verbose, model):
     '''Audit security issues for a Pod'''
-    chain = get_llm_chain(not short, model, enable_terminal)
+    chain = get_llm_chain(verbose, model)
     result = chain.run(get_audit_prompt(namespace, pod))
     print(result)
 
 
 def main():
     '''Main function'''
     cli()
```

### Comparing `kube_copilot-0.1.7/kube_copilot/llm.py` & `kube_copilot-0.1.8/kube_copilot/llm.py`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.7/kube_copilot/prompts.py` & `kube_copilot-0.1.8/kube_copilot/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 _base_prompt = '''Follow the below instructions to complete the tasks. Please ensure
 the tasks are within Kubernetes and cloud native networking domain. If any write
-or delete operations are quired, or you are not sure on the instructions, please
+or delete operations are required, or you are not sure on the instructions, please
 invoke human tool to ask more inputs. Please only use kubectl, docker, helm or trivy
 image commands while diagnosing issues and do not try to install anything. If some tools
 are missing, just skip executing and respond the instruction steps.'''
 
 _base_diagnose_prompt = '''As a technical expert in Kubernetes and cloud native
 networking, your task is to diagnose and resolve questions and issues related to
 these technologies. You should have a deep understanding of the underlying principles
```

### Comparing `kube_copilot-0.1.7/kube_copilot/shell.py` & `kube_copilot-0.1.8/kube_copilot/shell.py`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.7/pyproject.toml` & `kube_copilot-0.1.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "kube-copilot"
-version = "0.1.7"
+version = "0.1.8"
 description = "Kubernetes Copilot"
 authors = ["Pengfei Ni <feiskyer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "kube_copilot"}]
 homepage = "https://github.com/feiskyer/kube-copilot"
 repository = "https://github.com/feiskyer/kube-copilot"
 keywords = ["kubernetes", "copilot", "openai", "chatgpt"]
 
 [tool.poetry.scripts]
 kube-copilot = 'kube_copilot.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
-langchain = ">=0.0.141"
+langchain = ">=0.0.169"
 requests = ">=2.28"
 openai = ">=0.27.4"
 tiktoken = ">=0.3.1"
+lark = "==1.1.5"
+faiss-cpu = {version = "^1"}
 google-api-python-client = ">=2.85.0"
 click = ">=8.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

