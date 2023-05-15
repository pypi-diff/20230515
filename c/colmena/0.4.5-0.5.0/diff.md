# Comparing `tmp/colmena-0.4.5.tar.gz` & `tmp/colmena-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colmena-0.4.5.tar", last modified: Thu Mar 16 22:24:06 2023, max compression
+gzip compressed data, was "colmena-0.5.0.tar", last modified: Mon May 15 11:53:29 2023, max compression
```

## Comparing `colmena-0.4.5.tar` & `colmena-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-03-16 22:23:58.000000 colmena-0.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18817 2023-03-16 22:24:06.055746 colmena-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-16 22:23:58.000000 colmena-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/colmena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24077 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/colmena/queue/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/queue/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/queue/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/queue/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/colmena/queue/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/queue/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/queue/tests/test_queues.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/colmena/task_server/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/task_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/task_server/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/task_server/funcx.py
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/task_server/parsl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/colmena/task_server/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/task_server/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/task_server/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/task_server/tests/test_funcx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/task_server/tests/test_parsl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/colmena/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/tests/test_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/colmena/thinker/
--rw-r--r--   0 runner    (1001) docker     (123)    19328 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/thinker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/thinker/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/colmena/thinker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/thinker/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/thinker/tests/test_thinker.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-16 22:23:58.000000 colmena-0.4.5/colmena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:24:06.055746 colmena-0.4.5/colmena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18817 2023-03-16 22:24:06.000000 colmena-0.4.5/colmena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-16 22:24:06.000000 colmena-0.4.5/colmena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 22:24:06.000000 colmena-0.4.5/colmena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-16 22:24:06.000000 colmena-0.4.5/colmena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 22:24:06.000000 colmena-0.4.5/colmena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-16 22:23:58.000000 colmena-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 22:24:06.055746 colmena-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-15 11:53:21.000000 colmena-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-15 11:53:29.131730 colmena-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-15 11:53:21.000000 colmena-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.127730 colmena-0.5.0/colmena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.127730 colmena-0.5.0/colmena/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.127730 colmena-0.5.0/colmena/queue/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/tests/test_queues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/task_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/parsl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/task_server/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/tests/test_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/tests/test_parsl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/tests/test_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/thinker/
+-rw-r--r--   0 runner    (1001) docker     (123)    19328 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/thinker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/thinker/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/thinker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/thinker/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/thinker/tests/test_thinker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.127730 colmena-0.5.0/colmena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-15 11:53:21.000000 colmena-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:53:29.131730 colmena-0.5.0/setup.cfg
```

### Comparing `colmena-0.4.5/LICENSE.txt` & `colmena-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/PKG-INFO` & `colmena-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colmena
-Version: 0.4.5
+Version: 0.5.0
 Summary: colmena: Intelligent Steerable Pipelines on HPC
 Author-email: Globus Labs <labs@globus.org>, Logan Ward <lward@anl.gov>, Greg Pauloski <jgpauloski@uchicago.edu>, Yadu Babuji <yadudoc1729@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -215,15 +215,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: funcx
