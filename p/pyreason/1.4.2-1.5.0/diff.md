# Comparing `tmp/pyreason-1.4.2.tar.gz` & `tmp/pyreason-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.4.2.tar", last modified: Fri May 12 16:47:53 2023, max compression
+gzip compressed data, was "pyreason-1.5.0.tar", last modified: Mon May 15 05:16:20 2023, max compression
```

## Comparing `pyreason-1.4.2.tar` & `pyreason-1.5.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-12 16:47:42.000000 pyreason-1.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 16:47:42.000000 pyreason-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-12 16:47:53.772425 pyreason-1.4.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-12 16:47:42.000000 pyreason-1.4.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    27566 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/facts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    65031 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10162 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:47:53.772425 pyreason-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-12 16:47:42.000000 pyreason-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.990558 pyreason-1.5.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-15 05:16:04.000000 pyreason-1.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 05:16:04.000000 pyreason-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-15 05:16:20.990558 pyreason-1.5.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-15 05:16:04.000000 pyreason-1.5.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.982558 pyreason-1.5.0/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.982558 pyreason-1.5.0/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.982558 pyreason-1.5.0/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27566 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.986558 pyreason-1.5.0/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.986558 pyreason-1.5.0/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.986558 pyreason-1.5.0/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.986558 pyreason-1.5.0/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/facts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.986558 pyreason-1.5.0/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70076 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.986558 pyreason-1.5.0/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.986558 pyreason-1.5.0/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.990558 pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10901 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.990558 pyreason-1.5.0/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.990558 pyreason-1.5.0/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.990558 pyreason-1.5.0/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/utils/plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9056 2023-05-15 05:16:04.000000 pyreason-1.5.0/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:16:20.982558 pyreason-1.5.0/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-15 05:16:20.000000 pyreason-1.5.0/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 05:16:20.000000 pyreason-1.5.0/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 05:16:20.000000 pyreason-1.5.0/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 05:16:20.000000 pyreason-1.5.0/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 05:16:20.000000 pyreason-1.5.0/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 05:16:20.990558 pyreason-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 05:16:04.000000 pyreason-1.5.0/setup.py
```

### Comparing `pyreason-1.4.2/LICENSE.md` & `pyreason-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/PKG-INFO` & `pyreason-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.4.2
+Version: 1.5.0
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.4.2/README.md` & `pyreason-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/__init__.py` & `pyreason-1.5.0/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.5.0/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.5.0/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.5.0/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/pyreason.py` & `pyreason-1.5.0/pyreason/pyreason.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.5.0/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/args.py` & `pyreason-1.5.0/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/components/world.py` & `pyreason-1.5.0/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/diffuse.py` & `pyreason-1.5.0/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.5.0/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/facts/fact_node.py` & `pyreason-1.5.0/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.5.0/pyreason/scripts/interpretation/interpretation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # Types for the dictionaries
 node_type = numba.types.string
 edge_type = numba.types.UniTuple(numba.types.string, 2)
 
 # Type for storing list of qualified nodes
 list_of_nodes = numba.types.ListType(node_type)
 
+# Type for storing int tuple
+int_tuple = numba.types.UniTuple(numba.types.int64, 2)
 
 
 class Interpretation:
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(node_type))
 	specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(edge_type))
@@ -33,22 +35,22 @@
 		self.time = 0
 
 		# Initialize list of tuples for rules/facts to be applied, along with all the ground atoms that fired the rule. One to One correspondence between rules_to_be_applied_node and rules_to_be_applied_node_trace if atom_trace is true
 		self.rules_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.rules_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.facts_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.string)
 		self.facts_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.string)
-		self.rules_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, node_type, label.label_type, interval.interval_type)))
-		self.rules_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, edge_type, label.label_type, interval.interval_type)))
+		self.rules_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, node_type, label.label_type, interval.interval_type, numba.types.boolean)))
+		self.rules_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, edge_type, label.label_type, interval.interval_type, numba.types.boolean)))
 		self.facts_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, node_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
 		self.facts_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, edge_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
 		self.edges_to_be_added_node_rule = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(node_type), numba.types.ListType(node_type), label.label_type)))
 		self.edges_to_be_added_edge_rule = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(node_type), numba.types.ListType(node_type), label.label_type)))
 
-		# Keep track of all the rules that have affeceted each node/edge at each timestep/fp operation, and all ground atoms that have affected the rules as well. Keep track of previous bounds and name of the rule/fact here
+		# Keep track of all the rules that have affected each node/edge at each timestep/fp operation, and all ground atoms that have affected the rules as well. Keep track of previous bounds and name of the rule/fact here
 		self.rule_trace_node_atoms = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), interval.interval_type, numba.types.string)))
 		self.rule_trace_edge_atoms = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), interval.interval_type, numba.types.string)))
 		self.rule_trace_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, numba.types.int8, node_type, label.label_type, interval.interval_type)))
 		self.rule_trace_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, numba.types.int8, edge_type, label.label_type, interval.interval_type)))
 
 		# Nodes and edges of the graph
 		self.nodes = numba.typed.List(self.graph.nodes())
@@ -195,14 +197,22 @@
 
 			# Convergence parameters
 			changes_cnt = 0
 			bound_delta = 0
 			max_rules_time = 0
 			update = False
 
+			# Parameters for immediate rules
+			immediate_node_rule_fire = False
+			immediate_edge_rule_fire = False
+			immediate_rule_applied = False
+			# When delta_t = 0, we don't want to check the same rule with the same node/edge after coming back to the fp operator
+			nodes_to_skip = numba.typed.List.empty_list(int_tuple)
+			edges_to_skip = numba.typed.List.empty_list(int_tuple)
+
 			# Start by applying facts
 			# Nodes
 			for i in range(len(facts_to_be_applied_node)):
 				if facts_to_be_applied_node[i][0]==t:
 					comp, l, bnd, static, graph_attribute = facts_to_be_applied_node[i][1], facts_to_be_applied_node[i][2], facts_to_be_applied_node[i][3], facts_to_be_applied_node[i][4], facts_to_be_applied_node[i][5]
 					# Check if bnd is static. Then no need to update, just add to rule trace, check if graph attribute and add ipl complement to rule trace as well
 					if interpretations_node[comp].world[l].is_static():
