# Comparing `tmp/renus-1.1.3.tar.gz` & `tmp/renus-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.1.3.tar", last modified: Sun May 14 05:42:37 2023, max compression
+gzip compressed data, was "renus-1.1.4.tar", last modified: Mon May 15 08:08:00 2023, max compression
```

## Comparing `renus-1.1.3.tar` & `renus-1.1.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.525927 renus-1.1.3/
--rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      220 2023-05-14 05:42:37.523925 renus-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.351939 renus-1.1.3/renus/
--rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.3/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.3/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.392960 renus-1.1.3/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.410923 renus-1.1.3/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     1786 2023-05-03 04:46:26.000000 renus-1.1.3/renus/commands/app/controller.temp
--rw-rw-rw-   0        0        0     1008 2023-05-03 09:35:45.000000 renus-1.1.3/renus/commands/app/model.temp
--rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.3/renus/commands/app/route.temp
--rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.3/renus/commands/app/run.py
--rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.3/renus/commands/app/vue.temp
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.416923 renus-1.1.3/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.3/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.422959 renus-1.1.3/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.3/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.428959 renus-1.1.3/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-30 01:41:46.000000 renus-1.1.3/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.1.3/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.439920 renus-1.1.3/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.3/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.1.3/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.3/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.444925 renus-1.1.3/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.3/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.506927 renus-1.1.3/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.3/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/config.py
--rw-rw-rw-   0        0        0     2368 2023-05-03 09:54:55.000000 renus-1.1.3/renus/core/cprint.py
--rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.3/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.3/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.3/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.3/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/middleware.py
--rw-rw-rw-   0        0        0    14800 2023-04-20 18:01:14.000000 renus-1.1.3/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.3/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.3/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.3/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.3/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.3/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.515932 renus-1.1.3/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8909 2023-05-14 05:18:01.000000 renus-1.1.3/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3552 2023-05-14 05:22:21.000000 renus-1.1.3/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/websockets.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.520931 renus-1.1.3/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.3/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.382927 renus-1.1.3/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-05-14 05:42:37.000000 renus-1.1.3/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1426 2023-05-14 05:42:37.000000 renus-1.1.3/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 05:42:37.000000 renus-1.1.3/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-14 05:42:37.000000 renus-1.1.3/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 05:42:37.526935 renus-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-05-14 05:39:59.000000 renus-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:08:00.091553 renus-1.1.4/
+-rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      220 2023-05-15 08:08:00.091553 renus-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.532617 renus-1.1.4/renus/
+-rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.4/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.4/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.560619 renus-1.1.4/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.619617 renus-1.1.4/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     1786 2023-05-03 04:46:26.000000 renus-1.1.4/renus/commands/app/controller.temp
+-rw-rw-rw-   0        0        0     1143 2023-05-15 07:03:04.000000 renus-1.1.4/renus/commands/app/model.temp
+-rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.4/renus/commands/app/route.temp
+-rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.4/renus/commands/app/run.py
+-rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.4/renus/commands/app/vue.temp
+drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.644763 renus-1.1.4/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.4/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.654761 renus-1.1.4/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.4/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.672132 renus-1.1.4/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-30 01:41:46.000000 renus-1.1.4/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1472 2023-05-15 06:28:58.000000 renus-1.1.4/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.707949 renus-1.1.4/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.4/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     4042 2023-05-15 07:57:33.000000 renus-1.1.4/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.4/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.725527 renus-1.1.4/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.4/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:08:00.051537 renus-1.1.4/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.4/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/config.py
+-rw-rw-rw-   0        0        0     2368 2023-05-03 09:54:55.000000 renus-1.1.4/renus/core/cprint.py
+-rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.4/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.4/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.4/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.4/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    14400 2023-05-15 07:00:53.000000 renus-1.1.4/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.4/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.4/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.4/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.4/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.4/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:08:00.079555 renus-1.1.4/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0     8909 2023-05-14 05:18:01.000000 renus-1.1.4/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3552 2023-05-14 05:22:21.000000 renus-1.1.4/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/websockets.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:08:00.089537 renus-1.1.4/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.4/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.551618 renus-1.1.4/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-05-15 08:07:59.000000 renus-1.1.4/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1426 2023-05-15 08:07:59.000000 renus-1.1.4/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 08:07:59.000000 renus-1.1.4/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-15 08:07:59.000000 renus-1.1.4/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 08:08:00.091553 renus-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-05-15 08:07:19.000000 renus-1.1.4/setup.py
```

### Comparing `renus-1.1.3/LICENSE` & `renus-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/app.py` & `renus-1.1.4/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/commands/app/controller.temp` & `renus-1.1.4/renus/commands/app/controller.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/commands/app/model.temp` & `renus-1.1.4/renus/commands/app/model.temp`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing
 from datetime import datetime
 from bson import ObjectId
 from renus.core.model import ModelBase
 from app.extension.renus.activity.service import ActivityService
 from app.extension.renus.crud.model import CRUD
+from app.extension.renus.storage.model import Storage
 
 class _Base(dict):
     _id: ObjectId
     created_at: datetime
     updated_at: datetime
 
     def __init__(self, doc):
@@ -15,18 +16,20 @@
         for k, v in doc.items():
             setattr(self, k, v)
 
 
 class {name_camel}(ModelBase,CRUD):
     collection_name="{name_db}"
     document_model=_Base
+    file_remove_func=
 
     def __init__(self,request) -> None:
         super().__init__()
         self.request=request
+        self.file_remove_func = Storage(request).remove
 
     def get(self,police: bool = True) -> typing.List[document_model]:
         return self._get(police)
 
     def first(self,police: bool = True) -> typing.Union[document_model,None]:
         return self._first(police)
```

