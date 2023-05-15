# Comparing `tmp/core_utils-0.1.0.tar.gz` & `tmp/core_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_utils-0.1.0.tar", max compression
+gzip compressed data, was "core_utils-0.1.1.tar", max compression
```

## Comparing `core_utils-0.1.0.tar` & `core_utils-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0        0 2023-05-12 14:32:00.496539 core_utils-0.1.0/core_utils/__init__.py
--rw-r--r--   0        0        0       33 2023-05-01 18:12:25.578891 core_utils-0.1.0/core_utils/base_repository.py
--rw-r--r--   0        0        0     4020 2023-05-12 15:22:02.118024 core_utils-0.1.0/core_utils/base_service.py
--rw-r--r--   0        0        0        0 2023-05-12 15:20:47.867710 core_utils-0.1.0/core_utils/db/__init__.py
--rw-r--r--   0        0        0      680 2023-05-12 14:45:46.281981 core_utils-0.1.0/core_utils/db/session.py
--rw-r--r--   0        0        0      991 2023-05-12 14:36:16.785730 core_utils-0.1.0/core_utils/logger.py
--rw-r--r--   0        0        0        0 2023-05-12 14:30:34.021812 core_utils-0.1.0/core_utils/models/__init__.py
--rw-r--r--   0        0        0     3443 2023-05-15 07:05:54.979875 core_utils-0.1.0/core_utils/models/base_model.py
--rw-r--r--   0        0        0      436 2023-04-24 09:28:50.892496 core_utils-0.1.0/core_utils/models/mixins.py
--rw-r--r--   0        0        0      455 2023-05-15 07:05:54.987438 core_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-12 14:04:03.786079 core_utils-0.1.0/README.md
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 core_utils-0.1.0/setup.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 core_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-15 07:21:22.447851 core_utils-0.1.1/core_utils/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-15 07:21:22.448852 core_utils-0.1.1/core_utils/base_repository.py
+-rw-r--r--   0        0        0     3932 2023-05-15 07:37:47.969749 core_utils-0.1.1/core_utils/base_service.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:21:22.448852 core_utils-0.1.1/core_utils/db/__init__.py
+-rw-r--r--   0        0        0      680 2023-05-15 07:21:22.449853 core_utils-0.1.1/core_utils/db/session.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:37:34.380355 core_utils-0.1.1/core_utils/grpc_gen/__init__.py
+-rw-r--r--   0        0        0      991 2023-05-15 07:21:22.449853 core_utils-0.1.1/core_utils/logger.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:21:22.450855 core_utils-0.1.1/core_utils/models/__init__.py
+-rw-r--r--   0        0        0     3443 2023-05-15 07:21:22.450855 core_utils-0.1.1/core_utils/models/base_model.py
+-rw-r--r--   0        0        0      436 2023-05-15 07:21:22.450855 core_utils-0.1.1/core_utils/models/mixins.py
+-rw-r--r--   0        0        0      455 2023-05-15 07:42:23.769892 core_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-12 14:04:03.786079 core_utils-0.1.1/README.md
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 core_utils-0.1.1/setup.py
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 core_utils-0.1.1/PKG-INFO
```

### Comparing `core_utils-0.1.0/core_utils/base_service.py` & `core_utils-0.1.1/core_utils/base_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import sys
 from contextlib import asynccontextmanager
 from pathlib import Path
 from typing import AsyncGenerator, Any, List
 
-# from google.protobuf.struct_pb2 import Value
+from google.protobuf.struct_pb2 import Value
 from google.protobuf.wrappers_pb2 import BoolValue
 from grpclib.client import Channel
 from grpclib.server import Server
 
 from logger import log
 
-grpc_gen_path = Path(__file__).resolve().parent.parent.parent / "grpc_gen"
+grpc_gen_path = Path(__file__).resolve() / "grpc_gen"
 sys.path.insert(0, str(grpc_gen_path))
 
-# from grpc_gen.helper_pb2 import Filter
+from grpc_gen.helper_pb2 import Filter
 
 
 class BaseService:
     @property
     def _client_host(self) -> str | None:
         return self.__client_host
 
