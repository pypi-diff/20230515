# Comparing `tmp/kuflow_temporal_activity_kuflow-0.4.2.tar.gz` & `tmp/kuflow_temporal_activity_kuflow-0.4.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_kuflow-0.4.2.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_kuflow-0.4.3.dev0.tar", max compression
```

## Comparing `kuflow_temporal_activity_kuflow-0.4.2.tar` & `kuflow_temporal_activity_kuflow-0.4.3.dev0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      878 2023-03-22 13:32:42.999843 kuflow_temporal_activity_kuflow-0.4.2/README.md
--rw-r--r--   0        0        0        6 2023-03-22 13:32:42.999843 kuflow_temporal_activity_kuflow-0.4.2/VERSION
--rw-r--r--   0        0        0     1320 2023-03-22 13:32:42.999843 kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/__init__.py
--rw-r--r--   0        0        0     2696 2023-03-22 13:32:42.999843 kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/converter.py
--rw-r--r--   0        0        0      849 2023-03-22 13:32:42.999843 kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
--rw-r--r--   0        0        0    11009 2023-03-22 13:32:42.999843 kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
--rw-r--r--   0        0        0     3391 2023-03-22 13:32:42.999843 kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/models/__init__.py
--rw-r--r--   0        0        0    13208 2023-03-22 13:32:42.999843 kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/models/_models.py
--rw-r--r--   0        0        0     7215 2023-03-22 13:32:42.999843 kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/validation.py
--rw-r--r--   0        0        0      838 2023-03-22 13:33:54.146996 kuflow_temporal_activity_kuflow-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.4.2/setup.py
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-05-15 10:43:31.536858 kuflow_temporal_activity_kuflow-0.4.3.dev0/README.md
+-rw-r--r--   0        0        0       11 2023-05-15 10:43:31.536858 kuflow_temporal_activity_kuflow-0.4.3.dev0/VERSION
+-rw-r--r--   0        0        0     1320 2023-05-15 10:43:31.536858 kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/__init__.py
+-rw-r--r--   0        0        0     2696 2023-05-15 10:43:31.536858 kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/converter.py
+-rw-r--r--   0        0        0      849 2023-05-15 10:43:31.536858 kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
+-rw-r--r--   0        0        0    11009 2023-05-15 10:43:31.536858 kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
+-rw-r--r--   0        0        0     3391 2023-05-15 10:43:31.536858 kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/models/__init__.py
+-rw-r--r--   0        0        0    13208 2023-05-15 10:43:31.536858 kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/models/_models.py
+-rw-r--r--   0        0        0     7215 2023-05-15 10:43:31.536858 kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/validation.py
+-rw-r--r--   0        0        0      843 2023-05-15 10:44:37.162474 kuflow_temporal_activity_kuflow-0.4.3.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.4.3.dev0/setup.py
+-rw-r--r--   0        0        0     1672 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.4.3.dev0/PKG-INFO
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/README.md` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/__init__.py` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from .kuflow_async_activities import KuFlowAsyncActivities
 from .kuflow_sync_activities import KuFlowSyncActivities
 
 __all__ = ["KuFlowAsyncActivities", "KuFlowSyncActivities"]
-__version__ = "0.4.2"
+__version__ = "0.4.3"
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/converter.py` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/converter.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/kuflow_async_activities.py` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/kuflow_async_activities.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/models/__init__.py` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/models/_models.py` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/kuflow_temporal_activity_kuflow/validation.py` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/kuflow_temporal_activity_kuflow/validation.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/pyproject.toml` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-activity-kuflow"
-version = "0.4.2"
+version = "0.4.3.dev0"
 description = "KuFlow SDK :: Temporal.io activities to interact with KuFlow"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,15 +13,15 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-temporal-common = "^0.4.2"
+kuflow-temporal-common = "^0.4.3"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "0.910"
 flake8 = "4.0.1"
 black = "^23.1.0"
 pytest = "^7.2.1"
 pyyaml = "^6.0"
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/setup.py` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['kuflow_temporal_activity_kuflow', 'kuflow_temporal_activity_kuflow.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=0.4.2,<0.5.0']
+['kuflow-temporal-common>=0.4.3,<0.5.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-kuflow',
-    'version': '0.4.2',
+    'version': '0.4.3.dev0',
     'description': 'KuFlow SDK :: Temporal.io activities to interact with KuFlow',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n\n# KuFlow Temporal Activities KuFlow\n\nTemporal.io activities to interact with KuFlow\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.2/PKG-INFO` & `kuflow_temporal_activity_kuflow-0.4.3.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-kuflow
-Version: 0.4.2
+Version: 0.4.3.dev0
 Summary: KuFlow SDK :: Temporal.io activities to interact with KuFlow
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kuflow-temporal-common (>=0.4.2,<0.5.0)
+Requires-Dist: kuflow-temporal-common (>=0.4.3,<0.5.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
 [![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
```

