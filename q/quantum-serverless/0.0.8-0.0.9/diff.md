# Comparing `tmp/quantum_serverless-0.0.8.tar.gz` & `tmp/quantum_serverless-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.0.8.tar", last modified: Tue May  9 19:36:47 2023, max compression
+gzip compressed data, was "quantum_serverless-0.0.9.tar", last modified: Mon May 15 18:38:21 2023, max compression
```

## Comparing `quantum_serverless-0.0.8.tar` & `quantum_serverless-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.088641 quantum_serverless-0.0.8/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/serializers/program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/test_program_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/serializers/test_program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.834397 quantum_serverless-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-15 18:38:21.834397 quantum_serverless-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.830397 quantum_serverless-0.0.9/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.830397 quantum_serverless-0.0.9/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/core/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.830397 quantum_serverless-0.0.9/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.830397 quantum_serverless-0.0.9/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.830397 quantum_serverless-0.0.9/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/quantum_serverless/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.830397 quantum_serverless-0.0.9/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-15 18:38:21.000000 quantum_serverless-0.0.9/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-15 18:38:21.000000 quantum_serverless-0.0.9/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:38:21.000000 quantum_serverless-0.0.9/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-15 18:38:21.000000 quantum_serverless-0.0.9/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 18:38:21.000000 quantum_serverless-0.0.9/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 18:38:21.834397 quantum_serverless-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.830397 quantum_serverless-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.834397 quantum_serverless-0.0.9/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/core/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/core/test_program_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/core/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.834397 quantum_serverless-0.0.9/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:21.834397 quantum_serverless-0.0.9/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-15 18:38:12.000000 quantum_serverless-0.0.9/tests/utils.py
```

### Comparing `quantum_serverless-0.0.8/PKG-INFO` & `quantum_serverless-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum_serverless
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.0.8/README.md` & `quantum_serverless-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/__init__.py` & `quantum_serverless-0.0.9/quantum_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/core/__init__.py` & `quantum_serverless-0.0.9/quantum_serverless/core/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/core/constants.py` & `quantum_serverless-0.0.9/quantum_serverless/core/constants.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/core/decorators.py` & `quantum_serverless-0.0.9/quantum_serverless/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/core/events.py` & `quantum_serverless-0.0.9/quantum_serverless/core/events.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/core/job.py` & `quantum_serverless-0.0.9/quantum_serverless/core/job.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     RuntimeEnv
     Job
 """
 import json
 import logging
 import os
 import tarfile
-from typing import Dict, Any, Optional
+from typing import Dict, Any, Optional, List
 from uuid import uuid4
 
 import ray.runtime_env
 import requests
 from ray.dashboard.modules.job.sdk import JobSubmissionClient
 
 from quantum_serverless.core.constants import (
@@ -44,30 +44,37 @@
     ENV_JOB_GATEWAY_TOKEN,
     ENV_JOB_GATEWAY_HOST,
     ENV_JOB_ID_GATEWAY,
     ENV_GATEWAY_PROVIDER_VERSION,
     GATEWAY_PROVIDER_VERSION_DEFAULT,
 )
 from quantum_serverless.core.program import Program
-from quantum_serverless.exception import QuantumServerlessException
 from quantum_serverless.serializers.program_serializers import QiskitObjectsEncoder
-from quantum_serverless.utils.json import is_jsonable
+from quantum_serverless.utils.json import is_jsonable, safe_json_request
 
 RuntimeEnv = ray.runtime_env.RuntimeEnv
 
 
 class BaseJobClient:
     """Base class for Job clients."""
 
     def run_program(
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> "Job":
         """Runs program."""
         raise NotImplementedError
 
+    def get(self, job_id) -> Optional["Job"]:
+        """Returns job by job id"""
+        raise NotImplementedError
+
+    def list(self, **kwargs) -> List["Job"]:
+        """Returns list of jobs."""
+        raise NotImplementedError
+
     def status(self, job_id: str):
         """Check status."""
         raise NotImplementedError
 
     def stop(self, job_id: str):
         """Stops job/program."""
         raise NotImplementedError
@@ -101,14 +108,22 @@
 
     def logs(self, job_id: str):
         return self._job_client.get_job_logs(job_id)
 
     def result(self, job_id: str):
         return self.logs(job_id)
 
+    def get(self, job_id) -> Optional["Job"]:
+        return Job(self._job_client.get_job_info(job_id).job_id, job_client=self)
+
+    def list(self, **kwargs) -> List["Job"]:
+        return [
+            Job(job.job_id, job_client=self) for job in self._job_client.list_jobs()
+        ]
+
     def run_program(self, program: Program, arguments: Optional[Dict[str, Any]] = None):
         arguments = arguments or {}
         arguments_string = ""
         if program.arguments is not None:
             arg_list = []
             for key, value in arguments.items():
                 if isinstance(value, dict):
@@ -147,112 +162,124 @@
             version: gateway version
             token: authorization token
         """
         self.host = host
         self.version = version
         self._token = token
 