@@ -75,37 +75,37 @@
                     if isinstance(value, bool):
                         bool_value = BoolValue(value=value)
                         getattr(obj_proto, field_name).CopyFrom(bool_value)
                     else:
                         setattr(obj_proto, field_name, value)
         return obj_proto
 
-    # @staticmethod
-    # def filters_to_proto(filters: dict[str, Any]) -> List[Filter]:
-    #     proto_filters = []
-    #     for key, value in filters.items():
-    #         filter_value = Value()
-    #         if isinstance(value, str):
-    #             filter_value.string_value = value
-    #         elif isinstance(value, (int, float)):
-    #             filter_value.number_value = value
-    #         elif isinstance(value, bool):
-    #             filter_value.bool_value = value
-    #         else:
-    #             raise ValueError(f"Unsupported value type: {type(value)}")
-    #         proto_filters.append(Filter(field=key, value=filter_value))
-    #     return proto_filters
-    #
-    # @staticmethod
-    # def filters_from_proto(proto_filters: List[Filter]) -> dict[str, Any]:
-    #     filters = {}
-    #     for proto_filter in proto_filters:
-    #         value = proto_filter.value
-    #         if value.HasField("string_value"):
-    #             filters[proto_filter.field] = value.string_value
-    #         elif value.HasField("number_value"):
-    #             filters[proto_filter.field] = value.number_value
-    #         elif value.HasField("bool_value"):
-    #             filters[proto_filter.field] = value.bool_value
-    #         else:
-    #             raise ValueError(f"Unsupported value type in filter: {proto_filter.field}")
-    #     return filters
+    @staticmethod
+    def filters_to_proto(filters: dict[str, Any]) -> List[Filter]:
+        proto_filters = []
+        for key, value in filters.items():
+            filter_value = Value()
+            if isinstance(value, str):
+                filter_value.string_value = value
+            elif isinstance(value, (int, float)):
+                filter_value.number_value = value
+            elif isinstance(value, bool):
+                filter_value.bool_value = value
+            else:
+                raise ValueError(f"Unsupported value type: {type(value)}")
+            proto_filters.append(Filter(field=key, value=filter_value))
+        return proto_filters
+
+    @staticmethod
+    def filters_from_proto(proto_filters: List[Filter]) -> dict[str, Any]:
+        filters = {}
+        for proto_filter in proto_filters:
+            value = proto_filter.value
+            if value.HasField("string_value"):
+                filters[proto_filter.field] = value.string_value
+            elif value.HasField("number_value"):
+                filters[proto_filter.field] = value.number_value
+            elif value.HasField("bool_value"):
+                filters[proto_filter.field] = value.bool_value
+            else:
+                raise ValueError(f"Unsupported value type in filter: {proto_filter.field}")
+        return filters
```

### Comparing `core_utils-0.1.0/core_utils/db/session.py` & `core_utils-0.1.1/core_utils/db/session.py`

 * *Files identical despite different names*

### Comparing `core_utils-0.1.0/core_utils/logger.py` & `core_utils-0.1.1/core_utils/logger.py`

 * *Files identical despite different names*

### Comparing `core_utils-0.1.0/core_utils/models/base_model.py` & `core_utils-0.1.1/core_utils/models/base_model.py`

 * *Files identical despite different names*

### Comparing `core_utils-0.1.0/setup.py` & `core_utils-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['core_utils', 'core_utils.db', 'core_utils.models']
+['core_utils', 'core_utils.db', 'core_utils.grpc_gen', 'core_utils.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['asyncpg>=0.27.0,<0.28.0',
  'grpcio-tools>=1.54.0,<2.0.0',
  'grpcio>=1.54.0,<2.0.0',
  'grpclib>=0.4.4,<0.5.0',
  'protobuf>=4.23.0,<5.0.0',
  'sqlalchemy>=2.0.13,<3.0.0']
 
 setup_kwargs = {
     'name': 'core-utils',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Common base classes for microservices',
     'long_description': '',
     'author': 'Dmitry Roshupkin',
     'author_email': 'd3po13@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `core_utils-0.1.0/PKG-INFO` & `core_utils-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Common base classes for microservices
 Author: Dmitry Roshupkin
 Author-email: d3po13@yandex.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
```

