# Comparing `tmp/openshift-python-utilities-4.13.8.tar.gz` & `tmp/openshift-python-utilities-4.13.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-python-utilities-4.13.8.tar", last modified: Thu Mar 30 09:47:10 2023, max compression
+gzip compressed data, was "openshift-python-utilities-4.13.9.tar", last modified: Thu May  4 10:33:39 2023, max compression
```

## Comparing `openshift-python-utilities-4.13.8.tar` & `openshift-python-utilities-4.13.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:47:10.819367 openshift-python-utilities-4.13.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1455 2023-03-30 09:47:10.819367 openshift-python-utilities-4.13.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-30 09:47:06.000000 openshift-python-utilities-4.13.8/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:47:10.818366 openshift-python-utilities-4.13.8/ocp_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/ocp_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/ocp_utilities/debugger.py
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/ocp_utilities/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/ocp_utilities/infra.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/ocp_utilities/logger.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/ocp_utilities/must_gather.py
--rw-r--r--   0 root         (0) root         (0)     6768 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/ocp_utilities/operators.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/ocp_utilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:47:10.819367 openshift-python-utilities-4.13.8/openshift_python_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1455 2023-03-30 09:47:10.000000 openshift-python-utilities-4.13.8/openshift_python_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      495 2023-03-30 09:47:10.000000 openshift-python-utilities-4.13.8/openshift_python_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 09:47:10.000000 openshift-python-utilities-4.13.8/openshift_python_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-03-30 09:47:10.000000 openshift-python-utilities-4.13.8/openshift_python_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-30 09:47:10.000000 openshift-python-utilities-4.13.8/openshift_python_utilities.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1466 2023-03-30 09:47:05.000000 openshift-python-utilities-4.13.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 09:47:10.819367 openshift-python-utilities-4.13.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      670 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 10:33:37.000000 openshift-python-utilities-4.13.9/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/ocp_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/debugger.py
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/infra.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/must_gather.py
+-rw-r--r--   0 root         (0) root         (0)     6768 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/operators.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/ocp_utilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      471 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-04 10:33:39.000000 openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-05-04 10:33:36.000000 openshift-python-utilities-4.13.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 10:33:39.312427 openshift-python-utilities-4.13.9/setup.cfg
```

### Comparing `openshift-python-utilities-4.13.8/LICENSE` & `openshift-python-utilities-4.13.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.13.8/PKG-INFO` & `openshift-python-utilities-4.13.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-utilities
-Version: 4.13.8
+Version: 4.13.9
 Summary: A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-python-utilities
 Project-URL: Download, https://pypi.org/project/openshift-python-utilities/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-utilities/issues
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-python-utilities/blob/main/README.md
 Keywords: Openshift
```

### Comparing `openshift-python-utilities-4.13.8/README.md` & `openshift-python-utilities-4.13.9/README.md`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.13.8/ocp_utilities/debugger.py` & `openshift-python-utilities-4.13.9/ocp_utilities/debugger.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.13.8/ocp_utilities/infra.py` & `openshift-python-utilities-4.13.9/ocp_utilities/infra.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 import kubernetes
 from ocp_resources.node import Node
 from ocp_wrapper_data_collector.data_collector import (
     get_data_collector_base_dir,
     get_data_collector_dict,
 )
+from simple_logger.logger import get_logger
 from urllib3.exceptions import MaxRetryError
 
 from ocp_utilities.exceptions import (
     NodeNotReadyError,
     NodesNotHealthyConditionError,
     NodeUnschedulableError,
     PodsFailedOrPendingError,
 )
-from ocp_utilities.logger import get_logger
 
 
 LOGGER = get_logger(name=__name__)
 
 
 def get_client(config_file=None, config_dict=None, context=None, **kwargs):
     """
```

### Comparing `openshift-python-utilities-4.13.8/ocp_utilities/must_gather.py` & `openshift-python-utilities-4.13.9/ocp_utilities/must_gather.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import shlex
 