@@ -309,16 +319,21 @@
 			while in_loop:
 				# This will become true only if delta_t = 0 for some rule, otherwise we go to the next timestep
 				in_loop = False
 
 				# Apply the rules that need to be applied at this timestep
 				# Nodes
 				for idx, i in enumerate(rules_to_be_applied_node):
+					# If we are coming here from an immediate rule firing with delta_t=0 we have to apply that one rule. Which was just added to the list to_be_applied
+					if immediate_node_rule_fire and rules_to_be_applied_node[-1][4]:
+						i = rules_to_be_applied_node[-1]
+						idx = -1
+
 					if i[0]==t:
-						comp, l, bnd = i[1], i[2], i[3]
+						comp, l, bnd, immediate = i[1], i[2], i[3], i[4]
 						sources, targets, edge_l = edges_to_be_added_node_rule[idx]
 						edges_added, changes = _add_edges(sources, targets, neighbors, nodes, edges, edge_l, interpretations_node, interpretations_edge)
 						changes_cnt += changes
 
 						# Update bound for newly added edges. Use bnd to update all edges if label is specified, else use bnd to update normally
 						if edge_l.value!='':
 							for e in edges_added:
@@ -368,21 +383,33 @@
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 
 						# Delete rules that have been applied from list by changing t to -1
-						rules_to_be_applied_node[idx] = (numba.types.int8(-1), comp, l, bnd)
+						rules_to_be_applied_node[idx] = (numba.types.int8(-1), comp, l, bnd, False)
 
+						# Break out of the apply rules loop if a rule is immediate. Then we go to the fp operator and check for other applicable rules then come back
+						if immediate:
+							# If delta_t=0 we want to apply one rule and go back to the fp operator
+							# If delta_t>0 we want to come back here and apply the rest of the rules
+							if not immediate_node_rule_fire:
+								immediate_rule_applied = True
+							break
 
 				# Edges
 				for idx, i in enumerate(rules_to_be_applied_edge):
+					# If we are coming here from an immediate rule firing with delta_t=0 we have to apply that one rule. Which was just added to the list to_be_applied
+					if immediate_edge_rule_fire and rules_to_be_applied_edge[-1][4]:
+						i = rules_to_be_applied_edge[-1]
+						idx = -1
+
 					if i[0]==t:
-						comp, l, bnd = i[1], i[2], i[3]
+						comp, l, bnd, immediate = i[1], i[2], i[3], i[4]
 						sources, targets, edge_l = edges_to_be_added_edge_rule[idx]
 						edges_added, changes = _add_edges(sources, targets, neighbors, nodes, edges, edge_l, interpretations_node, interpretations_edge)
 						changes_cnt += changes
 
 						# Update bound for newly added edges. Use bnd to update all edges if label is specified, else use bnd to update normally
 						if edge_l.value!='':
 							for e in edges_added:
@@ -411,77 +438,141 @@
 										else:
 											changes_cnt += changes
 
 						else:
 							# Check for inconsistencies
 							if check_consistent_edge(interpretations_edge, comp, (l, bnd)):
 								u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode='rule')
-								
+
 								update = u or update
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 							# Resolve inconsistency
 							else:
 								if inconsistency_check:
 									resolve_inconsistency_edge(interpretations_edge, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms)
 								else:
 									u, changes = _override_update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode='rule')
-								
+
 									update = u or update
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 
 						# Delete rules that have been applied from list by changing t to -1
-						rules_to_be_applied_edge[idx] = (numba.types.int8(-1), comp, l, bnd)
+						rules_to_be_applied_edge[idx] = (numba.types.int8(-1), comp, l, bnd, False)
 
+						# Break out of the apply rules loop if a rule is immediate. Then we go to the fp operator and check for other applicable rules then come back
+						if immediate:
+							# If t=0 we want to apply one rule and go back to the fp operator
+							# If t>0 we want to come back here and apply the rest of the rules
+							if not immediate_edge_rule_fire:
+								immediate_rule_applied = True
+							break
 
 				# Fixed point
+				# if update or immediate_node_rule_fire or immediate_edge_rule_fire or immediate_rule_applied:
 				if update:
-					fp_cnt += 1
-					for rule in rules:
+					# Increase fp operator count only if not an immediate rule
+					if not (immediate_node_rule_fire or immediate_edge_rule_fire):
+						fp_cnt += 1
+
+					for i in range(len(rules)):
+						rule = rules[i]
+						immediate_rule = rule.is_immediate_rule()
+						immediate_node_rule_fire = False
+						immediate_edge_rule_fire = False
 						# Go through all nodes and check if any rules apply to them
-						# Only go through everything if the rule can be applied within the given timesteps. Otherwise it's an unnecessary loop
-						if t+rule.get_delta()<=tmax or tmax==-1:
-							for n in nodes:
+						# Only go through everything if the rule can be applied within the given timesteps, or we're running until convergence or it's an immediate rule.
+						# Otherwise, it's an unnecessary loop
+						delta_t = rule.get_delta()
+						if t+delta_t<=tmax or tmax==-1:
+							for j in range(len(nodes)):
+								if (i, j) in nodes_to_skip:
+									continue
+								n = nodes[j]
 								target_criteria_satisfaction = are_satisfied_node(interpretations_node, n, rule.get_target_criteria())
 								if (target_criteria_satisfaction and is_satisfied_node(interpretations_node, n, (rule.get_target(), interval.closed(0,1)))) or (target_criteria_satisfaction and rule.get_target().value==''):
 									result, annotations, qualified_nodes, qualified_edges, edges_to_add = _is_rule_applicable(interpretations_node, interpretations_edge, neighbors, n, rule.get_neigh_criteria(), rule.get_thresholds(), reverse_graph, rule.get_annotation_function(), rule.get_annotation_label(), rule.get_edges(), atom_trace)
 									if (result and rule.get_target().value=='') or (result and not interpretations_node[n].world[rule.get_target()].is_static()):
 										bnd = influence(rule, annotations, rule.get_weights())
