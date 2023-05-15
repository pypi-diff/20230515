# Comparing `tmp/tikit-1.4.2.230424.tar.gz` & `tmp/tikit-1.4.3.230512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikit-1.4.2.230424.tar", last modified: Fri May  5 03:32:35 2023, max compression
+gzip compressed data, was "dist/tikit-1.4.3.230512.tar", last modified: Mon May 15 07:26:37 2023, max compression
```

## Comparing `tikit-1.4.2.230424.tar` & `tikit-1.4.3.230512.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.167060 tikit-1.4.2.230424/
--rw-r--r--   0 liuliu     (501) staff       (20)       71 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/MANIFEST.in
--rw-r--r--   0 liuliu     (501) staff       (20)      700 2023-05-05 03:32:35.166245 tikit-1.4.2.230424/PKG-INFO
--rw-r--r--   0 liuliu     (501) staff       (20)      499 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/README.md
--rw-r--r--   0 liuliu     (501) staff       (20)      413 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/requirements.txt
--rw-r--r--   0 liuliu     (501) staff       (20)       38 2023-05-05 03:32:35.167300 tikit-1.4.2.230424/setup.cfg
--rw-r--r--   0 liuliu     (501) staff       (20)      858 2023-05-05 03:32:25.000000 tikit-1.4.2.230424/setup.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.115871 tikit-1.4.2.230424/tikit/
--rw-r--r--   0 liuliu     (501) staff       (20)      185 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     7896 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/cli.py
--rw-r--r--   0 liuliu     (501) staff       (20)   194491 2023-05-05 03:32:25.000000 tikit-1.4.2.230424/tikit/client.py
--rw-r--r--   0 liuliu     (501) staff       (20)     3976 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/default_client.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.130488 tikit-1.4.2.230424/tikit/display_optimize/
--rw-r--r--   0 liuliu     (501) staff       (20)      133 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     3820 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/dataset.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1628 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/resource_group.py
--rw-r--r--   0 liuliu     (501) staff       (20)     3951 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/training_model.py
--rw-r--r--   0 liuliu     (501) staff       (20)     4973 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/display_optimize/training_task.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1779 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/hdfs.py
--rw-r--r--   0 liuliu     (501) staff       (20)    35661 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/hive.py
--rw-r--r--   0 liuliu     (501) staff       (20)    19526 2023-05-05 03:32:25.000000 tikit-1.4.2.230424/tikit/models.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.131709 tikit-1.4.2.230424/tikit/templates/
--rw-r--r--   0 liuliu     (501) staff       (20)     7622 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/templates/service_config.yaml
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.133098 tikit-1.4.2.230424/tikit/tencentcloud/
--rw-r--r--   0 liuliu     (501) staff       (20)      630 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/__init__.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.139191 tikit-1.4.2.230424/tikit/tencentcloud/common/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)    16473 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/abstract_client.py
--rw-r--r--   0 liuliu     (501) staff       (20)     2337 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/abstract_model.py
--rw-r--r--   0 liuliu     (501) staff       (20)     2002 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/common_client.py
--rw-r--r--   0 liuliu     (501) staff       (20)    12338 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/credential.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.141706 tikit-1.4.2.230424/tikit/tencentcloud/common/exception/
--rw-r--r--   0 liuliu     (501) staff       (20)      741 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)      760 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.143927 tikit-1.4.2.230424/tikit/tencentcloud/common/http/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/http/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     5071 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/http/request.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.147151 tikit-1.4.2.230424/tikit/tencentcloud/common/profile/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1657 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1857 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 liuliu     (501) staff       (20)     1574 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/common/sign.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.148120 tikit-1.4.2.230424/tikit/tencentcloud/emr/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.151420 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)     6015 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 liuliu     (501) staff       (20)     3465 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 liuliu     (501) staff       (20)    33848 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/models.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.153323 tikit-1.4.2.230424/tikit/tencentcloud/tione/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.157770 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)    12419 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 liuliu     (501) staff       (20)   747496 2023-05-05 03:32:25.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 liuliu     (501) staff       (20)   260703 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/tione_client.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.160680 tikit-1.4.2.230424/tikit/tencentcloud/wedata/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.165030 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/
--rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 liuliu     (501) staff       (20)      819 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 liuliu     (501) staff       (20)    19834 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 liuliu     (501) staff       (20)     4802 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 liuliu     (501) staff       (20)      893 2023-04-06 06:58:27.000000 tikit-1.4.2.230424/tikit/util.py
-drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-05 03:32:35.125569 tikit-1.4.2.230424/tikit.egg-info/
--rw-r--r--   0 liuliu     (501) staff       (20)      700 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/PKG-INFO
--rw-r--r--   0 liuliu     (501) staff       (20)     1883 2023-05-05 03:32:35.000000 tikit-1.4.2.230424/tikit.egg-info/SOURCES.txt
--rw-r--r--   0 liuliu     (501) staff       (20)        1 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/dependency_links.txt
--rw-r--r--   0 liuliu     (501) staff       (20)       40 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/entry_points.txt
--rw-r--r--   0 liuliu     (501) staff       (20)      413 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/requires.txt
--rw-r--r--   0 liuliu     (501) staff       (20)        6 2023-05-05 03:32:34.000000 tikit-1.4.2.230424/tikit.egg-info/top_level.txt
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/
+-rw-r--r--   0 kaihuang   (501) staff       (20)       71 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/MANIFEST.in
+-rw-r--r--   0 kaihuang   (501) staff       (20)      858 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/PKG-INFO
+-rw-r--r--   0 kaihuang   (501) staff       (20)      499 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/README.md
+-rw-r--r--   0 kaihuang   (501) staff       (20)      413 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/requirements.txt
+-rw-r--r--   0 kaihuang   (501) staff       (20)       38 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/setup.cfg
+-rw-r--r--   0 kaihuang   (501) staff       (20)      858 2023-05-15 03:33:34.000000 tikit-1.4.3.230512/setup.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/
+-rw-r--r--   0 kaihuang   (501) staff       (20)      185 2023-01-05 02:27:12.000000 tikit-1.4.3.230512/tikit/__init__.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     7896 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/cli.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)   195907 2023-05-15 04:30:12.000000 tikit-1.4.3.230512/tikit/client.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     3976 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/default_client.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/display_optimize/
+-rw-r--r--   0 kaihuang   (501) staff       (20)      133 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/__init__.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     3820 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/dataset.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     1628 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/resource_group.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     3951 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/training_model.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     4973 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/training_task.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     1779 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/hdfs.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)    35661 2023-04-17 06:40:50.000000 tikit-1.4.3.230512/tikit/hive.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)    19526 2023-05-05 11:53:57.000000 tikit-1.4.3.230512/tikit/models.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/templates/
+-rw-r--r--   0 kaihuang   (501) staff       (20)     7622 2023-04-17 06:40:50.000000 tikit-1.4.3.230512/tikit/templates/service_config.yaml
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/
+-rw-r--r--   0 kaihuang   (501) staff       (20)      630 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/__init__.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/
+-rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/__init__.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)    16473 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     2337 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     2002 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/common_client.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)    12338 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/credential.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/exception/
+-rw-r--r--   0 kaihuang   (501) staff       (20)      741 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)      760 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/http/
+-rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     5071 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/http/request.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/profile/
+-rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     1657 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     1857 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     1574 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/sign.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/
+-rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/
+-rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     6015 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     3465 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)    33848 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/models.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/
+-rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/
+-rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)    12419 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)   747496 2023-05-05 11:53:57.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)   260703 2023-04-17 06:40:50.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/tione_client.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/
+-rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)      819 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)    19834 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)     4802 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 kaihuang   (501) staff       (20)      893 2023-04-17 06:40:50.000000 tikit-1.4.3.230512/tikit/util.py
+drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/
+-rw-r--r--   0 kaihuang   (501) staff       (20)      858 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/PKG-INFO
+-rw-r--r--   0 kaihuang   (501) staff       (20)     1883 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/SOURCES.txt
+-rw-r--r--   0 kaihuang   (501) staff       (20)        1 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/dependency_links.txt
+-rw-r--r--   0 kaihuang   (501) staff       (20)       41 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/entry_points.txt
+-rw-r--r--   0 kaihuang   (501) staff       (20)      413 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/requires.txt
+-rw-r--r--   0 kaihuang   (501) staff       (20)        6 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tikit-1.4.2.230424/PKG-INFO` & `tikit-1.4.3.230512/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.0
 Name: tikit
