# Comparing `tmp/kedro_vertexai-0.8.0.tar.gz` & `tmp/kedro_vertexai-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_vertexai-0.8.0.tar", max compression
+gzip compressed data, was "kedro_vertexai-0.8.1.tar", max compression
```

## Comparing `kedro_vertexai-0.8.0.tar` & `kedro_vertexai-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11338 2022-12-09 16:50:44.390277 kedro_vertexai-0.8.0/LICENSE
--rw-r--r--   0        0        0     2517 2022-12-09 16:50:44.390277 kedro_vertexai-0.8.0/README.md
--rw-r--r--   0        0        0       22 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/__init__.py
--rw-r--r--   0        0        0       18 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/auth/__init__.py
--rw-r--r--   0        0        0     5770 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/auth/gcp.py
--rw-r--r--   0        0        0     2257 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/auth/mlflow_request_header_provider.py
--rw-r--r--   0        0        0     1044 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/auth/mlflow_request_header_provider_hook.py
--rw-r--r--   0        0        0     9599 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/cli.py
--rw-r--r--   0        0        0     7633 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/client.py
--rw-r--r--   0        0        0     5912 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/config.py
--rw-r--r--   0        0        0      418 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/constants.py
--rw-r--r--   0        0        0     2586 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/context_helper.py
--rw-r--r--   0        0        0      790 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/data_models.py
--rw-r--r--   0        0        0     1594 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/dynamic_config.py
--rw-r--r--   0        0        0     9175 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/generator.py
--rw-r--r--   0        0        0     1585 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/hooks.py
--rw-r--r--   0        0        0      210 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/runtime_config.py
--rw-r--r--   0        0        0     1540 2022-12-09 16:50:44.398277 kedro_vertexai-0.8.0/kedro_vertexai/templates/github-on-push.yml
--rw-r--r--   0        0        0     3007 2022-12-09 16:50:44.402277 kedro_vertexai-0.8.0/kedro_vertexai/utils.py
--rw-r--r--   0        0        0       31 2022-12-09 16:50:44.402277 kedro_vertexai-0.8.0/kedro_vertexai/vertex_ai/__init__.py
--rw-r--r--   0        0        0     1639 2022-12-09 16:50:44.402277 kedro_vertexai-0.8.0/kedro_vertexai/vertex_ai/datasets.py
--rw-r--r--   0        0        0     1924 2022-12-09 16:50:44.402277 kedro_vertexai-0.8.0/kedro_vertexai/vertex_ai/io.py
--rw-r--r--   0        0        0     1616 2022-12-09 16:50:44.402277 kedro_vertexai-0.8.0/kedro_vertexai/vertex_ai/runner.py
--rw-r--r--   0        0        0     2330 2022-12-09 16:50:44.402277 kedro_vertexai-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4368 1970-01-01 00:00:00.000000 kedro_vertexai-0.8.0/setup.py
--rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 kedro_vertexai-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2022-12-30 12:01:15.310806 kedro_vertexai-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2517 2022-12-30 12:01:15.310806 kedro_vertexai-0.8.1/README.md
+-rw-r--r--   0        0        0       22 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/__init__.py
+-rw-r--r--   0        0        0       18 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/auth/__init__.py
+-rw-r--r--   0        0        0     5770 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/auth/gcp.py
+-rw-r--r--   0        0        0     2257 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/auth/mlflow_request_header_provider.py
+-rw-r--r--   0        0        0     1044 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/auth/mlflow_request_header_provider_hook.py
+-rw-r--r--   0        0        0     9599 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/cli.py
+-rw-r--r--   0        0        0     7633 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/client.py
+-rw-r--r--   0        0        0     5912 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/config.py
+-rw-r--r--   0        0        0      418 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/constants.py
+-rw-r--r--   0        0        0     2636 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/context_helper.py
+-rw-r--r--   0        0        0      790 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/data_models.py
+-rw-r--r--   0        0        0     1594 2022-12-30 12:01:15.318806 kedro_vertexai-0.8.1/kedro_vertexai/dynamic_config.py
+-rw-r--r--   0        0        0     9175 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/kedro_vertexai/generator.py
+-rw-r--r--   0        0        0     1585 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/kedro_vertexai/hooks.py
+-rw-r--r--   0        0        0      210 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/kedro_vertexai/runtime_config.py
+-rw-r--r--   0        0        0     1540 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/kedro_vertexai/templates/github-on-push.yml
+-rw-r--r--   0        0        0     3007 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/kedro_vertexai/utils.py
+-rw-r--r--   0        0        0       31 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/kedro_vertexai/vertex_ai/__init__.py
+-rw-r--r--   0        0        0     1639 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/kedro_vertexai/vertex_ai/datasets.py
+-rw-r--r--   0        0        0     1924 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/kedro_vertexai/vertex_ai/io.py
+-rw-r--r--   0        0        0     1616 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/kedro_vertexai/vertex_ai/runner.py
+-rw-r--r--   0        0        0     2330 2022-12-30 12:01:15.322806 kedro_vertexai-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4368 1970-01-01 00:00:00.000000 kedro_vertexai-0.8.1/setup.py
+-rw-r--r--   0        0        0     4142 1970-01-01 00:00:00.000000 kedro_vertexai-0.8.1/PKG-INFO
```

### Comparing `kedro_vertexai-0.8.0/LICENSE` & `kedro_vertexai-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/README.md` & `kedro_vertexai-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/auth/gcp.py` & `kedro_vertexai-0.8.1/kedro_vertexai/auth/gcp.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/auth/mlflow_request_header_provider.py` & `kedro_vertexai-0.8.1/kedro_vertexai/auth/mlflow_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/auth/mlflow_request_header_provider_hook.py` & `kedro_vertexai-0.8.1/kedro_vertexai/auth/mlflow_request_header_provider_hook.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/cli.py` & `kedro_vertexai-0.8.1/kedro_vertexai/cli.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/client.py` & `kedro_vertexai-0.8.1/kedro_vertexai/client.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/config.py` & `kedro_vertexai-0.8.1/kedro_vertexai/config.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/context_helper.py` & `kedro_vertexai-0.8.1/kedro_vertexai/context_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from functools import lru_cache
+from functools import cached_property
 from typing import Any, Dict
 
 from kedro.config import TemplatedConfigLoader
 
 from kedro_vertexai.client import VertexAIPipelinesClient
 
 from .config import PluginConfig