-										max_rules_time = max(max_rules_time, t+rule.get_delta())
+										max_rules_time = max(max_rules_time, t+delta_t)
 										edges_to_be_added_node_rule.append(edges_to_add)
-										rules_to_be_applied_node.append((numba.types.int8(t+rule.get_delta()), n, rule.get_target(), bnd))
+										rules_to_be_applied_node.append((numba.types.int8(t+delta_t), n, rule.get_target(), bnd, immediate_rule))
 										if atom_trace:
 											rules_to_be_applied_node_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
-										if rule.get_delta()==0:
+
+										# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
+										nodes_to_skip.append((i, j))
+
+										# Handle loop parameters for the next (maybe) fp operation
+										# If it is a t=0 rule or an immediate rule we want to go back for another fp operation to check for new rules that may fire
+										# Next fp operation we will skip this rule on this node because anyway there won't be an update
+										if delta_t==0:
 											in_loop = True
 											update = False
+										if immediate_rule and delta_t==0:
+											# immediate_rule_fire becomes True because we still need to check for more eligible rules, we're not done.
+											in_loop = True
+											update = False
+											immediate_node_rule_fire = True
+											break
+
+							# Break, apply immediate rule then come back to check for more applicable rules
+							if immediate_node_rule_fire:
+								break
+
 							# Go through all edges and check if any rules apply to them.
 							# Comment out the following lines if there are no labels or rules that deal with edges. It will be an unnecessary loop
-							for e in edges:
+							for j in range(len(edges)):
+								if (i, j) in edges_to_skip:
+									continue
+								e = edges[j]
 								target_criteria_satisfaction = are_satisfied_edge(interpretations_edge, e, rule.get_target_criteria())
 								if (target_criteria_satisfaction and is_satisfied_node(interpretations_edge, e, (rule.get_target(), interval.closed(0,1)))) or (target_criteria_satisfaction and rule.get_target().value==''):
-									# Find out if rule is applicable. returns list of list of qualified nodes and qualified edges. one for each clause
+									# Find out if rule is applicable. returns list of list, of qualified nodes and qualified edges. one for each clause
 									result, annotations, qualified_nodes, qualified_edges, edges_to_add = _is_rule_applicable_edge(interpretations_node, interpretations_edge, neighbors, e, rule.get_neigh_criteria(), rule.get_thresholds(), reverse_graph, rule.get_annotation_function(), rule.get_annotation_label(), rule.get_edges(), atom_trace)
 									if (result and rule.get_target().value=='') or (result and not interpretations_edge[e].world[rule.get_target()].is_static()):
 										bnd = influence(rule, annotations, rule.get_weights())
-										max_rules_time = max(max_rules_time, t+rule.get_delta())
+										max_rules_time = max(max_rules_time, t+delta_t)
 										edges_to_be_added_edge_rule.append(edges_to_add)
-										rules_to_be_applied_edge.append((numba.types.int8(t+rule.get_delta()), e, rule.get_target(), bnd))
+										rules_to_be_applied_edge.append((numba.types.int8(t+delta_t), e, rule.get_target(), bnd, immediate_rule))
 										if atom_trace:
 											rules_to_be_applied_edge_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
-										if rule.get_delta()==0:
+
+										# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
+										edges_to_skip.append((i, j))
+
+										# Handle loop parameters for the next (maybe) fp operation
+										# If it is a t=0 rule or an immediate rule we want to go back for another fp operation to check for new rules that may fire
+										# Next fp operation we will skip this rule on this node because anyway there won't be an update
+										if delta_t==0:
 											in_loop = True
 											update = False
+										if immediate_rule and delta_t == 0:
+											# immediate_rule_fire becomes True because we still need to check for more eligible rules, we're not done.
+											in_loop = True
+											update = False
+											immediate_edge_rule_fire = True
+											break
+
+							# Break, apply immediate rule then come back to check for more applicable rules
+							if immediate_edge_rule_fire:
+								break
+								
+					# Go through all the rules and go back to applying the rules if we came here because of an immediate rule where delta_t>0
+					if immediate_rule_applied and not (immediate_node_rule_fire or immediate_edge_rule_fire):
+						immediate_rule_applied = False
+						in_loop = True
+						update = False
 				
 			# Check for convergence after each timestep (perfect convergence or convergence specified by user)
 			# Check number of changed interpretations or max bound change
 			# User specified convergence
 			if convergence_mode=='delta_interpretation':
 				if changes_cnt <= convergence_delta:
 					if verbose:
@@ -501,22 +592,21 @@
 						print(f'\nConverged at time: {t}')					
 					break
 
 			# Increment t
 			t += 1
 
 		return fp_cnt, t	
-		
 
 
 @numba.njit(cache=True)
 def _is_rule_applicable(interpretations_node, interpretations_edge, neighbors, target_node, neigh_criteria, thresholds, reverse_graph, ann_fn, ann_fn_label, edges, atom_trace):
 	# Initialize dictionary where keys are strings (x1, x2 etc.) and values are lists of qualified neighbors
 	# Keep track of all the edges that are qualified
-	# If its a node clause update (x1 or x2 etc.) qualified neighbors, if its an edge clause update the qualified neighbors for the source and target (x1, x2)
+	# If it's a node clause update (x1 or x2 etc.) qualified neighbors, if it's an edge clause update the qualified neighbors for the source and target (x1, x2)
 	# First gather all the qualified nodes for each clause
 	subsets = numba.typed.Dict.empty(key_type=numba.types.string, value_type=list_of_nodes)
 	qualified_nodes = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 	qualified_edges = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 	annotations = numba.typed.List.empty_list(numba.typed.List.empty_list(interval.interval_type))
 	edges_to_be_added = (numba.typed.List.empty_list(node_type), numba.typed.List.empty_list(node_type), edges[-1])
 
@@ -527,44 +617,49 @@
 	# 4. Collect edges and nodes to be added to the graph when rule fires
 
 	# 1.
 	satisfaction = True
 	for i, clause in enumerate(neigh_criteria):
 		# Gather qualified nodes/edges
 		if clause[0]=='node':
