# Comparing `tmp/dbt-sqlserver-1.3.2.tar.gz` & `tmp/dbt-sqlserver-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-sqlserver-1.3.2.tar", last modified: Fri May 12 21:03:28 2023, max compression
+gzip compressed data, was "dbt-sqlserver-1.4.0.tar", last modified: Mon May 15 20:55:07 2023, max compression
```

## Comparing `dbt-sqlserver-1.3.2.tar` & `dbt-sqlserver-1.4.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.505787 dbt-sqlserver-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-12 21:03:28.505787 dbt-sqlserver-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.497787 dbt-sqlserver-1.3.2/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.501787 dbt-sqlserver-1.3.2/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.501787 dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/sql_server_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/sql_server_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/sql_server_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/sql_server_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/sql_server_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.501787 dbt-sqlserver-1.3.2/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.501787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.497787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.501787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.497787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.497787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.501787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.501787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.501787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.501787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.505787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.505787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/tests/test.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.505787 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:03:28.505787 dbt-sqlserver-1.3.2/dbt_sqlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-12 21:03:28.000000 dbt-sqlserver-1.3.2/dbt_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-12 21:03:28.000000 dbt-sqlserver-1.3.2/dbt_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:03:28.000000 dbt-sqlserver-1.3.2/dbt_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 21:03:28.000000 dbt-sqlserver-1.3.2/dbt_sqlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 21:03:28.000000 dbt-sqlserver-1.3.2/dbt_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:03:28.505787 dbt-sqlserver-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-12 21:02:53.000000 dbt-sqlserver-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/tests/test.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/setup.py
```

### Comparing `dbt-sqlserver-1.3.2/LICENSE` & `dbt-sqlserver-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/PKG-INFO` & `dbt-sqlserver-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-sqlserver
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Microsoft SQL Server adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-sqlserver
 Author: Mikael Ene, Anders Swanson, Sam Debruyn, Cor Zuurmond
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-sqlserver
 
 [dbt](https://www.getdbt.com) adapter for Microsoft SQL Server and Azure SQL services.
```

### Comparing `dbt-sqlserver-1.3.2/README.md` & `dbt-sqlserver-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/__init__.py` & `dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/sql_server_adapter.py` & `dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     def get_rows_different_sql(
         self,
         relation_a: BaseRelation,
         relation_b: BaseRelation,
         column_names: Optional[List[str]] = None,
         except_operator: str = "EXCEPT",
     ) -> str:
-
         """
         note: using is not supported on Synapse so COLUMNS_EQUAL_SQL is adjsuted
         Generate SQL for a query that returns a single row with a two
         columns: the number of rows that are different between the two
         relations and the number of mismatched rows.
         """
         # This method only really exists for test reasons.
```

### Comparing `dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/sql_server_connection_manager.py` & `dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_connection_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,41 +246,39 @@
 
             try:
                 # attempt to release the connection
                 self.release()
             except pyodbc.Error:
                 logger.debug("Failed to release connection!")
 
-            raise dbt.exceptions.DatabaseException(str(e).strip()) from e
+            raise dbt.exceptions.DbtDatabaseError(str(e).strip()) from e
 
         except Exception as e:
             logger.debug(f"Error running SQL: {sql}")
             logger.debug("Rolling back transaction.")
             self.release()
-            if isinstance(e, dbt.exceptions.RuntimeException):
+            if isinstance(e, dbt.exceptions.DbtRuntimeError):
                 # during a sql query, an internal to dbt exception was raised.
                 # this sounds a lot like a signal handler and probably has
                 # useful information, so raise it without modification.
                 raise
 
-            raise dbt.exceptions.RuntimeException(e)
+            raise dbt.exceptions.DbtRuntimeError(e)
 
     @classmethod
     def open(cls, connection: Connection) -> Connection:
-
         if connection.state == ConnectionState.OPEN:
             logger.debug("Connection is already open, skipping open.")
             return connection
 
         credentials = cls.get_credentials(connection.credentials)
 
         con_str = [f"DRIVER={{{credentials.driver}}}"]
 
         if "\\" in credentials.host:
-
             # If there is a backslash \ in the host name, the host is a
             # SQL Server named instance. In this case then port number has to be omitted.
             con_str.append(f"SERVER={credentials.host}")
         else:
             con_str.append(f"SERVER={credentials.host},{credentials.port}")
 
         con_str.append(f"Database={credentials.database}")
@@ -370,15 +368,14 @@
     def add_query(
         self,
         sql: str,
         auto_begin: bool = True,
         bindings: Optional[Any] = None,
         abridge_sql_log: bool = False,
     ) -> Tuple[Connection, Any]:
-
         connection = self.get_thread_connection()
 
         if auto_begin and connection.transaction_open is False:
             self.begin()
 
         logger.debug('Using {} connection "{}".'.format(self.TYPE, connection.name))
```

### Comparing `dbt-sqlserver-1.3.2/dbt/adapters/sqlserver/sql_server_credentials.py` & `dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/apply_grants.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/apply_grants.sql`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% macro sqlserver__get_show_grant_sql(relation) %}
     select
         GRANTEE as grantee,
         PRIVILEGE_TYPE as privilege_type
-    from INFORMATION_SCHEMA.TABLE_PRIVILEGES
+    from INFORMATION_SCHEMA.TABLE_PRIVILEGES with (nolock)
     where TABLE_CATALOG = '{{ relation.database }}'
       and TABLE_SCHEMA = '{{ relation.schema }}'
       and TABLE_NAME = '{{ relation.identifier }}'
 {% endmacro %}
 
 
 {%- macro sqlserver__get_grant_sql(relation, privilege, grantees) -%}
```

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/columns.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/columns.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,31 @@
 {% macro sqlserver__get_columns_in_relation(relation) -%}
   {% call statement('get_columns_in_relation', fetch_result=True) %}
 
-    with
-        regular_db_cols as (
-            select
-                ordinal_position,
-                column_name,
-                data_type,
-                character_maximum_length,
-                numeric_precision,
-                numeric_scale
-            from [{{ relation.database }}].INFORMATION_SCHEMA.COLUMNS
-            where table_name = '{{ relation.identifier }}'
-              and table_schema = '{{ relation.schema }}'
-        ),
-
-        temp_db_cols as (
-            select
-                ordinal_position,
-                column_name collate database_default as column_name,
-                data_type collate database_default as data_type,
-                character_maximum_length,
-                numeric_precision,
-                numeric_scale
-            from tempdb.INFORMATION_SCHEMA.COLUMNS
-            where table_name like '{{ relation.identifier }}%'
-        ),
-
-        all_cols as (
-            select *
-            from regular_db_cols
-            union
-            select *
-            from temp_db_cols
-        )
+    with mapping as (
+        select
+            row_number() over (partition by object_name(c.object_id) order by c.column_id) as ordinal_position,
+            c.name collate database_default as column_name,
+            t.name as data_type,
+            c.max_length as character_maximum_length,
+            c.precision as numeric_precision,
+            c.scale as numeric_scale
+        from [{{ 'tempdb' if '#' in relation.identifier else relation.database }}].sys.columns c with (nolock)
+        inner join sys.types t with (nolock)
+        on c.user_type_id = t.user_type_id
+        where c.object_id = object_id('{{ 'tempdb..' ~ relation.include(database=false, schema=false) if '#' in relation.identifier else relation }}')
+    )
 
     select
         column_name,
         data_type,
         character_maximum_length,
         numeric_precision,
         numeric_scale
-    from
-        all_cols
+    from mapping
     order by ordinal_position
 
   {% endcall %}
   {% set table = load_result('get_columns_in_relation').table %}
   {{ return(sql_convert_columns_in_relation(table)) }}
 {% endmacro %}
 
@@ -63,16 +42,35 @@
 {% endmacro %}
 
 {% macro sqlserver__alter_column_type(relation, column_name, new_column_type) %}
 
   {%- set tmp_column = column_name + "__dbt_alter" -%}
 
   {% call statement('alter_column_type') -%}
-
-    alter {{ relation.type }} {{ relation }} add {{ tmp_column }} {{ new_column_type }};
-    update {{ relation }} set {{ tmp_column }} = {{ column_name }};
-    alter {{ relation.type }} {{ relation }} drop column {{ column_name }};
+    alter {{ relation.type }} {{ relation }} add "{{ tmp_column }}" {{ new_column_type }};
+  {%- endcall -%}
+  {% call statement('alter_column_type') -%}
+    update {{ relation }} set "{{ tmp_column }}" = "{{ column_name }}";
+  {%- endcall -%}
+  {% call statement('alter_column_type') -%}
+    alter {{ relation.type }} {{ relation }} drop column "{{ column_name }}";
+  {%- endcall -%}
+  {% call statement('alter_column_type') -%}
     exec sp_rename '{{ relation | replace('"', '') }}.{{ tmp_column }}', '{{ column_name }}', 'column'
-
   {%- endcall -%}
 
 {% endmacro %}
+
+
+{% macro sqlserver__alter_relation_add_remove_columns(relation, add_columns, remove_columns) %}
+  {% call statement('add_drop_columns') -%}
+    {% if add_columns %}
+        alter {{ relation.type }} {{ relation }}
+        add {% for column in add_columns %}"{{ column.name }}" {{ column.data_type }}{{ ', ' if not loop.last }}{% endfor %};
+    {% endif %}
+
+    {% if remove_columns %}
+        alter {{ relation.type }} {{ relation }}
+        drop column {% for column in remove_columns %}"{{ column.name }}"{{ ',' if not loop.last }}{% endfor %};
+    {% endif %}
+  {%- endcall -%}
+{% endmacro %}
```

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/indexes.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/metadata.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/metadata.sql`

 * *Files 6% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         select
             table_catalog as table_database,
             table_schema,
             table_name,
             column_name,
             ordinal_position as column_index,
             data_type as column_type
-        from INFORMATION_SCHEMA.COLUMNS
+        from INFORMATION_SCHEMA.COLUMNS with (nolock)
 
     )
 
     select
         cols.table_database,
         tv.schema_name as table_schema,
         tv.table_name,
@@ -114,22 +114,26 @@
     {%- endcall -%}
 
   {{ return(load_result('catalog').table) }}
 
 {%- endmacro %}
 
 {% macro sqlserver__information_schema_name(database) -%}
-  information_schema
+  {%- if database -%}
+    [{{ database }}].INFORMATION_SCHEMA
+  {%- else -%}
+    INFORMATION_SCHEMA
+  {%- endif -%}
 {%- endmacro %}
 
 {% macro sqlserver__list_schemas(database) %}
   {% call statement('list_schemas', fetch_result=True, auto_begin=False) -%}
     USE {{ database }};
     select  name as [schema]
-    from sys.schemas
+    from sys.schemas with (nolock)
   {% endcall %}
   {{ return(load_result('list_schemas').table) }}
 {% endmacro %}
 
 {% macro sqlserver__check_schema_exists(information_schema, schema) -%}
   {% call statement('check_schema_exists', fetch_result=True, auto_begin=False) -%}
     --USE {{ database_name }}
@@ -145,12 +149,12 @@
       table_name as [name],
       table_schema as [schema],
       case when table_type = 'BASE TABLE' then 'table'
            when table_type = 'VIEW' then 'view'
            else table_type
       end as table_type
 
-    from [{{ schema_relation.database }}].INFORMATION_SCHEMA.TABLES
+    from [{{ schema_relation.database }}].INFORMATION_SCHEMA.TABLES with (nolock)
     where table_schema like '{{ schema_relation.schema }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
```

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/adapters/schema.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,57 @@
   {# global project no longer includes semi-colons in merge statements, so
      default macro are invoked below w/ a semi-colons after it.
      more context:
      https://github.com/dbt-labs/dbt-core/pull/3510
      https://getdbt.slack.com/archives/C50NEBJGG/p1636045535056600
   #}
 
-{% macro sqlserver__get_merge_sql(target, source, unique_key, dest_columns, predicates) %}
-  {{ default__get_merge_sql(target, source, unique_key, dest_columns, predicates) }};
+{% macro sqlserver__get_merge_sql(target, source, unique_key, dest_columns, incremental_predicates=none) %}
+  {{ default__get_merge_sql(target, source, unique_key, dest_columns, incremental_predicates) }};
 {% endmacro %}
 
-{% macro sqlserver__get_delete_insert_merge_sql(target, source, unique_key, dest_columns) %}
+{% macro sqlserver__get_insert_overwrite_merge_sql(target, source, dest_columns, predicates, include_sql_header) %}
+  {{ default__get_insert_overwrite_merge_sql(target, source, dest_columns, predicates, include_sql_header) }};
+{% endmacro %}
 
-      {%- set dest_cols_csv = get_quoted_csv(dest_columns | map(attribute="name")) -%}
+{% macro sqlserver__get_delete_insert_merge_sql(target, source, unique_key, dest_columns, incremental_predicates=none) %}
+    {%- set dest_cols_csv = get_quoted_csv(dest_columns | map(attribute="name")) -%}
 
-      {% if unique_key %}
-      {% if unique_key is sequence and unique_key is not string %}
-      delete from {{ target }}
-          where exists (
-                SELECT NULL
-                FROM
-                  {{ source }}
-                WHERE
+    {% if unique_key %}
+        {% if unique_key is sequence and unique_key is not string %}
+            delete from {{ target }}
+            where exists (
+                select null
+                from {{ source }}
+                where
                 {% for key in unique_key %}
                     {{ source }}.{{ key }} = {{ target }}.{{ key }}
                     {{ "and " if not loop.last }}
                 {% endfor %}
-            );
-      {% else %}
-      delete from {{ target }}
-          where (
-                {{ unique_key }}) in (
-      select ({{ unique_key }})
-      from {{ source }}
-          );
-
-      {% endif %}
-      {% endif %}
-
-      insert into {{ target }} ({{ dest_cols_csv }})
-          (
-      select {{ dest_cols_csv }}
-      from {{ source }}
-          )
-
-{% endmacro %}
 
-{% macro sqlserver__get_insert_overwrite_merge_sql(target, source, dest_columns, predicates, include_sql_header) %}
-  {{ default__get_insert_overwrite_merge_sql(target, source, dest_columns, predicates, include_sql_header) }};
+            )
+            {% if incremental_predicates %}
+                {% for predicate in incremental_predicates %}
+                    and {{ predicate }}
+                {% endfor %}
+            {% endif %};
+        {% else %}
+            delete from {{ target }}
+            where (
+                {{ unique_key }}) in (
+                select ({{ unique_key }})
+                from {{ source }}
+            )
+            {%- if incremental_predicates %}
+                {% for predicate in incremental_predicates %}
+                    and {{ predicate }}
+                {% endfor %}
+            {%- endif -%};
+        {% endif %}
+    {% endif %}
+
+    insert into {{ target }} ({{ dest_cols_csv }})
+    (
+        select {{ dest_cols_csv }}
+        from {{ source }}
+    )
 {% endmacro %}
```

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/materializations/tests/test.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/dbt/include/sqlserver/macros/utils/split_part.sql` & `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.3.2/dbt_sqlserver.egg-info/PKG-INFO` & `dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-sqlserver
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Microsoft SQL Server adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-sqlserver
 Author: Mikael Ene, Anders Swanson, Sam Debruyn, Cor Zuurmond
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-sqlserver
 
 [dbt](https://www.getdbt.com) adapter for Microsoft SQL Server and Azure SQL services.
```

### Comparing `dbt-sqlserver-1.3.2/dbt_sqlserver.egg-info/SOURCES.txt` & `dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 dbt/adapters/sqlserver/sql_server_connection_manager.py
 dbt/adapters/sqlserver/sql_server_credentials.py
 dbt/include/__init__.py
 dbt/include/sqlserver/__init__.py
 dbt/include/sqlserver/dbt_project.yml
 dbt/include/sqlserver/macros/adapters/apply_grants.sql
 dbt/include/sqlserver/macros/adapters/columns.sql
-dbt/include/sqlserver/macros/adapters/freshness.sql
 dbt/include/sqlserver/macros/adapters/indexes.sql
 dbt/include/sqlserver/macros/adapters/metadata.sql
 dbt/include/sqlserver/macros/adapters/persist_docs.sql
 dbt/include/sqlserver/macros/adapters/relation.sql
 dbt/include/sqlserver/macros/adapters/schema.sql
 dbt/include/sqlserver/macros/materializations/models/incremental/incremental_strategies.sql
 dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql
@@ -41,12 +40,13 @@
 dbt/include/sqlserver/macros/utils/hash.sql
 dbt/include/sqlserver/macros/utils/last_day.sql
 dbt/include/sqlserver/macros/utils/length.sql
 dbt/include/sqlserver/macros/utils/listagg.sql
 dbt/include/sqlserver/macros/utils/position.sql
 dbt/include/sqlserver/macros/utils/safe_cast.sql
 dbt/include/sqlserver/macros/utils/split_part.sql
+dbt/include/sqlserver/macros/utils/timestamps.sql
 dbt_sqlserver.egg-info/PKG-INFO
 dbt_sqlserver.egg-info/SOURCES.txt
 dbt_sqlserver.egg-info/dependency_links.txt
 dbt_sqlserver.egg-info/requires.txt
 dbt_sqlserver.egg-info/top_level.txt
```

### Comparing `dbt-sqlserver-1.3.2/setup.py` & `dbt-sqlserver-1.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 
 from setuptools import find_namespace_packages, setup
 from setuptools.command.install import install
 
 package_name = "dbt-sqlserver"
 authors_list = ["Mikael Ene", "Anders Swanson", "Sam Debruyn", "Cor Zuurmond"]
-dbt_version = "1.3"
+dbt_version = "1.4"
 description = """A Microsoft SQL Server adapter plugin for dbt"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
@@ -62,26 +62,27 @@
     long_description_content_type="text/markdown",
     license="MIT",
     author=", ".join(authors_list),
     url="https://github.com/dbt-msft/dbt-sqlserver",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-core~=1.3.4",
-        "pyodbc>=4.0.32,!=4.0.34",
-        "azure-identity>=1.10.0",
+        "dbt-core~=1.4.5",
+        "pyodbc~=4.0.35,!=4.0.36,!=4.0.37",
+        "azure-identity>=1.12.0",
     ],
     cmdclass={
         "verify": VerifyVersionCommand,
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

