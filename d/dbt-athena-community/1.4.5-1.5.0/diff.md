# Comparing `tmp/dbt-athena-community-1.4.5.tar.gz` & `tmp/dbt-athena-community-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-athena-community-1.4.5.tar", last modified: Thu May  4 10:11:45 2023, max compression
+gzip compressed data, was "dbt-athena-community-1.5.0.tar", last modified: Mon May 15 13:38:15 2023, max compression
```

## Comparing `dbt-athena-community-1.4.5.tar` & `dbt-athena-community-1.5.0.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22332 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/adapters/athena/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32056 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.844940 dbt-athena-community-1.4.5/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/include/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.844940 dbt-athena-community-1.4.5/dbt/include/athena/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.844940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.844940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/ddl_data_type.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.842986 dbt-athena-community-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24015 2023-05-15 13:38:15.842986 dbt-athena-community-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.822985 dbt-athena-community-1.5.0/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.822985 dbt-athena-community-1.5.0/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.826985 dbt-athena-community-1.5.0/dbt/adapters/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36236 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.818985 dbt-athena-community-1.5.0/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.830985 dbt-athena-community-1.5.0/dbt/include/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.822985 dbt-athena-community-1.5.0/dbt/include/athena/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.830985 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.822985 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.818985 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.838986 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.842986 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24015 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:38:15.842986 dbt-athena-community-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/setup.py
```

### Comparing `dbt-athena-community-1.4.5/LICENSE.txt` & `dbt-athena-community-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/PKG-INFO` & `dbt-athena-community-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,18 @@
-Metadata-Version: 2.1
-Name: dbt-athena-community
-Version: 1.4.5
-Summary: The athena adapter plugin for dbt (data build tool)
-Home-page: https://github.com/dbt-athena/dbt-athena
-License: Apache License 2.0
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/"><img src="https://badge.fury.io/py/dbt-athena-community.svg" /></a>
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
 
 ## Features
 
-* Supports dbt version `1.4.*`
+* Supports dbt version `1.5.*`
 * Supports [seeds][seeds]
 * Correctly detects views and their columns
 * Supports [table materialization][table]
   * [Iceberg tables][athena-iceberg] are supported **only with Athena Engine v3** and **a unique table location**
   (see table location section below)
   * Hive tables are supported by both Athena engines.
 * Supports [incremental models][incremental]
@@ -131,25 +111,29 @@
 
 
 ## Models
 
 ### Table Configuration
 
 * `external_location` (`default=none`)
-  * If set, the full S3 path in which the table will be saved. (Does not work with Iceberg table).
+  * If set, the full S3 path in which the table will be saved.
+  * Does not work with Iceberg table or Hive table with `ha` set to true.
 * `partitioned_by` (`default=none`)
   * An array list of columns by which the table will be partitioned
   * Limited to creation of 100 partitions (_currently_)
 * `bucketed_by` (`default=none`)
   * An array list of columns to bucket data, ignored if using Iceberg
 * `bucket_count` (`default=none`)
   * The number of buckets for bucketing your data, ignored if using Iceberg
 * `table_type` (`default='hive'`)
   * The type of table
   * Supports `hive` or `iceberg`