-			subset = neighbors[target_node] if clause[1][0] not in subsets else subsets[clause[1][0]]
+			if clause[1][0]=='target':
+				subset = numba.typed.List([target_node])
+			else:
+				subset = neighbors[target_node] if clause[1][0] not in subsets else subsets[clause[1][0]]
+
 			subsets[clause[1][0]] = get_qualified_components_node_clause(interpretations_node, subset, clause[2], clause[3])
 			if atom_trace:
 				qualified_nodes.append(numba.typed.List(subsets[clause[1][0]]))
 				qualified_edges.append(numba.typed.List.empty_list(edge_type))
 
 		elif clause[0]=='edge':
 			# Set sources for possible edges, if target use target node as source
-			subset_source = neighbors[target_node] if clause[1][0] not in subsets else subsets[clause[1][0]]
 			if clause[1][0]=='target':
 				subset_source = numba.typed.List([target_node])
-				
-			subset_target = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
-			for source in subset_source:
-				subset_target.append(neighbors[source] if clause[1][1] not in subsets else subsets[clause[1][1]])
+			else:
+				subset_source = neighbors[target_node] if clause[1][0] not in subsets else subsets[clause[1][0]]
 
-			# Set targets for possible edges, if target use target node as target
+			subset_target = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 			if clause[1][1]=='target':
+				# Set targets for possible edges, if target use target node as target
 				for source in subset_source:
 					subset_target.append(numba.typed.List([target_node]))
+			else:
+				for source in subset_source:
+					subset_target.append(neighbors[source] if clause[1][1] not in subsets else subsets[clause[1][1]])
 
 			qe = get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause[2], clause[3], reverse_graph)
 			subsets[clause[1][0]] = qe[0]
 			subsets[clause[1][1]] = qe[1]
 
 			if atom_trace:
 				qualified_nodes.append(numba.typed.List.empty_list(node_type))
 				qualified_edges.append(numba.typed.List(zip(subsets[clause[1][0]], subsets[clause[1][1]])))
 
-		# Check if clause satisfies threshold
+		# Check if the clause satisfies threshold
 		if thresholds[i][1][1]=='total':
 			if clause[0]=='node':
 				neigh_len = len(subset)
 			elif clause[0]=='edge':
 				neigh_len = sum([len(l) for l in subset_target])
 
 		# Available is all neighbors that have a particular label with bound inside [0,1]
@@ -615,19 +710,20 @@
 			elif target in subsets:
 				edges_to_be_added[1].extend(subsets[target])
 			else:
 				edges_to_be_added[1].append(target)
 
 	return (satisfaction, annotations, qualified_nodes, qualified_edges, edges_to_be_added)
 
+
 @numba.njit(cache=True)
 def _is_rule_applicable_edge(interpretations_node, interpretations_edge, neighbors, target_edge, neigh_criteria, thresholds, reverse_graph, ann_fn, ann_fn_label, edges, atom_trace):
 	# Initialize dictionary where keys are strings (x1, x2 etc.) and values are lists of qualified neighbors
 	# Keep track of all the edges that are qualified
-	# If its a node clause update (x1 or x2 etc.) qualified neighbors, if its an edge clause update the qualified neighbors for the source and target (x1, x2)
+	# If it's a node clause update (x1 or x2 etc.) qualified neighbors, if it's an edge clause update the qualified neighbors for the source and target (x1, x2)
 	# First gather all the qualified nodes for each clause
 	subsets = numba.typed.Dict.empty(key_type=numba.types.string, value_type=list_of_nodes)
 	qualified_nodes = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 	qualified_edges = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 	annotations = numba.typed.List.empty_list(numba.typed.List.empty_list(interval.interval_type))
 	edges_to_be_added = (numba.typed.List.empty_list(node_type), numba.typed.List.empty_list(node_type), edges[-1])
 
@@ -662,31 +758,35 @@
 				subset_source = numba.typed.List([target_edge[0]])
 			elif clause[1][0]=='target':
 				subset_source = numba.typed.List([target_edge[1]])
 			else:
 				subset_source = neighbors[target_edge[0]] if clause[1][0] not in subsets else subsets[clause[1][0]]
 				
 			subset_target = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
-			for source in subset_source:
-				subset_target.append(neighbors[source] if clause[1][1] not in subsets else subsets[clause[1][1]])
-
-			# Set targets for possible edges, if target use target node as target
-			if clause[1][1]=='target':
+			if clause[1][1]=='source':
+				# Set targets for possible edges, if source use source node as target
+				for source in subset_source:
+					subset_target.append(numba.typed.List([target_edge[0]]))
+			elif clause[1][1]=='target':
+				# Set targets for possible edges, if target use target node as target
 				for source in subset_source:
 					subset_target.append(numba.typed.List([target_edge[1]]))
+			else:
+				for source in subset_source:
+					subset_target.append(neighbors[source] if clause[1][1] not in subsets else subsets[clause[1][1]])
 
 			qe = get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause[2], clause[3], reverse_graph)
 			subsets[clause[1][0]] = qe[0]
 			subsets[clause[1][1]] = qe[1]
 
 			if atom_trace:
 				qualified_nodes.append(numba.typed.List.empty_list(node_type))
 				qualified_edges.append(numba.typed.List(zip(subsets[clause[1][0]], subsets[clause[1][1]])))
 
-		# Check if clause satisfies threshold
+		# Check if the clause satisfies threshold
 		if thresholds[i][1][1]=='total':
 			if clause[0]=='node':
 				neigh_len = len(subset)
 			elif clause[0]=='edge':
 				neigh_len = sum([len(l) for l in subset_target])
 
 		# Available is all neighbors that have a particular label with bound inside [0,1]
@@ -742,15 +842,14 @@
 				edges_to_be_added[1].extend(subsets[target])
 			else:
 				edges_to_be_added[1].append(target)
 
 	return (satisfaction, annotations, qualified_nodes, qualified_edges, edges_to_be_added)
 
 
-
 @numba.njit(cache=True)
 def get_qualified_components_node_clause(interpretations_node, candidates, l, bnd):
 	# Get all the qualified neighbors for a particular clause
 	qualified_nodes = numba.typed.List.empty_list(node_type)
 	for n in candidates:
 		if is_satisfied_node(interpretations_node, n, (l, bnd)):
 			qualified_nodes.append(n)
