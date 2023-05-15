# Comparing `tmp/ultipa-4.2.4.tar.gz` & `tmp/ultipa-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ultipa-4.2.4.tar", last modified: Wed Mar  8 10:31:04 2023, max compression
+gzip compressed data, was "dist/ultipa-4.3.0.tar", last modified: Mon May 15 08:56:44 2023, max compression
```

## Comparing `ultipa-4.2.4.tar` & `ultipa-4.3.0.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa/
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa/types/
--rw-r--r--   0 ultipa     (501) staff       (20)     8460 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/types/types_response.py
--rw-r--r--   0 ultipa     (501) staff       (20)      206 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/types/__init__.py
--rw-r--r--   0 ultipa     (501) staff       (20)    34640 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/types/types.py
--rw-r--r--   0 ultipa     (501) staff       (20)    22230 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/types/types_request.py
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa/proto/
--rw-r--r--   0 ultipa     (501) staff       (20)    27096 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/proto/ultipa_pb2_grpc.py
--rw-r--r--   0 ultipa     (501) staff       (20)        0 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/proto/__init__.py
--rw-r--r--   0 ultipa     (501) staff       (20)    44242 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/proto/ultipa_pb2.py
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa/connection/
--rw-r--r--   0 ultipa     (501) staff       (20)     2116 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/download_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1836 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/searchAB_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1553 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/searchKhop_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     6540 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/task_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1750 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/nodeSpread_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     2635 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/truncate_extra.py
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa/connection/algo/
--rw-r--r--   0 ultipa     (501) staff       (20)    13994 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/algo/algos_params.py
--rw-r--r--   0 ultipa     (501) staff       (20)     6715 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/algo/community_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)       63 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/algo/__init__.py
--rw-r--r--   0 ultipa     (501) staff       (20)    16296 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/algo/algo_params4.py
--rw-r--r--   0 ultipa     (501) staff       (20)     4212 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/algo/embedding_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)    18755 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/algo/makeAlgoClass.py
--rw-r--r--   0 ultipa     (501) staff       (20)     8292 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/algo/algo_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1986 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/algo/degrees_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)       55 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/__init__.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1557 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/autoNet_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     6478 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/policy_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     3799 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/edge_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)      386 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/export_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     2400 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/connection.py
--rw-r--r--   0 ultipa     (501) staff       (20)     6148 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/connectionPoolMaker.py
--rw-r--r--   0 ultipa     (501) staff       (20)     4539 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/property_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     3566 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/node_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     4137 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/schema_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     6164 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/user_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1408 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/lte_ufe_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)    52886 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/connection_base.py
--rw-r--r--   0 ultipa     (501) staff       (20)     3690 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/index_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     3189 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/graph_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1074 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/template_extra.py
--rw-r--r--   0 ultipa     (501) staff       (20)      711 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/connection/connectionPool.py
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa/printer/
--rw-r--r--   0 ultipa     (501) staff       (20)     7161 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/printer/prettyPrint.py
--rw-r--r--   0 ultipa     (501) staff       (20)      138 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/printer/__init__.py
--rw-r--r--   0 ultipa     (501) staff       (20)      370 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/__init__.py
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa/utils/
--rw-r--r--   0 ultipa     (501) staff       (20)     8964 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/serialize.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1383 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/raftRetry.py
--rw-r--r--   0 ultipa     (501) staff       (20)     2800 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/typeCheck.py
--rw-r--r--   0 ultipa     (501) staff       (20)      233 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/password2md5.py
--rw-r--r--   0 ultipa     (501) staff       (20)     2547 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/convert.py
--rw-r--r--   0 ultipa     (501) staff       (20)      713 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/fileSize.py
--rw-r--r--   0 ultipa     (501) staff       (20)      139 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/__init__.py
--rw-r--r--   0 ultipa     (501) staff       (20)    48516 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/format.py
--rw-r--r--   0 ultipa     (501) staff       (20)      954 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/logger.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1463 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/ultipaSchedule.py
--rw-r--r--   0 ultipa     (501) staff       (20)    14874 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/uql_marker.py
--rw-r--r--   0 ultipa     (501) staff       (20)      353 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/common.py
--rw-r--r--   0 ultipa     (501) staff       (20)      581 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/checkStrTime.py
--rw-r--r--   0 ultipa     (501) staff       (20)      648 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/errors.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1585 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/privileges.py
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa/utils/ufilter/
--rw-r--r--   0 ultipa     (501) staff       (20)     3757 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/ufilter/ufilter.py
--rw-r--r--   0 ultipa     (501) staff       (20)        0 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/ufilter/__init__.py
--rw-r--r--   0 ultipa     (501) staff       (20)     4019 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/ufilter/new_ufilter.py
--rw-r--r--   0 ultipa     (501) staff       (20)     8636 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/ultipa_datetime.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1969 2023-03-08 10:23:17.000000 ultipa-4.2.4/ultipa/utils/ResposeFormat.py
--rw-r--r--   0 ultipa     (501) staff       (20)     1920 2023-03-08 10:31:04.000000 ultipa-4.2.4/PKG-INFO
-drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa.egg-info/
--rw-r--r--   0 ultipa     (501) staff       (20)     1920 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa.egg-info/PKG-INFO
--rw-r--r--   0 ultipa     (501) staff       (20)     2087 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa.egg-info/SOURCES.txt
--rw-r--r--   0 ultipa     (501) staff       (20)      181 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa.egg-info/requires.txt
--rw-r--r--   0 ultipa     (501) staff       (20)        7 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa.egg-info/top_level.txt
--rw-r--r--   0 ultipa     (501) staff       (20)        1 2023-03-08 10:31:04.000000 ultipa-4.2.4/ultipa.egg-info/dependency_links.txt
--rwxr-xr-x   0 ultipa     (501) staff       (20)     1869 2023-03-08 10:24:44.000000 ultipa-4.2.4/setup.py
--rw-r--r--   0 ultipa     (501) staff       (20)       38 2023-03-08 10:31:04.000000 ultipa-4.2.4/setup.cfg
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa/
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa/types/
+-rw-r--r--   0 ultipa     (501) staff       (20)     8452 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/types/types_response.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      206 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/types/__init__.py
+-rw-r--r--   0 ultipa     (501) staff       (20)    39899 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/types/types.py
+-rw-r--r--   0 ultipa     (501) staff       (20)    24089 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/types/types_request.py
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa/proto/
+-rw-r--r--   0 ultipa     (501) staff       (20)    28520 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/proto/ultipa_pb2_grpc.py
+-rw-r--r--   0 ultipa     (501) staff       (20)        0 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/proto/__init__.py
+-rw-r--r--   0 ultipa     (501) staff       (20)    42151 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/proto/ultipa_pb2.py
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa/connection/
+-rw-r--r--   0 ultipa     (501) staff       (20)     2116 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/download_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1836 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/searchAB_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1553 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/searchKhop_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     6540 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/task_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1750 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/nodeSpread_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     2635 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/truncate_extra.py
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa/connection/algo/
+-rw-r--r--   0 ultipa     (501) staff       (20)    13994 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/algo/algos_params.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     6715 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/algo/community_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)       63 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/algo/__init__.py
+-rw-r--r--   0 ultipa     (501) staff       (20)    16296 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/algo/algo_params4.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     4212 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/algo/embedding_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)    18755 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/algo/makeAlgoClass.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     8292 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/algo/algo_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1986 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/algo/degrees_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)       55 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/__init__.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1557 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/autoNet_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     6478 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/policy_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     3799 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/edge_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      386 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/export_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     2842 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/connection.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     6148 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/connectionPoolMaker.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     4639 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/property_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     3566 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/node_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     4137 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/schema_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     6164 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/user_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1408 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/lte_ufe_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)    53327 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/connection_base.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     3690 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/index_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     3189 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/graph_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1074 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/template_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1502 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/backup_data_extra.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      711 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/connection/connectionPool.py
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa/printer/
+-rw-r--r--   0 ultipa     (501) staff       (20)    10571 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/printer/prettyPrint.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      138 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/printer/__init__.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      370 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/__init__.py
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa/utils/
+-rw-r--r--   0 ultipa     (501) staff       (20)     8966 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/serialize.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1383 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/raftRetry.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     2800 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/typeCheck.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      233 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/password2md5.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     2547 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/convert.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      713 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/fileSize.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      139 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/__init__.py
+-rw-r--r--   0 ultipa     (501) staff       (20)    64510 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/format.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      954 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/logger.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1463 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/ultipaSchedule.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     2162 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/nullValue.py
+-rw-r--r--   0 ultipa     (501) staff       (20)    15253 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/uql_marker.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      353 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/common.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1054 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/propertyUtils.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      246 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/checkStrTime.py
+-rw-r--r--   0 ultipa     (501) staff       (20)      648 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/errors.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1585 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/privileges.py
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa/utils/ufilter/
+-rw-r--r--   0 ultipa     (501) staff       (20)     3757 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/ufilter/ufilter.py
+-rw-r--r--   0 ultipa     (501) staff       (20)        0 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/ufilter/__init__.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     4019 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/ufilter/new_ufilter.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     7205 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/ultipa_datetime.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1969 2023-05-15 08:46:03.000000 ultipa-4.3.0/ultipa/utils/ResposeFormat.py
+-rw-r--r--   0 ultipa     (501) staff       (20)     1921 2023-05-15 08:56:44.000000 ultipa-4.3.0/PKG-INFO
+drwxr-xr-x   0 ultipa     (501) staff       (20)        0 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa.egg-info/
+-rw-r--r--   0 ultipa     (501) staff       (20)     1921 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa.egg-info/PKG-INFO
+-rw-r--r--   0 ultipa     (501) staff       (20)     2182 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa.egg-info/SOURCES.txt
+-rw-r--r--   0 ultipa     (501) staff       (20)      181 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa.egg-info/requires.txt
+-rw-r--r--   0 ultipa     (501) staff       (20)        7 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa.egg-info/top_level.txt
+-rw-r--r--   0 ultipa     (501) staff       (20)        1 2023-05-15 08:56:44.000000 ultipa-4.3.0/ultipa.egg-info/dependency_links.txt
+-rwxr-xr-x   0 ultipa     (501) staff       (20)     1869 2023-05-15 08:49:20.000000 ultipa-4.3.0/setup.py
+-rw-r--r--   0 ultipa     (501) staff       (20)       38 2023-05-15 08:56:44.000000 ultipa-4.3.0/setup.cfg
```

### Comparing `ultipa-4.2.4/ultipa/types/types_response.py` & `ultipa-4.3.0/ultipa/types/types_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Dict
 
 from ultipa.printer.prettyPrint import PrettyPrint, PrettyTable
 from ultipa.types.types import BaseModel, Node, Edge, DataItem, Status, \
-	UltipaStatistics, Schema, ReturnReq, BaseUqlReply, ResultType, ResultAlias, PlanNodeType, ExplainPlan
+	UltipaStatistics, Schema, ReturnReq, BaseUqlReply, ResultType, ResultAlias, ExplainPlan
 from ultipa.utils.convert import Any
 
 
 class Property(BaseModel):
 	lte: bool
 	index: bool
 	propertyName: str
@@ -111,16 +111,16 @@
 
 			elif dataItem.type == ResultType.getTypeStr(ResultType.RESULT_TYPE_PATH):
 				pretty.prettyPath(dataItem)
 
 			elif dataItem.type == ResultType.getTypeStr(ResultType.RESULT_TYPE_ATTR):
 				pretty.prettyAttr(dataItem)
 
-			elif dataItem.type == ResultType.getTypeStr(ResultType.RESULT_TYPE_ARRAY):
-				pretty.prettyArray(dataItem)
+			# elif dataItem.type == ResultType.getTypeStr(ResultType.RESULT_TYPE_ARRAY):
+			# 	pretty.prettyArray(dataItem)
 
 		if self.explainPlan:
 			for explan in self.explainPlan:
 				explains.append(explan)
 			if explains:
 				pretty.prettyTree(explains)
 
@@ -417,7 +417,9 @@
 
 class ResponseStat(Response):
 	data: Stat
 
 
 class ResponseExport(Response):
 	data: List[Node]
+
+
```

### Comparing `ultipa-4.2.4/ultipa/types/types.py` & `ultipa-4.3.0/ultipa/types/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 	PROPERTY_DOUBLE = 'double'
 	PROPERTY_UINT32 = 'uint32'
 	PROPERTY_INT64 = 'int64'
 	PROPERTY_UINT64 = 'uint64'
 	PROPERTY_DATETIME = 'datetime'
 	PROPERTY_TIMESTAMP = 'timestamp'
 	PROPERTY_TEXT = 'text'
+	PROPERTY_UNSET = "unset"
+	PROPERTY_POINT = "point"
+	PROPERTY_DECIMAL = "decimal"
+	PROPERTY_LIST = "list"
+	PROPERTY_SET = "set"
+	PROPERTY_MAP = "map"
 
 
 # PROPERTY_BLOB = 'BLOB'
 
 
 class TaskStatus:
 	TASK_WAITING = 0
@@ -79,15 +85,21 @@
 	PROPERTY_DOUBLE = ultipa_pb2.DOUBLE
 	PROPERTY_UINT32 = ultipa_pb2.UINT32
 	PROPERTY_INT64 = ultipa_pb2.INT64
 	PROPERTY_UINT64 = ultipa_pb2.UINT64
 	PROPERTY_DATETIME = ultipa_pb2.DATETIME
 	PROPERTY_TIMESTAMP = ultipa_pb2.TIMESTAMP
 	PROPERTY_TEXT = ultipa_pb2.TEXT
-	# PROPERTY_BLOB = ultipa_pb2.BLOB
+	PROPERTY_BLOB = ultipa_pb2.BLOB
+	PROPERTY_POINT = ultipa_pb2.POINT
+	PROPERTY_DECIMAL = ultipa_pb2.DECIMAL
+	PROPERTY_LIST = ultipa_pb2.LIST
+	PROPERTY_SET = ultipa_pb2.SET
+	PROPERTY_MAP = ultipa_pb2.MAP
+	PROPERTY_NULL = ultipa_pb2.NULL_
 	PROPERTY_UUID = -1
 	PROPERTY_ID = -2
 	PROPERTY_FROM = -3
 	PROPERTY_FROM_UUID = -4
 	PROPERTY_TO = -5
 	PROPERTY_TO_UUID = -6
 	PROPERTY_IGNORE = -7
@@ -95,30 +107,30 @@
 
 class ResultType:
 	RESULT_TYPE_UNSET = ultipa_pb2.RESULT_TYPE_UNSET
 	RESULT_TYPE_PATH = ultipa_pb2.RESULT_TYPE_PATH
 	RESULT_TYPE_NODE = ultipa_pb2.RESULT_TYPE_NODE
 	RESULT_TYPE_EDGE = ultipa_pb2.RESULT_TYPE_EDGE
 	RESULT_TYPE_ATTR = ultipa_pb2.RESULT_TYPE_ATTR
-	RESULT_TYPE_ARRAY = ultipa_pb2.RESULT_TYPE_ARRAY
+	# RESULT_TYPE_ARRAY = ultipa_pb2.RESULT_TYPE_ARRAY
 	RESULT_TYPE_TABLE = ultipa_pb2.RESULT_TYPE_TABLE
 	RESULT_TYPE_ExplainPlan = "ExplainPlan"
 
 	@staticmethod
 	def getTypeStr(type):
 		if type == ResultType.RESULT_TYPE_PATH:
 			return 'PATH'
 		elif type == ResultType.RESULT_TYPE_NODE:
 			return 'NODE'
 		elif type == ResultType.RESULT_TYPE_EDGE:
 			return "EDGE"
 		elif type == ResultType.RESULT_TYPE_ATTR:
 			return "ATTR"
-		elif type == ResultType.RESULT_TYPE_ARRAY:
-			return "ARRAY"
+		elif type == PropertyType.PROPERTY_LIST:
+			return "LIST"
 		elif type == ResultType.RESULT_TYPE_TABLE:
 			return "TABLE"
 		elif type == ResultType.RESULT_TYPE_UNSET:
 			return "UNSET"
 		elif type == ResultType.RESULT_TYPE_ExplainPlan:
 			return "EXPLAINPLAN"
 		else:
@@ -151,248 +163,249 @@
 
 
 class ServerStatus:
 	DEAD = ultipa_pb2.DEAD
 	ALIVE = ultipa_pb2.ALIVE
 
 