-Version: 1.4.2.230424
+Version: 1.4.3.230512
 Summary: Kit for TI PLATFORM
 Home-page: https://cloud.tencent.com/
 Author: TI PLATFORM TEAM
 Author-email: TI_Platform@tencent.com
 License: MIT
-
-TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
-Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
-
-# 发布
-'''bash
-# 公网
-make publish
-'''
-
-# 开发
-'''bash
-yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
-pip install -r requirements.txt
-'''
-# 公网
-pip install tikit -U -i https://pypi.org/simple
-'''
+Description: TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
+        Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
+        
+        # 发布
+        '''bash
+        # 公网
+        make publish
+        '''
+        
+        # 开发
+        '''bash
+        yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
+        pip install -r requirements.txt
+        '''
+        # 公网
+        pip install tikit -U -i https://pypi.org/simple
+        '''
+Platform: UNKNOWN
```

### Comparing `tikit-1.4.2.230424/setup.py` & `tikit-1.4.3.230512/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def long_description():
     with io.open('README.md', 'r', encoding='utf8') as fileobj:
         return fileobj.read()
 
 
 setup(
     name='tikit',
-    version='1.4.2.230424',
+    version='1.4.3.230512',
     url='https://cloud.tencent.com/',
     license='MIT',
     author='TI PLATFORM TEAM',
     author_email='TI_Platform@tencent.com',
     description='Kit for TI PLATFORM',
     long_description=long_description(),
     packages=find_packages(),
```

### Comparing `tikit-1.4.2.230424/tikit/cli.py` & `tikit-1.4.3.230512/tikit/cli.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/client.py` & `tikit-1.4.3.230512/tikit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,41 @@
             Prefix=path.strip("/") + "/",
             MaxKeys=1
         )
         if "Contents" in objects and len(objects["Contents"]) > 0:
             return True
         return False
 