@@ -769,15 +868,14 @@
 			if is_satisfied_edge(interpretations_edge, edge, (l, bnd)):
 				qualified_nodes_source.append(source)
 				qualified_nodes_target.append(target)
 
 	return (qualified_nodes_source, qualified_nodes_target)
 	
 
-
 @numba.njit(cache=True)
 def _satisfies_threshold(num_neigh, num_qualified_component, threshold):
 	# Checks if qualified neighbors satisfy threshold. This is for one clause
 	if threshold[1][0]=='number':
 		if threshold[0]=='greater_equal':
 			result = True if num_qualified_component >= threshold[2] else False
 		elif threshold[0]=='greater':
@@ -832,15 +930,14 @@
 						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 						name = facts_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
 					elif mode=='rule':
 						qn, qe, name = rules_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
-			
 
 		# Update complement of predicate (if exists) based on new knowledge of predicate
 		if updated:
 			ip_update_cnt = 0
 			for p1, p2 in ipl:
 				if p1==l:
 					if atom_trace:
@@ -880,14 +977,15 @@
 					change = 1 + ip_update_cnt
 
 		return (updated, change)
 
 	except:
 		return (False, 0)
 
+
 @numba.njit(cache=True)
 def _override_update_node(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, mode):
 	updated = False
 	# This is to prevent a key error in case the label is a specific label
 	try:
 		world = interpretations[comp]
 		l, bnd = na
@@ -989,15 +1087,14 @@
 						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 						name = facts_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
 					elif mode=='rule':
 						qn, qe, name = rules_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
-			
 
 		# Update complement of predicate (if exists) based on new knowledge of predicate
 		if updated:
 			ip_update_cnt = 0
 			for p1, p2 in ipl:
 				if p1==l:
 					if atom_trace:
@@ -1036,14 +1133,15 @@
 				else:
 					change = 1 + ip_update_cnt
 		
 		return (updated, change)
 	except:
 		return (False, 0)
 
+
 @numba.njit(cache=True)
 def _override_update_edge(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, mode):
 	updated = False
 	# This is to prevent a key error in case the label is a specific label
 	try:
 		world = interpretations[comp]
 		l, bnd = na
@@ -1066,15 +1164,14 @@
 						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 						name = facts_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
 					elif mode=='rule':
 						qn, qe, name = rules_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
-			
 
 		# Update complement of predicate (if exists) based on new knowledge of predicate
 		if updated:
 			ip_update_cnt = 0
 			for p1, p2 in ipl:
 				if p1==l:
 					if atom_trace:
@@ -1126,49 +1223,53 @@
 @numba.njit(cache=True)
 def are_satisfied_node(interpretations, comp, nas):
 	result = True
 	for (label, interval) in nas:
 		result = result and is_satisfied_node(interpretations, comp, (label, interval))
 	return result
 
+
 @numba.njit(cache=True)
 def is_satisfied_node(interpretations, comp, na):
 	result = False
 	if (not (na[0] is None or na[1] is None)):
 		# This is to prevent a key error in case the label is a specific label
 		try:
 			world = interpretations[comp]
 			result = world.is_satisfied(na[0], na[1])
 		except:
 			result = False
 	else:
 		result = True
 	return result
 
+
 @numba.njit(cache=True)
 def are_satisfied_edge(interpretations, comp, nas):
 	result = True
 	for (label, interval) in nas:
 		result = result and is_satisfied_edge(interpretations, comp, (label, interval))
 	return result
 
+
 @numba.njit(cache=True)
 def is_satisfied_edge(interpretations, comp, na):
 	result = False
 	if (not (na[0] is None or na[1] is None)):
 		# This is to prevent a key error in case the label is a specific label
 		try:
 			world = interpretations[comp]
 			result = world.is_satisfied(na[0], na[1])
 		except:
 			result = False
 	else:
 		result = True
 	return result
 
+
 @numba.njit(cache=True)
 def influence(rule, annotations, weights):
 	func_name = rule.get_annotation_function()
 	if func_name=='':
 		return interval.closed(rule.get_bnd().lower, rule.get_bnd().upper)
 	elif func_name=='average':
 		return ann_fn.average(annotations, weights)
@@ -1253,14 +1354,15 @@
 
 @numba.njit(cache=True)
 def _add_node(node, neighbors, nodes, interpretations_node):
 	nodes.append(node)
 	neighbors[node] = numba.typed.List.empty_list(node_type)
 	interpretations_node[node] = world.World(numba.typed.List.empty_list(label.label_type))
 
+
 @numba.njit(cache=True)
 def _add_edge(source, target, neighbors, nodes, edges, l, interpretations_node, interpretations_edge):
 	# If not a node, add to list of nodes and initialize neighbors
 	if source not in nodes:
 		_add_node(source, neighbors, nodes, interpretations_node)
 
 	if target not in nodes:
@@ -1281,15 +1383,14 @@
 			interpretations_edge[edge] = world.World(numba.typed.List.empty_list(label.label_type))
 	else:
 		if l not in interpretations_edge[edge].world and l.value!='':
 			new_edge = True
 			interpretations_edge[edge].world[l] = interval.closed(0,1)
 
 	return (edge, new_edge)
-		
 
 
 @numba.njit(cache=True)
 def _add_edges(sources, targets, neighbors, nodes, edges, l, interpretations_node, interpretations_edge):
 	changes = 0
 	edges_added = numba.typed.List.empty_list(edge_type)
 	for source in sources:
```

### Comparing `pyreason-1.4.2/pyreason/scripts/interval/interval.py` & `pyreason-1.5.0/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 from numba.extending import models, register_model
 from numba.extending import make_attribute_wrapper
 from numba.extending import overload_method
 from numba.extending import lower_builtin
 from numba.core import cgutils
 from numba.extending import unbox, NativeValue, box
 
+
 # WARNING: problem with constructing inside jit function (not needed for now)
 # Create new numba type
 class RuleType(types.Type):
     def __init__(self):
         super(RuleType, self).__init__(name='Rule')
 