-class PlanNodeType:
-	CLAUSE_UNSET = ultipa_pb2.CLAUSE_UNSET
-	ORDER_BY_CLAUSE = ultipa_pb2.ORDER_BY_CLAUSE
-	AGGREGATION_CLAUSE = ultipa_pb2.AGGREGATION_CLAUSE
-	WITH_CLAUSE = ultipa_pb2.WITH_CLAUSE
-	WHERE_CLAUSE = ultipa_pb2.WHERE_CLAUSE
-	UNCOLLECT_CLAUSE = ultipa_pb2.UNCOLLECT_CLAUSE
-	TABLE_CLAUSE = ultipa_pb2.TABLE_CLAUSE
-	RETURN_CLAUSE = ultipa_pb2.RETURN_CLAUSE
-	LIMIT_SKIP_CLAUSE = ultipa_pb2.LIMIT_SKIP_CLAUSE
-	TEMPLATE_CLAUSE = ultipa_pb2.TEMPLATE_CLAUSE
-	KHOP_TEMPLATE_CLAUSE = ultipa_pb2.KHOP_TEMPLATE_CLAUSE
-	KHOP_CLAUSE = ultipa_pb2.KHOP_CLAUSE
-	AB_CLAUSE = ultipa_pb2.AB_CLAUSE
-	SPREAD_CLAUSE = ultipa_pb2.SPREAD_CLAUSE
-	AUTO_NET_CLAUSE = ultipa_pb2.AUTO_NET_CLAUSE
-	NODE_SEARCH_CLAUSE = ultipa_pb2.NODE_SEARCH_CLAUSE
-	EDGE_SEARCH_CLAUSE = ultipa_pb2.EDGE_SEARCH_CLAUSE
-	NODE_INSERT_CLAUSE = ultipa_pb2.NODE_INSERT_CLAUSE
-	EDGE_INSERT_CLAUSE = ultipa_pb2.EDGE_INSERT_CLAUSE
-	NODE_UPSERT_CLAUSE = ultipa_pb2.NODE_UPSERT_CLAUSE
-	EDGE_UPSERT_CLAUSE = ultipa_pb2.EDGE_UPSERT_CLAUSE
-	NODE_UPDATE_CLAUSE = ultipa_pb2.NODE_UPDATE_CLAUSE
-	EDGE_UPDATE_CLAUSE = ultipa_pb2.EDGE_UPDATE_CLAUSE
-	NODE_DELETE_CLAUSE = ultipa_pb2.NODE_DELETE_CLAUSE
-	EDGE_DELETE_CLAUSE = ultipa_pb2.EDGE_DELETE_CLAUSE
-	TRUNCATE_CLAUSE = ultipa_pb2.TRUNCATE_CLAUSE
-	COMPACT_CLAUSE = ultipa_pb2.COMPACT_CLAUSE
-	GRAPH_CREATE_CLAUSE = ultipa_pb2.GRAPH_CREATE_CLAUSE
-	GRAPH_DROP_CLAUSE = ultipa_pb2.GRAPH_DROP_CLAUSE
-	GRAPH_UPDATE_CLAUSE = ultipa_pb2.GRAPH_UPDATE_CLAUSE
-	GRAPH_SHOW_CLAUSE = ultipa_pb2.GRAPH_SHOW_CLAUSE
-	GRAPH_MOUNT_CLAUSE = ultipa_pb2.GRAPH_MOUNT_CLAUSE
-	GRAPH_UNMOUNT_CLAUSE = ultipa_pb2.GRAPH_UNMOUNT_CLAUSE
-	SCHEMA_CREATE_CLAUSE = ultipa_pb2.SCHEMA_CREATE_CLAUSE
-	SCHEMA_DROP_CLAUSE = ultipa_pb2.SCHEMA_DROP_CLAUSE
-	SCHEMA_ALTER_CLAUSE = ultipa_pb2.SCHEMA_ALTER_CLAUSE
-	SCHEMA_SHOW_CLAUSE = ultipa_pb2.SCHEMA_SHOW_CLAUSE
-	PROPERTY_CREATE_CLAUSE = ultipa_pb2.PROPERTY_CREATE_CLAUSE
-	PROPERTY_DROP_CLAUSE = ultipa_pb2.PROPERTY_DROP_CLAUSE
-	PROPERTY_ALTER_CLAUSE = ultipa_pb2.PROPERTY_ALTER_CLAUSE
-	PROPERTY_SHOW_CLAUSE = ultipa_pb2.PROPERTY_SHOW_CLAUSE
-	FULLTEXT_CREATE_CLAUSE = ultipa_pb2.FULLTEXT_CREATE_CLAUSE
-	FULLTEXT_DROP_CLAUSE = ultipa_pb2.FULLTEXT_DROP_CLAUSE
-	FULLTEXT_SHOW_CLAUSE = ultipa_pb2.FULLTEXT_SHOW_CLAUSE
-	INDEX_CREATE_CLAUSE = ultipa_pb2.INDEX_CREATE_CLAUSE
-	INDEX_DROP_CLAUSE = ultipa_pb2.INDEX_DROP_CLAUSE
-	INDEX_SHOW_CLAUSE = ultipa_pb2.INDEX_SHOW_CLAUSE
-	LTE_CLAUSE = ultipa_pb2.LTE_CLAUSE
-	UFE_CLAUSE = ultipa_pb2.UFE_CLAUSE
-	TASK_CLEAR_CLAUSE = ultipa_pb2.TASK_CLEAR_CLAUSE
-	TASK_STOP_CLAUSE = ultipa_pb2.TASK_STOP_CLAUSE
-	TASK_PAUSE_CLAUSE = ultipa_pb2.TASK_PAUSE_CLAUSE
-	TASK_RESUME_CLAUSE = ultipa_pb2.TASK_RESUME_CLAUSE
-	TASK_SHOW_CLAUSE = ultipa_pb2.TASK_SHOW_CLAUSE
-	TOP_CLAUSE = ultipa_pb2.TOP_CLAUSE
-	KILL_CLAUSE = ultipa_pb2.KILL_CLAUSE
-	STAT_CLAUSE = ultipa_pb2.STAT_CLAUSE
-	POLICY_SHOW_CLAUSE = ultipa_pb2.POLICY_SHOW_CLAUSE
-	POLICY_CREATE_CLAUSE = ultipa_pb2.POLICY_CREATE_CLAUSE
-	POLICY_DELETE_CLAUSE = ultipa_pb2.POLICY_DELETE_CLAUSE
-	POLICY_UPDATE_CLAUSE = ultipa_pb2.POLICY_UPDATE_CLAUSE
-	USER_SHOW_CLAUSE = ultipa_pb2.USER_SHOW_CLAUSE
-	USER_CREATE_CLAUSE = ultipa_pb2.USER_CREATE_CLAUSE
-	USER_DELETE_CLAUSE = ultipa_pb2.USER_DELETE_CLAUSE
-	USER_UPDATE_CLAUSE = ultipa_pb2.USER_UPDATE_CLAUSE
-	PRIVILEGE_SHOW_CLAUSE = ultipa_pb2.PRIVILEGE_SHOW_CLAUSE
-	GRANT_CLAUSE = ultipa_pb2.GRANT_CLAUSE
-	REVOKE_CLAUSE = ultipa_pb2.REVOKE_CLAUSE
-	SELF_INFO_GET_CLAUSE = ultipa_pb2.SELF_INFO_GET_CLAUSE
-	ALGO_CLAUSE = ultipa_pb2.ALGO_CLAUSE
-	ALGO_WRITE_CLAUSE = ultipa_pb2.ALGO_WRITE_CLAUSE
-	ALGO_LIST_CLAUSE = ultipa_pb2.ALGO_LIST_CLAUSE
-	SUB_GRAPH_CLAUSE = ultipa_pb2.SUB_GRAPH_CLAUSE
-	OPTIONAL_TEMPLATE_CLAUSE = ultipa_pb2.OPTIONAL_TEMPLATE_CLAUSE
-	SUBQUERY_CLAUSE = ultipa_pb2.SUBQUERY_CLAUSE
-	UNION_CLAUSE = ultipa_pb2.UNION_CLAUSE
-
-	@staticmethod
-	def getTypeStr(type):
-		if type == PlanNodeType.CLAUSE_UNSET:
-			return 'CLAUSE_UNSET'
-		elif type == PlanNodeType.ORDER_BY_CLAUSE:
-			return 'ORDER_BY_CLAUSE'
-		elif type == PlanNodeType.AGGREGATION_CLAUSE:
-			return "AGGREGATION_CLAUSE"
-		elif type == PlanNodeType.WITH_CLAUSE:
-			return "WITH_CLAUSE"
-		elif type == PlanNodeType.WHERE_CLAUSE:
-			return "WHERE_CLAUSE"
-		elif type == PlanNodeType.UNCOLLECT_CLAUSE:
-			return "UNCOLLECT_CLAUSE"
-		elif type == PlanNodeType.TABLE_CLAUSE:
-			return "TABLE_CLAUSE"
-		elif type == PlanNodeType.RETURN_CLAUSE:
-			return "RETURN_CLAUSE"
-		elif type == PlanNodeType.LIMIT_SKIP_CLAUSE:
-			return "LIMIT_SKIP_CLAUSE"
-		elif type == PlanNodeType.TEMPLATE_CLAUSE:
-			return "TEMPLATE_CLAUSE"
-		elif type == PlanNodeType.KHOP_TEMPLATE_CLAUSE:
-			return "KHOP_TEMPLATE_CLAUSE"
-		elif type == PlanNodeType.KHOP_CLAUSE:
-			return 'KHOP_CLAUSE'
-		elif type == PlanNodeType.AB_CLAUSE:
-			return "AB_CLAUSE"
-		elif type == PlanNodeType.SPREAD_CLAUSE:
-			return "SPREAD_CLAUSE"
-		elif type == PlanNodeType.AUTO_NET_CLAUSE:
-			return "AUTO_NET_CLAUSE"
-		elif type == PlanNodeType.NODE_SEARCH_CLAUSE:
-			return "NODE_SEARCH_CLAUSE"
-		elif type == PlanNodeType.NODE_INSERT_CLAUSE:
-			return "NODE_INSERT_CLAUSE"
-		elif type == PlanNodeType.NODE_UPSERT_CLAUSE:
-			return "NODE_UPSERT_CLAUSE"
-		elif type == PlanNodeType.NODE_UPDATE_CLAUSE:
-			return "NODE_UPDATE_CLAUSE"
-		elif type == PlanNodeType.NODE_DELETE_CLAUSE:
-			return "NODE_DELETE_CLAUSE"
-		elif type == PlanNodeType.EDGE_SEARCH_CLAUSE:
-			return "EDGE_SEARCH_CLAUSE"
-		elif type == PlanNodeType.EDGE_INSERT_CLAUSE:
-			return 'EDGE_INSERT_CLAUSE'
-		elif type == PlanNodeType.EDGE_UPSERT_CLAUSE:
-			return "EDGE_UPSERT_CLAUSE"
-		elif type == PlanNodeType.EDGE_UPDATE_CLAUSE:
-			return "EDGE_UPDATE_CLAUSE"
-		elif type == PlanNodeType.EDGE_DELETE_CLAUSE:
-			return "EDGE_DELETE_CLAUSE"
-		elif type == PlanNodeType.TRUNCATE_CLAUSE:
-			return "TRUNCATE_CLAUSE"
-		elif type == PlanNodeType.COMPACT_CLAUSE:
-			return "COMPACT_CLAUSE"
-		elif type == PlanNodeType.GRAPH_SHOW_CLAUSE:
-			return "GRAPH_SHOW_CLAUSE"
-		elif type == PlanNodeType.GRAPH_CREATE_CLAUSE:
-			return "GRAPH_CREATE_CLAUSE"
-		elif type == PlanNodeType.GRAPH_DROP_CLAUSE:
-			return "GRAPH_DROP_CLAUSE"
-		elif type == PlanNodeType.GRAPH_UPDATE_CLAUSE:
-			return "GRAPH_UPDATE_CLAUSE"
-		elif type == PlanNodeType.GRAPH_MOUNT_CLAUSE:
-			return 'GRAPH_MOUNT_CLAUSE'
-		elif type == PlanNodeType.GRAPH_UNMOUNT_CLAUSE:
-			return "GRAPH_UNMOUNT_CLAUSE"
-		elif type == PlanNodeType.SCHEMA_CREATE_CLAUSE:
-			return "SCHEMA_CREATE_CLAUSE"
-		elif type == PlanNodeType.SCHEMA_DROP_CLAUSE:
-			return "SCHEMA_DROP_CLAUSE"
-		elif type == PlanNodeType.SCHEMA_ALTER_CLAUSE:
-			return "SCHEMA_ALTER_CLAUSE"
-		elif type == PlanNodeType.SCHEMA_SHOW_CLAUSE:
-			return "SCHEMA_SHOW_CLAUSE"
-		elif type == PlanNodeType.PROPERTY_CREATE_CLAUSE:
-			return "PROPERTY_CREATE_CLAUSE"
-		elif type == PlanNodeType.PROPERTY_DROP_CLAUSE:
-			return "PROPERTY_DROP_CLAUSE"
-		elif type == PlanNodeType.PROPERTY_ALTER_CLAUSE:
-			return "PROPERTY_ALTER_CLAUSE"
-		elif type == PlanNodeType.PROPERTY_SHOW_CLAUSE:
-			return "PROPERTY_SHOW_CLAUSE"
-		elif type == PlanNodeType.FULLTEXT_CREATE_CLAUSE:
-			return 'FULLTEXT_CREATE_CLAUSE'
-		elif type == PlanNodeType.FULLTEXT_DROP_CLAUSE:
-			return "FULLTEXT_DROP_CLAUSE"
-		elif type == PlanNodeType.FULLTEXT_SHOW_CLAUSE:
-			return "FULLTEXT_SHOW_CLAUSE"
-		elif type == PlanNodeType.INDEX_CREATE_CLAUSE:
-			return "INDEX_CREATE_CLAUSE"
-		elif type == PlanNodeType.INDEX_DROP_CLAUSE:
-			return "INDEX_DROP_CLAUSE"
-		elif type == PlanNodeType.INDEX_SHOW_CLAUSE:
-			return "INDEX_SHOW_CLAUSE"
-		elif type == PlanNodeType.LTE_CLAUSE:
-			return "LTE_CLAUSE"
-		elif type == PlanNodeType.UFE_CLAUSE:
-			return "UFE_CLAUSE"
-		elif type == PlanNodeType.TASK_CLEAR_CLAUSE:
-			return "TASK_CLEAR_CLAUSE"
-		elif type == PlanNodeType.TASK_STOP_CLAUSE:
-			return "TASK_STOP_CLAUSE"
-		elif type == PlanNodeType.TASK_PAUSE_CLAUSE:
-			return 'TASK_PAUSE_CLAUSE'
-		elif type == PlanNodeType.TASK_RESUME_CLAUSE:
-			return "TASK_RESUME_CLAUSE"
-		elif type == PlanNodeType.TASK_SHOW_CLAUSE:
-			return "TASK_SHOW_CLAUSE"
-		elif type == PlanNodeType.TOP_CLAUSE:
-			return "TOP_CLAUSE"
-		elif type == PlanNodeType.KILL_CLAUSE:
-			return "KILL_CLAUSE"
-		elif type == PlanNodeType.STAT_CLAUSE:
-			return "STAT_CLAUSE"
-		elif type == PlanNodeType.POLICY_SHOW_CLAUSE:
-			return "POLICY_SHOW_CLAUSE"
-		elif type == PlanNodeType.POLICY_CREATE_CLAUSE:
-			return "POLICY_CREATE_CLAUSE"
-		elif type == PlanNodeType.POLICY_DELETE_CLAUSE:
-			return "POLICY_DELETE_CLAUSE"
-		elif type == PlanNodeType.POLICY_UPDATE_CLAUSE:
-			return "POLICY_UPDATE_CLAUSE"
-		elif type == PlanNodeType.USER_SHOW_CLAUSE:
-			return 'USER_SHOW_CLAUSE'
-		elif type == PlanNodeType.USER_CREATE_CLAUSE:
-			return "USER_CREATE_CLAUSE"
-		elif type == PlanNodeType.USER_DELETE_CLAUSE:
-			return "USER_DELETE_CLAUSE"
-		elif type == PlanNodeType.USER_UPDATE_CLAUSE:
-			return "USER_UPDATE_CLAUSE"
-		elif type == PlanNodeType.PRIVILEGE_SHOW_CLAUSE:
-			return "PRIVILEGE_SHOW_CLAUSE"
-		elif type == PlanNodeType.GRANT_CLAUSE:
-			return "GRANT_CLAUSE"
-		elif type == PlanNodeType.REVOKE_CLAUSE:
-			return "REVOKE_CLAUSE"
-		elif type == PlanNodeType.SELF_INFO_GET_CLAUSE:
-			return "SELF_INFO_GET_CLAUSE"
-		elif type == PlanNodeType.ALGO_CLAUSE:
-			return "ALGO_CLAUSE"
-		elif type == PlanNodeType.ALGO_WRITE_CLAUSE:
-			return "ALGO_WRITE_CLAUSE"
-		elif type == PlanNodeType.ALGO_LIST_CLAUSE:
-			return 'ALGO_LIST_CLAUSE'
-		elif type == PlanNodeType.SUB_GRAPH_CLAUSE:
-			return "SUB_GRAPH_CLAUSE"
-		elif type == PlanNodeType.OPTIONAL_TEMPLATE_CLAUSE:
-			return "OPTIONAL_TEMPLATE_CLAUSE"
-		elif type == PlanNodeType.SUBQUERY_CLAUSE:
-			return "SUBQUERY_CLAUSE"
-		elif type == PlanNodeType.UNION_CLAUSE:
-			return "UNION_CLAUSE"
-		else:
-			return type
+#
+# class PlanNodeType:
+# 	CLAUSE_UNSET = ultipa_pb2.CLAUSE_UNSET
+# 	ORDER_BY_CLAUSE = ultipa_pb2.ORDER_BY_CLAUSE
+# 	AGGREGATION_CLAUSE = ultipa_pb2.AGGREGATION_CLAUSE
+# 	WITH_CLAUSE = ultipa_pb2.WITH_CLAUSE
+# 	WHERE_CLAUSE = ultipa_pb2.WHERE_CLAUSE
+# 	UNCOLLECT_CLAUSE = ultipa_pb2.UNCOLLECT_CLAUSE
+# 	TABLE_CLAUSE = ultipa_pb2.TABLE_CLAUSE
+# 	RETURN_CLAUSE = ultipa_pb2.RETURN_CLAUSE
+# 	LIMIT_SKIP_CLAUSE = ultipa_pb2.LIMIT_SKIP_CLAUSE
+# 	TEMPLATE_CLAUSE = ultipa_pb2.TEMPLATE_CLAUSE
+# 	KHOP_TEMPLATE_CLAUSE = ultipa_pb2.KHOP_TEMPLATE_CLAUSE
+# 	KHOP_CLAUSE = ultipa_pb2.KHOP_CLAUSE
+# 	AB_CLAUSE = ultipa_pb2.AB_CLAUSE
+# 	SPREAD_CLAUSE = ultipa_pb2.SPREAD_CLAUSE
+# 	AUTO_NET_CLAUSE = ultipa_pb2.AUTO_NET_CLAUSE
+# 	NODE_SEARCH_CLAUSE = ultipa_pb2.NODE_SEARCH_CLAUSE
+# 	EDGE_SEARCH_CLAUSE = ultipa_pb2.EDGE_SEARCH_CLAUSE
+# 	NODE_INSERT_CLAUSE = ultipa_pb2.NODE_INSERT_CLAUSE
+# 	EDGE_INSERT_CLAUSE = ultipa_pb2.EDGE_INSERT_CLAUSE
+# 	NODE_UPSERT_CLAUSE = ultipa_pb2.NODE_UPSERT_CLAUSE
+# 	EDGE_UPSERT_CLAUSE = ultipa_pb2.EDGE_UPSERT_CLAUSE
+# 	NODE_UPDATE_CLAUSE = ultipa_pb2.NODE_UPDATE_CLAUSE
+# 	EDGE_UPDATE_CLAUSE = ultipa_pb2.EDGE_UPDATE_CLAUSE
+# 	NODE_DELETE_CLAUSE = ultipa_pb2.NODE_DELETE_CLAUSE
+# 	EDGE_DELETE_CLAUSE = ultipa_pb2.EDGE_DELETE_CLAUSE
+# 	TRUNCATE_CLAUSE = ultipa_pb2.TRUNCATE_CLAUSE
+# 	COMPACT_CLAUSE = ultipa_pb2.COMPACT_CLAUSE
+# 	GRAPH_CREATE_CLAUSE = ultipa_pb2.GRAPH_CREATE_CLAUSE
+# 	GRAPH_DROP_CLAUSE = ultipa_pb2.GRAPH_DROP_CLAUSE
+# 	GRAPH_UPDATE_CLAUSE = ultipa_pb2.GRAPH_UPDATE_CLAUSE
+# 	GRAPH_SHOW_CLAUSE = ultipa_pb2.GRAPH_SHOW_CLAUSE
+# 	GRAPH_MOUNT_CLAUSE = ultipa_pb2.GRAPH_MOUNT_CLAUSE
+# 	GRAPH_UNMOUNT_CLAUSE = ultipa_pb2.GRAPH_UNMOUNT_CLAUSE
+# 	SCHEMA_CREATE_CLAUSE = ultipa_pb2.SCHEMA_CREATE_CLAUSE
+# 	SCHEMA_DROP_CLAUSE = ultipa_pb2.SCHEMA_DROP_CLAUSE
+# 	SCHEMA_ALTER_CLAUSE = ultipa_pb2.SCHEMA_ALTER_CLAUSE
+# 	SCHEMA_SHOW_CLAUSE = ultipa_pb2.SCHEMA_SHOW_CLAUSE
+# 	PROPERTY_CREATE_CLAUSE = ultipa_pb2.PROPERTY_CREATE_CLAUSE
+# 	PROPERTY_DROP_CLAUSE = ultipa_pb2.PROPERTY_DROP_CLAUSE
+# 	PROPERTY_ALTER_CLAUSE = ultipa_pb2.PROPERTY_ALTER_CLAUSE
+# 	PROPERTY_SHOW_CLAUSE = ultipa_pb2.PROPERTY_SHOW_CLAUSE
+# 	FULLTEXT_CREATE_CLAUSE = ultipa_pb2.FULLTEXT_CREATE_CLAUSE
+# 	FULLTEXT_DROP_CLAUSE = ultipa_pb2.FULLTEXT_DROP_CLAUSE
+# 	FULLTEXT_SHOW_CLAUSE = ultipa_pb2.FULLTEXT_SHOW_CLAUSE
+# 	INDEX_CREATE_CLAUSE = ultipa_pb2.INDEX_CREATE_CLAUSE
+# 	INDEX_DROP_CLAUSE = ultipa_pb2.INDEX_DROP_CLAUSE
+# 	INDEX_SHOW_CLAUSE = ultipa_pb2.INDEX_SHOW_CLAUSE
+# 	LTE_CLAUSE = ultipa_pb2.LTE_CLAUSE
+# 	UFE_CLAUSE = ultipa_pb2.UFE_CLAUSE
+# 	TASK_CLEAR_CLAUSE = ultipa_pb2.TASK_CLEAR_CLAUSE
+# 	TASK_STOP_CLAUSE = ultipa_pb2.TASK_STOP_CLAUSE
+# 	TASK_PAUSE_CLAUSE = ultipa_pb2.TASK_PAUSE_CLAUSE
+# 	TASK_RESUME_CLAUSE = ultipa_pb2.TASK_RESUME_CLAUSE
+# 	TASK_SHOW_CLAUSE = ultipa_pb2.TASK_SHOW_CLAUSE
+# 	TOP_CLAUSE = ultipa_pb2.TOP_CLAUSE
+# 	KILL_CLAUSE = ultipa_pb2.KILL_CLAUSE
+# 	STAT_CLAUSE = ultipa_pb2.STAT_CLAUSE
+# 	POLICY_SHOW_CLAUSE = ultipa_pb2.POLICY_SHOW_CLAUSE
+# 	POLICY_CREATE_CLAUSE = ultipa_pb2.POLICY_CREATE_CLAUSE
+# 	POLICY_DELETE_CLAUSE = ultipa_pb2.POLICY_DELETE_CLAUSE
+# 	POLICY_UPDATE_CLAUSE = ultipa_pb2.POLICY_UPDATE_CLAUSE
+# 	USER_SHOW_CLAUSE = ultipa_pb2.USER_SHOW_CLAUSE
+# 	USER_CREATE_CLAUSE = ultipa_pb2.USER_CREATE_CLAUSE
+# 	USER_DELETE_CLAUSE = ultipa_pb2.USER_DELETE_CLAUSE
+# 	USER_UPDATE_CLAUSE = ultipa_pb2.USER_UPDATE_CLAUSE
+# 	PRIVILEGE_SHOW_CLAUSE = ultipa_pb2.PRIVILEGE_SHOW_CLAUSE
+# 	GRANT_CLAUSE = ultipa_pb2.GRANT_CLAUSE
+# 	REVOKE_CLAUSE = ultipa_pb2.REVOKE_CLAUSE
+# 	SELF_INFO_GET_CLAUSE = ultipa_pb2.SELF_INFO_GET_CLAUSE
+# 	ALGO_CLAUSE = ultipa_pb2.ALGO_CLAUSE
+# 	ALGO_WRITE_CLAUSE = ultipa_pb2.ALGO_WRITE_CLAUSE
+# 	ALGO_LIST_CLAUSE = ultipa_pb2.ALGO_LIST_CLAUSE
+# 	SUB_GRAPH_CLAUSE = ultipa_pb2.SUB_GRAPH_CLAUSE
+# 	OPTIONAL_TEMPLATE_CLAUSE = ultipa_pb2.OPTIONAL_TEMPLATE_CLAUSE
+# 	SUBQUERY_CLAUSE = ultipa_pb2.SUBQUERY_CLAUSE
+# 	UNION_CLAUSE = ultipa_pb2.UNION_CLAUSE
+#
+# 	@staticmethod
+# 	def getTypeStr(type):
+# 		if type == PlanNodeType.CLAUSE_UNSET:
+# 			return 'CLAUSE_UNSET'
+# 		elif type == PlanNodeType.ORDER_BY_CLAUSE:
+# 			return 'ORDER_BY_CLAUSE'
+# 		elif type == PlanNodeType.AGGREGATION_CLAUSE:
+# 			return "AGGREGATION_CLAUSE"
+# 		elif type == PlanNodeType.WITH_CLAUSE:
+# 			return "WITH_CLAUSE"
+# 		elif type == PlanNodeType.WHERE_CLAUSE:
+# 			return "WHERE_CLAUSE"
+# 		elif type == PlanNodeType.UNCOLLECT_CLAUSE:
+# 			return "UNCOLLECT_CLAUSE"
+# 		elif type == PlanNodeType.TABLE_CLAUSE:
+# 			return "TABLE_CLAUSE"
+# 		elif type == PlanNodeType.RETURN_CLAUSE:
+# 			return "RETURN_CLAUSE"
+# 		elif type == PlanNodeType.LIMIT_SKIP_CLAUSE:
+# 			return "LIMIT_SKIP_CLAUSE"
+# 		elif type == PlanNodeType.TEMPLATE_CLAUSE:
+# 			return "TEMPLATE_CLAUSE"
+# 		elif type == PlanNodeType.KHOP_TEMPLATE_CLAUSE:
+# 			return "KHOP_TEMPLATE_CLAUSE"
+# 		elif type == PlanNodeType.KHOP_CLAUSE:
+# 			return 'KHOP_CLAUSE'
+# 		elif type == PlanNodeType.AB_CLAUSE:
+# 			return "AB_CLAUSE"
+# 		elif type == PlanNodeType.SPREAD_CLAUSE:
+# 			return "SPREAD_CLAUSE"
+# 		elif type == PlanNodeType.AUTO_NET_CLAUSE:
+# 			return "AUTO_NET_CLAUSE"
+# 		elif type == PlanNodeType.NODE_SEARCH_CLAUSE:
+# 			return "NODE_SEARCH_CLAUSE"
+# 		elif type == PlanNodeType.NODE_INSERT_CLAUSE:
+# 			return "NODE_INSERT_CLAUSE"
+# 		elif type == PlanNodeType.NODE_UPSERT_CLAUSE:
+# 			return "NODE_UPSERT_CLAUSE"
+# 		elif type == PlanNodeType.NODE_UPDATE_CLAUSE:
+# 			return "NODE_UPDATE_CLAUSE"
+# 		elif type == PlanNodeType.NODE_DELETE_CLAUSE:
+# 			return "NODE_DELETE_CLAUSE"
+# 		elif type == PlanNodeType.EDGE_SEARCH_CLAUSE:
+# 			return "EDGE_SEARCH_CLAUSE"
+# 		elif type == PlanNodeType.EDGE_INSERT_CLAUSE:
+# 			return 'EDGE_INSERT_CLAUSE'
+# 		elif type == PlanNodeType.EDGE_UPSERT_CLAUSE:
+# 			return "EDGE_UPSERT_CLAUSE"
+# 		elif type == PlanNodeType.EDGE_UPDATE_CLAUSE:
+# 			return "EDGE_UPDATE_CLAUSE"
+# 		elif type == PlanNodeType.EDGE_DELETE_CLAUSE:
+# 			return "EDGE_DELETE_CLAUSE"
+# 		elif type == PlanNodeType.TRUNCATE_CLAUSE:
+# 			return "TRUNCATE_CLAUSE"
+# 		elif type == PlanNodeType.COMPACT_CLAUSE:
+# 			return "COMPACT_CLAUSE"
+# 		elif type == PlanNodeType.GRAPH_SHOW_CLAUSE:
+# 			return "GRAPH_SHOW_CLAUSE"
+# 		elif type == PlanNodeType.GRAPH_CREATE_CLAUSE:
+# 			return "GRAPH_CREATE_CLAUSE"
+# 		elif type == PlanNodeType.GRAPH_DROP_CLAUSE:
+# 			return "GRAPH_DROP_CLAUSE"
+# 		elif type == PlanNodeType.GRAPH_UPDATE_CLAUSE:
+# 			return "GRAPH_UPDATE_CLAUSE"
+# 		elif type == PlanNodeType.GRAPH_MOUNT_CLAUSE:
+# 			return 'GRAPH_MOUNT_CLAUSE'
+# 		elif type == PlanNodeType.GRAPH_UNMOUNT_CLAUSE:
+# 			return "GRAPH_UNMOUNT_CLAUSE"
+# 		elif type == PlanNodeType.SCHEMA_CREATE_CLAUSE:
+# 			return "SCHEMA_CREATE_CLAUSE"
+# 		elif type == PlanNodeType.SCHEMA_DROP_CLAUSE:
+# 			return "SCHEMA_DROP_CLAUSE"
+# 		elif type == PlanNodeType.SCHEMA_ALTER_CLAUSE:
+# 			return "SCHEMA_ALTER_CLAUSE"
+# 		elif type == PlanNodeType.SCHEMA_SHOW_CLAUSE:
+# 			return "SCHEMA_SHOW_CLAUSE"
+# 		elif type == PlanNodeType.PROPERTY_CREATE_CLAUSE:
+# 			return "PROPERTY_CREATE_CLAUSE"
+# 		elif type == PlanNodeType.PROPERTY_DROP_CLAUSE:
+# 			return "PROPERTY_DROP_CLAUSE"
+# 		elif type == PlanNodeType.PROPERTY_ALTER_CLAUSE:
+# 			return "PROPERTY_ALTER_CLAUSE"
+# 		elif type == PlanNodeType.PROPERTY_SHOW_CLAUSE:
+# 			return "PROPERTY_SHOW_CLAUSE"
+# 		elif type == PlanNodeType.FULLTEXT_CREATE_CLAUSE:
+# 			return 'FULLTEXT_CREATE_CLAUSE'
+# 		elif type == PlanNodeType.FULLTEXT_DROP_CLAUSE:
+# 			return "FULLTEXT_DROP_CLAUSE"
+# 		elif type == PlanNodeType.FULLTEXT_SHOW_CLAUSE:
+# 			return "FULLTEXT_SHOW_CLAUSE"
+# 		elif type == PlanNodeType.INDEX_CREATE_CLAUSE:
+# 			return "INDEX_CREATE_CLAUSE"
+# 		elif type == PlanNodeType.INDEX_DROP_CLAUSE:
+# 			return "INDEX_DROP_CLAUSE"
+# 		elif type == PlanNodeType.INDEX_SHOW_CLAUSE:
+# 			return "INDEX_SHOW_CLAUSE"
+# 		elif type == PlanNodeType.LTE_CLAUSE:
+# 			return "LTE_CLAUSE"
+# 		elif type == PlanNodeType.UFE_CLAUSE:
+# 			return "UFE_CLAUSE"
+# 		elif type == PlanNodeType.TASK_CLEAR_CLAUSE:
+# 			return "TASK_CLEAR_CLAUSE"
+# 		elif type == PlanNodeType.TASK_STOP_CLAUSE:
+# 			return "TASK_STOP_CLAUSE"
+# 		elif type == PlanNodeType.TASK_PAUSE_CLAUSE:
+# 			return 'TASK_PAUSE_CLAUSE'
+# 		elif type == PlanNodeType.TASK_RESUME_CLAUSE:
+# 			return "TASK_RESUME_CLAUSE"
+# 		elif type == PlanNodeType.TASK_SHOW_CLAUSE:
+# 			return "TASK_SHOW_CLAUSE"
+# 		elif type == PlanNodeType.TOP_CLAUSE:
+# 			return "TOP_CLAUSE"
+# 		elif type == PlanNodeType.KILL_CLAUSE:
+# 			return "KILL_CLAUSE"
+# 		elif type == PlanNodeType.STAT_CLAUSE:
+# 			return "STAT_CLAUSE"
+# 		elif type == PlanNodeType.POLICY_SHOW_CLAUSE:
+# 			return "POLICY_SHOW_CLAUSE"
+# 		elif type == PlanNodeType.POLICY_CREATE_CLAUSE:
+# 			return "POLICY_CREATE_CLAUSE"
+# 		elif type == PlanNodeType.POLICY_DELETE_CLAUSE:
+# 			return "POLICY_DELETE_CLAUSE"
+# 		elif type == PlanNodeType.POLICY_UPDATE_CLAUSE:
+# 			return "POLICY_UPDATE_CLAUSE"
+# 		elif type == PlanNodeType.USER_SHOW_CLAUSE:
+# 			return 'USER_SHOW_CLAUSE'
+# 		elif type == PlanNodeType.USER_CREATE_CLAUSE:
+# 			return "USER_CREATE_CLAUSE"
+# 		elif type == PlanNodeType.USER_DELETE_CLAUSE:
+# 			return "USER_DELETE_CLAUSE"
+# 		elif type == PlanNodeType.USER_UPDATE_CLAUSE:
+# 			return "USER_UPDATE_CLAUSE"
+# 		elif type == PlanNodeType.PRIVILEGE_SHOW_CLAUSE:
+# 			return "PRIVILEGE_SHOW_CLAUSE"
+# 		elif type == PlanNodeType.GRANT_CLAUSE:
+# 			return "GRANT_CLAUSE"
+# 		elif type == PlanNodeType.REVOKE_CLAUSE:
+# 			return "REVOKE_CLAUSE"
+# 		elif type == PlanNodeType.SELF_INFO_GET_CLAUSE:
+# 			return "SELF_INFO_GET_CLAUSE"
+# 		elif type == PlanNodeType.ALGO_CLAUSE:
+# 			return "ALGO_CLAUSE"
+# 		elif type == PlanNodeType.ALGO_WRITE_CLAUSE:
+# 			return "ALGO_WRITE_CLAUSE"
+# 		elif type == PlanNodeType.ALGO_LIST_CLAUSE:
+# 			return 'ALGO_LIST_CLAUSE'
+# 		elif type == PlanNodeType.SUB_GRAPH_CLAUSE:
+# 			return "SUB_GRAPH_CLAUSE"
+# 		elif type == PlanNodeType.OPTIONAL_TEMPLATE_CLAUSE:
+# 			return "OPTIONAL_TEMPLATE_CLAUSE"
+# 		elif type == PlanNodeType.SUBQUERY_CLAUSE:
+# 			return "SUBQUERY_CLAUSE"
+# 		elif type == PlanNodeType.UNION_CLAUSE:
+# 			return "UNION_CLAUSE"
+# 		else:
+# 			return type
 
 
 class SchemaProperty:
 	'''
 	Schema properties
 	'''
 
@@ -590,14 +603,38 @@
 	def set(self, propertyName: str, value):
 		self.values.update({propertyName: value})
 
 	def _getIndex(self):
 		return self._index
 
 
+class EntityRow:
+	_index = None
+
+	def __init__(self, values: Dict, schema: str = None, id: str = None, from_id: str = None, to_id: str = None,
+				 uuid: int = None, from_uuid: int = None, to_uuid: int = None, **kwargs):
+		self.uuid = uuid
+		self.id = id
+		self.from_uuid = from_uuid
+		self.to_uuid = to_uuid
+		self.from_id = from_id
+		self.to_id = to_id
+		if schema is None:
+			if kwargs.get("schema_name") is not None:
+				self.schema = kwargs.get("schema_name")
+			else:
+				self.schema = None
+		else:
+			self.schema = schema
+		self.values = values
+
+	def _getIndex(self):
+		return self._index
+
+
 class Path(BaseModel):
 	nodeSchemas: Dict[str, Schema] = {}
 	edgeSchemas: Dict[str, Schema] = {}
 
 	def __init__(self, nodes: List[Node], edges: List[Edge], nodeSchemas, edgeSchemas):
 		self.nodes = nodes
 		self.edges = edges
@@ -668,33 +705,109 @@
 			nodeRows = []
 		self.nodeRows = nodeRows
 
 	def __del__(self):
 		pass
 
 
+class NodeEntityTable:
+	def __init__(self, schemas: List[object], nodeRows: List[EntityRow] = None):
+		self.schemas = schemas
+		if nodeRows is None:
+			nodeRows = []
+		self.nodeRows = nodeRows
+
+	def __del__(self):
+		pass
+
+
 class EdgeTable:
 	def __init__(self, schemas: List[object], edgeRows: List[Edge] = None):
 		self.schemas = schemas
 		if edgeRows is None:
 			edgeRows = []
 		self.edgeRows = edgeRows
 
 
+class EdgeEntityTable:
+	def __init__(self, schemas: List[object], edgeRows: List[EntityRow] = None):
+		self.schemas = schemas
+		if edgeRows is None:
+			edgeRows = []
+		self.edgeRows = edgeRows
+
+	def __del__(self):
+		pass
+
+
+class EntityTable:
+	def __init__(self, schemas: List[object], entity_rows: List[EntityRow] = None):
+		# newHeaderList = [{"schema_name": schema_name, "properties":[{"property_name":"","property_type(PropertyType)":""}]}]
+		# nodeRowsList = [{"schema_name": schema_name, 'values': [values]}]
+		self.schemas = schemas
+		if entity_rows is None:
+			entity_rows = []
+		self.entity_rows = entity_rows
+
+	def __del__(self):
+		pass
+
+
 class EdgeAlias:
 	def __init__(self, alias: str, edges: List[Edge]):
 		self.alias = alias
 		self.edges = edges
 
 
+
+
+
 class AttrAlias:
-	def __init__(self, alias: str, values: List[str], type: str = None):
+	def __init__(self, alias: str, values: any, type: ResultType = None,type_desc:str=None):
 		self.name = alias
-		self.rows = values
+		self.values = values
 		self.type = type
+		self.type_desc = type_desc
+
+class AttrNodeAlias:
+	def __init__(self, alias: str, values:  List[List[Node]], type: ResultType = None,type_desc:str=None):
+		self.name = alias
+		self.values = values
+		self.type = type
+		self.type_desc = type_desc
+
+class AttrEdgeAlias:
+	def __init__(self, alias: str, values: List[List[Edge]], type: ResultType = None,type_desc:str=None):
+		self.name = alias
+		self.values = values
+		self.type = type
+		self.type_desc = type_desc
+
+class AttrPathAlias:
+	def __init__(self, alias: str, values: List[List[Path]], type: ResultType = None,type_desc:str=None):
+		self.name = alias
+		self.values = values
+		self.type = type
+		self.type_desc = type_desc
+
+class Attr:
+
+	def __init__(self, type: PropertyType, values: any,has_attr_data:bool=False,has_ultipa_data:bool=False,type_desc: any = None):
+		self.values = values
+		self.type = type
+		self.type_desc = type_desc
+		self.has_attr_data = has_attr_data
+		self.has_ultipa_data = has_ultipa_data
+
+
+class AttrNewAlias:
+	def __init__(self, alias: str, attr: Attr):
+		self.alias = alias
+		self.attr = attr
+
 
 
 class ResultAlias:
 	def __init__(self, alias: str, result_type: int):
 		self.alias = alias
 		self.result_type = result_type
 
@@ -739,16 +852,16 @@
 class ArrayAlias:
 	def __init__(self, alias: str, elements):
 		self.alias = alias
 		self.elements = elements
 
 
 class ExplainPlan:
-	def __init__(self, type: PlanNodeType, alias, childrenNum, uql, infos):
-		self.type = PlanNodeType.getTypeStr(type)
+	def __init__(self, alias, childrenNum, uql, infos):
+		# self.type = type
 		self.alias = alias
 		self.children_num = childrenNum
 		self.uql = uql
 		self.infos = infos
 		self.id = str(uuid.uuid4())
 
 
@@ -810,30 +923,40 @@
 			return self.data
 		if self.type != ResultType.getTypeStr(ResultType.RESULT_TYPE_ATTR):
 			error = f"DataItem {self.alias} is not Type Attribute list"
 			raise ParameterException(error)
 
 		return self.data
 
+	def asNodeList(self) -> AttrNodeAlias:
+		return self.asAttr()
+
+	def asEdgeList(self) -> AttrEdgeAlias:
+		return self.asAttr()
+
+	def asPathList(self) -> AttrPathAlias:
+		return self.asAttr()
+
+
 	def asTable(self) -> Table:
 		if self.type == ResultType.getTypeStr(ResultType.RESULT_TYPE_UNSET):
 			return self.data
 		if self.type != ResultType.getTypeStr(ResultType.RESULT_TYPE_TABLE):
 			error = f"DataItem {self.alias} is not Type Table"
 			raise ParameterException(error)
 		return self.data
 
 	def asArray(self) -> ArrayAlias:
 		if self.type == ResultType.getTypeStr(ResultType.RESULT_TYPE_UNSET):
 			if self.data is None:
 				return None
 			return self.data
-		if self.type != ResultType.getTypeStr(ResultType.RESULT_TYPE_ARRAY):
-			error = f"DataItem {self.alias} is not Type Array"
-			raise ParameterException(error)
+		# if self.type != ResultType.getTypeStr(ResultType.RESULT_TYPE_ARRAY):
+		# 	error = f"DataItem {self.alias} is not Type Array"
+		# 	raise ParameterException(error)
 		return self.data
 
 	def asSchemas(self) -> List[UQLSchema]:
 		if self.type == ResultType.getTypeStr(ResultType.RESULT_TYPE_UNSET):
 			if self.data is None:
 				return []
 			return self.data
@@ -928,22 +1051,22 @@
 
 	def asKV(self):
 		return self.toDict()
 
 
 class BaseUqlReply:
 	def __init__(self, paths: List[PathAlias], nodes: List[NodeAlias], edges: List[EdgeAlias], tables: List[Table],
-				 arrays: [ArrayAlias], attrs: List = None, resultAlias: List = None,
+				 attrs: List = None, resultAlias: List = None,
 				 explainPlan: List[ExplainPlan] = None):
 		self.paths = paths
 		self.nodes = nodes
 		self.edges = edges
 		self.tables = tables
 		self.attrs = attrs
-		self.arrays = arrays
+		# self.arrays = arrays
 		self.resultAlias = resultAlias
 		self.explainPlan = explainPlan
 
 
 class UltipaStatistics(BaseModel):
 	def __init__(self, edge_affected: int, node_affected: int, engine_time_cost: int, total_time_cost: int):
 		self.edgeAffected = edge_affected
@@ -986,24 +1109,54 @@
 				self._aliasMap[data.alias].data.extend(data.edges)
 				continue
 			self._aliasMap[data.alias] = DataItem(data.alias, data.edges,
 												  ResultType.getTypeStr(ResultType.RESULT_TYPE_EDGE))
 
 		for data in self._dataBase.attrs:
 			if self._aliasMap.get(data.name):
-				self._aliasMap[data.name].data.extend(data.rows)
+				self._aliasMap[data.name].data.append(data)
 				continue
 			self._aliasMap[data.name] = DataItem(data.name, data, ResultType.getTypeStr(ResultType.RESULT_TYPE_ATTR))
-
-		for data in self._dataBase.arrays:
-			if self._aliasMap.get(data.alias):
-				self._aliasMap[data.alias].data.extend(data)
-				continue
-			self._aliasMap[data.alias] = DataItem(data.alias, data,
-												  ResultType.getTypeStr(ResultType.RESULT_TYPE_ARRAY))
+			# if data.type in ["list"]:
+			# 	for attrRow in data.rows:
+			# 		if attrRow.type == ResultType.RESULT_TYPE_NODE:
+			# 			if attrRow.nodes and len(attrRow.nodes)>0:
+			# 				if self._aliasMap.get(data.name):
+			# 					self._aliasMap[data.name].data.extend(attrRow.nodes)
+			# 				else:
+			# 					self._aliasMap[data.name] = DataItem(data.name, attrRow.nodes,
+			# 														 ResultType.getTypeStr(ResultType.RESULT_TYPE_NODE))
+			# 		elif attrRow.type == ResultType.RESULT_TYPE_EDGE:
+			# 			if attrRow.edges and len(attrRow.edges)>0:
+			# 				if self._aliasMap.get(data.name):
+			# 					self._aliasMap[data.name].data.extend(attrRow.nodes)
+			# 				else:
+			# 					self._aliasMap[data.name] = DataItem(data.name, attrRow.edges,
+			# 														 ResultType.getTypeStr(ResultType.RESULT_TYPE_EDGE))
+			# 		elif attrRow.type == ResultType.RESULT_TYPE_PATH:
+			# 			if attrRow.paths and len(attrRow.paths)>0:
+			# 				if self._aliasMap.get(data.name):
+			# 					self._aliasMap[data.name].data.extend(attrRow.paths)
+			# 				else:
+			# 					self._aliasMap[data.name] = DataItem(data.name, attrRow.paths,
+			# 														 ResultType.getTypeStr(ResultType.RESULT_TYPE_PATH))
+			# 		else:
+			# 			if attrRow.attrs and len(attrRow.attrs) > 0:
+			# 				self._aliasMap[data.name] = DataItem(data.name, data,
+			# 													 ResultType.getTypeStr(ResultType.RESULT_TYPE_ATTR))
+			# else:
+			# 	self._aliasMap[data.name] = DataItem(data.name, data,
+			# 										 ResultType.getTypeStr(ResultType.RESULT_TYPE_ATTR))
+
+		# for data in self._dataBase.arrays:
+		# 	if self._aliasMap.get(data.alias):
+		# 		self._aliasMap[data.alias].data.extend(data)
+		# 		continue
+		# 	self._aliasMap[data.alias] = DataItem(data.alias, data,
+		# 										  ResultType.getTypeStr(ResultType.RESULT_TYPE_ARRAY))
 
 		for data in self._dataBase.tables:
 			if self._aliasMap.get(data.name):
 				self._aliasMap[data.name].data.extend(data)
 				continue
 			self._aliasMap[data.name] = DataItem(data.name, data, ResultType.getTypeStr(ResultType.RESULT_TYPE_TABLE))
 
@@ -1103,15 +1256,16 @@
 	Debug: bool = False
 	timeZone = None
 	timeZoneOffset = None
 
 	def __init__(self, hosts=None, username=None, password=None, crtFilePath=None, defaultGraph: str = defaultGraph,
 				 timeout: int = timeoutWithSeconds, responseWithRequestInfo: bool = responseWithRequestInfo,
 				 consistency: bool = consistency, heartBeat: int = 10, maxRecvSize: int = -1,
-				 uqlLoggerConfig: LoggerConfig = uqlLoggerConfig, debug: bool = False,timeZone=None,timeZoneOffset=None, **kwargs):
+				 uqlLoggerConfig: LoggerConfig = uqlLoggerConfig, debug: bool = False, timeZone=None,
+				 timeZoneOffset=None, **kwargs):
 		if hosts is None:
 			hosts = []
 		self.hosts = hosts
 		self.username = username
 		self.password = password
 		self.crtFilePath = crtFilePath
 		self.defaultGraph = defaultGraph
@@ -1127,16 +1281,21 @@
 		if kwargs.get("timeoutWithSeconds") is not None:
 			self.timeoutWithSeconds = kwargs.get("timeoutWithSeconds")
 
 	def setDefaultGraphName(self, graph: str):
 		self.defaultGraph = graph
 
 
-# class DefaultConfig(UltipaConfig):
-#     pass
+class PaserAttrListData:
+	def __init__(self, type, nodes: List[Node]=None, edges: List[Edge]=None, paths: List[Path]=None, attrs: Attr=None):
+		self.type = type
+		self.nodes = nodes
+		self.edges = edges
+		self.paths = paths
+		self.attrs = attrs
 
 
 class OrderType(Enum):
 	desc = 'desc'
 	asc = 'asc'
```

### Comparing `ultipa-4.2.4/ultipa/types/types_request.py` & `ultipa-4.3.0/ultipa/types/types_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -188,29 +188,30 @@
 	def __init__(self, name: str, type: ULTIPA.PropertyType):
 		self.name = name
 		self.type = type
 
 
 class InsertNodeBulk:
 	def __init__(self, schema: str, rows: List[dict], insertType: ULTIPA.InsertType, silent: bool = False,
-				 batch: bool = False, n: int = 100,timeZone=None,timeZoneOffset=None):
+				 batch: bool = False, n: int = 100, timeZone=None, timeZoneOffset=None):
 		# self.headers = headers
 		self.schema = schema
 		self.rows = rows
 		self.silent = silent
 		self.insertType = insertType
 		self.batch = batch
 		self.n = n
 		self.timeZone = timeZone
 		self.timeZoneOffset = timeZoneOffset
 
 
 class InsertEdgeBulk:
 	def __init__(self, schema: str, rows: List[dict], insertType: ULTIPA.InsertType, silent: bool = False,
-				 create_node_if_not_exist: bool = False, batch: bool = False, n: int = 100,timeZone=None,timeZoneOffset=None):
+				 create_node_if_not_exist: bool = False, batch: bool = False, n: int = 100, timeZone=None,
+				 timeZoneOffset=None):
 		self.schema = schema
 		self.rows = rows
 		self.silent = silent
 		self.create_node_if_not_exist = create_node_if_not_exist
 		self.insertType = insertType
 		self.batch = batch
 		self.n = n
@@ -326,31 +327,31 @@
 		self.timeZone = timeZone
 		self.timeZoneOffset = timeZoneOffset
 
 
 class InsertConfig(RequestConfig):
 	def __init__(self, insertType: ULTIPA.InsertType, graphName: str = '', timeout: int = 3600,
 				 retry: Retry = Retry(), stream: bool = False, useHost: str = None, useMaster: bool = False,
-				 CreateNodeIfNotExist: bool = False,timeZone = None,timeZoneOffset = None,**kwargs):
-		super().__init__(graphName, timeout, retry, stream, useHost, useMaster,timeZone=timeZone,timeZoneOffset=timeZoneOffset)
+				 CreateNodeIfNotExist: bool = False, timeZone=None, timeZoneOffset=None, **kwargs):
+		super().__init__(graphName, timeout, retry, stream, useHost, useMaster, timeZone=timeZone,
+						 timeZoneOffset=timeZoneOffset)
 		self.insertType = insertType
 		if kwargs.get("silent") is not None:
 			self.silent = kwargs.get("silent")
 		else:
 			self.silent = True
 		if kwargs.get("batch") is not None:
 			self.batch = kwargs.get("batch")
 		if kwargs.get("n") is not None:
 			self.n = kwargs.get("n")
 		if kwargs.get("timeoutWithSeconds") is not None:
 			self.timeoutWithSeconds = kwargs.get("timeoutWithSeconds")
 		self.createNodeIfNotExist = CreateNodeIfNotExist
 
 
-
 class Common(InsertConfig):
 	...
 
 
 class LTE:
 
 	def __init__(self, schemaName: CommonSchema, type: ULTIPA.DBType):
