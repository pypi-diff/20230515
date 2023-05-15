# Comparing `tmp/MindsDB-23.4.4.4.tar.gz` & `tmp/MindsDB-23.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MindsDB-23.4.4.4.tar", last modified: Fri Apr 28 12:46:21 2023, max compression
+gzip compressed data, was "dist/MindsDB-23.5.3.1.tar", last modified: Mon May 15 16:04:06 2023, max compression
```

## Comparing `MindsDB-23.4.4.4.tar` & `MindsDB-23.5.3.1.tar`

### file list

```diff
@@ -1,1167 +1,1298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/MindsDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23809 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54604 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23809 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    56478 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)    23115 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    67024 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/nlp/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autokeras_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autokeras_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/file_handler/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/huggingface_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/jira_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/langchain_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20696 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99045 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    98530 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/predict-db.png
--rw-r--r--   0 runner    (1001) docker     (123)   100718 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mlflow_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27870 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/postgres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/ray_serve_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/rockset_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/rockset_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/solr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
--rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/error.png
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
--rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
--rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/statsforecast_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tpot_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/db_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/ml_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/ml_grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/ml_exec_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/ml_handler_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/libs/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    18638 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/base/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/kafka/kafkadb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/redis/redisdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/interfaces/stream/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:46:21.000000 MindsDB-23.4.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-28 12:46:07.000000 MindsDB-23.4.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23210 2023-05-15 16:04:05.000000 MindsDB-23.5.3.1/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    61801 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:04:05.000000 MindsDB-23.5.3.1/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-15 16:04:05.000000 MindsDB-23.5.3.1/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 16:04:05.000000 MindsDB-23.5.3.1/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23210 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/namespaces/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56525 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23115 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67024 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/nlp/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autokeras_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autokeras_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/file_handler/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/gitlab_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/gitlab_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/gitlab_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_fit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_fit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_fit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_fit_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hackernews_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hackernews_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hackernews_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_api_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/langchain_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    88354 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/1-create_db.png
+-rw-r--r--   0 runner    (1001) docker     (123)   110633 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/2-create_predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)   109269 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/3-predict_target.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62778 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/4-drop_db.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99045 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98530 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/predict-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100718 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/maxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/maxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/maxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mlflow_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png
+-rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/newsapi_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/newsapi_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/newsapi_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28085 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/postgres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/quickbooks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/rockset_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sendinblue_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/slack_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/slack_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/slack_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/slack_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/slack_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/slack_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/solr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+-rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/strava_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/strava_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/strava_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/strava_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/strava_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tpot_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/youtube_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/youtube_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/youtube_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/youtube_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/youtube_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/db_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/ml_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/ml_grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/handler_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/ml_exec_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/ml_handler_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/libs/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22438 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/base/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/kafka/kafkadb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/redis/redisdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/interfaces/stream/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:04:06.000000 MindsDB-23.5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-15 16:03:54.000000 MindsDB-23.5.3.1/setup.py
```

### Comparing `MindsDB-23.4.4.4/MindsDB.egg-info/PKG-INFO` & `MindsDB-23.5.3.1/MindsDB.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.4.4.4
+Version: 23.5.3.1
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -123,32 +123,33 @@
         
         ## Database Integrations
         
         MindsDB works with most of the SQL and NoSQL databases, data lakes, data Streams and popular applications.
         
         | Connect your Data | Connect your Data | Connect your Data
         |-|-|-|