+Provides-Extra: globus
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # Colmena
 
 [![CI](https://github.com/exalearn/colmena/actions/workflows/CI.yml/badge.svg)](https://github.com/exalearn/colmena/actions/workflows/CI.yml)
 [![Documentation Status](https://readthedocs.org/projects/colmena/badge/?version=latest)](https://colmena.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `colmena-0.4.5/README.md` & `colmena-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/models.py` & `colmena-0.5.0/colmena/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,16 +157,15 @@
 
     # Serialization options
     serialization_method: SerializationMethod = Field(SerializationMethod.JSON,
                                                       description="Method used to serialize input data")
     keep_inputs: bool = Field(True, description="Whether to keep the inputs with the result object or delete "
                                                 "them after the method has completed")
     proxystore_name: Optional[str] = Field(None, description="Name of ProxyStore backend you use for transferring large objects")
-    proxystore_type: Optional[str] = Field(None, description="Type of ProxyStore backend being used")
-    proxystore_kwargs: Optional[Dict] = Field(None, description="Kwargs to reinitialize ProxyStore backend")
+    proxystore_config: Optional[Dict] = Field(None, description="ProxyStore backend configuration")
     proxystore_threshold: Optional[int] = Field(None,
                                                 description="Proxy all input/output objects larger than this threshold in bytes")
 
     def __init__(self, inputs: Tuple[Tuple[Any], Dict[str, Any]], **kwargs):
         """
         Args:
              inputs (Any, Dict): Inputs to a function. Separated into positional and keyword arguments
@@ -303,16 +302,15 @@
                     value_size >= self.proxystore_threshold
             ):
                 # Proxy the value. We use the id of the object as the key
                 # so multiple copies of the object are not added to ProxyStore,
                 # but the value in ProxyStore will still be updated.
                 store = get_store(
                     name=self.proxystore_name,
-                    kind=self.proxystore_type,
-                    **self.proxystore_kwargs,
+                    config=self.proxystore_config,
                 )
                 value_proxy = store.proxy(value, evict=evict)
                 logger.debug(f'Proxied object of type {type(value)} with id={id(value)}')
                 proxies.append(value_proxy)
 
                 # Update the statistics
                 store_proxy_stats(value_proxy, self.proxy_timing)
```

### Comparing `colmena-0.4.5/colmena/proxy.py` & `colmena-0.5.0/colmena/proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,45 @@
 """Utilities for interacting with ProxyStore"""
 import logging
-import importlib
 import warnings
-from dataclasses import asdict
 
 import proxystore
 from proxystore.proxy import extract
 from proxystore.proxy import is_resolved
 from proxystore.proxy import Proxy
 from proxystore.store.base import Store
 from proxystore.store.utils import resolve_async, get_key
 
-from typing import Any, Union, List, Optional, Type
+from typing import Any, Dict, Union, List, Optional
 
 logger = logging.getLogger(__name__)
 
 
 class ProxyJSONSerializationWarning(Warning):
     pass
 
 
-def get_class_path(cls: Type[Any]) -> str:
-    """Get the fully qualified pass of a type."""
-    return f'{cls.__module__}.{cls.__qualname__}'
-
-
-def import_class(path: str) -> Type[Any]:
-    """Import class via its fully qualified pass."""
-    module_path, _, name = path.rpartition('.')
-    if len(module_path) == 0:
-        raise ImportError(f'Class path must contain at least one module. Got {path}')
-    module = importlib.import_module(module_path)
-    return getattr(module, name)
-
-
 def get_store(
     name: str,
-    kind: Optional[Union[Type[Store], str]] = None,
-    **kwargs: Any,
+    config: Optional[Dict[str, Any]] = None,
 ) -> Optional[Store]:
     """Get a Store by name or create one if it does not already exist.
 
     Args:
         name (str): name of the store.
-        kind (type[Store], str): if ``None``, (the default) this function will
-            lookup the store by `name` returning either the found store or
-            ``None``. If not ``None`` and a store by `name` does not exist,
-            `kind` will be used to initialize and register a new store. The
-            type of `kind` can be a string with the fully qualified class path
-            or the class type itself.
-        kwargs: keyword arguments to initialize the store with. Only used if
-            a store does not already exist and `kind` is not ``None``.
+        config: ``Store`` configuration that can be used to reinitialize the
+            ``Store`` if provided and a store with `name` is not found.
 
     Returns:
         The store registered as `name` or a newly intialized and registered
         store if `kind` is not ``None``.
     """
     store = proxystore.store.get_store(name)
-    if store is None and kind is not None:
-        if isinstance(kind, str):
-            kind = import_class(kind)
-        store = kind(name=name, **kwargs)
+    if store is None and config is not None:
+        store = Store.from_config(config)
         proxystore.store.register_store(store)
     return store
 
 
 def proxy_json_encoder(proxy: Proxy) -> Any:
     """Custom encoder function for proxies
 
@@ -159,19 +134,19 @@
     key = get_key(proxy)
 
     # ProxyStore keys are NamedTuples so we cast to a string
     # so we can use the key as a JSON key.
     key = str(key)
 
     # Get the store associated with this proxy
-    store = get_store(proxy)
-    if store.has_stats:
+    store = proxystore.store.get_store(proxy)
+    if store.metrics is not None:
         # Get the stats and convert them to a JSON-serializable form
-        stats = store.stats(proxy)
-        stats = dict((k, asdict(v)) for k, v in stats.items())
+        metrics = store.metrics.get_metrics(proxy)
+        stats = metrics.as_dict() if metrics is not None else {}
     else:
         stats = {}
 
     # Update existing timings
     if key not in proxy_timing:
         proxy_timing[key] = {}
     proxy_timing[key].update(stats)
```

### Comparing `colmena-0.4.5/colmena/queue/base.py` & `colmena-0.5.0/colmena/queue/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import warnings
 from abc import abstractmethod
 from enum import Enum
 from threading import Lock, Event
 from typing import Optional, Tuple, Any, Collection, Union, Dict, Set
 import logging
 
-import proxystore as ps
+import proxystore.store
 
 from colmena.models import Result, SerializationMethod, ResourceRequirements
-from colmena.proxy import get_class_path
 
 logger = logging.getLogger(__name__)
 
 
 class QueueRole(str, Enum):
     """Role a queue is used for"""
 
@@ -36,18 +35,19 @@
                  proxystore_name: Optional[Union[str, Dict[str, str]]] = None,
                  proxystore_threshold: Optional[Union[int, Dict[str, int]]] = None):
         """
         Args:
             topics: Names of topics that are known for this queue
             serialization_method: Method used to serialize task inputs and results
             keep_inputs: Whether to return task inputs with the result object
-            proxystore_name (str, dict): Name of ProxyStore backend to use for all
-                topics or a mapping of topic to ProxyStore backend for specifying
-                backends for certain tasks. If a mapping is provided but a topic is
-                not in the mapping, ProxyStore will not be used.
+            proxystore_name (str, dict): Name of a registered ProxyStore
+                `Store` instance. This can be a single name such that the
+                corresponding `Store` is used for all topics or a mapping of
+                topics to registered `Store` names. If a mapping is provided
+                but a topic is not in the mapping, ProxyStore will not be used.
             proxystore_threshold (int, dict): Threshold in bytes for using
                 ProxyStore to transfer objects. Optionally can pass a dict
                 mapping topics to threshold to use different threshold values
                 for different topics. None values in the mapping will exclude
                 ProxyStore use with that topic.
         """
 
@@ -76,19 +76,19 @@
         elif proxystore_threshold is not None:
             raise ValueError(f'Unexpected type {type(proxystore_threshold)} for proxystore_threshold')
 
         # Verify that ProxyStore backends exist
         for ps_name in set(self.proxystore_name.values()):
             if ps_name is None:
                 continue
-            store = ps.store.get_store(ps_name)
+            store = proxystore.store.get_store(ps_name)
             if store is None:
                 raise ValueError(
-                    f'ProxyStore backend with name "{ps_name}" was not '
-                    'found. This is likely because the store needs to be '
+                    f'A Store with name "{ps_name}" has not been registered. '
+                    'This is likely because the store needs to be '
                     'initialized prior to initializing the Colmena queue.'
                 )
 
         # Log the ProxyStore configuration
         for topic in self.topics:
             ps_name = self.proxystore_name[topic]
             ps_threshold = self.proxystore_threshold[topic]
@@ -209,40 +209,36 @@
 
         # Determine whether to override the default "keep_inputs"
         _keep_inputs = self.keep_inputs
         if keep_inputs is not None:
             _keep_inputs = keep_inputs
 
         # Gather ProxyStore info if we are using it with this topic
-        proxystore_kwargs = {}
-        if (
-                self.proxystore_name[topic] is not None and
-                self.proxystore_threshold[topic] is not None
-        ):
-            store = ps.store.get_store(self.proxystore_name[topic])
+        ps_name = self.proxystore_name[topic]
+        ps_threshold = self.proxystore_threshold[topic]
+        ps_kwargs = {}
+        if ps_name is not None and ps_threshold is not None:
+            store = proxystore.store.get_store(ps_name)
             # proxystore_kwargs contains all the information we would need to
             # reconnect to the ProxyStore backend on any worker
-            proxystore_kwargs.update({
-                'proxystore_name': self.proxystore_name[topic],
-                'proxystore_threshold': self.proxystore_threshold[topic],
-                # Pydantic prefers to not have types as attributes, so we
-                # get the string corresponding to the type of the store we use
-                'proxystore_type': get_class_path(type(store)),
-                'proxystore_kwargs': store.kwargs
+            ps_kwargs.update({
+                'proxystore_name': ps_name,
+                'proxystore_threshold': ps_threshold,
+                'proxystore_config': store.config(),
             })
 
         # Create a new Result object
         result = Result(
             (input_args, input_kwargs),
             method=method,
             keep_inputs=_keep_inputs,
             serialization_method=self.serialization_method,
             task_info=task_info,
             resources=resources or ResourceRequirements(),  # Takes either the user specified or a default
-            **proxystore_kwargs
+            **ps_kwargs
         )
 
         # Push the serialized value to the task server
         result.time_serialize_inputs, proxies = result.serialize()
         self._send_request(result.json(exclude_none=True), topic)
         logger.info(f'Client sent a {method} task with topic {topic}. Created {len(proxies)} proxies for input values')
```

### Comparing `colmena-0.4.5/colmena/queue/python.py` & `colmena-0.5.0/colmena/queue/python.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/queue/redis.py` & `colmena-0.5.0/colmena/queue/redis.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/queue/tests/test_base.py` & `colmena-0.5.0/colmena/queue/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/queue/tests/test_queues.py` & `colmena-0.5.0/colmena/queue/tests/test_queues.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/task_server/base.py` & `colmena-0.5.0/colmena/task_server/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     Note that implementations are still responsible for adding the :meth:`run_and_record_timing` decorator.
     """
 
     def perform_callback(self, future: Future, result: Result, topic: str):
         """Send a completed result back to queue. Used as a callback for complete tasks
 
         Args:
-            future: Future created by FuncX
+            future: Future for a task
             result: Initial result object. Used if the future throws an exception
             topic: Topic used to send back to the user
         """
 
         task_exc = future.exception()
 
         # If it was, send back a modified copy of the input structure
```

### Comparing `colmena-0.4.5/colmena/task_server/funcx.py` & `colmena-0.5.0/colmena/task_server/globus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,83 +1,85 @@
-"""Task server based on FuncX
+"""Task server based on Globus Compute
 
-FuncX provides the ability to execute functions on remote "endpoints" that provide access to computational resources (e.g., cloud providers, HPC).
+Globus Compute provides the ability to execute functions on remote "endpoints" that provide access to
+computational resources (e.g., cloud providers, HPC).
 Tasks and results are communicated to/from the endpoint through a cloud service secured using Globus Auth."""
 
 import logging
 from functools import partial, update_wrapper
 from typing import Dict, Callable, Optional, Tuple
 from concurrent.futures import Future
 
-from funcx import FuncXClient, FuncXExecutor
+from globus_compute_sdk import Client, Executor
 
 from colmena.task_server.base import run_and_record_timing, FutureBasedTaskServer
 from colmena.queue.python import PipeQueues
 
 from colmena.models import Result
 
 logger = logging.getLogger(__name__)
 
 
-class FuncXTaskServer(FutureBasedTaskServer):
-    """Task server that uses FuncX to execute tasks on remote systems
+class GlobusComputeTaskServer(FutureBasedTaskServer):
+    """Task server that uses Globus Compute to execute tasks on remote systems
 
-    Create a FuncXTaskServer by providing a dictionary of functions along with a FuncX endpoint ID
+    Create a task server by providing a dictionary of functions
     mapped to the `endpoint <https://funcx.readthedocs.io/en/latest/endpoints.html>`_
-    on which it should run. The task server will wrap the provided function
+    on which each should run. The task server will wrap the provided function
     in an interface that tracks execution information (e.g., runtime) and
     `registers <https://funcx.readthedocs.io/en/latest/sdk.html#registering-functions>`_
-    the wrapped function with FuncX.
-    You must also provide a :class:`FuncXClient` that the task server can use to authenticate with the
-    FuncX web service.
-
-    The task server works using the :class:`FuncXExecutor` to communicate with FuncX via a RabbitMQ.
-    Once the task service process is created, the `FuncXClient` is used to instantiate a new
-    `FuncXExecutor` to perform work, and we use callbacks on the Python :class:`Future` objects
-    to send completed work back to the task queue.
+    the wrapped function with Globus Compute.
+    You must also provide a Globus Compute :class:`~globus_compute_sdk.client.Client`
+     that the task server will use to authenticate with the web service.
+
+    The task server works using Globus Compute's :class:`~globus_compute_sdk.executor.Executor`
+    to communicate to the web service over a web socket.
+    The functions used by the executor are registered when you create the task server,
+    and the Executor is launched when you start the task server.
     """
 
-    def __init__(self, methods: Dict[Callable, str],
-                 funcx_client: FuncXClient,
+    def __init__(self,
+                 methods: Dict[Callable, str],
+                 funcx_client: Client,
                  queues: PipeQueues,
                  timeout: Optional[int] = None,
                  batch_size: int = 128):
         """
         Args:
             methods: Map of functions to the endpoint on which it will run
-            funcx_client: Authenticated FuncX client
+            funcx_client: Authenticated Globus Compute client
             queues: Queues used to communicate with thinker
             timeout: Timeout for requests from the task queue
             batch_size: Maximum number of task request to receive before submitting
         """
         # Store the client that has already been authenticated.
         self.fx_client = funcx_client
-        self.fx_exec: FuncXExecutor = None
+        self.fx_exec: Optional[Executor] = None
 
         # Create a function with the latest version of the wrapper function
-        self.registered_funcs: Dict[str, Tuple[Callable, str]] = {}  # Function name -> (funcX id, endpoints)
+        self.registered_funcs: Dict[str, Tuple[str, str]] = {}  # Function name -> (funcX id, endpoints)
         for func, endpoint in methods.items():
             # Make a wrapped version of the function
             func_name = func.__name__
             new_func = partial(run_and_record_timing, func)
             update_wrapper(new_func, func)
             func_fxid = self.fx_client.register_function(new_func)
-            # Store the FuncX information for the function
+            # Store the information for the function
             self.registered_funcs[func_name] = (func_fxid, endpoint)
 
         self._batch_options = dict(
             batch_size=batch_size,
         )
 
         # Initialize the outputs
         super().__init__(queues, self.registered_funcs.keys(), timeout)
 
     def perform_callback(self, future: Future, result: Result, topic: str):
         # Check if the failure was due to a ManagerLost
-        #  TODO (wardlt): Remove when we have retry support in FuncX
+        #  TODO (wardlt): Remove when we have retry support in Globus Compute
         exc = future.exception()
         if 'Task failure due to loss of manager' in str(exc):
             logger.info('Caught an task that failed due to a lost manager. Resubmitting')
             self.process_queue(topic, result)
         else:
             super().perform_callback(future, result, topic)
 
@@ -93,13 +95,13 @@
         # Submit it to funcX to be executed
         future = self.fx_exec.submit_to_registered_function(func, kwargs={'result': task})
 
         logger.info(f'Submitted {task.method} to run on {endp_id}')
         return future
 
     def _setup(self):
-        # Create an executor to asynchronously transmit funcX tasks and recieve results
-        self.fx_exec = FuncXExecutor(funcx_client=self.fx_client,
-                                     batch_size=self._batch_options['batch_size'])
+        # Create an executor to asynchronously transmit funcX tasks and receive results
+        self.fx_exec = Executor(funcx_client=self.fx_client,
+                                batch_size=self._batch_options['batch_size'])
 
     def _cleanup(self):
-        self.fx_exec.shutdown()
+        self.fx_exec.shutdown(cancel_futures=True)
```

### Comparing `colmena-0.4.5/colmena/task_server/parsl.py` & `colmena-0.5.0/colmena/task_server/parsl.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/task_server/tests/test_base.py` & `colmena-0.5.0/colmena/task_server/tests/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Any, Dict, Tuple, List, Optional
 from pathlib import Path
 
+from proxystore.connectors.file import FileConnector
+from proxystore.store import Store
+from proxystore.store import register_store
 from proxystore.store import unregister_store
-from proxystore.store.file import FileStore
 from pytest import fixture
 
 from colmena.models import Result, ExecutableTask, SerializationMethod
 from colmena.task_server.base import run_and_record_timing
 
 
 # TODO (wardlt): Figure how to import this from test_models
@@ -40,32 +42,32 @@
     run_and_record_timing(func, result)
     result.deserialize()
     assert result.value == '1\n'
 
 
 @fixture
 def store(tmpdir):
-    store = FileStore(name='store', store_dir=tmpdir, stats=True)
-    yield store
-    unregister_store('store')
+    with Store('store', FileConnector(tmpdir), metrics=True) as store:
+        register_store(store)
+        yield store
+        unregister_store(store)
 
 
 def test_run_function(store):
     """Make sure the run function behaves as expected:
 
     - Records runtimes
     - Tracks proxy statistics
     """
 
     # Make the result and configure it to use the store
     result = Result(inputs=(('a' * 1024,), {}))
     result.proxystore_name = store.name
-    result.proxystore_type = f'{store.__class__.__module__}.{store.__class__.__name__}'
     result.proxystore_threshold = 128
-    result.proxystore_kwargs = store.kwargs
+    result.proxystore_config = store.config()
 
     # Serialize it
     result.serialization_method = SerializationMethod.PICKLE
     result.serialize()
 
     # Run the function
     run_and_record_timing(lambda x: x.upper(), result)
@@ -75,8 +77,8 @@
     assert result.time_async_resolve_proxies > 0
     assert result.time_deserialize_inputs > 0
     assert result.time_serialize_results > 0
     assert result.time_compute_ended > result.time_compute_started
 
     # Make sure we have stats for both proxies
     assert len(result.proxy_timing) == 2
-    assert all('set_bytes' in v for v in result.proxy_timing.values())
+    assert all('store.proxy' in v['times'] for v in result.proxy_timing.values())
```

### Comparing `colmena-0.4.5/colmena/task_server/tests/test_funcx.py` & `colmena-0.5.0/colmena/task_server/tests/test_globus.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from time import sleep
 from uuid import uuid4
 
 from pytest_mock import MockFixture
 from pytest import fixture, mark
 
 from colmena.queue.python import PipeQueues
-from colmena.task_server.funcx import FuncXTaskServer
+from colmena.task_server.globus import GlobusComputeTaskServer
 
 my_funcs: dict = {}
 
 
 class FakeClient:
-    """Faked FuncXClient that allows you to register functions"""
+    """Faked Client that allows you to register functions"""
 
     def register_function(self, new_func, function_name: str = None, **kwargs):
         global my_funcs
         uuid = uuid4()
         if function_name is None:
             function_name = new_func.__name__
         my_funcs[uuid] = (new_func, function_name)
@@ -42,30 +42,30 @@
         return new_future
 
     def shutdown(self):
         pass
 
 
 @fixture()
-def mock_funcx(mocker: MockFixture):
-    mocker.patch('colmena.task_server.funcx.FuncXExecutor', FakeExecutor)
+def mock_globus(mocker: MockFixture):
+    mocker.patch('colmena.task_server.globus.Executor', FakeExecutor)
 
 
 @mark.timeout(10)
-def test_mocked_server(mock_funcx):
+def test_mocked_server(mock_globus):
     # Create the task server with a single, no-op function
     client = FakeClient()
     queues = PipeQueues()
 
     def func(x):
         if x is None:
             raise MemoryError()
         return x
 
-    fts = FuncXTaskServer({func: 'fake_endp'}, client, queues)
+    fts = GlobusComputeTaskServer({func: 'fake_endp'}, client, queues)
     fts.start()
 
     # Submit a task to the queue and see how it works
     try:
         # Send a task that will execute properly
         queues.send_inputs(1, method='func')
         sleep(1)
```

### Comparing `colmena-0.4.5/colmena/task_server/tests/test_parsl.py` & `colmena-0.5.0/colmena/task_server/tests/test_parsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Tests for the Parsl implementation of the task server"""
 from typing import Tuple, List
 
 from parsl import HighThroughputExecutor
 from parsl.config import Config
 from pytest import fixture, mark
-import proxystore
-from proxystore.store.redis import RedisStore
+
+from proxystore.connectors.redis import RedisConnector
+from proxystore.store import Store
+from proxystore.store import register_store
+from proxystore.store import unregister_store
 
 from colmena.queue.base import ColmenaQueues
 
 from colmena.queue.python import PipeQueues
 from colmena.models import ResourceRequirements
 from .test_base import EchoTask, FakeMPITask
 from colmena.task_server.parsl import ParslTaskServer
@@ -42,19 +45,19 @@
         run_dir=str(tmpdir),
     )
 
 
 # Make a proxy store for larger objects
 @fixture(scope='module')
 def store():
-    store = RedisStore('store', hostname='localhost', port=6379, stats=True)
-    proxystore.store.register_store(store)
-    yield store
-    proxystore.store.unregister_store(store.name)
-    store.close()
+    connector = RedisConnector(hostname='localhost', port=6379)
+    with Store('store', connector=connector, metrics=True) as store:
+        register_store(store)
+        yield store
+        unregister_store(store.name)
 
 
 @fixture(autouse=True)
 def server_and_queue(config, store) -> Tuple[ParslTaskServer, ColmenaQueues]:
     queues = PipeQueues(proxystore_name='store', proxystore_threshold=5000, serialization_method='pickle')
     server = ParslTaskServer([f, capitalize, bad_task, EchoTask(), FakeMPITask(), count_nodes], queues, config)
     yield server, queues
```

### Comparing `colmena-0.4.5/colmena/tests/test_model.py` & `colmena-0.5.0/colmena/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/thinker/__init__.py` & `colmena-0.5.0/colmena/thinker/__init__.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/thinker/resources.py` & `colmena-0.5.0/colmena/thinker/resources.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/thinker/tests/test_resources.py` & `colmena-0.5.0/colmena/thinker/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena/thinker/tests/test_thinker.py` & `colmena-0.5.0/colmena/thinker/tests/test_thinker.py`

 * *Files identical despite different names*

### Comparing `colmena-0.4.5/colmena.egg-info/PKG-INFO` & `colmena-0.5.0/colmena.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colmena
-Version: 0.4.5
+Version: 0.5.0
 Summary: colmena: Intelligent Steerable Pipelines on HPC
 Author-email: Globus Labs <labs@globus.org>, Logan Ward <lward@anl.gov>, Greg Pauloski <jgpauloski@uchicago.edu>, Yadu Babuji <yadudoc1729@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -215,15 +215,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: funcx
+Provides-Extra: globus
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # Colmena
 
 [![CI](https://github.com/exalearn/colmena/actions/workflows/CI.yml/badge.svg)](https://github.com/exalearn/colmena/actions/workflows/CI.yml)
 [![Documentation Status](https://readthedocs.org/projects/colmena/badge/?version=latest)](https://colmena.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `colmena-0.4.5/colmena.egg-info/SOURCES.txt` & `colmena-0.5.0/colmena.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 colmena/queue/base.py
 colmena/queue/python.py
 colmena/queue/redis.py
 colmena/queue/tests/test_base.py
 colmena/queue/tests/test_queues.py
 colmena/task_server/__init__.py
 colmena/task_server/base.py
-colmena/task_server/funcx.py
+colmena/task_server/globus.py
 colmena/task_server/parsl.py
 colmena/task_server/tests/__init__.py
 colmena/task_server/tests/test_base.py
-colmena/task_server/tests/test_funcx.py
+colmena/task_server/tests/test_globus.py
 colmena/task_server/tests/test_parsl.py
 colmena/tests/test_model.py
 colmena/tests/test_proxy.py
 colmena/thinker/__init__.py
 colmena/thinker/resources.py
 colmena/thinker/tests/test_resources.py
 colmena/thinker/tests/test_thinker.py
```

### Comparing `colmena-0.4.5/pyproject.toml` & `colmena-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "colmena"
-version = "0.4.5"
+version = "0.5.0"
 authors = [
     { name = "Globus Labs", email = "labs@globus.org" },
     { name = "Logan Ward", email = "lward@anl.gov" },
     { name = "Greg Pauloski", email = "jgpauloski@uchicago.edu" },
     { name = "Yadu Babuji", email = "yadudoc1729@gmail.com" },
 ]
 description = 'colmena: Intelligent Steerable Pipelines on HPC'
@@ -21,27 +21,27 @@
     "Topic :: System :: Distributed Computing",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering"
 ]
 dependencies = [
     "parsl>=2022",
     "pydantic==1.*",
-    "redis==3.4.*",
-    "proxystore==0.4.*"
+    "redis>=4.3",
+    "proxystore==0.5.*"
 ]
 
 [tool.setuptools.packages.find]
 include = ['colmena*']
 
 [project.urls]
 repository = "https://github.com/exalearn/colmena"
 documentation = "https://colmena.readthedocs.io/"
 
 [project.optional-dependencies]
-funcx = ['funcx>=1.0.5']
+globus = ['globus-compute-sdk>=1.0.5']
 test = [
     'flake8',
     'pytest',
     'pytest-timeout',
     'pytest-mock',
     'pytest-repeat',
     'pytest-cov',
```

