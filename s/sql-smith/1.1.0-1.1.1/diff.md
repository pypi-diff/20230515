# Comparing `tmp/sql_smith-1.1.0.tar.gz` & `tmp/sql_smith-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_smith-1.1.0.tar", max compression
+gzip compressed data, was "sql_smith-1.1.1.tar", max compression
```

## Comparing `sql_smith-1.1.0.tar` & `sql_smith-1.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1069 2022-12-20 20:32:20.605117 sql_smith-1.1.0/LICENSE
--rw-r--r--   0        0        0     1617 2022-12-21 07:03:12.247114 sql_smith-1.1.0/README.rst
--rw-r--r--   0        0        0      975 2023-05-09 15:31:55.047479 sql_smith-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/__init__.py
--rw-r--r--   0        0        0      130 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/builder/__init__.py
--rw-r--r--   0        0        0     1564 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/builder/criteria_builder.py
--rw-r--r--   0        0        0     1150 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/builder/like_builder.py
--rw-r--r--   0        0        0      440 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/capability/__init__.py
--rw-r--r--   0        0        0      310 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/capability/can_union.py
--rw-r--r--   0        0        0      569 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/capability/has_from.py
--rw-r--r--   0        0        0      331 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/capability/has_limit.py
--rw-r--r--   0        0        0      364 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/capability/has_offset.py
--rw-r--r--   0        0        0      532 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/capability/has_order_by.py
--rw-r--r--   0        0        0      372 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/capability/has_returning.py
--rw-r--r--   0        0        0      683 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/capability/has_where.py
--rw-r--r--   0        0        0      386 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/engine/__init__.py
--rw-r--r--   0        0        0     2598 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/engine/basic_engine.py
--rw-r--r--   0        0        0      293 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/engine/common_engine.py
--rw-r--r--   0        0        0      802 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/engine/mysql_engine.py
--rw-r--r--   0        0        0      655 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/engine/postgres_engine.py
--rw-r--r--   0        0        0     1022 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/engine/sql_server_engine.py
--rw-r--r--   0        0        0      430 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/engine/sqlite_engine.py
--rw-r--r--   0        0        0     3803 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/functions.py
--rw-r--r--   0        0        0      384 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/interfaces/__init__.py
--rw-r--r--   0        0        0      436 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/interfaces/criteria_interface.py
--rw-r--r--   0        0        0     1715 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/interfaces/engine_interface.py
--rw-r--r--   0        0        0      329 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/interfaces/expression_interface.py
--rw-r--r--   0        0        0      393 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/interfaces/query_interface.py
--rw-r--r--   0        0        0      336 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/interfaces/statement_interface.py
--rw-r--r--   0        0        0      499 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/partial/__init__.py
--rw-r--r--   0        0        0      663 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/partial/criteria.py
--rw-r--r--   0        0        0      725 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/partial/expression.py
--rw-r--r--   0        0        0      336 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/partial/identifier.py
--rw-r--r--   0        0        0      366 2023-05-09 15:31:55.047479 sql_smith-1.1.0/src/sql_smith/partial/like_begins.py
--rw-r--r--   0        0        0      374 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/partial/like_contains.py
--rw-r--r--   0        0        0      364 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/partial/like_ends.py
--rw-r--r--   0        0        0      477 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/partial/listing.py
--rw-r--r--   0        0        0      311 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/partial/literal.py
--rw-r--r--   0        0        0      176 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/partial/parameter/__init__.py
--rw-r--r--   0        0        0      343 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/partial/parameter/bool_parameter.py
--rw-r--r--   0        0        0      270 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/partial/parameter/null_parameter.py
--rw-r--r--   0        0        0      696 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/partial/parameter/parameter.py
--rw-r--r--   0        0        0      423 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/partial/qualified_identifier.py
--rw-r--r--   0        0        0      398 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/__init__.py
--rw-r--r--   0        0        0     1023 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/abstract_query.py
--rw-r--r--   0        0        0      770 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/delete_query.py
--rw-r--r--   0        0        0     1796 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/insert_query.py
--rw-r--r--   0        0        0      118 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/mysql/__init__.py
--rw-r--r--   0        0        0      555 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/mysql/insert_query.py
--rw-r--r--   0        0        0      617 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/mysql/select_query.py
--rw-r--r--   0        0        0      118 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/postgres/__init__.py
--rw-r--r--   0        0        0      384 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/postgres/insert_query.py
--rw-r--r--   0        0        0      384 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/postgres/update_query.py
--rw-r--r--   0        0        0      413 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/query.py
--rw-r--r--   0        0        0     5506 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/select_query.py
--rw-r--r--   0        0        0      118 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/sql_server/__init__.py
--rw-r--r--   0        0        0      512 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/sql_server/delete_query.py
--rw-r--r--   0        0        0      632 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/sql_server/select_query.py
--rw-r--r--   0        0        0     1285 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/union_query.py
--rw-r--r--   0        0        0     1644 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query/update_query.py
--rw-r--r--   0        0        0     1428 2023-05-09 15:31:55.051479 sql_smith-1.1.0/src/sql_smith/query_factory.py
--rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 sql_smith-1.1.0/setup.py
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 sql_smith-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-09 18:13:59.927440 sql_smith-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1617 2023-05-09 18:13:59.927440 sql_smith-1.1.1/README.rst
+-rw-r--r--   0        0        0      975 2023-05-15 15:22:30.566362 sql_smith-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/__init__.py
+-rw-r--r--   0        0        0      130 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/builder/__init__.py
+-rw-r--r--   0        0        0     1564 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/builder/criteria_builder.py
+-rw-r--r--   0        0        0     1150 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/builder/like_builder.py
+-rw-r--r--   0        0        0      440 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/capability/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/capability/can_union.py
+-rw-r--r--   0        0        0      569 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/capability/has_from.py
+-rw-r--r--   0        0        0      481 2023-05-15 15:19:04.411083 sql_smith-1.1.1/src/sql_smith/capability/has_limit.py
+-rw-r--r--   0        0        0      508 2023-05-15 15:16:59.579539 sql_smith-1.1.1/src/sql_smith/capability/has_offset.py
+-rw-r--r--   0        0        0      633 2023-05-15 15:20:15.122832 sql_smith-1.1.1/src/sql_smith/capability/has_order_by.py
+-rw-r--r--   0        0        0      372 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/capability/has_returning.py
+-rw-r--r--   0        0        0      844 2023-05-15 15:07:40.713921 sql_smith-1.1.1/src/sql_smith/capability/has_where.py
+-rw-r--r--   0        0        0      386 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/engine/__init__.py
+-rw-r--r--   0        0        0     2598 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/engine/basic_engine.py
+-rw-r--r--   0        0        0      293 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/engine/common_engine.py
+-rw-r--r--   0        0        0      802 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/engine/mysql_engine.py
+-rw-r--r--   0        0        0      655 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/engine/postgres_engine.py
+-rw-r--r--   0        0        0     1022 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/engine/sql_server_engine.py
+-rw-r--r--   0        0        0      430 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/engine/sqlite_engine.py
+-rw-r--r--   0        0        0     3803 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/functions.py
+-rw-r--r--   0        0        0      384 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/interfaces/__init__.py
+-rw-r--r--   0        0        0      436 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/interfaces/criteria_interface.py
+-rw-r--r--   0        0        0     1715 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/interfaces/engine_interface.py
+-rw-r--r--   0        0        0      329 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/interfaces/expression_interface.py
+-rw-r--r--   0        0        0      393 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/interfaces/query_interface.py
+-rw-r--r--   0        0        0      336 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/interfaces/statement_interface.py
+-rw-r--r--   0        0        0      499 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/partial/__init__.py
+-rw-r--r--   0        0        0      663 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/partial/criteria.py
+-rw-r--r--   0        0        0      725 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/partial/expression.py
+-rw-r--r--   0        0        0      336 2023-05-09 18:13:59.931440 sql_smith-1.1.1/src/sql_smith/partial/identifier.py
+-rw-r--r--   0        0        0      366 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/like_begins.py
+-rw-r--r--   0        0        0      374 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/like_contains.py
+-rw-r--r--   0        0        0      364 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/like_ends.py
+-rw-r--r--   0        0        0      477 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/listing.py
+-rw-r--r--   0        0        0      311 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/literal.py
+-rw-r--r--   0        0        0      176 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/parameter/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/parameter/bool_parameter.py
+-rw-r--r--   0        0        0      270 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/parameter/null_parameter.py
+-rw-r--r--   0        0        0      696 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/parameter/parameter.py
+-rw-r--r--   0        0        0      423 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/partial/qualified_identifier.py
+-rw-r--r--   0        0        0      398 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/__init__.py
+-rw-r--r--   0        0        0     1023 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/abstract_query.py
+-rw-r--r--   0        0        0      770 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/delete_query.py
+-rw-r--r--   0        0        0     1796 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/insert_query.py
+-rw-r--r--   0        0        0      118 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/mysql/__init__.py
+-rw-r--r--   0        0        0      555 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/mysql/insert_query.py
+-rw-r--r--   0        0        0      617 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/mysql/select_query.py
+-rw-r--r--   0        0        0      118 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/postgres/__init__.py
+-rw-r--r--   0        0        0      384 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/postgres/insert_query.py
+-rw-r--r--   0        0        0      384 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/postgres/update_query.py
+-rw-r--r--   0        0        0      413 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/query.py
+-rw-r--r--   0        0        0     5506 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/select_query.py
+-rw-r--r--   0        0        0      118 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/sql_server/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/sql_server/delete_query.py
+-rw-r--r--   0        0        0      632 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/sql_server/select_query.py
+-rw-r--r--   0        0        0     1285 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/union_query.py
+-rw-r--r--   0        0        0     1644 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query/update_query.py
+-rw-r--r--   0        0        0     1428 2023-05-09 18:13:59.935440 sql_smith-1.1.1/src/sql_smith/query_factory.py
+-rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 sql_smith-1.1.1/setup.py
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 sql_smith-1.1.1/PKG-INFO
```

### Comparing `sql_smith-1.1.0/LICENSE` & `sql_smith-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/README.rst` & `sql_smith-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/pyproject.toml` & `sql_smith-1.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-smith"
-version = "1.1.0"
+version = "1.1.1"
 description = "sql-smith is an SQL query builder with zero dependencies and a fluent interface."
 authors = ["fbraem <franky.braem@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `sql_smith-1.1.0/src/sql_smith/builder/criteria_builder.py` & `sql_smith-1.1.1/src/sql_smith/builder/criteria_builder.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/builder/like_builder.py` & `sql_smith-1.1.1/src/sql_smith/builder/like_builder.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/capability/has_from.py` & `sql_smith-1.1.1/src/sql_smith/capability/has_from.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/capability/has_order_by.py` & `sql_smith-1.1.1/src/sql_smith/capability/has_order_by.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from sql_smith.functions import order, listing
 
 
 class HasOrderByMixin:
-    def order_by(self, column: str = None, direction: str = None):
+    def order_by(self, column: str | None = None, direction: str | None = None):
         if column:
             self._order_by.append(order(column, direction))
             return self
 
         self._order_by = []
         return self
 
+    @property
+    def has_order(self) -> bool:
+        return len(self._order_by) > 0
+
     def _apply_order_by(self, query: "ExpressionInterface") -> "ExpressionInterface":
         return (
             query.append("ORDER BY {}", listing(self._order_by))
             if len(self._order_by) > 0
             else query
         )
```

### Comparing `sql_smith-1.1.0/src/sql_smith/engine/basic_engine.py` & `sql_smith-1.1.1/src/sql_smith/engine/basic_engine.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/engine/mysql_engine.py` & `sql_smith-1.1.1/src/sql_smith/engine/mysql_engine.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/engine/postgres_engine.py` & `sql_smith-1.1.1/src/sql_smith/engine/postgres_engine.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/engine/sql_server_engine.py` & `sql_smith-1.1.1/src/sql_smith/engine/sql_server_engine.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/functions.py` & `sql_smith-1.1.1/src/sql_smith/functions.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/interfaces/engine_interface.py` & `sql_smith-1.1.1/src/sql_smith/interfaces/engine_interface.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/partial/criteria.py` & `sql_smith-1.1.1/src/sql_smith/partial/criteria.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/partial/expression.py` & `sql_smith-1.1.1/src/sql_smith/partial/expression.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/partial/parameter/parameter.py` & `sql_smith-1.1.1/src/sql_smith/partial/parameter/parameter.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/abstract_query.py` & `sql_smith-1.1.1/src/sql_smith/query/abstract_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/delete_query.py` & `sql_smith-1.1.1/src/sql_smith/query/delete_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/insert_query.py` & `sql_smith-1.1.1/src/sql_smith/query/insert_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/mysql/insert_query.py` & `sql_smith-1.1.1/src/sql_smith/query/mysql/insert_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/mysql/select_query.py` & `sql_smith-1.1.1/src/sql_smith/query/mysql/select_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/select_query.py` & `sql_smith-1.1.1/src/sql_smith/query/select_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/sql_server/delete_query.py` & `sql_smith-1.1.1/src/sql_smith/query/sql_server/delete_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/sql_server/select_query.py` & `sql_smith-1.1.1/src/sql_smith/query/sql_server/select_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/union_query.py` & `sql_smith-1.1.1/src/sql_smith/query/union_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query/update_query.py` & `sql_smith-1.1.1/src/sql_smith/query/update_query.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/src/sql_smith/query_factory.py` & `sql_smith-1.1.1/src/sql_smith/query_factory.py`

 * *Files identical despite different names*

### Comparing `sql_smith-1.1.0/setup.py` & `sql_smith-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'sql_smith.query.sql_server']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'sql-smith',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'sql-smith is an SQL query builder with zero dependencies and a fluent interface.',
     'long_description': '=========\nsql-smith\n=========\n\n**sql-smith** is an SQL query builder with zero dependencies and a fluent interface.\n\n    The sentence above is, beside the name, a copy from the website of the PHP library\n    Latitude_, for the simple reason that this Python module is a port of Latitude.\n\nRead the full `documentation <https://fbraem.github.io/sql-smith>`_.\n\nInstallation\n************\n\n.. code-block:: sh\n\n    $ pip install sql-smith\n\nQuick Start\n***********\n\nQueryFactory is a factory to create a **SELECT**, **INSERT**, **UPDATE** or **DELETE** query.\nUse the fluent interface of the queries to complete the query.\n\n.. code-block:: python\n\n    from sql_smith import QueryFactory\n    from sql_smith.engine import CommonEngine\n    from sql_smith.functions import field\n    \n    factory = QueryFactory(CommonEngine())\n    query = factory \\\n        .select(\'id\', \'username\') \\\n        .from_(\'users\') \\\n        .where(field(\'id\').eq(5)) \\\n        .compile()\n    \n    print(query.sql)  # SELECT "id", "username" FROM "users" WHERE "id" = ?\n    print(query.params)  # (5)\n\nWhen the query is ready, compile it. The return value of compile is a Query class instance\nwith two properties: sql and params. Use these properties to pass the query to a database.\n\n.. code-block:: python\n\n    import sqlite3\n    \n    db = sqlite3.connect(\'test.db\')\n    cur = db.cursor()\n\n    for row in cur.execute(query.sql, query.params):\n        print(row)\n\nAcknowledgment\n==============\nBig thanks to JetBrains_ to let me use PyCharm for free!\n\n.. _Latitude: https://latitude.shadowhand.com/\n.. _JetBrains: https://www.jetbrains.com/pycharm/\n',
     'author': 'fbraem',
     'author_email': 'franky.braem@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `sql_smith-1.1.0/PKG-INFO` & `sql_smith-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-smith
-Version: 1.1.0
+Version: 1.1.1
 Summary: sql-smith is an SQL query builder with zero dependencies and a fluent interface.
 License: MIT
 Keywords: sql-smith,query,builder,querybuilder,sql,mysql,sqlite,postgres,sqlserver,database
 Author: fbraem
 Author-email: franky.braem@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