-from ocp_utilities.logger import get_logger
+from simple_logger.logger import get_logger
+
 from ocp_utilities.utils import run_command
 
 
 LOGGER = get_logger(name=__name__)
 
 
 def run_must_gather(
```

### Comparing `openshift-python-utilities-4.13.8/ocp_utilities/operators.py` & `openshift-python-utilities-4.13.9/ocp_utilities/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from ocp_resources.cluster_service_version import ClusterServiceVersion
 from ocp_resources.installplan import InstallPlan
 from ocp_resources.namespace import Namespace
 from ocp_resources.operator import Operator
 from ocp_resources.operator_group import OperatorGroup
 from ocp_resources.subscription import Subscription
 from ocp_resources.utils import TimeoutExpiredError, TimeoutSampler
+from simple_logger.logger import get_logger
 
 from ocp_utilities.infra import cluster_resource
-from ocp_utilities.logger import get_logger
 
 
 LOGGER = get_logger(name=__name__)
 TIMEOUT_5MIN = 5 * 60
 TIMEOUT_10MIN = 10 * 60
 TIMEOUT_30MIN = 30 * 60
```

### Comparing `openshift-python-utilities-4.13.8/ocp_utilities/utils.py` & `openshift-python-utilities-4.13.9/ocp_utilities/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 import subprocess
 
+from simple_logger.logger import get_logger
+
 from ocp_utilities.exceptions import CommandExecFailed
-from ocp_utilities.logger import get_logger
 
 
 LOGGER = get_logger(name=__name__)
 
 TIMEOUT_30MIN = 30 * 60
 
 
-def run_command(command, verify_stderr=True, shell=False, timeout=None):
+def run_command(
+    command,
+    verify_stderr=True,
+    shell=False,
+    timeout=None,
+    capture_output=True,
+    check=True,
+    **kwargs,
+):
     """
     Run command locally.
 
     Args:
         command (list): Command to run
         verify_stderr (bool, default True): Check command stderr
         shell (bool, default False): run subprocess with shell toggle
         timeout (int, optional): Command wait timeout
+        capture_output (bool, default False): Capture command output
+        check (boot, default True):  If check is True and the exit code was non-zero, it raises a
+            CalledProcessError
 
     Returns:
         tuple: True, out if command succeeded, False, err otherwise.
     """
     LOGGER.info(f"Running {' '.join(command)} command")
-    sub_process = subprocess.Popen(
+    sub_process = subprocess.run(
         command,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=capture_output,
+        check=check,
         shell=shell,
+        text=True,
+        timeout=timeout,
+        **kwargs,
     )
-    out, err = sub_process.communicate(timeout=timeout)
-    out_decoded = out.decode("utf-8")
-    err_decoded = err.decode("utf-8")
+    out_decoded = sub_process.stdout
+    err_decoded = sub_process.stderr
 
     error_msg = f"Failed to run {command}. rc: {sub_process.returncode}, out: {out_decoded}, error: {err_decoded}"
     if sub_process.returncode != 0:
         LOGGER.error(error_msg)
         return False, out_decoded, err_decoded
 
     # From this point and onwards we are guaranteed that sub_process.returncode == 0
```

### Comparing `openshift-python-utilities-4.13.8/openshift_python_utilities.egg-info/PKG-INFO` & `openshift-python-utilities-4.13.9/openshift_python_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-utilities
-Version: 4.13.8
+Version: 4.13.9
 Summary: A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-python-utilities
 Project-URL: Download, https://pypi.org/project/openshift-python-utilities/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-utilities/issues
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-python-utilities/blob/main/README.md
 Keywords: Openshift
```

### Comparing `openshift-python-utilities-4.13.8/pyproject.toml` & `openshift-python-utilities-4.13.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 dependencies = [
     "openshift",
     "colorlog",
     "pytest",
     "pytest-testconfig",
     "PyYAML",
     "openshift-python-wrapper-data-collector",
+    "python-simple-logger",
 ]
 dynamic = ["version"]
 # ...
 [tool.setuptools.dynamic]
 version = {file = "VERSION"}
 
 [project.readme]
```