@@ -377,17 +378,18 @@
 	def __str__(self):
 		return '@' + self.schemaName
 
 
 class CreateProperty(Property):
 	def __init__(self, type: ULTIPA.DBType, commonSchema: CommonSchema,
 				 propertyType: ULTIPA.CreatePropertyType = ULTIPA.CreatePropertyType.PROPERTY_STRING,
-				 description: str = ''):
+				 description: str = '', subTypes: List[ULTIPA.CreatePropertyType] = None):
 		super().__init__(type)
 		self.propertyType = propertyType
+		self.subTypes = subTypes
 		self.description = description
 		self.schemaName = commonSchema
 
 
 class DropProperty(Property):
 	def __init__(self, type: ULTIPA.DBType, commonSchema: CommonSchema):
 		super().__init__(type)
@@ -709,14 +711,21 @@
 		"_id": ULTIPA.PropertyType.PROPERTY_ID,
 		"_uuid": ULTIPA.PropertyType.PROPERTY_UUID,
 		"_from": ULTIPA.PropertyType.PROPERTY_FROM,
 		"_to": ULTIPA.PropertyType.PROPERTY_TO,
 		"_from_uuid": ULTIPA.PropertyType.PROPERTY_FROM_UUID,
 		"_to_uuid": ULTIPA.PropertyType.PROPERTY_TO_UUID,
 		"_ignore": ULTIPA.PropertyType.PROPERTY_IGNORE,
+		"unset": ULTIPA.PropertyType.PROPERTY_UNSET,
+		"point": ULTIPA.PropertyType.PROPERTY_POINT,
+		"decimal": ULTIPA.PropertyType.PROPERTY_DECIMAL,
+		"list": ULTIPA.PropertyType.PROPERTY_LIST,
+		"set": ULTIPA.PropertyType.PROPERTY_SET,
+		"map": ULTIPA.PropertyType.PROPERTY_MAP,
+		"null": ULTIPA.PropertyType.PROPERTY_NULL,
 	}
 
 	PropertyReverseMap = {
 		ULTIPA.PropertyType.PROPERTY_STRING: "string",
 		ULTIPA.PropertyType.PROPERTY_INT32: "int32",
 		ULTIPA.PropertyType.PROPERTY_INT64: "int64",
 		ULTIPA.PropertyType.PROPERTY_UINT32: "uint32",
@@ -730,20 +739,59 @@
 		ULTIPA.PropertyType.PROPERTY_UUID: "_uuid",
 		ULTIPA.PropertyType.PROPERTY_FROM: "_from",
 		ULTIPA.PropertyType.PROPERTY_TO: "_to",
 		ULTIPA.PropertyType.PROPERTY_FROM_UUID: "_from_uuid",
 		ULTIPA.PropertyType.PROPERTY_TO_UUID: "_to_uuid",
 		ULTIPA.PropertyType.PROPERTY_IGNORE: "_ignore",
 		ULTIPA.PropertyType.PROPERTY_UNSET: "unset",
+		ULTIPA.PropertyType.PROPERTY_POINT: "point",
+		ULTIPA.PropertyType.PROPERTY_DECIMAL: "decimal",
+		ULTIPA.PropertyType.PROPERTY_LIST: "list",
+		ULTIPA.PropertyType.PROPERTY_SET: "set",
+		ULTIPA.PropertyType.PROPERTY_MAP: "map",
+		ULTIPA.PropertyType.PROPERTY_NULL: "null",
 	}
 
-	def __init__(self, name: str, type: ULTIPA.PropertyType = None, desc: str = None):
+	def __init__(self, name: str, type: ULTIPA.PropertyType = None, desc: str = None,
+				 subTypes: List[ULTIPA.PropertyType] = None):
 		self.name = name
 		self.desc = desc
 		self.type = type
+		self.subTypes = subTypes
+
+	def setSubTypesbyType(self, type: str):
+		if "string" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_STRING]
+
+		if "int32" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_INT32]
+
+		if "uint32" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_UINT32]
+
+		if "int64" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_INT64]
+
+		if "uint64" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_UINT64]
+
+		if "float" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_FLOAT]
+
+		if "double" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_DOUBLE]
+
+		if "datetime" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_DATETIME]
+
+		if "timestamp" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_TIMESTAMP]
+
+		if "text" in type:
+			self.subTypes = [ULTIPA.PropertyType.PROPERTY_TEXT]
 
 	def isIdType(self) -> bool:
 		idTypes = [
 			ULTIPA.PropertyType.PROPERTY_ID,
 			ULTIPA.PropertyType.PROPERTY_TO,
 			ULTIPA.PropertyType.PROPERTY_UUID,
 			ULTIPA.PropertyType.PROPERTY_FROM,
@@ -761,23 +809,34 @@
 	def setTypeInt(self, value):
 		self.type = self.getPropertyTypeByString(value)
 
 	def getStringType(self):
 		return self.getStringByPropertyType(self.type)
 
 	def getPropertyTypeByString(self, v):
-		return self.PropertyMap[v]
+		if not self.PropertyMap.get(v):
+			if "[" in v:
+				self.setSubTypesbyType(v)
+				return ULTIPA.PropertyType.PROPERTY_LIST
+
+		return self.PropertyMap.get(v)
 
 	def getStringByPropertyType(self, v):
 		return self.PropertyReverseMap[v]
 
 	@staticmethod
 	def _getStringByPropertyType(v):
 		return Property.PropertyReverseMap[v]
 
+	@staticmethod
+	def _getPropertyTypeByString(v):
+		return Property.PropertyMap.get(v)
+
+
+
 
 class Schema:
 
 	def __init__(self, name: str, properties: List[Property], desc: str = None, type: str = None,
 				 DBType: ULTIPA.DBType = None, total: int = None):
 		self.name = name
 		self.properties = properties
@@ -790,19 +849,20 @@
 		find = list(filter(lambda x: x.get('name') == name, self.properties))
 		if find:
 			return find[0]
 		return None
 
 
 class Batch:
-	Nodes: List[ULTIPA.Node]
-	Edges: List[ULTIPA.Edge]
+	Nodes: List[ULTIPA.EntityRow]
+	Edges: List[ULTIPA.EntityRow]
 	Schema: Schema
 
-	def __init__(self, Schema: Schema = None, Nodes: List[ULTIPA.Node] = None, Edges: List[ULTIPA.Edge] = None):
+	def __init__(self, Schema: Schema = None, Nodes: List[ULTIPA.EntityRow] = None,
+				 Edges: List[ULTIPA.EntityRow] = None):
 		if Nodes is None:
 			Nodes = []
 		if Edges is None:
 			Edges = []
 		self.Nodes = Nodes
 		self.Edges = Edges
 		self.Schema = Schema
```

### Comparing `ultipa-4.2.4/ultipa/proto/ultipa_pb2_grpc.py` & `ultipa-4.3.0/ultipa/proto/ultipa_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from ultipa.proto import ultipa_pb2 as ultipa__pb2
+from  ultipa.proto import ultipa_pb2 as ultipa__pb2
 
 
 class UltipaRpcsStub(object):
     """The ultipa service definition.
     """
 
     def __init__(self, channel):
@@ -242,14 +242,19 @@
                 response_deserializer=ultipa__pb2.UninstallExtaReply.FromString,
                 )
         self.Authenticate = channel.unary_unary(
                 '/ultipa.UltipaControls/Authenticate',
                 request_serializer=ultipa__pb2.AuthenticateRequest.SerializeToString,
                 response_deserializer=ultipa__pb2.AuthenticateReply.FromString,
                 )
