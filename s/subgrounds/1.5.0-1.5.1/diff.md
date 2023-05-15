# Comparing `tmp/subgrounds-1.5.0.tar.gz` & `tmp/subgrounds-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subgrounds-1.5.0.tar", max compression
+gzip compressed data, was "subgrounds-1.5.1.tar", max compression
```

## Comparing `subgrounds-1.5.0.tar` & `subgrounds-1.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11347 2023-04-25 07:05:05.071162 subgrounds-1.5.0/LICENSE
--rw-r--r--   0        0        0     8943 2023-04-25 07:05:05.071162 subgrounds-1.5.0/README.md
--rw-r--r--   0        0        0     1929 2023-04-25 07:06:45.810722 subgrounds-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      317 2023-04-25 07:06:45.786722 subgrounds-1.5.0/subgrounds/__init__.py
--rw-r--r--   0        0        0     4521 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/client.py
--rw-r--r--   0        0        0     1895 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/contrib/README.md
--rw-r--r--   0        0        0      349 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/contrib/dash/__init__.py
--rw-r--r--   0        0        0      399 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/contrib/dash/abcs.py
--rw-r--r--   0        0        0     3893 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/contrib/dash/components.py
--rw-r--r--   0        0        0     1285 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/contrib/plotly/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/contrib/plotly/figure.py
--rw-r--r--   0        0        0     5866 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/contrib/plotly/traces.py
--rw-r--r--   0        0        0      934 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/contrib/pyodide.py
--rw-r--r--   0        0        0      438 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/dash_wrappers.py
--rw-r--r--   0        0        0    10062 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/dataframe_utils.py
--rw-r--r--   0        0        0      395 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/errors.py
--rw-r--r--   0        0        0     1027 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/pagination/__init__.py
--rw-r--r--   0        0        0     4761 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/pagination/pagination.py
--rw-r--r--   0        0        0    10550 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/pagination/preprocess.py
--rw-r--r--   0        0        0    17076 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/pagination/strategies.py
--rw-r--r--   0        0        0     1530 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/pagination/utils.py
--rw-r--r--   0        0        0     1460 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/plotly_wrappers.py
--rw-r--r--   0        0        0    62357 2023-04-25 07:05:05.071162 subgrounds-1.5.0/subgrounds/query.py
--rw-r--r--   0        0        0    12755 2023-04-25 07:05:05.075162 subgrounds-1.5.0/subgrounds/schema.py
--rw-r--r--   0        0        0      308 2023-04-25 07:05:05.075162 subgrounds-1.5.0/subgrounds/subgraph/__init__.py
--rw-r--r--   0        0        0    38895 2023-04-25 07:05:05.075162 subgrounds-1.5.0/subgrounds/subgraph/fieldpath.py
--rw-r--r--   0        0        0     1669 2023-04-25 07:05:05.075162 subgrounds-1.5.0/subgrounds/subgraph/filter.py
--rw-r--r--   0        0        0     4754 2023-04-25 07:05:05.075162 subgrounds-1.5.0/subgrounds/subgraph/object.py
--rw-r--r--   0        0        0     2552 2023-04-25 07:05:05.075162 subgrounds-1.5.0/subgrounds/subgraph/subgraph.py
--rw-r--r--   0        0        0    21574 2023-04-25 07:05:05.075162 subgrounds-1.5.0/subgrounds/subgrounds.py
--rw-r--r--   0        0        0    20072 2023-04-25 07:05:05.075162 subgrounds-1.5.0/subgrounds/transform.py
--rw-r--r--   0        0        0     6901 2023-04-25 07:05:05.075162 subgrounds-1.5.0/subgrounds/utils.py
--rw-r--r--   0        0        0    10369 1970-01-01 00:00:00.000000 subgrounds-1.5.0/setup.py
--rw-r--r--   0        0        0    10020 1970-01-01 00:00:00.000000 subgrounds-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 17:03:03.320694 subgrounds-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3855 2023-05-15 17:03:03.320694 subgrounds-1.5.1/README.md
+-rw-r--r--   0        0        0     1929 2023-05-15 17:05:01.117202 subgrounds-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      317 2023-05-15 17:05:01.089202 subgrounds-1.5.1/subgrounds/__init__.py
+-rw-r--r--   0        0        0     4521 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/client.py
+-rw-r--r--   0        0        0     1895 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/README.md
+-rw-r--r--   0        0        0      349 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/dash/__init__.py
+-rw-r--r--   0        0        0      399 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/dash/abcs.py
+-rw-r--r--   0        0        0     3893 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/dash/components.py
+-rw-r--r--   0        0        0     1285 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/plotly/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/plotly/figure.py
+-rw-r--r--   0        0        0     5866 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/plotly/traces.py
+-rw-r--r--   0        0        0      873 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/pyodide.py
+-rw-r--r--   0        0        0      438 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/dash_wrappers.py
+-rw-r--r--   0        0        0    10062 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/dataframe_utils.py
+-rw-r--r--   0        0        0      395 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/errors.py
+-rw-r--r--   0        0        0     1027 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/__init__.py
+-rw-r--r--   0        0        0     4761 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/pagination.py
+-rw-r--r--   0        0        0    12577 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/preprocess.py
+-rw-r--r--   0        0        0    17155 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/strategies.py
+-rw-r--r--   0        0        0     2901 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/utils.py
+-rw-r--r--   0        0        0     1460 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/plotly_wrappers.py
+-rw-r--r--   0        0        0    62357 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/query.py
+-rw-r--r--   0        0        0    13291 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/schema.py
+-rw-r--r--   0        0        0      308 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/__init__.py
+-rw-r--r--   0        0        0    38891 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/fieldpath.py
+-rw-r--r--   0        0        0     1669 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/filter.py
+-rw-r--r--   0        0        0     4754 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/object.py
+-rw-r--r--   0        0        0     2550 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/subgraph.py
+-rw-r--r--   0        0        0    21574 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgrounds.py
+-rw-r--r--   0        0        0    20072 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/transform.py
+-rw-r--r--   0        0        0     6981 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/utils.py
+-rw-r--r--   0        0        0     5138 1970-01-01 00:00:00.000000 subgrounds-1.5.1/setup.py
+-rw-r--r--   0        0        0     4932 1970-01-01 00:00:00.000000 subgrounds-1.5.1/PKG-INFO
```

### Comparing `subgrounds-1.5.0/LICENSE` & `subgrounds-1.5.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022 Protean Labs Inc.
+   Copyright 2023 Playgrounds Analytics, Inc.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `subgrounds-1.5.0/pyproject.toml` & `subgrounds-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subgrounds"
-version = "1.5.0"
+version = "1.5.1"
 description = "A Pythonic data access layer for applications querying data from The Graph Network."
 authors = [
     "cvauclair <cvauclair@playgrounds.network>",
     "0xMochan <mochan@playgrounds.network>",
 ]
 repository = "https://github.com/0xPlaygrounds/subgrounds"
```