### Comparing `renus-1.1.3/renus/commands/app/route.temp` & `renus-1.1.4/renus/commands/app/route.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/commands/app/run.py` & `renus-1.1.4/renus/commands/app/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/commands/backup/run.py` & `renus-1.1.4/renus/commands/backup/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/commands/copy/run.py` & `renus-1.1.4/renus/commands/copy/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/commands/default/run.py` & `renus-1.1.4/renus/commands/default/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/commands/help.py` & `renus-1.1.4/renus/commands/help.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,13 +28,14 @@
         for row_format, row in zip(table_format, table))
 
 
 def Help():
     print(format({
         'app': 'Create New Package',
         'install renus/user/*': 'Install Apps',
+        'install -update renus/user/*': 'Update Apps',
         'backup': 'Backing up the entire project',
         'copy': 'Get a copy of the app to upload to the server',
         'permission': 'Add All Permissions to DB',
         'default super_admin': 'Create Super Admin'
     },
         '{:<{}}', '{:<{}}', '\n\n', ' | '))
```

### Comparing `renus-1.1.3/renus/commands/install/build.py` & `renus-1.1.4/renus/commands/install/build.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/commands/install/run.py` & `renus-1.1.4/renus/commands/install/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
     installed[app] = res.headers['version']
     f = zipfile.ZipFile(BytesIO(res.content))
     shutil.rmtree(f"extension/{app}", True)
     f.extractall(f"extension/{app}")
     if not isUpdate:
         install_app(app, installed)
+    else:
+        print(f'{bc.OKBLUE}   updated to version{res.headers["version"]}{bc.ENDC}')
     return res.headers['version']
 
 
 def rewrite(installed):
     print('   rewrite installed')
     pre_line = ''
     with open('extension/install.py', 'r') as f:
```

### Comparing `renus-1.1.3/renus/commands/install/service.py` & `renus-1.1.4/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/commands/permission/run.py` & `renus-1.1.4/renus/commands/permission/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/cache.py` & `renus-1.1.4/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/concurrency.py` & `renus-1.1.4/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/cprint.py` & `renus-1.1.4/renus/core/cprint.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/crypt.py` & `renus-1.1.4/renus/core/crypt.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/datastructures.py` & `renus-1.1.4/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/exception.py` & `renus-1.1.4/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/formparsers.py` & `renus-1.1.4/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/injection.py` & `renus-1.1.4/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/log.py` & `renus-1.1.4/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/model.py` & `renus-1.1.4/renus/core/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,21 @@
                           Config('database').get('port', 27017),
                           username=Config('database').get('username', None),
                           password=Config('database').get('password', None))
 
     _database_name = Config('database').get('name', 'renus')
     collection_name=None
     metro = None
-    public_folder='public'
+    file_remove_func=None
     hidden_fields = []
     document_model=dict
     add_time_fields=True
     def __init__(self) -> None:
         if hasattr(self, '_collection_name'):
             raise RuntimeError('_collection_name has expired. Use collection_name')
-        if hasattr(self, '_public_folder'):
-            raise RuntimeError('_public_folder has expired. Use public_folder')
         self._steps = None
         self._where = None
         self._distinct = None
         self._limit = None
         self._skip = None
         self._sort = None
         self._select = None
@@ -408,23 +406,16 @@
         if type(links) is dict:
             links = list(links.values())
         if type(links) is not list:
             links = [links]
 
         for link in links:
             if type(link) is str:
-                link = link.replace('storage/img/', '', 1)
-                link = link.replace('storage/', '', 1)
+                self.file_remove_func(link)
             elif type(link) is dict:
-                link = link.get('url').replace('storage/img/', '', 1)
-                link = link.replace('storage/', '', 1)
+                self.file_remove_func(link.get('url'))
             else:
                 raise RuntimeError(f"type {link} must be string or dict but its {type(link)}")
 
-            try:
-                os.remove(f'storage/{self.public_folder}/' + link)
-            except:
-                pass
-
     @property
     def database_name(self):
         return self._database_name
```

### Comparing `renus-1.1.3/renus/core/request.py` & `renus-1.1.4/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/response.py` & `renus-1.1.4/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/routing.py` & `renus-1.1.4/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/schedule.py` & `renus-1.1.4/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/serialize.py` & `renus-1.1.4/renus/core/serialize.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/status.py` & `renus-1.1.4/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/validation/rules.py` & `renus-1.1.4/renus/core/validation/rules.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/validation/validate.py` & `renus-1.1.4/renus/core/validation/validate.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/core/websockets.py` & `renus-1.1.4/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus/util/helper.py` & `renus-1.1.4/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.3/renus.egg-info/SOURCES.txt` & `renus-1.1.4/renus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