@@ -56,34 +56,32 @@
         self._metadata = metadata
         self._env = env
 
     @property
     def project_name(self):
         return self._metadata.project_name
 
-    @property
-    @lru_cache()
+    @cached_property
     def session(self):
         from kedro.framework.session import KedroSession
 
         return KedroSession.create(self._metadata.package_name, env=self._env)
 
-    @property
+    @cached_property
     def context(self):
+        assert self.session is not None, "Session not initialized"
         return self.session.load_context()
 
-    @property
-    @lru_cache()
+    @cached_property
     def config(self) -> PluginConfig:
         raw = EnvTemplatedConfigLoader(self.context.config_loader.conf_source).get(
             self.CONFIG_FILE_PATTERN
         )
         return PluginConfig.parse_obj(raw)
 
-    @property
-    @lru_cache()
+    @cached_property
     def vertexai_client(self) -> VertexAIPipelinesClient:
         return VertexAIPipelinesClient(self.config, self.project_name, self.context)
 
     @staticmethod
     def init(metadata, env):
         return ContextHelper(metadata, env)
```

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/data_models.py` & `kedro_vertexai-0.8.1/kedro_vertexai/data_models.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/dynamic_config.py` & `kedro_vertexai-0.8.1/kedro_vertexai/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/generator.py` & `kedro_vertexai-0.8.1/kedro_vertexai/generator.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/hooks.py` & `kedro_vertexai-0.8.1/kedro_vertexai/hooks.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/templates/github-on-push.yml` & `kedro_vertexai-0.8.1/kedro_vertexai/templates/github-on-push.yml`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/utils.py` & `kedro_vertexai-0.8.1/kedro_vertexai/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/vertex_ai/datasets.py` & `kedro_vertexai-0.8.1/kedro_vertexai/vertex_ai/datasets.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/vertex_ai/io.py` & `kedro_vertexai-0.8.1/kedro_vertexai/vertex_ai/io.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/kedro_vertexai/vertex_ai/runner.py` & `kedro_vertexai-0.8.1/kedro_vertexai/vertex_ai/runner.py`

 * *Files identical despite different names*

### Comparing `kedro_vertexai-0.8.0/pyproject.toml` & `kedro_vertexai-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kedro-vertexai"
-version = "0.8.0"
+version = "0.8.1"
 description = "Kedro plugin with GCP Vertex AI support"
 readme = "README.md"
 authors = ['Marcin Zabłocki <marcin.zablocki@getindata.com>', 'Mateusz Pytel <mateusz.pytel@getindata.com>', 'Mariusz Strzelecki <mariusz.strzelecki@getindata.com>']
 maintainers = ['GetInData MLOPS <mlops@getindata.com>']
 homepage = "https://github.com/getindata/kedro-vertexai"
 repository = "https://github.com/getindata/kedro-vertexai"
 documentation = "https://kedro-vertexai.readthedocs.io/"