### Comparing `subgrounds-1.5.0/subgrounds/client.py` & `subgrounds-1.5.1/subgrounds/client.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/contrib/README.md` & `subgrounds-1.5.1/subgrounds/contrib/README.md`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/contrib/dash/components.py` & `subgrounds-1.5.1/subgrounds/contrib/dash/components.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/contrib/plotly/__init__.py` & `subgrounds-1.5.1/subgrounds/contrib/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/contrib/plotly/figure.py` & `subgrounds-1.5.1/subgrounds/contrib/plotly/figure.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/contrib/plotly/traces.py` & `subgrounds-1.5.1/subgrounds/contrib/plotly/traces.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/contrib/pyodide.py` & `subgrounds-1.5.1/subgrounds/contrib/pyodide.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 """
 
 import sys
 import warnings
 
 __all__ = ["patch"]
 
+
 def patch():
     """Attempts to patch `requests` to allow `subgrounds` to work in `pyodide`
-    
+
     Outputs warnings instead of exceptions when things go wrong
     """
-    
+
     if "pyodide" in sys.modules:
         try:
             import pyodide_http
         except ImportError:
             warnings.warn(
                 "`pyodide-http` failed to import in the auto-detected `pyodide`"
                 " environment. Did you install `subgrounds` with `pyodide` support?\n\n"
                 "    `pip install subgrounds[pyodide]`"
             )
             return
-        
+
         try:
             pyodide_http.patch_all()
         except Exception as e:
