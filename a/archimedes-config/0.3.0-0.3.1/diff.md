# Comparing `tmp/archimedes_config-0.3.0.tar.gz` & `tmp/archimedes_config-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archimedes_config-0.3.0.tar", max compression
+gzip compressed data, was "archimedes_config-0.3.1.tar", max compression
```

## Comparing `archimedes_config-0.3.0.tar` & `archimedes_config-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      188 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/__init__.py
--rw-r--r--   0        0        0     8622 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/arckeyl.py
--rw-r--r--   0        0        0    13575 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/config_manager.py
--rw-r--r--   0        0        0     2308 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/keyvault_client.py
--rw-r--r--   0        0        0     1242 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/keyvault_config_manager.py
--rw-r--r--   0        0        0     1947 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/utils/path_utils.py
--rw-r--r--   0        0        0     3898 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/utils/util.py
--rw-r--r--   0        0        0      673 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/add_secrets.py
--rw-r--r--   0        0        0      965 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/lock_secrets.py
--rw-r--r--   0        0        0     2127 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/secret_creation.py
--rw-r--r--   0        0        0      944 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/unlock_secrets.py
--rw-r--r--   0        0        0     4126 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/workflow_base.py
--rw-r--r--   0        0        0      753 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      238 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/__init__.py
+-rw-r--r--   0        0        0     8543 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/arckeyl.py
+-rw-r--r--   0        0        0    13575 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/config_manager.py
+-rw-r--r--   0        0        0     2308 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/keyvault_client.py
+-rw-r--r--   0        0        0     1242 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/keyvault_config_manager.py
+-rw-r--r--   0        0        0     1613 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/utils/path_utils.py
+-rw-r--r--   0        0        0     3898 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/utils/util.py
+-rw-r--r--   0        0        0      673 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/add_secrets.py
+-rw-r--r--   0        0        0      965 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/lock_secrets.py
+-rw-r--r--   0        0        0     2127 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/secret_creation.py
+-rw-r--r--   0        0        0      944 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/unlock_secrets.py
+-rw-r--r--   0        0        0     4126 2023-05-15 08:32:42.181291 archimedes_config-0.3.1/archimedes_config/workflows/workflow_base.py
+-rw-r--r--   0        0        0      753 2023-05-15 08:32:42.185291 archimedes_config-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.3.1/PKG-INFO
```

### Comparing `archimedes_config-0.3.0/archimedes_config/arckeyl.py` & `archimedes_config-0.3.1/archimedes_config/arckeyl.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import os
 import stat
 from pathlib import Path
 
 import click
 import tomlkit
 
+from archimedes_config import CLI_COMMAND_NAME as COMMAND_NAME
 from archimedes_config.utils.path_utils import (
     clean_filename,
-    find_pyproject_directory,
     find_repo_root,
+    get_cli_exec_bin_path,
 )
 from archimedes_config.utils.util import (
     RegisteredConfigDecrypted,
     check_encrypted,
     get_registered_configs,
     get_secret,
     register_config,
@@ -23,16 +24,14 @@
     unregister_config,
 )
 from archimedes_config.workflows.add_secrets import AddSecret
 from archimedes_config.workflows.lock_secrets import LockConfig
 from archimedes_config.workflows.secret_creation import ConfigCreator
 from archimedes_config.workflows.unlock_secrets import UnlockConfig
 
-COMMAND_NAME = "arckeyl"
-
 ROOT_PATH = find_repo_root()
 
 PRE_COMMIT_CHECK_FILE_NAME = f".{COMMAND_NAME}_config"
 PRE_COMMIT_CHECK_PATH = str(ROOT_PATH / PRE_COMMIT_CHECK_FILE_NAME)
 
 SECRET_KEYS_FILE_NAME = f".{COMMAND_NAME}_secrets"
 SECRET_PATH = ROOT_PATH / SECRET_KEYS_FILE_NAME