+    def check_object_exist(self, bucket, cos_path):
+        """ 判断某个object是否存在
+        如果是判断某个目录存在，需要保证cos_path 以 / 结尾
+        如果是判断某个文件存在，需要保证cos_path 不以 / 结尾
+
+        :param bucket:      cos上的桶
+        :param cos_path:    cos上的路径key
+        :return:            指定对象是否存在
+        :rtype:             bool, 错误信息通过 raise 给出
+        """
+        rsp = self._cos_client.object_exists(bucket, cos_path)
+        return rsp
+
+    def mkdir(self, bucket, cos_path):
+        """ cos上创建目录
+        注: 对象存储本身是没有目录概念, 为了保证用户的使用习惯, 此处创建一个以cos_path为指定key, key以 / 结尾的0kb大小的对象
+
+        :param bucket:      cos上的桶
+        :param cos_path:    cos上的路径key
+        :return:            None, 错误信息通过 raise 给出
+        """
+        cos_path = str(cos_path)
+        if cos_path.endswith("/"):
+            cos_path = cos_path.rstrip("/")
+        cos_path = cos_path + "/"
+        self._cos_client.put_object(Bucket=bucket, Key=cos_path, Body=b'')
+
     def upload_to_cos(self, local_path, bucket, cos_path):
         """把本地路径下的文件或者目录上传到cos上
 
         :param local_path:  本地路径
         :type local_path:   str
         :param bucket:      cos上的桶
         :type bucket:       str
@@ -158,14 +185,17 @@
         :type cos_path:     str
         :return:            None. 错误信息通过 raise 给出。
         :rtype:
         """
         if not os.path.exists(local_path):
             raise Exception("local path is not exist, please check it.")
 