-            warnings.warn(
-                "Failed to patch with `pyodide-http`:\n"
-                + str(e)
-            )
+            warnings.warn("Failed to patch with `pyodide-http`:\n" + str(e))
```

### Comparing `subgrounds-1.5.0/subgrounds/dataframe_utils.py` & `subgrounds-1.5.1/subgrounds/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/pagination/__init__.py` & `subgrounds-1.5.1/subgrounds/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/pagination/pagination.py` & `subgrounds-1.5.1/subgrounds/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/pagination/preprocess.py` & `subgrounds-1.5.1/subgrounds/pagination/preprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """ Helper functions and classes used by Subgrounds' own pagination strategies.
 """
 
 from __future__ import annotations
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, replace
+from functools import reduce
 from itertools import count
-from typing import Any
+from typing import Any, cast
 
-from pipe import map, traverse
+from pipe import map, reverse, skip, traverse
 
-from subgrounds.pagination.utils import DEFAULT_NUM_ENTITIES
 from subgrounds.query import (
     Argument,
     Document,
     InputValue,
     Selection,
     VariableDefinition,
 )
 from subgrounds.schema import SchemaMeta, TypeMeta, TypeRef
+from subgrounds.utils import accumulate
+
+from .utils import DEFAULT_NUM_ENTITIES, merge_input_value_object_metas
 
 
 @dataclass(frozen=True)
 class PaginationNode:
     """Class representing the pagination config for a single GraphQL list field.
 
     Attributes:
@@ -89,205 +92,248 @@
     )
 
 
 def get_orderBy_value(selection: Selection) -> str:
     order_by_val = selection.find_args(lambda arg: arg.name == "orderBy", recurse=False)
     if order_by_val is None:
         return "id"
-    else:
-        return order_by_val.value.value
+
+    return order_by_val.value.value
 
 
 def get_orderDirection_value(selection: Selection) -> str:
     order_direction_arg = selection.find_args(
         lambda arg: arg.name == "orderDirection", recurse=False
     )
-
     if order_direction_arg is None:
         return "asc"
-    else:
-        return order_direction_arg.value.value
+
+    return order_direction_arg.value.value
 
 
-def get_filtering_arg(selection: Selection) -> str:
+def get_filtering_args(selection: Selection) -> list[str]:
     orderBy_val = get_orderBy_value(selection)
     orderDirection_val = get_orderDirection_value(selection)
 
-    return "{}_{}".format(orderBy_val, "gt" if orderDirection_val == "asc" else "lt")
+    *names, last = orderBy_val.split("__")
 
+    return [*names, "{}_{}".format(last, "gt" if orderDirection_val == "asc" else "lt")]
 
-def get_filtering_value(selection: Selection) -> Any:
-    where_arg = selection.find_args(lambda arg: arg.name == "where", recurse=False)
-    if where_arg is None:
-        return None
-    else:
-        filtering_arg = get_filtering_arg(selection)
-        if filtering_arg in where_arg.value.value:
-            return where_arg.value.value[filtering_arg].value
-        else:
+
+def get_filtering_value(selection: Selection) -> Any | None:
+    def recurse_filtering_values(
+        filtering_args: list[str],
+        obj: InputValue.Object,
+    ) -> Any | None:
+        if not filtering_args:
             return None
 
+        if (filtering_arg := filtering_args.pop(0)) not in obj.value:
+            return None
 
-""" normalize:
+        match obj.value[filtering_arg]:
+            case InputValue.Object() as obj:
+                return recurse_filtering_values(filtering_args, obj)
+            case value:
+                return value.value
 