+
 rule_type = RuleType()
 
 
 # Type ann_fnerence
 @typeof_impl.register(Rule)
 def typeof_rule(val, c):
     return rule_type
 
 
 # Construct object from Numba functions (Doesn't work. We don't need this currently)
 @type_callable(Rule)
 def type_rule(context):
-    def typer(name, target, tc, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges):
-        if isinstance(name, types.UnicodeType) and isinstance(target, label.LabelType) and isinstance(tc, (types.NoneType, types.ListType)) and isinstance(delta, types.Integer) and isinstance(neigh_criteria, (types.NoneType, types.ListType)) and isinstance(bnd, interval.IntervalType) and isinstance(thresholds, types.ListType) and isinstance(ann_fn, types.UnicodeType) and isinstance(ann_label, label.LabelType) and isinstance(weights, types.Array) and isinstance(edges, types.Tuple):
+    def typer(name, target, tc, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule):
+        if isinstance(name, types.UnicodeType) and isinstance(target, label.LabelType) and isinstance(tc, (types.NoneType, types.ListType)) and isinstance(delta, types.Integer) and isinstance(neigh_criteria, (types.NoneType, types.ListType)) and isinstance(bnd, interval.IntervalType) and isinstance(thresholds, types.ListType) and isinstance(ann_fn, types.UnicodeType) and isinstance(ann_label, label.LabelType) and isinstance(weights, types.Array) and isinstance(edges, types.Tuple) and isinstance(immediate_rule, types.Boolean):
             return rule_type
     return typer
 
 
 # Define native representation: datamodel
 @register_model(RuleType)
 class RuleModel(models.StructModel):
@@ -47,15 +49,16 @@
             ('delta', types.int8),
             ('neigh_criteria', types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type)))),
             ('bnd', interval.interval_type),
             ('thresholds', types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64)))),
             ('ann_fn', types.string),
             ('ann_label', label.label_type),
             ('weights', types.float64[::1]),
-            ('edges', types.Tuple((types.string, types.string, label.label_type)))
+            ('edges', types.Tuple((types.string, types.string, label.label_type))),
+            ('immediate_rule', types.boolean)
             ]
         models.StructModel.__init__(self, dmm, fe_type, members)
 
 
 # Expose datamodel attributes
 make_attribute_wrapper(RuleType, 'name', 'name')
 make_attribute_wrapper(RuleType, 'target', 'target')
@@ -64,104 +67,124 @@
 make_attribute_wrapper(RuleType, 'neigh_criteria', 'neigh_criteria')
 make_attribute_wrapper(RuleType, 'bnd', 'bnd')
 make_attribute_wrapper(RuleType, 'thresholds', 'thresholds')
 make_attribute_wrapper(RuleType, 'ann_fn', 'ann_fn')
 make_attribute_wrapper(RuleType, 'ann_label', 'ann_label')
 make_attribute_wrapper(RuleType, 'weights', 'weights')
 make_attribute_wrapper(RuleType, 'edges', 'edges')
+make_attribute_wrapper(RuleType, 'immediate_rule', 'immediate_rule')
+
 
 # Implement constructor
-@lower_builtin(Rule, types.string, label.label_type, types.ListType(types.Tuple((label.label_type, interval.interval_type))), types.int8, types.ListType(types.Tuple((types.string, label.label_type, interval.interval_type))), interval.interval_type, types.ListType(types.ListType(types.Tuple((types.string, types.string, types.float64)))), types.string, label.label_type, types.float64[::1], types.Tuple((types.string, types.string, label.label_type)))
+@lower_builtin(Rule, types.string, label.label_type, types.ListType(types.Tuple((label.label_type, interval.interval_type))), types.int8, types.ListType(types.Tuple((types.string, label.label_type, interval.interval_type))), interval.interval_type, types.ListType(types.ListType(types.Tuple((types.string, types.string, types.float64)))), types.string, label.label_type, types.float64[::1], types.Tuple((types.string, types.string, label.label_type)), types.boolean)
 def impl_rule(context, builder, sig, args):
     typ = sig.return_type
-    name, target, target_criteria, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges = args
+    name, target, target_criteria, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule = args
     context.nrt.incref(builder, types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type))), neigh_criteria)
     context.nrt.incref(builder, types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), thresholds)
     rule = cgutils.create_struct_proxy(typ)(context, builder)
     rule.name = name
     rule.target = target
     rule.target_criteria = target_criteria
     rule.delta = delta
     rule.neigh_criteria = neigh_criteria
     rule.bnd = bnd
     rule.thresholds = thresholds
     rule.ann_fn = ann_fn
     rule.ann_label = ann_label
     rule.weights = weights
     rule.edges = edges
+    rule.immediate_rule = immediate_rule
     return rule._getvalue()
 
+
 # Expose properties
 @overload_method(RuleType, "get_name")
 def get_name(rule):
     def getter(rule):
         return rule.name
     return getter
 
+
 @overload_method(RuleType, "get_target")
 def get_target(rule):
     def getter(rule):
         return rule.target
     return getter
 
+
 @overload_method(RuleType, "get_target_criteria")
 def get_target_criteria(rule):
     def getter(rule):
         return rule.target_criteria
     return getter
 
+
 @overload_method(RuleType, "get_delta")
 def get_delta(rule):
     def getter(rule):
         return rule.delta
     return getter
 
+
 @overload_method(RuleType, "get_neigh_criteria")
 def get_neigh_criteria(rule):
     def getter(rule):
         return rule.neigh_criteria
     return getter
 
+
 @overload_method(RuleType, "get_bnd")
 def get_bnd(rule):
     def impl(rule):
         return rule.bnd
     return impl
 
+
 @overload_method(RuleType, "get_thresholds")
 def get_thresholds(rule):
     def impl(rule):
         return rule.thresholds
     return impl
 
+
 @overload_method(RuleType, "get_annotation_function")
 def get_annotation_function(rule):
     def impl(rule):
         return rule.ann_fn
     return impl
 
+
 @overload_method(RuleType, "get_annotation_label")
 def get_label(rule):
     def impl(rule):
         return rule.ann_label
     return impl
 