```

### Comparing `kedro_vertexai-0.8.0/setup.py` & `kedro_vertexai-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                  'kedro_vertexai.hooks:mlflow_tags_hook'],
  'kedro.project_commands': ['vertexai = kedro_vertexai.cli:commands'],
  'mlflow.request_header_provider': ['unused = '
                                     'kedro_vertexai.auth.mlflow_request_header_provider:DynamicMLFlowRequestHeaderProvider']}
 
 setup_kwargs = {
     'name': 'kedro-vertexai',
-    'version': '0.8.0',
+    'version': '0.8.1',
     'description': 'Kedro plugin with GCP Vertex AI support',
     'long_description': '# Kedro Vertex AI Plugin\n\n[![Python Version](https://img.shields.io/pypi/pyversions/kedro-vertexai)](https://github.com/getindata/kedro-vertexai)\n[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![SemVer](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)\n[![PyPI version](https://badge.fury.io/py/kedro-vertexai.svg)](https://pypi.org/project/kedro-vertexai/)\n[![Downloads](https://pepy.tech/badge/kedro-vertexai)](https://pepy.tech/project/kedro-vertexai)\n\n[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=getindata_kedro-vertexai&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=getindata_kedro-vertexai)\n[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=getindata_kedro-vertexai&metric=coverage)](https://sonarcloud.io/summary/new_code?id=getindata_kedro-vertexai)\n[![Documentation Status](https://readthedocs.org/projects/kedro-vertexai/badge/?version=latest)](https://kedro-vertexai.readthedocs.io/en/latest/?badge=latest)\n\n## About\n\nThe main purpose of this plugin is to enable running kedro pipeline on Google Cloud Platform - Vertex AI Pipelines.\nIt supports translation from Kedro pipeline DSL to [kfp](https://www.kubeflow.org/docs/pipelines/sdk/sdk-overview/) \n(pipelines SDK) and deployment to Vertex AI service with some convenient commands.\n\nThe plugin can be used together with `kedro-docker` to simplify preparation of docker image for pipeline execution.   \n\n## Documentation\n\nFor detailed documentation refer to https://kedro-vertexai.readthedocs.io/\n\n## Usage guide \n\n```\nUsage: kedro vertexai [OPTIONS] COMMAND [ARGS]...\n\n  Interact with Google Cloud Platform :: Vertex AI Pipelines\n\nOptions:\n  -e, --env TEXT  Environment to use.\n  -h, --help      Show this message and exit.\n\nCommands:\n  compile         Translates Kedro pipeline into JSON file with Kubeflow...\n  init            Initializes configuration for the plugin\n  list-pipelines  List deployed pipeline definitions\n  run-once        Deploy pipeline as a single run within given experiment.\n  ui              Open VertexAI Pipelines UI in new browser tab\n```\n\n## Configuration file\n\n`kedro init` generates configuration file for the plugin, but users may want to adjust it to match the run environment \nrequirements. Check documentation for details - [kedro-vertexai.readthedocs.io](https://kedro-vertexai.readthedocs.io/en/latest/source/02_installation/02_configuration.html)\n',
     'author': 'Marcin Zabłocki',
     'author_email': 'marcin.zablocki@getindata.com',
     'maintainer': 'GetInData MLOPS',
     'maintainer_email': 'mlops@getindata.com',
     'url': 'https://github.com/getindata/kedro-vertexai',
```

### Comparing `kedro_vertexai-0.8.0/PKG-INFO` & `kedro_vertexai-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-vertexai
-Version: 0.8.0
+Version: 0.8.1
 Summary: Kedro plugin with GCP Vertex AI support
 Home-page: https://github.com/getindata/kedro-vertexai
 License: Apache-2.0
 Keywords: kedro-plugin,kedro,mlops,vertexai,googlecloudplatform,machinelearning
 Author: Marcin Zabłocki
 Author-email: marcin.zablocki@getindata.com
 Maintainer: GetInData MLOPS
@@ -24,15 +24,15 @@
 Requires-Dist: google-auth (<3)
 Requires-Dist: google-cloud-iam (<3)
 Requires-Dist: google-cloud-scheduler (>=2.3.2)
 Requires-Dist: google-cloud-storage (<3.0.0)
 Requires-Dist: grpcio (>=1.44.0,<1.45.0)
 Requires-Dist: grpcio-status (>=1.44.0,<1.45.0)
 Requires-Dist: kedro (>=0.18.1,<0.19.0)
-Requires-Dist: kedro-mlflow (>=0.11.1,<0.12.0); extra == "mlflow"
+Requires-Dist: kedro-mlflow (>=0.11.1,<0.12.0) ; extra == "mlflow"
 Requires-Dist: kfp (>=1.8.12,<2.0)
 Requires-Dist: protobuf (<=3.20.0)
 Requires-Dist: pydantic (>=1.9.0,<1.10.0)
 Requires-Dist: semver (>=2.10,<3.0)
 Requires-Dist: tabulate (>=0.8.7)
 Project-URL: Documentation, https://kedro-vertexai.readthedocs.io/
 Project-URL: Repository, https://github.com/getindata/kedro-vertexai
```