-For each selection:
-1. If `id` not selected, add `id` to selection
-2. Replace `first` argument value by `$firstX`
-3. Replace `skip` argument value by `$skipX`
-4. If `orderBy` argument is not defined, add argument with value `asc`
-5. If `where` argument specified 
-"""
+    where_arg = selection.find_args(lambda arg: arg.name == "where", recurse=False)
+    if where_arg is None:
+        return None
+
+    return recurse_filtering_values(
+        get_filtering_args(selection), cast(InputValue.Object, where_arg.value)
+    )
 
 
 def generate_pagination_nodes(
     schema: SchemaMeta, document: Document
 ) -> list[PaginationNode]:
     counter = count()
 
     def fold_f(
         current: Selection, parents: list[Selection], children: list[PaginationNode]
-    ) -> list[PaginationNode]:
-        if is_pagination_node(schema, current):
-            idx = next(counter)
-
-            orderBy_val = get_orderBy_value(current)
-            filtering_arg = get_filtering_arg(current)
-
-            t: TypeRef.T = current.fmeta.type_of_arg("where")
-            where_arg_type: TypeMeta.InputObjectMeta = schema.type_of_typeref(t)
-            filtering_arg_type: TypeRef.T = where_arg_type.type_of_input_field(
-                filtering_arg
-            )
-
-            return PaginationNode(
-                node_idx=idx,
-                filter_field=orderBy_val,
-                first_value=(
-                    current.find_args(
-                        lambda arg: arg.name == "first", recurse=False
-                    ).value.value
-                    if current.exists_args(
-                        lambda arg: arg.name == "first", recurse=False
-                    )
-                    else DEFAULT_NUM_ENTITIES
-                ),
-                skip_value=(
-                    current.find_args(
-                        lambda arg: arg.name == "skip", recurse=False
-                    ).value.value
-                    if current.exists_args(
-                        lambda arg: arg.name == "skip", recurse=False
-                    )
-                    else 0
-                ),
-                filter_value=get_filtering_value(current),
-                filter_value_type=filtering_arg_type,
-                key_path=[select.key for select in [*parents, current]],
-                inner=children,
-            )
-        else:
+    ) -> PaginationNode | list[PaginationNode]:
+        if not is_pagination_node(schema, current):
             return children
+        idx = next(counter)
+
+        orderBy_val = get_orderBy_value(current)
+        filtering_args = get_filtering_args(current)
+
+        t: TypeRef.T = current.fmeta.type_of_arg("where")
+        where_arg_type: TypeMeta.InputObjectMeta = schema.type_of_typeref(t)
+        filtering_arg_type: TypeRef.T = schema.type_of_input_object_meta(
+            where_arg_type, filtering_args
+        )
+
+        return PaginationNode(
+            node_idx=idx,
+            filter_field=orderBy_val,
+            first_value=(
+                current.find_args(
+                    lambda arg: arg.name == "first", recurse=False
+                ).value.value
+                if current.exists_args(lambda arg: arg.name == "first", recurse=False)
+                else DEFAULT_NUM_ENTITIES
+            ),
+            skip_value=(
+                current.find_args(
+                    lambda arg: arg.name == "skip", recurse=False
+                ).value.value
+                if current.exists_args(lambda arg: arg.name == "skip", recurse=False)
+                else 0
+            ),
+            filter_value=get_filtering_value(current),
+            filter_value_type=filtering_arg_type,
+            key_path=[select.key for select in [*parents, current]],
+            inner=children,
+        )
 
     return list(document.query.fold(fold_f) | traverse)
 
 
 def normalize(
-    schema: SchemaMeta, document: Document, pagination_nodes: list[PaginationNode]
+    schema: SchemaMeta,
+    document: Document,
+    pagination_nodes: list[PaginationNode],
 ):
+    """Inject various graphql components to "normalize" the query for pagination.
+
+    When we paginate a query, we inject custom filtering based on the order by values.
+    We also add GraphQL variables so that `PaginationStrategy` only need to change those
+     to perform pagination.
+
+    The main process for normalization begins by recursively adjusting `Selection` nodes
+     within the Query tree. We only apply the following steps if the node needs to be
+     paginated.
+
+    > Note, these steps always check the current selection and will merge new values
+     and selections onto whats currently there.
+
+    1. Ensure `id` is on the `Selection`
+    2. Replace `first` argument value by `$firstX`
+    3. Replace `skip` argument value by `$skipX`
+    4. With the `orderBy` (default being `id`), generate where filtering arguments
+      a) These are used to filter out values when paginating
+    5. Set `where` filtering values (deep union / merge)
+    """
+
     counter = count()
 
-    def map_f(
-        current: Selection,
-    ) -> Selection:
-        if is_pagination_node(schema, current):
-            idx = next(counter)
+    def map_f(current: Selection) -> Selection:
+        if not is_pagination_node(schema, current):
+            return current
 
-            where_value: dict[str, Any] = (
-                current.find_args(
-                    lambda arg: arg.name == "where", recurse=False
-                ).value.value
-                if current.exists_args(lambda arg: arg.name == "where", recurse=False)
-                else {}
-            )
+        idx = next(counter)
 
-            orderBy_value = get_orderBy_value(current)
+        where_value: dict[str, Any] = cast(
+            dict,
+            current.find_args(
+                lambda arg: arg.name == "where", recurse=False
+            ).value.value  # type: ignore
+            if current.exists_args(lambda arg: arg.name == "where", recurse=False)
+            else {},
+        )
+
+        orderBy_value = get_orderBy_value(current)
+
+        # Build out a nested dictionary of `InputValue.Object` containing the
+        #  `lastOrderingValue{idx}` used for pagination. We do this by iterating through
+        #  the args backwards starting from the innermost and nesting them in dicts.
+        # We need to add a trailing `_` to outer arguments for `InputValue.Object` for
+        #  where clauses to work properly.
+        *args, innermost_arg = get_filtering_args(current)
+        where_filtering_args: InputValue.Object = reduce(
+            lambda inner, outer_arg: InputValue.Object({f"{outer_arg}_": inner}),
+            args | reverse,
+            InputValue.Object(
+                {innermost_arg: InputValue.Variable(f"lastOrderingValue{idx}")}
+            ),
+        )
 
-            pagination_args = [
-                Argument(name="first", value=InputValue.Variable(f"first{idx}")),
-                Argument(name="skip", value=InputValue.Variable(f"skip{idx}")),
-                Argument(name="orderBy", value=InputValue.Enum(orderBy_value)),
-                Argument(
-                    name="orderDirection",
-                    value=InputValue.Enum(get_orderDirection_value(current)),
-                ),
-                Argument(
-                    name="where",
-                    value=InputValue.Object(
-                        where_value
-                        | {
-                            get_filtering_arg(current): InputValue.Variable(
-                                f"lastOrderingValue{idx}"
-                            )
-                        }
-                    ),
+        pagination_args = [
+            Argument(name="first", value=InputValue.Variable(f"first{idx}")),
+            Argument(name="skip", value=InputValue.Variable(f"skip{idx}")),
+            Argument(name="orderBy", value=InputValue.Enum(orderBy_value)),
+            Argument(
+                name="orderDirection",
+                value=InputValue.Enum(get_orderDirection_value(current)),
+            ),
+            Argument(
+                name="where",
+                value=InputValue.Object(
+                    merge_input_value_object_metas(
+                        where_filtering_args.value, where_value
+                    )
                 ),
-            ]
+            ),
+        ]
 
-            selections = current.selection
-            if not any(selections | map(lambda s: s.fmeta.name == "id")):
-                selections.append(
-                    Selection(
-                        fmeta=TypeMeta.FieldMeta(
-                            name="id",
-                            description="",
-                            args=[],
-                            type=TypeRef.Named(name="String", kind="SCALAR"),
-                        )
-                    )
+        # This ensures `id` always exists
+        current = current.add(
+            Selection(
+                fmeta=TypeMeta.FieldMeta(
+                    name="id",
+                    description="",
+                    args=[],
+                    type=TypeRef.Named(name="String", kind="SCALAR"),
                 )
+            )
+        )
 
-            if orderBy_value != "id" and not any(
-                selections | map(lambda s: s.fmeta.name == orderBy_value)
-            ):
-                current_type: TypeMeta.ObjectMeta = schema.type_of_typeref(
-                    current.fmeta.type_
-                )
-                selections.append(
-                    Selection(
+        # Using nested orderBy values (tabulated by "__"), gather the type of the field
+        #  from the schema.
+        orderBy_values = orderBy_value.split("__")
+
+        # Note, we skip the first type since that is the type of the current `Selection`
+        orderBy_types = (
+            orderBy_values
+            | accumulate(
+                func=lambda curr, val: (
+                    schema.type_of_typeref(curr).type_of_field(val)
+                ),
+                initial=schema.type_of_typeref(current.fmeta.type_),
+            )
+            | skip(1)
+        )
+
+        # Generate a `Selection` tree to add to the current selection.
+        # This tree is generated from the orderBy values and types as nested `FieldMeta`
+        #  constructed through `reduce` by placing singular `Selection` objects in the
+        #  `selection` field on the `Selection`.
+        current = current.add(
+            reduce(
+                lambda current, new: replace(current, selection=[new]),
+                zip(orderBy_values, orderBy_types)
+                | map(
+                    lambda tup: Selection(
                         fmeta=TypeMeta.FieldMeta(
-                            name=orderBy_value,
+                            name=tup[0],
                             description="",
                             args=[],
-                            type=current_type.type_of_field(orderBy_value),
-                        )
+                            type=tup[1],
+                        ),
                     )
-                )
-
-            return Selection(
-                fmeta=current.fmeta,
-                alias=current.alias,
-                arguments=pagination_args
-                + current.find_all_args(
-                    lambda arg: arg.name not in PAGINATION_ARGS, recurse=False
                 ),
-                selection=selections,
             )
-        else:
-            return current
+        )
 
-    query = document.query.map(map_f, priority="children")
+        # add the other arguments that aren't used for pagination
+        pagination_args += current.find_all_args(
+            lambda arg: arg.name not in PAGINATION_ARGS, recurse=False
+        )
 
+        return replace(current, arguments=pagination_args)
+
+    query = document.query.map(map_f, priority="children")
     vardefs = list(pagination_nodes | map(PaginationNode.get_vardefs) | traverse)
 
-    return Document(
-        url=document.url,
-        query=query.add_vardefs(vardefs),
-        fragments=document.fragments,  # TODO: normalize fragments
-        variables=document.variables,
-    )
+    # TODO: normalize document fragments
+    return replace(document, query=query.add_vardefs(vardefs))
 
 
 def prune_doc(document: Document, args: dict[str, Any]) -> Document:
     def prune_where_arg(where_arg: Argument) -> Argument:
         input_val: InputValue.Object = where_arg.value
         return Argument(
             name=where_arg.name,
```

### Comparing `subgrounds-1.5.0/subgrounds/pagination/strategies.py` & `subgrounds-1.5.1/subgrounds/pagination/strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
 from __future__ import annotations
 
 from ast import Tuple
 from dataclasses import dataclass, field
 from functools import partial
 from itertools import count
-from pprint import pprint
 from typing import Any, Callable, Iterator, Literal, Optional
 
 from pipe import map, traverse
 
 from subgrounds.pagination.preprocess import (
     PaginationNode,
     generate_pagination_nodes,
@@ -133,15 +132,19 @@
               data (dict): Previous response data
             Raises:
               StopIteration: _description_
             """
             # Current node step
             index_field_data = list(
                 extract_data(
-                    [*self.page_node.key_path, self.page_node.filter_field], data
+                    [
+                        *self.page_node.key_path,
+                        *self.page_node.filter_field.split("__"),
+                    ],
+                    data,
                 )
                 | traverse
             )
             num_entities = len(index_field_data)
             filter_value = index_field_data[-1] if len(index_field_data) > 0 else None
 
             id_data = list(
@@ -255,15 +258,15 @@
             raise SkipPagination
 
         self.arg_generator = LegacyStrategyArgGenerator(pagination_nodes)
         self.normalized_doc = normalize(schema, document, pagination_nodes)
 
     def step(
         self, page_data: Optional[dict[str, Any]] = None
-    ) -> Tuple[Document, dict[str, Any]]:
+    ) -> tuple[Document, dict[str, Any]]:
         args = self.arg_generator.step(page_data)
         trimmed_doc = prune_doc(self.normalized_doc, args)
         return (trimmed_doc, args)
 
 
 @dataclass
 class ShallowStrategyArgGenerator:
```

### Comparing `subgrounds-1.5.0/subgrounds/plotly_wrappers.py` & `subgrounds-1.5.1/subgrounds/plotly_wrappers.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/query.py` & `subgrounds-1.5.1/subgrounds/query.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/schema.py` & `subgrounds-1.5.1/subgrounds/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -378,15 +378,15 @@
     @root_validator(allow_reuse=True)
     def type_map_generator(cls, values):
         if "types" in values and len(values["types"]) > 0:
             values["type_map"] = {type_.name: type_ for type_ in values["types"]}
 
         return values
 
-    def type_of_typeref(self: SchemaMeta, typeref: TypeRef.T) -> TypeMeta.T:
+    def type_of_typeref(self: SchemaMeta, typeref: TypeRef.T) -> TypeMeta_T:
         """Returns the type information of the type reference `typeref`
 
         Args:
         self (SchemaMeta): The schema.
         typeref (TypeRef.T): The type reference pointing to the type of interest.
 
         Raises:
@@ -402,11 +402,27 @@
         except KeyError:
             raise KeyError(
                 f"SchemaMeta.type_of_typeref: No type named {typeref.name} in schema!"
             )
 
     def type_of(
         self: SchemaMeta, tmeta: TypeMeta.ArgumentMeta | TypeMeta.FieldMeta
-    ) -> TypeMeta.T:
+    ) -> TypeMeta_T:
         """Returns the argument or field definition's underlying type"""
 
         return self.type_of_typeref(tmeta.type_)