+
 @overload_method(RuleType, "get_weights")
 def get_weights(rule):
     def impl(rule):
         return rule.weights
     return impl
 
+
 @overload_method(RuleType, "get_edges")
 def get_edges(rule):
     def impl(rule):
         return rule.edges
     return impl
 
 
+@overload_method(RuleType, "is_immediate_rule")
+def is_immediate_rule(rule):
+    def impl(rule):
+        return rule.immediate_rule
+    return impl
+
 
 # Tell numba how to make native
 @unbox(RuleType)
 def unbox_rule(typ, obj, c):
     name_obj = c.pyapi.object_getattr_string(obj, "_name")
     target_obj = c.pyapi.object_getattr_string(obj, "_target")
     tc_obj = c.pyapi.object_getattr_string(obj, "_target_criteria")
@@ -169,64 +192,68 @@
     neigh_criteria_obj = c.pyapi.object_getattr_string(obj, "_neigh_criteria")
     bnd_obj = c.pyapi.object_getattr_string(obj, "_bnd")
     thresholds_obj = c.pyapi.object_getattr_string(obj, "_thresholds")
     ann_fn_obj = c.pyapi.object_getattr_string(obj, "_ann_fn")
     ann_label_obj = c.pyapi.object_getattr_string(obj, "_ann_label")
     weights_obj = c.pyapi.object_getattr_string(obj, "_weights")
     edges_obj = c.pyapi.object_getattr_string(obj, "_edges")
+    immediate_rule_obj = c.pyapi.object_getattr_string(obj, "_immediate_rule")
     rule = cgutils.create_struct_proxy(typ)(c.context, c.builder)
     rule.name = c.unbox(types.string, name_obj).value
     rule.target = c.unbox(label.label_type, target_obj).value
     rule.target_criteria = c.unbox(types.ListType(types.Tuple((label.label_type, interval.interval_type))), tc_obj).value
     rule.delta = c.unbox(types.int8, delta_obj).value
     rule.neigh_criteria = c.unbox(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type))), neigh_criteria_obj).value
     rule.bnd = c.unbox(interval.interval_type, bnd_obj).value
     rule.thresholds = c.unbox(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), thresholds_obj).value
     rule.ann_fn = c.unbox(types.string, ann_fn_obj).value
     rule.ann_label = c.unbox(label.label_type, ann_label_obj).value
     rule.weights = c.unbox(types.float64[::1], weights_obj).value
     rule.edges = c.unbox(types.Tuple((types.string, types.string, label.label_type)), edges_obj).value
+    rule.immediate_rule = c.unbox(types.boolean, immediate_rule_obj).value
     c.pyapi.decref(name_obj)
     c.pyapi.decref(target_obj)
     c.pyapi.decref(tc_obj)
     c.pyapi.decref(delta_obj)
     c.pyapi.decref(neigh_criteria_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(thresholds_obj)
     c.pyapi.decref(ann_fn_obj)
     c.pyapi.decref(ann_label_obj)
     c.pyapi.decref(weights_obj)
     c.pyapi.decref(edges_obj)
+    c.pyapi.decref(immediate_rule_obj)
     is_error = cgutils.is_not_null(c.builder, c.pyapi.err_occurred())
     return NativeValue(rule._getvalue(), is_error=is_error)
 
 
-
 @box(RuleType)
 def box_rule(typ, val, c):
     rule = cgutils.create_struct_proxy(typ)(c.context, c.builder, value=val)
     class_obj = c.pyapi.unserialize(c.pyapi.serialize_object(Rule))
     name_obj = c.box(types.string, rule.name)
     target_obj = c.box(label.label_type, rule.target)
-    tc_obj = c.box(types.ListType(types.Tuple((label.label_type, interval.interval_type))), rule.tc_node)
+    tc_obj = c.box(types.ListType(types.Tuple((label.label_type, interval.interval_type))), rule.target_criteria)
     delta_obj = c.box(types.int8, rule.delta)
     neigh_criteria_obj = c.box(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type))), rule.neigh_criteria)
     bnd_obj = c.box(interval.interval_type, rule.bnd)
     thresholds_obj = c.box(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), rule.thresholds)
     ann_fn_obj = c.box(types.string, rule.ann_fn)
     ann_label_obj = c.box(label.label_type, rule.ann_label)
     weights_obj = c.box(types.float64[::1], rule.weights)
     edges_obj = c.box(types.Tuple((types.string, types.string, label.label_type)), rule.edges)