-    def run_program(
+    def run_program(  # pylint: disable=too-many-locals
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> "Job":
         url = f"{self.host}/api/{self.version}/programs/run/"
         artifact_file_path = os.path.join(program.working_dir, "artifact.tar")
 
         with tarfile.open(artifact_file_path, "w") as tar:
             for filename in os.listdir(program.working_dir):
                 fpath = os.path.join(program.working_dir, filename)
                 tar.add(fpath, arcname=filename)
 
         with open(artifact_file_path, "rb") as file:
-            response = requests.post(
-                url=url,
-                data={
-                    "title": program.title,
-                    "entrypoint": program.entrypoint,
-                    "arguments": json.dumps(arguments or {}, cls=QiskitObjectsEncoder),
-                    "dependencies": json.dumps(program.dependencies or []),
-                },
-                files={"artifact": file},
-                headers={"Authorization": f"Bearer {self._token}"},
-                timeout=REQUESTS_TIMEOUT,
-            )
-            if not response.ok:
-                raise QuantumServerlessException(
-                    f"Something went wrong with program execution. {response.text}"
+            response_data = safe_json_request(
+                request=lambda: requests.post(
+                    url=url,
+                    data={
+                        "title": program.title,
+                        "entrypoint": program.entrypoint,
+                        "arguments": json.dumps(
+                            arguments or {}, cls=QiskitObjectsEncoder
+                        ),
+                        "dependencies": json.dumps(program.dependencies or []),
+                    },
+                    files={"artifact": file},
+                    headers={"Authorization": f"Bearer {self._token}"},
+                    timeout=REQUESTS_TIMEOUT,
                 )
-
-            json_response = json.loads(response.text)
-            job_id = json_response.get("id")
+            )
+            job_id = response_data.get("id")
 
         if os.path.exists(artifact_file_path):
             os.remove(artifact_file_path)
 
         return Job(job_id, job_client=self)
 
     def status(self, job_id: str):
         default_status = "Unknown"
-        status = default_status
-        response = requests.get(
-            f"{self.host}/api/{self.version}/jobs/{job_id}/",
-            headers={"Authorization": f"Bearer {self._token}"},
-            timeout=REQUESTS_TIMEOUT,
-        )
-        if response.ok:
-            status = json.loads(response.text).get("status", default_status)
-        else:
-            logging.warning(
-                "Something went wrong during job status fetching. %s", response.text
+        response_data = safe_json_request(
+            request=lambda: requests.get(
+                f"{self.host}/api/{self.version}/jobs/{job_id}/",
+                headers={"Authorization": f"Bearer {self._token}"},
+                timeout=REQUESTS_TIMEOUT,
             )
-        return status
+        )
+
+        return response_data.get("status", default_status)
 
     def stop(self, job_id: str):
-        message = ""
-        response = requests.post(
-            f"{self.host}/api/{self.version}/jobs/{job_id}/stop/",
-            headers={"Authorization": f"Bearer {self._token}"},
-            timeout=REQUESTS_TIMEOUT,
-        )
-        if response.ok:
-            message = json.loads(response.text).get("message", None)
-        else:
-            logging.warning(
-                "Something went wrong during job stopping. %s", response.text
+        response_data = safe_json_request(
+            request=lambda: requests.post(
+                f"{self.host}/api/{self.version}/jobs/{job_id}/stop/",
+                headers={"Authorization": f"Bearer {self._token}"},
+                timeout=REQUESTS_TIMEOUT,
             )
-        return message
+        )
+
+        return response_data.get("message")
 
     def logs(self, job_id: str):
-        result = None
-        response = requests.get(
-            f"{self.host}/api/{self.version}/jobs/{job_id}/logs/",
-            headers={"Authorization": f"Bearer {self._token}"},
-            timeout=REQUESTS_TIMEOUT,
-        )
-        if response.ok:
-            result = json.loads(response.text).get("logs", None)
-        else:
-            logging.warning(
-                "Something went wrong during job result fetching. %s", response.text
+        response_data = safe_json_request(
+            request=lambda: requests.get(
+                f"{self.host}/api/{self.version}/jobs/{job_id}/logs/",
+                headers={"Authorization": f"Bearer {self._token}"},
+                timeout=REQUESTS_TIMEOUT,
             )
-        return result
+        )
+        return response_data.get("logs")
 
     def result(self, job_id: str):
-        result = None
-        response = requests.get(
-            f"{self.host}/api/{self.version}/jobs/{job_id}/",
-            headers={"Authorization": f"Bearer {self._token}"},
-            timeout=REQUESTS_TIMEOUT,
-        )
-        if response.ok:
-            json_result = json.loads(response.text).get("result", "{}")
-            result = json.loads(json_result or "{}")
-        else:
-            logging.warning(
-                "Something went wrong during job result fetching. %s", response.text
+        response_data = safe_json_request(
+            request=lambda: requests.get(
+                f"{self.host}/api/{self.version}/jobs/{job_id}/",
+                headers={"Authorization": f"Bearer {self._token}"},
+                timeout=REQUESTS_TIMEOUT,
+            )
+        )
+        return json.loads(response_data.get("result", "{}") or "{}")
+
+    def get(self, job_id) -> Optional["Job"]:
+        url = f"{self.host}/api/{self.version}/jobs/{job_id}/"
+        response_data = safe_json_request(
+            request=lambda: requests.get(
+                url,
+                headers={"Authorization": f"Bearer {self._token}"},
+                timeout=REQUESTS_TIMEOUT,
             )
-        return result
+        )
+
+        job = None
+        job_id = response_data.get("id")
+        if job_id is not None:
+            job = Job(
+                job_id=response_data.get("id"),
+                job_client=self,
+            )
+
+        return job
+
+    def list(self, **kwargs) -> List["Job"]:
+        response_data = safe_json_request(
+            request=lambda: requests.get(
+                f"{self.host}/api/{self.version}/jobs/",
+                headers={"Authorization": f"Bearer {self._token}"},
+                timeout=REQUESTS_TIMEOUT,
+            )
+        )
+        return [
+            Job(job.get("id"), job_client=self)
+            for job in response_data.get("results", [])
+        ]
 
 
 class Job:
     """Job."""
 
     def __init__(self, job_id: str, job_client: BaseJobClient):
         """Job class for async script execution.
```

### Comparing `quantum_serverless-0.0.8/quantum_serverless/core/program.py` & `quantum_serverless-0.0.9/quantum_serverless/core/program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/core/provider.py` & `quantum_serverless-0.0.9/quantum_serverless/core/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 .. autosummary::
     :toctree: ../stubs/
 
     ComputeResource
     Provider
 """
-import json
 import logging
 import os.path
 from dataclasses import dataclass
 from typing import Optional, List, Dict, Any
 
 import ray
 import requests
@@ -49,14 +48,15 @@
     GatewayJobClient,
     BaseJobClient,
 )
 from quantum_serverless.core.program import Program
 from quantum_serverless.core.tracing import _trace_env_vars
 from quantum_serverless.exception import QuantumServerlessException
 from quantum_serverless.utils import JsonSerializable
+from quantum_serverless.utils.json import safe_json_request
 
 TIMEOUT = 30
 
 
 @dataclass
 class ComputeResource:
     """ComputeResource class.
@@ -479,14 +479,15 @@
         self,
         name: Optional[str] = None,
         host: Optional[str] = None,
         version: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
         token: Optional[str] = None,
+        verbose: bool = False,
     ):
         """GatewayProvider.
 
         Args:
             name: name of provider
             host: host of gateway
             version: version of gateway
@@ -508,14 +509,15 @@
             raise QuantumServerlessException(
                 "Authentication credentials must "
                 "be provided in form of `username` "
                 "and `password` or `token`."
             )
 
         super().__init__(name)
+        self.verbose = verbose
         self.host = host
         self.version = version
         self._token = token
         if token is None:
             self._fetch_token(username, password)
 
         self._job_client = GatewayJobClient(self.host, self._token, self.version)
@@ -526,63 +528,27 @@
     def create_compute_resource(self, resource) -> int:
         raise NotImplementedError("GatewayProvider does not support resources api yet.")
 
     def delete_compute_resource(self, resource) -> int:
         raise NotImplementedError("GatewayProvider does not support resources api yet.")
 
     def get_job_by_id(self, job_id: str) -> Optional[Job]:
-        job = None
-        url = f"{self.host}/api/{self.version}/jobs/{job_id}/"
-        response = requests.get(
-            url,
-            headers={"Authorization": f"Bearer {self._token}"},
-            timeout=REQUESTS_TIMEOUT,
-        )
-        if response.ok:
-            data = json.loads(response.text)
-            job = Job(
-                job_id=data.get("id"),
-                job_client=self._job_client,
-            )
-        else:
-            logging.warning(response.text)
-
-        return job
+        return self._job_client.get(job_id)
 
     def run_program(
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> Job:
         return self._job_client.run_program(program, arguments)
 
     def get_jobs(self, **kwargs) -> List[Job]:
-        jobs = []
-        url = f"{self.host}/api/{self.version}/jobs/"
-        response = requests.get(
-            url,
-            headers={"Authorization": f"Bearer {self._token}"},
-            timeout=REQUESTS_TIMEOUT,
-        )
-        if response.ok:
-            jobs = [
-                Job(
-                    job_id=job.get("id"),
-                    job_client=self._job_client,
-                )
-                for job in json.loads(response.text).get("results", [])
-            ]
-        else:
-            logging.warning(response.text)
-
-        return jobs
+        return self._job_client.list(**kwargs)
 
     def _fetch_token(self, username: str, password: str):
-        gateway_response = requests.post(
-            url=f"{self.host}/dj-rest-auth/keycloak/login/",
-            data={"username": username, "password": password},
-            timeout=REQUESTS_TIMEOUT,
+        response_data = safe_json_request(
+            request=lambda: requests.post(
+                url=f"{self.host}/dj-rest-auth/keycloak/login/",
+                data={"username": username, "password": password},
+                timeout=REQUESTS_TIMEOUT,
+            )
         )
 
-        if not gateway_response.ok:
-            raise QuantumServerlessException(gateway_response.text)
-
-        gateway_token = json.loads(gateway_response.text).get("access")
-        self._token = gateway_token
+        self._token = response_data.get("access")
```

### Comparing `quantum_serverless-0.0.8/quantum_serverless/core/state.py` & `quantum_serverless-0.0.9/quantum_serverless/core/state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/core/tracing.py` & `quantum_serverless-0.0.9/quantum_serverless/core/tracing.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/exception.py` & `quantum_serverless-0.0.9/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/library/__init__.py` & `quantum_serverless-0.0.9/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.0.9/quantum_serverless/library/transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.0.9/quantum_serverless/quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.0.9/quantum_serverless/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/serializers/program_serializers.py` & `quantum_serverless-0.0.9/quantum_serverless/serializers/program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.0.9/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.0.9/quantum_serverless/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/quantum_serverless.egg-info/PKG-INFO` & `quantum_serverless-0.0.9/quantum_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-serverless
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.0.8/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.0.9/quantum_serverless.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 quantum_serverless/core/tracing.py
 quantum_serverless/library/__init__.py
 quantum_serverless/library/transpiler.py
 quantum_serverless/serializers/__init__.py
 quantum_serverless/serializers/program_serializers.py
 quantum_serverless/serializers/serializers.py
 quantum_serverless/utils/__init__.py
+quantum_serverless/utils/errors.py
 quantum_serverless/utils/json.py
 tests/__init__.py
 tests/test_quantum_serverless.py
 tests/utils.py
 tests/core/__init__.py
 tests/core/test_decorator.py
 tests/core/test_program.py
```

### Comparing `quantum_serverless-0.0.8/setup.py` & `quantum_serverless-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/tests/core/test_decorator.py` & `quantum_serverless-0.0.9/tests/core/test_decorator.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/tests/core/test_program.py` & `quantum_serverless-0.0.9/tests/core/test_program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/tests/core/test_program_repository.py` & `quantum_serverless-0.0.9/tests/core/test_program_repository.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/tests/core/test_state.py` & `quantum_serverless-0.0.9/tests/core/test_state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/tests/library/test_transpiler.py` & `quantum_serverless-0.0.9/tests/library/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/tests/serializers/test_program_serializers.py` & `quantum_serverless-0.0.9/tests/serializers/test_program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/tests/serializers/test_serializers.py` & `quantum_serverless-0.0.9/tests/serializers/test_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/tests/test_quantum_serverless.py` & `quantum_serverless-0.0.9/tests/test_quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.8/tests/utils.py` & `quantum_serverless-0.0.9/tests/utils.py`

 * *Files identical despite different names*

