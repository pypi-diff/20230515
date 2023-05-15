# Comparing `tmp/ewokscore-0.4.0.tar.gz` & `tmp/ewokscore-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewokscore-0.4.0.tar", last modified: Mon Mar 27 15:52:10 2023, max compression
+gzip compressed data, was "dist/ewokscore-0.4.1.tar", last modified: Mon May 15 08:25:37 2023, max compression
```

## Comparing `ewokscore-0.4.0.tar` & `ewokscore-0.4.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-27 13:03:13.000000 ewokscore-0.4.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2622 2023-03-27 15:52:10.000000 ewokscore-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-03-27 13:03:13.000000 ewokscore-0.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-03-27 13:03:13.000000 ewokscore-0.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-03-27 15:52:10.000000 ewokscore-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-27 13:03:13.000000 ewokscore-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-27 15:50:12.000000 ewokscore-0.4.0/src/ewokscore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/bindings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/cliutils/
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/cliutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-03-27 15:36:25.000000 ewokscore-0.4.0/src/ewokscore/cliutils/cliconvertutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4893 2023-03-27 15:36:25.000000 ewokscore-0.4.0/src/ewokscore/cliutils/cliexecuteutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/cliutils/clilogutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-03-27 15:36:25.000000 ewokscore-0.4.0/src/ewokscore/cliutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/dynamictask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/events/
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/events/contexts.py
--rw-rw-rw-   0 root         (0) root         (0)     4996 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/events/global_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/events/handlers/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/events/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/events/handlers/base.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/events/handlers/sqlite3.py
--rw-rw-rw-   0 root         (0) root         (0)     1891 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/events/initialize_events.py
--rw-rw-rw-   0 root         (0) root         (0)     8067 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/events/send_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/graph/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12469 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/compare.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/error_handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/graph/execute/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 15:52:04.000000 ewokscore-0.4.0/src/ewokscore/graph/execute/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4888 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/execute/sequential.py
--rw-rw-rw-   0 root         (0) root         (0)     7008 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/multigraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/graph/schema/
--rw-rw-rw-   0 root         (0) root         (0)     4434 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/schema/v0_0.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/schema/v0_1.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/schema/v0_2.py
--rw-rw-rw-   0 root         (0) root         (0)     6805 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)    10936 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/subgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     5551 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/taskgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/graph/validate.py
--rw-rw-rw-   0 root         (0) root         (0)     8690 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     8557 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/inittask.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/methodtask.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/missing_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/persistence/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/persistence/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     5623 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/persistence/file.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/persistence/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/persistence/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     6064 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/persistence/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/persistence/uri.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/ppftasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3415 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2287 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/registration.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/scripttask.py
--rw-rw-rw-   0 root         (0) root         (0)    12629 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/task.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/taskwithprogress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 15:52:04.000000 ewokscore-0.4.0/src/ewokscore/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/discover_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 15:52:04.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4825 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/acyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/acyclic2.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/acyclic3.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/cyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     4139 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/demo.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/empty.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/triangle1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/loadtest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 15:52:04.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/loadtest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/loadtest/graph.json
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/loadtest/subgraph.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 15:52:04.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/addfunc.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/condsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/errorsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/nooutputtask.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/simplemethods.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/sumlist.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/sumtask.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-03-27 15:36:25.000000 ewokscore-0.4.0/src/ewokscore/tests/test_cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7990 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_default_error_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_dynamic_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     7317 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_execute_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     6597 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_graph_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2700 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_graph_start_end_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     7463 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_link_is_required.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_method_task.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_persistence.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_script_task.py
--rw-rw-rw-   0 root         (0) root         (0)     8223 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_sub_graph.py
--rw-rw-rw-   0 root         (0) root         (0)    10730 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_sub_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     4961 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_task_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_uri.py
--rw-rw-rw-   0 root         (0) root         (0)    14270 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_variable.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_variable_namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     7495 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/test_workflow_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 15:52:04.000000 ewokscore-0.4.0/src/ewokscore/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4910 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/tests/utils/show.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19364 2023-03-27 13:03:13.000000 ewokscore-0.4.0/src/ewokscore/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2622 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4175 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      264 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-27 15:52:10.000000 ewokscore-0.4.0/src/ewokscore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-15 07:53:03.000000 ewokscore-0.4.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-05-15 08:25:37.000000 ewokscore-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-05-15 07:53:03.000000 ewokscore-0.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-15 07:53:03.000000 ewokscore-0.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2023-05-15 08:25:37.000000 ewokscore-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-15 07:53:03.000000 ewokscore-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-15 08:23:36.000000 ewokscore-0.4.1/src/ewokscore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/bindings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/cliutils/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/cliconvertutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/cliexecuteutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/clilogutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/cliutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/dynamictask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/events/
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/contexts.py
+-rw-rw-rw-   0 root         (0) root         (0)     4996 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/global_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/events/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/handlers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/handlers/sqlite3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1891 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/initialize_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/events/send_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/graph/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12469 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/error_handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/graph/execute/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/graph/execute/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4888 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/execute/sequential.py
+-rw-rw-rw-   0 root         (0) root         (0)     7034 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/multigraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/v0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/v0_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/schema/v0_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6805 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)    10936 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/subgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5551 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/taskgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/graph/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8690 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8562 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/inittask.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/methodtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/missing_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     5623 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/file.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6064 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/persistence/uri.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/ppftasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3415 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/registration.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/scripttask.py
+-rw-rw-rw-   0 root         (0) root         (0)    14259 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/taskwithprogress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/discover_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/cyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4139 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/triangle1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/loadtest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/loadtest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/loadtest/graph.json
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/loadtest/subgraph.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/addfunc.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/condsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/errorsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/nooutputtask.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/simplemethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/sumlist.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/sumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7990 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_default_error_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_dynamic_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     7341 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_execute_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     6597 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_graph_start_end_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_link_is_required.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_method_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_persistence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_script_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     8223 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_sub_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    10730 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_sub_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_task_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_uri.py
+-rw-rw-rw-   0 root         (0) root         (0)    14406 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_variable_namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     7495 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/test_workflow_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 08:25:31.000000 ewokscore-0.4.1/src/ewokscore/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4916 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/tests/utils/show.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21246 2023-05-15 07:53:03.000000 ewokscore-0.4.1/src/ewokscore/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4175 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-15 08:25:37.000000 ewokscore-0.4.1/src/ewokscore.egg-info/top_level.txt
```

### Comparing `ewokscore-0.4.0/LICENSE.md` & `ewokscore-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/PKG-INFO` & `ewokscore-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.4.0
+Version: 0.4.1
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
```

### Comparing `ewokscore-0.4.0/README.md` & `ewokscore-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/setup.cfg` & `ewokscore-0.4.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -53,19 +53,14 @@
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 
-[build_sphinx]
-project = ewokscore
-version = attr: ewokscore.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
 [egg_info]
 tag_build =
