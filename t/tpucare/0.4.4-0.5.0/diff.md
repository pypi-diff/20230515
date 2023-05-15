# Comparing `tmp/tpucare-0.4.4.tar.gz` & `tmp/tpucare-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpucare-0.4.4.tar", last modified: Fri May  5 13:33:28 2023, max compression
+gzip compressed data, was "tpucare-0.5.0.tar", last modified: Mon May 15 11:20:46 2023, max compression
```

## Comparing `tpucare-0.4.4.tar` & `tpucare-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 13:33:28.412765 tpucare-0.4.4/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-05-02 17:44:22.000000 tpucare-0.4.4/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-05 13:33:28.412765 tpucare-0.4.4/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     7570 2023-05-02 17:44:22.000000 tpucare-0.4.4/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-05 13:33:28.412765 tpucare-0.4.4/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1106 2023-05-05 13:33:18.000000 tpucare-0.4.4/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 13:33:28.412765 tpucare-0.4.4/tpucare/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    11135 2023-05-05 13:33:03.000000 tpucare-0.4.4/tpucare/__init__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 13:33:28.412765 tpucare-0.4.4/tpucare.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-05 13:33:28.000000 tpucare-0.4.4/tpucare.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      170 2023-05-05 13:33:28.000000 tpucare-0.4.4/tpucare.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-05 13:33:28.000000 tpucare-0.4.4/tpucare.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-05 13:33:28.000000 tpucare-0.4.4/tpucare.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-15 11:20:46.570427 tpucare-0.5.0/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-05-02 17:44:22.000000 tpucare-0.5.0/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8385 2023-05-15 11:20:46.570427 tpucare-0.5.0/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7570 2023-05-02 17:44:22.000000 tpucare-0.5.0/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-15 11:20:46.570427 tpucare-0.5.0/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1106 2023-05-15 08:21:34.000000 tpucare-0.5.0/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-15 11:20:46.566427 tpucare-0.5.0/tpucare/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    11574 2023-05-15 08:21:42.000000 tpucare-0.5.0/tpucare/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-15 11:20:46.570427 tpucare-0.5.0/tpucare.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8385 2023-05-15 11:20:46.000000 tpucare-0.5.0/tpucare.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      170 2023-05-15 11:20:46.000000 tpucare-0.5.0/tpucare.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-15 11:20:46.000000 tpucare-0.5.0/tpucare.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-15 11:20:46.000000 tpucare-0.5.0/tpucare.egg-info/top_level.txt
```

### Comparing `tpucare-0.4.4/LICENSE` & `tpucare-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tpucare-0.4.4/PKG-INFO` & `tpucare-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tpucare
-Version: 0.4.4
+Version: 0.5.0
 Summary: Automatically take good care of your preemptible TPUs
 Home-page: https://github.com/clashluke/tpucare
 Author: Lucas Nestler
 Author-email: github.tpucare@nestler.sh
 License: BSD
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
@@ -198,7 +199,8 @@
   month        = jul,
   year         = 2022,
   publisher    = {Zenodo},
   version      = {0.0.2},
   doi          = {10.5281/zenodo.6837312},
   url          = {https://doi.org/10.5281/zenodo.6837312}
 }```
+
```

### Comparing `tpucare-0.4.4/README.md` & `tpucare-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tpucare-0.4.4/setup.py` & `tpucare-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.tpucare@nestler.sh",
     name='tpucare',
     license='BSD',
     description='Automatically take good care of your preemptible TPUs',
-    version='0.4.4',
+    version='0.5.0',
     long_description=README,
     url='https://github.com/clashluke/tpucare',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
```

### Comparing `tpucare-0.4.4/tpucare/__init__.py` & `tpucare-0.5.0/tpucare/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import subprocess
 import tempfile
 import threading
 import time
 import types
 import typing
 from contextlib import nullcontext
-from typing import Callable
+from typing import Callable, List, Optional
 
 
 def call(cmd: str) -> str:
     return subprocess.check_output(cmd.split()).rstrip().decode()
 
 
 class CallReturnError(ValueError):
@@ -50,15 +50,15 @@
 def log(*message, log_level=1e9):
     if log_level > LOG_LEVEL:
         print(f'{datetime.datetime.now()} | {" ".join(map(str, message))}', flush=True)
 
 
 def exec_command(repository: str, wandb_key: typing.Optional[str] = None, branch: str = "main",
                  setup_command: str = "(bash setup.sh; exit 0)", run_command: str = "bash run.sh",
-                 install_python: bool = True):
+                 install_python: bool = True, pkilled: Optional[List[str]] = None):
     path = repository.split('/')[-1]
     if path.endswith('.git'):
         path = path[:-len('.git')]
     script = []
     if install_python:
         script.append("sudo apt-get -o DPkg::Lock::Timeout=-1 update")
         script.append("sudo apt-get -o DPkg::Lock::Timeout=-1 --fix-missing --fix-broken install -y git python3 "
@@ -66,15 +66,24 @@
     script.append(f"(rm -rf {path} ; pkill -f python3 ; exit 0)")
     script.append(f"python3 -m pip install --upgrade pip")
     script.append(f"git clone --depth 1 --branch {branch} {repository}")
     script.append(f"cd {path}")
     if wandb_key is not None:
         script.append("python3 -m pip install --upgrade wandb typer click")
         script.append(f"/home/ubuntu/.local/bin/wandb login {wandb_key}")
-    script.extend([setup_command, f'screen -dmS model bash -c "cd {path} ; {run_command}"'])
+    script.append(setup_command)
+    start_command = f'screen -dmS model bash -c "cd {path} ; git pull ; {run_command}"'
+    script.append(start_command)
+    if pkilled is None:
+        pkilled = []
+    if pkilled:
+        pkilled = ' ; '.join(f'pkill -f {k}' for k in pkilled)
+        script.append(f"echo '{pkilled} ; sleep 30 ; {pkilled} ; {start_command} ; screen -r model' >> .bashrc")
+    else:
+        script.append(f"echo '{start_command} ; screen -r model' >> .bashrc")
     return ' &&\\\n'.join(script)
 
 
 def retry_delete(host: str, zone: str, cmd: typing.List[str], retries: int = -2):
     try:
         return retry_call(cmd, retries)
     except CallReturnError:
```

### Comparing `tpucare-0.4.4/tpucare.egg-info/PKG-INFO` & `tpucare-0.5.0/tpucare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tpucare
-Version: 0.4.4
+Version: 0.5.0
 Summary: Automatically take good care of your preemptible TPUs
 Home-page: https://github.com/clashluke/tpucare
 Author: Lucas Nestler
 Author-email: github.tpucare@nestler.sh
 License: BSD
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
@@ -198,7 +199,8 @@
   month        = jul,
   year         = 2022,
   publisher    = {Zenodo},
   version      = {0.0.2},
   doi          = {10.5281/zenodo.6837312},
   url          = {https://doi.org/10.5281/zenodo.6837312}
 }```
+
```