@@ -104,16 +103,15 @@
         print("Created .gitignore and added secrets to it")
         with open(gitignore_path, "a", encoding="utf8") as file:
             file.write(f"{SECRET_KEYS_FILE_NAME}\n")
 
     # CREATE PRE-COMMIT HOOK
     pre_commit_path = ROOT_PATH / ".git" / "hooks" / "pre-commit"
     command_header = "##### ARCHIMEDES CONFIGURATION START ######\n"
-    pyproject_directory = str(find_pyproject_directory()).replace("\\", "\\\\")
-    command = f"pushd {pyproject_directory};poetry run {COMMAND_NAME} check;popd;\n"
+    command = f"{get_cli_exec_bin_path()} check;\n"
     command_tail = "##### ARCHIMEDES CONFIGURATION END ######\n"
     try:
         with open(pre_commit_path, "r", encoding="utf8") as file:
             lines = file.readlines()
         if command_header not in lines:
             lines.append(command_header)
             lines.append(command)
```

### Comparing `archimedes_config-0.3.0/archimedes_config/config_manager.py` & `archimedes_config-0.3.1/archimedes_config/config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.0/archimedes_config/keyvault_client.py` & `archimedes_config-0.3.1/archimedes_config/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.0/archimedes_config/keyvault_config_manager.py` & `archimedes_config-0.3.1/archimedes_config/keyvault_config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.0/archimedes_config/utils/path_utils.py` & `archimedes_config-0.3.1/archimedes_config/utils/path_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 """
 Utils related to path
 """
 
 import os
+import sys
 from functools import wraps
 from pathlib import Path
 
+from archimedes_config import CLI_COMMAND_NAME
 
-def find_pyproject_directory() -> str:
-    """Finds the top level directory containing pyproject.toml in the git repo"""
-    root = Path(find_repo_root())
-    current_directory = Path(os.getcwd())
-    pyproject_directories = []
-    while True:
-        if "pyproject.toml" in os.listdir(current_directory):
-            if Path(current_directory / "pyproject.toml").is_file():
-                pyproject_directories.append(current_directory)
-        if current_directory == root:
-            break
-        current_directory = current_directory.parent
-    return pyproject_directories[-1]
+
+def get_cli_exec_bin_path() -> str:
+    """Return path to cli bin executable"""
+    pyexec_path = Path(sys.executable)
+    return str(pyexec_path.parent / CLI_COMMAND_NAME).replace("\\", "/")
 
 
 def find_repo_root() -> Path:
     """Finds root directory of repo"""
 
     current_path = Path(".").absolute().resolve()
     while len(current_path.parents) > 0:
```

### Comparing `archimedes_config-0.3.0/archimedes_config/utils/util.py` & `archimedes_config-0.3.1/archimedes_config/utils/util.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.0/archimedes_config/workflows/add_secrets.py` & `archimedes_config-0.3.1/archimedes_config/workflows/add_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.0/archimedes_config/workflows/lock_secrets.py` & `archimedes_config-0.3.1/archimedes_config/workflows/lock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.0/archimedes_config/workflows/secret_creation.py` & `archimedes_config-0.3.1/archimedes_config/workflows/secret_creation.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.0/archimedes_config/workflows/unlock_secrets.py` & `archimedes_config-0.3.1/archimedes_config/workflows/unlock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.0/archimedes_config/workflows/workflow_base.py` & `archimedes_config-0.3.1/archimedes_config/workflows/workflow_base.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.0/pyproject.toml` & `archimedes_config-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archimedes-config"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["BigyaPradhan <bigya.pradhan@optimeering.com>"]
 packages = [{include = "archimedes_config"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<3.12"
 cryptography = "^39.0.1"
```

### Comparing `archimedes_config-0.3.0/PKG-INFO` & `archimedes_config-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archimedes-config
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: BigyaPradhan
 Author-email: bigya.pradhan@optimeering.com
 Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