+        # 不管cos_path是否存在, 都以此路径创建目录
+        self.mkdir(bucket, cos_path)
+
         if os.path.isfile(local_path):
             if cos_path.endswith("/"):
                 cos_path = os.path.join(cos_path, os.path.basename(local_path))
             self._cos_client.upload_file(
                 Bucket=bucket,
                 LocalFilePath=local_path,
                 Key=cos_path,
@@ -182,19 +212,24 @@
             if self.is_cos_dir(bucket, cos_path):
                 base_path = os.path.join(base_path, os.path.basename(local_path))
             for path, dir_list, file_list in walk:
                 pre_path = os.path.join(base_path, path[local_path_length:].strip('/'))
                 for file_name in file_list:
                     src_key = os.path.join(path, file_name)
                     cos_object_key = os.path.join(pre_path, file_name).strip('/')
+                    # 假如存在错误的软链时, 或者其他意外情况导致的文件不存在时, 跳过
+                    if not os.path.exists(src_key):
+                        print(src_key, 'does not exist, ignore it')
+                        continue
                     pool.add_task(self._cos_client.upload_file, bucket, cos_object_key, src_key)
 
             pool.wait_completion()
             result = pool.get_result()
             if not result['success_all']:
+                self.__dump_error_result(result)
                 raise Exception("failed to upload files to cos, please retry")
             return
 
     def describe_cos_path(self, bucket, path, maker="", max_keys=1000, encoding_type=""):
         """获取cos的目录的信息。目录下的内容最多显示1000个。要显示目录下的文件和文件夹，请以"/"结尾
 
         :param bucket:          cos的桶
@@ -268,76 +303,77 @@
             marker = response["NextMarker"]
 
         pool.wait_completion()
         result = pool.get_result()
         if not result['success_all']:
             raise Exception("failed to delete files, please retry")
 
+    def __dump_error_result(self, result):
+        """
+        私有方法, 用来dump出cos的SimpleThreadPool运行过程中的错误信息
+        """
+        if 'detail' not in result:
+            return
+
+        detail = result['detail']
+        for tp in detail:
+            if tp[1] != 0:
+                # 当failed的任务个数不为0时，打印第三个返回值, 即错误信息
+                print(tp[2])
+
     def download_from_cos(self, bucket, cos_path, local_path):
         """从cos上下载文件或者目录本地。
         注意：本地文件存在会直接覆盖。 cos_path为目录且local_path 为存在的目录的时候，cos_path的文件夹名会作为子目录保留。
 
         :param bucket:      cos上的桶
         :type bucket:       str
         :param cos_path:    cos上的路径
         :type cos_path:     str
-        :param local_path:  本地路径
+        :param local_path:  本地路径, 需要为目录
         :type local_path:   str
         :return:            None. 错误信息通过 raise 给出。
         :rtype:
         """
         file_infos = self.get_cos_sub_files(bucket, cos_path)
-        # 下载文件
-        if len(file_infos) == 1 and file_infos[0]["Key"] == cos_path:
-            if os.path.isdir(local_path) or local_path.endswith("/"):
-                local_name = os.path.join(local_path, os.path.basename(cos_path))
-                if self.__need_download_from_cos(bucket, cos_path, local_name):
-                    self._cos_client.download_file(bucket, cos_path, local_name)
-            else:
-                local_dir = os.path.dirname(local_path)
-                if local_dir != "" and not os.path.exists(local_dir):
-                    os.makedirs(local_dir)
-                if self.__need_download_from_cos(bucket, cos_path, local_path):
-                    self._cos_client.download_file(bucket, cos_path, local_path)
-            return
         if len(file_infos) == 0:
             raise Exception("cos path \"%s\" not existed" % cos_path)
-
-        # 下载目录
         if os.path.isfile(local_path):
-            raise Exception("cannot download directory into file \"%s\"" % local_path)
+            raise Exception("local_path parameter \"%s\" should be directory" % local_path)
+
         # 下载目录时，如果不存在则创建
         os.makedirs(local_path, exist_ok=True)
         target_path = local_path
         # local_path 为存在的目录的时候
         if os.path.isdir(local_path):
             target_path = os.path.join(target_path, os.path.basename(cos_path))
         cos_path_length = len(cos_path)
         pool = SimpleThreadPool()
         for file in file_infos:
             # 文件下载 获取文件到本地
             file_cos_key = file["Key"]
-            local_name = os.path.join(target_path, file_cos_key[cos_path_length:].strip('/'))
+            local_name = os.path.join(target_path, file_cos_key[cos_path_length:].strip('/')).strip("/")
+
+            # 如果存在目录类型的object, 则直接跳过不做下载操作
+            file_cos_key = str(file_cos_key)
+            if file_cos_key.endswith("/") and int(file["Size"]) == 0:
+                continue
 
             # 如果本地目录结构不存在，递归创建
             local_dir = os.path.dirname(local_name)
             if local_dir != "" and not os.path.exists(local_dir):
                 os.makedirs(local_dir)
 
-            # skip dir, no need to download it
-            if str(local_name).endswith("/"):
-                continue
-
             # 使用线程池方式
             if self.__need_download_from_cos(bucket, file_cos_key, local_name):
                 pool.add_task(self._cos_client.download_file, bucket, file_cos_key, local_name)
 
         pool.wait_completion()
         result = pool.get_result()
         if not result['success_all']:
+            self.__dump_error_result(result)
             raise Exception("failed to download files, please retry")
 
     def get_cos_sub_files(self, bucket, prefix):
         """列出当前目录子节点，返回所有子节点信息
 
         :param bucket:
         :type bucket:
```

### Comparing `tikit-1.4.2.230424/tikit/default_client.py` & `tikit-1.4.3.230512/tikit/default_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/display_optimize/dataset.py` & `tikit-1.4.3.230512/tikit/display_optimize/dataset.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/display_optimize/resource_group.py` & `tikit-1.4.3.230512/tikit/display_optimize/resource_group.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/display_optimize/training_model.py` & `tikit-1.4.3.230512/tikit/display_optimize/training_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/display_optimize/training_task.py` & `tikit-1.4.3.230512/tikit/display_optimize/training_task.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/hdfs.py` & `tikit-1.4.3.230512/tikit/hdfs.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/hive.py` & `tikit-1.4.3.230512/tikit/hive.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/models.py` & `tikit-1.4.3.230512/tikit/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/templates/service_config.yaml` & `tikit-1.4.3.230512/tikit/templates/service_config.yaml`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/__init__.py` & `tikit-1.4.3.230512/tikit/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/abstract_client.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/abstract_model.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/common_client.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/credential.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/exception/__init__.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/http/request.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/profile/client_profile.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/profile/http_profile.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/common/sign.py` & `tikit-1.4.3.230512/tikit/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/emr_client.py` & `tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/errorcodes.py` & `tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/emr/v20190103/models.py` & `tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/errorcodes.py` & `tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/models.py` & `tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/tione/v20211111/tione_client.py` & `tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/errorcodes.py` & `tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/models.py` & `tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/tencentcloud/wedata/v20210820/wedata_client.py` & `tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit/util.py` & `tikit-1.4.3.230512/tikit/util.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.2.230424/tikit.egg-info/PKG-INFO` & `tikit-1.4.3.230512/tikit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.0
 Name: tikit
-Version: 1.4.2.230424
+Version: 1.4.3.230512
 Summary: Kit for TI PLATFORM
 Home-page: https://cloud.tencent.com/
 Author: TI PLATFORM TEAM
 Author-email: TI_Platform@tencent.com
 License: MIT
-
-TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
-Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
-
-# 发布
-'''bash
-# 公网
-make publish
-'''
-
-# 开发
-'''bash
-yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
-pip install -r requirements.txt
-'''
-# 公网
-pip install tikit -U -i https://pypi.org/simple
-'''
+Description: TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
+        Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
+        
+        # 发布
+        '''bash
+        # 公网
+        make publish
+        '''
+        
+        # 开发
+        '''bash
+        yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
+        pip install -r requirements.txt
+        '''
+        # 公网
+        pip install tikit -U -i https://pypi.org/simple
+        '''
+Platform: UNKNOWN
```

### Comparing `tikit-1.4.2.230424/tikit.egg-info/SOURCES.txt` & `tikit-1.4.3.230512/tikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

