# Comparing `tmp/ewoksdask-0.1.1.tar.gz` & `tmp/ewoksdask-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksdask-0.1.1.tar", last modified: Thu Mar  9 06:15:00 2023, max compression
+gzip compressed data, was "dist/ewoksdask-0.1.2.tar", last modified: Mon May 15 16:51:27 2023, max compression
```

## Comparing `ewoksdask-0.1.1.tar` & `ewoksdask-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-09 06:11:46.000000 ewoksdask-0.1.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1040 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-03-09 06:11:46.000000 ewoksdask-0.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-09 06:11:46.000000 ewoksdask-0.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-09 06:11:46.000000 ewoksdask-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/src/ewoksdask/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-09 06:11:46.000000 ewoksdask-0.1.1/src/ewoksdask/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5680 2023-03-09 06:11:46.000000 ewoksdask-0.1.1/src/ewoksdask/bindings.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-03-09 06:11:46.000000 ewoksdask-0.1.1/src/ewoksdask/schedulers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/src/ewoksdask/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 06:14:54.000000 ewoksdask-0.1.1/src/ewoksdask/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-03-09 06:11:46.000000 ewoksdask-0.1.1/src/ewoksdask/tests/test_examples.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-03-09 06:11:46.000000 ewoksdask-0.1.1/src/ewoksdask/tests/test_workflow_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/src/ewoksdask.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/src/ewoksdask.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/src/ewoksdask.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/src/ewoksdask.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      222 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/src/ewoksdask.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-09 06:15:00.000000 ewoksdask-0.1.1/src/ewoksdask.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-15 09:03:12.000000 ewoksdask-0.1.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-15 09:03:12.000000 ewoksdask-0.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-15 09:03:12.000000 ewoksdask-0.1.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-15 09:03:12.000000 ewoksdask-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/src/ewoksdask/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-15 16:46:02.000000 ewoksdask-0.1.2/src/ewoksdask/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5670 2023-05-15 15:49:45.000000 ewoksdask-0.1.2/src/ewoksdask/bindings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2023-05-15 09:03:12.000000 ewoksdask-0.1.2/src/ewoksdask/schedulers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/src/ewoksdask/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 16:51:21.000000 ewoksdask-0.1.2/src/ewoksdask/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-15 09:03:12.000000 ewoksdask-0.1.2/src/ewoksdask/tests/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-05-15 09:03:12.000000 ewoksdask-0.1.2/src/ewoksdask/tests/test_workflow_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/src/ewoksdask.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/src/ewoksdask.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/src/ewoksdask.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/src/ewoksdask.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/src/ewoksdask.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-15 16:51:27.000000 ewoksdask-0.1.2/src/ewoksdask.egg-info/top_level.txt
```

### Comparing `ewoksdask-0.1.1/LICENSE.md` & `ewoksdask-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksdask-0.1.1/PKG-INFO` & `ewoksdask-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdask
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dask binding for Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksdask/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksdask/
 Project-URL: Documentation, https://ewoksdask.readthedocs.io/
@@ -23,20 +23,20 @@
 # ewoksdask
 
 *ewoksdask* provides distributed task scheduling for [ewoks](https://ewoks.readthedocs.io/) workflows.
 
 ## Install
 
 ```bash
-python3 -m pip install ewoksdask[test]
+pip install ewoksdask[test]
 ```
 
 ## Test
 
 ```bash
-python3 -m pytest --pyargs ewoksdask.tests
+pytest --pyargs ewoksdask.tests
 ```
 
 ## Documentation
 
 https://ewoksdask.readthedocs.io/
```

### Comparing `ewoksdask-0.1.1/setup.cfg` & `ewoksdask-0.1.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	ewokscore >=0.3.1
+	ewokscore >=0.4.1
 	dask[distributed] >=2021.3.0
 	dask-jobqueue >=0.7.3
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
@@ -46,19 +46,14 @@
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 
-[build_sphinx]
-project = ewoksdask
-version = attr: ewoksdask.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
 [egg_info]
 tag_build =
```

### Comparing `ewoksdask-0.1.1/src/ewoksdask/bindings.py` & `ewoksdask-0.1.2/src/ewoksdask/bindings.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         inputs=dynamic_inputs,
         varinfo=execute_options.get("varinfo"),
         execinfo=execute_options.get("execinfo"),
     )
 
     task.execute()
 
-    return task.output_transfer_data
+    return task.get_output_transfer_data()
 
 
 def _create_dask_graph(ewoksgraph, **execute_options) -> dict:
     daskgraph = dict()
     for target_id, node_attrs in ewoksgraph.graph.nodes.items():
         source_ids = tuple(analysis.node_predecessors(ewoksgraph.graph, target_id))
         link_attrs = tuple(
@@ -85,15 +85,15 @@
         context = scheduler_options.pop("context", "spawn")
         dask.config.set({"multiprocessing.context": context})
         results = multiprocessing_scheduler(daskgraph, node_ids, **scheduler_options)
     elif scheduler == "multithreading":
         # num_workers: CPU_COUNT by default
         results = multithreading_scheduler(daskgraph, node_ids, **scheduler_options)
     elif scheduler == "cluster":
-        # n_worker: n worker with m threads (n_worker= n * m)
+        # n_workers: n workers with m threads
         with Client(**scheduler_options) as client:
             results = client.get(daskgraph, node_ids)
     elif isinstance(scheduler, str):
         with Client(address=scheduler, **scheduler_options) as client:
             results = client.get(daskgraph, node_ids)
     elif isinstance(scheduler, Client):
         results = client.get(daskgraph, node_ids)
```

### Comparing `ewoksdask-0.1.1/src/ewoksdask/schedulers.py` & `ewoksdask-0.1.2/src/ewoksdask/schedulers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dask.distributed import LocalCluster
 from dask_jobqueue import SLURMCluster
 
 
 def local_scheduler(**kw):
     """
-    :param n_worker:
+    :param n_workers:
     :param processes: True by default
     :param threads_per_worker:
     :param scheduler_port:
     :param dashboard_address:
     :param worker_dashboard_address:
     """
     # Run this on any machine
```

### Comparing `ewoksdask-0.1.1/src/ewoksdask/tests/test_examples.py` & `ewoksdask-0.1.2/src/ewoksdask/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ewoksdask-0.1.1/src/ewoksdask/tests/test_workflow_events.py` & `ewoksdask-0.1.2/src/ewoksdask/tests/test_workflow_events.py`

 * *Files identical despite different names*

### Comparing `ewoksdask-0.1.1/src/ewoksdask.egg-info/PKG-INFO` & `ewoksdask-0.1.2/src/ewoksdask.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdask
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dask binding for Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksdask/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksdask/
 Project-URL: Documentation, https://ewoksdask.readthedocs.io/
@@ -23,20 +23,20 @@
 # ewoksdask
 
 *ewoksdask* provides distributed task scheduling for [ewoks](https://ewoks.readthedocs.io/) workflows.
 
 ## Install
 
 ```bash
-python3 -m pip install ewoksdask[test]
+pip install ewoksdask[test]
 ```
 
 ## Test
 
 ```bash
-python3 -m pytest --pyargs ewoksdask.tests
+pytest --pyargs ewoksdask.tests
 ```
 
 ## Documentation
 
 https://ewoksdask.readthedocs.io/
```