-    res = c.pyapi.call_function_objargs(class_obj, (name_obj, target_obj, tc_obj, delta_obj, neigh_criteria_obj, bnd_obj, thresholds_obj, ann_fn_obj, ann_label_obj, weights_obj, edges_obj))
+    immediate_rule_obj = c.box(types.boolean, rule.immediate_rule)
+    res = c.pyapi.call_function_objargs(class_obj, (name_obj, target_obj, tc_obj, delta_obj, neigh_criteria_obj, bnd_obj, thresholds_obj, ann_fn_obj, ann_label_obj, weights_obj, edges_obj, immediate_rule_obj))
     c.pyapi.decref(name_obj)
     c.pyapi.decref(target_obj)
     c.pyapi.decref(tc_obj)
     c.pyapi.decref(delta_obj)
     c.pyapi.decref(neigh_criteria_obj)
     c.pyapi.decref(ann_fn_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(thresholds_obj)
     c.pyapi.decref(ann_label_obj)
     c.pyapi.decref(weights_obj)
     c.pyapi.decref(edges_obj)
+    c.pyapi.decref(immediate_rule_obj)
     c.pyapi.decref(class_obj)
     return res
```

### Comparing `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.5.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/program/program.py` & `pyreason-1.5.0/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/rules/rule.py` & `pyreason-1.5.0/pyreason/scripts/rules/rule.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 class Rule:
 
-    def __init__(self, name, target, target_criteria, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges):
+    def __init__(self, name, target, target_criteria, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule):
         self._name = name
         self._target = target
         self._target_criteria = target_criteria
         self._delta = delta
         self._neigh_criteria = neigh_criteria
         self._bnd = bnd
         self._thresholds = thresholds
         self._ann_fn = ann_fn
         self._ann_label = ann_label
         self._weights = weights
         self._edges = edges
+        self._immediate_rule = immediate_rule
 
     def get_name(self):
         return self._name
     
     def get_target(self):
         return self._target
 
@@ -38,7 +39,10 @@
         return self._ann_fn
 
     def get_ann_label(self):
         return self._ann_label
     
     def get_edges(self):
         return self._edges
+
+    def is_immediate_rule(self):
+        return self._immediate_rule
```

### Comparing `pyreason-1.4.2/pyreason/scripts/utils/filter.py` & `pyreason-1.5.0/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.5.0/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/utils/output.py` & `pyreason-1.5.0/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/utils/plotter.py` & `pyreason-1.5.0/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/utils/visuals.py` & `pyreason-1.5.0/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.5.0/pyreason/scripts/utils/yaml_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.rule_type as rule
 import pyreason.scripts.numba_wrapper.numba_types.fact_node_type as fact_node
 import pyreason.scripts.numba_wrapper.numba_types.fact_edge_type as fact_edge
 
 
-
 def parse_rules(path):
     with open(path, 'r') as file:
         rules_yaml = yaml.safe_load(file)
 
     rules = numba.typed.List.empty_list(rule.rule_type)
+    immediate_rules = numba.typed.List.empty_list(rule.rule_type)
     for rule_name, values in rules_yaml.items():
         # Set rule target
         target = label.Label('')
         if values['target'] is not None:
             target = label.Label(values['target'])
-        
+
         # Set rule target criteria
         target_criteria = numba.typed.List.empty_list(numba.types.Tuple((label.label_type, interval.interval_type)))
         if values['target_criteria'] is not None:
             for tc in values['target_criteria']:
                 target_criteria.append((label.Label(tc[0]), interval.closed(tc[1], tc[2])))
 
         # Set delta t
         delta_t = numba.types.int8(values['delta_t'])
 
         # neigh_criteria = [c1, c2, c3, c4]
         # thresholds = [t1, t2, t3, t4]
-        
+
         # Array of thresholds to keep track of for each neighbor criterion. Form [(comparison, (number/percent, total/available), thresh)]
         thresholds = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), numba.types.float64)))
 
         # Array to store clauses for nodes: node/edge, [subset]/[subset1, subset2], label, interval
         neigh_criteria = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), label.label_type, interval.interval_type)))
         if values['neigh_criteria'] is not None:
             # Loop through clauses
@@ -72,15 +72,14 @@
             elif len(values['edges'])==3:
                 values['edges'][2] = label.Label(values['edges'][2])
                 edges = tuple(values['edges'])
 
         # Both target and edge label (if edges are being added) cannot be '' at the same time. One has to have a value
         assert edges[2].get_value()!='' or target.get_value()!='', 'Both target and edge label cannot empty at the same time, one has to take a value. Modify the rules YAML file'
 
-        
         # If annotation function is a string, it is the name of the function. If it is a bound then set it to an empty string
         ann_fn, ann_label = values['ann_fn']
         if isinstance(ann_fn, str):
             bnd = interval.closed(0, 1)
             ann_label = label.Label(ann_label)
         elif isinstance(ann_fn, (float, int)):
             bnd = interval.closed(values['ann_fn'][0], values['ann_fn'][1])
@@ -88,19 +87,33 @@
             ann_label = label.Label('')
 
         # If there are weights provided, store them. Default is [1,1,1...1,0]
         num_clauses = 0 if values['neigh_criteria'] is None else len(values['neigh_criteria'])
         weights = np.ones(num_clauses, dtype=np.float64)
         weights = np.append(weights, 0)
         if 'weights' in values and values['weights']:
-            weights = np.array(values['weights'], dtype=np.float64)   
-        r = rule.Rule(rule_name, target, target_criteria, delta_t, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges)
-        rules.append(r)
+            weights = np.array(values['weights'], dtype=np.float64)
 
-    return rules
+        # Immediate rule flag -- whether to be applied before all other rules
+        immediate_rule = False
+        if 'immediate' in values and values['immediate'] is not None:
+            immediate_rule = True
+
+        r = rule.Rule(rule_name, target, target_criteria, delta_t, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule)
+
+        # Insert to beginning of list if flag for immediate rule is true
+        if immediate_rule:
+            immediate_rules.append(r)
+        else:
+            rules.append(r)
+
+    all_rules = numba.typed.List.empty_list(rule.rule_type)
+    all_rules.extend(immediate_rules)
+    all_rules.extend(rules)
+    return all_rules
 
 
 def parse_facts(path, reverse):
     with open(path, 'r') as file:
         facts_yaml = yaml.safe_load(file)
 
     facts_node = numba.typed.List.empty_list(fact_node.fact_type)
@@ -171,14 +184,15 @@
         for entry in labels_yaml['edge_specific_labels']:
             for label_name, edges in entry.items():
                 l = label.Label(str(label_name))
                 specific_edge_labels[l] = numba.typed.List([(str(e[0]), str(e[1])) for e in edges])
 
     return node_labels, edge_labels, specific_node_labels, specific_edge_labels
 
+
 def parse_ipl(path):
     with open(path, 'r') as file:
         ipl_yaml = yaml.safe_load(file)
 
     ipl = numba.typed.List.empty_list(numba.types.Tuple((label.label_type, label.label_type)))
     if ipl_yaml['ipl'] is not None:
         for labels in ipl_yaml['ipl']:
```

### Comparing `pyreason-1.4.2/pyreason.egg-info/PKG-INFO` & `pyreason-1.5.0/pyreason.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.4.2
+Version: 1.5.0
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.4.2/pyreason.egg-info/SOURCES.txt` & `pyreason-1.5.0/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.2/setup.py` & `pyreason-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name = 'pyreason',
-    version = '1.4.2',
+    version = '1.5.0',
     author = 'Dyuman Aditya',
     author_email = 'dyuman.aditya@gmail.com',
     description = 'An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/lab-v2/pyreason',
     license = 'BSD 3-clause',
```