+        self.Backup = channel.unary_unary(
+                '/ultipa.UltipaControls/Backup',
+                request_serializer=ultipa__pb2.BackupRequest.SerializeToString,
+                response_deserializer=ultipa__pb2.BackupReply.FromString,
+                )
 
 
 class UltipaControlsServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def SayHello(self, request, context):
         """1.Sends a greeting
@@ -339,14 +344,21 @@
     def Authenticate(self, request, context):
         """13.仅鉴权
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def Backup(self, request, context):
+        """14.backup data
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_UltipaControlsServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'SayHello': grpc.unary_unary_rpc_method_handler(
                     servicer.SayHello,
                     request_deserializer=ultipa__pb2.HelloUltipaRequest.FromString,
                     response_serializer=ultipa__pb2.HelloUltipaReply.SerializeToString,
@@ -407,14 +419,19 @@
                     response_serializer=ultipa__pb2.UninstallExtaReply.SerializeToString,
             ),
             'Authenticate': grpc.unary_unary_rpc_method_handler(
                     servicer.Authenticate,
                     request_deserializer=ultipa__pb2.AuthenticateRequest.FromString,
                     response_serializer=ultipa__pb2.AuthenticateReply.SerializeToString,
             ),
+            'Backup': grpc.unary_unary_rpc_method_handler(
+                    servicer.Backup,
+                    request_deserializer=ultipa__pb2.BackupRequest.FromString,
+                    response_serializer=ultipa__pb2.BackupReply.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'ultipa.UltipaControls', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -637,7 +654,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/ultipa.UltipaControls/Authenticate',
             ultipa__pb2.AuthenticateRequest.SerializeToString,
             ultipa__pb2.AuthenticateReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Backup(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ultipa.UltipaControls/Backup',
+            ultipa__pb2.BackupRequest.SerializeToString,
+            ultipa__pb2.BackupReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ultipa-4.2.4/ultipa/proto/ultipa_pb2.py` & `ultipa-4.3.0/ultipa/proto/ultipa_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cultipa.proto\x12\x06ultipa\"\"\n\x12HelloUltipaRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"C\n\x10HelloUltipaReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x0f\n\x07message\x18\x02 \x01(\t\"e\n\nUqlRequest\x12\x0b\n\x03uql\x18\x01 \x01(\t\x12\x0f\n\x07timeout\x18\x02 \x01(\r\x12\x12\n\ngraph_name\x18\x03 \x01(\t\x12\x11\n\tuser_name\x18\x04 \x01(\t\x12\x12\n\nthread_num\x18\x05 \x01(\r\"E\n\x0bResultAlias\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\'\n\x0bresult_type\x18\x02 \x01(\x0e\x32\x12.ultipa.ResultType\"\x9a\x03\n\x08UqlReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x17\n\x0ftotal_time_cost\x18\x02 \x01(\x05\x12\x18\n\x10\x65ngine_time_cost\x18\x03 \x01(\x05\x12\"\n\x05\x61lias\x18\x04 \x03(\x0b\x32\x13.ultipa.ResultAlias\x12 \n\x05paths\x18\x05 \x03(\x0b\x32\x11.ultipa.PathAlias\x12 \n\x05nodes\x18\x06 \x03(\x0b\x32\x11.ultipa.NodeAlias\x12 \n\x05\x65\x64ges\x18\x07 \x03(\x0b\x32\x11.ultipa.EdgeAlias\x12 \n\x05\x61ttrs\x18\x08 \x03(\x0b\x32\x11.ultipa.AttrAlias\x12\"\n\x06\x61rrays\x18\t \x03(\x0b\x32\x12.ultipa.ArrayAlias\x12\x1d\n\x06tables\x18\n \x03(\x0b\x32\r.ultipa.Table\x12!\n\nstatistics\x18\x0b \x01(\x0b\x32\r.ultipa.Table\x12)\n\x0c\x65xplain_plan\x18\x0c \x01(\x0b\x32\x13.ultipa.ExplainPlan\"7\n\tPathAlias\x12\x1b\n\x05paths\x18\x01 \x03(\x0b\x32\x0c.ultipa.Path\x12\r\n\x05\x61lias\x18\x02 \x01(\t\"A\n\tEdgeAlias\x12%\n\nedge_table\x18\x01 \x01(\x0b\x32\x11.ultipa.EdgeTable\x12\r\n\x05\x61lias\x18\x02 \x01(\t\"A\n\tNodeAlias\x12%\n\nnode_table\x18\x01 \x01(\x0b\x32\x11.ultipa.NodeTable\x12\r\n\x05\x61lias\x18\x02 \x01(\t\"W\n\tAttrAlias\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12+\n\rproperty_type\x18\x02 \x01(\x0e\x32\x14.ultipa.PropertyType\x12\x0e\n\x06values\x18\x03 \x03(\x0c\"\x1e\n\x0c\x41rrayElement\x12\x0e\n\x06values\x18\x01 \x03(\x0c\"p\n\nArrayAlias\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12+\n\rproperty_type\x18\x02 \x01(\x0e\x32\x14.ultipa.PropertyType\x12&\n\x08\x65lements\x18\x03 \x03(\x0b\x32\x14.ultipa.ArrayElement\"\x97\x01\n\x12UserSettingRequest\x12\x11\n\tuser_name\x18\x01 \x01(\t\x12.\n\x03opt\x18\x02 \x01(\x0e\x32!.ultipa.UserSettingRequest.OPTION\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\"\"\n\x06OPTION\x12\x0b\n\x07OPT_GET\x10\x00\x12\x0b\n\x07OPT_SET\x10\x01\"@\n\x10UserSettingReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\";\n\x15\x44ownloadFileRequestV2\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"V\n\x11\x44ownloadFileReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x12\n\ntotal_size\x18\x02 \x01(\x05\x12\r\n\x05\x63hunk\x18\x03 \x01(\x0c\"j\n\rExportRequest\x12\x1f\n\x07\x64\x62_type\x18\x01 \x01(\x0e\x32\x0e.ultipa.DBType\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x19\n\x11select_properties\x18\x03 \x03(\t\x12\x0e\n\x06schema\x18\x04 \x01(\t\"{\n\x0b\x45xportReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12%\n\nnode_table\x18\x02 \x01(\x0b\x32\x11.ultipa.NodeTable\x12%\n\nedge_table\x18\x03 \x01(\x0b\x32\x11.ultipa.EdgeTable\"\x12\n\x10GetLeaderRequest\"0\n\x0eGetLeaderReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"\x88\x01\n\x12InsertNodesRequest\x12%\n\nnode_table\x18\x01 \x01(\x0b\x32\x11.ultipa.NodeTable\x12\x0e\n\x06silent\x18\x02 \x01(\x08\x12\x12\n\ngraph_name\x18\x03 \x01(\t\x12\'\n\x0binsert_type\x18\x04 \x01(\x0e\x32\x12.ultipa.InsertType\"\xb2\x01\n\x10InsertNodesReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x11\n\ttime_cost\x18\x02 \x01(\x05\x12\x18\n\x10\x65ngine_time_cost\x18\x03 \x01(\x05\x12\x11\n\x05uuids\x18\x04 \x03(\x04\x42\x02\x30\x01\x12\x0b\n\x03ids\x18\x05 \x03(\t\x12\x16\n\x0eignore_indexes\x18\x06 \x03(\r\x12\x19\n\x11ignore_error_code\x18\x07 \x03(\r\"\xaa\x01\n\x12InsertEdgesRequest\x12%\n\nedge_table\x18\x01 \x01(\x0b\x32\x11.ultipa.EdgeTable\x12\x0e\n\x06silent\x18\x02 \x01(\x08\x12\x12\n\ngraph_name\x18\x03 \x01(\t\x12 \n\x18\x63reate_node_if_not_exist\x18\x04 \x01(\x08\x12\'\n\x0binsert_type\x18\x05 \x01(\x0e\x32\x12.ultipa.InsertType\"\xa5\x01\n\x10InsertEdgesReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x11\n\ttime_cost\x18\x02 \x01(\x05\x12\x18\n\x10\x65ngine_time_cost\x18\x03 \x01(\x05\x12\x11\n\x05uuids\x18\x04 \x03(\x04\x42\x02\x30\x01\x12\x16\n\x0eignore_indexes\x18\x05 \x03(\r\x12\x19\n\x11ignore_error_code\x18\x06 \x03(\r\"C\n\x12InstallAlgoRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x0b\n\x03md5\x18\x02 \x01(\t\x12\r\n\x05\x63hunk\x18\x03 \x01(\x0c\"2\n\x10InstallAlgoReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\")\n\x14UninstallAlgoRequest\x12\x11\n\talgo_name\x18\x01 \x01(\t\"4\n\x12UninstallAlgoReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"\x96\x01\n\x0fUploaderRequest\x12\x1f\n\x07\x64\x62_type\x18\x01 \x01(\x0e\x32\x0e.ultipa.DBType\x12\x12\n\ngraph_name\x18\x02 \x01(\t\x12\x19\n\x11total_file_counts\x18\x03 \x01(\x04\x12\x11\n\tfile_name\x18\x04 \x01(\t\x12\x11\n\tfile_size\x18\x05 \x01(\x04\x12\r\n\x05\x63hunk\x18\x06 \x01(\x0c\"/\n\rUploaderReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"M\n\x1c\x43reateGraphByUploaderRequest\x12\x12\n\ngraph_name\x18\x01 \x01(\t\x12\x19\n\x11graph_description\x18\x02 \x01(\t\"<\n\x1a\x43reateGraphByUploaderReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"C\n\x12InstallExtaRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x0b\n\x03md5\x18\x02 \x01(\t\x12\r\n\x05\x63hunk\x18\x03 \x01(\x0c\"2\n\x10InstallExtaReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\")\n\x14UninstallExtaRequest\x12\x11\n\texta_name\x18\x01 \x01(\t\"4\n\x12UninstallExtaReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"g\n\x06Status\x12%\n\nerror_code\x18\x01 \x01(\x0e\x32\x11.ultipa.ErrorCode\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12)\n\x0c\x63luster_info\x18\x03 \x01(\x0b\x32\x13.ultipa.ClusterInfo\"S\n\x0cRaftFollower\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04role\x18\x02 \x01(\x05\x12$\n\x06status\x18\x03 \x01(\x0e\x32\x14.ultipa.ServerStatus\"`\n\x0b\x43lusterInfo\x12\x10\n\x08redirect\x18\x01 \x01(\t\x12\x16\n\x0eleader_address\x18\x02 \x01(\t\x12\'\n\tfollowers\x18\x03 \x03(\x0b\x32\x14.ultipa.RaftFollower\"T\n\x04Path\x12%\n\nnode_table\x18\x01 \x01(\x0b\x32\x11.ultipa.NodeTable\x12%\n\nedge_table\x18\x02 \x01(\x0b\x32\x11.ultipa.EdgeTable\"b\n\x05Table\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x1f\n\x07headers\x18\x02 \x03(\x0b\x32\x0e.ultipa.Header\x12$\n\ntable_rows\x18\x03 \x03(\x0b\x32\x10.ultipa.TableRow\"\x1a\n\x08TableRow\x12\x0e\n\x06values\x18\x01 \x03(\x0c\"P\n\tNodeTable\x12\x1f\n\x07schemas\x18\x01 \x03(\x0b\x32\x0e.ultipa.Schema\x12\"\n\tnode_rows\x18\x02 \x03(\x0b\x32\x0f.ultipa.NodeRow\"P\n\tEdgeTable\x12\x1f\n\x07schemas\x18\x01 \x03(\x0b\x32\x0e.ultipa.Schema\x12\"\n\tedge_rows\x18\x03 \x03(\x0b\x32\x0f.ultipa.EdgeRow\"L\n\x07NodeRow\x12\x10\n\x04uuid\x18\x01 \x01(\x04\x42\x02\x30\x01\x12\n\n\x02id\x18\x02 \x01(\t\x12\x13\n\x0bschema_name\x18\x03 \x01(\t\x12\x0e\n\x06values\x18\x04 \x03(\x0c\"\x8c\x01\n\x07\x45\x64geRow\x12\x10\n\x04uuid\x18\x01 \x01(\x04\x42\x02\x30\x01\x12\x13\n\x0bschema_name\x18\x02 \x01(\t\x12\x15\n\tfrom_uuid\x18\x03 \x01(\x04\x42\x02\x30\x01\x12\x13\n\x07to_uuid\x18\x04 \x01(\x04\x42\x02\x30\x01\x12\x0f\n\x07\x66rom_id\x18\x05 \x01(\t\x12\r\n\x05to_id\x18\x06 \x01(\t\x12\x0e\n\x06values\x18\x07 \x03(\x0c\"C\n\x06Schema\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12$\n\nproperties\x18\x02 \x03(\x0b\x32\x10.ultipa.Property\"N\n\x08Property\x12\x15\n\rproperty_name\x18\x01 \x01(\t\x12+\n\rproperty_type\x18\x02 \x01(\x0e\x32\x14.ultipa.PropertyType\"L\n\x06Header\x12\x15\n\rproperty_name\x18\x01 \x01(\t\x12+\n\rproperty_type\x18\x02 \x01(\x0e\x32\x14.ultipa.PropertyType\"#\n\x05Value\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"3\n\x0b\x45xplainPlan\x12$\n\nplan_nodes\x18\x01 \x03(\x0b\x32\x10.ultipa.PlanNode\"o\n\x08PlanNode\x12\"\n\x04type\x18\x01 \x01(\x0e\x32\x14.ultipa.PlanNodeType\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12\x14\n\x0c\x63hildren_num\x18\x03 \x01(\r\x12\x0b\n\x03uql\x18\x04 \x01(\t\x12\r\n\x05infos\x18\x05 \x01(\t\"J\n\x13\x41uthenticateRequest\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.ultipa.AuthenticateType\x12\x0b\n\x03uql\x18\x02 \x01(\t\"3\n\x11\x41uthenticateReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status*\xa9\x01\n\nResultType\x12\x15\n\x11RESULT_TYPE_UNSET\x10\x00\x12\x14\n\x10RESULT_TYPE_PATH\x10\x01\x12\x14\n\x10RESULT_TYPE_NODE\x10\x02\x12\x14\n\x10RESULT_TYPE_EDGE\x10\x03\x12\x14\n\x10RESULT_TYPE_ATTR\x10\x04\x12\x15\n\x11RESULT_TYPE_ARRAY\x10\x05\x12\x15\n\x11RESULT_TYPE_TABLE\x10\x06*3\n\nInsertType\x12\n\n\x06NORMAL\x10\x00\x12\r\n\tOVERWRITE\x10\x01\x12\n\n\x06UPSERT\x10\x02*\x9b\x01\n\x0cPropertyType\x12\t\n\x05UNSET\x10\x00\x12\t\n\x05INT32\x10\x01\x12\n\n\x06UINT32\x10\x02\x12\t\n\x05INT64\x10\x03\x12\n\n\x06UINT64\x10\x04\x12\t\n\x05\x46LOAT\x10\x05\x12\n\n\x06\x44OUBLE\x10\x06\x12\n\n\x06STRING\x10\x07\x12\x0c\n\x08\x44\x41TETIME\x10\x08\x12\r\n\tTIMESTAMP\x10\t\x12\x08\n\x04TEXT\x10\n\x12\x08\n\x04\x42LOB\x10\x0b*\xb2\x02\n\tErrorCode\x12\x0b\n\x07SUCCESS\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\x0f\n\x0bPARAM_ERROR\x10\x02\x12\x11\n\rBASE_DB_ERROR\x10\x03\x12\x10\n\x0c\x45NGINE_ERROR\x10\x04\x12\x10\n\x0cSYSTEM_ERROR\x10\x05\x12\x11\n\rRAFT_REDIRECT\x10\x06\x12\x1f\n\x1bRAFT_LEADER_NOT_YET_ELECTED\x10\x07\x12\x12\n\x0eRAFT_LOG_ERROR\x10\x08\x12\r\n\tUQL_ERROR\x10\t\x12\x11\n\rNOT_RAFT_MODE\x10\n\x12\x1f\n\x1bRAFT_NO_AVAILABLE_FOLLOWERS\x10\x0b\x12\"\n\x1eRAFT_NO_AVAILABLE_ALGO_SERVERS\x10\x0c\x12\x15\n\x11PERMISSION_DENIED\x10\r*]\n\x0c\x46ollowerRole\x12\x0e\n\nROLE_UNSET\x10\x00\x12\x11\n\rROLE_READABLE\x10\x01\x12\x18\n\x14ROLE_ALGO_EXECUTABLE\x10\x02\x12\x10\n\x0cROLE_LEARNER\x10\x04*#\n\x0cServerStatus\x12\x08\n\x04\x44\x45\x41\x44\x10\x00\x12\t\n\x05\x41LIVE\x10\x01*.\n\x06\x44\x42Type\x12\n\n\x06\x44\x42NODE\x10\x00\x12\n\n\x06\x44\x42\x45\x44GE\x10\x01\x12\x0c\n\x08\x44\x42GLOBAL\x10\x02*w\n\x0bTASK_STATUS\x12\x10\n\x0cTASK_PENDING\x10\x00\x12\x12\n\x0eTASK_COMPUTING\x10\x01\x12\x10\n\x0cTASK_WRITING\x10\x02\x12\r\n\tTASK_DONE\x10\x03\x12\x0f\n\x0bTASK_FAILED\x10\x04\x12\x10\n\x0cTASK_STOPPED\x10\x05*\xc4\r\n\x0cPlanNodeType\x12\x10\n\x0c\x43LAUSE_UNSET\x10\x00\x12\x13\n\x0fORDER_BY_CLAUSE\x10\x01\x12\x16\n\x12\x41GGREGATION_CLAUSE\x10\x02\x12\x0f\n\x0bWITH_CLAUSE\x10\x03\x12\x10\n\x0cWHERE_CLAUSE\x10\x04\x12\x14\n\x10UNCOLLECT_CLAUSE\x10\x05\x12\x10\n\x0cTABLE_CLAUSE\x10\x06\x12\x11\n\rRETURN_CLAUSE\x10\x07\x12\x15\n\x11LIMIT_SKIP_CLAUSE\x10\x08\x12\x13\n\x0fTEMPLATE_CLAUSE\x10\t\x12\x18\n\x14KHOP_TEMPLATE_CLAUSE\x10\n\x12\x0f\n\x0bKHOP_CLAUSE\x10\x0b\x12\r\n\tAB_CLAUSE\x10\x0c\x12\x11\n\rSPREAD_CLAUSE\x10\r\x12\x13\n\x0f\x41UTO_NET_CLAUSE\x10\x0e\x12\x16\n\x12NODE_SEARCH_CLAUSE\x10\x0f\x12\x16\n\x12\x45\x44GE_SEARCH_CLAUSE\x10\x10\x12\x16\n\x12NODE_INSERT_CLAUSE\x10\x11\x12\x16\n\x12\x45\x44GE_INSERT_CLAUSE\x10\x12\x12\x16\n\x12NODE_UPSERT_CLAUSE\x10\x13\x12\x16\n\x12\x45\x44GE_UPSERT_CLAUSE\x10\x14\x12\x16\n\x12NODE_UPDATE_CLAUSE\x10\x15\x12\x16\n\x12\x45\x44GE_UPDATE_CLAUSE\x10\x16\x12\x16\n\x12NODE_DELETE_CLAUSE\x10\x17\x12\x16\n\x12\x45\x44GE_DELETE_CLAUSE\x10\x18\x12\x13\n\x0fTRUNCATE_CLAUSE\x10\x19\x12\x12\n\x0e\x43OMPACT_CLAUSE\x10\x1a\x12\x17\n\x13GRAPH_CREATE_CLAUSE\x10\x1b\x12\x15\n\x11GRAPH_DROP_CLAUSE\x10\x1c\x12\x17\n\x13GRAPH_UPDATE_CLAUSE\x10\x1d\x12\x15\n\x11GRAPH_SHOW_CLAUSE\x10\x1e\x12\x16\n\x12GRAPH_MOUNT_CLAUSE\x10\x1f\x12\x18\n\x14GRAPH_UNMOUNT_CLAUSE\x10 \x12\x18\n\x14SCHEMA_CREATE_CLAUSE\x10!\x12\x16\n\x12SCHEMA_DROP_CLAUSE\x10\"\x12\x17\n\x13SCHEMA_ALTER_CLAUSE\x10#\x12\x16\n\x12SCHEMA_SHOW_CLAUSE\x10$\x12\x1a\n\x16PROPERTY_CREATE_CLAUSE\x10%\x12\x18\n\x14PROPERTY_DROP_CLAUSE\x10&\x12\x19\n\x15PROPERTY_ALTER_CLAUSE\x10\'\x12\x18\n\x14PROPERTY_SHOW_CLAUSE\x10(\x12\x1a\n\x16\x46ULLTEXT_CREATE_CLAUSE\x10)\x12\x18\n\x14\x46ULLTEXT_DROP_CLAUSE\x10*\x12\x18\n\x14\x46ULLTEXT_SHOW_CLAUSE\x10+\x12\x17\n\x13INDEX_CREATE_CLAUSE\x10,\x12\x15\n\x11INDEX_DROP_CLAUSE\x10-\x12\x15\n\x11INDEX_SHOW_CLAUSE\x10.\x12\x0e\n\nLTE_CLAUSE\x10/\x12\x0e\n\nUFE_CLAUSE\x10\x30\x12\x15\n\x11TASK_CLEAR_CLAUSE\x10\x31\x12\x14\n\x10TASK_STOP_CLAUSE\x10\x32\x12\x15\n\x11TASK_PAUSE_CLAUSE\x10\x33\x12\x16\n\x12TASK_RESUME_CLAUSE\x10\x34\x12\x14\n\x10TASK_SHOW_CLAUSE\x10\x35\x12\x0e\n\nTOP_CLAUSE\x10\x36\x12\x0f\n\x0bKILL_CLAUSE\x10\x37\x12\x0f\n\x0bSTAT_CLAUSE\x10\x38\x12\x16\n\x12POLICY_SHOW_CLAUSE\x10\x39\x12\x18\n\x14POLICY_CREATE_CLAUSE\x10:\x12\x18\n\x14POLICY_DELETE_CLAUSE\x10;\x12\x18\n\x14POLICY_UPDATE_CLAUSE\x10<\x12\x14\n\x10USER_SHOW_CLAUSE\x10=\x12\x16\n\x12USER_CREATE_CLAUSE\x10>\x12\x16\n\x12USER_DELETE_CLAUSE\x10?\x12\x16\n\x12USER_UPDATE_CLAUSE\x10@\x12\x19\n\x15PRIVILEGE_SHOW_CLAUSE\x10\x41\x12\x10\n\x0cGRANT_CLAUSE\x10\x42\x12\x11\n\rREVOKE_CLAUSE\x10\x43\x12\x18\n\x14SELF_INFO_GET_CLAUSE\x10\x44\x12\x0f\n\x0b\x41LGO_CLAUSE\x10\x45\x12\x15\n\x11\x41LGO_WRITE_CLAUSE\x10\x46\x12\x14\n\x10\x41LGO_LIST_CLAUSE\x10G\x12\x14\n\x10SUB_GRAPH_CLAUSE\x10H\x12\x1c\n\x18OPTIONAL_TEMPLATE_CLAUSE\x10I\x12\x13\n\x0fSUBQUERY_CLAUSE\x10J\x12\x10\n\x0cUNION_CLAUSE\x10K*\xfc\x02\n\x10\x41uthenticateType\x12\x17\n\x13PERMISSION_TYPE_UQL\x10\x00\x12\x1f\n\x1bPERMISSION_TYPE_INSERTNODES\x10\x01\x12\x1f\n\x1bPERMISSION_TYPE_INSERTEDGES\x10\x02\x12\x1a\n\x16PERMISSION_TYPE_EXPORT\x10\x03\x12 \n\x1cPERMISSION_TYPE_DOWNLOADFILE\x10\x04\x12\x1f\n\x1bPERMISSION_TYPE_INSTALLALGO\x10\x05\x12!\n\x1dPERMISSION_TYPE_UNINSTALLALGO\x10\x06\x12\x1c\n\x18PERMISSION_TYPE_UPLOADER\x10\x07\x12)\n%PERMISSION_TYPE_CREATEGRAPHBYUPLOADER\x10\x08\x12\x1f\n\x1bPERMISSION_TYPE_INSTALLEXTA\x10\t\x12!\n\x1dPERMISSION_TYPE_UNINSTALLEXTA\x10\n2\x8f\x02\n\nUltipaRpcs\x12\x42\n\x08SayHello\x12\x1a.ultipa.HelloUltipaRequest\x1a\x18.ultipa.HelloUltipaReply\"\x00\x12/\n\x03Uql\x12\x12.ultipa.UqlRequest\x1a\x10.ultipa.UqlReply\"\x00\x30\x01\x12\x45\n\x0bInsertNodes\x12\x1a.ultipa.InsertNodesRequest\x1a\x18.ultipa.InsertNodesReply\"\x00\x12\x45\n\x0bInsertEdges\x12\x1a.ultipa.InsertEdgesRequest\x1a\x18.ultipa.InsertEdgesReply\"\x00\x32\xb4\x07\n\x0eUltipaControls\x12\x42\n\x08SayHello\x12\x1a.ultipa.HelloUltipaRequest\x1a\x18.ultipa.HelloUltipaReply\"\x00\x12\x45\n\x0bUserSetting\x12\x1a.ultipa.UserSettingRequest\x1a\x18.ultipa.UserSettingReply\"\x00\x12?\n\tGetLeader\x12\x18.ultipa.GetLeaderRequest\x1a\x16.ultipa.GetLeaderReply\"\x00\x12\x31\n\x05UqlEx\x12\x12.ultipa.UqlRequest\x1a\x10.ultipa.UqlReply\"\x00\x30\x01\x12\x38\n\x06\x45xport\x12\x15.ultipa.ExportRequest\x1a\x13.ultipa.ExportReply\"\x00\x30\x01\x12N\n\x0e\x44ownloadFileV2\x12\x1d.ultipa.DownloadFileRequestV2\x1a\x19.ultipa.DownloadFileReply\"\x00\x30\x01\x12G\n\x0bInstallAlgo\x12\x1a.ultipa.InstallAlgoRequest\x1a\x18.ultipa.InstallAlgoReply\"\x00(\x01\x12K\n\rUninstallAlgo\x12\x1c.ultipa.UninstallAlgoRequest\x1a\x1a.ultipa.UninstallAlgoReply\"\x00\x12>\n\x08Uploader\x12\x17.ultipa.UploaderRequest\x1a\x15.ultipa.UploaderReply\"\x00(\x01\x12\x63\n\x15\x43reateGraphByUploader\x12$.ultipa.CreateGraphByUploaderRequest\x1a\".ultipa.CreateGraphByUploaderReply\"\x00\x12G\n\x0bInstallExta\x12\x1a.ultipa.InstallExtaRequest\x1a\x18.ultipa.InstallExtaReply\"\x00(\x01\x12K\n\rUninstallExta\x12\x1c.ultipa.UninstallExtaRequest\x1a\x1a.ultipa.UninstallExtaReply\"\x00\x12H\n\x0c\x41uthenticate\x12\x1b.ultipa.AuthenticateRequest\x1a\x19.ultipa.AuthenticateReply\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cultipa.proto\x12\x06ultipa\"\"\n\x12HelloUltipaRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"C\n\x10HelloUltipaReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x0f\n\x07message\x18\x02 \x01(\t\"\x84\x01\n\nUqlRequest\x12\x0b\n\x03uql\x18\x01 \x01(\t\x12\x0f\n\x07timeout\x18\x02 \x01(\r\x12\x12\n\ngraph_name\x18\x03 \x01(\t\x12\x11\n\tuser_name\x18\x04 \x01(\t\x12\x12\n\nthread_num\x18\x05 \x01(\r\x12\n\n\x02tz\x18\x06 \x01(\t\x12\x11\n\ttz_offset\x18\x07 \x01(\t\"E\n\x0bResultAlias\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\'\n\x0bresult_type\x18\x02 \x01(\x0e\x32\x12.ultipa.ResultType\"\xf6\x02\n\x08UqlReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x17\n\x0ftotal_time_cost\x18\x02 \x01(\x05\x12\x18\n\x10\x65ngine_time_cost\x18\x03 \x01(\x05\x12\"\n\x05\x61lias\x18\x04 \x03(\x0b\x32\x13.ultipa.ResultAlias\x12 \n\x05paths\x18\x05 \x03(\x0b\x32\x11.ultipa.PathAlias\x12 \n\x05nodes\x18\x06 \x03(\x0b\x32\x11.ultipa.NodeAlias\x12 \n\x05\x65\x64ges\x18\x07 \x03(\x0b\x32\x11.ultipa.EdgeAlias\x12 \n\x05\x61ttrs\x18\x08 \x03(\x0b\x32\x11.ultipa.AttrAlias\x12\x1d\n\x06tables\x18\n \x03(\x0b\x32\r.ultipa.Table\x12!\n\nstatistics\x18\x0b \x01(\x0b\x32\r.ultipa.Table\x12)\n\x0c\x65xplain_plan\x18\x0c \x01(\x0b\x32\x13.ultipa.ExplainPlan\"7\n\tPathAlias\x12\x1b\n\x05paths\x18\x01 \x03(\x0b\x32\x0c.ultipa.Path\x12\r\n\x05\x61lias\x18\x02 \x01(\t\"C\n\tEdgeAlias\x12\'\n\nedge_table\x18\x01 \x01(\x0b\x32\x13.ultipa.EntityTable\x12\r\n\x05\x61lias\x18\x02 \x01(\t\"C\n\tNodeAlias\x12\'\n\nnode_table\x18\x01 \x01(\x0b\x32\x13.ultipa.EntityTable\x12\r\n\x05\x61lias\x18\x02 \x01(\t\"6\n\tAttrAlias\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\x1a\n\x04\x61ttr\x18\x02 \x01(\x0b\x32\x0c.ultipa.Attr\"@\n\x04\x41ttr\x12(\n\nvalue_type\x18\x01 \x01(\x0e\x32\x14.ultipa.PropertyType\x12\x0e\n\x06values\x18\x02 \x03(\x0c\"\xc3\x01\n\x0c\x41ttrListData\x12 \n\x04type\x18\x01 \x01(\x0e\x32\x12.ultipa.ResultType\x12\"\n\x05nodes\x18\x02 \x01(\x0b\x32\x13.ultipa.EntityTable\x12\"\n\x05\x65\x64ges\x18\x03 \x01(\x0b\x32\x13.ultipa.EntityTable\x12\x1b\n\x05paths\x18\x04 \x03(\x0b\x32\x0c.ultipa.Path\x12\x1b\n\x05\x61ttrs\x18\x05 \x03(\x0b\x32\x0c.ultipa.Attr\x12\x0f\n\x07is_null\x18\x06 \x01(\x08\"E\n\x0b\x41ttrMapData\x12\x19\n\x03key\x18\x01 \x01(\x0b\x32\x0c.ultipa.Attr\x12\x1b\n\x05value\x18\x02 \x01(\x0b\x32\x0c.ultipa.Attr\"\x97\x01\n\x12UserSettingRequest\x12\x11\n\tuser_name\x18\x01 \x01(\t\x12.\n\x03opt\x18\x02 \x01(\x0e\x32!.ultipa.UserSettingRequest.OPTION\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\"\"\n\x06OPTION\x12\x0b\n\x07OPT_GET\x10\x00\x12\x0b\n\x07OPT_SET\x10\x01\"@\n\x10UserSettingReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\";\n\x15\x44ownloadFileRequestV2\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"V\n\x11\x44ownloadFileReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x12\n\ntotal_size\x18\x02 \x01(\x05\x12\r\n\x05\x63hunk\x18\x03 \x01(\x0c\"j\n\rExportRequest\x12\x1f\n\x07\x64\x62_type\x18\x01 \x01(\x0e\x32\x0e.ultipa.DBType\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x19\n\x11select_properties\x18\x03 \x03(\t\x12\x0e\n\x06schema\x18\x04 \x01(\t\"\x7f\n\x0b\x45xportReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\'\n\nnode_table\x18\x02 \x01(\x0b\x32\x13.ultipa.EntityTable\x12\'\n\nedge_table\x18\x03 \x01(\x0b\x32\x13.ultipa.EntityTable\"\x12\n\x10GetLeaderRequest\"0\n\x0eGetLeaderReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"\x8a\x01\n\x12InsertNodesRequest\x12\'\n\nnode_table\x18\x01 \x01(\x0b\x32\x13.ultipa.EntityTable\x12\x0e\n\x06silent\x18\x02 \x01(\x08\x12\x12\n\ngraph_name\x18\x03 \x01(\t\x12\'\n\x0binsert_type\x18\x04 \x01(\x0e\x32\x12.ultipa.InsertType\"\xb2\x01\n\x10InsertNodesReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x11\n\ttime_cost\x18\x02 \x01(\x05\x12\x18\n\x10\x65ngine_time_cost\x18\x03 \x01(\x05\x12\x11\n\x05uuids\x18\x04 \x03(\x04\x42\x02\x30\x01\x12\x0b\n\x03ids\x18\x05 \x03(\t\x12\x16\n\x0eignore_indexes\x18\x06 \x03(\r\x12\x19\n\x11ignore_error_code\x18\x07 \x03(\r\"\xac\x01\n\x12InsertEdgesRequest\x12\'\n\nedge_table\x18\x01 \x01(\x0b\x32\x13.ultipa.EntityTable\x12\x0e\n\x06silent\x18\x02 \x01(\x08\x12\x12\n\ngraph_name\x18\x03 \x01(\t\x12 \n\x18\x63reate_node_if_not_exist\x18\x04 \x01(\x08\x12\'\n\x0binsert_type\x18\x05 \x01(\x0e\x32\x12.ultipa.InsertType\"\xa5\x01\n\x10InsertEdgesReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\x12\x11\n\ttime_cost\x18\x02 \x01(\x05\x12\x18\n\x10\x65ngine_time_cost\x18\x03 \x01(\x05\x12\x11\n\x05uuids\x18\x04 \x03(\x04\x42\x02\x30\x01\x12\x16\n\x0eignore_indexes\x18\x05 \x03(\r\x12\x19\n\x11ignore_error_code\x18\x06 \x03(\r\"C\n\x12InstallAlgoRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x0b\n\x03md5\x18\x02 \x01(\t\x12\r\n\x05\x63hunk\x18\x03 \x01(\x0c\"2\n\x10InstallAlgoReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\")\n\x14UninstallAlgoRequest\x12\x11\n\talgo_name\x18\x01 \x01(\t\"4\n\x12UninstallAlgoReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"\x96\x01\n\x0fUploaderRequest\x12\x1f\n\x07\x64\x62_type\x18\x01 \x01(\x0e\x32\x0e.ultipa.DBType\x12\x12\n\ngraph_name\x18\x02 \x01(\t\x12\x19\n\x11total_file_counts\x18\x03 \x01(\x04\x12\x11\n\tfile_name\x18\x04 \x01(\t\x12\x11\n\tfile_size\x18\x05 \x01(\x04\x12\r\n\x05\x63hunk\x18\x06 \x01(\x0c\"/\n\rUploaderReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"M\n\x1c\x43reateGraphByUploaderRequest\x12\x12\n\ngraph_name\x18\x01 \x01(\t\x12\x19\n\x11graph_description\x18\x02 \x01(\t\"<\n\x1a\x43reateGraphByUploaderReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"C\n\x12InstallExtaRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x0b\n\x03md5\x18\x02 \x01(\t\x12\r\n\x05\x63hunk\x18\x03 \x01(\x0c\"2\n\x10InstallExtaReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\")\n\x14UninstallExtaRequest\x12\x11\n\texta_name\x18\x01 \x01(\t\"4\n\x12UninstallExtaReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"$\n\rBackupRequest\x12\x13\n\x0b\x62\x61\x63kup_path\x18\x01 \x01(\t\"-\n\x0b\x42\x61\x63kupReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status\"g\n\x06Status\x12%\n\nerror_code\x18\x01 \x01(\x0e\x32\x11.ultipa.ErrorCode\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12)\n\x0c\x63luster_info\x18\x03 \x01(\x0b\x32\x13.ultipa.ClusterInfo\"S\n\x0cRaftFollower\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04role\x18\x02 \x01(\x05\x12$\n\x06status\x18\x03 \x01(\x0e\x32\x14.ultipa.ServerStatus\"`\n\x0b\x43lusterInfo\x12\x10\n\x08redirect\x18\x01 \x01(\t\x12\x16\n\x0eleader_address\x18\x02 \x01(\t\x12\'\n\tfollowers\x18\x03 \x03(\x0b\x32\x14.ultipa.RaftFollower\"X\n\x04Path\x12\'\n\nnode_table\x18\x01 \x01(\x0b\x32\x13.ultipa.EntityTable\x12\'\n\nedge_table\x18\x02 \x01(\x0b\x32\x13.ultipa.EntityTable\"b\n\x05Table\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x1f\n\x07headers\x18\x02 \x03(\x0b\x32\x0e.ultipa.Header\x12$\n\ntable_rows\x18\x03 \x03(\x0b\x32\x10.ultipa.TableRow\"\x1a\n\x08TableRow\x12\x0e\n\x06values\x18\x01 \x03(\x0c\"V\n\x0b\x45ntityTable\x12\x1f\n\x07schemas\x18\x01 \x03(\x0b\x32\x0e.ultipa.Schema\x12&\n\x0b\x65ntity_rows\x18\x03 \x03(\x0b\x32\x11.ultipa.EntityRow\"\xab\x01\n\tEntityRow\x12\x10\n\x04uuid\x18\x01 \x01(\x04\x42\x02\x30\x01\x12\n\n\x02id\x18\x02 \x01(\t\x12\x13\n\x0bschema_name\x18\x03 \x01(\t\x12\x15\n\tfrom_uuid\x18\x04 \x01(\x04\x42\x02\x30\x01\x12\x13\n\x07to_uuid\x18\x05 \x01(\x04\x42\x02\x30\x01\x12\x0f\n\x07\x66rom_id\x18\x06 \x01(\t\x12\r\n\x05to_id\x18\x07 \x01(\t\x12\x0e\n\x06values\x18\x08 \x03(\x0c\x12\x0f\n\x07is_null\x18\t \x01(\x08\"C\n\x06Schema\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12$\n\nproperties\x18\x02 \x03(\x0b\x32\x10.ultipa.Property\"w\n\x08Property\x12\x15\n\rproperty_name\x18\x01 \x01(\t\x12+\n\rproperty_type\x18\x02 \x01(\x0e\x32\x14.ultipa.PropertyType\x12\'\n\tsub_types\x18\x03 \x03(\x0e\x32\x14.ultipa.PropertyType\"L\n\x06Header\x12\x15\n\rproperty_name\x18\x01 \x01(\t\x12+\n\rproperty_type\x18\x02 \x01(\x0e\x32\x14.ultipa.PropertyType\"#\n\x05Value\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"+\n\x08ListData\x12\x0e\n\x06values\x18\x01 \x03(\x0c\x12\x0f\n\x07is_null\x18\x02 \x01(\x08\"*\n\x07SetData\x12\x0e\n\x06values\x18\x01 \x03(\x0c\x12\x0f\n\x07is_null\x18\x02 \x01(\x08\"&\n\x08MapValue\x12\x0b\n\x03key\x18\x01 \x01(\x0c\x12\r\n\x05value\x18\x02 \x01(\x0c\"<\n\x07MapData\x12 \n\x06values\x18\x01 \x03(\x0b\x32\x10.ultipa.MapValue\x12\x0f\n\x07is_null\x18\x02 \x01(\x08\"3\n\x0b\x45xplainPlan\x12$\n\nplan_nodes\x18\x01 \x03(\x0b\x32\x10.ultipa.PlanNode\"K\n\x08PlanNode\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\x14\n\x0c\x63hildren_num\x18\x02 \x01(\r\x12\x0b\n\x03uql\x18\x03 \x01(\t\x12\r\n\x05infos\x18\x04 \x01(\t\"J\n\x13\x41uthenticateRequest\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.ultipa.AuthenticateType\x12\x0b\n\x03uql\x18\x02 \x01(\t\"3\n\x11\x41uthenticateReply\x12\x1e\n\x06status\x18\x01 \x01(\x0b\x32\x0e.ultipa.Status*\x92\x01\n\nResultType\x12\x15\n\x11RESULT_TYPE_UNSET\x10\x00\x12\x14\n\x10RESULT_TYPE_PATH\x10\x01\x12\x14\n\x10RESULT_TYPE_NODE\x10\x02\x12\x14\n\x10RESULT_TYPE_EDGE\x10\x03\x12\x14\n\x10RESULT_TYPE_ATTR\x10\x04\x12\x15\n\x11RESULT_TYPE_TABLE\x10\x05*3\n\nInsertType\x12\n\n\x06NORMAL\x10\x00\x12\r\n\tOVERWRITE\x10\x01\x12\n\n\x06UPSERT\x10\x02*\xda\x01\n\x0cPropertyType\x12\t\n\x05UNSET\x10\x00\x12\t\n\x05INT32\x10\x01\x12\n\n\x06UINT32\x10\x02\x12\t\n\x05INT64\x10\x03\x12\n\n\x06UINT64\x10\x04\x12\t\n\x05\x46LOAT\x10\x05\x12\n\n\x06\x44OUBLE\x10\x06\x12\n\n\x06STRING\x10\x07\x12\x0c\n\x08\x44\x41TETIME\x10\x08\x12\r\n\tTIMESTAMP\x10\t\x12\x08\n\x04TEXT\x10\n\x12\x08\n\x04\x42LOB\x10\x0b\x12\t\n\x05POINT\x10\x0c\x12\x0b\n\x07\x44\x45\x43IMAL\x10\r\x12\x08\n\x04LIST\x10\x0e\x12\x07\n\x03SET\x10\x0f\x12\x07\n\x03MAP\x10\x10\x12\t\n\x05NULL_\x10\x11*\xb2\x02\n\tErrorCode\x12\x0b\n\x07SUCCESS\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\x0f\n\x0bPARAM_ERROR\x10\x02\x12\x11\n\rBASE_DB_ERROR\x10\x03\x12\x10\n\x0c\x45NGINE_ERROR\x10\x04\x12\x10\n\x0cSYSTEM_ERROR\x10\x05\x12\x11\n\rRAFT_REDIRECT\x10\x06\x12\x1f\n\x1bRAFT_LEADER_NOT_YET_ELECTED\x10\x07\x12\x12\n\x0eRAFT_LOG_ERROR\x10\x08\x12\r\n\tUQL_ERROR\x10\t\x12\x11\n\rNOT_RAFT_MODE\x10\n\x12\x1f\n\x1bRAFT_NO_AVAILABLE_FOLLOWERS\x10\x0b\x12\"\n\x1eRAFT_NO_AVAILABLE_ALGO_SERVERS\x10\x0c\x12\x15\n\x11PERMISSION_DENIED\x10\r*]\n\x0c\x46ollowerRole\x12\x0e\n\nROLE_UNSET\x10\x00\x12\x11\n\rROLE_READABLE\x10\x01\x12\x18\n\x14ROLE_ALGO_EXECUTABLE\x10\x02\x12\x10\n\x0cROLE_LEARNER\x10\x04*#\n\x0cServerStatus\x12\x08\n\x04\x44\x45\x41\x44\x10\x00\x12\t\n\x05\x41LIVE\x10\x01*.\n\x06\x44\x42Type\x12\n\n\x06\x44\x42NODE\x10\x00\x12\n\n\x06\x44\x42\x45\x44GE\x10\x01\x12\x0c\n\x08\x44\x42GLOBAL\x10\x02*w\n\x0bTASK_STATUS\x12\x10\n\x0cTASK_PENDING\x10\x00\x12\x12\n\x0eTASK_COMPUTING\x10\x01\x12\x10\n\x0cTASK_WRITING\x10\x02\x12\r\n\tTASK_DONE\x10\x03\x12\x0f\n\x0bTASK_FAILED\x10\x04\x12\x10\n\x0cTASK_STOPPED\x10\x05*\xfc\x02\n\x10\x41uthenticateType\x12\x17\n\x13PERMISSION_TYPE_UQL\x10\x00\x12\x1f\n\x1bPERMISSION_TYPE_INSERTNODES\x10\x01\x12\x1f\n\x1bPERMISSION_TYPE_INSERTEDGES\x10\x02\x12\x1a\n\x16PERMISSION_TYPE_EXPORT\x10\x03\x12 \n\x1cPERMISSION_TYPE_DOWNLOADFILE\x10\x04\x12\x1f\n\x1bPERMISSION_TYPE_INSTALLALGO\x10\x05\x12!\n\x1dPERMISSION_TYPE_UNINSTALLALGO\x10\x06\x12\x1c\n\x18PERMISSION_TYPE_UPLOADER\x10\x07\x12)\n%PERMISSION_TYPE_CREATEGRAPHBYUPLOADER\x10\x08\x12\x1f\n\x1bPERMISSION_TYPE_INSTALLEXTA\x10\t\x12!\n\x1dPERMISSION_TYPE_UNINSTALLEXTA\x10\n2\x8f\x02\n\nUltipaRpcs\x12\x42\n\x08SayHello\x12\x1a.ultipa.HelloUltipaRequest\x1a\x18.ultipa.HelloUltipaReply\"\x00\x12/\n\x03Uql\x12\x12.ultipa.UqlRequest\x1a\x10.ultipa.UqlReply\"\x00\x30\x01\x12\x45\n\x0bInsertNodes\x12\x1a.ultipa.InsertNodesRequest\x1a\x18.ultipa.InsertNodesReply\"\x00\x12\x45\n\x0bInsertEdges\x12\x1a.ultipa.InsertEdgesRequest\x1a\x18.ultipa.InsertEdgesReply\"\x00\x32\xec\x07\n\x0eUltipaControls\x12\x42\n\x08SayHello\x12\x1a.ultipa.HelloUltipaRequest\x1a\x18.ultipa.HelloUltipaReply\"\x00\x12\x45\n\x0bUserSetting\x12\x1a.ultipa.UserSettingRequest\x1a\x18.ultipa.UserSettingReply\"\x00\x12?\n\tGetLeader\x12\x18.ultipa.GetLeaderRequest\x1a\x16.ultipa.GetLeaderReply\"\x00\x12\x31\n\x05UqlEx\x12\x12.ultipa.UqlRequest\x1a\x10.ultipa.UqlReply\"\x00\x30\x01\x12\x38\n\x06\x45xport\x12\x15.ultipa.ExportRequest\x1a\x13.ultipa.ExportReply\"\x00\x30\x01\x12N\n\x0e\x44ownloadFileV2\x12\x1d.ultipa.DownloadFileRequestV2\x1a\x19.ultipa.DownloadFileReply\"\x00\x30\x01\x12G\n\x0bInstallAlgo\x12\x1a.ultipa.InstallAlgoRequest\x1a\x18.ultipa.InstallAlgoReply\"\x00(\x01\x12K\n\rUninstallAlgo\x12\x1c.ultipa.UninstallAlgoRequest\x1a\x1a.ultipa.UninstallAlgoReply\"\x00\x12>\n\x08Uploader\x12\x17.ultipa.UploaderRequest\x1a\x15.ultipa.UploaderReply\"\x00(\x01\x12\x63\n\x15\x43reateGraphByUploader\x12$.ultipa.CreateGraphByUploaderRequest\x1a\".ultipa.CreateGraphByUploaderReply\"\x00\x12G\n\x0bInstallExta\x12\x1a.ultipa.InstallExtaRequest\x1a\x18.ultipa.InstallExtaReply\"\x00(\x01\x12K\n\rUninstallExta\x12\x1c.ultipa.UninstallExtaRequest\x1a\x1a.ultipa.UninstallExtaReply\"\x00\x12H\n\x0c\x41uthenticate\x12\x1b.ultipa.AuthenticateRequest\x1a\x19.ultipa.AuthenticateReply\"\x00\x12\x36\n\x06\x42\x61\x63kup\x12\x15.ultipa.BackupRequest\x1a\x13.ultipa.BackupReply\"\x00\x62\x06proto3')
 
 _RESULTTYPE = DESCRIPTOR.enum_types_by_name['ResultType']
 ResultType = enum_type_wrapper.EnumTypeWrapper(_RESULTTYPE)
 _INSERTTYPE = DESCRIPTOR.enum_types_by_name['InsertType']
 InsertType = enum_type_wrapper.EnumTypeWrapper(_INSERTTYPE)
 _PROPERTYTYPE = DESCRIPTOR.enum_types_by_name['PropertyType']
 PropertyType = enum_type_wrapper.EnumTypeWrapper(_PROPERTYTYPE)
@@ -29,25 +29,22 @@
 FollowerRole = enum_type_wrapper.EnumTypeWrapper(_FOLLOWERROLE)
 _SERVERSTATUS = DESCRIPTOR.enum_types_by_name['ServerStatus']
 ServerStatus = enum_type_wrapper.EnumTypeWrapper(_SERVERSTATUS)
 _DBTYPE = DESCRIPTOR.enum_types_by_name['DBType']
 DBType = enum_type_wrapper.EnumTypeWrapper(_DBTYPE)
 _TASK_STATUS = DESCRIPTOR.enum_types_by_name['TASK_STATUS']
 TASK_STATUS = enum_type_wrapper.EnumTypeWrapper(_TASK_STATUS)
-_PLANNODETYPE = DESCRIPTOR.enum_types_by_name['PlanNodeType']
-PlanNodeType = enum_type_wrapper.EnumTypeWrapper(_PLANNODETYPE)
 _AUTHENTICATETYPE = DESCRIPTOR.enum_types_by_name['AuthenticateType']
 AuthenticateType = enum_type_wrapper.EnumTypeWrapper(_AUTHENTICATETYPE)
 RESULT_TYPE_UNSET = 0
 RESULT_TYPE_PATH = 1
 RESULT_TYPE_NODE = 2
 RESULT_TYPE_EDGE = 3
 RESULT_TYPE_ATTR = 4
-RESULT_TYPE_ARRAY = 5
-RESULT_TYPE_TABLE = 6
+RESULT_TYPE_TABLE = 5
 NORMAL = 0
 OVERWRITE = 1
 UPSERT = 2
 UNSET = 0
 INT32 = 1
 UINT32 = 2
 INT64 = 3
@@ -55,14 +52,20 @@
 FLOAT = 5
 DOUBLE = 6
 STRING = 7
 DATETIME = 8
 TIMESTAMP = 9
 TEXT = 10
 BLOB = 11
+POINT = 12
+DECIMAL = 13
+LIST = 14
+SET = 15
+MAP = 16
+NULL_ = 17
 SUCCESS = 0
 FAILED = 1
 PARAM_ERROR = 2
 BASE_DB_ERROR = 3
 ENGINE_ERROR = 4
 SYSTEM_ERROR = 5
 RAFT_REDIRECT = 6
@@ -84,90 +87,14 @@
 DBGLOBAL = 2
 TASK_PENDING = 0
 TASK_COMPUTING = 1
 TASK_WRITING = 2
 TASK_DONE = 3
 TASK_FAILED = 4
 TASK_STOPPED = 5
-CLAUSE_UNSET = 0
-ORDER_BY_CLAUSE = 1
-AGGREGATION_CLAUSE = 2
-WITH_CLAUSE = 3
-WHERE_CLAUSE = 4
-UNCOLLECT_CLAUSE = 5
-TABLE_CLAUSE = 6
-RETURN_CLAUSE = 7
-LIMIT_SKIP_CLAUSE = 8
-TEMPLATE_CLAUSE = 9
-KHOP_TEMPLATE_CLAUSE = 10
-KHOP_CLAUSE = 11
-AB_CLAUSE = 12
-SPREAD_CLAUSE = 13
-AUTO_NET_CLAUSE = 14
-NODE_SEARCH_CLAUSE = 15
-EDGE_SEARCH_CLAUSE = 16
-NODE_INSERT_CLAUSE = 17
-EDGE_INSERT_CLAUSE = 18
-NODE_UPSERT_CLAUSE = 19
-EDGE_UPSERT_CLAUSE = 20
-NODE_UPDATE_CLAUSE = 21
-EDGE_UPDATE_CLAUSE = 22
-NODE_DELETE_CLAUSE = 23
-EDGE_DELETE_CLAUSE = 24
-TRUNCATE_CLAUSE = 25
-COMPACT_CLAUSE = 26
-GRAPH_CREATE_CLAUSE = 27
-GRAPH_DROP_CLAUSE = 28
-GRAPH_UPDATE_CLAUSE = 29
-GRAPH_SHOW_CLAUSE = 30
-GRAPH_MOUNT_CLAUSE = 31
-GRAPH_UNMOUNT_CLAUSE = 32
-SCHEMA_CREATE_CLAUSE = 33
-SCHEMA_DROP_CLAUSE = 34
-SCHEMA_ALTER_CLAUSE = 35
-SCHEMA_SHOW_CLAUSE = 36
-PROPERTY_CREATE_CLAUSE = 37
-PROPERTY_DROP_CLAUSE = 38
-PROPERTY_ALTER_CLAUSE = 39
-PROPERTY_SHOW_CLAUSE = 40
-FULLTEXT_CREATE_CLAUSE = 41
-FULLTEXT_DROP_CLAUSE = 42
-FULLTEXT_SHOW_CLAUSE = 43
-INDEX_CREATE_CLAUSE = 44
-INDEX_DROP_CLAUSE = 45
-INDEX_SHOW_CLAUSE = 46
-LTE_CLAUSE = 47
-UFE_CLAUSE = 48
-TASK_CLEAR_CLAUSE = 49
-TASK_STOP_CLAUSE = 50
-TASK_PAUSE_CLAUSE = 51
-TASK_RESUME_CLAUSE = 52
-TASK_SHOW_CLAUSE = 53
-TOP_CLAUSE = 54
-KILL_CLAUSE = 55
-STAT_CLAUSE = 56
-POLICY_SHOW_CLAUSE = 57
-POLICY_CREATE_CLAUSE = 58
-POLICY_DELETE_CLAUSE = 59
-POLICY_UPDATE_CLAUSE = 60
-USER_SHOW_CLAUSE = 61
-USER_CREATE_CLAUSE = 62
-USER_DELETE_CLAUSE = 63
-USER_UPDATE_CLAUSE = 64
-PRIVILEGE_SHOW_CLAUSE = 65
-GRANT_CLAUSE = 66
-REVOKE_CLAUSE = 67
-SELF_INFO_GET_CLAUSE = 68
-ALGO_CLAUSE = 69
-ALGO_WRITE_CLAUSE = 70
-ALGO_LIST_CLAUSE = 71
-SUB_GRAPH_CLAUSE = 72
-OPTIONAL_TEMPLATE_CLAUSE = 73
-SUBQUERY_CLAUSE = 74
-UNION_CLAUSE = 75
 PERMISSION_TYPE_UQL = 0
 PERMISSION_TYPE_INSERTNODES = 1
 PERMISSION_TYPE_INSERTEDGES = 2
 PERMISSION_TYPE_EXPORT = 3
 PERMISSION_TYPE_DOWNLOADFILE = 4
 PERMISSION_TYPE_INSTALLALGO = 5
 PERMISSION_TYPE_UNINSTALLALGO = 6
@@ -182,16 +109,17 @@
 _UQLREQUEST = DESCRIPTOR.message_types_by_name['UqlRequest']
 _RESULTALIAS = DESCRIPTOR.message_types_by_name['ResultAlias']
 _UQLREPLY = DESCRIPTOR.message_types_by_name['UqlReply']
 _PATHALIAS = DESCRIPTOR.message_types_by_name['PathAlias']
 _EDGEALIAS = DESCRIPTOR.message_types_by_name['EdgeAlias']
 _NODEALIAS = DESCRIPTOR.message_types_by_name['NodeAlias']
 _ATTRALIAS = DESCRIPTOR.message_types_by_name['AttrAlias']
-_ARRAYELEMENT = DESCRIPTOR.message_types_by_name['ArrayElement']
-_ARRAYALIAS = DESCRIPTOR.message_types_by_name['ArrayAlias']
+_ATTR = DESCRIPTOR.message_types_by_name['Attr']
+_ATTRLISTDATA = DESCRIPTOR.message_types_by_name['AttrListData']
+_ATTRMAPDATA = DESCRIPTOR.message_types_by_name['AttrMapData']
 _USERSETTINGREQUEST = DESCRIPTOR.message_types_by_name['UserSettingRequest']
 _USERSETTINGREPLY = DESCRIPTOR.message_types_by_name['UserSettingReply']
 _DOWNLOADFILEREQUESTV2 = DESCRIPTOR.message_types_by_name['DownloadFileRequestV2']
 _DOWNLOADFILEREPLY = DESCRIPTOR.message_types_by_name['DownloadFileReply']
 _EXPORTREQUEST = DESCRIPTOR.message_types_by_name['ExportRequest']
 _EXPORTREPLY = DESCRIPTOR.message_types_by_name['ExportReply']
 _GETLEADERREQUEST = DESCRIPTOR.message_types_by_name['GetLeaderRequest']
@@ -208,28 +136,32 @@
 _UPLOADERREPLY = DESCRIPTOR.message_types_by_name['UploaderReply']
 _CREATEGRAPHBYUPLOADERREQUEST = DESCRIPTOR.message_types_by_name['CreateGraphByUploaderRequest']
 _CREATEGRAPHBYUPLOADERREPLY = DESCRIPTOR.message_types_by_name['CreateGraphByUploaderReply']
 _INSTALLEXTAREQUEST = DESCRIPTOR.message_types_by_name['InstallExtaRequest']
 _INSTALLEXTAREPLY = DESCRIPTOR.message_types_by_name['InstallExtaReply']
 _UNINSTALLEXTAREQUEST = DESCRIPTOR.message_types_by_name['UninstallExtaRequest']
 _UNINSTALLEXTAREPLY = DESCRIPTOR.message_types_by_name['UninstallExtaReply']
+_BACKUPREQUEST = DESCRIPTOR.message_types_by_name['BackupRequest']
+_BACKUPREPLY = DESCRIPTOR.message_types_by_name['BackupReply']
 _STATUS = DESCRIPTOR.message_types_by_name['Status']
 _RAFTFOLLOWER = DESCRIPTOR.message_types_by_name['RaftFollower']
 _CLUSTERINFO = DESCRIPTOR.message_types_by_name['ClusterInfo']
 _PATH = DESCRIPTOR.message_types_by_name['Path']
 _TABLE = DESCRIPTOR.message_types_by_name['Table']
 _TABLEROW = DESCRIPTOR.message_types_by_name['TableRow']
-_NODETABLE = DESCRIPTOR.message_types_by_name['NodeTable']
-_EDGETABLE = DESCRIPTOR.message_types_by_name['EdgeTable']
-_NODEROW = DESCRIPTOR.message_types_by_name['NodeRow']
-_EDGEROW = DESCRIPTOR.message_types_by_name['EdgeRow']
+_ENTITYTABLE = DESCRIPTOR.message_types_by_name['EntityTable']
+_ENTITYROW = DESCRIPTOR.message_types_by_name['EntityRow']
 _SCHEMA = DESCRIPTOR.message_types_by_name['Schema']
 _PROPERTY = DESCRIPTOR.message_types_by_name['Property']
 _HEADER = DESCRIPTOR.message_types_by_name['Header']
 _VALUE = DESCRIPTOR.message_types_by_name['Value']
+_LISTDATA = DESCRIPTOR.message_types_by_name['ListData']
+_SETDATA = DESCRIPTOR.message_types_by_name['SetData']
+_MAPVALUE = DESCRIPTOR.message_types_by_name['MapValue']
+_MAPDATA = DESCRIPTOR.message_types_by_name['MapData']
 _EXPLAINPLAN = DESCRIPTOR.message_types_by_name['ExplainPlan']
 _PLANNODE = DESCRIPTOR.message_types_by_name['PlanNode']
 _AUTHENTICATEREQUEST = DESCRIPTOR.message_types_by_name['AuthenticateRequest']
 _AUTHENTICATEREPLY = DESCRIPTOR.message_types_by_name['AuthenticateReply']
 _USERSETTINGREQUEST_OPTION = _USERSETTINGREQUEST.enum_types_by_name['OPTION']
 HelloUltipaRequest = _reflection.GeneratedProtocolMessageType('HelloUltipaRequest', (_message.Message,), {
   'DESCRIPTOR' : _HELLOULTIPAREQUEST,
@@ -290,27 +222,34 @@
 AttrAlias = _reflection.GeneratedProtocolMessageType('AttrAlias', (_message.Message,), {
   'DESCRIPTOR' : _ATTRALIAS,
   '__module__' : 'ultipa_pb2'
   # @@protoc_insertion_point(class_scope:ultipa.AttrAlias)
   })
 _sym_db.RegisterMessage(AttrAlias)
 
-ArrayElement = _reflection.GeneratedProtocolMessageType('ArrayElement', (_message.Message,), {
-  'DESCRIPTOR' : _ARRAYELEMENT,
+Attr = _reflection.GeneratedProtocolMessageType('Attr', (_message.Message,), {
+  'DESCRIPTOR' : _ATTR,
   '__module__' : 'ultipa_pb2'
-  # @@protoc_insertion_point(class_scope:ultipa.ArrayElement)
+  # @@protoc_insertion_point(class_scope:ultipa.Attr)
   })
-_sym_db.RegisterMessage(ArrayElement)
+_sym_db.RegisterMessage(Attr)
 
-ArrayAlias = _reflection.GeneratedProtocolMessageType('ArrayAlias', (_message.Message,), {
-  'DESCRIPTOR' : _ARRAYALIAS,
+AttrListData = _reflection.GeneratedProtocolMessageType('AttrListData', (_message.Message,), {
+  'DESCRIPTOR' : _ATTRLISTDATA,
   '__module__' : 'ultipa_pb2'
-  # @@protoc_insertion_point(class_scope:ultipa.ArrayAlias)
+  # @@protoc_insertion_point(class_scope:ultipa.AttrListData)
   })
-_sym_db.RegisterMessage(ArrayAlias)
+_sym_db.RegisterMessage(AttrListData)
+
+AttrMapData = _reflection.GeneratedProtocolMessageType('AttrMapData', (_message.Message,), {
+  'DESCRIPTOR' : _ATTRMAPDATA,
+  '__module__' : 'ultipa_pb2'
+  # @@protoc_insertion_point(class_scope:ultipa.AttrMapData)
+  })
+_sym_db.RegisterMessage(AttrMapData)
 
 UserSettingRequest = _reflection.GeneratedProtocolMessageType('UserSettingRequest', (_message.Message,), {
   'DESCRIPTOR' : _USERSETTINGREQUEST,
   '__module__' : 'ultipa_pb2'
   # @@protoc_insertion_point(class_scope:ultipa.UserSettingRequest)
   })
 _sym_db.RegisterMessage(UserSettingRequest)
@@ -472,14 +411,28 @@
 UninstallExtaReply = _reflection.GeneratedProtocolMessageType('UninstallExtaReply', (_message.Message,), {
   'DESCRIPTOR' : _UNINSTALLEXTAREPLY,
   '__module__' : 'ultipa_pb2'
   # @@protoc_insertion_point(class_scope:ultipa.UninstallExtaReply)
   })
 _sym_db.RegisterMessage(UninstallExtaReply)
 
+BackupRequest = _reflection.GeneratedProtocolMessageType('BackupRequest', (_message.Message,), {
+  'DESCRIPTOR' : _BACKUPREQUEST,
+  '__module__' : 'ultipa_pb2'
+  # @@protoc_insertion_point(class_scope:ultipa.BackupRequest)
+  })
+_sym_db.RegisterMessage(BackupRequest)
+
+BackupReply = _reflection.GeneratedProtocolMessageType('BackupReply', (_message.Message,), {
+  'DESCRIPTOR' : _BACKUPREPLY,
+  '__module__' : 'ultipa_pb2'
+  # @@protoc_insertion_point(class_scope:ultipa.BackupReply)
+  })
+_sym_db.RegisterMessage(BackupReply)
+
 Status = _reflection.GeneratedProtocolMessageType('Status', (_message.Message,), {
   'DESCRIPTOR' : _STATUS,
   '__module__' : 'ultipa_pb2'
   # @@protoc_insertion_point(class_scope:ultipa.Status)
   })
 _sym_db.RegisterMessage(Status)
 
@@ -514,41 +467,27 @@
 TableRow = _reflection.GeneratedProtocolMessageType('TableRow', (_message.Message,), {
   'DESCRIPTOR' : _TABLEROW,
   '__module__' : 'ultipa_pb2'
   # @@protoc_insertion_point(class_scope:ultipa.TableRow)
   })
 _sym_db.RegisterMessage(TableRow)
 
-NodeTable = _reflection.GeneratedProtocolMessageType('NodeTable', (_message.Message,), {
-  'DESCRIPTOR' : _NODETABLE,
+EntityTable = _reflection.GeneratedProtocolMessageType('EntityTable', (_message.Message,), {
+  'DESCRIPTOR' : _ENTITYTABLE,
   '__module__' : 'ultipa_pb2'
-  # @@protoc_insertion_point(class_scope:ultipa.NodeTable)
+  # @@protoc_insertion_point(class_scope:ultipa.EntityTable)
   })
-_sym_db.RegisterMessage(NodeTable)
+_sym_db.RegisterMessage(EntityTable)
 
-EdgeTable = _reflection.GeneratedProtocolMessageType('EdgeTable', (_message.Message,), {
-  'DESCRIPTOR' : _EDGETABLE,
+EntityRow = _reflection.GeneratedProtocolMessageType('EntityRow', (_message.Message,), {
+  'DESCRIPTOR' : _ENTITYROW,
   '__module__' : 'ultipa_pb2'
-  # @@protoc_insertion_point(class_scope:ultipa.EdgeTable)
+  # @@protoc_insertion_point(class_scope:ultipa.EntityRow)
   })
-_sym_db.RegisterMessage(EdgeTable)
-
-NodeRow = _reflection.GeneratedProtocolMessageType('NodeRow', (_message.Message,), {
-  'DESCRIPTOR' : _NODEROW,
-  '__module__' : 'ultipa_pb2'
-  # @@protoc_insertion_point(class_scope:ultipa.NodeRow)
-  })
-_sym_db.RegisterMessage(NodeRow)
-
-EdgeRow = _reflection.GeneratedProtocolMessageType('EdgeRow', (_message.Message,), {
-  'DESCRIPTOR' : _EDGEROW,
-  '__module__' : 'ultipa_pb2'
-  # @@protoc_insertion_point(class_scope:ultipa.EdgeRow)
-  })
-_sym_db.RegisterMessage(EdgeRow)
+_sym_db.RegisterMessage(EntityRow)
 
 Schema = _reflection.GeneratedProtocolMessageType('Schema', (_message.Message,), {
   'DESCRIPTOR' : _SCHEMA,
   '__module__' : 'ultipa_pb2'
   # @@protoc_insertion_point(class_scope:ultipa.Schema)
   })
 _sym_db.RegisterMessage(Schema)
@@ -570,14 +509,42 @@
 Value = _reflection.GeneratedProtocolMessageType('Value', (_message.Message,), {
   'DESCRIPTOR' : _VALUE,
   '__module__' : 'ultipa_pb2'
   # @@protoc_insertion_point(class_scope:ultipa.Value)
   })
 _sym_db.RegisterMessage(Value)
 
+ListData = _reflection.GeneratedProtocolMessageType('ListData', (_message.Message,), {
+  'DESCRIPTOR' : _LISTDATA,
+  '__module__' : 'ultipa_pb2'
+  # @@protoc_insertion_point(class_scope:ultipa.ListData)
+  })
+_sym_db.RegisterMessage(ListData)
+
+SetData = _reflection.GeneratedProtocolMessageType('SetData', (_message.Message,), {
+  'DESCRIPTOR' : _SETDATA,
+  '__module__' : 'ultipa_pb2'
+  # @@protoc_insertion_point(class_scope:ultipa.SetData)
+  })
+_sym_db.RegisterMessage(SetData)
+
+MapValue = _reflection.GeneratedProtocolMessageType('MapValue', (_message.Message,), {
+  'DESCRIPTOR' : _MAPVALUE,
+  '__module__' : 'ultipa_pb2'
+  # @@protoc_insertion_point(class_scope:ultipa.MapValue)
+  })
+_sym_db.RegisterMessage(MapValue)
+
+MapData = _reflection.GeneratedProtocolMessageType('MapData', (_message.Message,), {
+  'DESCRIPTOR' : _MAPDATA,
+  '__module__' : 'ultipa_pb2'
+  # @@protoc_insertion_point(class_scope:ultipa.MapData)
+  })
+_sym_db.RegisterMessage(MapData)
+
 ExplainPlan = _reflection.GeneratedProtocolMessageType('ExplainPlan', (_message.Message,), {
   'DESCRIPTOR' : _EXPLAINPLAN,
   '__module__' : 'ultipa_pb2'
   # @@protoc_insertion_point(class_scope:ultipa.ExplainPlan)
   })
 _sym_db.RegisterMessage(ExplainPlan)
 
@@ -607,148 +574,154 @@
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _INSERTNODESREPLY.fields_by_name['uuids']._options = None
   _INSERTNODESREPLY.fields_by_name['uuids']._serialized_options = b'0\001'
   _INSERTEDGESREPLY.fields_by_name['uuids']._options = None
   _INSERTEDGESREPLY.fields_by_name['uuids']._serialized_options = b'0\001'
-  _NODEROW.fields_by_name['uuid']._options = None
-  _NODEROW.fields_by_name['uuid']._serialized_options = b'0\001'
-  _EDGEROW.fields_by_name['uuid']._options = None
-  _EDGEROW.fields_by_name['uuid']._serialized_options = b'0\001'
-  _EDGEROW.fields_by_name['from_uuid']._options = None
-  _EDGEROW.fields_by_name['from_uuid']._serialized_options = b'0\001'
-  _EDGEROW.fields_by_name['to_uuid']._options = None
-  _EDGEROW.fields_by_name['to_uuid']._serialized_options = b'0\001'
-  _RESULTTYPE._serialized_start=4701
-  _RESULTTYPE._serialized_end=4870
-  _INSERTTYPE._serialized_start=4872
-  _INSERTTYPE._serialized_end=4923
-  _PROPERTYTYPE._serialized_start=4926
-  _PROPERTYTYPE._serialized_end=5081
-  _ERRORCODE._serialized_start=5084
-  _ERRORCODE._serialized_end=5390
-  _FOLLOWERROLE._serialized_start=5392
-  _FOLLOWERROLE._serialized_end=5485
-  _SERVERSTATUS._serialized_start=5487
-  _SERVERSTATUS._serialized_end=5522
-  _DBTYPE._serialized_start=5524
-  _DBTYPE._serialized_end=5570
-  _TASK_STATUS._serialized_start=5572
-  _TASK_STATUS._serialized_end=5691
-  _PLANNODETYPE._serialized_start=5694
-  _PLANNODETYPE._serialized_end=7426
-  _AUTHENTICATETYPE._serialized_start=7429
-  _AUTHENTICATETYPE._serialized_end=7809
+  _ENTITYROW.fields_by_name['uuid']._options = None
+  _ENTITYROW.fields_by_name['uuid']._serialized_options = b'0\001'
+  _ENTITYROW.fields_by_name['from_uuid']._options = None
+  _ENTITYROW.fields_by_name['from_uuid']._serialized_options = b'0\001'
+  _ENTITYROW.fields_by_name['to_uuid']._options = None
+  _ENTITYROW.fields_by_name['to_uuid']._serialized_options = b'0\001'
+  _RESULTTYPE._serialized_start=5027
+  _RESULTTYPE._serialized_end=5173
+  _INSERTTYPE._serialized_start=5175
+  _INSERTTYPE._serialized_end=5226
+  _PROPERTYTYPE._serialized_start=5229
+  _PROPERTYTYPE._serialized_end=5447
+  _ERRORCODE._serialized_start=5450
+  _ERRORCODE._serialized_end=5756
+  _FOLLOWERROLE._serialized_start=5758
+  _FOLLOWERROLE._serialized_end=5851
+  _SERVERSTATUS._serialized_start=5853
+  _SERVERSTATUS._serialized_end=5888
+  _DBTYPE._serialized_start=5890
+  _DBTYPE._serialized_end=5936
+  _TASK_STATUS._serialized_start=5938
+  _TASK_STATUS._serialized_end=6057
+  _AUTHENTICATETYPE._serialized_start=6060
+  _AUTHENTICATETYPE._serialized_end=6440
   _HELLOULTIPAREQUEST._serialized_start=24
   _HELLOULTIPAREQUEST._serialized_end=58
   _HELLOULTIPAREPLY._serialized_start=60
   _HELLOULTIPAREPLY._serialized_end=127
-  _UQLREQUEST._serialized_start=129
-  _UQLREQUEST._serialized_end=230
-  _RESULTALIAS._serialized_start=232
-  _RESULTALIAS._serialized_end=301
-  _UQLREPLY._serialized_start=304
-  _UQLREPLY._serialized_end=714
-  _PATHALIAS._serialized_start=716
-  _PATHALIAS._serialized_end=771
-  _EDGEALIAS._serialized_start=773
-  _EDGEALIAS._serialized_end=838
-  _NODEALIAS._serialized_start=840
+  _UQLREQUEST._serialized_start=130
+  _UQLREQUEST._serialized_end=262
+  _RESULTALIAS._serialized_start=264
+  _RESULTALIAS._serialized_end=333
+  _UQLREPLY._serialized_start=336
+  _UQLREPLY._serialized_end=710
+  _PATHALIAS._serialized_start=712
+  _PATHALIAS._serialized_end=767
+  _EDGEALIAS._serialized_start=769
+  _EDGEALIAS._serialized_end=836
+  _NODEALIAS._serialized_start=838
   _NODEALIAS._serialized_end=905
   _ATTRALIAS._serialized_start=907
-  _ATTRALIAS._serialized_end=994
-  _ARRAYELEMENT._serialized_start=996
-  _ARRAYELEMENT._serialized_end=1026
-  _ARRAYALIAS._serialized_start=1028
-  _ARRAYALIAS._serialized_end=1140
-  _USERSETTINGREQUEST._serialized_start=1143
-  _USERSETTINGREQUEST._serialized_end=1294
-  _USERSETTINGREQUEST_OPTION._serialized_start=1260
-  _USERSETTINGREQUEST_OPTION._serialized_end=1294
-  _USERSETTINGREPLY._serialized_start=1296
-  _USERSETTINGREPLY._serialized_end=1360
-  _DOWNLOADFILEREQUESTV2._serialized_start=1362
-  _DOWNLOADFILEREQUESTV2._serialized_end=1421
-  _DOWNLOADFILEREPLY._serialized_start=1423
-  _DOWNLOADFILEREPLY._serialized_end=1509
-  _EXPORTREQUEST._serialized_start=1511
-  _EXPORTREQUEST._serialized_end=1617
-  _EXPORTREPLY._serialized_start=1619
-  _EXPORTREPLY._serialized_end=1742
-  _GETLEADERREQUEST._serialized_start=1744
-  _GETLEADERREQUEST._serialized_end=1762
-  _GETLEADERREPLY._serialized_start=1764
-  _GETLEADERREPLY._serialized_end=1812
-  _INSERTNODESREQUEST._serialized_start=1815
-  _INSERTNODESREQUEST._serialized_end=1951
-  _INSERTNODESREPLY._serialized_start=1954
-  _INSERTNODESREPLY._serialized_end=2132
-  _INSERTEDGESREQUEST._serialized_start=2135
-  _INSERTEDGESREQUEST._serialized_end=2305
-  _INSERTEDGESREPLY._serialized_start=2308
-  _INSERTEDGESREPLY._serialized_end=2473
-  _INSTALLALGOREQUEST._serialized_start=2475
-  _INSTALLALGOREQUEST._serialized_end=2542
-  _INSTALLALGOREPLY._serialized_start=2544
-  _INSTALLALGOREPLY._serialized_end=2594
-  _UNINSTALLALGOREQUEST._serialized_start=2596
-  _UNINSTALLALGOREQUEST._serialized_end=2637
-  _UNINSTALLALGOREPLY._serialized_start=2639
-  _UNINSTALLALGOREPLY._serialized_end=2691
-  _UPLOADERREQUEST._serialized_start=2694
-  _UPLOADERREQUEST._serialized_end=2844
-  _UPLOADERREPLY._serialized_start=2846
-  _UPLOADERREPLY._serialized_end=2893
-  _CREATEGRAPHBYUPLOADERREQUEST._serialized_start=2895
-  _CREATEGRAPHBYUPLOADERREQUEST._serialized_end=2972
-  _CREATEGRAPHBYUPLOADERREPLY._serialized_start=2974
-  _CREATEGRAPHBYUPLOADERREPLY._serialized_end=3034
-  _INSTALLEXTAREQUEST._serialized_start=3036
-  _INSTALLEXTAREQUEST._serialized_end=3103
-  _INSTALLEXTAREPLY._serialized_start=3105
-  _INSTALLEXTAREPLY._serialized_end=3155
-  _UNINSTALLEXTAREQUEST._serialized_start=3157
-  _UNINSTALLEXTAREQUEST._serialized_end=3198
-  _UNINSTALLEXTAREPLY._serialized_start=3200
-  _UNINSTALLEXTAREPLY._serialized_end=3252
-  _STATUS._serialized_start=3254
-  _STATUS._serialized_end=3357
-  _RAFTFOLLOWER._serialized_start=3359
-  _RAFTFOLLOWER._serialized_end=3442
-  _CLUSTERINFO._serialized_start=3444
-  _CLUSTERINFO._serialized_end=3540
-  _PATH._serialized_start=3542
-  _PATH._serialized_end=3626
-  _TABLE._serialized_start=3628
-  _TABLE._serialized_end=3726
-  _TABLEROW._serialized_start=3728
-  _TABLEROW._serialized_end=3754
-  _NODETABLE._serialized_start=3756
-  _NODETABLE._serialized_end=3836
-  _EDGETABLE._serialized_start=3838
-  _EDGETABLE._serialized_end=3918
-  _NODEROW._serialized_start=3920
-  _NODEROW._serialized_end=3996
-  _EDGEROW._serialized_start=3999
-  _EDGEROW._serialized_end=4139
-  _SCHEMA._serialized_start=4141
-  _SCHEMA._serialized_end=4208
-  _PROPERTY._serialized_start=4210
-  _PROPERTY._serialized_end=4288
-  _HEADER._serialized_start=4290
-  _HEADER._serialized_end=4366
-  _VALUE._serialized_start=4368
-  _VALUE._serialized_end=4403
-  _EXPLAINPLAN._serialized_start=4405
-  _EXPLAINPLAN._serialized_end=4456
-  _PLANNODE._serialized_start=4458
-  _PLANNODE._serialized_end=4569
-  _AUTHENTICATEREQUEST._serialized_start=4571
-  _AUTHENTICATEREQUEST._serialized_end=4645
-  _AUTHENTICATEREPLY._serialized_start=4647
-  _AUTHENTICATEREPLY._serialized_end=4698
-  _ULTIPARPCS._serialized_start=7812
-  _ULTIPARPCS._serialized_end=8083
-  _ULTIPACONTROLS._serialized_start=8086
-  _ULTIPACONTROLS._serialized_end=9034
+  _ATTRALIAS._serialized_end=961
+  _ATTR._serialized_start=963
+  _ATTR._serialized_end=1027
+  _ATTRLISTDATA._serialized_start=1030
+  _ATTRLISTDATA._serialized_end=1225
+  _ATTRMAPDATA._serialized_start=1227
+  _ATTRMAPDATA._serialized_end=1296
+  _USERSETTINGREQUEST._serialized_start=1299
+  _USERSETTINGREQUEST._serialized_end=1450
+  _USERSETTINGREQUEST_OPTION._serialized_start=1416
+  _USERSETTINGREQUEST_OPTION._serialized_end=1450
+  _USERSETTINGREPLY._serialized_start=1452
+  _USERSETTINGREPLY._serialized_end=1516
+  _DOWNLOADFILEREQUESTV2._serialized_start=1518
+  _DOWNLOADFILEREQUESTV2._serialized_end=1577
+  _DOWNLOADFILEREPLY._serialized_start=1579
+  _DOWNLOADFILEREPLY._serialized_end=1665
+  _EXPORTREQUEST._serialized_start=1667
+  _EXPORTREQUEST._serialized_end=1773
+  _EXPORTREPLY._serialized_start=1775
+  _EXPORTREPLY._serialized_end=1902
+  _GETLEADERREQUEST._serialized_start=1904
+  _GETLEADERREQUEST._serialized_end=1922
+  _GETLEADERREPLY._serialized_start=1924
+  _GETLEADERREPLY._serialized_end=1972
+  _INSERTNODESREQUEST._serialized_start=1975
+  _INSERTNODESREQUEST._serialized_end=2113
+  _INSERTNODESREPLY._serialized_start=2116
+  _INSERTNODESREPLY._serialized_end=2294
+  _INSERTEDGESREQUEST._serialized_start=2297
+  _INSERTEDGESREQUEST._serialized_end=2469
+  _INSERTEDGESREPLY._serialized_start=2472
+  _INSERTEDGESREPLY._serialized_end=2637
+  _INSTALLALGOREQUEST._serialized_start=2639
+  _INSTALLALGOREQUEST._serialized_end=2706
+  _INSTALLALGOREPLY._serialized_start=2708
+  _INSTALLALGOREPLY._serialized_end=2758
+  _UNINSTALLALGOREQUEST._serialized_start=2760
+  _UNINSTALLALGOREQUEST._serialized_end=2801
+  _UNINSTALLALGOREPLY._serialized_start=2803
+  _UNINSTALLALGOREPLY._serialized_end=2855
+  _UPLOADERREQUEST._serialized_start=2858
+  _UPLOADERREQUEST._serialized_end=3008
+  _UPLOADERREPLY._serialized_start=3010
+  _UPLOADERREPLY._serialized_end=3057
+  _CREATEGRAPHBYUPLOADERREQUEST._serialized_start=3059
+  _CREATEGRAPHBYUPLOADERREQUEST._serialized_end=3136
+  _CREATEGRAPHBYUPLOADERREPLY._serialized_start=3138
+  _CREATEGRAPHBYUPLOADERREPLY._serialized_end=3198
+  _INSTALLEXTAREQUEST._serialized_start=3200
+  _INSTALLEXTAREQUEST._serialized_end=3267
+  _INSTALLEXTAREPLY._serialized_start=3269
+  _INSTALLEXTAREPLY._serialized_end=3319
+  _UNINSTALLEXTAREQUEST._serialized_start=3321
+  _UNINSTALLEXTAREQUEST._serialized_end=3362
+  _UNINSTALLEXTAREPLY._serialized_start=3364
+  _UNINSTALLEXTAREPLY._serialized_end=3416
+  _BACKUPREQUEST._serialized_start=3418
+  _BACKUPREQUEST._serialized_end=3454
+  _BACKUPREPLY._serialized_start=3456
+  _BACKUPREPLY._serialized_end=3501
+  _STATUS._serialized_start=3503
+  _STATUS._serialized_end=3606
+  _RAFTFOLLOWER._serialized_start=3608
+  _RAFTFOLLOWER._serialized_end=3691
+  _CLUSTERINFO._serialized_start=3693
+  _CLUSTERINFO._serialized_end=3789
+  _PATH._serialized_start=3791
+  _PATH._serialized_end=3879
+  _TABLE._serialized_start=3881
+  _TABLE._serialized_end=3979
+  _TABLEROW._serialized_start=3981
+  _TABLEROW._serialized_end=4007
+  _ENTITYTABLE._serialized_start=4009
+  _ENTITYTABLE._serialized_end=4095
+  _ENTITYROW._serialized_start=4098
+  _ENTITYROW._serialized_end=4269
+  _SCHEMA._serialized_start=4271
+  _SCHEMA._serialized_end=4338
+  _PROPERTY._serialized_start=4340
+  _PROPERTY._serialized_end=4459
+  _HEADER._serialized_start=4461
+  _HEADER._serialized_end=4537
+  _VALUE._serialized_start=4539
+  _VALUE._serialized_end=4574
+  _LISTDATA._serialized_start=4576
+  _LISTDATA._serialized_end=4619
+  _SETDATA._serialized_start=4621
+  _SETDATA._serialized_end=4663
+  _MAPVALUE._serialized_start=4665
+  _MAPVALUE._serialized_end=4703
+  _MAPDATA._serialized_start=4705
+  _MAPDATA._serialized_end=4765
+  _EXPLAINPLAN._serialized_start=4767
+  _EXPLAINPLAN._serialized_end=4818
+  _PLANNODE._serialized_start=4820
+  _PLANNODE._serialized_end=4895
+  _AUTHENTICATEREQUEST._serialized_start=4897
+  _AUTHENTICATEREQUEST._serialized_end=4971
+  _AUTHENTICATEREPLY._serialized_start=4973
+  _AUTHENTICATEREPLY._serialized_end=5024
+  _ULTIPARPCS._serialized_start=6443
+  _ULTIPARPCS._serialized_end=6714
+  _ULTIPACONTROLS._serialized_start=6717
+  _ULTIPACONTROLS._serialized_end=7721
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ultipa-4.2.4/ultipa/connection/download_extra.py` & `ultipa-4.3.0/ultipa/connection/download_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/searchAB_extra.py` & `ultipa-4.3.0/ultipa/connection/searchAB_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/searchKhop_extra.py` & `ultipa-4.3.0/ultipa/connection/searchKhop_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/task_extra.py` & `ultipa-4.3.0/ultipa/connection/task_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/nodeSpread_extra.py` & `ultipa-4.3.0/ultipa/connection/nodeSpread_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/truncate_extra.py` & `ultipa-4.3.0/ultipa/connection/truncate_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/algo/algos_params.py` & `ultipa-4.3.0/ultipa/connection/algo/algos_params.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/algo/community_extra.py` & `ultipa-4.3.0/ultipa/connection/algo/community_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/algo/algo_params4.py` & `ultipa-4.3.0/ultipa/connection/algo/algo_params4.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/algo/embedding_extra.py` & `ultipa-4.3.0/ultipa/connection/algo/embedding_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/algo/makeAlgoClass.py` & `ultipa-4.3.0/ultipa/connection/algo/makeAlgoClass.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/algo/algo_extra.py` & `ultipa-4.3.0/ultipa/connection/algo/algo_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/algo/degrees_extra.py` & `ultipa-4.3.0/ultipa/connection/algo/degrees_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/autoNet_extra.py` & `ultipa-4.3.0/ultipa/connection/autoNet_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/policy_extra.py` & `ultipa-4.3.0/ultipa/connection/policy_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/edge_extra.py` & `ultipa-4.3.0/ultipa/connection/edge_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/connection.py` & `ultipa-4.3.0/ultipa/connection/connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ultipa.connection.connection_base import ParameterException
 from ultipa.connection.user_extra import UserExtra
 from ultipa.connection.property_extra import PropertyExtra
 from ultipa.connection.node_extra import NodeExtra
 from ultipa.connection.edge_extra import EdgeExtra
 from ultipa.connection.lte_ufe_extra import LteUfeExtra
 from ultipa.connection.index_extra import IndexExtra
 from ultipa.connection.policy_extra import PolicyExtra
@@ -11,30 +12,37 @@
 from ultipa.connection.algo.algo_extra import AlgoExtra
 from ultipa.connection.task_extra import TaskExtra
 from ultipa.connection.export_extra import ExportExtra
 from ultipa.connection.graph_extra import GraphExtra
 from ultipa.connection.download_extra import DownloadExtra
 from ultipa.connection.truncate_extra import TruncateExtra
 from ultipa.connection.schema_extra import SchemaExtra
+from ultipa.connection.backup_data_extra import BackupDataExtra
 from ultipa.types.types import UltipaConfig
 from ultipa.utils.logger import LoggerConfig
 
 
 class Connection(DownloadExtra, UserExtra, PropertyExtra, NodeExtra, EdgeExtra, LteUfeExtra, IndexExtra, PolicyExtra,
-				 TaskExtra, ExportExtra, GraphExtra,AlgoExtra, SchemaExtra, TruncateExtra):
+				 TaskExtra, ExportExtra, GraphExtra,AlgoExtra, SchemaExtra, TruncateExtra,BackupDataExtra):
 
 	def RunHeartBeat(self, time: int):
 		self.keepConnectionAlive(time)
 
 	def StopHeartBeat(self):
 		self.stopConnectionAlive()
 
 	@staticmethod
 	def NewConnection(defaultConfig: UltipaConfig = UltipaConfig()):
 		conn = None
+		if not defaultConfig.hosts:
+			raise ParameterException(err="hosts is a required parameter")
+		if not defaultConfig.username:
+			raise ParameterException(err="username is a required parameter")
+		if not defaultConfig.password:
+			raise ParameterException(err="password is a required parameter")
 		for host in defaultConfig.hosts:
 			conn = Connection(host=host, defaultConfig=defaultConfig, crtFilePath=defaultConfig.crtFilePath)
 			testRes = conn.test()
 			if testRes.status.code == 0:
 				if defaultConfig.heartBeat > 0:
 					conn.RunHeartBeat(defaultConfig.heartBeat)
 				return conn
```

### Comparing `ultipa-4.2.4/ultipa/connection/connectionPoolMaker.py` & `ultipa-4.3.0/ultipa/connection/connectionPoolMaker.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/property_extra.py` & `ultipa-4.3.0/ultipa/connection/property_extra.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from ultipa.connection.connection_base import ConnectionBase
 from ultipa.types import ULTIPA, ULTIPA_REQUEST, ULTIPA_RESPONSE
 from ultipa.utils import UQLMAKER, CommandList
 
 # BOOL_KEYS = ["index","lte"]
 from ultipa.utils.ResposeFormat import ResponseKeyFormat
+from ultipa.utils.propertyUtils import getPropertyTypesDesc
 
 BOOL_KEYS = ["index", "lte"]
 REPLACE_KEYS = {
 	"name": "propertyName",
 	"type": "propertyType",
 }
 
@@ -63,15 +64,16 @@
 					   requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> ULTIPA_RESPONSE.UltipaResponse:
 		'''
 		:EXP: conn.createProperty(ULTIPA_REQUEST.CreatProperty(type=ULTIPA.DBType.DBNODE, name='test_int',property_type=ULTIPA.CreatePropertyType.PROPERTY_INT))
 		:param request: ULTIPA_REQUEST
 		:return:
 		'''
 		command = request.type == ULTIPA.DBType.DBNODE and CommandList.createNodeProperty or CommandList.createEdgeProperty
-		commandP = [request.schemaName.schemaName, request.schemaName.propertyName, request.propertyType]
+		commandP = [request.schemaName.schemaName, request.schemaName.propertyName, getPropertyTypesDesc(request.propertyType,request.subTypes)]
+
 		if request.description:
 			commandP.append(request.description)
 		uqlMaker = UQLMAKER(command=command, commonParams=requestConfig)
 		uqlMaker.setCommandParams(commandP=commandP)
 		# res = self.UqlUpdateSimple(self, uqlMaker=uqlMaker)
 		res = self.uqlSingle(uqlMaker)
 		return res
```

### Comparing `ultipa-4.2.4/ultipa/connection/node_extra.py` & `ultipa-4.3.0/ultipa/connection/node_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/schema_extra.py` & `ultipa-4.3.0/ultipa/connection/schema_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/user_extra.py` & `ultipa-4.3.0/ultipa/connection/user_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/lte_ufe_extra.py` & `ultipa-4.3.0/ultipa/connection/lte_ufe_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/connection_base.py` & `ultipa-4.3.0/ultipa/connection/connection_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 		else:
 			channel = grpc.insecure_channel(self.host, options=(
 				('grpc.max_send_message_length', -1), ('grpc.max_receive_message_length', maxRecvSize),
 				("grpc.keepalive_timeout_ms", 1500)))
 			self.Rpcsclient = ultipa_pb2_grpc.UltipaRpcsStub(channel=channel, )
 			self.Controlsclient = ultipa_pb2_grpc.UltipaControlsStub(channel=channel, )
 
-	def getMetadata(self, graphSetName,timeZone,timeZoneOffset):
+	def getMetadata(self, graphSetName, timeZone, timeZoneOffset):
 		metadata = copy.deepcopy(self._metadata)
 		metadata.append(('graph_name', graphSetName))
 		if timeZone is None and timeZoneOffset is None:
 			timeZone = get_localzone().__dict__.get("_key")
 			tz = pytz.timezone(timeZone)
 			timeZoneOffset = tz.utcoffset(datetime.now()).total_seconds()
 			metadata.append(('tz_offset', str(timeZoneOffset)))
@@ -169,15 +169,15 @@
 		CommandList.createUser,
 		CommandList.alterUser,
 		CommandList.dropUser,
 		CommandList.showIndex,
 		# CommandList.clearTask,
 	]
 
-	def __init__(self,uql:str):
+	def __init__(self, uql: str):
 		self.uql = uql
 		self.parseRet = UQL.parse(uql)
 
 	def uqlIsGlobal(self):
 		# p = UQL.parse_globle(uql)
 		# if p != None:
 		#     for command in p.commands:
@@ -186,15 +186,14 @@
 
 		if self.parseRet != None:
 			c1 = self.parseRet.getFirstCommands()
 			c2 = f"{c1}().{self.parseRet.getSecondCommands()}"
 			return c1 in UQLHelper._globalCommand or c2 in UQLHelper._globalCommand
 		return False
 
-
 	@staticmethod
 	def uqlIsWrite(uql: str):
 		p = UQL.parse(uql)
 		if p != None:
 			for command in p.commands:
 				if list(filter(lambda x: x == command, UQLHelper._write)):
 					return True
@@ -416,15 +415,14 @@
 		#     defaultConfig.password = passwrod2md5(defaultConfig.password) if defaultConfig.password else defaultConfig.password
 		self.host = host
 		self.username = defaultConfig.username
 		self.password = defaultConfig.password
 		self.crtPath = crtFilePath
 		self.defaultConfig = defaultConfig
 		self.crt = None
-
 		if crtFilePath:
 			try:
 				with open(f'{crtFilePath}', 'rb') as f:
 					self.crt = f.read()
 			except Exception as e:
 				raise ParameterException(err=e)
 		self.hostManagerControl = HostManagerControl(self.host, self.username, self.password,
@@ -543,28 +541,29 @@
 						raise errors.ParameterException("UnknownTimeZoneError:" + str(e))
 				timeZoneOffset = requestConfig.timeZoneOffset if requestConfig.timeZoneOffset else self.defaultConfig.timeZoneOffset
 				if timeZoneOffset is not None and type(timeZoneOffset) is not int:
 					raise errors.ParameterException("timeZoneOffset:" + str(timeZoneOffset))
 
 				clientInfo = self.getClientInfo(graphSetName=requestConfig.graphName, uql=uql,
 												useHost=requestConfig.useHost,
-												useMaster=requestConfig.useMaster,timezone=timeZone,timeZoneOffset=timeZoneOffset)
+												useMaster=requestConfig.useMaster, timezone=timeZone,
+												timeZoneOffset=timeZoneOffset)
 				if uqlLoggerConfig:
 					uqlLoggerConfig.getlogger().info(
 						f'Begin UQL: {uql} graphSetName: {clientInfo.graphSetName} Host: {clientInfo.host}')
 				uqlIsExtra = UQLHelper.uqlIsExtra(uql)
 				if uqlIsExtra:
 					res = clientInfo.Controlsclient.UqlEx(request, metadata=clientInfo.metadata)
 				else:
 					res = clientInfo.Rpcsclient.Uql(request, metadata=clientInfo.metadata)
 
 				if not requestConfig.stream:
-					ultipaRes = FormatType.uqlMergeResponse(res)
+					ultipaRes = FormatType.uqlMergeResponse(res, timeZone, timeZoneOffset)
 				else:
-					ultipaRes = FormatType.uqlResponse(_res=res)
+					ultipaRes = FormatType.uqlResponse(res, timeZone, timeZoneOffset)
 
 				if self.defaultConfig.responseWithRequestInfo and not requestConfig.stream:
 					ultipaRes.req = ULTIPA.ReturnReq(clientInfo.graphSetName, uql, clientInfo.host, onRetry,
 													 uqlIsExtra)
 				if not isinstance(ultipaRes, types.GeneratorType) and RetryHelp.checkRes(ultipaRes):
 					onRetry.current += 1
 					continue
@@ -593,21 +592,21 @@
 		res = self.uql(uqlMaker.toString(), uqlMaker.commonParams)
 		return res
 
 	def getGraphSetName(self, currentGraphName: str, uql: str = "", isGlobal: bool = False):
 		if isGlobal:
 			return RAFT_GLOBAL
 		if uql:
-			parse =UQLHelper(uql)
+			parse = UQLHelper(uql)
 			if parse.uqlIsGlobal():
 				return RAFT_GLOBAL
 			# // truncate，mount，unmount，update, 发给当前图集
 			c1 = parse.parseRet.getFirstCommands()
 			c2 = f"{c1}().{parse.parseRet.getSecondCommands()}"
-			if c2 in [CommandList.mount,CommandList.unmount,CommandList.truncate]:
+			if c2 in [CommandList.mount, CommandList.unmount, CommandList.truncate]:
 				graphName = parse.parseRet.getCommandsParam(1)
 				if graphName:
 					return graphName
 		return currentGraphName or self.defaultConfig.defaultGraph
 
 	def getTimeout(self, timeout: int):
 		return timeout or self.defaultConfig.timeoutWithSeconds
@@ -652,68 +651,76 @@
 			return res
 
 	@staticmethod
 	def UqlUpdateSimple(conn: 'ConnectionBase', uqlMaker: UQLMAKER):
 		res = conn.uqlSingle(uqlMaker)
 
 		if res.status.code != ULTIPA.Code.SUCCESS:
-			return ULTIPA_RESPONSE.Response(res.status)
+			return ULTIPA_RESPONSE.Response(res.status, statistics=res.statistics)
 
 		if res.req:
-			ret = ULTIPA_RESPONSE.Response(res.status)
+			ret = ULTIPA_RESPONSE.Response(res.status, statistics=res.statistics)
 			ret.req = res.req
 			return ret
-		return ULTIPA_RESPONSE.Response(res.status)
+		return ULTIPA_RESPONSE.Response(res.status, statistics=res.statistics)
 
 	def getClientInfo(self, clientType: int = ClientType.Default, graphSetName: str = '', uql: str = '',
-					  isGlobal: bool = False, ignoreRaft: bool = False, useHost: str = None, useMaster: bool = False,timezone=None,timeZoneOffset=None):
+					  isGlobal: bool = False, ignoreRaft: bool = False, useHost: str = None, useMaster: bool = False,
+					  timezone=None, timeZoneOffset=None):
 		goGraphName = self.getGraphSetName(currentGraphName=graphSetName, uql=uql, isGlobal=isGlobal)
 		if not ignoreRaft and not self.hostManagerControl.getHostManger(goGraphName).raftReady:
 			refreshRet = self.refreshRaftLeader(self.hostManagerControl.initHost,
 												ULTIPA_REQUEST.RequestConfig(graphName=goGraphName))
 			self.hostManagerControl.getHostManger(goGraphName).raftReady = refreshRet
 
 		clientInfo = self.hostManagerControl.chooseClientInfo(type=clientType, uql=uql, graphSetName=goGraphName,
 															  useHost=useHost, useMaster=useMaster)
-		metadata = clientInfo.getMetadata(goGraphName,timezone,timeZoneOffset)
+		metadata = clientInfo.getMetadata(goGraphName, timezone, timeZoneOffset)
 		return ClientInfo(Rpcsclient=clientInfo.Rpcsclient, Controlsclient=clientInfo.Controlsclient, metadata=metadata,
 						  graphSetName=goGraphName, host=clientInfo.host)
 
 	def test(self,
 			 requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> ULTIPA_RESPONSE.Response:
 		testResponse = ULTIPA_RESPONSE.Response()
+		returnReq = ULTIPA.ReturnReq(requestConfig.graphName, "test", None, None, False)
 		try:
 			clientInfo = self.getClientInfo(useHost=requestConfig.useHost, useMaster=requestConfig.useMaster)
 			name = 'Test'
 			res = clientInfo.Controlsclient.SayHello(ultipa_pb2.HelloUltipaRequest(name=name),
 													 metadata=clientInfo.metadata)
+			returnReq.host = clientInfo.host
 			if (res.message == name + " Welcome To Ultipa!"):
 				if self.defaultConfig.uqlLoggerConfig:
 					self.defaultConfig.uqlLoggerConfig.getlogger().info(res.message)
 
 				testResponse.status = ULTIPA.Status(code=res.status.error_code, message=res.status.msg)
 			else:
 				testResponse.status = ULTIPA.Status(code=res.status.error_code, message=res.status.msg)
 		except Exception as e:
 			# print(e)
 			testResponse = ULTIPA_RESPONSE.Response()
-			testResponse.status = ULTIPA.Status(code=ULTIPA.Code.UNKNOW_ERROR, message=str(e._state.details))
+			try:
+				message = str(e._state.details)
+			except:
+				message = str(e)
+			testResponse.status = ULTIPA.Status(code=ULTIPA.Code.UNKNOW_ERROR, message=message)
 		if self.defaultConfig.responseWithRequestInfo:
-			testResponse.req = ULTIPA.ReturnReq(requestConfig.graphName, "test", clientInfo.host, None, False)
+			testResponse.req = returnReq
 		return testResponse
 
 	def exportData(self, request: ULTIPA_REQUEST.Export,
 				   requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()):
 		try:
 			req = ultipa_pb2.ExportRequest(db_type=request.type, limit=request.limit,
 										   select_properties=request.properties, schema=request.schema)
 
 			clientInfo = self.getClientInfo(graphSetName=requestConfig.graphName, useMaster=requestConfig.useMaster)
 			res = clientInfo.Controlsclient.Export(req, metadata=clientInfo.metadata)
-			res = FormatType.exportResponse(_res=res)
+			res = FormatType.exportResponse(_res=res, timeZone=requestConfig.timeZone,
+											timeZoneOffset=requestConfig.timeZoneOffset)
 			return res
 		except Exception as e:
 			errorRes = ULTIPA_RESPONSE.Response()
 			try:
 				message = str(e._state.code) + ' : ' + str(e._state.details)
 			except:
 				message = 'UNKNOW ERROR'
@@ -827,16 +834,16 @@
 			  requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> ULTIPA_RESPONSE.ResponseStat:
 		uqlMaker = UQLMAKER(command=CommandList.stat, commonParams=requestConfig)
 		ret = ConnectionBase.UqlListSimple(self, uqlMaker=uqlMaker, isSingleOne=True)
 		if ret.status.code == ULTIPA.Code.SUCCESS:
 			ret.data = ret.data[0]
 		return ret
 
-	def insertNodesBulk(self, insertReq: ULTIPA_REQUEST.InsertNodeBulk,
-						requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> ULTIPA_RESPONSE.ResponseBulkInsert:
+	def _insertNodesBulk(self, insertReq: ULTIPA_REQUEST.InsertNodeBulk,
+						 requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> ULTIPA_RESPONSE.ResponseBulkInsert:
 		req = copy.deepcopy(insertReq)
 		try:
 			if requestConfig.graphName == '' and self.defaultConfig.defaultGraph != '':
 				requestConfig.graphName = self.defaultConfig.defaultGraph
 			clientInfo = self.getClientInfo(clientType=ClientType.Update, graphSetName=requestConfig.graphName,
 											useMaster=requestConfig.useMaster)
 			propertyRet = self.uql(GetPropertyBySchema.node,
@@ -850,15 +857,17 @@
 				if not schemaDict:
 					raise ParameterException(err='Please create Node Schema')
 
 			else:
 				raise ParameterException(err=propertyRet.status.message)
 
 			# nodeTable = FormatType.toNodeTable(nodeSchamHeaders, req.rows)
-			nodeTable = FormatType.toNodeTableSingle(schemaDict, req.schema, req.rows,getTimeZoneOffset(requestConfig=insertReq,defaultConfig=self.defaultConfig))
+			nodeTable = FormatType.toNodeTableSingle(schemaDict, req.schema, req.rows,
+													 getTimeZoneOffset(requestConfig=insertReq,
+																	   defaultConfig=self.defaultConfig))
 			_nodeTable = ultipa_pb2.NodeTable(schemas=nodeTable.schemas, node_rows=nodeTable.nodeRows)
 			request = ultipa_pb2.InsertNodesRequest()
 			request.silent = req.silent
 			request.insert_type = req.insertType
 			request.graph_name = requestConfig.graphName
 			request.node_table.MergeFrom(_nodeTable)
 			res = clientInfo.Rpcsclient.InsertNodes(request, metadata=clientInfo.metadata)
@@ -892,28 +901,28 @@
 		uqlres.data = uRes
 		uqlres.total_time = res.time_cost
 		uqlres.engine_time = res.engine_time_cost
 		if self.defaultConfig.responseWithRequestInfo:
 			uqlres.req = ULTIPA.ReturnReq(requestConfig.graphName, "insertNodesBulk", clientInfo.host, reTry, False)
 		return uqlres
 
-	def batchInsertNodesBulk(self, insertReq: ULTIPA_REQUEST.InsertNodeBulk,
-							 requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> List[
+	def _batchInsertNodesBulk(self, insertReq: ULTIPA_REQUEST.InsertNodeBulk,
+							  requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> List[
 		ULTIPA_RESPONSE.ResponseBulkInsert]:
 		batchRetList = []
 		if insertReq.batch:
 			for some in [insertReq.rows[i:i + insertReq.n] for i in range(0, len(insertReq.rows), insertReq.n)]:
 				batchReq = ULTIPA_REQUEST.InsertNodeBulk(insertReq.schema, some, insertReq.insertType,
 														 insertReq.silent)
-				ret = self.insertNodesBulk(batchReq, requestConfig)
+				ret = self._insertNodesBulk(batchReq, requestConfig)
 				batchRetList.append(ret)
 		return batchRetList
 
-	def insertEdgesBulk(self, insertReq: ULTIPA_REQUEST.InsertEdgeBulk,
-						requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> ULTIPA_RESPONSE.ResponseBulkInsert:
+	def _insertEdgesBulk(self, insertReq: ULTIPA_REQUEST.InsertEdgeBulk,
+						 requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> ULTIPA_RESPONSE.ResponseBulkInsert:
 		req = copy.deepcopy(insertReq)
 		try:
 			if requestConfig.graphName == '' and self.defaultConfig.defaultGraph != '':
 				requestConfig.graphName = self.defaultConfig.defaultGraph
 			clientInfo = self.getClientInfo(clientType=ClientType.Update, graphSetName=requestConfig.graphName)
 			propertyRet = self.uql(GetPropertyBySchema.edge,
 								   ULTIPA_REQUEST.RequestConfig(graphName=requestConfig.graphName))
@@ -924,15 +933,17 @@
 						schemaDict = convertTableToDict(propertyRet.alias(aliase.alias).data.rows,
 														propertyRet.alias(aliase.alias).data.headers)
 				if not schemaDict:
 					raise ParameterException(err='Please create Edge Schema')
 			else:
 				raise ParameterException(err=propertyRet.status.message)
 			# _edgeTable = FormatType.toEdgeTable(edgeSchamHeaders, req.rows)
-			_edgeTable = FormatType.toEdgeTableSingle(schemaDict, req.schema, req.rows,getTimeZoneOffset(requestConfig=insertReq,defaultConfig=self.defaultConfig))
+			_edgeTable = FormatType.toEdgeTableSingle(schemaDict, req.schema, req.rows,
+													  getTimeZoneOffset(requestConfig=insertReq,
+																		defaultConfig=self.defaultConfig))
 			edgeTable = ultipa_pb2.EdgeTable(schemas=_edgeTable.schemas, edge_rows=_edgeTable.edgeRows)
 			request = ultipa_pb2.InsertEdgesRequest()
 			request.silent = req.silent
 			request.insert_type = req.insertType
 			request.graph_name = requestConfig.graphName
 			request.create_node_if_not_exist = req.create_node_if_not_exist
 			request.edge_table.MergeFrom(edgeTable)
@@ -967,23 +978,23 @@
 		uqlres.data = uRes
 		uqlres.total_time = res.time_cost
 		uqlres.engine_time = res.engine_time_cost
 		if self.defaultConfig.responseWithRequestInfo:
 			uqlres.req = ULTIPA.ReturnReq(requestConfig.graphName, "insertEdgesBulk", clientInfo.host, reTry, False)
 		return uqlres
 
-	def batchInsertEdgesBulk(self, insertReq: ULTIPA_REQUEST.InsertEdgeBulk,
-							 requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> List[
+	def _batchInsertEdgesBulk(self, insertReq: ULTIPA_REQUEST.InsertEdgeBulk,
+							  requestConfig: ULTIPA_REQUEST.RequestConfig = ULTIPA_REQUEST.RequestConfig()) -> List[
 		ULTIPA_RESPONSE.ResponseBulkInsert]:
 		batchRetList = []
 		if insertReq.batch:
 			for some in [insertReq.rows[i:i + insertReq.n] for i in range(0, len(insertReq.rows), insertReq.n)]:
 				batchReq = ULTIPA_REQUEST.InsertEdgeBulk(insertReq.schema, some, insertReq.insertType,
 														 insertReq.silent)
-				ret = self.insertEdgesBulk(batchReq, requestConfig)
+				ret = self._insertEdgesBulk(batchReq, requestConfig)
 				batchRetList.append(ret)
 		return batchRetList
 
 	# def clearTimeoutHandle(self):
 	#     if self.timeoutHandle:
 	#         clearInterval(this.timeoutHandle)
 	#     self.timeoutHandle = null
@@ -994,15 +1005,15 @@
 	def keepConnectionAlive(self, timeIntervalSeconds: int = None):
 		timeIntervalSeconds = self.defaultConfig.heartBeat if timeIntervalSeconds == None else timeIntervalSeconds
 
 		def test_allconn():
 			goGraphName = self.defaultConfig.defaultGraph
 			for host in self.hostManagerControl.getAllClientInfos(goGraphName):
 				res = host.Controlsclient.SayHello(ultipa_pb2.HelloUltipaRequest(name="test"),
-												   metadata=host.getMetadata(goGraphName,None,None))
+												   metadata=host.getMetadata(goGraphName, None, None))
 				# print(host.host,res.message)
 				if self.defaultConfig.uqlLoggerConfig is None:
 					self.defaultConfig.uqlLoggerConfig = LoggerConfig(name="HeartBeat", fileName=None,
 																	  isWriteToFile=False,
 																	  isStream=True)
 				self.defaultConfig.uqlLoggerConfig.getlogger().info(f"HeartBeat:{host.host}--{res.message}")
 
@@ -1029,15 +1040,15 @@
 
 		status = FormatType.status(res.status)
 		uqlres = ULTIPA_RESPONSE.Response(status=status)
 		# 验证是否要跳转
 		reTry = RetryHelp.check(self, config, uqlres)
 		if reTry.canRetry:
 			config.retry = reTry.nextRetry
-			return self.InsertNodesBatch(nodeTable, config)
+			return self._InsertNodesBatch(nodeTable, config)
 
 		uRes = ULTIPA_RESPONSE.ResponseBulk()
 		uRes.uuids = [i for i in res.uuids]
 		errorDict = {}
 		for i, data in enumerate(res.ignore_error_code):
 			errorDict.update({res.ignore_indexes[i]: data})
 		uRes.errorItem = errorDict
@@ -1067,125 +1078,140 @@
 
 		status = FormatType.status(res.status)
 		uqlres = ULTIPA_RESPONSE.Response(status=status)
 		# 验证是否要跳转
 		reTry = RetryHelp.check(self, config, uqlres)
 		if reTry.canRetry:
 			config.retry = reTry.nextRetry
-			return self.InsertEdgesBatch(edgeTable, config)
+			return self._InsertEdgesBatch(edgeTable, config)
 
 		uRes = ULTIPA_RESPONSE.ResponseBulk()
 		uRes.uuids = [i for i in res.uuids]
 		errorDict = {}
 		for i, data in enumerate(res.ignore_error_code):
 			errorDict.update({res.ignore_indexes[i]: data})
 		uRes.errorItem = errorDict
 		uqlres.data = uRes
 		uqlres.total_time = res.time_cost
 		uqlres.engine_time = res.engine_time_cost
 		if self.defaultConfig.responseWithRequestInfo:
 			uqlres.req = ULTIPA.ReturnReq(config.graphName, "InsertEdgesBatch", clientInfo.host, reTry, False)
 		return uqlres
 
-	def InsertNodesBatchBySchema(self, schema: ULTIPA_REQUEST.Schema, rows: List[ULTIPA.Node],
+	def insertNodesBatchBySchema(self, schema: ULTIPA_REQUEST.Schema, rows: List[ULTIPA.EntityRow],
 								 config: ULTIPA_REQUEST.InsertConfig) -> ULTIPA_RESPONSE.InsertResponse:
 		config.useMaster = True
 		if config.graphName == '' and self.defaultConfig.defaultGraph != '':
 			config.graphName = self.defaultConfig.defaultGraph
 
 		clientInfo = self.getClientInfo(clientType=ClientType.Update, graphSetName=config.graphName,
 										useMaster=config.useMaster)
 
-		nodetable = FormatType.makeNodeTable(schema, rows, getTimeZoneOffset(requestConfig=config,defaultConfig=self.defaultConfig))
+		nodetable = FormatType.makeEntityNodeTable(schema, rows, getTimeZoneOffset(requestConfig=config,
+																				   defaultConfig=self.defaultConfig))
 
-		_nodeTable = ultipa_pb2.NodeTable(schemas=nodetable.schemas, node_rows=nodetable.nodeRows)
+		_nodeTable = ultipa_pb2.EntityTable(schemas=nodetable.schemas, entity_rows=nodetable.nodeRows)
 		request = ultipa_pb2.InsertNodesRequest()
 		request.silent = config.silent
 		request.insert_type = config.insertType
 		request.graph_name = config.graphName
 		request.node_table.MergeFrom(_nodeTable)
 		res = clientInfo.Rpcsclient.InsertNodes(request, metadata=clientInfo.metadata)
 
 		status = FormatType.status(res.status)
 		uqlres = ULTIPA_RESPONSE.Response(status=status)
 		# 验证是否要跳转
 		reTry = RetryHelp.check(self, config, uqlres)
 		if reTry.canRetry:
 			config.retry = reTry.nextRetry
-			return self.InsertNodesBatchBySchema(schema, rows, config)
+			return self.insertNodesBatchBySchema(schema, rows, config)
 
 		uRes = ULTIPA_RESPONSE.ResponseBulk()
 		uRes.uuids = [i for i in res.uuids]
 		errorDict = {}
 		for i, data in enumerate(res.ignore_error_code):
 			try:
 				index = rows[res.ignore_indexes[i]]._getIndex()
 			except Exception as e:
-				index = i
-			if index == None:
-				index = i
+				try:
+					index = res.ignore_indexes[i]
+				except Exception as e:
+					index = i
+			if index is None:
+				try:
+					index = res.ignore_indexes[i]
+				except Exception as e:
+					index = i
 			errorDict.update({index: data})
 		uRes.errorItem = errorDict
 		uqlres.data = uRes
 		uqlres.total_time = res.time_cost
 		uqlres.engine_time = res.engine_time_cost
 		if self.defaultConfig.responseWithRequestInfo:
 			uqlres.req = ULTIPA.ReturnReq(config.graphName, "InsertNodesBatchBySchema", clientInfo.host, reTry,
 										  False)
 		return uqlres
 
-	def InsertEdgesBatchBySchema(self, schema: ULTIPA_REQUEST.Schema, rows: List[ULTIPA.Edge],
+	def insertEdgesBatchBySchema(self, schema: ULTIPA_REQUEST.Schema, rows: List[ULTIPA.EntityRow],
 								 config: ULTIPA_REQUEST.InsertConfig) -> ULTIPA_RESPONSE.InsertResponse:
 		config.useMaster = True
 		if config.graphName == '' and self.defaultConfig.defaultGraph != '':
 			config.graphName = self.defaultConfig.defaultGraph
 
 		clientInfo = self.getClientInfo(clientType=ClientType.Update, graphSetName=config.graphName,
 										useMaster=config.useMaster)
 
-		edgetable = FormatType.makeEdgeTable(schema=schema, rows=rows,timeZoneOffset=getTimeZoneOffset(requestConfig=config,defaultConfig=self.defaultConfig))
+		edgetable = FormatType.makeEntityEdgeTable(schema=schema, rows=rows,
+												   timeZoneOffset=getTimeZoneOffset(requestConfig=config,
+																					defaultConfig=self.defaultConfig))
 
-		_edgeTable = ultipa_pb2.EdgeTable(schemas=edgetable.schemas, edge_rows=edgetable.edgeRows)
+		_edgeTable = ultipa_pb2.EntityTable(schemas=edgetable.schemas, entity_rows=edgetable.edgeRows)
 		request = ultipa_pb2.InsertEdgesRequest()
 		request.silent = config.silent
 		request.insert_type = config.insertType
 		request.graph_name = config.graphName
 		request.create_node_if_not_exist = config.createNodeIfNotExist
 		request.edge_table.MergeFrom(_edgeTable)
 		res = clientInfo.Rpcsclient.InsertEdges(request, metadata=clientInfo.metadata)
 
 		status = FormatType.status(res.status)
 		uqlres = ULTIPA_RESPONSE.Response(status=status)
 		# 验证是否要跳转
 		reTry = RetryHelp.check(self, config, uqlres)
 		if reTry.canRetry:
 			config.retry = reTry.nextRetry
-			return self.InsertEdgesBatchBySchema(schema, rows, config)
+			return self.insertEdgesBatchBySchema(schema, rows, config)
 
 		uRes = ULTIPA_RESPONSE.ResponseBulk()
 		uRes.uuids = [i for i in res.uuids]
 		errorDict = {}
 		for i, data in enumerate(res.ignore_error_code):
 			try:
 				index = rows[res.ignore_indexes[i]]._getIndex()
 			except Exception as e:
-				index = i
-			if index == None:
-				index = i
+				try:
+					index = res.ignore_indexes[i]
+				except Exception as e:
+					index = i
+			if index is None:
+				try:
+					index = res.ignore_indexes[i]
+				except Exception as e:
+					index = i
 			errorDict.update({index: data})
 		uRes.errorItem = errorDict
 		uqlres.data = uRes
 		uqlres.total_time = res.time_cost
 		uqlres.engine_time = res.engine_time_cost
 		if self.defaultConfig.responseWithRequestInfo:
 			uqlres.req = ULTIPA.ReturnReq(config.graphName, "InsertEdgesBatchBySchema", clientInfo.host, reTry,
 										  False)
 		return uqlres
 
-	def InsertNodesBatchAuto(self, nodes: List[ULTIPA.Node],
+	def insertNodesBatchAuto(self, nodes: List[ULTIPA.EntityRow],
 							 config: ULTIPA_REQUEST.InsertConfig) -> ULTIPA_RESPONSE.ResponseBatchAutoInsert:
 		Result = {}
 		schemaDict = {}
 		batches = {}
 		schemaRet = self.uql(GetPropertyBySchema.node, config)
 		if schemaRet.status.code == ULTIPA.Code.SUCCESS:
 			for aliase in schemaRet.aliases:
@@ -1199,32 +1225,27 @@
 		for index, node in enumerate(nodes):
 			node._index = index
 			if batches.get(node.schema) is None:
 				batches[node.schema] = ULTIPA_REQUEST.Batch()
 				find = list(filter(lambda x: x.get('name') == node.schema, schemaDict))
 				if find:
 					findSchema = find[0]
-					propertyList = []
-					for property in json.loads(findSchema.get("properties")):
-						reqProperty = ULTIPA_REQUEST.Property(property.get("name"))
-						reqProperty.setTypeInt(property.get("type"))
-						propertyList.append(reqProperty)
+					propertyList = FormatType.checkProperty(node, json.loads(findSchema.get("properties")))
 					reqSchema = ULTIPA_REQUEST.Schema(node.schema, propertyList)
 					batches[node.schema].Schema = reqSchema
-					FormatType.checkNodeRow(index, reqSchema, node)
 				else:
 					if node.schema is None:
 						raise ParameterException(err=f"Row [{index}]:Please set schema name for node.")
 					else:
 						raise ParameterException(err=f"Row [{index}]:Node Schema not found {node.schema}.")
 
 			batches.get(node.schema).Nodes.append(node)
 		for key in batches:
 			batch = batches.get(key)
-			Result.update({key: self.InsertNodesBatchBySchema(schema=batch.Schema, rows=batch.Nodes, config=config)})
+			Result.update({key: self.insertNodesBatchBySchema(schema=batch.Schema, rows=batch.Nodes, config=config)})
 
 		newStatusMsg = ""
 		newCode = None
 		for i, key in enumerate(Result):
 			ret = Result.get(key)
 			newStatusMsg += f"{key}:{ret.status.message} "
 			if ret.status.code != ULTIPA.Code.SUCCESS and not newCode:
@@ -1232,15 +1253,15 @@
 		if newCode is None:
 			newCode = ULTIPA.Code.SUCCESS
 		status = ULTIPA_RESPONSE.Status(newCode, newStatusMsg)
 		newResponse = ULTIPA_RESPONSE.ResponseBatchAutoInsert(status=status)
 		newResponse.data = Result
 		return newResponse
 
-	def InsertEdgesBatchAuto(self, edges: List[ULTIPA.Edge],
+	def insertEdgesBatchAuto(self, edges: List[ULTIPA.EntityRow],
 							 config: ULTIPA_REQUEST.InsertConfig) -> ULTIPA_RESPONSE.ResponseBatchAutoInsert:
 		Result = {}
 		schemaDict = []
 		batches = {}
 		schemaRet = self.uql(GetPropertyBySchema.edge, config)
 		if schemaRet.status.code == ULTIPA.Code.SUCCESS:
 			for aliase in schemaRet.aliases:
@@ -1254,31 +1275,26 @@
 		for index, edge in enumerate(edges):
 			edge._index = index
 			if batches.get(edge.schema) == None:
 				batches[edge.schema] = ULTIPA_REQUEST.Batch()
 				find = list(filter(lambda x: x.get('name') == edge.schema, schemaDict))
 				if find:
 					findSchema = find[0]
-					propertyList = []
-					for property in json.loads(findSchema.get("properties")):
-						reqProperty = ULTIPA_REQUEST.Property(property.get("name"))
-						reqProperty.setTypeInt(property.get("type"))
-						propertyList.append(reqProperty)
+					propertyList = FormatType.checkProperty(edge, json.loads(findSchema.get("properties")))
 					reqSchema = ULTIPA_REQUEST.Schema(edge.schema, propertyList)
 					batches[edge.schema].Schema = reqSchema
-					FormatType.checkEdgeRow(index, reqSchema, edge)
 				else:
 					if edge.schema is None:
 						raise ParameterException(err=f"Row [{index}]:Please set schema name for edge.")
 					else:
 						raise ParameterException(err=f"Row [{index}]:Edge Schema not found {edge.schema}.")
 			batches.get(edge.schema).Edges.append(edge)
 		for key in batches:
 			batch = batches.get(key)
-			Result.update({key: self.InsertEdgesBatchBySchema(schema=batch.Schema, rows=batch.Edges, config=config)})
+			Result.update({key: self.insertEdgesBatchBySchema(schema=batch.Schema, rows=batch.Edges, config=config)})
 
 		newStatusMsg = ""
 		newCode = None
 		for i, key in enumerate(Result):
 			ret = Result.get(key)
 			newStatusMsg += f"{key}:{ret.status.message} "
 			if ret.status.code != ULTIPA.Code.SUCCESS and not newCode:
@@ -1287,22 +1303,22 @@
 			newCode = ULTIPA.Code.SUCCESS
 		status = ULTIPA_RESPONSE.Status(newCode, newStatusMsg)
 		newResponse = ULTIPA_RESPONSE.ResponseBatchAutoInsert(status=status)
 		newResponse.data = Result
 		return newResponse
 
 	def _InsertByCSV(self, csvPath: str, type: ULTIPA.DBType, config: ULTIPA_REQUEST.InsertConfig,
-					schemaName: str = None) -> ULTIPA_RESPONSE.ResponseBatchAutoInsert:
+					 schemaName: str = None) -> ULTIPA_RESPONSE.ResponseBatchAutoInsert:
 		rows = []
 		propertyType = []
 		properties = []
 		types = []
 		with open(csvPath, "r", encoding="utf-8-sig") as csvfile:
 			reader = csv.reader(csvfile)
-			for i,line in enumerate(reader):
+			for i, line in enumerate(reader):
 				if i == 0:
 					for i, property in enumerate(line):
 						k1, k2 = property.split(":")
 						propertyType.append({k1: k2})
 						types.append({"index": i, "type": k2})
 						properties.append(k1)
 					continue
@@ -1314,15 +1330,15 @@
 						line[i.get("index")] = int(line[i.get("index")])
 					if i.get("type") in ["float", "double"]:
 						if line[i.get("index")] == "":
 							line[i.get("index")] = 0.0
 							continue
 						line[i.get("index")] = float(line[i.get("index")])
 				line = dict(zip(properties, line))
-				if i ==0:
+				if i == 0:
 					print(line.keys())
 				if type == ULTIPA.DBType.DBNODE:
 					if line.get("_uuid"):
 						uuid = line.get("_uuid")
 						line.__delitem__("_uuid")
 						rows.append(ULTIPA.Node(line, schema_name=schemaName, uuid=int(uuid)))
 					elif line.get("_id"):
@@ -1335,21 +1351,22 @@
 				elif type == ULTIPA.DBType.DBEDGE:
 					if line.get("_from_uuid") and line.get("_to_uuid"):
 						from_uuid = line.get("_from_uuid")
 						line.__delitem__("_from_uuid")
 						to_uuid = line.get("_to_uuid")
 						line.__delitem__("_to_uuid")
 						line.__delitem__("_id")
-						rows.append(ULTIPA.Edge(line, schema_name=schemaName, from_uuid=int(from_uuid), to_uuid=int(to_uuid)))
+						rows.append(
+							ULTIPA.Edge(line, schema_name=schemaName, from_uuid=int(from_uuid), to_uuid=int(to_uuid)))
 					elif line.get("_from_id") and line.get("_to_id"):
 						from_id = line.get("_from_id")
 						line.__delitem__("_from_id")
 						to_id = line.get("_to_id")
 						line.__delitem__("_to_id")
 						if line.get("_id"):
 							line.__delitem__("_id")
-						rows.append(ULTIPA.Edge(line, schema_name=schemaName, from_id=from_id,to_id=to_id))
+						rows.append(ULTIPA.Edge(line, schema_name=schemaName, from_id=from_id, to_id=to_id))
 
 		if type == ULTIPA.DBType.DBNODE:
-			return self.InsertNodesBatchAuto(rows, config)
+			return self.insertNodesBatchAuto(rows, config)
 		else:
-			return self.InsertEdgesBatchAuto(rows, config)
+			return self.insertEdgesBatchAuto(rows, config)
```

### Comparing `ultipa-4.2.4/ultipa/connection/index_extra.py` & `ultipa-4.3.0/ultipa/connection/index_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/graph_extra.py` & `ultipa-4.3.0/ultipa/connection/graph_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/template_extra.py` & `ultipa-4.3.0/ultipa/connection/template_extra.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/connection/connectionPool.py` & `ultipa-4.3.0/ultipa/connection/connectionPool.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/printer/prettyPrint.py` & `ultipa-4.3.0/ultipa/printer/prettyPrint.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,25 +4,46 @@
 # @Email   : support@ultipa.com
 # @File    : prettyPrint.py
 import json
 from typing import List
 from treelib import Tree
 from prettytable import PrettyTable
 
-from ultipa.types.types import DataItem, ExplainPlan
+from ultipa.types.types import DataItem, ExplainPlan, AttrAlias, PaserAttrListData, ResultType, EntityRow, PropertyType, \
+	Path, Node, Edge
 from ultipa.utils.convert import convertTableToDict
 
 
+class PrintAttrData:
+	ret = []
+
+	# def __init__(self,data:[AttrAlias]):
+	# 	self.data = data
+	def _formatAttr(self, data: AttrAlias):
+		if data.type == "list":
+			self._formatAttrList(data.rows)
+		else:
+			return data.rows
+
+	def _formatAttrList(self, rows: [AttrAlias]):
+		ret = []
+		for attr in rows:
+			ret.append(self._formatAttr(attr))
+		return ret
+
+
 class TreeNode:
 	# explain:ExplainPlan
 	# childNodes:List = []
 
 	def __init__(self, explain: ExplainPlan = None):
 		self.explain = explain
 		self.childNodes = []
+
+
 # def setExplan(self,plan):
 # 	self.explain=plan
 #
 # def childNodesAdd(self,node):
 # 	self.childNodes.append(node)
 
 
@@ -72,47 +93,110 @@
 		print(y)
 
 	def prettyNode(self, data: DataItem):
 		schemaDict = {}
 		for node in data.asNodes():
 			propertList = ["id", "uuid", "schema"]
 			if not schemaDict.get(node.getSchema()):
-				newPropertList = propertList+list(node.values.keys())
-				schemaDict.update({node.getSchema(): newPropertList})
+				if node.values:
+					newPropertList = propertList + list(node.values.keys())
+					schemaDict.update({node.getSchema(): newPropertList})
+				else:
+					schemaDict.update({node.getSchema(): propertList})
 
 		for key in schemaDict:
-			y = PrettyTable(schemaDict.get(key), title=f"Alias: {data.alias} AliasType: {data.type} Schema: {key}", align="l")
+			y = PrettyTable(schemaDict.get(key), title=f"Alias: {data.alias} AliasType: {data.type} Schema: {key}",
+							align="l")
 			for newNode in data.asNodes():
 				if newNode.getSchema() == key:
 					li = [newNode.getID(), newNode.getUUID(), newNode.getSchema()]
-					li.extend(list(newNode.values.values()))
+					if newNode.values:
+						li.extend(list(newNode.values.values()))
 					y.add_row(li)
 				else:
 					continue
 			print(y)
 
+	def prettyAttrNode(self, alias, nodes: List[Node]):
+		ret = []
+		schemaDict = {}
+		for node in nodes:
+			propertList = ["id", "uuid", "schema"]
+			if not schemaDict.get(node.getSchema()):
+				if node.values:
+					newPropertList = propertList + list(node.values.keys())
+					schemaDict.update({node.getSchema(): newPropertList})
+				else:
+					schemaDict.update({node.getSchema(): propertList})
+
+		for key in schemaDict:
+			y = PrettyTable(schemaDict.get(key), title=f"Alias: {alias} AliasType: NODE Schema: {key}",
+							align="l")
+			for newNode in nodes:
+				if newNode.getSchema() == key:
+					li = [newNode.getID(), newNode.getUUID(), newNode.getSchema()]
+					if newNode.values:
+						li.extend(list(newNode.values.values()))
+					y.add_row(li)
+				else:
+					continue
+			ret.append(y)
+		return ret
+
 	def prettyEdge(self, data: DataItem):
 		schemaDict = {}
 		for edge in data.asEdges():
 			propertList = ["uuid", "from_uuid", "to_uuid", "from_id", "to_id", "schema"]
 			if not schemaDict.get(edge.getSchema()):
-				newPropertList = propertList+list(edge.values.keys())
-				schemaDict.update({edge.getSchema(): newPropertList})
+				if edge.values:
+					newPropertList = propertList + list(edge.values.keys())
+					schemaDict.update({edge.getSchema(): newPropertList})
+				else:
+					schemaDict.update({edge.getSchema(): propertList})
 
 		for key in schemaDict:
-			y = PrettyTable(schemaDict.get(key), title=f"Alias: {data.alias} AliasType: {data.type} Schema: {key}", align="l")
+			y = PrettyTable(schemaDict.get(key), title=f"Alias: {data.alias} AliasType: {data.type} Schema: {key}",
+							align="l")
 			for newEdge in data.asEdges():
 				if newEdge.getSchema() == key:
-					li = [newEdge.getUUID(), newEdge.getFromUUID(), newEdge.getToUUID(), newEdge.getFrom(), newEdge.getTo(), newEdge.getSchema()]
-					li.extend(list(newEdge.values.values()))
+					li = [newEdge.getUUID(), newEdge.getFromUUID(), newEdge.getToUUID(), newEdge.getFrom(),
+						  newEdge.getTo(), newEdge.getSchema()]
+					if newEdge.values:
+						li.extend(list(newEdge.values.values()))
 					y.add_row(li)
 				else:
 					continue
 			print(y)
 
+	def prettyAttrEdge(self, alias, edges: List[Edge]):
+		ret = []
+		schemaDict = {}
+		for edge in edges:
+			propertList = ["uuid", "from_uuid", "to_uuid", "from_id", "to_id", "schema"]
+			if not schemaDict.get(edge.getSchema()):
+				if edge.values:
+					newPropertList = propertList + list(edge.values.keys())
+					schemaDict.update({edge.getSchema(): newPropertList})
+				else:
+					schemaDict.update({edge.getSchema(): propertList})
+
+		for key in schemaDict:
+			y = PrettyTable(schemaDict.get(key), title=f"Alias: {alias} AliasType: EDGE Schema: {key}", align="l")
+			for newEdge in edges:
+				if newEdge.getSchema() == key:
+					li = [newEdge.getUUID(), newEdge.getFromUUID(), newEdge.getToUUID(), newEdge.getFrom(),
+						  newEdge.getTo(), newEdge.getSchema()]
+					if newEdge.values:
+						li.extend(list(newEdge.values.values()))
+					y.add_row(li)
+				else:
+					continue
+			ret.append(y)
+		return ret
+
 	def prettyTable(self, data: DataItem):
 
 		if data.alias == "_algoList":
 			headers = data.asTable().getHeaders()
 			rows = data.asTable().getRows()
 			table_rows_dict = convertTableToDict(rows, headers)
 			algo_list = []
@@ -154,58 +238,87 @@
 				# 			y1.add_row(proper.values())
 				# 		li.append(y1)
 				# 	else:
 				# 		li.append(None)
 				y.add_row(row)
 		print(y)
 
+	def _PrintPath(self, path: Path):
+		pathStr = ""
+		end = ""
+		for index, edge in enumerate(path.edges):
+			d1 = "-"
+			d2 = "-"
+			node = path.getNodes()[index]
+			if edge.getFrom() == node.getID():
+				d2 = "->"
+				if index == len(path.edges) - 1:
+					end = f" ({str(edge.getTo())})"
+			else:
+				d1 = "<-"
+				if index == len(path.edges) - 1:
+					end = f" ({str(edge.getFrom())})"
+
+			pathStr += f"({node.getID()}) {d1} [{edge.getUUID()}] {d2}"
+			if end:
+				pathStr += end
+		return pathStr
+
 	def prettyPath(self, data: DataItem):
-		propertList = ["#","Path"]
+		propertList = ["#", "Path"]
 		y = PrettyTable(propertList, title=f"Alias: {data.alias} AliasType: {data.type}", align="l")
-		for i,path in enumerate(data.asPaths()):
+		for i, path in enumerate(data.asPaths()):
 			li = [i]
-			pathStr = ""
-			end = ""
-			for index, edge in enumerate(path.edges):
-				d1 = "-"
-				d2 = "-"
-				node = path.getNodes()[index]
-				if edge.getFrom() == node.getID():
-					d2 = "->"
-					if index == len(path.edges) - 1:
-						end = f" ({str(edge.getTo())})"
-				else:
-					d1 = "<-"
-					if index == len(path.edges) - 1:
-						end = f" ({str(edge.getFrom())})"
-
-				pathStr += f"({node.getID()}) {d1} [{edge.getUUID()}] {d2}"
-				if end:
-					pathStr += end
+			pathStr = self._PrintPath(path)
 			li.append(pathStr)
 			y.add_row(li)
 		print(y)
 
+	def _formatAttrListData(self, data: list, alias: str):
+		if isinstance(data,list) and len(data) > 0:
+			if isinstance(data[0], Path):
+				li = []
+				for i in data:
+					li.append(self._PrintPath(i))
+				return str(li)
+			elif isinstance(data[0], Node):
+				return self.prettyAttrNode(alias, data)
+
+			elif isinstance(data[0], Edge):
+				return self.prettyAttrEdge(alias, data)
+			else:
+				return str(data)
+		else:
+			return str(data)
+
 	def prettyAttr(self, data: DataItem):
-		propertList = [data.alias]
-		y = PrettyTable(propertList, title=f"Alias: {data.alias} AliasType: {data.type}", align="l")
-		if isinstance(data.asAttr(), list):
-			ret = [str(data.asAttr())]
-			y.add_row(ret)
+		if data.asAttr().type in [ResultType.RESULT_TYPE_PATH, ResultType.RESULT_TYPE_EDGE,
+								  ResultType.RESULT_TYPE_NODE]:
+			propertList = ["#", data.alias]
+			y = PrettyTable(propertList, title=f"Alias: {data.alias} AliasType: {data.type}", align="l")
+			for i, adata in enumerate(data.asAttr().values):
+				ret = self._formatAttrListData(adata, data.alias)
+				y.add_row([i + 1, ret])
 			print(y)
 		else:
-			for i in data.asAttr().rows:
-				y.add_row([str(i)])
+			propertList = ["#", data.alias]
+			y = PrettyTable(propertList, title=f"Alias: {data.alias} AliasType: {data.type}", align="l")
+			if len(data.asAttr().values) > 0:
+				for i, adata in enumerate(data.asAttr().values):
+					ret = self._formatAttrListData(adata, data.alias)
+					y.add_row([i + 1, ret])
+			else:
+				y.add_row([1, str(data.asAttr().values)])
 			print(y)
 
 	def prettyArray(self, data: DataItem):
 		propertList = [data.alias]
 		y = PrettyTable(propertList, title=f"Alias: {data.alias} AliasType: {data.type}", align="l")
 		for array in data.asArray().elements:
-			y.add_row([json.dumps(array,ensure_ascii=False)])
+			y.add_row([json.dumps(array, ensure_ascii=False)])
 		print(y)
 
 	def prettyTree(self, plans: List[ExplainPlan]):
 		def buildTree(plans: List[ExplainPlan]):
 			if plans == None or len(plans) == 0:
 				return TreeNode()
 			tree = TreeNode(plans[0])
```

### Comparing `ultipa-4.2.4/ultipa/utils/raftRetry.py` & `ultipa-4.3.0/ultipa/utils/raftRetry.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/typeCheck.py` & `ultipa-4.3.0/ultipa/utils/typeCheck.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/convert.py` & `ultipa-4.3.0/ultipa/utils/convert.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/fileSize.py` & `ultipa-4.3.0/ultipa/utils/fileSize.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/format.py` & `ultipa-4.3.0/ultipa/utils/format.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import json
 from typing import List
 
+from ultipa.proto.ultipa_pb2 import AttrListData
 from ultipa.types.types import ResultType
 from ultipa.utils import errors
 from ultipa.types import ULTIPA, ULTIPA_RESPONSE, ULTIPA_REQUEST
 from ultipa.utils.errors import ParameterException
 from ultipa.utils.serialize import _Serialize
 
 #
@@ -22,61 +23,41 @@
 #                     continue
 #                 if params.__dict__[k]:
 #                     uqlMaker.addParam(k, params.__dict__[k])
 #         return uqlMaker
 from ultipa.utils.typeCheck import TypeCheck
 
 
-class FormatResponse:
+class HasDataMap:
+	has_ultipa_data: bool
+	has_attr_data: bool
+	only_attr_list: bool
+
+	def __init__(self, has_ultipa_data, has_attr_data, only_attr_list):
+		self.has_ultipa_data = has_ultipa_data
+		self.has_attr_data = has_attr_data
+		self.only_attr_list = only_attr_list
 
-	# @staticmethod
-	# def uqlReplyData(uqlResponse: ULTIPA_RESPONSE.Response, index: int) -> ULTIPA_RESPONSE.Response:
-	#     if (uqlResponse.data and len(uqlResponse.data) > index):
-	#         uqlResponse.data = uqlResponse.data[index]
-	#         return uqlResponse
-	#     return uqlResponse
 
-	# @staticmethod
-	# def tableToArray(table: ULTIPA.Table):
-	#     res = []
-	#     if table:
-	#         try:
-	#             for row in table.table_rows:
-	#                 item = {}
-	#                 for index in range(len(row)):
-	#                     v = row[index]
-	#                     item[table.headers[index]] = v
-	#                 res.append(item)
-	#             # tret = ULTIPA.Tables(table_name=table.table_name,table_rows=res)
-	#             # tres.append(tret)
-	#         except Exception as e:
-	#             print(e)
-	#     return res
+class FormatResponse:
 
 	@staticmethod
 	def resTableToArray(table: ULTIPA.Table):
 		# SchemaNameList = ['_nodeSchema', '_edgeSchema']
 		tres = []
 		headers = []
 		if table:
 			try:
-				for header in table.headers:
+				for index, header in enumerate(table.headers):
+					if not header.property_name:
+						if header.property_type == ULTIPA.PropertyType.PROPERTY_NULL:
+							header.property_name = f"null({index})"
 					headers.append({"property_name": header.property_name,
 									"property_type": ULTIPA_REQUEST.Property._getStringByPropertyType(
 										header.property_type)})
-
-				# for row in table.rows:
-				#     item = {}
-				#     for index in range(len(row)):
-				#         v = row[index]
-				#         if table.name in SchemaNameList and table.headers[index].property_name == 'properties':
-				#             item[table.headers[index].property_name] = json.loads(v)
-				#         else:
-				#             item[table.headers[index].property_name] = v
-				#     res.append(item)
 				tret = ULTIPA.Table(table_name=table.name, headers=headers, table_rows=table.rows)
 				tres.append(tret)
 			except Exception as e:
 				raise errors.ParameterException(e)
 		return tret
 
 	@staticmethod
@@ -249,26 +230,25 @@
 
 			if bykey == 'values':
 				if isinstance(arr1, list) and isinstance(arr2, list):
 					newArry = arr2
 					newData = arr1
 					arrtlist = []
 					for new in newData:
-						arrtlist.append(new.name)
+						arrtlist.append(new.alias)
 
 					for arr in newArry:
-						if arr.name not in arrtlist:
+						if arr.alias not in arrtlist:
 							newData.append(arr)
-
 					for arr in newArry:
 						if not newData:
 							newData.append(arr)
 						for new in newData:
-							if arr.name in arrtlist and arr.name == new.name:
-								new.rows += arr.rows
+							if arr.alias in arrtlist and arr.alias == new.alias:
+								new.values += arr.values
 					return newData
 
 			if bykey == 'arrays':
 				if isinstance(arr1, list) and isinstance(arr2, list):
 					newArry = arr2
 					newData = arr1
 					arrtlist = []
@@ -293,15 +273,31 @@
 		elif isinstance(arr1, dict) and isinstance(arr2, dict):
 			return arr1.update(arr2)
 
 
 class FormatType:
 
 	@staticmethod
-	def checkNodeRow(i: int, schema: ULTIPA_REQUEST.Schema, row: ULTIPA.Node):
+	def checkProperty(row, schemaProperties):
+		propertyList = []
+		rowPropertyList = row.values.keys()
+		for property in rowPropertyList:
+			findSchema = list(filter(lambda x: x.get('name') == property, schemaProperties))
+			if findSchema:
+				schemaProperty = findSchema[0]
+				reqProperty = ULTIPA_REQUEST.Property(schemaProperty.get("name"))
+				reqProperty.setTypeInt(schemaProperty.get("type"))
+				propertyList.append(reqProperty)
+			else:
+				raise ParameterException(
+					err=f"row [{row._getIndex()}] error: schema[{row.schema}] doesn't contain property [{property}].")
+		return propertyList
+
+	@staticmethod
+	def checkNodeRow(i: int, schema: ULTIPA_REQUEST.Schema, row: ULTIPA.EntityRow):
 		if row._index != None:
 			i = row._index
 
 		if row is None:
 			raise ParameterException(err=f"The row [{i}] data is null")
 
 		if row.values is None:
@@ -320,15 +316,85 @@
 			if proper.isIdType() or proper.isIgnore():
 				continue
 			if proper.name not in row.values:
 				raise ParameterException(
 					err=f"node row [{i}] error: values doesn't contain property [{proper.name}].")
 
 	@staticmethod
-	def checkEdgeRow(i: int, schema: ULTIPA_REQUEST.Schema, row: ULTIPA.Edge):
+	def checkEdgeRow(i: int, schema: ULTIPA_REQUEST.Schema, row: ULTIPA.EntityRow):
+		if row._index != None:
+			i = row._index
+
+		if row is None:
+			raise ParameterException(err=f"The row [{i}] data is null")
+		if row.values is None:
+			raise ParameterException(err=f"edge row [{i}] error: values are empty but properties size > 0.")
+		if not schema.properties and row.values:
+			raise ParameterException(err=f"edge row [{i}] error: properties are empty but values size > 0.")
+
+		if len(row.values.keys()) > len(schema.properties):
+			raise ParameterException(err=f"edge row [{i}] error: values size larger than properties size.")
+
+		if len(row.values.keys()) < len(schema.properties):
+			raise ParameterException(err=f"edge row [{i}] error: values size smaller than properties size.")
+
+		if ((row.from_id is None or row.from_id == "") and (row.to_id is None or row.to_id == "")) \
+				and (row.from_uuid is None and row.to_uuid is None):
+			raise ParameterException(err=f"row [{i}] error: _from/_from_uuid and _to/_to_uuid are null.")
+
+		if (row.from_id != None and row.from_id != "") and (row.to_id is None or row.to_id == ""):
+			raise ParameterException(err=f"row [{i}] error: _from has value [{row.from_id}] but _to got null.")
+
+		if (row.from_id is None or row.from_id == "") and (row.to_id != None and row.to_id != ""):
+			raise ParameterException(err=f"row [{i}] error: _to has value [{row.to_id}] but _from got null.")
+
+		if row.from_uuid is None and row.to_uuid != None:
+			raise ParameterException(
+				err=f"row [{i}] error: _to_uuid has value [{row.to_uuid}] but _from_uuid got null.")
+
+		if row.from_uuid != None and row.to_uuid is None:
+			raise ParameterException(
+				err=f"row [{i}] error: _from_uuid has value [{row.from_uuid}] but _to_uuid got null.")
+
+		for proper in schema.properties:
+			if proper.isIdType() or proper.isIgnore():
+				continue
+			if proper.name not in row.values:
+				raise ParameterException(
+					err=f"edge row [{i}] error: values doesn't contain property [{proper.name}].")
+
+	@staticmethod
+	def checkEntityNodeRow(i: int, schema: ULTIPA_REQUEST.Schema, row: ULTIPA.EntityRow):
+		if row._index != None:
+			i = row._index
+
+		if row is None:
+			raise ParameterException(err=f"The row [{i}] data is null")
+
+		if row.values is None:
+			raise ParameterException(err=f"node row [{i}] error: values are empty but  properties size > 0.")
+
+		if not schema.properties and row.values:
+			raise ParameterException(err=f"node row [{i}] error: properties are empty but values size > 0.")
+
+		if len(row.values.keys()) > len(schema.properties):
+			raise ParameterException(err=f"node row [{i}] error: values size larger than properties size.")
+
+		if len(row.values.keys()) < len(schema.properties):
+			raise ParameterException(err=f"node row [{i}] error: values size smaller than properties size.")
+
+		for proper in schema.properties:
+			if proper.isIdType() or proper.isIgnore():
+				continue
+			if proper.name not in row.values:
+				raise ParameterException(
+					err=f"node row [{i}] error: values doesn't contain property [{proper.name}].")
+
+	@staticmethod
+	def checkEntityEdgeRow(i: int, schema: ULTIPA_REQUEST.Schema, row: ULTIPA.EntityRow):
 		if row._index != None:
 			i = row._index
 
 		if row is None:
 			raise ParameterException(err=f"The row [{i}] data is null")
 		if row.values is None:
 			raise ParameterException(err=f"edge row [{i}] error: values are empty but properties size > 0.")
@@ -400,127 +466,161 @@
 		statusData = ULTIPA.Status(code=data.get("code"), message=data.get("message"))
 		clusterInfo = ULTIPA.ClusterInfo(redirect=data.get("redirectHost"), raftPeers=data.get("followersPeerInfos"),
 										 leader=data.get("leaderInfos"))
 		statusData.clusterInfo = clusterInfo
 		return statusData
 
 	@staticmethod
-	def table(_table) -> ULTIPA.Table:
+	def table(_table, timeZone, timeZoneOffset) -> ULTIPA.Table:
 		table_name = _table.table_name
 		headers = []
 		for h in _table.headers:
 			headers.append(h)
 		values = []
 		for index, row in enumerate(_table.table_rows):
 			_vs = []
 			for index2, _v in enumerate(row.values):
 				if len(headers) > 0:
 					property_type = headers[index2].property_type
 				else:
 					property_type = ULTIPA.PropertyType.PROPERTY_STRING
-				_seria = _Serialize(type=property_type, value=_v)
+				# header type is NULL
+				# if property_type == ULTIPA.PropertyType.PROPERTY_NULL:
+				# 	_vs.append(None)
+				# 	continue
+				_seria = _Serialize(type=property_type, value=_v, timeZone=timeZone, timeZoneOffset=timeZoneOffset)
 				unret = _seria.unserialize()
 				_vs.append(unret)
 			values.append(_vs)
 		tableData = ULTIPA.Table(table_name=table_name, headers=headers, table_rows=values)
 		return tableData
 
 	@staticmethod
-	def tables(_tables) -> List[ULTIPA.Table]:
+	def tables(_tables, timeZone, timeZoneOffset) -> List[ULTIPA.Table]:
 		tablesData = []
 		if _tables:
 			for table in _tables:
-				tableData = FormatType.table(table)
+				tableData = FormatType.table(table, timeZone, timeZoneOffset)
 				# for ta in tables:
 				tret = FormatResponse.resTableToArray(table=tableData)
 				# tablesData += tret
 				tablesData.append(tret)
 		return tablesData
 
 	@staticmethod
-	def statistics(_table) -> ULTIPA.UltipaStatistics:
+	def statistics(_table, timeZone, timeZoneOffset) -> ULTIPA.UltipaStatistics:
 		if not _table:
 			return None
-		tableData = FormatType.table(_table)
+		tableData = FormatType.table(_table, timeZone, timeZoneOffset)
 		tret = FormatResponse.formatStatisticsTable(table=tableData)
 		return tret
 
 	@staticmethod
-	def nodeTable(nodeTableData):
+	def nodeTable(nodeTableData, timeZone, timeZoneOffset):
 		SchemaTypeDict = {}
 		SchemaHeaderDict = {}
+		SchemaSubTypeHeaderDict = {}
 		tables = []
 		for header in nodeTableData.node_table.schemas:
 			schemaName = header.schema_name
 			typesDict = {}
 			headerDict = {}
+			subTypesDict = {}
 			for index, header in enumerate(header.properties):
 				typesDict.update({index: header.property_type})
 				headerDict.update({index: header.property_name})
+				subTypesDict.update({index: header.sub_types})
+
 			SchemaTypeDict.update({schemaName: typesDict})
 			SchemaHeaderDict.update({schemaName: headerDict})
+			SchemaSubTypeHeaderDict.update({schemaName: subTypesDict})
 
 		schemaTypeGet = SchemaTypeDict.get
 		schemaHeaderGet = SchemaHeaderDict.get
+		schemaSubTypeGet = SchemaSubTypeHeaderDict.get
 
-		for node_row in nodeTableData.node_table.node_rows:
+		for node_row in nodeTableData.node_table.entity_rows:
+			if node_row.is_null is True:
+				tables.append(ULTIPA.Node(id=None, values=None, schema_name=None, uuid=None))
+				continue
 			data = {}
 			_id = node_row.id
-			# if node_row.id:
-			#     _id = node_row.id
-			# else:
-			#     _id = 0
-			uuid = node_row.uuid if node_row.uuid else None
+			uuid = node_row.uuid
 
 			schema_name = node_row.schema_name
 			if node_row.values:
 				for index, uvalue in enumerate(node_row.values):
-					seria = _Serialize(type=schemaTypeGet(schema_name).get(index), value=uvalue)
+					seria = _Serialize(type=schemaTypeGet(schema_name).get(index), value=uvalue,
+									   subTypes=schemaSubTypeGet(schema_name).get(index), timeZone=timeZone,
+									   timeZoneOffset=timeZoneOffset)
 					value = seria.unserialize()
 					data.update({schemaHeaderGet(schema_name).get(index): value})
 			node = ULTIPA.Node(id=_id, values=data, schema_name=schema_name, uuid=uuid)
 			tables.append(node)
 		return tables
 
 	@staticmethod
-	def edgeTable(edgeTableData):
+	def edgeTable(edgeTableData, timeZone, timeZoneOffset):
 		SchemaTypeDict = {}
 		SchemaHeaderDict = {}
+		SchemaSubTypeHeaderDict = {}
 		tables = []
 		for header in edgeTableData.edge_table.schemas:
 			schemaName = header.schema_name
 			typesDict = {}
 			headerDict = {}
+			subTypesDict = {}
 			for index, header in enumerate(header.properties):
 				typesDict.update({index: header.property_type})
 				headerDict.update({index: header.property_name})
+				subTypesDict.update({index: header.sub_types})
+
 			SchemaTypeDict.update({schemaName: typesDict})
 			SchemaHeaderDict.update({schemaName: headerDict})
+			SchemaSubTypeHeaderDict.update({schemaName: subTypesDict})
 
 		schemaTypeGet = SchemaTypeDict.get
 		schemaHeaderGet = SchemaHeaderDict.get
-		for node_row in edgeTableData.edge_table.edge_rows:
+		schemaSubTypeGet = SchemaSubTypeHeaderDict.get
+
+		for edge_row in edgeTableData.edge_table.entity_rows:
+			if edge_row.is_null is True:
+				tables.append(ULTIPA.Edge(from_id=None, to_id=None, values=None, uuid=None, from_uuid=None,
+										  to_uuid=None, schema_name=None))
+				continue
 			data = {}
-			_from_uuid = node_row.from_uuid
-			_from_id = node_row.from_id
-			_to_uuid = node_row.to_uuid
-			_to_id = node_row.to_id
-			schema_name = node_row.schema_name
-			uuid = node_row.uuid if node_row.uuid else None
-			if node_row.values:
-				for index, uvalue in enumerate(node_row.values):
-					seria = _Serialize(type=schemaTypeGet(schema_name).get(index), value=uvalue)
+			_from_uuid = edge_row.from_uuid
+			_from_id = edge_row.from_id
+			_to_uuid = edge_row.to_uuid
+			_to_id = edge_row.to_id
+			schema_name = edge_row.schema_name
+			uuid = edge_row.uuid
+			if edge_row.values:
+				for index, uvalue in enumerate(edge_row.values):
+					seria = _Serialize(type=schemaTypeGet(schema_name).get(index), value=uvalue,
+									   subTypes=schemaSubTypeGet(schema_name).get(index), timeZone=timeZone,
+									   timeZoneOffset=timeZoneOffset)
 					value = seria.unserialize()
 					data.update({schemaHeaderGet(schema_name).get(index): value})
 			edge = ULTIPA.Edge(from_id=_from_id, to_id=_to_id, values=data, uuid=uuid, from_uuid=_from_uuid,
 							   to_uuid=_to_uuid, schema_name=schema_name)
 			tables.append(edge)
 		return tables
 
 	@staticmethod
+	def attrEntity(entityRows, type: str):
+		entityList = []
+		for data in entityRows.entity_rows:
+			if type == "node":
+				entityList.append(ULTIPA.Node(values=None, uuid=data.uuid))
+			else:
+				entityList.append(ULTIPA.Edge(values=None, uuid=data.uuid))
+		return entityList
+
+	@staticmethod
 	def propertyType(type: str) -> ULTIPA.PropertyType:
 		'''
 		将用户传入的type 转化为 ULTIPA.PropertyType
 		:param type:
 		:return:
 		'''
 		if type.upper() == 'PROPERTY_STRING' or type.upper() == 'STRING':
@@ -633,15 +733,15 @@
 	#                 else:
 	#                     raise ParameterException(err=f'The database does not have a {key} property!')
 	#     else:
 	#         raise ParameterException(err='The database has no properties!')
 	#     return headerList
 
 	@staticmethod
-	def toNodeTableSingle(headers: List[dict], schemaName: str, rows: list,timeZoneOffset=None) -> ULTIPA.NodeTable:
+	def toNodeTableSingle(headers: List[dict], schemaName: str, rows: list, timeZoneOffset=None) -> ULTIPA.NodeTable:
 		newHeaderList = []
 		# 根据 rows 生成新的headers List
 
 		schema_name = schemaName
 		find = list(filter(lambda x: x.get('name') == schema_name, headers))
 		if find:
 			newproperties = []
@@ -690,15 +790,16 @@
 							if rdata in ['_uuid', '_id', '_from_uuid', '_to_uuid', '_from_id', '_to_id']:
 								continue
 							# findproperty = list(
 							#     filter(lambda x: x.get('property_name') == rdata, headerT.get("properties")))
 							if headerPropertyName.get('property_name') == rdata:
 								type = headerPropertyName.get('property_type')
 								if type != None:
-									_seria = _Serialize(type=type, value=row.get(rdata), name=rdata,timeZoneOffset=timeZoneOffset)
+									_seria = _Serialize(type=type, value=row.get(rdata), name=rdata,
+														timeZoneOffset=timeZoneOffset)
 									sdata = _seria.serialize()
 									values.append(sdata)
 									continue
 								else:
 									raise ParameterException('Please create Node Property')
 			nodedata.update({'schema_name': schema_name, 'values': values})
 			nodetable.nodeRows.append(nodedata)
@@ -839,15 +940,15 @@
 					data.update({"from_id": row.from_id})
 				if row.to_id:
 					data.update({"to_id": row.to_id})
 				newEdgeTable.edgeRows.append(data)
 		return newEdgeTable
 
 	@staticmethod
-	def makeNodeTable(schema: ULTIPA_REQUEST.Schema, rows: List[ULTIPA.Node],timeZoneOffset=None) -> ULTIPA.NodeTable:
+	def makeNodeTable(schema: ULTIPA_REQUEST.Schema, rows: List[ULTIPA.Node], timeZoneOffset=None) -> ULTIPA.NodeTable:
 
 		nodetable = ULTIPA.NodeTable([], [])
 		nodetable.schemas.append({"schema_name": schema.name, "properties": []})
 
 		for prop in schema.properties:
 			if prop.isIdType() or prop.isIgnore():
 				continue
@@ -861,15 +962,16 @@
 					continue
 				if proper.name in row.values:
 					value = row.values.get(proper.name)
 					ptype = proper.type
 					checkRet = TypeCheck.checkProperty(ptype, value)
 					if isinstance(checkRet, bool):
 						try:
-							_seria = _Serialize(type=ptype, value=value, name=proper.name,timeZoneOffset=timeZoneOffset)
+							_seria = _Serialize(type=ptype, value=value, name=proper.name,
+												timeZoneOffset=timeZoneOffset)
 							sdata = _seria.serialize()
 							values.append(sdata)
 						except Exception as e:
 							if len(e.args) > 0 and "%s" in e.args[0]:
 								e = e.args[0] % (proper.name, value)
 							raise ParameterException(err=f"node row [{i}] error: {e}")
 
@@ -896,15 +998,65 @@
 				if row.id:
 					data.update({"id": row.id})
 
 				nodetable.nodeRows.append(data)
 		return nodetable
 
 	@staticmethod
-	def makeEdgeTable(schema: ULTIPA_REQUEST.Schema, rows: List[ULTIPA.Edge],timeZoneOffset=None) -> ULTIPA.EdgeTable:
+	def makeEntityNodeTable(schema: ULTIPA_REQUEST.Schema, entity_rows: List[ULTIPA.EntityRow],
+							timeZoneOffset=None) -> ULTIPA.NodeEntityTable:
+
+		nodetable = ULTIPA.NodeEntityTable([], [])
+		nodetable.schemas.append({"schema_name": schema.name, "properties": []})
+
+		for prop in schema.properties:
+			if prop.isIdType() or prop.isIgnore():
+				continue
+			nodetable.schemas[0].get("properties").append(
+				{"property_name": prop.name, "property_type": prop.type, "sub_types": prop.subTypes})
+		for i, row in enumerate(entity_rows):
+			append = True
+			values = []
+			FormatType.checkEntityNodeRow(i, schema, row)
+			for proper in schema.properties:
+				if proper.isIdType() or proper.isIgnore():
+					continue
+				if proper.name in row.values:
+					value = row.values.get(proper.name)
+					ptype = proper.type
+					checkRet = TypeCheck.checkProperty(ptype, value)
+					if isinstance(checkRet, bool):
+						try:
+							_seria = _Serialize(type=ptype, value=value, name=proper.name,
+												timeZoneOffset=timeZoneOffset, subTypes=proper.subTypes)
+							sdata = _seria.serialize()
+							values.append(sdata)
+						except Exception as e:
+							if len(e.args) > 0 and "%s" in e.args[0]:
+								e = e.args[0] % (proper.name, value)
+							raise ParameterException(err=f"node row [{row._getIndex()}] error: {e}")
+
+					else:
+						raise ParameterException(
+							err=checkRet % ("node", row._getIndex(), proper.name, value))
+				else:
+					raise ParameterException(
+						err=f"node row [{row._getIndex()}] error: values doesn't contain property [{proper.name}].")
+			if append:
+				data = {"schema_name": schema.name, "values": values}
+				if row.uuid:
+					data.update({"uuid": row.uuid})
+				if row.id:
+					data.update({"id": row.id})
+
+				nodetable.nodeRows.append(data)
+		return nodetable
+
+	@staticmethod
+	def makeEdgeTable(schema: ULTIPA_REQUEST.Schema, rows: List[ULTIPA.Edge], timeZoneOffset=None) -> ULTIPA.EdgeTable:
 		edgetable = ULTIPA.EdgeTable([], [])
 		edgetable.schemas.append({"schema_name": schema.name, "properties": []})
 		for prop in schema.properties:
 			if prop.isIdType() or prop.isIgnore():
 				continue
 			edgetable.schemas[0].get("properties").append({"property_name": prop.name, "property_type": prop.type})
 		for i, row in enumerate(rows):
@@ -916,15 +1068,16 @@
 					continue
 				if proper.name in row.values:
 					value = row.values.get(proper.name)
 					ptype = proper.type
 					checkRet = TypeCheck.checkProperty(ptype, value)
 					if isinstance(checkRet, bool):
 						try:
-							_seria = _Serialize(type=ptype, value=value, name=proper.name,timeZoneOffset=timeZoneOffset)
+							_seria = _Serialize(type=ptype, value=value, name=proper.name,
+												timeZoneOffset=timeZoneOffset)
 							sdata = _seria.serialize()
 							values.append(sdata)
 						except Exception as e:
 							raise ParameterException(err=f"edge row [{i}] error:{e}.")
 					else:
 						raise ParameterException(
 							err=checkRet % ("edge", i, proper.name, value))
@@ -944,15 +1097,66 @@
 					data.update({"to_id": row.to_id})
 				if row.uuid:
 					data.update({"uuid": row.uuid})
 				edgetable.edgeRows.append(data)
 		return edgetable
 
 	@staticmethod
-	def toEdgeTableSingle(headers: List[object], schemaName: str, values: list,timeZoneOffset=None) -> ULTIPA.EdgeTable:
+	def makeEntityEdgeTable(schema: ULTIPA_REQUEST.Schema, rows: List[ULTIPA.EntityRow],
+							timeZoneOffset=None) -> ULTIPA.EdgeEntityTable:
+		edgetable = ULTIPA.EdgeTable([], [])
+		edgetable.schemas.append({"schema_name": schema.name, "properties": []})
+		for prop in schema.properties:
+			if prop.isIdType() or prop.isIgnore():
+				continue
+			edgetable.schemas[0].get("properties").append({"property_name": prop.name, "property_type": prop.type})
+		for i, row in enumerate(rows):
+			append = True
+			values = []
+			FormatType.checkEntityEdgeRow(i, schema, row)
+			for proper in schema.properties:
+				if proper.isIdType() or proper.isIgnore():
+					continue
+				if proper.name in row.values:
+					value = row.values.get(proper.name)
+					ptype = proper.type
+					checkRet = TypeCheck.checkProperty(ptype, value)
+					if isinstance(checkRet, bool):
+						try:
+							_seria = _Serialize(type=ptype, value=value, name=proper.name, subTypes=proper.subTypes,
+												timeZoneOffset=timeZoneOffset)
+							sdata = _seria.serialize()
+							values.append(sdata)
+						except Exception as e:
+							raise ParameterException(err=f"edge row [{row._getIndex()}] error:{e}.")
+					else:
+						raise ParameterException(
+							err=checkRet % ("edge", row._getIndex(), proper.name, value))
+				else:
+					raise ParameterException(
+						err=f"edge row [{row._getIndex()}] error: values doesn't contain property [{proper.name}].")
+
+			if append:
+				data = {"schema_name": schema.name, "values": values}
+				if row.from_uuid:
+					data.update({"from_uuid": row.from_uuid})
+				if row.to_uuid:
+					data.update({"to_uuid": row.to_uuid})
+				if row.from_id:
+					data.update({"from_id": row.from_id})
+				if row.to_id:
+					data.update({"to_id": row.to_id})
+				if row.uuid:
+					data.update({"uuid": row.uuid})
+				edgetable.edgeRows.append(data)
+		return edgetable
+
+	@staticmethod
+	def toEdgeTableSingle(headers: List[object], schemaName: str, values: list,
+						  timeZoneOffset=None) -> ULTIPA.EdgeTable:
 		# headerList, headertype = FormatType._formatTableHeader(headers)
 		# edgetable = ULTIPA.EdgeTable(headersList=headerList, edgeRowsList=[])
 		# edgetable.headersList = headerList
 		newHeaderList = []
 		schema_name = schemaName
 		find = list(filter(lambda x: x.get('name') == schema_name, headers))
 		if find:
@@ -1010,39 +1214,48 @@
 					if schema_name == headerT.get("schema_name"):
 						for rdata in row.keys():
 							if rdata in ['_uuid', '_id', '_from_uuid', '_to_uuid', '_from', '_to']:
 								continue
 							if headerPropertyName.get('property_name') == rdata:
 								type = headerPropertyName.get('property_type')
 								if type != None:
-									_seria = _Serialize(type=type, value=row.get(rdata), name=rdata,timeZoneOffset=timeZoneOffset)
+									_seria = _Serialize(type=type, value=row.get(rdata), name=rdata,
+														timeZoneOffset=timeZoneOffset)
 									sdata = _seria.serialize()
 									values.append(sdata)
 									continue
 								else:
 									raise ParameterException('Please create Node Property')
 
 			edgedata.update({'schema_name': schema_name, 'values': values})
 			edgetable.edgeRows.append(edgedata)
 		return edgetable
 
 	@staticmethod
-	def nodeAliases(_nodes) -> List[ULTIPA.NodeAlias]:
+	def nodeAliases(_nodes, timeZone, timeZoneOffset) -> List[ULTIPA.NodeAlias]:
 		nodeAliasesData = []
 		if _nodes:
 			for node in _nodes:
-				nodesData = FormatType.nodeTable(node)
+				nodesData = FormatType.nodeTable(node, timeZone, timeZoneOffset)
 				nodeAliasData = ULTIPA.NodeAlias(alias=node.alias, nodes=nodesData)
 				# nodeAliasData = DataItem(alias=node.alias,data=nodesData,type=ResultType.RESULT_TYPE_NODE)
 				# nodeAliasesData.append({'alias':node.alias,node.alias:nodesData})
 				nodeAliasesData.append(nodeAliasData)
 		# nodeAliasesData = nodeAliasData
 		return nodeAliasesData
 
 	@staticmethod
+	def attrNodeEntityTable(data) -> List[ULTIPA.Node]:
+		return FormatType.attrEntity(data, "node")
+
+	@staticmethod
+	def attrEdgeEntityTable(data) -> List[ULTIPA.Edge]:
+		return FormatType.attrEntity(data, "edge")
+
+	@staticmethod
 	def nodeAliases1(_nodes) -> List[ULTIPA.NodeAlias]:
 		if not _nodes:
 			return []
 		nodeData = [None] * len(_nodes)
 		index = -1
 		for node in _nodes:
 			index += 1
@@ -1051,46 +1264,163 @@
 			# nodeAliasData = DataItem(alias=node.alias,data=nodesData,type=ResultType.RESULT_TYPE_NODE)
 			# nodeAliasesData.append({'alias':node.alias,node.alias:nodesData})
 			nodeData[index] = nodeAliasData
 		# nodeAliasesData = nodeAliasData
 		return nodeData
 
 	@staticmethod
-	def edgeAliases(_edges) -> List[ULTIPA.EdgeAlias]:
+	def edgeAliases(_edges, timeZone, timeZoneOffset) -> List[ULTIPA.EdgeAlias]:
 		edgeAliasesData = []
 		if _edges:
 			for edge in _edges:
-				edgesData = FormatType.edgeTable(edge)
+				edgesData = FormatType.edgeTable(edge, timeZone, timeZoneOffset)
 				edgeAliasData = ULTIPA.EdgeAlias(alias=edge.alias, edges=edgesData)
 				edgeAliasesData.append(edgeAliasData)
 		return edgeAliasesData
 
 	@staticmethod
 	def values(_values) -> 'dict':
 		value_dict = {}
 		if _values:
 			for value in _values:
 				value_dict.update({value.key: value.value})
 		return value_dict
 
+	@classmethod
+	def parseAttrListData(cls, datas) -> List[ULTIPA.PaserAttrListData]:
+		PaserAttrRetList = []
+		for data in datas:
+			attrListRet = []
+			pathListRet = []
+			nodetRet = None
+			edgeRet = None
+			attrListData = AttrListData()
+			attrListData.ParseFromString(data)
+			if attrListData.type == ULTIPA.ResultType.RESULT_TYPE_ATTR:
+				for attr in attrListData.attrs:
+					attrListRet.append(cls.parseAttr(attr, None))
+
+			if attrListData.type == ULTIPA.ResultType.RESULT_TYPE_PATH:
+				pathListRet.extend(FormatType.attrPath(attrListData.paths, None, None))
+
+			if attrListData.type == ULTIPA.ResultType.RESULT_TYPE_NODE:
+				nodetRet = FormatType.attrNodeEntityTable(attrListData.nodes)
+
+			if attrListData.type == ULTIPA.ResultType.RESULT_TYPE_EDGE:
+				edgeRet = FormatType.attrEdgeEntityTable(attrListData.edges)
+
+			PaserAttrRetList.append(
+				ULTIPA.PaserAttrListData(attrListData.type, nodes=nodetRet, edges=edgeRet, paths=pathListRet,
+										 attrs=attrListRet))
+		return PaserAttrRetList
+
+	@classmethod
+	def parseAttr(cls, attr, aliasName) -> ULTIPA.AttrAlias:
+		valuesList = []
+		attr_type = attr.value_type
+		# if attr_type == ULTIPA.PropertyType.PROPERTY_NULL:
+		# 	return ULTIPA.AttrAlias(alias=aliasName, values=None,
+		# 							type=ULTIPA_REQUEST.Property._getStringByPropertyType(attr_type))
+		if attr_type == ULTIPA.PropertyType.PROPERTY_LIST:
+			valuesList = FormatType.parseAttrListData(attr.values)
+			return ULTIPA.AttrAlias(alias=aliasName, values=valuesList,
+									type=ULTIPA_REQUEST.Property._getStringByPropertyType(attr_type))
+
+		for att in attr.values:
+			_seria = _Serialize(type=attr_type, value=att)
+			sdata = _seria.unserialize()
+			valuesList.append(sdata)
+		return ULTIPA.AttrAlias(alias=aliasName, values=valuesList,
+								type=ULTIPA_REQUEST.Property._getStringByPropertyType(attr_type))
+
+	@classmethod
+	def parseAttrAlias(cls, attrAlias) -> ULTIPA.AttrAlias:
+		return cls.parseAttr(attrAlias.attr, attrAlias.alias)
+
 	@staticmethod
-	def attrs(_attrs) -> List[ULTIPA.AttrAlias]:
+	def attrAlias1(_attrs) -> List[ULTIPA.AttrAlias]:
 		attr_list = []
 		if _attrs:
 			for attr in _attrs:
-				li = []
-				attr_type = attr.property_type
-				for att in attr.values:
-					# li.append(att)
-					_seria = _Serialize(type=attr_type, value=att)
-					sdata = _seria.unserialize()
-					li.append(sdata)
-				ret = ULTIPA.AttrAlias(alias=attr.alias, values=li,
-									   type=ULTIPA_REQUEST.Property._getStringByPropertyType(attr_type))
-				attr_list.append(ret)
+				# li = []
+				# attr_type = attr.attr.property_type
+				# if attr_type==ULTIPA.PropertyType.PROPERTY_LIST:
+				# 	FormatType.attrListData(attr.attr.values)
+				#
+				# for att in attr.values:
+				# 	_seria = _Serialize(type=attr_type, value=att)
+				# 	sdata = _seria.unserialize()
+				# 	li.append(sdata)
+				# ret = ULTIPA.AttrAlias(alias=attr.alias, values=li,
+				# 					   type=ULTIPA_REQUEST.Property._getStringByPropertyType(attr_type))
+				attr_list.append(FormatType.parseAttrAlias(attr))
+		return attr_list
+
+	@staticmethod
+	def attr(attr, timeZone, timeZoneOffset) -> ULTIPA.Attr:
+		type = attr.value_type
+		result = ULTIPA.Attr(type, None, has_attr_data=False, has_ultipa_data=False,
+							 type_desc=ULTIPA_REQUEST.Property._getStringByPropertyType(type))
+		result.values = []
+		for value in attr.values:
+			if type == ULTIPA.PropertyType.PROPERTY_NULL:
+				result.has_attr_data = True
+				result.values.append(None)
+				continue
+			if type == ULTIPA.PropertyType.PROPERTY_LIST:
+				attrListData = AttrListData()
+				attrListData.ParseFromString(value)
+				result_type: any = attrListData.type
+				if attrListData.is_null:
+					result.values.append(None)
+					continue
+
+				if result_type == ULTIPA.ResultType.RESULT_TYPE_ATTR:
+					attrs = []
+					for attr in attrListData.attrs:
+						att = FormatType.attr(attr, timeZone, timeZoneOffset)
+						if not att.values:
+							attrs.append(att.values)
+						else:
+							attrs.extend(att.values)
+					if len(attrs) != 0:
+						result.has_attr_data = True
+					result.values.append(attrs)
+
+				if result_type == ULTIPA.ResultType.RESULT_TYPE_PATH:
+					result.has_ultipa_data = True
+					result.values.append(ULTIPA.PaserAttrListData(attrListData.type,
+																  paths=FormatType.attrPath(attrListData.paths,
+																							timeZone, timeZoneOffset)))
+
+				if result_type == ULTIPA.ResultType.RESULT_TYPE_NODE:
+					result.has_ultipa_data = True
+					result.values.append(ULTIPA.PaserAttrListData(attrListData.type,
+																  nodes=FormatType.attrNodeEntityTable(
+																	  attrListData.nodes)))
+
+				if result_type == ULTIPA.ResultType.RESULT_TYPE_EDGE:
+					result.has_ultipa_data = True
+					result.values.append(ULTIPA.PaserAttrListData(attrListData.type,
+																  edges=FormatType.attrEdgeEntityTable(
+																	  attrListData.edges)))
+			else:
+				_seria = _Serialize(type=type, value=value, timeZone=timeZone, timeZoneOffset=timeZoneOffset)
+				sdata = _seria.unserialize()
+				result.has_attr_data = True
+				result.values.append(sdata)
+		return result
+
+	@staticmethod
+	def attrAlias(_attrs, timeZone, timeZoneOffset) -> List[ULTIPA.AttrNewAlias]:
+		attr_list = []
+		if _attrs:
+			for attr in _attrs:
+				attr_data = FormatType.attr(attr.attr, timeZone, timeZoneOffset)
+				attr_list.append(ULTIPA.AttrNewAlias(alias=attr.alias, attr=attr_data))
 		return attr_list
 
 	@staticmethod
 	def arrays(_arrays) -> List[ULTIPA.ArrayAlias]:
 		arrays_list = []
 		if _arrays:
 			for attr in _arrays:
@@ -1118,15 +1448,15 @@
 
 	@staticmethod
 	def explainPlan(_explainPlan) -> List[ULTIPA.ExplainPlan]:
 		explainPlanRet = []
 		if _explainPlan:
 			for value in _explainPlan.plan_nodes:
 				explainPlanRet.append(
-					ULTIPA.ExplainPlan(value.type, value.alias, value.children_num, value.uql, value.infos))
+					ULTIPA.ExplainPlan(value.alias, value.children_num, value.uql, value.infos))
 		return explainPlanRet
 
 	# @staticmethod
 	# def nodes(_nodes) -> List:
 	#     nodeData = []
 	#     if _nodes:
 	#         for n in _nodes.nodes:
@@ -1146,52 +1476,67 @@
 	#             for v in n.values:
 	#                 valuesData[v.key] = v.value
 	#             eData = ULTIPA.Edge(n.id, n.from_id, n.to_id, values=valuesData)
 	#             edgeData.append((eData))
 	#     return edgeData
 
 	@staticmethod
-	def export_edges(_edges) -> List:
-		edgeTableData = FormatType.edgeTable(_edges)
+	def export_edges(_edges, timeZone, timeZoneOffset) -> List:
+		edgeTableData = FormatType.edgeTable(_edges, timeZone, timeZoneOffset)
 
 		return edgeTableData
 
 	@staticmethod
-	def export_nodes(_nodes) -> List:
-		nodeTableData = FormatType.nodeTable(_nodes)
+	def export_nodes(_nodes, timeZone, timeZoneOffset) -> List:
+		nodeTableData = FormatType.nodeTable(_nodes, timeZone, timeZoneOffset)
 		return nodeTableData
 
 	# @staticmethod
 	# def path(_paths) -> List[ULTIPA.Path]:
 	#     pathAliasesData = []
 	#     if _paths:
 	#         for path in _paths:
 	#             nodeAliasesData = FormatType.nodeTable(path)
 	#             edgeAliasesData = FormatType.edgeTable(path)
 	#             pathData = ULTIPA.Path(nodes=nodeAliasesData, edges=edgeAliasesData)
 	#             pathAliasesData.append(pathData)
 	#     return pathAliasesData
 
 	@staticmethod
-	def pathAlias(_paths) -> [ULTIPA.PathAlias]:
+	def pathAlias(_paths, timeZone, timeZoneOffset) -> [ULTIPA.PathAlias]:
 		pathData = []
 		if _paths:
 			for path in _paths:
 				pathAlia = ULTIPA.PathAlias(path.alias)
 				for npath in path.paths:
-					nodeAliasesData = FormatType.nodeTable(npath)
-					edgeAliasesData = FormatType.edgeTable(npath)
+					nodeAliasesData = FormatType.nodeTable(npath, timeZone, timeZoneOffset)
+					edgeAliasesData = FormatType.edgeTable(npath, timeZone, timeZoneOffset)
 					nodeSchema, edgeSchema = FormatType.pathScheams(npath)
 					newPath = ULTIPA.Path(nodes=nodeAliasesData, edges=edgeAliasesData, nodeSchemas=nodeSchema,
 										  edgeSchemas=edgeSchema)
 					pathAlia.paths.append(newPath)
 				pathData.append(pathAlia)
 		return pathData
 
 	@staticmethod
+	def attrPath(_paths, timeZone, timeZoneOffset) -> [ULTIPA.Path]:
+		pathData = []
+		if _paths:
+			for path in _paths:
+				# pathAlia = ULTIPA.PathAlias(path.alias)
+				# for npath in path.paths:
+				nodeAliasesData = FormatType.nodeTable(path, timeZone, timeZoneOffset)
+				edgeAliasesData = FormatType.edgeTable(path, timeZone, timeZoneOffset)
+				nodeSchema, edgeSchema = FormatType.pathScheams(path)
+				newPath = ULTIPA.Path(nodes=nodeAliasesData, edges=edgeAliasesData, nodeSchemas=nodeSchema,
+									  edgeSchemas=edgeSchema)
+				pathData.append(newPath)
+		return pathData
+
+	@staticmethod
 	def pathAlias1(_paths) -> [ULTIPA.PathAlias]:
 		if not _paths:
 			return []
 		pathData = [None] * len(_paths)
 		index = -1
 		for path in _paths:
 			index += 1
@@ -1219,54 +1564,104 @@
 			mergeRes.data.paths = DataMerge.concat(mergeRes.data.paths, res.data.paths)
 		if res.data.nodes:
 			mergeRes.data.nodes = DataMerge.concat(mergeRes.data.nodes, res.data.nodes, 'nodes')
 		if res.data.edges:
 			mergeRes.data.edges = DataMerge.concat(mergeRes.data.edges, res.data.edges, 'edges')
 		if res.data.attrs:
 			mergeRes.data.attrs = DataMerge.concat(mergeRes.data.attrs, res.data.attrs, 'values')
-		if res.data.arrays:
-			mergeRes.data.arrays = DataMerge.concat(mergeRes.data.arrays, res.data.arrays, 'arrays')
 		if res.data.tables:
 			mergeRes.data.tables = DataMerge.concat(mergeRes.data.tables, res.data.tables, "table_name", ["headers"])
 		if res.data.explainPlan:
 			mergeRes.data.explainPlan = DataMerge.concat(mergeRes.data.explainPlan, res.data.explainPlan)
 		if res.data.resultAlias:
 			mergeRes.data.resultAlias = DataMerge.concat(mergeRes.data.resultAlias, res.data.resultAlias)
 		if res.statistics:
 			mergeRes.statistics = DataMerge.concat(mergeRes.statistics, res.statistics)
 
 		return mergeRes
 
 	@staticmethod
-	def response(uql_response: ULTIPA_RESPONSE.Response, uqlReply) -> ULTIPA_RESPONSE.Response:
+	def response(uql_response: ULTIPA_RESPONSE.Response, uqlReply, timeZone,
+				 timeZoneOffset) -> ULTIPA_RESPONSE.Response:
+		attrs = FormatType.attrAlias(uqlReply.attrs, timeZone, timeZoneOffset)
+
+		attrs_attrs = []
+		attrs_map = {}
+
+		def addAttributes(alias: str, type: ULTIPA.ResultType, values: any, dataMap: HasDataMap) -> None:
+			if attrs_map.get(alias) is None:
+				if dataMap.has_attr_data:
+					type = ULTIPA.ResultType.RESULT_TYPE_ATTR
+				attralias = ULTIPA.AttrAlias(alias=alias, type=type, type_desc=ULTIPA.ResultType.getTypeStr(type),
+											 values=[])
+				attrs_map[alias] = attralias
+				attrs_attrs.append(attralias)
+			if type == ULTIPA.ResultType.RESULT_TYPE_ATTR and dataMap.only_attr_list:
+				attrs_map[alias].values = values
+			else:
+				attrs_map[alias].values.append(values)
+
+		for attrAlias in attrs:
+			alias = attrAlias.alias
+			has_attr_data = attrAlias.attr.has_attr_data
+			has_ultipa_data = attrAlias.attr.has_ultipa_data
+			only_attr_list = has_attr_data and not has_ultipa_data
+			dataMap = HasDataMap(has_ultipa_data=has_ultipa_data, has_attr_data=has_attr_data,
+								 only_attr_list=only_attr_list)
+			if attrAlias.attr.type == ULTIPA.PropertyType.PROPERTY_LIST:
+				if only_attr_list:
+					addAttributes(alias, ULTIPA.ResultType.RESULT_TYPE_ATTR, attrAlias.attr.values, dataMap)
+					continue
+
+				for row in attrAlias.attr.values:
+					if not row or not row.type:
+						addAttributes(alias, ULTIPA.ResultType.RESULT_TYPE_ATTR, row, dataMap)
+						continue
+
+					if not isinstance(row, ULTIPA.PaserAttrListData):
+						addAttributes(alias, ULTIPA.ResultType.RESULT_TYPE_ATTR, row, dataMap)
+						continue
+
+					if row.type == ULTIPA.ResultType.RESULT_TYPE_NODE:
+						addAttributes(alias, row.type, row.nodes, dataMap)
+
+					elif row.type == ULTIPA.ResultType.RESULT_TYPE_EDGE:
+						addAttributes(alias, row.type, row.edges, dataMap)
+
+					elif row.type == ULTIPA.ResultType.RESULT_TYPE_PATH:
+						addAttributes(alias, row.type, row.paths, dataMap)
+
+			else:
+				addAttributes(alias, ULTIPA.ResultType.RESULT_TYPE_ATTR, attrAlias.attr.values, dataMap)
+
 		status = FormatType.status(uqlReply.status)
-		tables = FormatType.tables(uqlReply.tables)
-		paths = FormatType.pathAlias(uqlReply.paths)
-		nodes = FormatType.nodeAliases(uqlReply.nodes)  # ForamtType.nodeAliases
-		edges = FormatType.edgeAliases(uqlReply.edges)
-		attrs = FormatType.attrs(uqlReply.attrs)
-		arrays = FormatType.arrays(uqlReply.arrays)
-		statistics = FormatType.statistics(uqlReply.statistics)
+		tables = FormatType.tables(uqlReply.tables, timeZone, timeZoneOffset)
+		paths = FormatType.pathAlias(uqlReply.paths, timeZone, timeZoneOffset)
+		nodes = FormatType.nodeAliases(uqlReply.nodes, timeZone, timeZoneOffset)  # ForamtType.nodeAliases
+		edges = FormatType.edgeAliases(uqlReply.edges, timeZone, timeZoneOffset)
+		attrs = attrs_attrs
+		# arrays = FormatType.arrays(uqlReply.arrays)
+		statistics = FormatType.statistics(uqlReply.statistics, timeZone, timeZoneOffset)
 		resultAlias = FormatType.resultalias(uqlReply.alias)
 		explainPlan = FormatType.explainPlan(uqlReply.explain_plan)
 		baseReply = ULTIPA.BaseUqlReply(paths=paths, nodes=nodes, edges=edges, tables=tables,
-										attrs=attrs, arrays=arrays, resultAlias=resultAlias, explainPlan=explainPlan)
+										attrs=attrs, resultAlias=resultAlias, explainPlan=explainPlan)
 		uql_response.status = status
 		uql_response.statistics = statistics
 		uql_response.data = baseReply
 		uql_response.aliases = resultAlias
 		return uql_response
 
 	@staticmethod
-	def uqlResponse(_res) -> ULTIPA_RESPONSE.UltipaResponse:
+	def uqlResponse(_res, timeZone, timeZoneOffset) -> ULTIPA_RESPONSE.UltipaResponse:
 		uql_response = ULTIPA_RESPONSE.Response()
 		ultipa_response = ULTIPA_RESPONSE.UltipaResponse()
 		for uqlReply in _res:
 			status = FormatType.status(uqlReply.status)
-			uql_response = FormatType.response(uql_response, uqlReply)
+			uql_response = FormatType.response(uql_response, uqlReply, timeZone, timeZoneOffset)
 			ret = ULTIPA.UqlReply(dataBase=uql_response.data)
 
 			if status.code != ULTIPA.Code.SUCCESS:
 				ultipa_response.status = uql_response.status
 				ultipa_response.req = uql_response.req
 				return ultipa_response
 
@@ -1274,21 +1669,21 @@
 			# ultipa_response._data = ret.datas
 			ultipa_response.status = uql_response.status
 			ultipa_response.req = uql_response.req
 			ultipa_response.statistics = uql_response.statistics
 			yield ultipa_response
 
 	@staticmethod
-	def uqlMergeResponse(_res) -> ULTIPA_RESPONSE.UltipaResponse:
+	def uqlMergeResponse(_res, timeZone, timeZoneOffset) -> ULTIPA_RESPONSE.UltipaResponse:
 		uql_response = ULTIPA_RESPONSE.Response()
 		mergeRes = ULTIPA_RESPONSE.Response()
 		ultipa_response = ULTIPA_RESPONSE.UltipaResponse()
 		for uqlReply in _res:
 			status = FormatType.status(uqlReply.status)
-			uql_response = FormatType.response(uql_response, uqlReply)
+			uql_response = FormatType.response(uql_response, uqlReply, timeZone, timeZoneOffset)
 			if status.code != ULTIPA.Code.SUCCESS:
 				ultipa_response.status = uql_response.status
 				ultipa_response.req = uql_response.req
 				return ultipa_response
 			mergeRes = FormatType.mergeUqlResponse(mergeRes, uql_response)
 
 		ret = ULTIPA.UqlReply(dataBase=mergeRes.data)
@@ -1308,25 +1703,25 @@
 			data = FormatType.status(uqlReply.chunk)
 			total_time = uqlReply.total_time_cost
 			engine_time = uqlReply.total_time_cost
 			res = ULTIPA_RESPONSE.Response(status, total_time, engine_time, data)
 			return res
 
 	@staticmethod
-	def exportResponse(_res) -> ULTIPA_RESPONSE.Response:
+	def exportResponse(_res, timeZone, timeZoneOffset) -> ULTIPA_RESPONSE.Response:
 		nodedata = []
 		edgedata = []
 		res = ULTIPA_RESPONSE.Response()
 		for uqlReply in _res:
 			# res.statistics=FormatType.statistics(uqlReply.statistics)
 			res.status = FormatType.status(uqlReply.status)
 			if uqlReply.node_table:
-				nodedata = FormatType.export_nodes(uqlReply)
+				nodedata = FormatType.export_nodes(uqlReply, timeZone, timeZoneOffset)
 			if uqlReply.edge_table:
-				edgedata = FormatType.export_edges(uqlReply)
+				edgedata = FormatType.export_edges(uqlReply, timeZone, timeZoneOffset)
 			if nodedata:
 				uql = ULTIPA.ExportReply(data=nodedata)
 				res.data = uql.data
 			if edgedata:
 				uql = ULTIPA.ExportReply(data=edgedata)
 				res.data = uql.data
 			break
```

### Comparing `ultipa-4.2.4/ultipa/utils/logger.py` & `ultipa-4.3.0/ultipa/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/ultipaSchedule.py` & `ultipa-4.3.0/ultipa/utils/ultipaSchedule.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/uql_marker.py` & `ultipa-4.3.0/ultipa/utils/uql_marker.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,23 +89,37 @@
     resumeTask = "resume().task"
     stopTask = "stop().task"
     top = "top"
     kill = "kill"
     mount = "mount().graph"
     unmount = "unmount().graph"
 
+def _replace(value:str):
+    template = re.compile(r"\'?\"?(point\([^)]*\))\'?\"?")
+    matches = re.search(template, value)
+    if matches:
+        return re.sub(r"\'?\"?(point\([^)]*\))\'?\"?",matches.group(1),value)
+    return value
 
 class UQLMAKER:
     def __init__(self, command: CommandList, commandP: any = None, commonParams=None):
         self._command = command
         self._commandP = commandP
         self.commonParams = commonParams
         self._params: List[object] = []
         self.templateParams: List[object] = []
 
+    @staticmethod
+    def PointFunction(latitude: float, longitude: float):
+        return "point({latitude:%s, longitude:%s})" % (latitude,longitude)
+
+    @staticmethod
+    def PointString(latitude: float, longitude: float):
+        return f"POINT({latitude} {longitude})"
+
     def setCommandParams(self, commandP: any):
         if commandP:
             if not isinstance(commandP, list):
                 self._commandP = [commandP]
             else:
                 self._commandP = commandP
             newcommandP = []
@@ -196,14 +210,17 @@
                     value = [{value.toDict().get('name'): value.toDict().get('values')}]
 
             # 判断value 是否为对象 或者 为 str -> select('name')
             # 将 value 变成双引号
             if type(value) == object or type(value) == dict or (
                     type(value) == str and len(value) > 0 and not _notStringify):
                 value = json.dumps(value,ensure_ascii=False)
+            if isinstance(value,list):
+                value =[i for i in value]
+            # value = re.sub("(point\([^)]*\))",value,value)
 
             if value == [] or value == None:
                 return
             self._params.append({"key": key, "value": value})
         except Exception as e:
             raise errors.ParameterException(e)
 
@@ -243,15 +260,15 @@
 
                 if p['key'] in ["select_node_properties", "select_edge_properties", "srcs",
                                 "dests", "return"]:
                     fstr = "{}({})".format(p["key"], value)
                     # fstr = fstr.replace('"' or "'", '')
                 else:
                     fstr = "{}({})".format(p["key"], value)
-
+                fstr = _replace(fstr)
                 ps.append(fstr)
             if len(ps) > 0:
                 uql += "." + ".".join(ps)
         uql += " " + str_return
         return uql.strip()
 
 
@@ -393,13 +410,7 @@
         index = 0
         if matchAll:
             for value in matchAll:
                 result.commands.append(value.strip("("))
                 index += 1
             return result
 
-
-if __name__ == '__main__':
-    ret = UQL.parse("'find().nodes({@test_node}) as n1                insert().overwrite().into(@test_node).nodes([{_uuid:n1._uuid,name:n1.name,age:n1.age+10}])'")
-    # ret = UQL.parse_globle('alter().graph("test_graph125").set({"name": "test_graph126"})')
-
-    print(ret.commands)
```

### Comparing `ultipa-4.2.4/ultipa/utils/errors.py` & `ultipa-4.3.0/ultipa/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/privileges.py` & `ultipa-4.3.0/ultipa/utils/privileges.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/ufilter/ufilter.py` & `ultipa-4.3.0/ultipa/utils/ufilter/ufilter.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/ufilter/new_ufilter.py` & `ultipa-4.3.0/ultipa/utils/ufilter/new_ufilter.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/ultipa/utils/ResposeFormat.py` & `ultipa-4.3.0/ultipa/utils/ResposeFormat.py`

 * *Files identical despite different names*

### Comparing `ultipa-4.2.4/PKG-INFO` & `ultipa-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultipa
-Version: 4.2.4
+Version: 4.3.0
 Summary: Pure Python Ultipa Driver
 Home-page: https://www.ultipa.com/document/ultipa-drivers/python-installation
 Author: Ultipa
 Author-email: support@ultipa.com
 License: PSF
 Keywords: ultipa sdk,ultipa graph
 Platform: UNKNOWN
@@ -25,15 +25,15 @@
 
 <p tit="Bash"></p> 
 
 ```bash
 python3 -m pip install ultipa
 ```
 ## <b>Documentation</b>
-Documentation is available online: [https://www.ultipa.com/document/ultipa-drivers/python-installation/v4.2](https://www.ultipa.cn/document/ultipa-drivers/python-installation/v4.2).
+Documentation is available online: [https://www.ultipa.com/document/ultipa-drivers/python-installation/v4.3](https://www.ultipa.com/document/ultipa-drivers/python-installation/v4.3).
 
 ## <b>Example</b>
 
 Example: Create a server connection and use graphset 'amz'
 <p tit= "Python" ></p> 
  
 ```python
```

### Comparing `ultipa-4.2.4/ultipa.egg-info/PKG-INFO` & `ultipa-4.3.0/ultipa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultipa
-Version: 4.2.4
+Version: 4.3.0
 Summary: Pure Python Ultipa Driver
 Home-page: https://www.ultipa.com/document/ultipa-drivers/python-installation
 Author: Ultipa
 Author-email: support@ultipa.com
 License: PSF
 Keywords: ultipa sdk,ultipa graph
 Platform: UNKNOWN
@@ -25,15 +25,15 @@
 
 <p tit="Bash"></p> 
 
 ```bash
 python3 -m pip install ultipa
 ```
 ## <b>Documentation</b>
-Documentation is available online: [https://www.ultipa.com/document/ultipa-drivers/python-installation/v4.2](https://www.ultipa.cn/document/ultipa-drivers/python-installation/v4.2).
+Documentation is available online: [https://www.ultipa.com/document/ultipa-drivers/python-installation/v4.3](https://www.ultipa.com/document/ultipa-drivers/python-installation/v4.3).
 
 ## <b>Example</b>
 
 Example: Create a server connection and use graphset 'amz'
 <p tit= "Python" ></p> 
  
 ```python
```

### Comparing `ultipa-4.2.4/ultipa.egg-info/SOURCES.txt` & `ultipa-4.3.0/ultipa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ultipa.egg-info/PKG-INFO
 ultipa.egg-info/SOURCES.txt
 ultipa.egg-info/dependency_links.txt
 ultipa.egg-info/requires.txt
 ultipa.egg-info/top_level.txt
 ultipa/connection/__init__.py
 ultipa/connection/autoNet_extra.py
+ultipa/connection/backup_data_extra.py
 ultipa/connection/connection.py
 ultipa/connection/connectionPool.py
 ultipa/connection/connectionPoolMaker.py
 ultipa/connection/connection_base.py
 ultipa/connection/download_extra.py
 ultipa/connection/edge_extra.py
 ultipa/connection/export_extra.py
@@ -50,16 +51,18 @@
 ultipa/utils/checkStrTime.py
 ultipa/utils/common.py
 ultipa/utils/convert.py
 ultipa/utils/errors.py
 ultipa/utils/fileSize.py
 ultipa/utils/format.py
 ultipa/utils/logger.py
+ultipa/utils/nullValue.py
 ultipa/utils/password2md5.py
 ultipa/utils/privileges.py
+ultipa/utils/propertyUtils.py
 ultipa/utils/raftRetry.py
 ultipa/utils/serialize.py
 ultipa/utils/typeCheck.py
 ultipa/utils/ultipaSchedule.py
 ultipa/utils/ultipa_datetime.py
 ultipa/utils/uql_marker.py
 ultipa/utils/ufilter/__init__.py
```

### Comparing `ultipa-4.2.4/setup.py` & `ultipa-4.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     except Exception as e:
         return ""
     return ret
 
 setup(
     app=APP,
     name="ultipa",
-    version="4.2.4",
+    version="4.3.0",
     python_requires='>=3.6, <=3.10',
     packages=find_packages(),  # 常用,要熟悉 :会自动查找当前目录下的所有模块(.py文件) 和包(包含__init___.py文件的文件夹)
     # scripts = ['say_hello.py'],
     # Project uses reStructuredText, so ensure that the docutils get
     # installed or upgraded on the target machine
     install_requires=[
                 'grpcio==1.48.2',
```