+
+    def type_of_input_object_meta(
+        self, tmeta: TypeMeta.InputObjectMeta, args: list[str]
+    ) -> TypeRef.T:
+        """Recursively finds the nested type"""
+
+        if len(args) < 1:
+            raise Exception("type_of_input_object_meta: TODO")
+
+        type_ref = tmeta.type_of_input_field(args.pop(0))
+        match self.type_of_typeref(type_ref):
+            case TypeMeta.InputObjectMeta() as tmeta:
+                return self.type_of_input_object_meta(tmeta, args)
+
+            case _:
+                return type_ref
```

### Comparing `subgrounds-1.5.0/subgrounds/subgraph/fieldpath.py` & `subgrounds-1.5.1/subgrounds/subgraph/fieldpath.py`

 * *Files 0% similar despite different names*

```diff
@@ -682,15 +682,15 @@
             """
             match deps:
                 case []:
 
                     def new_f(*args):
                         new_args = []
                         _counter = 0
-                        for (f_, deps) in acc:
+                        for f_, deps in acc:
                             match (f_, deps):
                                 case (None, FieldPath()):
                                     new_args.append(args[_counter])
                                     _counter += 1
                                 case (
                                     None,
                                     int() | float() | str() | bool() as constant,
@@ -701,15 +701,15 @@
                                         f_(*args[_counter : _counter + len(deps)])
                                     )
                                     _counter += len(deps)
 
                         return f(*new_args)
 
                     new_deps = []
-                    for (_, deps) in acc:
+                    for _, deps in acc:
                         match deps:
                             case FieldPath() as dep:
                                 new_deps.append(dep)
                             case int() | float() | str() | bool():
                                 pass
                             case list() as deps:
                                 new_deps = new_deps + deps
```

### Comparing `subgrounds-1.5.0/subgrounds/subgraph/filter.py` & `subgrounds-1.5.1/subgrounds/subgraph/filter.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/subgraph/object.py` & `subgrounds-1.5.1/subgrounds/subgraph/object.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/subgraph/subgraph.py` & `subgrounds-1.5.1/subgrounds/subgraph/subgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ) -> None:
         self._url = url
         self._schema = schema
         self._transforms = transforms
         self._is_subgraph = is_subgraph
 
         # Add objects as attributes
-        for (key, obj) in self._schema.type_map.items():
+        for key, obj in self._schema.type_map.items():
             match obj:
                 case TypeMeta.ObjectMeta() | TypeMeta.InterfaceMeta():
                     super().__setattr__(key, Object(self, obj))
                 case _:
                     pass
 
     def _add_synthetic_field(
```

### Comparing `subgrounds-1.5.0/subgrounds/subgrounds.py` & `subgrounds-1.5.1/subgrounds/subgrounds.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/transform.py` & `subgrounds-1.5.1/subgrounds/transform.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.0/subgrounds/utils.py` & `subgrounds-1.5.1/subgrounds/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Utility module for Subgrounds
 """
 
 import platform
 from functools import cache
+from itertools import accumulate as _accumulate
 from itertools import filterfalse
 from typing import Any, Callable, Iterator, Optional, Tuple, TypeVar
 
 from pipe import Pipe, map
 
+accumulate = Pipe(_accumulate)
+
 
 def flatten(t):
     return [item for sublist in t for item in sublist]
 
 
 def identity(x):
     return x
```