-        | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
-        | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/Apache-Pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/TiDB#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#yugabyte"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
+        | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href="https://docs.mindsdb.com/data-integrations/datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
+        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
+        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
+        | <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
+        
         
         
         [:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
         
         
         ## Documentation
         
@@ -196,12 +197,13 @@
         
         Join our [Slack community](https://mindsdb.com/joincommunity) and subscribe to the monthly [Developer Newsletter](https://mindsdb.com/newsletter/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get product updates, information about MindsDB events and contests, and useful content, like tutorials.
         
         
         ## License
         
         MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.4.4.4 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.5.3.1 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -137,9 +137,9 @@
 joincommunity) and subscribe to the monthly [Developer Newsletter](https://
 mindsdb.com/newsletter/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
 product updates, information about MindsDB events and contests, and useful
 content, like tutorials. ## License MindsDB is licensed under [GNU General
 Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
+Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown
```

### Comparing `MindsDB-23.4.4.4/MindsDB.egg-info/SOURCES.txt` & `MindsDB-23.5.3.1/MindsDB.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 mindsdb/api/http/namespaces/analysis.py
 mindsdb/api/http/namespaces/auth.py
 mindsdb/api/http/namespaces/config.py
 mindsdb/api/http/namespaces/databases.py
 mindsdb/api/http/namespaces/default.py
 mindsdb/api/http/namespaces/file.py
 mindsdb/api/http/namespaces/handlers.py
+mindsdb/api/http/namespaces/models.py
 mindsdb/api/http/namespaces/projects.py
 mindsdb/api/http/namespaces/sql.py
 mindsdb/api/http/namespaces/stream.py
 mindsdb/api/http/namespaces/tab.py
 mindsdb/api/http/namespaces/tree.py
 mindsdb/api/http/namespaces/util.py
+mindsdb/api/http/namespaces/views.py
 mindsdb/api/http/namespaces/configs/__init__.py
 mindsdb/api/http/namespaces/configs/analysis.py
 mindsdb/api/http/namespaces/configs/auth.py
 mindsdb/api/http/namespaces/configs/config.py
 mindsdb/api/http/namespaces/configs/databases.py
 mindsdb/api/http/namespaces/configs/default.py
 mindsdb/api/http/namespaces/configs/files.py
@@ -289,16 +291,19 @@
 mindsdb/integrations/handlers/crate_handler/crate_handler.py
 mindsdb/integrations/handlers/crate_handler/icon.svg
 mindsdb/integrations/handlers/crate_handler/requirements.txt
 mindsdb/integrations/handlers/crate_handler/tests/__init__.py
 mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
 mindsdb/integrations/handlers/d0lt_handler/__about__.py
 mindsdb/integrations/handlers/d0lt_handler/__init__.py
+mindsdb/integrations/handlers/d0lt_handler/create-db.png
+mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
 mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
 mindsdb/integrations/handlers/d0lt_handler/icon.svg
+mindsdb/integrations/handlers/d0lt_handler/predict-target.png
 mindsdb/integrations/handlers/d0lt_handler/requirements.txt
 mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
 mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
 mindsdb/integrations/handlers/databend_handler/__about__.py
 mindsdb/integrations/handlers/databend_handler/__init__.py
 mindsdb/integrations/handlers/databend_handler/databend_handler.py
 mindsdb/integrations/handlers/databend_handler/icon.png
@@ -403,22 +408,63 @@
 mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
 mindsdb/integrations/handlers/github_handler/__about__.py
 mindsdb/integrations/handlers/github_handler/__init__.py
 mindsdb/integrations/handlers/github_handler/github_handler.py
 mindsdb/integrations/handlers/github_handler/github_tables.py
 mindsdb/integrations/handlers/github_handler/icon.svg
 mindsdb/integrations/handlers/github_handler/requirements.txt
+mindsdb/integrations/handlers/gitlab_handler/__about__.py
+mindsdb/integrations/handlers/gitlab_handler/__init__.py
+mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+mindsdb/integrations/handlers/gitlab_handler/icon.svg
+mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+mindsdb/integrations/handlers/google_books_handler/__about__.py
+mindsdb/integrations/handlers/google_books_handler/__init__.py
+mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+mindsdb/integrations/handlers/google_books_handler/icon.svg
+mindsdb/integrations/handlers/google_books_handler/requirements.txt
+mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
 mindsdb/integrations/handlers/google_calendar_handler/__about__.py
 mindsdb/integrations/handlers/google_calendar_handler/__init__.py
 mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
 mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
 mindsdb/integrations/handlers/google_calendar_handler/icon.svg
 mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
 mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
 mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
+mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+mindsdb/integrations/handlers/google_fit_handler/__about__.py
+mindsdb/integrations/handlers/google_fit_handler/__init__.py
+mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+mindsdb/integrations/handlers/google_fit_handler/icon.png
+mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+mindsdb/integrations/handlers/google_search_handler/__about__.py
+mindsdb/integrations/handlers/google_search_handler/__init__.py
+mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+mindsdb/integrations/handlers/google_search_handler/icon.svg
+mindsdb/integrations/handlers/google_search_handler/requirements.txt
+mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+mindsdb/integrations/handlers/hackernews_handler/__about__.py
+mindsdb/integrations/handlers/hackernews_handler/__init__.py
+mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+mindsdb/integrations/handlers/hackernews_handler/icon.svg
 mindsdb/integrations/handlers/hana_handler/__about__.py
 mindsdb/integrations/handlers/hana_handler/__init__.py
 mindsdb/integrations/handlers/hana_handler/hana_handler.py
 mindsdb/integrations/handlers/hana_handler/icon.svg
 mindsdb/integrations/handlers/hana_handler/requirements.txt
 mindsdb/integrations/handlers/hive_handler/__about__.py
 mindsdb/integrations/handlers/hive_handler/__init__.py
@@ -428,14 +474,21 @@
 mindsdb/integrations/handlers/hive_handler/tests/__init__.py
 mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
 mindsdb/integrations/handlers/hsqldb_handler/__about__.py
 mindsdb/integrations/handlers/hsqldb_handler/__init__.py
 mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
 mindsdb/integrations/handlers/hsqldb_handler/icon.png
 mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+mindsdb/integrations/handlers/huggingface_api_handler/setup.py
+mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
 mindsdb/integrations/handlers/huggingface_handler/__about__.py
 mindsdb/integrations/handlers/huggingface_handler/__init__.py
 mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
 mindsdb/integrations/handlers/huggingface_handler/requirements.txt
 mindsdb/integrations/handlers/huggingface_handler/setup.py
 mindsdb/integrations/handlers/ignite_handler/__about__.py
 mindsdb/integrations/handlers/ignite_handler/__init__.py
@@ -476,14 +529,15 @@
 mindsdb/integrations/handlers/jira_handler/icon.png
 mindsdb/integrations/handlers/jira_handler/jira_handler.py
 mindsdb/integrations/handlers/jira_handler/jira_table.py
 mindsdb/integrations/handlers/jira_handler/requirements.txt
 mindsdb/integrations/handlers/langchain_handler/__about__.py
 mindsdb/integrations/handlers/langchain_handler/__init__.py
 mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
 mindsdb/integrations/handlers/langchain_handler/requirements.txt
 mindsdb/integrations/handlers/langchain_handler/setup.py
 mindsdb/integrations/handlers/lightwood_handler/__init__.py
 mindsdb/integrations/handlers/lightwood_handler/requirements.txt
 mindsdb/integrations/handlers/lightwood_handler/setup.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
@@ -495,14 +549,18 @@
 mindsdb/integrations/handlers/ludwig_handler/__about__.py
 mindsdb/integrations/handlers/ludwig_handler/__init__.py
 mindsdb/integrations/handlers/ludwig_handler/functions.py
 mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
 mindsdb/integrations/handlers/ludwig_handler/requirements.txt
 mindsdb/integrations/handlers/ludwig_handler/setup.py
 mindsdb/integrations/handlers/ludwig_handler/utils.py
+mindsdb/integrations/handlers/mariadb_handler/1-create_db.png
+mindsdb/integrations/handlers/mariadb_handler/2-create_predictor.png
+mindsdb/integrations/handlers/mariadb_handler/3-predict_target.png
+mindsdb/integrations/handlers/mariadb_handler/4-drop_db.png
 mindsdb/integrations/handlers/mariadb_handler/__about__.py
 mindsdb/integrations/handlers/mariadb_handler/__init__.py
 mindsdb/integrations/handlers/mariadb_handler/create-db.png
 mindsdb/integrations/handlers/mariadb_handler/icon.svg
 mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
 mindsdb/integrations/handlers/mariadb_handler/predict-db.png
 mindsdb/integrations/handlers/mariadb_handler/predictor.png
@@ -517,30 +575,40 @@
 mindsdb/integrations/handlers/matrixone_handler/__about__.py
 mindsdb/integrations/handlers/matrixone_handler/__init__.py
 mindsdb/integrations/handlers/matrixone_handler/icon.png
 mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
 mindsdb/integrations/handlers/matrixone_handler/requirements.txt
 mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
 mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+mindsdb/integrations/handlers/maxdb_handler/__about__.py
+mindsdb/integrations/handlers/maxdb_handler/__init__.py
+mindsdb/integrations/handlers/maxdb_handler/icon.png
+mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
 mindsdb/integrations/handlers/merlion_handler/__about__.py
 mindsdb/integrations/handlers/merlion_handler/__init__.py
 mindsdb/integrations/handlers/merlion_handler/adapters.py
 mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
 mindsdb/integrations/handlers/merlion_handler/requirements.txt
 mindsdb/integrations/handlers/merlion_handler/setup.py
 mindsdb/integrations/handlers/mlflow_handler/__about__.py
 mindsdb/integrations/handlers/mlflow_handler/__init__.py
 mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
 mindsdb/integrations/handlers/mlflow_handler/requirements.txt
 mindsdb/integrations/handlers/mlflow_handler/setup.py
 mindsdb/integrations/handlers/monetdb_handler/__about__.py
 mindsdb/integrations/handlers/monetdb_handler/__init__.py
+mindsdb/integrations/handlers/monetdb_handler/create-database.png
+mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
 mindsdb/integrations/handlers/monetdb_handler/icon.png
 mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
 mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
 mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
 mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
 mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
 mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
 mindsdb/integrations/handlers/mongodb_handler/__about__.py
 mindsdb/integrations/handlers/mongodb_handler/__init__.py
 mindsdb/integrations/handlers/mongodb_handler/icon.svg
@@ -561,14 +629,21 @@
 mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
 mindsdb/integrations/handlers/mysql_handler/requirements.txt
 mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
 mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
 mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
 mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
 mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+mindsdb/integrations/handlers/newsapi_handler/__about__.py
+mindsdb/integrations/handlers/newsapi_handler/__init__.py
+mindsdb/integrations/handlers/newsapi_handler/icon.png
+mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
 mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
 mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
 mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
 mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
 mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
 mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
 mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
@@ -624,29 +699,39 @@
 mindsdb/integrations/handlers/plaid_handler/icon.svg
 mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
 mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
 mindsdb/integrations/handlers/plaid_handler/requirements.txt
 mindsdb/integrations/handlers/plaid_handler/utils.py
 mindsdb/integrations/handlers/planetscale_handler/__about__.py
 mindsdb/integrations/handlers/planetscale_handler/__init__.py
+mindsdb/integrations/handlers/planetscale_handler/create-db.png
+mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
+mindsdb/integrations/handlers/planetscale_handler/drop-db.png
 mindsdb/integrations/handlers/planetscale_handler/icon.svg
 mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+mindsdb/integrations/handlers/planetscale_handler/predict-target.png
 mindsdb/integrations/handlers/planetscale_handler/requirements.txt
 mindsdb/integrations/handlers/postgres_handler/__about__.py
 mindsdb/integrations/handlers/postgres_handler/__init__.py
 mindsdb/integrations/handlers/postgres_handler/icon.svg
 mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
 mindsdb/integrations/handlers/postgres_handler/requirements.txt
 mindsdb/integrations/handlers/questdb_handler/__about__.py
 mindsdb/integrations/handlers/questdb_handler/__init__.py
 mindsdb/integrations/handlers/questdb_handler/icon.svg
 mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
 mindsdb/integrations/handlers/questdb_handler/requirements.txt
 mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
 mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
 mindsdb/integrations/handlers/ray_serve_handler/__about__.py
 mindsdb/integrations/handlers/ray_serve_handler/__init__.py
 mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
 mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
 mindsdb/integrations/handlers/ray_serve_handler/setup.py
 mindsdb/integrations/handlers/reddit_handler/__about__.py
 mindsdb/integrations/handlers/reddit_handler/__init__.py
@@ -675,27 +760,40 @@
 mindsdb/integrations/handlers/scylla_handler/__about__.py
 mindsdb/integrations/handlers/scylla_handler/__init__.py
 mindsdb/integrations/handlers/scylla_handler/logo.png
 mindsdb/integrations/handlers/scylla_handler/requirements.txt
 mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
 mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
 mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+mindsdb/integrations/handlers/sendinblue_handler/icon.png
+mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
 mindsdb/integrations/handlers/sheets_handler/__about__.py
 mindsdb/integrations/handlers/sheets_handler/__init__.py
 mindsdb/integrations/handlers/sheets_handler/icon.png
 mindsdb/integrations/handlers/sheets_handler/requirements.txt
 mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
 mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
 mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
 mindsdb/integrations/handlers/singlestore_handler/__about__.py
 mindsdb/integrations/handlers/singlestore_handler/__init__.py
 mindsdb/integrations/handlers/singlestore_handler/requirements.txt
 mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
 mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
 mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+mindsdb/integrations/handlers/slack_handler/__about__.py
+mindsdb/integrations/handlers/slack_handler/__init__.py
+mindsdb/integrations/handlers/slack_handler/icon.svg
+mindsdb/integrations/handlers/slack_handler/requirements.txt
+mindsdb/integrations/handlers/slack_handler/slack_handler.py
+mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
 mindsdb/integrations/handlers/snowflake_handler/__about__.py
 mindsdb/integrations/handlers/snowflake_handler/__init__.py
 mindsdb/integrations/handlers/snowflake_handler/requirements.txt
 mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
 mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
 mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
 mindsdb/integrations/handlers/solr_handler/__about__.py
@@ -736,14 +834,20 @@
 mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
 mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
 mindsdb/integrations/handlers/statsforecast_handler/__about__.py
 mindsdb/integrations/handlers/statsforecast_handler/__init__.py
 mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
 mindsdb/integrations/handlers/statsforecast_handler/setup.py
 mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+mindsdb/integrations/handlers/strava_handler/__about__.py
+mindsdb/integrations/handlers/strava_handler/__init__.py
+mindsdb/integrations/handlers/strava_handler/icon.png
+mindsdb/integrations/handlers/strava_handler/requirements.txt
+mindsdb/integrations/handlers/strava_handler/strava_handler.py
+mindsdb/integrations/handlers/strava_handler/strava_tables.py
 mindsdb/integrations/handlers/supabase_handler/__about__.py
 mindsdb/integrations/handlers/supabase_handler/__init__.py
 mindsdb/integrations/handlers/supabase_handler/icon.svg
 mindsdb/integrations/handlers/supabase_handler/requirements.txt
 mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
 mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
 mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
@@ -809,14 +913,20 @@
 mindsdb/integrations/handlers/vitess_handler/__about__.py
 mindsdb/integrations/handlers/vitess_handler/__init__.py
 mindsdb/integrations/handlers/vitess_handler/icon.svg
 mindsdb/integrations/handlers/vitess_handler/requirements.txt
 mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
 mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
 mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+mindsdb/integrations/handlers/youtube_handler/__about__.py
+mindsdb/integrations/handlers/youtube_handler/__init__.py
+mindsdb/integrations/handlers/youtube_handler/icon.png
+mindsdb/integrations/handlers/youtube_handler/requirements.txt
+mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
 mindsdb/integrations/handlers/yugabyte_handler/__about__.py
 mindsdb/integrations/handlers/yugabyte_handler/__init__.py
 mindsdb/integrations/handlers/yugabyte_handler/icon.svg
 mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
 mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
 mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
 mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
```

### Comparing `MindsDB-23.4.4.4/MindsDB.egg-info/requires.txt` & `MindsDB-23.5.3.1/MindsDB.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lightwood<23.5.1.0,>=23.4.3.0
+lightwood<23.6.1.0,>=23.5.1.0
 markupsafe==2.0.1
 flask-restx<2.0.0,>=1.0.1
 flask<2.0,>=1.0
 python-multipart>=0.0.5
 pyparsing==2.3.1
 cryptography>=35.0
 psycopg[binary]>=1.15.3
@@ -19,15 +19,15 @@
 flask-compress>=1.0.0
 kafka-python>=2.0.0
 appdirs>=1.0.0
 mindsdb-sql<0.7.0,>=0.6.1
 mindsdb-evaluator<0.1.0,>=0.0.7
 checksumdir>=1.2.0
 mindsdb-streams==0.1.1
-duckdb==0.4.0
+duckdb==0.6.0
 requests>=2.0.0
 mysql-connector-python
 clickhouse-driver
 clickhouse-sqlalchemy
 charset-normalizer
 dill>=0.3.4
 pyOpenSSL>=22.0.0
```

### Comparing `MindsDB-23.4.4.4/PKG-INFO` & `MindsDB-23.5.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.4.4.4
+Version: 23.5.3.1
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -123,32 +123,33 @@
         
         ## Database Integrations
         
         MindsDB works with most of the SQL and NoSQL databases, data lakes, data Streams and popular applications.
         
         | Connect your Data | Connect your Data | Connect your Data
         |-|-|-|
-        | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
-        | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/Apache-Pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/TiDB#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#yugabyte"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
+        | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href="https://docs.mindsdb.com/data-integrations/datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
+        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
+        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
+        | <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
+        
         
         
         [:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
         
         
         ## Documentation
         
@@ -196,12 +197,13 @@
         
         Join our [Slack community](https://mindsdb.com/joincommunity) and subscribe to the monthly [Developer Newsletter](https://mindsdb.com/newsletter/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get product updates, information about MindsDB events and contests, and useful content, like tutorials.
         
         
         ## License
         
         MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.4.4.4 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.5.3.1 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -137,9 +137,9 @@
 joincommunity) and subscribe to the monthly [Developer Newsletter](https://
 mindsdb.com/newsletter/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
 product updates, information about MindsDB events and contests, and useful
 content, like tutorials. ## License MindsDB is licensed under [GNU General
 Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
+Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown
```

### Comparing `MindsDB-23.4.4.4/README.md` & `MindsDB-23.5.3.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -114,32 +114,33 @@
 
 ## Database Integrations
 
 MindsDB works with most of the SQL and NoSQL databases, data lakes, data Streams and popular applications.
 
 | Connect your Data | Connect your Data | Connect your Data
 |-|-|-|
-| <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
-| <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/Apache-Pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/TiDB#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#yugabyte"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-| <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
-| <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
+| <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href="https://docs.mindsdb.com/data-integrations/datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
+| <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
+| <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
+| <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
+
 
 
 [:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
 
 
 ## Documentation
 
@@ -186,8 +187,8 @@
 ## Subscribe to updates
 
 Join our [Slack community](https://mindsdb.com/joincommunity) and subscribe to the monthly [Developer Newsletter](https://mindsdb.com/newsletter/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get product updates, information about MindsDB events and contests, and useful content, like tutorials.
 
 
 ## License
 
-MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
+MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
```

### Comparing `MindsDB-23.4.4.4/mindsdb/__main__.py` & `MindsDB-23.5.3.1/mindsdb/__main__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/common/check_auth.py` & `MindsDB-23.5.3.1/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/gui.py` & `MindsDB-23.5.3.1/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-23.5.3.1/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/initialize.py` & `MindsDB-23.5.3.1/mindsdb/api/http/initialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,19 +21,21 @@
 from mindsdb.api.http.namespaces.analysis import ns_conf as analysis_ns
 from mindsdb.api.http.namespaces.auth import ns_conf as auth_ns
 from mindsdb.api.http.namespaces.config import ns_conf as conf_ns
 from mindsdb.api.http.namespaces.databases import ns_conf as databases_ns
 from mindsdb.api.http.namespaces.default import ns_conf as default_ns, check_auth
 from mindsdb.api.http.namespaces.file import ns_conf as file_ns
 from mindsdb.api.http.namespaces.handlers import ns_conf as handlers_ns
+from mindsdb.api.http.namespaces.models import ns_conf as models_ns
 from mindsdb.api.http.namespaces.projects import ns_conf as projects_ns
 from mindsdb.api.http.namespaces.sql import ns_conf as sql_ns
 from mindsdb.api.http.namespaces.stream import ns_conf as stream_ns
 from mindsdb.api.http.namespaces.tab import ns_conf as tab_ns
 from mindsdb.api.http.namespaces.tree import ns_conf as tree_ns
+from mindsdb.api.http.namespaces.views import ns_conf as views_ns
 from mindsdb.api.http.namespaces.util import ns_conf as utils_ns
 from mindsdb.api.nlp.nlp import ns_conf as nlp_ns
 from mindsdb.interfaces.database.integrations import integration_controller
 from mindsdb.interfaces.database.database import DatabaseController
 from mindsdb.interfaces.file.file_controller import FileController
 from mindsdb.interfaces.storage import db
 from mindsdb.utilities import log
@@ -204,15 +206,17 @@
         conf_ns,
         file_ns,
         sql_ns,
         analysis_ns,
         handlers_ns,
         tree_ns,
         projects_ns,
-        databases_ns
+        databases_ns,
+        views_ns,
+        models_ns
     ]
     if with_nlp:
         protected_namespaces.append(nlp_ns)
 
     for ns in protected_namespaces:
         api.add_namespace(ns)
     api.add_namespace(default_ns)
```

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/auth.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/config.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/databases.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/default.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/file.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/sql.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/stream.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/tab.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/tree.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/namespaces/util.py` & `MindsDB-23.5.3.1/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/start.py` & `MindsDB-23.5.3.1/mindsdb/api/http/start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/http/utils.py` & `MindsDB-23.5.3.1/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/classes/responder.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/classes/scram.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/classes/session.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/delete.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/find.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/insert.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/server.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-23.5.3.1/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -841,14 +841,15 @@
 
             predictions = project_datanode.predict(
                 model_name=predictor_name,
                 data=where_data,
                 version=version,
                 params=step.params,
             )
+
             columns_dtypes = dict(predictions.dtypes)
             predictions = predictions.to_dict(orient='records')
 
             # update predictions with input data
             for row in predictions:
                 for k, v in where_data.items():
                     if k not in row:
@@ -959,15 +960,15 @@
                             data=where_data,
                             version=version,
                             params=params
                         )
                         data = predictions.to_dict(orient='records')
                         columns_dtypes = dict(predictions.dtypes)
 
-                        if data is not None and isinstance(data, list):
+                        if data is not None and isinstance(data, list) and self.session.predictor_cache is not False:
                             predictor_cache.set(key, data)
                     else:
                         columns_dtypes = {}
 
                     if len(data) > 0:
                         cols = list(data[0].keys())
                         for col in cols:
```

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/data_types.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     logger,
 )
 import mindsdb.utilities.profiler as profiler
 from mindsdb.api.mysql.mysql_proxy.executor.executor_commands import ExecuteCommands
 
 
 class Executor:
-    """This class stores initial and intermediatea params
+    """This class stores initial and intermediate params
     between different steps of query execution. And it is also
     creates a separate instance of ExecuteCommands to execute the current
     query step.
 
     IMPORTANT: A public API of this class is a contract.
     And there are at least 2 classes strongly depend on it:
         ExecuctorClient
```

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/functions.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/mysql/mysql_proxy/utilities/sql.py` & `MindsDB-23.5.3.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/nlp/nlp.py` & `MindsDB-23.5.3.1/mindsdb/api/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-23.5.3.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/autokeras_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/autokeras_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/autosklearn_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/logo.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def create(self, target, df=None, args=None, **kwargs):
         is_cloud = Config().get('cloud', False)
         if is_cloud is True:
             raise RuntimeError('BYOM is disabled on cloud')
 
         model_proxy = self._get_model_proxy()
 
-        model_state = model_proxy.train(df, target)
+        model_state = model_proxy.train(df, target, args)
 
         self.model_storage.file_set('model', model_state)
 
         # TODO return columns?
 
         def convert_type(field_type):
             if pd_types.is_integer_dtype(field_type):
@@ -59,20 +59,21 @@
         columns = {
             target: convert_type(np.object)
         }
 
         self.model_storage.columns_set(columns)
 
     def predict(self, df, args=None):
+        pred_args = args.get('predict_params', {})
 
         model_proxy = self._get_model_proxy()
 
         model_state = self.model_storage.file_get('model')
 
-        pred_df = model_proxy.predict(df, model_state)
+        pred_df = model_proxy.predict(df, model_state, pred_args)
 
         return pred_df
 
     def create_engine(self, connection_args):
         # check code and requirements
 
         model_proxy = self._get_model_proxy()
@@ -191,32 +192,34 @@
 
         params = {
             'method': 'check',
             'code': self.code,
         }
         return self._run_command(params)
 
-    def train(self, df, target):
+    def train(self, df, target, args):
         params = {
             'method': 'train',
             'df': pd_encode(df),
             'code': self.code,
-            'to_predict': target
+            'to_predict': target,
+            'args': args,
         }
 
         model_state = self._run_command(params)
         return model_state
 
-    def predict(self, df, model_state):
+    def predict(self, df, model_state, args):
 
         params = {
             'method': 'predict',
             'code': self.code,
             'df': pd_encode(df),
             'model_state': model_state,
+            'args': args,
         }
         pred_df = self._run_command(params)
         return pd_decode(pred_df)
 
 
 connection_args = OrderedDict(
     code={
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,31 +105,40 @@
             raise RuntimeError('Model class has to have "predict" method')
 
         return_output(True)
 
     if method == 'train':
         df = pd_decode(params['df'])
         to_predict = params['to_predict']
+        args = params['args']
         model = model_class()
-        model.train(df, to_predict)
+
+        call_args = [df, to_predict]
+        if args:
+            call_args.append(args)
+        model.train(*call_args)
 
         # return model
         data = model.__dict__
 
         model_state = encode(data)
         return_output(model_state)
 
     elif method == 'predict':
         model_state = params['model_state']
         df = pd_decode(params['df'])
+        args = params['args']
 
         model = model_class()
         model.__dict__ = decode(model_state)
 
-        res = model.predict(df)
+        call_args = [df]
+        if args:
+            call_args.append(args)
+        res = model.predict(*call_args)
         return_output(pd_encode(res))
 
     raise NotImplementedError(method)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/logo.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/logo.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections import OrderedDict
 
 import pandas as pd
-import clickhouse_driver
 from sqlalchemy import create_engine
 from clickhouse_sqlalchemy.drivers.base import ClickHouseDialect
 from mindsdb_sql.parser.ast.base import ASTNode
 from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 
 from mindsdb.utilities import log
 from mindsdb.integrations.libs.base import DatabaseHandler
@@ -26,35 +25,45 @@
 
     def __init__(self, name, connection_data, **kwargs):
         super().__init__(name)
         self.dialect = 'clickhouse'
         self.connection_data = connection_data
         self.renderer = SqlalchemyRender(ClickHouseDialect)
         self.is_connected = False
-        self.protocol = connection_data.get('protocol', 'native')
+        self.protocol = connection_data.get('protocol', 'clickhouse')
+
+        # region added for back-compatibility with connections creatad before 11.05.2023
+        protocols_map = {
+            'native': 'clickhouse+native',
+            'http': 'clickhouse+http',
+            'https': 'clickhouse+https',
+        }
+        if self.protocol in protocols_map:
+            self.protocol = protocols_map[self.protocol]
+        # endregion
 
     def __del__(self):
         if self.is_connected is True:
             self.disconnect()
 
     def connect(self):
         """
         Handles the connection to a ClickHouse
         """
         if self.is_connected is True:
             return self.connection
 
-        protocol = "clickhouse+native" if self.protocol == 'native' else "clickhouse+http"
+        protocol = self.protocol
         host = self.connection_data['host']
         port = self.connection_data['port']
         user = self.connection_data['user']
         password = self.connection_data['password']
         database = self.connection_data['database']
         url = f'{protocol}://{user}:{password}@{host}:{port}/{database}'
-        if self.protocol == 'https':
+        if self.protocol == 'clickhouse+https':
             url = url + "?protocol=https"
 
         engine = create_engine(url)
         connection = engine.raw_connection()
         self.is_connected = True
         self.connection = connection
         return self.connection
@@ -150,15 +159,15 @@
         result = self.native_query(q)
         return result
 
 
 connection_args = OrderedDict(
     protocol={
         'type': ARG_TYPE.STR,
-        'protocol': 'The protocol to query clickhouse. Supported: native, http, https. Default: native'
+        'protocol': 'The protocol to query clickhouse. Supported: clickhouse, clickhouse+native, clickhouse+http, clickhouse+https. Default: clickhouse'
     },
     user={
         'type': ARG_TYPE.STR,
         'description': 'The user name used to authenticate with the ClickHouse server.'
     },
     password={
         'type': ARG_TYPE.STR,
@@ -175,14 +184,14 @@
     port={
         'type': ARG_TYPE.INT,
         'description': 'The TCP/IP port of the ClickHouse server. Must be an integer.'
     }
 )
 
 connection_args_example = OrderedDict(
-    protocol='native',
+    protocol='clickhouse',
     host='127.0.0.1',
     port=9000,
     user='root',
     password='password',
     database='database'
 )
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/confluence_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/confluence_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/logo.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,13 +304,13 @@
 
     def get_columns(self, table_name) -> Response:
         file_meta = self.file_controller.get_file_meta(table_name)
         result = Response(
             RESPONSE_TYPE.TABLE,
             data_frame=pd.DataFrame([
                 {
-                    'Field': x.strip(),
+                    'Field': x['name'].strip() if isinstance(x, dict) else x.strip(),
                     'Type': 'str'
                 } for x in file_meta['columns']
             ])
         )
         return result
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import github
 
-from mindsdb.integrations.handlers.github_handler.github_tables import GithubIssuesTable
+from mindsdb.integrations.handlers.github_handler.github_tables import (
+    GithubIssuesTable,
+    GithubPullRequestsTable,
+)
 from mindsdb.integrations.libs.api_handler import APIHandler
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
 )
 
 from mindsdb.utilities.log import get_log
 from mindsdb_sql import parse_sql
@@ -31,15 +34,17 @@
         self.repository = connection_data["repository"]
         self.kwargs = kwargs
 
         self.connection = None
         self.is_connected = False
 
         github_issues_data = GithubIssuesTable(self)
+        github_pull_requests_data = GithubPullRequestsTable(self)
         self._register_table("issues", github_issues_data)
+        self._register_table("pull_requests", github_pull_requests_data)
 
     def connect(self) -> StatusResponse:
         """Set up the connection required by the handler.
 
         Returns
         -------
         StatusResponse
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 import os
-
 import pandas as pd
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
-from mindsdb_sql import parse_sql
-from pandas import DataFrame
-
 from mindsdb.api.mysql.mysql_proxy.libs.constants.response_type import RESPONSE_TYPE
 from .google_calendar_tables import GoogleCalendarEventsTable
 from mindsdb.integrations.libs.api_handler import APIHandler, FuncParser
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
 )
 from mindsdb.utilities import log
 
-
 class GoogleCalendarHandler(APIHandler):
     """
         A class for handling connections and interactions with the Google Calendar API.
     """
     name = 'google_calendar'
 
     def __init__(self, name: str, **kwargs):
@@ -35,18 +30,19 @@
         """
         super().__init__(name)
 
         self.token = None
         self.service = None
         self.connection_data = kwargs.get('connection_data', {})
         self.credentials_file = self.connection_data.get('credentials', None)
+        self.scopes = ['https://www.googleapis.com/auth/calendar', 
+              'https://www.googleapis.com/auth/calendar.events',
+              'https://www.googleapis.com/auth/calendar.readonly'
+            ]
         self.credentials = None
-        self.scopes = ['https://www.googleapis.com/auth/calendar', 'https://www.googleapis.com/auth/calendar.events',
-                       'https://www.googleapis.com/auth/calendar.readonly',
-                       'https://www.googleapis.com/auth/calendar.readonly']
         self.is_connected = False
         events = GoogleCalendarEventsTable(self)
         self.events = events
         self._register_table('events', events)
 
     def connect(self):
         """
@@ -107,15 +103,15 @@
         df = self.call_application_api(method_name, params)
 
         return Response(
             RESPONSE_TYPE.TABLE,
             data_frame=df
         )
 
-    def get_events(self, params: dict = None) -> DataFrame:
+    def get_events(self, params: dict = None) -> pd.DataFrame:
         """
         Get events from Google Calendar API
         Args:
             params (dict): query parameters
         Returns:
             DataFrame
         """
@@ -129,24 +125,27 @@
                 ignore_index=True
             )
             page_token = events_result.get('nextPageToken')
             if not page_token:
                 break
         return events
 
-    def create_event(self, params: dict = None) -> DataFrame:
+    def create_event(self, params: dict = None) -> pd.DataFrame:
         """
         Create an event in the calendar.
         Args:
             params (dict): query parameters
         Returns:
             DataFrame
         """
         service = self.connect()
-        params['attendees'] = params['attendees'].split(',')
+        # Check if 'attendees' is a string and split it into a list
+        if isinstance(params['attendees'], str):
+            params['attendees'] = params['attendees'].split(',')
+
         event = {
             'summary': params['summary'],
             'location': params['location'],
             'description': params['description'],
             'start': {
                 'dateTime': params['start']['dateTime'],
                 'timeZone': params['start']['timeZone'],
@@ -154,29 +153,30 @@
             'end': {
                 'dateTime': params['end']['dateTime'],
                 'timeZone': params['end']['timeZone'],
             },
             'recurrence': [
                 'RRULE:FREQ=DAILY;COUNT=2'
             ],
-            'attendees': {
-                [{'email': attendee} for attendee in params['attendees']]
-            },
+            'attendees': [{'email': attendee['email']} for attendee in (params['attendees'] 
+                            if isinstance(params['attendees'], list) else [params['attendees']])],
             'reminders': {
                 'useDefault': False,
                 'overrides': [
                     {'method': 'email', 'minutes': 24 * 60},
                     {'method': 'popup', 'minutes': 10},
                 ],
             },
         }
-        event = service.events().insert(calendarId='primary', body=event).execute()
+
+        event = service.events().insert(calendarId='primary', 
+                                        body=event).execute()
         return pd.DataFrame([event], columns=self.events.get_columns())
 
-    def update_event(self, params: dict = None) -> DataFrame:
+    def update_event(self, params: dict = None) -> pd.DataFrame:
         """
         Update event or events in the calendar.
         Args:
             params (dict): query parameters
         Returns:
             DataFrame
         """
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import datetime
 from mindsdb_sql.parser import ast
 from pandas import DataFrame
 
 from mindsdb.integrations.libs.api_handler import APITable
 from mindsdb.integrations.libs.response import (
     HandlerResponse as Response,
 )
@@ -36,16 +37,15 @@
                     raise NotImplementedError
             elif arg1 == 'timeZone':
                 params[arg1] = arg2
             elif arg1 == 'maxAttendees':
                 params[arg1] = arg2
             elif arg1 == 'q':
                 params[arg1] = arg2
-            else:
-                raise NotImplementedError
+           
 
         # Get the order by from the query.
         if query.order_by is not None:
             if query.order_by[0].value == 'start_time':
                 params['orderBy'] = 'startTime'
             elif query.order_by[0].value == 'updated':
                 params['orderBy'] = 'updated'
@@ -87,39 +87,45 @@
             Response: Response object containing the results.
         """
 
         # Get the values from the query.
         values = query.values[0]
         # Get the event data from the values.
         event_data = {}
+        timestamp_columns = {'start_time', 'end_time', 'created', 'updated'}
+        regular_columns = {'summary', 'description', 'location', 'status', 'html_link',
+                            'creator', 'organizer', 'reminders', 'timeZone', 'calendar_id', 'attendees'}
+
+        # TODO: check why query.columns is None
         for col, val in zip(query.columns, values):
-            if col == 'start_time' or col == 'end_time' or col == 'created' or col == 'updated':
-                event_data[col] = utc_date_str_to_timestamp_ms(val)
-            elif col == 'summary' or col == 'description' or col == 'location' or col == 'status' or col == 'html_link' \
-                    or col == 'creator' or col == 'organizer' or col == 'reminders' \
-                    or col == 'timeZone' or col == 'calendar_id' or col == 'attendees':
-                event_data[col] = val
+            if col.name in timestamp_columns:
+                event_data[col.name] = utc_date_str_to_timestamp_ms(val)
+            elif col.name in regular_columns:
+                event_data[col.name] = val
             else:
                 raise NotImplementedError
+            
+        st = datetime.datetime.utcfromtimestamp(event_data['start_time'] / 1000).isoformat() + 'Z'
+        et = datetime.datetime.utcfromtimestamp(event_data['end_time'] / 1000).isoformat() + 'Z'
 
         event_data['start'] = {
-            'dateTime': event_data['start_time'],
+            'dateTime': st,
             'timeZone': event_data['timeZone']
         }
 
         event_data['end'] = {
-            'dateTime': event_data['end_time'],
+            'dateTime': et,
             'timeZone': event_data['timeZone']
         }
 
         event_data['attendees'] = event_data['attendees'].split(',')
         event_data['attendees'] = [{'email': attendee} for attendee in event_data['attendees']]
 
         # Insert the event into the Google Calendar API.
-        self.handler.call_application_api(method_name='insert_event', params=event_data)
+        self.handler.call_application_api(method_name='create_event', params=event_data)
 
     def update(self, query: ast.Update):
         """
         Updates an event or events in the calendar.
 
         Args:
             query (ast.Update): SQL query to parse.
@@ -200,15 +206,14 @@
 
         # Delete the events in the Google Calendar API.
         self.handler.call_application_api(method_name='delete_event', params=params)
 
     def get_columns(self) -> list:
         """Gets all columns to be returned in pandas DataFrame responses"""
         return [
-            'kind',
             'etag',
             'id',
             'status',
             'htmlLink',
             'created',
             'updated',
             'summary',
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/huggingface_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/huggingface_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/jira_handler/jira_table.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/jira_handler/jira_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/langchain_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/langchain_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,27 +466,25 @@
         if attribute == 'info':
 
             model_description = {}
 
             model_info = self.model_storage.get_info()
             model_data = model_info['data']
             to_predict = model_info['to_predict'][0]
-            json_ai = self.model_storage.json_get('json_ai')
 
             if model_data.get('accuracies', None) is not None:
                 if len(model_data['accuracies']) > 0:
                     model_data['accuracy'] = float(np.mean(list(model_data['accuracies'].values())))
 
             model_columns = self.model_storage.columns_get()
 
             model_description['accuracies'] = model_data['accuracies']
             model_description['column_importances'] = model_data['column_importances']
             model_description['outputs'] = [to_predict]
             model_description['inputs'] = [col for col in model_columns if col not in model_description['outputs']]
-            model_description['model'] = ' --> '.join(str(k) for k in json_ai)
 
             return pd.DataFrame([model_description])
 
         elif attribute == "features":
             return self._get_features_info()
 
         elif attribute == "model":
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ludwig_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ludwig_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/create-db.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/predict-db.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/predict-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mariadb_handler/predictor.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mariadb_handler/predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/merlion_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/merlion_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mlflow_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mlflow_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         """
         need_to_close = self.is_connected is False
         conn = self.connect()
         cur=conn.cursor() 
         try:
             cur.execute(query)
                    
-            if cur._rows>0 :
+            if len(cur._rows)>0 :
                 result = cur.fetchall() 
                 response = Response(
                     RESPONSE_TYPE.TABLE,
                     data_frame=pd.DataFrame(
                         result,
                         columns=[x[0] for x in cur.description]
                     )
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/neuralforecast_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 
 from mindsdb.utilities import log
 from mindsdb.utilities.config import Config
 from mindsdb.integrations.libs.base import BaseMLEngine
 from mindsdb.integrations.handlers.openai_handler.helpers import retry_with_exponential_backoff, \
     truncate_msgs_for_token_limit
 
+CHAT_MODELS = ('gpt-3.5-turbo', 'gpt-3.5-turbo-0301', 'gpt-4', 'gpt-4-0314', 'gpt-4-32k', 'gpt-4-32k-0314')
+
 
 class OpenAIHandler(BaseMLEngine):
     name = 'openai'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.default_model = 'gpt-3.5-turbo'
         self.default_mode = 'default'  # can also be 'conversational' or 'conversational-full'
         self.supported_modes = ['default', 'conversational', 'conversational-full', 'image']
         self.rate_limit = 60  # requests per minute
         self.max_batch_size = 20
         self.default_max_tokens = 100
-        self.chat_completion_models = (
-            'gpt-3.5-turbo', 'gpt-3.5-turbo-0301',
-            'gpt-4', 'gpt-4-0314', 'gpt-4-32k', 'gpt-4-32k-0314'
-        )
+        self.chat_completion_models = CHAT_MODELS
 
     @staticmethod
     def create_validation(target, args=None, **kwargs):
         if 'using' not in args:
             raise Exception("OpenAI engine requires a USING clause! Refer to its documentation for more details.")
         else:
             args = args['using']
@@ -61,16 +60,20 @@
                         3) a `json_struct`
                 '''))
 
     def create(self, target, args=None, **kwargs):
         args = args['using']
 
         args['target'] = target
+        available_models = [m.openai_id for m in openai.Model.list().data]
         if not args.get('model_name'):
             args['model_name'] = self.default_model
+        elif args['model_name'] not in available_models:
+            raise Exception(f"Invalid model name. Please use one of {available_models}")
+
         if not args.get('mode'):
             args['mode'] = self.default_mode
         elif args['mode'] not in self.supported_modes:
             raise Exception(f"Invalid operation mode. Please use one of {self.supported_modes}")
 
         self.model_storage.json_set('args', args)
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/openai_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/openai_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/planetscale_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/ray_serve_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/rockset_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/rockset_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/logo.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/solr.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/solr.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/db_connection.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/error.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/error.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/model_drop.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/statsforecast_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/teradata_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/teradata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/tpot_handler/setup.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/tpot_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/icon.png` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/twitter_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/twitter_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/ml_client_factory.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/ml_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers_client/ml_grpc_client.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers_client/ml_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-23.5.3.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/libs/api_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/libs/api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/libs/base.py` & `MindsDB-23.5.3.1/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-23.5.3.1/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-23.5.3.1/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from mindsdb.integrations.utilities.sql_utils import make_sql_session
 from mindsdb.utilities.config import Config
 import mindsdb.interfaces.storage.db as db
 from mindsdb.integrations.libs.response import (
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
-from mindsdb import __version__ as mindsdb_version
+from mindsdb.__about__ import __version__ as mindsdb_version
 from mindsdb.utilities.hooks import after_predict as after_predict_hook
 from mindsdb.interfaces.model.model_controller import ModelController
 from mindsdb.interfaces.model.functions import (
     get_model_record
 )
 from mindsdb.api.mysql.mysql_proxy.classes.sql_query import SQLQuery
 from mindsdb.integrations.libs.const import PREDICTOR_STATUS
@@ -365,14 +365,25 @@
         # if self.handler_class.__name__ == 'LightwoodHandler':
         if self.handler_class.__name__ == 'LightwoodHandler':
             args['code'] = predictor_record.code
             args['target'] = predictor_record.to_predict[0]
             args['dtype_dict'] = predictor_record.dtype_dict
             args['learn_args'] = predictor_record.learn_args
 
+        if self.handler_class.__name__ in ('LangChainHandler',):
+            from mindsdb.api.mysql.mysql_proxy.controllers import SessionController
+            from mindsdb.api.mysql.mysql_proxy.executor.executor_commands import ExecuteCommands
+
+            sql_session = SessionController()
+            sql_session.database = 'mindsdb'
+
+            command_executor = ExecuteCommands(sql_session, executor=None)
+
+            args['executor'] = command_executor
+
         try:
             predictions = ml_handler.predict(df, args)
         except Exception as e:
             msg = str(e).strip()
             if msg == '':
                 msg = e.__class__.__name__
             msg = f'[{self.name}/{model_name}]: {msg}'
```

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/libs/ml_handler_proc.py` & `MindsDB-23.5.3.1/mindsdb/integrations/libs/ml_handler_proc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-23.5.3.1/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/libs/response.py` & `MindsDB-23.5.3.1/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-23.5.3.1/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-23.5.3.1/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/utilities/install.py` & `MindsDB-23.5.3.1/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-23.5.3.1/mindsdb/integrations/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-23.5.3.1/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-23.5.3.1/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/database/database.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/database/integrations.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/database/integrations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,155 @@
+import os
+import sys
 import base64
 import shutil
 import tempfile
 import importlib
+import threading
 from time import time
 from pathlib import Path
 from copy import deepcopy
+from typing import Optional
 from collections import OrderedDict
 
 from sqlalchemy import func
 
 from mindsdb.interfaces.storage import db
 from mindsdb.utilities.config import Config
 from mindsdb.interfaces.storage.fs import FsStore, FileStorage, FileStorageFactory, RESOURCE_GROUP
 from mindsdb.interfaces.file.file_controller import FileController
+from mindsdb.integrations.libs.base import DatabaseHandler
 from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE, HANDLER_TYPE
 from mindsdb.integrations.handlers_client.db_client_factory import DBClient
 from mindsdb.interfaces.model.functions import get_model_records
 from mindsdb.utilities.context import context as ctx
 from mindsdb.utilities.log import get_log
 
 
 logger = get_log()
 
 
+class HandlersCache:
+    """ Cache for data handlers that keep connections opened during ttl time from handler last use
+    """
+
+    def __init__(self, ttl: int = 60):
+        """ init cache
+
+            Args:
+                ttl (int): time to live (in seconds) for record in cache
+        """
+        self.ttl = ttl
+        self.handlers = {}
+        self._lock = threading.RLock()
+        self._stop_event = threading.Event()
+        self.cleaner_thread = None
+
+    def __del__(self):
+        self._stop_clean()
+
+    def _start_clean(self) -> None:
+        """ start worker that close connections after ttl expired
+        """
+        if (
+            isinstance(self.cleaner_thread, threading.Thread)
+            and self.cleaner_thread.is_alive()
+        ):
+            return
+        self._stop_event.clear()
+        self.cleaner_thread = threading.Thread(target=self._clean)
+        self.cleaner_thread.start()
+
+    def _stop_clean(self) -> None:
+        """ stop clean worker
+        """
+        self._stop_event.set()
+
+    def set(self, handler: DatabaseHandler):
+        """ add (or replace) handler in cache
+
+            Args:
+                handler (DatabaseHandler)
+        """
+        # print(f'!!!! set {handler.name} {ctx.company_id} {threading.get_ident()}')
+        with self._lock:
+            try:
+                key = (handler.name, ctx.company_id, threading.get_ident())
+                handler.connect()
+                self.handlers[key] = {
+                    'handler': handler,
+                    'expired_at': time() + self.ttl
+                }
+            except Exception:
+                pass
+            self._start_clean()
+
+    def get(self, name: str) -> Optional[DatabaseHandler]:
+        """ get handler from cache by name
+
+            Args:
+                name (str): handler name
+
+            Returns:
+                DatabaseHandler
+        """
+        with self._lock:
+            key = (name, ctx.company_id, threading.get_ident())
+            if (
+                key not in self.handlers
+                or self.handlers[key]['expired_at'] < time()
+            ):
+                return None
+            self.handlers[key]['expired_at'] = time() + self.ttl
+            return self.handlers[key]['handler']
+
+    def delete(self, name: str) -> None:
+        """ delete handler from cache
+
+            Args:
+                name (str): handler name
+        """
+        with self._lock:
+            key = (name, ctx.company_id, threading.get_ident())
+            if key in self.handlers:
+                try:
+                    self.handlers[key].disconnect()
+                except Exception:
+                    pass
+                del self.handlers[key]
+            if len(self.handlers) == 0:
+                self._stop_clean()
+
+    def _clean(self) -> None:
+        """ worker that delete from cache handlers that was not in use for ttl
+        """
+        while self._stop_event.wait(timeout=3) is False:
+            with self._lock:
+                for key in list(self.handlers.keys()):
+                    if (
+                        self.handlers[key]['expired_at'] < time()
+                        and sys.getrefcount(self.handlers[key]) == 2    # returned ref count is always 1 higher
+                    ):
+                        try:
+                            self.handlers[key].disconnect()
+                        except Exception:
+                            pass
+                        del self.handlers[key]
+                if len(self.handlers) == 0:
+                    self._stop_event.set()
+
+
 class IntegrationController:
     @staticmethod
     def _is_not_empty_str(s):
         return isinstance(s, str) and len(s) > 0
 
     def __init__(self):
         self._load_handler_modules()
+        self.handlers_cache = HandlersCache()
 
     def _add_integration_record(self, name, engine, connection_args):
         integration_record = db.Integration(
             name=name,
             engine=engine,
             data=connection_args or {},
             company_id=ctx.company_id
@@ -77,14 +193,15 @@
             )
             store.add(files_dir, '')
             store.push()
 
         return integration_id
 
     def modify(self, name, data):
+        self.handlers_cache.delete(name)
         integration_record = db.session.query(db.Integration).filter_by(
             company_id=ctx.company_id, name=name
         ).first()
         old_data = deepcopy(integration_record.data)
         for k in old_data:
             if k not in data:
                 data[k] = old_data[k]
@@ -92,14 +209,16 @@
         integration_record.data = data
         db.session.commit()
 
     def delete(self, name):
         if name in ('files', 'lightwood'):
             raise Exception('Unable to drop: is system database')
 
+        self.handlers_cache.delete(name)
+
         # check permanent integration
         if name in self.handler_modules:
             handler = self.handler_modules[name]
 
             if getattr(handler, 'permanent', False) is True:
                 raise Exception('Unable to drop: is permanent integration')
 
@@ -263,14 +382,18 @@
         logger.debug("%s.create_tmp_handler: create a client to db of %s type", self.__class__.__name__, handler_type)
         if DBClient.is_local:
             return self.handler_modules[handler_type].Handler(**handler_ars)
         else:
             return DBClient(handler_type, **handler_ars)
 
     def get_handler(self, name, case_sensitive=False):
+        handler = self.handlers_cache.get(name)
+        if handler is not None:
+            return handler
+
         if case_sensitive:
             integration_record = db.session.query(db.Integration).filter_by(company_id=ctx.company_id, name=name).first()
         else:
             integration_record = db.session.query(db.Integration).filter(
                 (db.Integration.company_id == ctx.company_id)
                 & (func.lower(db.Integration.name) == func.lower(name))
             ).first()
@@ -330,14 +453,15 @@
             handler = BaseMLEngineExec(**handler_ars)
             # handler = MLClient(**handler_ars)
         else:
 
             logger.info("%s.get_handler: create a client to db service of %s type, args - %s", self.__class__.__name__, integration_engine, handler_ars)
             if DBClient.is_local:
                 handler = HandlerClass(**handler_ars)
+                self.handlers_cache.set(handler)
             else:
                 handler = DBClient(integration_engine, **handler_ars)
 
         return handler
 
     def reload_handler_module(self, handler_name):
         importlib.reload(self.handler_modules[handler_name])
@@ -418,14 +542,20 @@
                 handler_meta['permanent'] = False
 
         return handler_meta
 
     def _load_handler_modules(self):
         mindsdb_path = Path(importlib.util.find_spec('mindsdb').origin).parent
         handlers_path = mindsdb_path.joinpath('integrations/handlers')
+
+        # edge case: running from tests directory, find_spec finds the base folder instead of actual package
+        if not os.path.isdir(handlers_path):
+            mindsdb_path = Path(importlib.util.find_spec('mindsdb').origin).parent.joinpath('mindsdb')
+            handlers_path = mindsdb_path.joinpath('integrations/handlers')
+
         self.handler_modules = {}
         self.handlers_import_status = {}
         for handler_dir in handlers_path.iterdir():
             if handler_dir.is_dir() is False or handler_dir.name.startswith('__'):
                 continue
             handler_folder_name = str(handler_dir.name)
```

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/database/projects.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/database/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/database/views.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/file/file_controller.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/model/functions.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/model/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/model/model_controller.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/model/model_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,17 +63,46 @@
         data['json_ai'] = json_storage.get('json_ai')
 
         if data.get('accuracies', None) is not None:
             if len(data['accuracies']) > 0:
                 data['accuracy'] = float(np.mean(list(data['accuracies'].values())))
         return data
 
-    def describe_model(self, session,  project_name, model_name, attribute):
+    def get_reduced_model_data(self, name: str = None, predictor_record=None, ml_handler_name='lightwood') -> dict:
+        full_model_data = self.get_model_data(name=name, predictor_record=predictor_record, ml_handler_name=ml_handler_name)
+        reduced_model_data = {}
+        for k in ['id', 'name', 'version', 'is_active', 'predict', 'status',
+                  'current_phase', 'accuracy', 'data_source', 'update', 'active',
+                  'mindsdb_version', 'error', 'created_at', 'fetch_data_query']:
+            reduced_model_data[k] = full_model_data.get(k, None)
+
+        reduced_model_data['training_time'] = None
+        if full_model_data.get('training_start_at') is not None:
+            if full_model_data.get('training_stop_at') is not None:
+                reduced_model_data['training_time'] = (
+                    full_model_data.get('training_stop_at')
+                    - full_model_data.get('training_start_at')
+                )
+            elif full_model_data.get('status') == 'training':
+                reduced_model_data['training_time'] = (
+                    dt.datetime.now()
+                    - full_model_data.get('training_start_at')
+                )
+            if reduced_model_data['training_time'] is not None:
+                reduced_model_data['training_time'] = (
+                    reduced_model_data['training_time']
+                    - dt.timedelta(microseconds=reduced_model_data['training_time'].microseconds)
+                )
+
+        return reduced_model_data
+
+    def describe_model(self, session, project_name, model_name, attribute, version=None):
         model_record = get_model_record(
             name=model_name,
+            version=version,
             project_name=project_name,
             except_absent=True
         )
         integration_record = db.Integration.query.get(model_record.integration_id)
 
         ml_handler_base = session.integration_controller.get_handler(integration_record.name)
 
@@ -96,69 +125,62 @@
                     attributes = attributes[0]
 
             model_info.insert(0, 'tables', [attributes])
             return model_info
         else:
             return df
 
+    def get_model(self, name, version=None, ml_handler_name=None, project_name=None):
+        show_active = True if version is None else False
+        model_record = get_model_record(
+            active=show_active,
+            version=version,
+            name=name,
+            ml_handler_name=ml_handler_name,
+            project_name=project_name)
+        return self.get_reduced_model_data(predictor_record=model_record)
+
     def get_models(self, with_versions=False, ml_handler_name=None, integration_id=None,
                    project_name=None):
         models = []
         show_active = True if with_versions is False else None
-        for predictor_record in get_model_records(active=show_active, ml_handler_name=ml_handler_name,
-                                                  integration_id=integration_id, project_name=project_name):
-            model_data = self.get_model_data(predictor_record=predictor_record)
-            reduced_model_data = {}
-
-            for k in ['id', 'name', 'version', 'is_active', 'predict', 'status',
-                      'current_phase', 'accuracy', 'data_source', 'update', 'active',
-                      'mindsdb_version', 'error', 'created_at', 'fetch_data_query']:
-                reduced_model_data[k] = model_data.get(k, None)
-
-            reduced_model_data['training_time'] = None
-            if model_data.get('training_start_at') is not None:
-                if model_data.get('training_stop_at') is not None:
-                    reduced_model_data['training_time'] = (
-                        model_data.get('training_stop_at')
-                        - model_data.get('training_start_at')
-                    )
-                elif model_data.get('status') == 'training':
-                    reduced_model_data['training_time'] = (
-                        dt.datetime.now()
-                        - model_data.get('training_start_at')
-                    )
-                if reduced_model_data['training_time'] is not None:
-                    reduced_model_data['training_time'] = (
-                        reduced_model_data['training_time']
-                        - dt.timedelta(microseconds=reduced_model_data['training_time'].microseconds)
-                    )
-
-            models.append(reduced_model_data)
+        for model_record in get_model_records(active=show_active, ml_handler_name=ml_handler_name,
+                                              integration_id=integration_id, project_name=project_name):
+            model_data = self.get_reduced_model_data(predictor_record=model_record)
+            models.append(model_data)
         return models
 
-    def delete_model(self, model_name: str, project_name: str = 'mindsdb'):
+    def delete_model(self, model_name: str, project_name: str = 'mindsdb', version=None):
         from mindsdb.interfaces.database.database import DatabaseController
 
         project_record = db.Project.query.filter(
             (func.lower(db.Project.name) == func.lower(project_name))
             & (db.Project.company_id == ctx.company_id)
             & (db.Project.deleted_at == null())
         ).first()
         if project_record is None:
             raise Exception(f"Project '{project_name}' does not exists")
 
         database_controller = DatabaseController()
 
         project = database_controller.get_project(project_name)
 
-        predictors_records = get_model_records(
-            name=model_name,
-            project_id=project.id,
-            active=None,
-        )
+        if version is None:
+            # Delete latest version
+            predictors_records = get_model_records(
+                name=model_name,
+                project_id=project.id,
+                active=None,
+            )
+        else:
+            predictors_records = get_model_records(
+                name=model_name,
+                project_id=project.id,
+                version=version,
+            )
         if len(predictors_records) == 0:
             raise Exception(f"Model '{model_name}' does not exist")
 
         is_cloud = self.config.get('cloud', False)
         if is_cloud:
             for predictor_record in predictors_records:
                 model_data = self.get_model_data(predictor_record=predictor_record)
@@ -191,15 +213,15 @@
         predictor_record = get_model_record(name=name, except_absent=True)
 
         fs_name = f'predictor_{ctx.company_id}_{predictor_record.id}'
         self.fs_store.pull()
         local_predictor_savefile = os.path.join(self.fs_store.folder_path, fs_name)
         predictor_binary = open(local_predictor_savefile, 'rb').read()
 
-        # Serialize a predictor record into a dictionary 
+        # Serialize a predictor record into a dictionary
         # move into the Predictor db class itself if we use it again somewhere
         json_storage = get_json_storage(
             resource_id=predictor_record.id
         )
         predictor_record_serialized = {
             'name': predictor_record.name,
             'data': predictor_record.data,
@@ -519,8 +541,7 @@
                 model_record.deleted_at = dt.datetime.now()
             else:
                 db.session.delete(model_record)
             modelStorage = ModelStorage(model_record.id)
             modelStorage.delete()
 
         db.session.commit()
-
```

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/storage/db.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/storage/db.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/storage/fs.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/storage/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/storage/json.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/stream/base/integration.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/stream/base/integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/stream/kafka/kafkadb.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/stream/kafka/kafkadb.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/stream/redis/redisdb.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/stream/redis/redisdb.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/interfaces/stream/stream.py` & `MindsDB-23.5.3.1/mindsdb/interfaces/stream/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-23.5.3.1/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-23.5.3.1/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-23.5.3.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-23.5.3.1/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-23.5.3.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-23.5.3.1/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-23.5.3.1/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-23.5.3.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/alembic.ini` & `MindsDB-23.5.3.1/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/env.py` & `MindsDB-23.5.3.1/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/migrate.py` & `MindsDB-23.5.3.1/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-23.5.3.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/auth.py` & `MindsDB-23.5.3.1/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/cache.py` & `MindsDB-23.5.3.1/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/config.py` & `MindsDB-23.5.3.1/mindsdb/utilities/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/context.py` & `MindsDB-23.5.3.1/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/fs.py` & `MindsDB-23.5.3.1/mindsdb/utilities/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/functions.py` & `MindsDB-23.5.3.1/mindsdb/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/hooks/profiling.py` & `MindsDB-23.5.3.1/mindsdb/utilities/hooks/profiling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/json_encoder.py` & `MindsDB-23.5.3.1/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/log.py` & `MindsDB-23.5.3.1/mindsdb/utilities/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/log_controller.py` & `MindsDB-23.5.3.1/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/profiler/profiler.py` & `MindsDB-23.5.3.1/mindsdb/utilities/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/ps.py` & `MindsDB-23.5.3.1/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/telemetry.py` & `MindsDB-23.5.3.1/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/mindsdb/utilities/wizards.py` & `MindsDB-23.5.3.1/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.4/setup.py` & `MindsDB-23.5.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,9 +60,9 @@
     install_requires=pkgs,
     dependency_links=new_links,
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7"
+    python_requires=">=3.8"
 )
```