```

### Comparing `ewokscore-0.4.0/src/ewokscore/bindings.py` & `ewokscore-0.4.1/src/ewokscore/bindings.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/cliutils/__init__.py` & `ewokscore-0.4.1/src/ewokscore/cliutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/cliutils/cliconvertutils.py` & `ewokscore-0.4.1/src/ewokscore/cliutils/cliconvertutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/cliutils/cliexecuteutils.py` & `ewokscore-0.4.1/src/ewokscore/cliutils/cliexecuteutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,16 +70,15 @@
         "--jobid",
         dest="job_id",
         type=str,
         default=None,
         help="Job id for ewoks events",
     )
     parser.add_argument(
-        "--disable_events",
-        dest="disable_events",
+        "--disable-events",
         action="store_true",
         help="Disable ewoks events",
     )
     parser.add_argument(
         "--sqlite3",
         dest="sqlite3_uri",
         type=str,
@@ -148,23 +147,22 @@
     if args.root_module:
         load_options["root_module"] = args.root_module
     if args.root_dir:
         load_options["root_dir"] = args.root_dir
     if args.representation:
         load_options["representation"] = args.representation
 
-    if not args.disable_events:
-        execinfo = dict()
-        execute_options["execinfo"] = execinfo
-        if args.job_id:
-            execinfo["job_id"] = args.job_id
-        if args.sqlite3_uri:
-            # TODO: asynchronous handling may loose events
-            execinfo["asynchronous"] = False
-            execinfo["handlers"] = [
-                {
-                    "class": "ewokscore.events.handlers.Sqlite3EwoksEventHandler",
-                    "arguments": [{"name": "uri", "value": args.sqlite3_uri}],
-                }
-            ]
+    execinfo = dict()
+    execute_options["execinfo"] = execinfo
+    if args.job_id:
+        execinfo["job_id"] = args.job_id
+    if args.sqlite3_uri:
+        # TODO: asynchronous handling may loose events
+        execinfo["asynchronous"] = False
+        execinfo["handlers"] = [
+            {
+                "class": "ewokscore.events.handlers.Sqlite3EwoksEventHandler",
+                "arguments": [{"name": "uri", "value": args.sqlite3_uri}],
+            }
+        ]
 
     args.execute_options = execute_options
```

### Comparing `ewokscore-0.4.0/src/ewokscore/cliutils/clilogutils.py` & `ewokscore-0.4.1/src/ewokscore/cliutils/clilogutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/cliutils/utils.py` & `ewokscore-0.4.1/src/ewokscore/cliutils/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/dynamictask.py` & `ewokscore-0.4.1/src/ewokscore/dynamictask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/events/__init__.py` & `ewokscore-0.4.1/src/ewokscore/events/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/events/contexts.py` & `ewokscore-0.4.1/src/ewokscore/events/contexts.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/events/global_state.py` & `ewokscore-0.4.1/src/ewokscore/events/global_state.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/events/initialize_events.py` & `ewokscore-0.4.1/src/ewokscore/events/initialize_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/events/send_events.py` & `ewokscore-0.4.1/src/ewokscore/events/send_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     else:
         engine_field = "binding"
     if binding:
         if engine:
             raise ValueError("'binding' and 'engine' cannot be used together")
         engine = binding
         if engine_field == "engine":
-            warn("'binding' is deprecated in favor of 'engine'", FutureWarning)
+            warn("'binding' is deprecated in favor of 'engine'", DeprecationWarning)
     event_data = {
         "host_name": host_name,
         "process_id": process_id,
         "user_name": user_name,
         "job_id": job_id,
         engine_field: engine,
         "type": event,
```

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/analysis.py` & `ewokscore-0.4.1/src/ewokscore/graph/analysis.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/compare.py` & `ewokscore-0.4.1/src/ewokscore/graph/compare.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/error_handlers.py` & `ewokscore-0.4.1/src/ewokscore/graph/error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/execute/sequential.py` & `ewokscore-0.4.1/src/ewokscore/graph/execute/sequential.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/graph_io.py` & `ewokscore-0.4.1/src/ewokscore/graph/graph_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,22 @@
     keys_to_update = "name", "value"
     for input_item in inputs:
         node_id = input_item.get("id")
         if node_id is None:
             continue
         node_attrs = graph.nodes[node_id]
         default_inputs = node_attrs.get("default_inputs")
+        input_item = {k: input_item[k] for k in keys_to_update}
         if default_inputs:
             for existing_input_item in default_inputs:
                 if existing_input_item["name"] == input_item["name"]:
-                    existing_input_item["value"] = input_item["value"]
+                    existing_input_item.update(input_item)
                     break
             else:
-                default_inputs.append({k: input_item[k] for k in keys_to_update})
+                default_inputs.append(input_item)
         else:
             node_attrs["default_inputs"] = [input_item]
 
 
 def parse_inputs(
     graph: networkx.DiGraph, inputs: Optional[List[dict]] = None
 ) -> List[dict]:
@@ -162,15 +163,15 @@
         task_output_values = None
     else:
         task_output_values = task_or_outputs
     for output_item in outputs:
         if output_item.get("id") != node_id:
             continue
         if task_output_values is None:
-            task_output_values = task_or_outputs.output_values
+            task_output_values = task_or_outputs.get_output_values()
         if output_values is None:
             output_values = dict()
         name = output_item.get("name")
         if name:
             new_name = output_item.get("new_name", name)
             output_values[new_name] = task_output_values.get(
                 name, missing_data.MISSING_DATA
```

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/multigraph.py` & `ewokscore-0.4.1/src/ewokscore/graph/multigraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/schema/__init__.py` & `ewokscore-0.4.1/src/ewokscore/graph/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/serialize.py` & `ewokscore-0.4.1/src/ewokscore/graph/serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/subgraph.py` & `ewokscore-0.4.1/src/ewokscore/graph/subgraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/taskgraph.py` & `ewokscore-0.4.1/src/ewokscore/graph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/graph/validate.py` & `ewokscore-0.4.1/src/ewokscore/graph/validate.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/hashing.py` & `ewokscore-0.4.1/src/ewokscore/hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/inittask.py` & `ewokscore-0.4.1/src/ewokscore/inittask.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     key = key.pop()
 
     if key == "task_type":
         task_type = node_attrs[key]
     else:
         warnings.warn(
             f"'{key}' is deprecated in favor of 'task_type' with 'task_identifier'",
-            FutureWarning,
+            DeprecationWarning,
         )
         value = node_attrs.pop(key)
         if key != "ppfport":
             node_attrs["task_identifier"] = value
         if key == "task":
             task_type = "generated"
         else:
```

### Comparing `ewokscore-0.4.0/src/ewokscore/methodtask.py` & `ewokscore-0.4.1/src/ewokscore/methodtask.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class MethodExecutorTask(
     Task, input_names=[METHOD_ARGUMENT], output_names=["return_value"]
 ):
     METHOD_ARGUMENT = METHOD_ARGUMENT
 
     def run(self):
-        kwargs = self.named_input_values
-        args = self.positional_input_values
+        kwargs = self.get_named_input_values()
+        args = self.get_positional_input_values()
         fullname = kwargs.pop(self.METHOD_ARGUMENT)
         method = import_method(fullname)
 
         result = method(*args, **kwargs)
 
         self.outputs.return_value = result
```

### Comparing `ewokscore-0.4.0/src/ewokscore/missing_data.py` & `ewokscore-0.4.1/src/ewokscore/missing_data.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/node.py` & `ewokscore-0.4.1/src/ewokscore/node.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/persistence/atomic.py` & `ewokscore-0.4.1/src/ewokscore/persistence/atomic.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/persistence/file.py` & `ewokscore-0.4.1/src/ewokscore/persistence/file.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/persistence/json.py` & `ewokscore-0.4.1/src/ewokscore/persistence/json.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/persistence/nexus.py` & `ewokscore-0.4.1/src/ewokscore/persistence/nexus.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/persistence/proxy.py` & `ewokscore-0.4.1/src/ewokscore/persistence/proxy.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/persistence/uri.py` & `ewokscore-0.4.1/src/ewokscore/persistence/uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/ppftasks.py` & `ewokscore-0.4.1/src/ewokscore/ppftasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     arguments and passed to the method.
     """
 
     METHOD_ARGUMENT = METHOD_ARGUMENT
     PPF_DICT_ARGUMENT = PPF_DICT_ARGUMENT
 
     def run(self):
-        method_kwargs = self.input_values
+        method_kwargs = self.get_input_values()
         fullname = method_kwargs.pop(self.METHOD_ARGUMENT)
         method = import_method(fullname)
         ppfdict = method_kwargs.pop(self.PPF_DICT_ARGUMENT, None)
         if ppfdict:
             method_kwargs.update(ppfdict)
 
         result = method(**method_kwargs)
@@ -37,12 +37,12 @@
     Task, optional_input_names=[PPF_DICT_ARGUMENT], output_names=[PPF_DICT_ARGUMENT]
 ):
     """A ppfmethod which represents the identity mapping"""
 
     PPF_DICT_ARGUMENT = PPF_DICT_ARGUMENT
 
     def run(self):
-        method_kwargs = self.input_values
+        method_kwargs = self.get_input_values()
         ppfdict = method_kwargs.pop(self.PPF_DICT_ARGUMENT, None)
         if ppfdict:
             method_kwargs.update(ppfdict)
         self.outputs._ppfdict = method_kwargs
```

### Comparing `ewokscore-0.4.0/src/ewokscore/progress.py` & `ewokscore-0.4.1/src/ewokscore/progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/registration.py` & `ewokscore-0.4.1/src/ewokscore/registration.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/scripttask.py` & `ewokscore-0.4.1/src/ewokscore/scripttask.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,13 +20,13 @@
             argmarker = "--"
             args.append(sys.executable)
         else:
             argmarker = "-"
             if not WIN32:
                 args.append("bash")
         args.append(fullname)
-        for k, v in self.input_values.items():
+        for k, v in self.get_input_values().items():
             if k != self.SCRIPT_ARGUMENT:
                 args.extend((argmarker + k, str(v)))
         result = subprocess.run(args)
         # result.check_returncode()
         self.outputs.return_code = result.returncode
```

### Comparing `ewokscore-0.4.0/src/ewokscore/task.py` & `ewokscore-0.4.1/src/ewokscore/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Optional, Union, Mapping
 
 from .hashing import UniversalHashable
 from .registration import Registered
 from .variable import VariableContainer
 from .variable import VariableContainerNamespace
 from .variable import ReadOnlyVariableContainerNamespace
@@ -194,31 +195,55 @@
     def get_input_value(self, key, default=missing_data.MISSING_DATA):
         if self.missing_inputs[key]:
             return default
         return self.inputs[key]
 
     @property
     def input_uhashes(self):
-        return self.input_variables.variable_uhashes
+        return self.get_input_uhashes()
+
+    def get_input_uhashes(self):
+        return self.__inputs.get_variable_uhashes()
 
     @property
     def input_values(self):
-        return self.input_variables.variable_values
+        warnings.warn(
+            "the property 'input_values' is deprecated in favor of the function 'get_input_values'",
+            DeprecationWarning,
+        )
+        return self.get_input_values()
+
+    def get_input_values(self):
+        return self.__inputs.get_variable_values()
 
     @property
     def named_input_values(self):
-        return self.input_variables.named_variable_values
+        warnings.warn(
+            "the property 'named_input_values' is deprecated in favor of the function 'get_named_input_values'",
+            DeprecationWarning,
+        )
+        return self.get_named_input_values()
+
+    def get_named_input_values(self):
+        return self.__inputs.get_named_variable_values()
 
     @property
     def positional_input_values(self):
-        return self.input_variables.positional_variable_values
+        warnings.warn(
+            "the property 'positional_input_values' is deprecated in favor of the function 'get_positional_input_values'",
+            DeprecationWarning,
+        )
+        return self.__inputs.get_positional_input_values()
+
+    def get_positional_input_values(self):
+        return self.__inputs.get_positional_variable_values()
 
     @property
     def npositional_inputs(self):
-        return self.input_variables.n_positional_variables
+        return self.__inputs.n_positional_variables
 
     @property
     def output_variables(self):
         return self.__outputs
 
     @property
     def missing_outputs(self):
@@ -231,24 +256,45 @@
     def get_output_value(self, key, default=missing_data.MISSING_DATA):
         if self.missing_outputs[key]:
             return default
         return self.outputs[key]
 
     @property
     def output_uhashes(self):
-        return self.__outputs.variable_uhashes
+        warnings.warn(
+            "the property 'output_uhashes' is deprecated in favor of the function 'get_output_uhashes'",
+            DeprecationWarning,
+        )
+        return self.get_output_uhashes()
+
+    def get_output_uhashes(self):
+        return self.__outputs.get_variable_uhashes()
 
     @property
     def output_values(self):
-        return self.__outputs.variable_values
+        warnings.warn(
+            "the property 'output_values' is deprecated in favor of the function 'get_output_values'",
+            DeprecationWarning,
+        )
+        return self.get_output_values()
+
+    def get_output_values(self):
+        return self.__outputs.get_variable_values()
 
     @property
     def output_transfer_data(self):
+        warnings.warn(
+            "the property 'output_transfer_data' is deprecated in favor of the function 'get_output_transfer_data'",
+            DeprecationWarning,
+        )
+        return self.get_output_transfer_data()
+
+    def get_output_transfer_data(self):
         """The values are either `DataUri` or `Variable`"""
-        return self.__outputs.variable_transfer_data
+        return self.__outputs.get_variable_transfer_data()
 
     @property
     def output_metadata(self) -> Union[dict, None]:
         return self.__outputs.metadata
 
     def _update_output_metadata(self):
         metadata = self.output_metadata
@@ -305,15 +351,15 @@
     @property
     def workflow_id(self) -> Optional[str]:
         if self.__execinfo:
             return self.__execinfo.get("workflow_id")
 
     def _iter_missing_input_values(self):
         for iname in self._INPUT_NAMES:
-            var = self.input_variables.get(iname)
+            var = self.__inputs.get(iname)
             if var is None or not var.has_value:
                 yield iname
 
     @property
     def is_ready_to_execute(self):
         try:
             next(iter(self._iter_missing_input_values()))
@@ -364,21 +410,21 @@
         """Send an ewoks event"""
         if self.__execinfo:
             events.send_task_event(execinfo=self.__execinfo, **kwargs)
 
     def _send_start_event(self):
         input_uris = [
             {"name": name, "value": str(uri) if uri else None}
-            for name, uri in self.input_variables.variable_uris.items()
+            for name, uri in self.__inputs.get_variable_uris().items()
         ]
         output_uris = [
             {"name": name, "value": str(uri) if uri else None}
-            for name, uri in self.output_variables.variable_uris.items()
+            for name, uri in self.__outputs.get_variable_uris().items()
         ]
-        task_uri = self.output_variables.data_uri
+        task_uri = self.__outputs.data_uri
         if task_uri:
             task_uri = str(task_uri)
         self._send_event(
             event="start",
             input_uris=input_uris,
             output_uris=output_uris,
             task_uri=task_uri,
```

### Comparing `ewokscore-0.4.0/src/ewokscore/task_discovery.py` & `ewokscore-0.4.1/src/ewokscore/task_discovery.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/taskwithprogress.py` & `ewokscore-0.4.1/src/ewokscore/taskwithprogress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/__init__.py` & `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/acyclic1.py` & `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/acyclic2.py` & `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic2.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/acyclic3.py` & `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/acyclic3.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/cyclic1.py` & `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/cyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/demo.py` & `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/demo.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/examples/graphs/triangle1.py` & `ewokscore-0.4.1/src/ewokscore/tests/examples/graphs/triangle1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/sumlist.py` & `ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/sumlist.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/examples/tasks/sumtask.py` & `ewokscore-0.4.1/src/ewokscore/tests/examples/tasks/sumtask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_cli_utils.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_default_error_handlers.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_default_error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_dynamic_tasks.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_dynamic_tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,8 +22,8 @@
         {
             "task_type": "generated",
             "task_identifier": task_name,
             "task_generator": qualname(task_class_generator),
         },
     )
     task.execute()
-    assert task.output_values == {"result": task_name}
+    assert task.get_output_values() == {"result": task_name}
```

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_events.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_examples.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_execute_graph.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_execute_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     output_names=["result", "inputs", "label"],
 ):
     def run(self):
         result = self.inputs.a
         if self.inputs.b:
             result += self.inputs.b
         self.outputs.result = result
-        self.outputs.inputs = {k: v for k, v in self.input_values.items() if v}
+        self.outputs.inputs = {k: v for k, v in self.get_input_values().items() if v}
         self.outputs.label = self.label
 
 
 def create_graph():
     task = qualname(SumTask)
     nodes = [
         {
@@ -103,15 +103,15 @@
         "nodes": nodes,
     }
 
 
 def test_execute_graph_outputs():
     # All task instances
     results = execute_graph(create_graph(), output_tasks=True)
-    results = {k: v.output_values for k, v in results.items()}
+    results = {k: v.get_output_values() for k, v in results.items()}
     expected = {
         "task1": {"inputs": {"a": 1}, "result": 1, "label": "task1"},
         "task3": {"inputs": {"a": 1, "b": 3}, "result": 4, "label": "task3"},
         "task2": {"inputs": {"a": 2}, "result": 2, "label": "task2"},
         "task4": {"inputs": {"a": 2, "b": 4}, "result": 6, "label": "task4"},
         "task5": {"inputs": {"a": 4, "b": 6}, "result": 10, "label": "task5"},
         "task6": {"inputs": {"a": 10, "b": 6}, "result": 16, "label": "task6"},
@@ -191,15 +191,15 @@
 
 def test_execute_graph_inputs():
     results = execute_graph(
         create_graph(),
         inputs=[{"id": "task1", "name": "b", "value": 1}],
         output_tasks=True,
     )
-    results = {k: v.output_values for k, v in results.items()}
+    results = {k: v.get_output_values() for k, v in results.items()}
     expected = {
         "task1": {"inputs": {"a": 1, "b": 1}, "result": 2, "label": "task1"},
         "task3": {"inputs": {"a": 2, "b": 3}, "result": 5, "label": "task3"},
         "task2": {"inputs": {"a": 2}, "result": 2, "label": "task2"},
         "task4": {"inputs": {"a": 2, "b": 4}, "result": 6, "label": "task4"},
         "task5": {"inputs": {"a": 5, "b": 6}, "result": 11, "label": "task5"},
         "task6": {"inputs": {"a": 11, "b": 6}, "result": 17, "label": "task6"},
@@ -208,15 +208,15 @@
     assert results == expected
 
     results = execute_graph(
         create_graph(),
         inputs=[{"name": "b", "value": 1}],
         output_tasks=True,
     )
-    results = {k: v.output_values for k, v in results.items()}
+    results = {k: v.get_output_values() for k, v in results.items()}
     expected = {
         "task1": {"inputs": {"a": 1, "b": 1}, "result": 2, "label": "task1"},
         "task3": {"inputs": {"a": 2, "b": 3}, "result": 5, "label": "task3"},
         "task2": {"inputs": {"a": 2, "b": 1}, "result": 3, "label": "task2"},
         "task4": {"inputs": {"a": 3, "b": 4}, "result": 7, "label": "task4"},
         "task5": {"inputs": {"a": 5, "b": 7}, "result": 12, "label": "task5"},
         "task6": {"inputs": {"a": 12, "b": 6}, "result": 18, "label": "task6"},
```

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_graph.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_graph_io.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_graph_io.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_graph_schema.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_graph_schema.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_graph_serialize.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_graph_start_end_nodes.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_graph_start_end_nodes.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_hashing.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_link_is_required.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_link_is_required.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_method_task.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_method_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     task = Task.instantiate(
         "MethodExecutorTask",
         inputs={"_method": qualname(mymethod1), "a": 3, "b": 5},
         varinfo=varinfo,
     )
     task.execute()
     assert task.done
-    assert task.output_values == {"return_value": 8}
+    assert task.get_output_values() == {"return_value": 8}
 
 
 def mymethod2(*args):
     return sum(args)
 
 
 def test_method_task2(varinfo):
     task = Task.instantiate(
         "MethodExecutorTask",
         inputs={"_method": qualname(mymethod2), 0: 3, 1: 5},
         varinfo=varinfo,
     )
     task.execute()
     assert task.done
-    assert task.output_values == {"return_value": 8}
+    assert task.get_output_values() == {"return_value": 8}
 
 
 def mymethod3(a, *args, b=None, c=3, **kw):
     print("a:", a)
     print("b:", b)
     print("c:", c)
     print("args:", args)
@@ -45,23 +45,23 @@
     task = Task.instantiate(
         "MethodExecutorTask",
         inputs={"_method": qualname(mymethod3), 0: 2, 1: 4, "b": 7, "d": 10},
         varinfo=varinfo,
     )
     task.execute()
     assert task.done
-    assert task.output_values == {"return_value": 26}
+    assert task.get_output_values() == {"return_value": 26}
 
 
 def myppfmethod(a=0, b=0, **kw):
     return {"a": a + b}
 
 
 def test_ppfmethod_task(varinfo):
     task = Task.instantiate(
         "PpfMethodExecutorTask",
         inputs={"_method": qualname(myppfmethod), "a": 3, "b": 5},
         varinfo=varinfo,
     )
     task.execute()
     assert task.done
-    assert task.output_values == {"_ppfdict": {"a": 8, "b": 5}}
+    assert task.get_output_values() == {"_ppfdict": {"a": 8, "b": 5}}
```

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_persistence.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_script_task.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_script_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_sub_graph.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_sub_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_sub_graph_serialize.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_sub_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_task.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,21 +156,21 @@
     task1 = MyTask(inputs={"mylist": obj})
     task2 = MyTask(inputs=task1.output_variables)
     task1.execute()
     task2.execute()
     assert len(gc.get_referrers(obj)) > nref_start
 
     uhash1 = task1.uhash
-    uhashes1 = task1.output_uhashes
+    uhashes1 = task1.get_output_uhashes()
     uhash2 = task2.uhash
-    uhashes2 = task2.output_uhashes
+    uhashes2 = task2.get_output_uhashes()
 
     task1.cleanup_references()
 
     while gc.collect():
         pass
     assert len(gc.get_referrers(obj)) == nref_start
 
     assert uhash1 == task1.uhash
-    assert uhashes1 == task1.output_uhashes
+    assert uhashes1 == task1.get_output_uhashes()
     assert uhash2 == task2.uhash
-    assert uhashes2 == task2.output_uhashes
+    assert uhashes2 == task2.get_output_uhashes()
```

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_task_discovery.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_task_discovery.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_task_progress.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_task_progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_uri.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_variable.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,24 +264,29 @@
     container.metadata["myvalue"] = 999
     container["var1"].metadata["myvalue"] = 888
     container.dump()
 
     # Common ways to receive data
     ref_uri = MutableVariableContainer(data_uri=container.data_uri)
     ref_transfer_data = MutableVariableContainer(
-        value=container.variable_transfer_data, varinfo={"has_data_proxy": True}
+        value=container.get_variable_transfer_data(), varinfo={"has_data_proxy": True}
     )
     assert ref_uri.uhash == container.uhash
     assert ref_transfer_data.uhash == container.uhash
 
     # Check data
-    assert container.variable_values == ref_transfer_data.variable_values
-    assert container.variable_transfer_data == ref_transfer_data.variable_transfer_data
-    assert container.variable_values == ref_uri.variable_values
-    assert container.variable_transfer_data == ref_uri.variable_transfer_data
+    assert container.get_variable_values() == ref_transfer_data.get_variable_values()
+    assert (
+        container.get_variable_transfer_data()
+        == ref_transfer_data.get_variable_transfer_data()
+    )
+    assert container.get_variable_values() == ref_uri.get_variable_values()
+    assert (
+        container.get_variable_transfer_data() == ref_uri.get_variable_transfer_data()
+    )
 
     # Check metadata
     if scheme == "nexus":
         if root_uri_type == "path_in_file":
             assert ref_uri.metadata["@NX_class"] == "NXcollection"
         else:
             assert ref_uri.metadata["@NX_class"] == "NXprocess"
@@ -374,15 +379,15 @@
 
 
 def test_variable_container_uri(tmpdir):
     var1 = VariableContainer(value={"a": 1, "b": 2}, varinfo={"root_uri": str(tmpdir)})
     var1.dump()
 
     var2 = VariableContainer(data_uri=str(var1.data_uri))
-    assert var1.variable_values == {"a": 1, "b": 2}
+    assert var1.get_variable_values() == {"a": 1, "b": 2}
     assert var1.value == var2.value
     assert var1 == var2
 
 
 @pytest.mark.parametrize("scheme", ("json", "nexus"))
 def test_variable_none_dump(scheme, tmpdir):
     var = Variable(value=None, varinfo={"root_uri": str(tmpdir), "scheme": scheme})
@@ -392,30 +397,30 @@
 
 def test_variable_container_values():
     c = MutableVariableContainer(
         value={"a": None, "b": MISSING_DATA, 2: "Two", 3: MISSING_DATA}
     )
     assert not c["a"].is_missing()
     assert c["b"].is_missing()
-    assert c.variable_values == {"a": None, 2: "Two"}
-    assert c.named_variable_values == {"a": None}
-    assert c.positional_variable_values == (
+    assert c.get_variable_values() == {"a": None, 2: "Two"}
+    assert c.get_named_variable_values() == {"a": None}
+    assert c.get_positional_variable_values() == (
         MISSING_DATA,
         MISSING_DATA,
         "Two",
         MISSING_DATA,
     )
 
     c["a"] = MISSING_DATA
     c["b"] = None
     c[1] = "One"
     c[2] = MISSING_DATA
     assert c["a"].is_missing()
     assert not c["b"].is_missing()
-    assert c.variable_values == {"b": None, 1: "One"}
-    assert c.named_variable_values == {"b": None}
-    assert c.positional_variable_values == (
+    assert c.get_variable_values() == {"b": None, 1: "One"}
+    assert c.get_named_variable_values() == {"b": None}
+    assert c.get_positional_variable_values() == (
         MISSING_DATA,
         "One",
         MISSING_DATA,
         MISSING_DATA,
     )
```

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_variable_namespaces.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_variable_namespaces.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/test_workflow_events.py` & `ewokscore-0.4.1/src/ewokscore/tests/test_workflow_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/tests/utils/results.py` & `ewokscore-0.4.1/src/ewokscore/tests/utils/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             expected_value = dict()
 
     if expected_value is None:
         assert not task.done, node_id
     else:
         assert task.done, node_id
         try:
-            assert task.output_values == expected_value, node_id
+            assert task.get_output_values() == expected_value, node_id
         except AssertionError:
             raise
         except Exception as e:
             raise RuntimeError(f"{node_id} does not have a result") from e
 
 
 def assert_result(value, expected_value, varinfo: Optional[dict] = None):
```

### Comparing `ewokscore-0.4.0/src/ewokscore/utils.py` & `ewokscore-0.4.1/src/ewokscore/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.4.0/src/ewokscore/variable.py` & `ewokscore-0.4.1/src/ewokscore/variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Any, Dict, Optional, Union
 from numbers import Integral
 from collections.abc import Mapping, MutableMapping, Iterable, Sequence
 
 from . import hashing
 from . import missing_data
 from .persistence import instantiate_data_proxy
@@ -416,57 +417,106 @@
     def force_non_existing(self):
         super().force_non_existing()
         for v in self.values():
             v.force_non_existing()
 
     @property
     def variable_uhashes(self):
+        warnings.warn(
+            "the property 'variable_uhashes' is deprecated in favor of the function 'get_variable_uhashes'",
+            DeprecationWarning,
+        )
+        return self.get_variable_uhashes()
+
+    def get_variable_uhashes(self):
         return {name: var.uhash for name, var in self.items()}
 
     @property
     def variable_values(self):
+        warnings.warn(
+            "the property 'variable_values' is deprecated in favor of the function 'get_variable_values'",
+            DeprecationWarning,
+        )
+        return self.get_variable_values()
+
+    def get_variable_values(self):
         return {k: v.value for k, v in self.items() if not v.is_missing()}
 
     @property
     def variable_data_proxies(self):
+        warnings.warn(
+            "the property 'variable_data_proxies' is deprecated in favor of the function 'get_variable_data_proxies'",
+            DeprecationWarning,
+        )
+        return self.get_variable_data_proxies()
+
+    def get_variable_data_proxies(self):
         return {k: v.data_proxy for k, v in self.items()}
 
     @property
     def variable_uris(self):
+        warnings.warn(
+            "the property 'variable_uris' is deprecated in favor of the function 'get_variable_uris'",
+            DeprecationWarning,
+        )
+        return self.get_variable_uris()
+
+    def get_variable_uris(self):
         uris = dict()
         for k, v in self.items():
             proxy = v.data_proxy
             if proxy:
                 uris[k] = proxy.uri
         return uris
 
     @property
     def variable_transfer_data(self):
+        warnings.warn(
+            "the property 'variable_transfer_data' is deprecated in favor of the function 'get_variable_transfer_data'",
+            DeprecationWarning,
+        )
+        return self.get_variable_transfer_data()
+
+    def get_variable_transfer_data(self):
         """Transfer data by variable or URI"""
         data = dict()
         for name, var in self.items():
             if var.has_persistent_value:
                 data[name] = var.data_proxy.uri
             elif var.hashing_enabled:
                 # Remove possible references to a uhashable
                 data[name] = var.copy_without_references()
             else:
                 data[name] = var.value
         return data
 
     @property
     def named_variable_values(self):
+        warnings.warn(
+            "the property 'named_variable_values' is deprecated in favor of the function 'get_named_variable_values'",
+            DeprecationWarning,
+        )
+        return self.get_named_variable_values()
+
+    def get_named_variable_values(self):
         return {
             k: v.value
             for k, v in self.items()
             if isinstance(k, str) and not v.is_missing()
         }
 
     @property
     def positional_variable_values(self):
+        warnings.warn(
+            "the property 'positional_variable_values' is deprecated in favor of the function 'get_positional_variable_values'",
+            DeprecationWarning,
+        )
+        return self.get_positional_variable_values()
+
+    def get_positional_variable_values(self):
         values = [self.MISSING_DATA] * self.__npositional_vars
         for i, var in self.items():
             if isinstance(i, int):
                 values[i] = var.value
         return tuple(values)
```

### Comparing `ewokscore-0.4.0/src/ewokscore.egg-info/PKG-INFO` & `ewokscore-0.4.1/src/ewokscore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.4.0
+Version: 0.4.1
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
```

### Comparing `ewokscore-0.4.0/src/ewokscore.egg-info/SOURCES.txt` & `ewokscore-0.4.1/src/ewokscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