+* `ha` (`default=false`)
+  * If the table should be built using the high-availability method. This option is only available for Hive tables
+    since it is by default for Iceberg tables (see the section [below](#highly-available-table))
 * `format` (`default='parquet'`)
   * The data format for the table
   * Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE`
 * `write_compression` (`default=none`)
   * The compression type to use for any storage format that allows compression to be specified. To see which options are available, check out [CREATE TABLE AS][create-table-as]
 * `field_delimiter` (`default=none`)
   * Custom field delimiter, for when format is set to `TEXTFILE`
@@ -168,15 +152,15 @@
 The location in which a table is saved is determined by:
 
 1. If `external_location` is defined, that value is used.
 2. If `s3_data_dir` is defined, the path is determined by that and `s3_data_naming`
 3. If `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/`
 
 Here all the options available for `s3_data_naming`:
-* `uuid`: `{s3_data_dir}/{uuid4()}/`
+* `unique`: `{s3_data_dir}/{uuid4()}/`
 * `table`: `{s3_data_dir}/{table}/`
 * `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/`
 * `schema_table`: `{s3_data_dir}/{schema}/{table}/`
 * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/{table}/{uuid4()}/`
 
 It's possible to set the `s3_data_naming` globally in the target profile, or overwrite the value in the table config,
 or setting up the value for groups of model in dbt_project.yml.
@@ -263,25 +247,27 @@
 	'active' as status,
 	17.89 as cost,
 	1 as quantity,
 	100000000 as quantity_big,
 	current_date as my_date
 ```
 
-### High availability table materialization
+### Highly available table
 The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
-To have the less destructive behavior it's possible to use `table='table_hive_ha'` materialization.
-**table_hive_ha** leverages the table versions feature of Glue catalog, creating a temp table and swapping
-the target table to the location of the temp table.
-This materialization is only available for `table_type='hive'` and requires using unique locations.
+To have the less destructive behavior it's possible to use the `ha` config on your `table` materialized models.
+It leverages the table versions feature of glue catalog, creating a tmp table and swapping the target table to the
+location of the tmp table. This materialization is only available for `table_type=hive` and requires using unique
+locations. For iceberg, high availability is by default.
 
 ```sql
 {{ config(
-    materialized='table_hive_ha',
+    materialized='table',
+    ha=true,
     format='parquet',
+    table_type='hive',
     partition_by=['status'],
     s3_data_naming='table_unique'
 ) }}
 
 select
   'a' as user_id,
   'pi' as user_name,
@@ -423,14 +409,24 @@
 
 * In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not installed in the target environment.
   See https://github.com/dbt-athena/dbt-athena/issues/103 for more details.
 
 * Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
 
 
+## Contracts
+
+The adapter partly supports contract definition.
+* Concerning the `data_type`, it is supported but needs to be adjusted for complex types. They must be specified
+  entirely (for instance `array<int>`) even though they won't be checked. Indeed, as dbt recommends, we only compare
+  the broader type (array, map, int, varchar). The complete definition is used in order to check that the data types
+  defined in athena are ok (pre-flight check).
+* the adapter does not support the constraints since no constraints don't exist in Athena.
+
+
 ## Contributing
 
 See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 
 ## Contributors ✨
```

#### html2text {}

```diff
@@ -1,25 +1,14 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.5 Summary: The
-athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
-dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
  code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
                                     month]
-## Features * Supports dbt version `1.4.*` * Supports [seeds][seeds] *
+## Features * Supports dbt version `1.5.*` * Supports [seeds][seeds] *
 Correctly detects views and their columns * Supports [table materialization]
 [table] * [Iceberg tables][athena-iceberg] are supported **only with Athena
 Engine v3** and **a unique table location** (see table location section below)
 * Hive tables are supported by both Athena engines. * Supports [incremental
 models][incremental] * On Iceberg tables : * Supports the use of `unique_key`
 only with the `merge` strategy * Supports the `append` strategy * On Hive
 tables : * Supports two incremental update strategies: `insert_overwrite` and
@@ -73,38 +62,42 @@
 profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
 s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
 your_s3_bucket/dbt/ s3_data_naming: schema_table region_name: eu-west-1 schema:
 dbt database: awsdatacatalog aws_profile_name: my-profile work_group: my-
 workgroup lf_tags: origin: dbt team: analytics ``` _Additional information_ *
 `threads` is supported * `database` and `catalog` can be used interchangeably
 ## Models ### Table Configuration * `external_location` (`default=none`) * If
-set, the full S3 path in which the table will be saved. (Does not work with
-Iceberg table). * `partitioned_by` (`default=none`) * An array list of columns
-by which the table will be partitioned * Limited to creation of 100 partitions
-(_currently_) * `bucketed_by` (`default=none`) * An array list of columns to
-bucket data, ignored if using Iceberg * `bucket_count` (`default=none`) * The
-number of buckets for bucketing your data, ignored if using Iceberg *
-`table_type` (`default='hive'`) * The type of table * Supports `hive` or
-`iceberg` * `format` (`default='parquet'`) * The data format for the table *
-Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
+set, the full S3 path in which the table will be saved. * Does not work with
+Iceberg table or Hive table with `ha` set to true. * `partitioned_by`
+(`default=none`) * An array list of columns by which the table will be
+partitioned * Limited to creation of 100 partitions (_currently_) *
+`bucketed_by` (`default=none`) * An array list of columns to bucket data,
+ignored if using Iceberg * `bucket_count` (`default=none`) * The number of
+buckets for bucketing your data, ignored if using Iceberg * `table_type`
+(`default='hive'`) * The type of table * Supports `hive` or `iceberg` * `ha`
+(`default=false`) * If the table should be built using the high-availability
+method. This option is only available for Hive tables since it is by default
+for Iceberg tables (see the section [below](#highly-available-table)) *
+`format` (`default='parquet'`) * The data format for the table * Supports
+`ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
 (`default=none`) * The compression type to use for any storage format that
 allows compression to be specified. To see which options are available, check
 out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
 Custom field delimiter, for when format is set to `TEXTFILE` *
 `table_properties`: table properties to add to the table, valid for Iceberg
 only * `lf_tags` (`default=none`) * lf tags to associate with the table *
 format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
 (`default=none`) * lf tags to associate with the table columns * format: `
 {"tag1": {"value1": ["column1": "column2"]}}` [create-table-as]: https://
 docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 ### Table location The location in which a table is saved is determined by: 1.
 If `external_location` is defined, that value is used. 2. If `s3_data_dir` is
 defined, the path is determined by that and `s3_data_naming` 3. If
 `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/
-` Here all the options available for `s3_data_naming`: * `uuid`: `
+` Here all the options available for `s3_data_naming`: * `unique`: `
 {s3_data_dir}/{uuid4()}/` * `table`: `{s3_data_dir}/{table}/` * `table_unique`:
 `{s3_data_dir}/{table}/{uuid4()}/` * `schema_table`: `{s3_data_dir}/{schema}/
 {table}/` * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/
 {table}/{uuid4()}/` It's possible to set the `s3_data_naming` globally in the
 target profile, or overwrite the value in the table config, or setting up the
 value for groups of model in dbt_project.yml. > Note: when using a workgroup
 with a default output location configured, `s3_data_naming` and any configured
@@ -142,26 +135,27 @@
 can use any column of the incremental table (`src`) or the final table
 (`target`). You must prefix the column by the name of the table to prevent
 `Column is ambiguous` error. ```sql {{ config( materialized='incremental',
 table_type='iceberg', incremental_strategy='merge', unique_key='user_id',
 delete_condition="src.status != 'active' and target.my_date < now() - interval
 '2' year", format='parquet' ) }} select 'A' as user_id, 'pi' as name, 'active'
 as status, 17.89 as cost, 1 as quantity, 100000000 as quantity_big,
-current_date as my_date ``` ### High availability table materialization The
-current implementation of the table materialization can lead to downtime, as
-target table is dropped and re-created. To have the less destructive behavior
-it's possible to use `table='table_hive_ha'` materialization. **table_hive_ha**
-leverages the table versions feature of Glue catalog, creating a temp table and
-swapping the target table to the location of the temp table. This
-materialization is only available for `table_type='hive'` and requires using
-unique locations. ```sql {{ config( materialized='table_hive_ha',
-format='parquet', partition_by=['status'], s3_data_naming='table_unique' ) }}
-select 'a' as user_id, 'pi' as user_name, 'active' as status union all select
-'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default, the
-materialization keeps the last 4 table versions, you can change it by setting
+current_date as my_date ``` ### Highly available table The current
+implementation of the table materialization can lead to downtime, as target
+table is dropped and re-created. To have the less destructive behavior it's
+possible to use the `ha` config on your `table` materialized models. It
+leverages the table versions feature of glue catalog, creating a tmp table and
+swapping the target table to the location of the tmp table. This
+materialization is only available for `table_type=hive` and requires using
+unique locations. For iceberg, high availability is by default. ```sql {
+{ config( materialized='table', ha=true, format='parquet', table_type='hive',
+partition_by=['status'], s3_data_naming='table_unique' ) }} select 'a' as
+user_id, 'pi' as user_name, 'active' as status union all select 'b' as user_id,
+'sh' as user_name, 'disabled' as status ``` By default, the materialization
+keeps the last 4 table versions, you can change it by setting
 `versions_to_keep`. #### Known issues * When swapping from a table with
 partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions * By default, Glue "duplicates" the versions internally,
 so the last two versions of a table point to the same location * It's
 recommended to have `versions_to_keep` >= 4, as this will avoid having the
 older location removed * The macro `athena__end_of_time` needs to be
@@ -202,18 +196,25 @@
 way, from a dbt perspective, is to do a full-refresh of the incremental model.
 * Tables, schemas and database should only be lowercase * In order to avoid
 potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/
 dbt-athena) is not installed in the target environment. See https://github.com/
 dbt-athena/dbt-athena/issues/103 for more details. * Snapshot does not support
 dropping columns from the source table. If you drop a column make sure to drop
 the column from the snapshot as well. Another workaround is to NULL the column
-in the snapshot definition to preserve history ## Contributing See
-[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
-this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
+in the snapshot definition to preserve history ## Contracts The adapter partly
+supports contract definition. * Concerning the `data_type`, it is supported but
+needs to be adjusted for complex types. They must be specified entirely (for
+instance `array`) even though they won't be checked. Indeed, as dbt recommends,
+we only compare the broader type (array, map, int, varchar). The complete
+definition is used in order to check that the data types defined in athena are
+ok (pre-flight check). * the adapter does not support the constraints since no
+constraints don't exist in Athena. ## Contributing See [CONTRIBUTING]
+(CONTRIBUTING.md) for more information on how to contribute to this project. ##
+Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):
         [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]            [Mattia]     [Gatsby
          nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom              Mattia        Lee]
       ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð      ð§    Gatsby
                                ð ð§                                                                    Lee
                                                                                                                     ð
       [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii       [chrischin478]
        BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]       chrischin478
```

### Comparing `dbt-athena-community-1.4.5/README.md` & `dbt-athena-community-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,38 @@
+Metadata-Version: 2.1
+Name: dbt-athena-community
+Version: 1.5.0
+Summary: The athena adapter plugin for dbt (data build tool)
+Home-page: https://github.com/dbt-athena/dbt-athena
+License: Apache License 2.0
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/"><img src="https://badge.fury.io/py/dbt-athena-community.svg" /></a>
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
 
 ## Features
 
-* Supports dbt version `1.4.*`
+* Supports dbt version `1.5.*`
 * Supports [seeds][seeds]
 * Correctly detects views and their columns
 * Supports [table materialization][table]
   * [Iceberg tables][athena-iceberg] are supported **only with Athena Engine v3** and **a unique table location**
   (see table location section below)
   * Hive tables are supported by both Athena engines.
 * Supports [incremental models][incremental]
@@ -111,25 +131,29 @@
 
 
 ## Models
 
 ### Table Configuration
 
 * `external_location` (`default=none`)
-  * If set, the full S3 path in which the table will be saved. (Does not work with Iceberg table).
+  * If set, the full S3 path in which the table will be saved.
+  * Does not work with Iceberg table or Hive table with `ha` set to true.
 * `partitioned_by` (`default=none`)
   * An array list of columns by which the table will be partitioned
   * Limited to creation of 100 partitions (_currently_)
 * `bucketed_by` (`default=none`)
   * An array list of columns to bucket data, ignored if using Iceberg
 * `bucket_count` (`default=none`)
   * The number of buckets for bucketing your data, ignored if using Iceberg
 * `table_type` (`default='hive'`)
   * The type of table
   * Supports `hive` or `iceberg`
+* `ha` (`default=false`)
+  * If the table should be built using the high-availability method. This option is only available for Hive tables
+    since it is by default for Iceberg tables (see the section [below](#highly-available-table))
 * `format` (`default='parquet'`)
   * The data format for the table
   * Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE`
 * `write_compression` (`default=none`)
   * The compression type to use for any storage format that allows compression to be specified. To see which options are available, check out [CREATE TABLE AS][create-table-as]
 * `field_delimiter` (`default=none`)
   * Custom field delimiter, for when format is set to `TEXTFILE`
@@ -148,15 +172,15 @@
 The location in which a table is saved is determined by:
 
 1. If `external_location` is defined, that value is used.
 2. If `s3_data_dir` is defined, the path is determined by that and `s3_data_naming`
 3. If `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/`
 
 Here all the options available for `s3_data_naming`:
-* `uuid`: `{s3_data_dir}/{uuid4()}/`
+* `unique`: `{s3_data_dir}/{uuid4()}/`
 * `table`: `{s3_data_dir}/{table}/`
 * `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/`
 * `schema_table`: `{s3_data_dir}/{schema}/{table}/`
 * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/{table}/{uuid4()}/`
 
 It's possible to set the `s3_data_naming` globally in the target profile, or overwrite the value in the table config,
 or setting up the value for groups of model in dbt_project.yml.
@@ -243,25 +267,27 @@
 	'active' as status,
 	17.89 as cost,
 	1 as quantity,
 	100000000 as quantity_big,
 	current_date as my_date
 ```
 
-### High availability table materialization
+### Highly available table
 The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
-To have the less destructive behavior it's possible to use `table='table_hive_ha'` materialization.
-**table_hive_ha** leverages the table versions feature of Glue catalog, creating a temp table and swapping
-the target table to the location of the temp table.
-This materialization is only available for `table_type='hive'` and requires using unique locations.
+To have the less destructive behavior it's possible to use the `ha` config on your `table` materialized models.
+It leverages the table versions feature of glue catalog, creating a tmp table and swapping the target table to the
+location of the tmp table. This materialization is only available for `table_type=hive` and requires using unique
+locations. For iceberg, high availability is by default.
 
 ```sql
 {{ config(
-    materialized='table_hive_ha',
+    materialized='table',
+    ha=true,
     format='parquet',
+    table_type='hive',
     partition_by=['status'],
     s3_data_naming='table_unique'
 ) }}
 
 select
   'a' as user_id,
   'pi' as user_name,
@@ -403,14 +429,24 @@
 
 * In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not installed in the target environment.
   See https://github.com/dbt-athena/dbt-athena/issues/103 for more details.
 
 * Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
 
 
+## Contracts
+
+The adapter partly supports contract definition.
+* Concerning the `data_type`, it is supported but needs to be adjusted for complex types. They must be specified
+  entirely (for instance `array<int>`) even though they won't be checked. Indeed, as dbt recommends, we only compare
+  the broader type (array, map, int, varchar). The complete definition is used in order to check that the data types
+  defined in athena are ok (pre-flight check).
+* the adapter does not support the constraints since no constraints don't exist in Athena.
+
+
 ## Contributing
 
 See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 
 ## Contributors ✨
```

#### html2text {}

```diff
@@ -1,14 +1,25 @@
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.5.0 Summary: The
+athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
+dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
  code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
                                     month]
-## Features * Supports dbt version `1.4.*` * Supports [seeds][seeds] *
+## Features * Supports dbt version `1.5.*` * Supports [seeds][seeds] *
 Correctly detects views and their columns * Supports [table materialization]
 [table] * [Iceberg tables][athena-iceberg] are supported **only with Athena
 Engine v3** and **a unique table location** (see table location section below)
 * Hive tables are supported by both Athena engines. * Supports [incremental
 models][incremental] * On Iceberg tables : * Supports the use of `unique_key`
 only with the `merge` strategy * Supports the `append` strategy * On Hive
 tables : * Supports two incremental update strategies: `insert_overwrite` and
@@ -62,38 +73,42 @@
 profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
 s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
 your_s3_bucket/dbt/ s3_data_naming: schema_table region_name: eu-west-1 schema:
 dbt database: awsdatacatalog aws_profile_name: my-profile work_group: my-
 workgroup lf_tags: origin: dbt team: analytics ``` _Additional information_ *
 `threads` is supported * `database` and `catalog` can be used interchangeably
 ## Models ### Table Configuration * `external_location` (`default=none`) * If
-set, the full S3 path in which the table will be saved. (Does not work with
-Iceberg table). * `partitioned_by` (`default=none`) * An array list of columns
-by which the table will be partitioned * Limited to creation of 100 partitions
-(_currently_) * `bucketed_by` (`default=none`) * An array list of columns to
-bucket data, ignored if using Iceberg * `bucket_count` (`default=none`) * The
-number of buckets for bucketing your data, ignored if using Iceberg *
-`table_type` (`default='hive'`) * The type of table * Supports `hive` or
-`iceberg` * `format` (`default='parquet'`) * The data format for the table *
-Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
+set, the full S3 path in which the table will be saved. * Does not work with
+Iceberg table or Hive table with `ha` set to true. * `partitioned_by`
+(`default=none`) * An array list of columns by which the table will be
+partitioned * Limited to creation of 100 partitions (_currently_) *
+`bucketed_by` (`default=none`) * An array list of columns to bucket data,
+ignored if using Iceberg * `bucket_count` (`default=none`) * The number of
+buckets for bucketing your data, ignored if using Iceberg * `table_type`
+(`default='hive'`) * The type of table * Supports `hive` or `iceberg` * `ha`
+(`default=false`) * If the table should be built using the high-availability
+method. This option is only available for Hive tables since it is by default
+for Iceberg tables (see the section [below](#highly-available-table)) *
+`format` (`default='parquet'`) * The data format for the table * Supports
+`ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
 (`default=none`) * The compression type to use for any storage format that
 allows compression to be specified. To see which options are available, check
 out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
 Custom field delimiter, for when format is set to `TEXTFILE` *
 `table_properties`: table properties to add to the table, valid for Iceberg
 only * `lf_tags` (`default=none`) * lf tags to associate with the table *
 format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
 (`default=none`) * lf tags to associate with the table columns * format: `
 {"tag1": {"value1": ["column1": "column2"]}}` [create-table-as]: https://
 docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 ### Table location The location in which a table is saved is determined by: 1.
 If `external_location` is defined, that value is used. 2. If `s3_data_dir` is
 defined, the path is determined by that and `s3_data_naming` 3. If
 `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/
-` Here all the options available for `s3_data_naming`: * `uuid`: `
+` Here all the options available for `s3_data_naming`: * `unique`: `
 {s3_data_dir}/{uuid4()}/` * `table`: `{s3_data_dir}/{table}/` * `table_unique`:
 `{s3_data_dir}/{table}/{uuid4()}/` * `schema_table`: `{s3_data_dir}/{schema}/
 {table}/` * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/
 {table}/{uuid4()}/` It's possible to set the `s3_data_naming` globally in the
 target profile, or overwrite the value in the table config, or setting up the
 value for groups of model in dbt_project.yml. > Note: when using a workgroup
 with a default output location configured, `s3_data_naming` and any configured
@@ -131,26 +146,27 @@
 can use any column of the incremental table (`src`) or the final table
 (`target`). You must prefix the column by the name of the table to prevent
 `Column is ambiguous` error. ```sql {{ config( materialized='incremental',
 table_type='iceberg', incremental_strategy='merge', unique_key='user_id',
 delete_condition="src.status != 'active' and target.my_date < now() - interval
 '2' year", format='parquet' ) }} select 'A' as user_id, 'pi' as name, 'active'
 as status, 17.89 as cost, 1 as quantity, 100000000 as quantity_big,
-current_date as my_date ``` ### High availability table materialization The
-current implementation of the table materialization can lead to downtime, as
-target table is dropped and re-created. To have the less destructive behavior
-it's possible to use `table='table_hive_ha'` materialization. **table_hive_ha**
-leverages the table versions feature of Glue catalog, creating a temp table and
-swapping the target table to the location of the temp table. This
-materialization is only available for `table_type='hive'` and requires using
-unique locations. ```sql {{ config( materialized='table_hive_ha',
-format='parquet', partition_by=['status'], s3_data_naming='table_unique' ) }}
-select 'a' as user_id, 'pi' as user_name, 'active' as status union all select
-'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default, the
-materialization keeps the last 4 table versions, you can change it by setting
+current_date as my_date ``` ### Highly available table The current
+implementation of the table materialization can lead to downtime, as target
+table is dropped and re-created. To have the less destructive behavior it's
+possible to use the `ha` config on your `table` materialized models. It
+leverages the table versions feature of glue catalog, creating a tmp table and
+swapping the target table to the location of the tmp table. This
+materialization is only available for `table_type=hive` and requires using
+unique locations. For iceberg, high availability is by default. ```sql {
+{ config( materialized='table', ha=true, format='parquet', table_type='hive',
+partition_by=['status'], s3_data_naming='table_unique' ) }} select 'a' as
+user_id, 'pi' as user_name, 'active' as status union all select 'b' as user_id,
+'sh' as user_name, 'disabled' as status ``` By default, the materialization
+keeps the last 4 table versions, you can change it by setting
 `versions_to_keep`. #### Known issues * When swapping from a table with
 partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions * By default, Glue "duplicates" the versions internally,
 so the last two versions of a table point to the same location * It's
 recommended to have `versions_to_keep` >= 4, as this will avoid having the
 older location removed * The macro `athena__end_of_time` needs to be
@@ -191,18 +207,25 @@
 way, from a dbt perspective, is to do a full-refresh of the incremental model.
 * Tables, schemas and database should only be lowercase * In order to avoid
 potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/
 dbt-athena) is not installed in the target environment. See https://github.com/
 dbt-athena/dbt-athena/issues/103 for more details. * Snapshot does not support
 dropping columns from the source table. If you drop a column make sure to drop
 the column from the snapshot as well. Another workaround is to NULL the column
-in the snapshot definition to preserve history ## Contributing See
-[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
-this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
+in the snapshot definition to preserve history ## Contracts The adapter partly
+supports contract definition. * Concerning the `data_type`, it is supported but
+needs to be adjusted for complex types. They must be specified entirely (for
+instance `array`) even though they won't be checked. Indeed, as dbt recommends,
+we only compare the broader type (array, map, int, varchar). The complete
+definition is used in order to check that the data types defined in athena are
+ok (pre-flight check). * the adapter does not support the constraints since no
+constraints don't exist in Athena. ## Contributing See [CONTRIBUTING]
+(CONTRIBUTING.md) for more information on how to contribute to this project. ##
+Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):
         [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]            [Mattia]     [Gatsby
          nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom              Mattia        Lee]
       ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð      ð§    Gatsby
                                ð ð§                                                                    Lee
                                                                                                                     ð
       [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii       [chrischin478]
        BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]       chrischin478
```

### Comparing `dbt-athena-community-1.4.5/dbt/adapters/athena/__init__.py` & `dbt-athena-community-1.5.0/dbt/adapters/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/adapters/athena/column.py` & `dbt-athena-community-1.5.0/dbt/adapters/athena/column.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/adapters/athena/connections.py` & `dbt-athena-community-1.5.0/dbt/adapters/athena/connections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import hashlib
 from concurrent.futures.thread import ThreadPoolExecutor
 from contextlib import contextmanager
 from copy import deepcopy
 from dataclasses import dataclass
 from decimal import Decimal
-from typing import Any, ContextManager, Dict, List, Optional, Tuple
+from typing import Any, ContextManager, Dict, List, Optional, Tuple, Union
 
 import tenacity
 from pyathena.connection import Connection as AthenaConnection
 from pyathena.cursor import Cursor
 from pyathena.error import OperationalError, ProgrammingError
 
 # noinspection PyProtectedMember
@@ -53,15 +54,15 @@
 
     @property
     def type(self) -> str:
         return "athena"
 
     @property
     def unique_field(self):
-        return self.host
+        return f"athena-{hashlib.md5(self.s3_staging_dir.encode()).hexdigest()}"
 
     def _connection_keys(self) -> Tuple[str, ...]:
         return (
             "s3_staging_dir",
             "work_group",
             "region_name",
             "database",
@@ -97,14 +98,15 @@
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         endpoint_url: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
+        **kwargs,
     ):
         def inner():
             query_id = self._execute(
                 operation,
                 parameters=parameters,
                 work_group=work_group,
                 s3_staging_dir=s3_staging_dir,
@@ -137,14 +139,24 @@
         )
         return retry(inner)
 
 
 class AthenaConnectionManager(SQLConnectionManager):
     TYPE = "athena"
 
+    @classmethod
+    def data_type_code_to_name(cls, type_code: Union[int, str]) -> str:
+        """
+        Get the string representation of the data type from the Athena metadata. Dbt performs a
+        query to retrieve the types of the columns in the SQL query. Then these types are compared
+        to the types in the contract config, simplified because they need to match what is returned
+        by Athena metadata (we are only interested in the broader type, without subtypes nor granularity).
+        """
+        return type_code.split("(")[0].split("<")[0].upper()
+
     @contextmanager
     def exception_handler(self, sql: str) -> ContextManager:
         try:
             yield
         except Exception as e:
             logger.debug(f"Error running SQL: {sql}")
             raise DbtRuntimeError(str(e)) from e
```

### Comparing `dbt-athena-community-1.4.5/dbt/adapters/athena/impl.py` & `dbt-athena-community-1.5.0/dbt/adapters/athena/impl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 import csv
 import os
 import posixpath as path
 import tempfile
 from itertools import chain
+from textwrap import dedent
 from threading import Lock
-from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union
+from typing import Any, Dict, Iterator, List, Optional, Set, Tuple
 from urllib.parse import urlparse
 from uuid import uuid4
 
 import agate
 from botocore.exceptions import ClientError
 from mypy_boto3_athena.type_defs import DataCatalogTypeDef
 
 from dbt.adapters.athena import AthenaConnectionManager
 from dbt.adapters.athena.column import AthenaColumn
 from dbt.adapters.athena.config import get_boto3_config
+from dbt.adapters.athena.constants import LOGGER
+from dbt.adapters.athena.exceptions import (
+    S3LocationException,
+    SnapshotMigrationRequired,
+)
 from dbt.adapters.athena.relation import (
+    RELATION_TYPE_MAP,
     AthenaRelation,
     AthenaSchemaSearchMap,
-    TableType,
+    get_table_type,
 )
+from dbt.adapters.athena.s3 import S3DataNaming
 from dbt.adapters.athena.utils import clean_sql_comment, get_catalog_id
-from dbt.adapters.base import available
+from dbt.adapters.base import ConstraintSupport, available
 from dbt.adapters.base.relation import BaseRelation, InformationSchema
 from dbt.adapters.sql import SQLAdapter
 from dbt.contracts.graph.manifest import Manifest
-from dbt.contracts.graph.nodes import CompiledNode
-from dbt.events import AdapterLogger
+from dbt.contracts.graph.nodes import CompiledNode, ConstraintType
 from dbt.exceptions import DbtRuntimeError
 
-logger = AdapterLogger("Athena")
-
 boto3_client_lock = Lock()
 
 
 class AthenaAdapter(SQLAdapter):
     ConnectionManager = AthenaConnectionManager
     Relation = AthenaRelation
 
-    relation_type_map = {
-        "EXTERNAL_TABLE": TableType.TABLE,
-        "MANAGED_TABLE": TableType.TABLE,
-        "VIRTUAL_VIEW": TableType.VIEW,
-        "table": TableType.TABLE,
-        "view": TableType.VIEW,
-        "cte": TableType.CTE,
-        "materializedview": TableType.MATERIALIZED_VIEW,
+    # There is no such concept as constraints in Athena
+    CONSTRAINT_SUPPORT = {
+        ConstraintType.check: ConstraintSupport.NOT_SUPPORTED,
+        ConstraintType.not_null: ConstraintSupport.NOT_SUPPORTED,
+        ConstraintType.unique: ConstraintSupport.NOT_SUPPORTED,
+        ConstraintType.primary_key: ConstraintSupport.NOT_SUPPORTED,
+        ConstraintType.foreign_key: ConstraintSupport.NOT_SUPPORTED,
     }
 
     @classmethod
     def date_function(cls) -> str:
         return "now()"
 
     @classmethod
@@ -79,15 +83,15 @@
         columns_appendix = f" for columns {columns}" if columns else ""
         msg_appendix = tbl_appendix + columns_appendix
         if failures:
             base_msg = f"Failed to add LF tags: {lf_tags} to {database}" + msg_appendix
             for failure in failures:
                 tag = failure.get("LFTag", {}).get("TagKey")
                 error = failure.get("Error", {}).get("ErrorMessage")
-                logger.error(f"Failed to set {tag} for {database}" + msg_appendix + f" - {error}")
+                LOGGER.error(f"Failed to set {tag} for {database}" + msg_appendix + f" - {error}")
             raise DbtRuntimeError(base_msg)
         return f"Added LF tags: {lf_tags} to {database}" + msg_appendix
 
     @classmethod
     def lf_tags_columns_is_valid(cls, lf_tags_columns: Dict[str, Dict[str, List[str]]]) -> Optional[bool]:
         if not lf_tags_columns:
             return False
@@ -112,41 +116,41 @@
     ):
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         lf_tags = lf_tags or conn.credentials.lf_tags
 
         if not lf_tags and not lf_tags_columns:
-            logger.debug("No LF tags configured")
+            LOGGER.debug("No LF tags configured")
         else:
             with boto3_client_lock:
                 lf_client = client.session.client(
                     "lakeformation", region_name=client.region_name, config=get_boto3_config()
                 )
 
             if lf_tags:
                 resource = {"Database": {"Name": database}}
                 if table:
                     resource = {"Table": {"DatabaseName": database, "Name": table}}
 
                 response = lf_client.add_lf_tags_to_resource(
                     Resource=resource, LFTags=[{"TagKey": key, "TagValues": [value]} for key, value in lf_tags.items()]
                 )
-                logger.debug(self.parse_lf_response(response, database, table, None, lf_tags))
+                LOGGER.debug(self.parse_lf_response(response, database, table, None, lf_tags))
 
             if self.lf_tags_columns_is_valid(lf_tags_columns):
                 for tag_key, tag_config in lf_tags_columns.items():
                     for tag_value, columns in tag_config.items():
                         response = lf_client.add_lf_tags_to_resource(
                             Resource={
                                 "TableWithColumns": {"DatabaseName": database, "Name": table, "ColumnNames": columns}
                             },
                             LFTags=[{"TagKey": tag_key, "TagValues": [tag_value]}],
                         )
-                        logger.debug(self.parse_lf_response(response, database, table, columns, {tag_key: tag_value}))
+                        LOGGER.debug(self.parse_lf_response(response, database, table, columns, {tag_key: tag_value}))
 
     @available
     def is_work_group_output_location_enforced(self) -> bool:
         conn = self.connections.get_thread_connection()
         creds = conn.credentials
         client = conn.handle
 
@@ -166,137 +170,154 @@
                 work_group.get("WorkGroup", {}).get("Configuration", {}).get("EnforceWorkGroupConfiguration", False)
             )
 
             return output_location is not None and output_location_enforced
         else:
             return False
 
-    @available
-    def s3_table_prefix(self, s3_data_dir: Optional[str]) -> str:
+    def _s3_table_prefix(self, s3_data_dir: Optional[str]) -> str:
         """
         Returns the root location for storing tables in S3.
-        This is `s3_data_dir`, if set, and `s3_staging_dir/tables/` if not.
+        This is `s3_data_dir`, if set at the model level, the s3_data_dir of the connection if provided,
+        and `s3_staging_dir/tables/` if nothing provided as data dir.
         We generate a value here even if `s3_data_dir` is not set,
         since creating a seed table requires a non-default location.
         """
         conn = self.connections.get_thread_connection()
         creds = conn.credentials
         if s3_data_dir is not None:
             return s3_data_dir
-        else:
-            return path.join(creds.s3_staging_dir, "tables")
+
+        return path.join(creds.s3_staging_dir, "tables")
+
+    def _s3_data_naming(self, s3_data_naming: Optional[str]) -> Optional[S3DataNaming]:
+        """
+        Returns the s3 data naming strategy if provided, otherwise the value from the connection.
+        """
+        conn = self.connections.get_thread_connection()
+        creds = conn.credentials
+        if s3_data_naming is not None:
+            return S3DataNaming(s3_data_naming)
+
+        return S3DataNaming(creds.s3_data_naming) or S3DataNaming.TABLE_UNIQUE
 
     @available
-    def s3_table_location(
+    def generate_s3_location(
         self,
-        s3_data_dir: Optional[str],
-        s3_data_naming: str,
-        schema_name: str,
-        table_name: str,
-        s3_path_table_part: Optional[str] = None,
+        relation: AthenaRelation,
+        s3_data_dir: Optional[str] = None,
+        s3_data_naming: Optional[str] = None,
         external_location: Optional[str] = None,
         is_temporary_table: bool = False,
     ) -> str:
         """
         Returns either a UUID or database/table prefix for storing a table,
         depending on the value of s3_table
         """
         if external_location and not is_temporary_table:
             return external_location.rstrip("/")
 
-        if not s3_path_table_part:
-            s3_path_table_part = table_name
+        s3_path_table_part = relation.s3_path_table_part or relation.identifier
+        schema_name = relation.schema
+        s3_data_naming = self._s3_data_naming(s3_data_naming)
+        table_prefix = self._s3_table_prefix(s3_data_dir)
 
         mapping = {
-            "uuid": path.join(self.s3_table_prefix(s3_data_dir), str(uuid4())),
-            "table": path.join(self.s3_table_prefix(s3_data_dir), s3_path_table_part),
-            "table_unique": path.join(self.s3_table_prefix(s3_data_dir), s3_path_table_part, str(uuid4())),
-            "schema_table": path.join(self.s3_table_prefix(s3_data_dir), schema_name, s3_path_table_part),
-            "schema_table_unique": path.join(
-                self.s3_table_prefix(s3_data_dir), schema_name, s3_path_table_part, str(uuid4())
-            ),
+            S3DataNaming.UNIQUE: path.join(table_prefix, str(uuid4())),
+            S3DataNaming.TABLE: path.join(table_prefix, s3_path_table_part),
+            S3DataNaming.TABLE_UNIQUE: path.join(table_prefix, s3_path_table_part, str(uuid4())),
+            S3DataNaming.SCHEMA_TABLE: path.join(table_prefix, schema_name, s3_path_table_part),
+            S3DataNaming.SCHEMA_TABLE_UNIQUE: path.join(table_prefix, schema_name, s3_path_table_part, str(uuid4())),
         }
-        table_location = mapping.get(s3_data_naming)
-
-        if table_location is None:
-            raise ValueError(f"Unknown value for s3_data_naming: {s3_data_naming}")
 
-        return table_location
+        return mapping[s3_data_naming]
 
     @available
-    def get_table_location(self, database_name: str, table_name: str) -> Union[str, None]:
+    def get_glue_table_location(self, relation: AthenaRelation) -> Optional[str]:
         """
-        Helper function to S3 get table location
+        Helper function to get location of a relation in S3.
+        Will return None if the table does not exist or does not have a location (views)
         """
         conn = self.connections.get_thread_connection()
         client = conn.handle
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
+
         try:
-            table = glue_client.get_table(DatabaseName=database_name, Name=table_name)
-            table_location = table["Table"]["StorageDescriptor"]["Location"]
-            logger.debug(f"{database_name}.{table_name} is stored in {table_location}")
-            return table_location
+            table = glue_client.get_table(DatabaseName=relation.schema, Name=relation.identifier)
         except ClientError as e:
             if e.response["Error"]["Code"] == "EntityNotFoundException":
-                logger.debug(f"Table '{table_name}' does not exists - Ignoring")
-                return
+                LOGGER.debug(f"Table {relation.render()} does not exists - Ignoring")
+                return None
+            raise e
+
+        table_type = get_table_type(table["Table"])
+        table_location = table["Table"].get("StorageDescriptor", {}).get("Location")
+        if table_type.is_physical():
+            if not table_location:
+                raise S3LocationException(
+                    f"Relation {relation.render()} is of type '{table_type.value}' which requires a location, "
+                    f"but no location returned by Glue."
+                )
+            LOGGER.debug(f"{relation.render()} is stored in {table_location}")
+            return table_location
+
+        return None
 
     @available
-    def clean_up_partitions(self, database_name: str, table_name: str, where_condition: str):
+    def clean_up_partitions(self, relation: AthenaRelation, where_condition: str):
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
         paginator = glue_client.get_paginator("get_partitions")
         partition_params = {
-            "DatabaseName": database_name,
-            "TableName": table_name,
+            "DatabaseName": relation.schema,
+            "TableName": relation.identifier,
             "Expression": where_condition,
             "ExcludeColumnSchema": True,
         }
         partition_pg = paginator.paginate(**partition_params)
         partitions = partition_pg.build_full_result().get("Partitions")
         for partition in partitions:
             self.delete_from_s3(partition["StorageDescriptor"]["Location"])
 
     @available
-    def clean_up_table(self, database_name: str, table_name: str):
-        table_location = self.get_table_location(database_name, table_name)
+    def clean_up_table(self, relation: AthenaRelation):
+        table_location = self.get_glue_table_location(relation)
 
         # this check avoid issues for when the table location is an empty string
         # or when the table do not exist and table location is None
         if table_location:
             self.delete_from_s3(table_location)
 
     @available
     def quote_seed_column(self, column: str, quote_config: Optional[bool]) -> str:
         return super().quote_seed_column(column, False)
 
     @available
     def upload_seed_to_s3(
         self,
-        s3_data_dir: Optional[str],
-        s3_data_naming: Optional[str],
-        external_location: Optional[str],
-        database_name: str,
-        table_name: str,
+        relation: AthenaRelation,
         table: agate.Table,
+        s3_data_dir: Optional[str] = None,
+        s3_data_naming: Optional[str] = None,
+        external_location: Optional[str] = None,
     ) -> str:
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         # TODO: consider using the workgroup default location when configured
-        s3_location = self.s3_table_location(
-            s3_data_dir, s3_data_naming, database_name, table_name, external_location=external_location
+        s3_location = self.generate_s3_location(
+            relation, s3_data_dir, s3_data_naming, external_location=external_location
         )
         bucket, prefix = self._parse_s3_path(s3_location)
 
-        file_name = f"{table_name}.csv"
+        file_name = f"{relation.identifier}.csv"
         object_name = path.join(prefix, file_name)
 
         with boto3_client_lock:
             s3_client = client.session.client("s3", region_name=client.region_name, config=get_boto3_config())
             # This ensures cross-platform support, tempfile.NamedTemporaryFile does not
             tmpfile = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
             table.to_csv(tmpfile, quoting=csv.QUOTE_NONNUMERIC)
@@ -314,32 +335,32 @@
         """
         conn = self.connections.get_thread_connection()
         client = conn.handle
         bucket_name, prefix = self._parse_s3_path(s3_path)
         if self._s3_path_exists(bucket_name, prefix):
             s3_resource = client.session.resource("s3", region_name=client.region_name, config=get_boto3_config())
             s3_bucket = s3_resource.Bucket(bucket_name)
-            logger.debug(f"Deleting table data: path='{s3_path}', bucket='{bucket_name}', prefix='{prefix}'")
+            LOGGER.debug(f"Deleting table data: path='{s3_path}', bucket='{bucket_name}', prefix='{prefix}'")
             response = s3_bucket.objects.filter(Prefix=prefix).delete()
             is_all_successful = True
             for res in response:
                 if "Errors" in res:
                     for err in res["Errors"]:
                         is_all_successful = False
-                        logger.error(
+                        LOGGER.error(
                             "Failed to delete files: Key='{}', Code='{}', Message='{}', s3_bucket='{}'",
                             err["Key"],
                             err["Code"],
                             err["Message"],
                             bucket_name,
                         )
             if is_all_successful is False:
                 raise DbtRuntimeError("Failed to delete files from S3.")
         else:
-            logger.debug("S3 path does not exist")
+            LOGGER.debug("S3 path does not exist")
 
     @staticmethod
     def _parse_s3_path(s3_path: str) -> Tuple[str, str]:
         """
         Parses and splits a s3 path into bucket name and prefix.
         This assumes that s3_path is a prefix instead of a URI. It adds a
         trailing slash to the prefix, if there is none.
@@ -382,15 +403,15 @@
         )
 
     def _get_one_table_for_catalog(self, table: dict, database: str) -> list:
         table_catalog = {
             "table_database": database,
             "table_schema": table["DatabaseName"],
             "table_name": table["Name"],
-            "table_type": self.relation_type_map[table.get("TableType", "EXTERNAL_TABLE")].value,
+            "table_type": RELATION_TYPE_MAP[table.get("TableType", "EXTERNAL_TABLE")].value,
             "table_comment": table.get("Parameters", {}).get("comment", table.get("Description", "")),
         }
         return [
             {
                 **table_catalog,
                 **{
                     "column_name": col["Name"],
@@ -485,15 +506,15 @@
         quote_policy = {"database": True, "schema": True, "identifier": True}
 
         try:
             for page in page_iterator:
                 tables = page["TableList"]
                 for table in tables:
                     if "TableType" not in table:
-                        logger.debug(f"Table '{table['Name']}' has no TableType attribute - Ignoring")
+                        LOGGER.debug(f"Table '{table['Name']}' has no TableType attribute - Ignoring")
                         continue
                     _type = table["TableType"]
                     if _type == "VIRTUAL_VIEW":
                         _type = self.Relation.View
                     else:
                         _type = self.Relation.Table
 
@@ -505,146 +526,117 @@
                             quote_policy=quote_policy,
                             type=_type,
                         )
                     )
         except ClientError as e:
             # don't error out when schema doesn't exist
             # this allows dbt to create and manage schemas/databases
-            logger.debug(f"Schema '{schema_relation.schema}' does not exist - Ignoring: {e}")
+            LOGGER.debug(f"Schema '{schema_relation.schema}' does not exist - Ignoring: {e}")
 
         return relations
 
     @available
-    def get_table_type(self, db_name, table_name) -> TableType:
-        conn = self.connections.get_thread_connection()
-        client = conn.handle
-
-        with boto3_client_lock:
-            glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
-
-        try:
-            response = glue_client.get_table(DatabaseName=db_name, Name=table_name)
-            _type = self.relation_type_map.get(response.get("Table", {}).get("TableType"))
-            _specific_type = response.get("Table", {}).get("Parameters", {}).get("table_type", "")
-
-            if _specific_type.lower() == "iceberg":
-                _type = TableType.ICEBERG
-
-            if _type is None:
-                raise ValueError("Table type cannot be None")
-
-            logger.debug(f"table_name : {table_name}")
-            logger.debug(f"table type : {_type}")
-
-            return _type
-
-        except glue_client.exceptions.EntityNotFoundException as e:
-            logger.debug(f"Error calling Glue get_table: {e}")
-
-    @available
-    def swap_table(self, src_database: str, src_table_name: str, target_database: str, target_table_name: str):
+    def swap_table(self, src_relation: AthenaRelation, target_relation: AthenaRelation):
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
-        src_table = glue_client.get_table(DatabaseName=src_database, Name=src_table_name).get("Table")
-        src_table_partitions = glue_client.get_partitions(DatabaseName=src_database, TableName=src_table_name).get(
-            "Partitions"
-        )
+        src_table = glue_client.get_table(DatabaseName=src_relation.schema, Name=src_relation.identifier).get("Table")
+        src_table_partitions = glue_client.get_partitions(
+            DatabaseName=src_relation.schema, TableName=src_relation.identifier
+        ).get("Partitions")
 
         target_table_partitions = glue_client.get_partitions(
-            DatabaseName=target_database, TableName=target_table_name
+            DatabaseName=target_relation.schema, TableName=target_relation.identifier
         ).get("Partitions")
 
         target_table_version = {
-            "Name": target_table_name,
+            "Name": target_relation.identifier,
             "StorageDescriptor": src_table["StorageDescriptor"],
             "PartitionKeys": src_table["PartitionKeys"],
             "TableType": src_table["TableType"],
             "Parameters": src_table["Parameters"],
             "Description": src_table.get("Description", ""),
         }
 
         # perform a table swap
-        glue_client.update_table(DatabaseName=target_database, TableInput=target_table_version)
-        logger.debug(
-            f"Table {target_database}.{target_table_name} swapped with the content of {src_database}.{src_table}"
-        )
+        glue_client.update_table(DatabaseName=target_relation.schema, TableInput=target_table_version)
+        LOGGER.debug(f"Table {target_relation.render()} swapped with the content of {src_relation.render()}")
 
         # we delete the target table partitions in any case
         # if source table has partitions we need to delete and add partitions
         # it source table hasn't any partitions we need to delete target table partitions
         if target_table_partitions:
             glue_client.batch_delete_partition(
-                DatabaseName=target_database,
-                TableName=target_table_name,
+                DatabaseName=target_relation.schema,
+                TableName=target_relation.identifier,
                 PartitionsToDelete=[{"Values": i["Values"]} for i in target_table_partitions],
             )
 
         if src_table_partitions:
             glue_client.batch_create_partition(
-                DatabaseName=target_database,
-                TableName=target_table_name,
+                DatabaseName=target_relation.schema,
+                TableName=target_relation.identifier,
                 PartitionInputList=[
                     {"Values": p["Values"], "StorageDescriptor": p["StorageDescriptor"], "Parameters": p["Parameters"]}
                     for p in src_table_partitions
                 ],
             )
 
-    def _get_glue_table_versions_to_expire(self, database_name: str, table_name: str, to_keep: int):
+    def _get_glue_table_versions_to_expire(self, relation: AthenaRelation, to_keep: int):
         """
         Given a table and the amount of its version to keep, it returns the versions to delete
         """
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
         paginator = glue_client.get_paginator("get_table_versions")
         response_iterator = paginator.paginate(
             **{
-                "DatabaseName": database_name,
-                "TableName": table_name,
+                "DatabaseName": relation.schema,
+                "TableName": relation.identifier,
             }
         )
         table_versions = response_iterator.build_full_result().get("TableVersions")
-        logger.debug(f"Total table versions: {[v['VersionId'] for v in table_versions]}")
+        LOGGER.debug(f"Total table versions: {[v['VersionId'] for v in table_versions]}")
         table_versions_ordered = sorted(table_versions, key=lambda i: int(i["Table"]["VersionId"]), reverse=True)
         return table_versions_ordered[int(to_keep) :]
 
     @available
-    def expire_glue_table_versions(self, database_name: str, table_name: str, to_keep: int, delete_s3: bool):
+    def expire_glue_table_versions(self, relation: AthenaRelation, to_keep: int, delete_s3: bool):
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
-        versions_to_delete = self._get_glue_table_versions_to_expire(database_name, table_name, to_keep)
-        logger.debug(f"Versions to delete: {[v['VersionId'] for v in versions_to_delete]}")
+        versions_to_delete = self._get_glue_table_versions_to_expire(relation, to_keep)
+        LOGGER.debug(f"Versions to delete: {[v['VersionId'] for v in versions_to_delete]}")
 
         deleted_versions = []
         for v in versions_to_delete:
             version = v["Table"]["VersionId"]
             location = v["Table"]["StorageDescriptor"]["Location"]
             try:
                 glue_client.delete_table_version(
-                    DatabaseName=database_name, TableName=table_name, VersionId=str(version)
+                    DatabaseName=relation.schema, TableName=relation.identifier, VersionId=str(version)
                 )
                 deleted_versions.append(version)
-                logger.debug(f"Deleted version {version} of table {database_name}.{table_name} ")
+                LOGGER.debug(f"Deleted version {version} of table {relation.render()} ")
                 if delete_s3:
                     self.delete_from_s3(location)
             except Exception as err:
-                logger.debug(f"There was an error when expiring table version {version} with error: {err}")
+                LOGGER.debug(f"There was an error when expiring table version {version} with error: {err}")
 
-            logger.debug(f"{location} was deleted")
+            LOGGER.debug(f"{location} was deleted")
 
         return deleted_versions
 
     @available
     def persist_docs_to_glue(
         self,
         relation: AthenaRelation,
@@ -712,25 +704,26 @@
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
         try:
             table = glue_client.get_table(DatabaseName=relation.schema, Name=relation.identifier)["Table"]
         except ClientError as e:
             if e.response["Error"]["Code"] == "EntityNotFoundException":
-                logger.debug("table not exist, catching the error")
+                LOGGER.debug("table not exist, catching the error")
                 return []
             else:
-                logger.error(e)
+                LOGGER.error(e)
                 raise e
-        table_type = self.get_table_type(relation.schema, relation.identifier)
+
+        table_type = get_table_type(table)
 
         columns = [c for c in table["StorageDescriptor"]["Columns"] if self._is_current_column(c)]
         partition_keys = table.get("PartitionKeys", [])
 
-        logger.debug(f"Columns in relation {relation.identifier}: {columns + partition_keys}")
+        LOGGER.debug(f"Columns in relation {relation.identifier}: {columns + partition_keys}")
 
         return [
             AthenaColumn(column=c["Name"], dtype=c["Type"], table_type=table_type) for c in columns + partition_keys
         ]
 
     @available
     def delete_from_glue_catalog(self, relation: AthenaRelation):
@@ -741,14 +734,101 @@
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
         try:
             glue_client.delete_table(DatabaseName=schema_name, Name=table_name)
-            logger.debug(f"Deleted table from glue catalog: {relation.render()}")
+            LOGGER.debug(f"Deleted table from glue catalog: {relation.render()}")
         except ClientError as e:
             if e.response["Error"]["Code"] == "EntityNotFoundException":
-                logger.debug(f"Table {relation.render()} does not exist and will not be deleted, ignoring")
+                LOGGER.debug(f"Table {relation.render()} does not exist and will not be deleted, ignoring")
             else:
-                logger.error(e)
+                LOGGER.error(e)
                 raise e
+
+    @available.parse_none
+    def valid_snapshot_target(self, relation: BaseRelation) -> None:
+        """Log an error to help developers migrate to the new snapshot logic"""
+        super().valid_snapshot_target(relation)
+        columns = self.get_columns_in_relation(relation)
+        names = {c.name.lower() for c in columns}
+
+        table_columns = [col for col in names if not col.startswith("dbt_") and col != "is_current_record"]
+
+        if "dbt_unique_key" in names:
+            sql = self._generate_snapshot_migration_sql(relation=relation, table_columns=table_columns)
+            msg = (
+                f"{'!'*90}\n"
+                "The snapshot logic of dbt-athena has changed in an incompatible way to be more consistent "
+                "with the dbt-core implementation.\nYou will need to migrate your existing snapshot tables to be "
+                "able to keep using them with the latest dbt-athena version.\nYou can find more information "
+                "in the release notes:\nhttps://github.com/dbt-athena/dbt-athena/releases\n"
+                f"{'!'*90}\n\n"
+                "You can use the example query below as a baseline to perform the migration:\n\n"
+                f"{'-'*90}\n"
+                f"{sql}\n"
+                f"{'-'*90}\n\n"
+            )
+            LOGGER.error(msg)
+            raise SnapshotMigrationRequired("Look into 1.5 dbt-athena docs for the complete migration procedure")
+
+    def _generate_snapshot_migration_sql(self, relation: AthenaRelation, table_columns: List[str]) -> str:
+        """Generate a sequence of queries that can be used to migrate the existing table to the new format.
+
+        The queries perform the following steps:
+        - Backup the existing table
+        - Make the necessary modifications and store the results in a staging table
+        - Delete the target table (users might have to delete the S3 files manually)
+        - Copy the content of the staging table to the final table
+        - Delete the staging table
+        """
+        col_csv = f",\n{' '*16}".join(table_columns)
+        staging_relation = relation.incorporate(
+            path={"identifier": relation.identifier + "__dbt_tmp_migration_staging"}
+        )
+        ctas = dedent(
+            f"""\
+            select
+                {col_csv},
+                dbt_snapshot_at as dbt_updated_at,
+                dbt_valid_from,
+                if(dbt_valid_to > cast('9000-01-01' as timestamp), null, dbt_valid_to) as dbt_valid_to,
+                dbt_scd_id
+            from {relation}
+            where dbt_change_type != 'delete'
+            ;
+            """
+        )
+        staging_sql = self.execute_macro(
+            "create_table_as", kwargs=dict(temporary=True, relation=staging_relation, compiled_code=ctas)
+        )
+
+        backup_relation = relation.incorporate(path={"identifier": relation.identifier + "__dbt_tmp_migration_backup"})
+        backup_sql = self.execute_macro(
+            "create_table_as",
+            kwargs=dict(temporary=True, relation=backup_relation, compiled_code=f"select * from {relation};"),
+        )
+
+        drop_target_sql = f"drop table {relation.render_hive()};"
+
+        copy_to_target_sql = self.execute_macro(
+            "create_table_as", kwargs=dict(relation=relation, compiled_code=f"select * from {staging_relation};")
+        )
+
+        drop_staging_sql = f"drop table {staging_relation.render_hive()};"
+
+        return "\n".join(
+            [
+                "-- Backup original table",
+                backup_sql.strip(),
+                "\n\n-- Store new results in staging table",
+                staging_sql.strip(),
+                "\n\n-- Drop target table\n"
+                "-- Note: you will need to manually remove the S3 files if you have a static table location\n",
+                drop_target_sql.strip(),
+                "\n\n-- Copy staging to target",
+                copy_to_target_sql.strip(),
+                "\n\n-- Drop staging table",
+                drop_staging_sql.strip(),
+            ]
+        )
```

### Comparing `dbt-athena-community-1.4.5/dbt/adapters/athena/query_headers.py` & `dbt-athena-community-1.5.0/dbt/adapters/athena/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/persist_docs.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/relation.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/relation.sql`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 {% macro athena__drop_relation(relation) -%}
-  {% set rel_type_object = adapter.get_table_type(relation.schema, relation.identifier) %}
-  {%- if rel_type_object is not none %}
-    {% set rel_type = rel_type_object.value %}
-    {%- if rel_type == 'table' or rel_type == 'iceberg_table' %}
-      {%- do adapter.clean_up_table(relation.schema, relation.identifier) -%}
-    {%- endif %}
-    {%- do adapter.delete_from_glue_catalog(relation) -%}
-  {%- endif %}
+  {%- do adapter.clean_up_table(relation) -%}
+  {%- do adapter.delete_from_glue_catalog(relation) -%}
 {% endmacro %}
 
 {% macro set_table_classification(relation) -%}
   {%- set format = config.get('format', default='parquet') -%}
   {% call statement('set_table_classification', auto_begin=False) -%}
     alter table {{ relation.render_hive() }} set tblproperties ('classification' = '{{ format }}')
   {%- endcall %}
```

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/helpers.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/helpers.sql`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
       {%- endif -%}
       {%- do single_partition.append(partitioned_by[loop.index0] + '=' + value) -%}
     {%- endfor -%}
     {%- set single_partition_expression = single_partition | join(' and ') -%}
     {%- do partitions.append('(' + single_partition_expression + ')') -%}
   {%- endfor -%}
   {%- for i in range(partitions | length) %}
-    {%- do adapter.clean_up_partitions(target_relation.schema, target_relation.table, partitions[i]) -%}
+    {%- do adapter.clean_up_partitions(target_relation, partitions[i]) -%}
   {%- endfor -%}
 {%- endmacro %}
 
 {% macro remove_partitions_from_columns(columns_with_partitions, partition_keys) %}
   {%- set columns = [] -%}
   {%- for column in columns_with_partitions -%}
     {%- if column.name not in partition_keys -%}
```

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/incremental.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/merge.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/create_table_as.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/create_table_as.sql`

 * *Files 5% similar despite different names*

```diff
@@ -11,42 +11,41 @@
   {%- set s3_data_dir = config.get('s3_data_dir', default=target.s3_data_dir) -%}
   {%- set s3_data_naming = config.get('s3_data_naming', default=target.s3_data_naming) -%}
   {%- set extra_table_properties = config.get('table_properties', default=none) -%}
 
   {%- set location_property = 'external_location' -%}
   {%- set partition_property = 'partitioned_by' -%}
   {%- set work_group_output_location_enforced = adapter.is_work_group_output_location_enforced() -%}
-  {%- set location = adapter.s3_table_location(s3_data_dir,
-                                               s3_data_naming,
-                                               relation.schema,
-                                               relation.identifier,
-                                               relation.s3_path_table_part,
-                                               external_location,
-                                               temporary) -%}
+  {%- set location = adapter.generate_s3_location(relation,
+                                                 s3_data_dir,
+                                                 s3_data_naming,
+                                                 external_location,
+                                                 temporary) -%}
 
-  {%- if materialized == 'table_hive_ha' -%}
-    {%- set location = location.replace('__ha', '') -%}
-  {%- endif %}
+  {%- set contract_config = config.get('contract') -%}
+  {%- if contract_config.enforced -%}
+    {{ get_assert_columns_equivalent(sql) }}
+  {%- endif -%}
 
   {%- if table_type == 'iceberg' -%}
     {%- set location_property = 'location' -%}
     {%- set partition_property = 'partitioning' -%}
     {%- if bucketed_by is not none or bucket_count is not none -%}
       {%- set ignored_bucket_iceberg -%}
       bucketed_by or bucket_count cannot be used with Iceberg tables. You have to use the bucket function
       when partitioning. Will be ignored
       {%- endset -%}
       {%- set bucketed_by = none -%}
       {%- set bucket_count = none -%}
       {% do log(ignored_bucket_iceberg) %}
     {%- endif -%}
-    {%- if s3_data_naming in ['table', 'schema_table'] or external_location is not none -%}
+    {%- if 'unique' not in s3_data_naming or external_location is not none -%}
       {%- set error_unique_location_iceberg -%}
-        You need to have an unique table location when creating Iceberg table. Right now we are building tables in
-        a destructive way but in the near future we will be using the RENAME feature to provide near-zero downtime.
+        You need to have an unique table location when creating Iceberg table since we use the RENAME feature
+        to have near-zero downtime.
       {%- endset -%}
       {% do exceptions.raise_compiler_error(error_unique_location_iceberg) %}
     {%- endif -%}
   {%- endif %}
 
   {% do adapter.delete_from_s3(location) %}
```

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/table.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/table.sql`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,113 @@
+-- TODO create a drop_relation_with_versions, to be sure to remove all historical versions of a table
 {% materialization table, adapter='athena' -%}
   {%- set identifier = model['alias'] -%}
 
   {%- set lf_tags = config.get('lf_tags', default=none) -%}
   {%- set lf_tags_columns = config.get('lf_tags_columns', default=none) -%}
   {%- set table_type = config.get('table_type', default='hive') | lower -%}
   {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
+  {%- set is_ha = config.get('ha', default=false) -%}
+  {%- set s3_data_dir = config.get('s3_data_dir', default=target.s3_data_dir) -%}
+  {%- set s3_data_naming = config.get('s3_data_naming', default='table_unique') -%}
+  {%- set full_refresh_config = config.get('full_refresh', default=False) -%}
+  {%- set is_full_refresh_mode = (flags.FULL_REFRESH == True or full_refresh_config == True) -%}
+  {%- set versions_to_keep = config.get('versions_to_keep', default=4) -%}
+  {%- set external_location = config.get('external_location', default=none) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
                                                 database=database,
                                                 type='table') -%}
+  {%- set tmp_relation = api.Relation.create(identifier=target_relation.identifier ~ '__ha',
+                                             schema=schema,
+                                             database=database,
+                                             s3_path_table_part=target_relation.identifier,
+                                             type='table') -%}
+
+  {%- if (
+    table_type == 'hive'
+    and is_ha
+    and ('unique' not in s3_data_naming or external_location is not none)
+  ) -%}
+      {%- set error_unique_location_hive_ha -%}
+          You need to have an unique table location when using ha config with hive table.
+          Use s3_data_naming unique, table_unique or schema_table_unique, and avoid to set an explicit
+          external_location.
+      {%- endset -%}
+      {% do exceptions.raise_compiler_error(error_unique_location_hive_ha) %}
+  {%- endif -%}
 
   {{ run_hooks(pre_hooks) }}
 
-  {%- if old_relation is none or table_type != 'iceberg' -%}
-    {%- if old_relation is not none -%}
-      {{ drop_relation(old_relation) }}
+  {%- if table_type == 'hive' -%}
+
+    -- for ha tables that are not in full refresh mode and when the relation exists we use the swap behavior
+    {%- if is_ha and not is_full_refresh_mode and old_relation is not none -%}
+      -- drop the tmp_relation
+      {%- if tmp_relation is not none -%}
+        {%- do adapter.delete_from_glue_catalog(tmp_relation) -%}
+      {%- endif -%}
+
+      -- create tmp table
+      {% call statement('main') -%}
+        {{ create_table_as(False, tmp_relation, sql) }}
+      {%- endcall %}
+
+      -- swap table
+      {%- set swap_table = adapter.swap_table(tmp_relation,
+                                              target_relation) -%}
+
+      -- delete glue tmp table, do not use drop_relation, as it will remove data of the target table
+      {%- do adapter.delete_from_glue_catalog(tmp_relation) -%}
+
+      {% do adapter.expire_glue_table_versions(target_relation,
+                                               versions_to_keep,
+                                               True) %}
+    {%- else -%}
+      -- Here we are in the case of non-ha tables or ha tables but in case of full refresh.
+      {%- if old_relation is not none -%}
+        {{ drop_relation(old_relation) }}
+      {%- endif -%}
+      {%- call statement('main') -%}
+        {{ create_table_as(False, target_relation, sql) }}
+      {%- endcall %}
     {%- endif -%}
 
-    {%- call statement('main') -%}
-      {{ create_table_as(False, target_relation, sql) }}
-    {%- endcall %}
+    {{ set_table_classification(target_relation) }}
 
-    {%- if table_type != 'iceberg' -%}
-      {{ set_table_classification(target_relation) }}
-    {%- endif -%}
   {%- else -%}
-    {%- set tmp_relation = api.Relation.create(identifier=target_relation.identifier ~ '__ha',
-                                               schema=schema,
-                                               database=database,
-                                               s3_path_table_part=target_relation.identifier,
-                                               type='table') -%}
-    {%- if tmp_relation is not none -%}
-      {%- do drop_relation(tmp_relation) -%}
-    {%- endif -%}
 
-    {%- set old_relation_bkp = make_temp_relation(old_relation, '__bkp') -%}
-    -- If we have this, it means that at least the first renaming occurred but there was an issue
-    -- afterwards, therefore we are in weird state. The easiest and cleanest should be to remove
-    -- the backup relation. It won't have an impact because since we are in the else condition, that
-    -- means that old relation exists therefore no downtime yet.
-    {%- if old_relation_bkp is not none -%}
-      {%- do drop_relation(old_relation_bkp) -%}
-    {%- endif -%}
+    {%- if old_relation is none -%}
+      {%- call statement('main') -%}
+        {{ create_table_as(False, target_relation, sql) }}
+      {%- endcall %}
+    {%- else -%}
+      {%- if tmp_relation is not none -%}
+        {%- do drop_relation(tmp_relation) -%}
+      {%- endif -%}
+
+      {%- set old_relation_bkp = make_temp_relation(old_relation, '__bkp') -%}
+      -- If we have this, it means that at least the first renaming occurred but there was an issue
+      -- afterwards, therefore we are in weird state. The easiest and cleanest should be to remove
+      -- the backup relation. It won't have an impact because since we are in the else condition,
+      -- that means that old relation exists therefore no downtime yet.
+      {%- if old_relation_bkp is not none -%}
+        {%- do drop_relation(old_relation_bkp) -%}
+      {%- endif -%}
+
+      {%- call statement('main') -%}
+        {{ create_table_as(False, tmp_relation, sql) }}
+      {%- endcall -%}
 
-    {%- call statement('main') -%}
-      {{ create_table_as(False, tmp_relation, sql) }}
-    {%- endcall -%}
+      {{ rename_relation(old_relation, old_relation_bkp) }}
+      {{ rename_relation(tmp_relation, target_relation) }}
 
-    {{ rename_relation(old_relation, old_relation_bkp) }}
-    {{ rename_relation(tmp_relation, target_relation) }}
+      {{ drop_relation(old_relation_bkp) }}
+    {%- endif -%}
 
-    {{ drop_relation(old_relation_bkp) }}
   {%- endif -%}
 
   {{ run_hooks(post_hooks) }}
 
   {% if lf_tags is not none or lf_tags_columns is not none %}
     {{ adapter.add_lf_tags(target_relation.schema, identifier, lf_tags, lf_tags_columns) }}
   {% endif %}
```

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/seeds/helpers.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/seeds/helpers.sql`

 * *Files 5% similar despite different names*

```diff
@@ -38,31 +38,29 @@
   {%- set lf_tags_columns = config.get('lf_tags_columns', default=none) -%}
   {%- set column_override = config.get('column_types', {}) -%}
   {%- set quote_seed_column = config.get('quote_columns', None) -%}
   {%- set s3_data_dir = config.get('s3_data_dir', default=target.s3_data_dir) -%}
   {%- set s3_data_naming = config.get('s3_data_naming', target.s3_data_naming) -%}
   {%- set external_location = config.get('external_location', default=none) -%}
 
-  {%- set tmp_s3_location = adapter.upload_seed_to_s3(
-    s3_data_dir,
-    s3_data_naming,
-    external_location,
-    model.schema,
-    model.name + "__dbt_tmp",
-    agate_table,
-  ) -%}
-
-  -- create tmp relation
   {%- set tmp_relation = api.Relation.create(
     identifier=identifier + "__dbt_tmp",
     schema=model.schema,
     database=model.database,
     type='table'
   ) -%}
 
+  {%- set tmp_s3_location = adapter.upload_seed_to_s3(
+    tmp_relation,
+    agate_table,
+    s3_data_dir,
+    s3_data_naming,
+    external_location,
+  ) -%}
+
   -- create target relation
   {%- set relation = api.Relation.create(
     identifier=identifier,
     schema=model.schema,
     database=model.database,
     type='table'
   ) -%}
```

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/datediff.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/timestamps.sql` & `dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/timestamps.sql`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 {% macro athena__current_timestamp() -%}
   {{ cast_timestamp('now()') }}
 {%- endmacro %}
 
 
 {% macro cast_timestamp(timestamp_col) -%}
-  {%- set config = model['config'] -%}
+  {%- set config = model.get('config', {}) -%}
   {%- set table_type = config.get('table_type', 'glue') -%}
   {%- if table_type == 'iceberg' -%}
     cast({{ timestamp_col }} as timestamp(6))
   {%- else -%}
     cast({{ timestamp_col }} as timestamp)
   {%- endif -%}
 {%- endmacro %}
```

### Comparing `dbt-athena-community-1.4.5/dbt/include/athena/profile_template.yml` & `dbt-athena-community-1.5.0/dbt/include/athena/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/dbt_athena_community.egg-info/PKG-INFO` & `dbt-athena-community-1.5.0/dbt_athena_community.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.4.5
+Version: 1.5.0
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,15 +24,15 @@
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
 
 ## Features
 
-* Supports dbt version `1.4.*`
+* Supports dbt version `1.5.*`
 * Supports [seeds][seeds]
 * Correctly detects views and their columns
 * Supports [table materialization][table]
   * [Iceberg tables][athena-iceberg] are supported **only with Athena Engine v3** and **a unique table location**
   (see table location section below)
   * Hive tables are supported by both Athena engines.
 * Supports [incremental models][incremental]
@@ -131,25 +131,29 @@
 
 
 ## Models
 
 ### Table Configuration
 
 * `external_location` (`default=none`)
-  * If set, the full S3 path in which the table will be saved. (Does not work with Iceberg table).
+  * If set, the full S3 path in which the table will be saved.
+  * Does not work with Iceberg table or Hive table with `ha` set to true.
 * `partitioned_by` (`default=none`)
   * An array list of columns by which the table will be partitioned
   * Limited to creation of 100 partitions (_currently_)
 * `bucketed_by` (`default=none`)
   * An array list of columns to bucket data, ignored if using Iceberg
 * `bucket_count` (`default=none`)
   * The number of buckets for bucketing your data, ignored if using Iceberg
 * `table_type` (`default='hive'`)
   * The type of table
   * Supports `hive` or `iceberg`
+* `ha` (`default=false`)
+  * If the table should be built using the high-availability method. This option is only available for Hive tables
+    since it is by default for Iceberg tables (see the section [below](#highly-available-table))
 * `format` (`default='parquet'`)
   * The data format for the table
   * Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE`
 * `write_compression` (`default=none`)
   * The compression type to use for any storage format that allows compression to be specified. To see which options are available, check out [CREATE TABLE AS][create-table-as]
 * `field_delimiter` (`default=none`)
   * Custom field delimiter, for when format is set to `TEXTFILE`
@@ -168,15 +172,15 @@
 The location in which a table is saved is determined by:
 
 1. If `external_location` is defined, that value is used.
 2. If `s3_data_dir` is defined, the path is determined by that and `s3_data_naming`
 3. If `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/`
 
 Here all the options available for `s3_data_naming`:
-* `uuid`: `{s3_data_dir}/{uuid4()}/`
+* `unique`: `{s3_data_dir}/{uuid4()}/`
 * `table`: `{s3_data_dir}/{table}/`
 * `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/`
 * `schema_table`: `{s3_data_dir}/{schema}/{table}/`
 * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/{table}/{uuid4()}/`
 
 It's possible to set the `s3_data_naming` globally in the target profile, or overwrite the value in the table config,
 or setting up the value for groups of model in dbt_project.yml.
@@ -263,25 +267,27 @@
 	'active' as status,
 	17.89 as cost,
 	1 as quantity,
 	100000000 as quantity_big,
 	current_date as my_date
 ```
 
-### High availability table materialization
+### Highly available table
 The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
-To have the less destructive behavior it's possible to use `table='table_hive_ha'` materialization.
-**table_hive_ha** leverages the table versions feature of Glue catalog, creating a temp table and swapping
-the target table to the location of the temp table.
-This materialization is only available for `table_type='hive'` and requires using unique locations.
+To have the less destructive behavior it's possible to use the `ha` config on your `table` materialized models.
+It leverages the table versions feature of glue catalog, creating a tmp table and swapping the target table to the
+location of the tmp table. This materialization is only available for `table_type=hive` and requires using unique
+locations. For iceberg, high availability is by default.
 
 ```sql
 {{ config(
-    materialized='table_hive_ha',
+    materialized='table',
+    ha=true,
     format='parquet',
+    table_type='hive',
     partition_by=['status'],
     s3_data_naming='table_unique'
 ) }}
 
 select
   'a' as user_id,
   'pi' as user_name,
@@ -423,14 +429,24 @@
 
 * In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not installed in the target environment.
   See https://github.com/dbt-athena/dbt-athena/issues/103 for more details.
 
 * Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
 
 
+## Contracts
+
+The adapter partly supports contract definition.
+* Concerning the `data_type`, it is supported but needs to be adjusted for complex types. They must be specified
+  entirely (for instance `array<int>`) even though they won't be checked. Indeed, as dbt recommends, we only compare
+  the broader type (array, map, int, varchar). The complete definition is used in order to check that the data types
+  defined in athena are ok (pre-flight check).
+* the adapter does not support the constraints since no constraints don't exist in Athena.
+
+
 ## Contributing
 
 See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 
 ## Contributors ✨
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.5 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.5.0 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -11,15 +11,15 @@
 License-File: LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
  code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
                                     month]
-## Features * Supports dbt version `1.4.*` * Supports [seeds][seeds] *
+## Features * Supports dbt version `1.5.*` * Supports [seeds][seeds] *
 Correctly detects views and their columns * Supports [table materialization]
 [table] * [Iceberg tables][athena-iceberg] are supported **only with Athena
 Engine v3** and **a unique table location** (see table location section below)
 * Hive tables are supported by both Athena engines. * Supports [incremental
 models][incremental] * On Iceberg tables : * Supports the use of `unique_key`
 only with the `merge` strategy * Supports the `append` strategy * On Hive
 tables : * Supports two incremental update strategies: `insert_overwrite` and
@@ -73,38 +73,42 @@
 profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
 s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
 your_s3_bucket/dbt/ s3_data_naming: schema_table region_name: eu-west-1 schema:
 dbt database: awsdatacatalog aws_profile_name: my-profile work_group: my-
 workgroup lf_tags: origin: dbt team: analytics ``` _Additional information_ *
 `threads` is supported * `database` and `catalog` can be used interchangeably
 ## Models ### Table Configuration * `external_location` (`default=none`) * If
-set, the full S3 path in which the table will be saved. (Does not work with
-Iceberg table). * `partitioned_by` (`default=none`) * An array list of columns
-by which the table will be partitioned * Limited to creation of 100 partitions
-(_currently_) * `bucketed_by` (`default=none`) * An array list of columns to
-bucket data, ignored if using Iceberg * `bucket_count` (`default=none`) * The
-number of buckets for bucketing your data, ignored if using Iceberg *
-`table_type` (`default='hive'`) * The type of table * Supports `hive` or
-`iceberg` * `format` (`default='parquet'`) * The data format for the table *
-Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
+set, the full S3 path in which the table will be saved. * Does not work with
+Iceberg table or Hive table with `ha` set to true. * `partitioned_by`
+(`default=none`) * An array list of columns by which the table will be
+partitioned * Limited to creation of 100 partitions (_currently_) *
+`bucketed_by` (`default=none`) * An array list of columns to bucket data,
+ignored if using Iceberg * `bucket_count` (`default=none`) * The number of
+buckets for bucketing your data, ignored if using Iceberg * `table_type`
+(`default='hive'`) * The type of table * Supports `hive` or `iceberg` * `ha`
+(`default=false`) * If the table should be built using the high-availability
+method. This option is only available for Hive tables since it is by default
+for Iceberg tables (see the section [below](#highly-available-table)) *
+`format` (`default='parquet'`) * The data format for the table * Supports
+`ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
 (`default=none`) * The compression type to use for any storage format that
 allows compression to be specified. To see which options are available, check
 out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
 Custom field delimiter, for when format is set to `TEXTFILE` *
 `table_properties`: table properties to add to the table, valid for Iceberg
 only * `lf_tags` (`default=none`) * lf tags to associate with the table *
 format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
 (`default=none`) * lf tags to associate with the table columns * format: `
 {"tag1": {"value1": ["column1": "column2"]}}` [create-table-as]: https://
 docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 ### Table location The location in which a table is saved is determined by: 1.
 If `external_location` is defined, that value is used. 2. If `s3_data_dir` is
 defined, the path is determined by that and `s3_data_naming` 3. If
 `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/
-` Here all the options available for `s3_data_naming`: * `uuid`: `
+` Here all the options available for `s3_data_naming`: * `unique`: `
 {s3_data_dir}/{uuid4()}/` * `table`: `{s3_data_dir}/{table}/` * `table_unique`:
 `{s3_data_dir}/{table}/{uuid4()}/` * `schema_table`: `{s3_data_dir}/{schema}/
 {table}/` * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/
 {table}/{uuid4()}/` It's possible to set the `s3_data_naming` globally in the
 target profile, or overwrite the value in the table config, or setting up the
 value for groups of model in dbt_project.yml. > Note: when using a workgroup
 with a default output location configured, `s3_data_naming` and any configured
@@ -142,26 +146,27 @@
 can use any column of the incremental table (`src`) or the final table
 (`target`). You must prefix the column by the name of the table to prevent
 `Column is ambiguous` error. ```sql {{ config( materialized='incremental',
 table_type='iceberg', incremental_strategy='merge', unique_key='user_id',
 delete_condition="src.status != 'active' and target.my_date < now() - interval
 '2' year", format='parquet' ) }} select 'A' as user_id, 'pi' as name, 'active'
 as status, 17.89 as cost, 1 as quantity, 100000000 as quantity_big,
-current_date as my_date ``` ### High availability table materialization The
-current implementation of the table materialization can lead to downtime, as
-target table is dropped and re-created. To have the less destructive behavior
-it's possible to use `table='table_hive_ha'` materialization. **table_hive_ha**
-leverages the table versions feature of Glue catalog, creating a temp table and
-swapping the target table to the location of the temp table. This
-materialization is only available for `table_type='hive'` and requires using
-unique locations. ```sql {{ config( materialized='table_hive_ha',
-format='parquet', partition_by=['status'], s3_data_naming='table_unique' ) }}
-select 'a' as user_id, 'pi' as user_name, 'active' as status union all select
-'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default, the
-materialization keeps the last 4 table versions, you can change it by setting
+current_date as my_date ``` ### Highly available table The current
+implementation of the table materialization can lead to downtime, as target
+table is dropped and re-created. To have the less destructive behavior it's
+possible to use the `ha` config on your `table` materialized models. It
+leverages the table versions feature of glue catalog, creating a tmp table and
+swapping the target table to the location of the tmp table. This
+materialization is only available for `table_type=hive` and requires using
+unique locations. For iceberg, high availability is by default. ```sql {
+{ config( materialized='table', ha=true, format='parquet', table_type='hive',
+partition_by=['status'], s3_data_naming='table_unique' ) }} select 'a' as
+user_id, 'pi' as user_name, 'active' as status union all select 'b' as user_id,
+'sh' as user_name, 'disabled' as status ``` By default, the materialization
+keeps the last 4 table versions, you can change it by setting
 `versions_to_keep`. #### Known issues * When swapping from a table with
 partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions * By default, Glue "duplicates" the versions internally,
 so the last two versions of a table point to the same location * It's
 recommended to have `versions_to_keep` >= 4, as this will avoid having the
 older location removed * The macro `athena__end_of_time` needs to be
@@ -202,18 +207,25 @@
 way, from a dbt perspective, is to do a full-refresh of the incremental model.
 * Tables, schemas and database should only be lowercase * In order to avoid
 potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/
 dbt-athena) is not installed in the target environment. See https://github.com/
 dbt-athena/dbt-athena/issues/103 for more details. * Snapshot does not support
 dropping columns from the source table. If you drop a column make sure to drop
 the column from the snapshot as well. Another workaround is to NULL the column
-in the snapshot definition to preserve history ## Contributing See
-[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
-this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
+in the snapshot definition to preserve history ## Contracts The adapter partly
+supports contract definition. * Concerning the `data_type`, it is supported but
+needs to be adjusted for complex types. They must be specified entirely (for
+instance `array`) even though they won't be checked. Indeed, as dbt recommends,
+we only compare the broader type (array, map, int, varchar). The complete
+definition is used in order to check that the data types defined in athena are
+ok (pre-flight check). * the adapter does not support the constraints since no
+constraints don't exist in Athena. ## Contributing See [CONTRIBUTING]
+(CONTRIBUTING.md) for more information on how to contribute to this project. ##
+Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):
         [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]            [Mattia]     [Gatsby
          nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom              Mattia        Lee]
       ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð      ð§    Gatsby
                                ð ð§                                                                    Lee
                                                                                                                     ð
       [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii       [chrischin478]
        BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]       chrischin478
```

### Comparing `dbt-athena-community-1.4.5/dbt_athena_community.egg-info/SOURCES.txt` & `dbt-athena-community-1.5.0/dbt_athena_community.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 dbt/__init__.py
 dbt/adapters/__init__.py
 dbt/adapters/athena/__init__.py
 dbt/adapters/athena/__version__.py
 dbt/adapters/athena/column.py
 dbt/adapters/athena/config.py
 dbt/adapters/athena/connections.py
+dbt/adapters/athena/constants.py
+dbt/adapters/athena/exceptions.py
 dbt/adapters/athena/impl.py
 dbt/adapters/athena/query_headers.py
 dbt/adapters/athena/relation.py
+dbt/adapters/athena/s3.py
 dbt/adapters/athena/session.py
 dbt/adapters/athena/utils.py
 dbt/include/athena/__init__.py
 dbt/include/athena/dbt_project.yml
 dbt/include/athena/profile_template.yml
 dbt/include/athena/sample_profiles.yml
 dbt/include/athena/macros/adapters/columns.sql
@@ -27,30 +30,29 @@
 dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
 dbt/include/athena/macros/materializations/models/incremental/helpers.sql
 dbt/include/athena/macros/materializations/models/incremental/incremental.sql
 dbt/include/athena/macros/materializations/models/incremental/merge.sql
 dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
 dbt/include/athena/macros/materializations/models/table/create_table_as.sql
 dbt/include/athena/macros/materializations/models/table/table.sql
-dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql
 dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
 dbt/include/athena/macros/materializations/models/view/create_view_as.sql
 dbt/include/athena/macros/materializations/models/view/view.sql
 dbt/include/athena/macros/materializations/seeds/helpers.sql
 dbt/include/athena/macros/materializations/snapshots/snapshot.sql
 dbt/include/athena/macros/utils/any_value.sql
 dbt/include/athena/macros/utils/array_append.sql
 dbt/include/athena/macros/utils/array_concat.sql
 dbt/include/athena/macros/utils/array_construct.sql
 dbt/include/athena/macros/utils/bool_or.sql
 dbt/include/athena/macros/utils/datatypes.sql
 dbt/include/athena/macros/utils/date_trunc.sql
 dbt/include/athena/macros/utils/dateadd.sql
 dbt/include/athena/macros/utils/datediff.sql
-dbt/include/athena/macros/utils/ddl_data_type.sql
+dbt/include/athena/macros/utils/ddl_dml_data_type.sql
 dbt/include/athena/macros/utils/hash.sql
 dbt/include/athena/macros/utils/right.sql
 dbt/include/athena/macros/utils/safe_cast.sql
 dbt/include/athena/macros/utils/timestamps.sql
 dbt_athena_community.egg-info/PKG-INFO
 dbt_athena_community.egg-info/SOURCES.txt
 dbt_athena_community.egg-info/dependency_links.txt
```

### Comparing `dbt-athena-community-1.4.5/pyproject.toml` & `dbt-athena-community-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.5/setup.py` & `dbt-athena-community-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 def _get_package_version():
     parts = _get_plugin_version_dict()
     return f'{parts["major"]}.{parts["minor"]}.{parts["patch"]}'
 
 
-dbt_version = "1.4"
+dbt_version = "1.5"
 package_version = _get_package_version()
 description = "The athena adapter plugin for dbt (data build tool)"
 
 if not package_version.startswith(dbt_version):
     raise ValueError(f"Invalid setup.py: package_version={package_version} must start with dbt_version={dbt_version}")
 
 
@@ -50,16 +50,16 @@
     url="https://github.com/dbt-athena/dbt-athena",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         # In order to control dbt-core version and package version
         "boto3~=1.26",
         "boto3-stubs[athena,glue,lakeformation,sts]~=1.26",
-        "dbt-core~=1.4.6",
-        "pyathena~=2.25",
+        "dbt-core~=1.5.0",
+        "pyathena>=2.25,<4.0",
         "tenacity~=8.2",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

