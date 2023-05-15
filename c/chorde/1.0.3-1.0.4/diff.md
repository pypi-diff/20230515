# Comparing `tmp/chorde-1.0.3.tar.gz` & `tmp/chorde-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chorde-1.0.3.tar", last modified: Fri Apr 21 13:38:18 2023, max compression
+gzip compressed data, was "chorde-1.0.4.tar", last modified: Mon May 15 17:04:26 2023, max compression
```

## Comparing `chorde-1.0.3.tar` & `chorde-1.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-04-21 13:38:18.450059 chorde-1.0.3/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     7983 2023-04-21 13:35:41.000000 chorde-1.0.3/CHANGELOG
--rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.3/MANIFEST.in
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-04-21 13:38:18.450059 chorde-1.0.3/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.3/README.rst
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-04-21 13:38:18.422059 chorde-1.0.3/lib/
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-04-21 13:38:18.426059 chorde-1.0.3/lib/chorde/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.3/lib/chorde/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-04-21 13:34:45.000000 chorde-1.0.3/lib/chorde/_version.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-04-21 13:38:18.450059 chorde-1.0.3/lib/chorde/clients/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/clients/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   656375 2023-04-17 14:22:41.000000 chorde-1.0.3/lib/chorde/clients/_async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      333 2020-05-05 20:27:26.000000 chorde-1.0.3/lib/chorde/clients/_async.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    15340 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/clients/_async.pyx
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.3/lib/chorde/clients/async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2731676 2023-04-17 14:22:41.000000 chorde-1.0.3/lib/chorde/clients/asyncache.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    65380 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/clients/asyncache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.3/lib/chorde/clients/base.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/clients/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/clients/coherent.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/clients/elasticache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/clients/files.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.3/lib/chorde/clients/inproc.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/clients/inproc.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.3/lib/chorde/clients/memcached.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.3/lib/chorde/clients/tiered.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/clients/tiered.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.3/lib/chorde/decorators.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.3/lib/chorde/decorators.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/decorators.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/dnsutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/external_integration.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-04-21 13:38:18.450059 chorde-1.0.3/lib/chorde/mq/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.3/lib/chorde/mq/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/mq/coherence.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.3/lib/chorde/mq/compat.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-04-21 13:38:18.450059 chorde-1.0.3/lib/chorde/mq/ipsub/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.3/lib/chorde/mq/ipsub/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/mq/ipsub/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/mq/ipsub/ipsub_zmq.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4920 2023-04-21 13:34:45.000000 chorde-1.0.3/lib/chorde/sPickle.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.3/lib/chorde/serialize.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/shmemutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/threadpool.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.3/lib/chorde/worker.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-04-21 13:38:18.430059 chorde-1.0.3/lib/chorde.egg-info/
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-04-21 13:38:18.000000 chorde-1.0.3/lib/chorde.egg-info/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-04-21 13:38:18.000000 chorde-1.0.3/lib/chorde.egg-info/SOURCES.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-04-21 13:38:18.000000 chorde-1.0.3/lib/chorde.egg-info/dependency_links.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.3/lib/chorde.egg-info/not-zip-safe
--rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-04-21 13:38:18.000000 chorde-1.0.3/lib/chorde.egg-info/requires.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-04-21 13:38:18.000000 chorde-1.0.3/lib/chorde.egg-info/top_level.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-03-03 18:03:18.000000 chorde-1.0.3/requirements.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-04-21 13:38:18.450059 chorde-1.0.3/setup.cfg
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-04-21 13:36:23.000000 chorde-1.0.3/setup.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.548640 chorde-1.0.4/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     8084 2023-05-15 17:02:17.000000 chorde-1.0.4/CHANGELOG
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.4/MANIFEST.in
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-05-15 17:04:26.548640 chorde-1.0.4/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.4/README.rst
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.532639 chorde-1.0.4/lib/
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.536640 chorde-1.0.4/lib/chorde/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-05-15 17:04:06.000000 chorde-1.0.4/lib/chorde/_version.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.548640 chorde-1.0.4/lib/chorde/clients/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   663617 2023-05-15 17:02:59.000000 chorde-1.0.4/lib/chorde/clients/_async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      333 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/clients/_async.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    15767 2023-05-15 17:00:02.000000 chorde-1.0.4/lib/chorde/clients/_async.pyx
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.4/lib/chorde/clients/async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2731676 2023-04-17 14:22:41.000000 chorde-1.0.4/lib/chorde/clients/asyncache.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    65380 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/asyncache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.4/lib/chorde/clients/base.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/coherent.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/elasticache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/files.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.4/lib/chorde/clients/inproc.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/inproc.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.4/lib/chorde/clients/memcached.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.4/lib/chorde/clients/tiered.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/clients/tiered.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.4/lib/chorde/decorators.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.4/lib/chorde/decorators.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/decorators.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/dnsutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/external_integration.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.548640 chorde-1.0.4/lib/chorde/mq/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/mq/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/mq/coherence.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/mq/compat.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.548640 chorde-1.0.4/lib/chorde/mq/ipsub/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.4/lib/chorde/mq/ipsub/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/mq/ipsub/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/mq/ipsub/ipsub_zmq.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4920 2023-04-21 13:34:45.000000 chorde-1.0.4/lib/chorde/sPickle.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.4/lib/chorde/serialize.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/shmemutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/threadpool.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.4/lib/chorde/worker.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-05-15 17:04:26.540639 chorde-1.0.4/lib/chorde.egg-info/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/SOURCES.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/dependency_links.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.4/lib/chorde.egg-info/not-zip-safe
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/requires.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-05-15 17:04:26.000000 chorde-1.0.4/lib/chorde.egg-info/top_level.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-05-15 15:39:00.000000 chorde-1.0.4/requirements.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-05-15 17:04:26.548640 chorde-1.0.4/setup.cfg
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-05-15 17:03:37.000000 chorde-1.0.4/setup.py
```

### Comparing `chorde-1.0.3/CHANGELOG` & `chorde-1.0.4/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Change Log
 
 All notable changes to this project will be documented here.
 
+## [1.0.4] - 2023-05-15
+### Bugfixes
+- Fix empty reason field when re-raising tornado.web.HTTPError
+
 ## [1.0.3] - 2023-04-21
 ### Bugfixes
 - Various string encoding fixes
 
 ## [1.0.0] - 2023-03-02
 ### Removed
 - Dropped Python 2.x support
```

### Comparing `chorde-1.0.3/PKG-INFO` & `chorde-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.3
+Version: 1.0.4
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.3/README.rst` & `chorde-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/__init__.py` & `chorde-1.0.4/lib/chorde/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/_async.c` & `chorde-1.0.4/lib/chorde/clients/_async.c`

 * *Files 4% similar despite different names*

```diff
@@ -964,16 +964,16 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "stringsource",
   "lib/chorde/clients/_async.pyx",
+  "stringsource",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6chorde_7clients_6_async_Future;
 struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper;
 struct __pyx_obj_6chorde_7clients_6_async_WeakCallback;
 struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback;
@@ -981,15 +981,15 @@
 struct __pyx_obj_6chorde_7clients_6_async_MissCallback;
 struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback;
 struct __pyx_obj_6chorde_7clients_6_async_AnyCallback;
 struct __pyx_obj_6chorde_7clients_6_async_DoneCallback;
 struct __pyx_obj_6chorde_7clients_6_async_NONE;
 struct __pyx_opt_args_6chorde_7clients_6_async_16ExceptionWrapper_reraise;
 
-/* "chorde/clients/_async.pyx":43
+/* "chorde/clients/_async.pyx":50
  * 
  *     @cython.ccall
  *     def reraise(self, bint strip=True):             # <<<<<<<<<<<<<<
  *         exc = self.value
  *         if strip:
  */
 struct __pyx_opt_args_6chorde_7clients_6_async_16ExceptionWrapper_reraise {
@@ -1012,101 +1012,101 @@
   PyObject *__weakref__;
   int _running;
   int _cancel_pending;
   int _cancelled;
 };
 
 
-/* "chorde/clients/_async.pyx":35
+/* "chorde/clients/_async.pyx":42
  * 
  * @cython.freelist(100)
  * cdef class ExceptionWrapper:             # <<<<<<<<<<<<<<
  *     cdef public object value
  *     cdef object __weakref__
  */
 struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper {
   PyObject_HEAD
   struct __pyx_vtabstruct_6chorde_7clients_6_async_ExceptionWrapper *__pyx_vtab;
   PyObject *value;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":71
+/* "chorde/clients/_async.pyx":83
  * 
  * @cython.freelist(100)
  * cdef class WeakCallback:             # <<<<<<<<<<<<<<
  *     cdef object me, callback, __weakref__
  * 
  */
 struct __pyx_obj_6chorde_7clients_6_async_WeakCallback {
   PyObject_HEAD
   PyObject *me;
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":85
+/* "chorde/clients/_async.pyx":97
  * 
  * @cython.freelist(100)
  * cdef class DeferExceptionCallback:             # <<<<<<<<<<<<<<
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):
  */
 struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback {
   PyObject_HEAD
   PyObject *defer;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":93
+/* "chorde/clients/_async.pyx":105
  * 
  * @cython.freelist(100)
  * cdef class ValueCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_ValueCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":102
+/* "chorde/clients/_async.pyx":114
  * 
  * @cython.freelist(100)
  * cdef class MissCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_MissCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":111
+/* "chorde/clients/_async.pyx":123
  * 
  * @cython.freelist(100)
  * cdef class ExceptionCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":120
+/* "chorde/clients/_async.pyx":132
  * 
  * @cython.freelist(100)
  * cdef class AnyCallback:             # <<<<<<<<<<<<<<
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):
  */
 struct __pyx_obj_6chorde_7clients_6_async_AnyCallback {
@@ -1114,42 +1114,42 @@
   PyObject *on_value;
   PyObject *on_miss;
   PyObject *on_exc;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":138
+/* "chorde/clients/_async.pyx":150
  * 
  * @cython.freelist(100)
  * cdef class DoneCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_DoneCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":145
+/* "chorde/clients/_async.pyx":157
  *         return self.callback()
  * 
  * cdef class NONE:             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 struct __pyx_obj_6chorde_7clients_6_async_NONE {
   PyObject_HEAD
 };
 
 
 
-/* "chorde/clients/_async.pyx":149
+/* "chorde/clients/_async.pyx":161
  * 
  * @cython.freelist(100)
  * cdef class Future:             # <<<<<<<<<<<<<<
  *     def __cinit__(self, logger = None):
  *         self._cb = None
  */
 
@@ -1159,15 +1159,15 @@
   PyObject *(*_set_nothreads)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*set)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*_on_stuff)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *__pyx_vtabptr_6chorde_7clients_6_async_Future;
 
 
-/* "chorde/clients/_async.pyx":35
+/* "chorde/clients/_async.pyx":42
  * 
  * @cython.freelist(100)
  * cdef class ExceptionWrapper:             # <<<<<<<<<<<<<<
  *     cdef public object value
  *     cdef object __weakref__
  */
 
@@ -1645,20 +1645,22 @@
 static PyTypeObject *__pyx_ptype_6chorde_7clients_6_async_NONE = 0;
 static PyObject *__pyx_v_6chorde_7clients_6_async_CacheMissError = 0;
 static PyObject *__pyx_v_6chorde_7clients_6_async_CancelledError = 0;
 static PyObject *__pyx_v_6chorde_7clients_6_async_TimeoutError = 0;
 static PyObject *__pyx_v_6chorde_7clients_6_async_wref = 0;
 static PyObject *__pyx_v_6chorde_7clients_6_async_functools_partial = 0;
 static int __pyx_v_6chorde_7clients_6_async_strip_tracebacks;
+static PyObject *__pyx_v_6chorde_7clients_6_async__HTTPError = 0;
 static PyObject *__pyx_f_6chorde_7clients_6_async___pyx_unpickle_NONE__set_state(struct __pyx_obj_6chorde_7clients_6_async_NONE *, PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "chorde.clients._async"
 extern int __pyx_module_is_main_chorde__clients___async;
 int __pyx_module_is_main_chorde__clients___async = 0;
 
 /* Implementation of 'chorde.clients._async' */
+static PyObject *__pyx_builtin_ImportError;
 static PyObject *__pyx_builtin_TypeError;
 static const char __pyx_k_me[] = "me";
 static const char __pyx_k_exc[] = "exc";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_ref[] = "ref";
 static const char __pyx_k_set[] = "set";
 static const char __pyx_k_NONE[] = "NONE";
@@ -1676,14 +1678,15 @@
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_Future[] = "Future";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_logger[] = "logger";
 static const char __pyx_k_on_any[] = "on_any";
 static const char __pyx_k_on_exc[] = "on_exc";
 static const char __pyx_k_pickle[] = "pickle";
+static const char __pyx_k_reason[] = "reason";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_logging[] = "logging";
 static const char __pyx_k_on_miss[] = "on_miss";
 static const char __pyx_k_partial[] = "partial";
 static const char __pyx_k_reraise[] = "reraise";
 static const char __pyx_k_timeout[] = "timeout";
@@ -1691,26 +1694,29 @@
 static const char __pyx_k_callback[] = "callback";
 static const char __pyx_k_exc_info[] = "exc_info";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_on_stuff[] = "_on_stuff";
 static const char __pyx_k_on_value[] = "on_value";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_HTTPError[] = "HTTPError";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_functools[] = "functools";
 static const char __pyx_k_norecurse[] = "norecurse";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_threading[] = "threading";
 static const char __pyx_k_traceback[] = "__traceback__";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_set_result[] = "set_result";
 static const char __pyx_k_AnyCallback[] = "AnyCallback";
+static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_PickleError[] = "PickleError";
+static const char __pyx_k_tornado_web[] = "tornado.web";
 static const char __pyx_k_DoneCallback[] = "DoneCallback";
 static const char __pyx_k_MissCallback[] = "MissCallback";
 static const char __pyx_k_TimeoutError[] = "TimeoutError";
 static const char __pyx_k_WeakCallback[] = "WeakCallback";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_ValueCallback[] = "ValueCallback";
@@ -1740,14 +1746,16 @@
 static PyObject *__pyx_n_s_DeferExceptionCallback;
 static PyObject *__pyx_n_s_DoneCallback;
 static PyObject *__pyx_kp_s_Error_in_async_callback;
 static PyObject *__pyx_n_s_Event;
 static PyObject *__pyx_n_s_ExceptionCallback;
 static PyObject *__pyx_n_s_ExceptionWrapper;
 static PyObject *__pyx_n_s_Future;
+static PyObject *__pyx_n_s_HTTPError;
+static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_MissCallback;
 static PyObject *__pyx_n_s_NONE;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_TimeoutError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_ValueCallback;
@@ -1785,14 +1793,15 @@
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_NONE;
 static PyObject *__pyx_n_s_pyx_vtable;
+static PyObject *__pyx_n_s_reason;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_ref;
 static PyObject *__pyx_n_s_reraise;
 static PyObject *__pyx_n_s_set;
 static PyObject *__pyx_n_s_set_exception;
@@ -1802,14 +1811,15 @@
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_strip;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_threading;
 static PyObject *__pyx_n_s_timeout;
+static PyObject *__pyx_n_s_tornado_web;
 static PyObject *__pyx_n_s_traceback;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_wait;
 static PyObject *__pyx_n_s_weakref;
 static PyObject *__pyx_n_s_with_traceback;
 static PyObject *__pyx_pf_6chorde_7clients_6_async_set_strip_tracebacks(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_strip); /* proto */
@@ -1916,15 +1926,15 @@
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_codeobj__22;
 static PyObject *__pyx_codeobj__24;
 /* Late includes */
 
-/* "chorde/clients/_async.pyx":22
+/* "chorde/clients/_async.pyx":29
  * 
  * 
  * def set_strip_tracebacks(bint strip):             # <<<<<<<<<<<<<<
  *     """ Sets traceback stripping behavior for async futures
  * 
  */
 
@@ -1937,15 +1947,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_strip_tracebacks (wrapper)", 0);
   assert(__pyx_arg_strip); {
-    __pyx_v_strip = __Pyx_PyObject_IsTrue(__pyx_arg_strip); if (unlikely((__pyx_v_strip == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 22, __pyx_L3_error)
+    __pyx_v_strip = __Pyx_PyObject_IsTrue(__pyx_arg_strip); if (unlikely((__pyx_v_strip == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.set_strip_tracebacks", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -1957,39 +1967,39 @@
 }
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_set_strip_tracebacks(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_strip) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_strip_tracebacks", 0);
 
-  /* "chorde/clients/_async.pyx":31
+  /* "chorde/clients/_async.pyx":38
  *     """
  *     global strip_tracebacks
  *     strip_tracebacks = strip             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_6chorde_7clients_6_async_strip_tracebacks = __pyx_v_strip;
 
-  /* "chorde/clients/_async.pyx":22
+  /* "chorde/clients/_async.pyx":29
  * 
  * 
  * def set_strip_tracebacks(bint strip):             # <<<<<<<<<<<<<<
  *     """ Sets traceback stripping behavior for async futures
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":39
+/* "chorde/clients/_async.pyx":46
  *     cdef object __weakref__
  * 
  *     def __cinit__(self, value):             # <<<<<<<<<<<<<<
  *         self.value = value
  * 
  */
 
@@ -2018,26 +2028,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 39, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 39, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionWrapper.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_16ExceptionWrapper___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_self), __pyx_v_value);
 
@@ -2047,56 +2057,57 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_16ExceptionWrapper___cinit__(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":40
+  /* "chorde/clients/_async.pyx":47
  * 
  *     def __cinit__(self, value):
  *         self.value = value             # <<<<<<<<<<<<<<
  * 
  *     @cython.ccall
  */
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   __Pyx_GOTREF(__pyx_v_self->value);
   __Pyx_DECREF(__pyx_v_self->value);
   __pyx_v_self->value = __pyx_v_value;
 
-  /* "chorde/clients/_async.pyx":39
+  /* "chorde/clients/_async.pyx":46
  *     cdef object __weakref__
  * 
  *     def __cinit__(self, value):             # <<<<<<<<<<<<<<
  *         self.value = value
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":43
+/* "chorde/clients/_async.pyx":50
  * 
  *     @cython.ccall
  *     def reraise(self, bint strip=True):             # <<<<<<<<<<<<<<
  *         exc = self.value
  *         if strip:
  */
 
 static PyObject *__pyx_pw_6chorde_7clients_6_async_16ExceptionWrapper_3reraise(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_6chorde_7clients_6_async_16ExceptionWrapper_reraise(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *__pyx_v_self, int __pyx_skip_dispatch, struct __pyx_opt_args_6chorde_7clients_6_async_16ExceptionWrapper_reraise *__pyx_optional_args) {
   int __pyx_v_strip = ((int)1);
   PyObject *__pyx_v_exc = NULL;
   PyObject *__pyx_v_exc_typ = NULL;
   PyObject *__pyx_v_exc_obj = NULL;
   PyObject *__pyx_v_exc_tb = NULL;
+  PyObject *__pyx_v_kwargs = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -2127,19 +2138,19 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reraise); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 43, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reraise); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_16ExceptionWrapper_3reraise)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 43, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -2147,15 +2158,15 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 43, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -2168,77 +2179,77 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":44
+  /* "chorde/clients/_async.pyx":51
  *     @cython.ccall
  *     def reraise(self, bint strip=True):
  *         exc = self.value             # <<<<<<<<<<<<<<
  *         if strip:
  *             del self.value
  */
   __pyx_t_1 = __pyx_v_self->value;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_exc = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":45
+  /* "chorde/clients/_async.pyx":52
  *     def reraise(self, bint strip=True):
  *         exc = self.value
  *         if strip:             # <<<<<<<<<<<<<<
  *             del self.value
  *         try:
  */
   __pyx_t_6 = (__pyx_v_strip != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":46
+    /* "chorde/clients/_async.pyx":53
  *         exc = self.value
  *         if strip:
  *             del self.value             # <<<<<<<<<<<<<<
  *         try:
  *             exc_typ, exc_obj, exc_tb = exc
  */
-    if (__Pyx_PyObject_DelAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_value) < 0) __PYX_ERR(1, 46, __pyx_L1_error)
+    if (__Pyx_PyObject_DelAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_value) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":45
+    /* "chorde/clients/_async.pyx":52
  *     def reraise(self, bint strip=True):
  *         exc = self.value
  *         if strip:             # <<<<<<<<<<<<<<
  *             del self.value
  *         try:
  */
   }
 
-  /* "chorde/clients/_async.pyx":47
+  /* "chorde/clients/_async.pyx":54
  *         if strip:
  *             del self.value
  *         try:             # <<<<<<<<<<<<<<
  *             exc_typ, exc_obj, exc_tb = exc
  *         finally:
  */
   /*try:*/ {
 
-    /* "chorde/clients/_async.pyx":48
+    /* "chorde/clients/_async.pyx":55
  *             del self.value
  *         try:
  *             exc_typ, exc_obj, exc_tb = exc             # <<<<<<<<<<<<<<
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  */
     if ((likely(PyTuple_CheckExact(__pyx_v_exc))) || (PyList_CheckExact(__pyx_v_exc))) {
       PyObject* sequence = __pyx_v_exc;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 3)) {
         if (size > 3) __Pyx_RaiseTooManyValuesError(3);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(1, 48, __pyx_L5_error)
+        __PYX_ERR(0, 55, __pyx_L5_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
       } else {
@@ -2246,52 +2257,52 @@
         __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
         __pyx_t_4 = PyList_GET_ITEM(sequence, 2); 
       }
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       #else
-      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 48, __pyx_L5_error)
+      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 48, __pyx_L5_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 48, __pyx_L5_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 55, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_3 = PyObject_GetIter(__pyx_v_exc); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 48, __pyx_L5_error)
+      __pyx_t_3 = PyObject_GetIter(__pyx_v_exc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext;
       index = 0; __pyx_t_1 = __pyx_t_7(__pyx_t_3); if (unlikely(!__pyx_t_1)) goto __pyx_L7_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_1);
       index = 1; __pyx_t_2 = __pyx_t_7(__pyx_t_3); if (unlikely(!__pyx_t_2)) goto __pyx_L7_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_2);
       index = 2; __pyx_t_4 = __pyx_t_7(__pyx_t_3); if (unlikely(!__pyx_t_4)) goto __pyx_L7_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_3), 3) < 0) __PYX_ERR(1, 48, __pyx_L5_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_3), 3) < 0) __PYX_ERR(0, 55, __pyx_L5_error)
       __pyx_t_7 = NULL;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       goto __pyx_L8_unpacking_done;
       __pyx_L7_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_7 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(1, 48, __pyx_L5_error)
+      __PYX_ERR(0, 55, __pyx_L5_error)
       __pyx_L8_unpacking_done:;
     }
     __pyx_v_exc_typ = __pyx_t_1;
     __pyx_t_1 = 0;
     __pyx_v_exc_obj = __pyx_t_2;
     __pyx_t_2 = 0;
     __pyx_v_exc_tb = __pyx_t_4;
     __pyx_t_4 = 0;
   }
 
-  /* "chorde/clients/_async.pyx":51
+  /* "chorde/clients/_async.pyx":58
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  *             del exc             # <<<<<<<<<<<<<<
  *         try:
  *             if not strip:
  */
   /*finally:*/ {
@@ -2336,269 +2347,319 @@
       __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0;
       __pyx_lineno = __pyx_t_8; __pyx_clineno = __pyx_t_9; __pyx_filename = __pyx_t_10;
       goto __pyx_L1_error;
     }
     __pyx_L6:;
   }
 
-  /* "chorde/clients/_async.pyx":52
+  /* "chorde/clients/_async.pyx":59
  *             # Don't leave references to the exc/tb in the frame
  *             del exc
  *         try:             # <<<<<<<<<<<<<<
  *             if not strip:
- *                 raise exc_typ(*exc_obj.args) from exc_obj
+ *                 kwargs = {}
  */
   /*try:*/ {
 
-    /* "chorde/clients/_async.pyx":53
+    /* "chorde/clients/_async.pyx":60
  *             del exc
  *         try:
  *             if not strip:             # <<<<<<<<<<<<<<
- *                 raise exc_typ(*exc_obj.args) from exc_obj
- *             elif exc_tb is not None:
+ *                 kwargs = {}
+ *                 if isinstance(exc_obj, _HTTPError):
  */
     __pyx_t_6 = ((!(__pyx_v_strip != 0)) != 0);
-    if (unlikely(__pyx_t_6)) {
+    if (__pyx_t_6) {
 
-      /* "chorde/clients/_async.pyx":54
+      /* "chorde/clients/_async.pyx":61
  *         try:
  *             if not strip:
- *                 raise exc_typ(*exc_obj.args) from exc_obj             # <<<<<<<<<<<<<<
+ *                 kwargs = {}             # <<<<<<<<<<<<<<
+ *                 if isinstance(exc_obj, _HTTPError):
+ *                     # Workaround for tornado's HTTPError which does not function
+ */
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L12_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_v_kwargs = ((PyObject*)__pyx_t_4);
+      __pyx_t_4 = 0;
+
+      /* "chorde/clients/_async.pyx":62
+ *             if not strip:
+ *                 kwargs = {}
+ *                 if isinstance(exc_obj, _HTTPError):             # <<<<<<<<<<<<<<
+ *                     # Workaround for tornado's HTTPError which does not function
+ *                     # correctly without a reason, and reason is given only as kwarg
+ */
+      __pyx_t_4 = __pyx_v_6chorde_7clients_6_async__HTTPError;
+      __Pyx_INCREF(__pyx_t_4);
+      __pyx_t_6 = PyObject_IsInstance(__pyx_v_exc_obj, __pyx_t_4); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 62, __pyx_L12_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_17 = (__pyx_t_6 != 0);
+      if (__pyx_t_17) {
+
+        /* "chorde/clients/_async.pyx":65
+ *                     # Workaround for tornado's HTTPError which does not function
+ *                     # correctly without a reason, and reason is given only as kwarg
+ *                     kwargs["reason"] = exc_obj.reason             # <<<<<<<<<<<<<<
+ *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
+ *             elif exc_tb is not None:
+ */
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_reason); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L12_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        if (unlikely(PyDict_SetItem(__pyx_v_kwargs, __pyx_n_s_reason, __pyx_t_4) < 0)) __PYX_ERR(0, 65, __pyx_L12_error)
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+        /* "chorde/clients/_async.pyx":62
+ *             if not strip:
+ *                 kwargs = {}
+ *                 if isinstance(exc_obj, _HTTPError):             # <<<<<<<<<<<<<<
+ *                     # Workaround for tornado's HTTPError which does not function
+ *                     # correctly without a reason, and reason is given only as kwarg
+ */
+      }
+
+      /* "chorde/clients/_async.pyx":66
+ *                     # correctly without a reason, and reason is given only as kwarg
+ *                     kwargs["reason"] = exc_obj.reason
+ *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj             # <<<<<<<<<<<<<<
  *             elif exc_tb is not None:
  *                 if exc_obj is not None:
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_args); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 54, __pyx_L12_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_args); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 54, __pyx_L12_error)
+      __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_v_exc_typ, __pyx_t_2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 54, __pyx_L12_error)
+      __pyx_t_4 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_v_exc_typ, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L12_error)
+      __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_Raise(__pyx_t_4, 0, 0, __pyx_v_exc_obj);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(1, 54, __pyx_L12_error)
+      __Pyx_Raise(__pyx_t_1, 0, 0, __pyx_v_exc_obj);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __PYX_ERR(0, 66, __pyx_L12_error)
 
-      /* "chorde/clients/_async.pyx":53
+      /* "chorde/clients/_async.pyx":60
  *             del exc
  *         try:
  *             if not strip:             # <<<<<<<<<<<<<<
- *                 raise exc_typ(*exc_obj.args) from exc_obj
- *             elif exc_tb is not None:
+ *                 kwargs = {}
+ *                 if isinstance(exc_obj, _HTTPError):
  */
     }
 
-    /* "chorde/clients/_async.pyx":55
- *             if not strip:
- *                 raise exc_typ(*exc_obj.args) from exc_obj
+    /* "chorde/clients/_async.pyx":67
+ *                     kwargs["reason"] = exc_obj.reason
+ *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:             # <<<<<<<<<<<<<<
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  */
-    __pyx_t_6 = (__pyx_v_exc_tb != Py_None);
-    __pyx_t_17 = (__pyx_t_6 != 0);
-    if (__pyx_t_17) {
+    __pyx_t_17 = (__pyx_v_exc_tb != Py_None);
+    __pyx_t_6 = (__pyx_t_17 != 0);
+    if (__pyx_t_6) {
 
-      /* "chorde/clients/_async.pyx":56
- *                 raise exc_typ(*exc_obj.args) from exc_obj
+      /* "chorde/clients/_async.pyx":68
+ *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:
  *                 if exc_obj is not None:             # <<<<<<<<<<<<<<
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  */
-      __pyx_t_17 = (__pyx_v_exc_obj != Py_None);
-      __pyx_t_6 = (__pyx_t_17 != 0);
-      if (likely(__pyx_t_6)) {
+      __pyx_t_6 = (__pyx_v_exc_obj != Py_None);
+      __pyx_t_17 = (__pyx_t_6 != 0);
+      if (likely(__pyx_t_17)) {
 
-        /* "chorde/clients/_async.pyx":57
+        /* "chorde/clients/_async.pyx":69
  *             elif exc_tb is not None:
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:             # <<<<<<<<<<<<<<
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj
  */
-        __pyx_t_4 = __Pyx_GetAttr(__pyx_v_exc_obj, __pyx_n_s_traceback); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 57, __pyx_L12_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_6 = (__pyx_t_4 != __pyx_v_exc_tb);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_17 = (__pyx_t_6 != 0);
-        if (__pyx_t_17) {
+        __pyx_t_1 = __Pyx_GetAttr(__pyx_v_exc_obj, __pyx_n_s_traceback); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L12_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_17 = (__pyx_t_1 != __pyx_v_exc_tb);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_6 = (__pyx_t_17 != 0);
+        if (__pyx_t_6) {
 
-          /* "chorde/clients/_async.pyx":58
+          /* "chorde/clients/_async.pyx":70
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)             # <<<<<<<<<<<<<<
  *                     raise exc_obj
  *                 else:
  */
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 58, __pyx_L12_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_1 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-            __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
-            if (likely(__pyx_t_1)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-              __Pyx_INCREF(__pyx_t_1);
+          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L12_error)
+          __Pyx_GOTREF(__pyx_t_4);
+          __pyx_t_2 = NULL;
+          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+            __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
+            if (likely(__pyx_t_2)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+              __Pyx_INCREF(__pyx_t_2);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_2, function);
+              __Pyx_DECREF_SET(__pyx_t_4, function);
             }
           }
-          __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_exc_tb);
-          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 58, __pyx_L12_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __Pyx_DECREF_SET(__pyx_v_exc_obj, __pyx_t_4);
-          __pyx_t_4 = 0;
+          __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_exc_tb);
+          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L12_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+          __Pyx_DECREF_SET(__pyx_v_exc_obj, __pyx_t_1);
+          __pyx_t_1 = 0;
 
-          /* "chorde/clients/_async.pyx":57
+          /* "chorde/clients/_async.pyx":69
  *             elif exc_tb is not None:
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:             # <<<<<<<<<<<<<<
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj
  */
         }
 
-        /* "chorde/clients/_async.pyx":59
+        /* "chorde/clients/_async.pyx":71
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  */
         __Pyx_Raise(__pyx_v_exc_obj, 0, 0, 0);
-        __PYX_ERR(1, 59, __pyx_L12_error)
+        __PYX_ERR(0, 71, __pyx_L12_error)
 
-        /* "chorde/clients/_async.pyx":56
- *                 raise exc_typ(*exc_obj.args) from exc_obj
+        /* "chorde/clients/_async.pyx":68
+ *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:
  *                 if exc_obj is not None:             # <<<<<<<<<<<<<<
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  */
       }
 
-      /* "chorde/clients/_async.pyx":61
+      /* "chorde/clients/_async.pyx":73
  *                     raise exc_obj
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)             # <<<<<<<<<<<<<<
  *             elif exc_obj is not None:
  *                 raise exc_obj
  */
       /*else*/ {
         __Pyx_INCREF(__pyx_v_exc_typ);
-        __pyx_t_1 = __pyx_v_exc_typ; __pyx_t_3 = NULL;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+        __pyx_t_2 = __pyx_v_exc_typ; __pyx_t_3 = NULL;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_3)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_1, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
-        __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+        __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 61, __pyx_L12_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 61, __pyx_L12_error)
-        __Pyx_GOTREF(__pyx_t_1);
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L12_error)
+        __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-          if (likely(__pyx_t_2)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-            __Pyx_INCREF(__pyx_t_2);
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L12_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __pyx_t_4 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+          if (likely(__pyx_t_4)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+            __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_1, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
-        __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_exc_tb);
-        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 61, __pyx_L12_error)
-        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_exc_tb);
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L12_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 61, __pyx_L12_error)
+        __PYX_ERR(0, 73, __pyx_L12_error)
       }
 
-      /* "chorde/clients/_async.pyx":55
- *             if not strip:
- *                 raise exc_typ(*exc_obj.args) from exc_obj
+      /* "chorde/clients/_async.pyx":67
+ *                     kwargs["reason"] = exc_obj.reason
+ *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:             # <<<<<<<<<<<<<<
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  */
     }
 
-    /* "chorde/clients/_async.pyx":62
+    /* "chorde/clients/_async.pyx":74
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:             # <<<<<<<<<<<<<<
  *                 raise exc_obj
  *             else:
  */
-    __pyx_t_17 = (__pyx_v_exc_obj != Py_None);
-    __pyx_t_6 = (__pyx_t_17 != 0);
-    if (unlikely(__pyx_t_6)) {
+    __pyx_t_6 = (__pyx_v_exc_obj != Py_None);
+    __pyx_t_17 = (__pyx_t_6 != 0);
+    if (unlikely(__pyx_t_17)) {
 
-      /* "chorde/clients/_async.pyx":63
+      /* "chorde/clients/_async.pyx":75
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:
  *                 raise exc_obj             # <<<<<<<<<<<<<<
  *             else:
  *                 raise exc_typ()
  */
       __Pyx_Raise(__pyx_v_exc_obj, 0, 0, 0);
-      __PYX_ERR(1, 63, __pyx_L12_error)
+      __PYX_ERR(0, 75, __pyx_L12_error)
 
-      /* "chorde/clients/_async.pyx":62
+      /* "chorde/clients/_async.pyx":74
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:             # <<<<<<<<<<<<<<
  *                 raise exc_obj
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":65
+    /* "chorde/clients/_async.pyx":77
  *                 raise exc_obj
  *             else:
  *                 raise exc_typ()             # <<<<<<<<<<<<<<
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  */
     /*else*/ {
       __Pyx_INCREF(__pyx_v_exc_typ);
-      __pyx_t_1 = __pyx_v_exc_typ; __pyx_t_2 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-        if (likely(__pyx_t_2)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-          __Pyx_INCREF(__pyx_t_2);
+      __pyx_t_2 = __pyx_v_exc_typ; __pyx_t_4 = NULL;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_1, function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
-      __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 65, __pyx_L12_error)
-      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L12_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(1, 65, __pyx_L12_error)
+      __PYX_ERR(0, 77, __pyx_L12_error)
     }
   }
 
-  /* "chorde/clients/_async.pyx":68
+  /* "chorde/clients/_async.pyx":80
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  *             del exc_typ, exc_obj, exc_tb             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
   /*finally:*/ {
@@ -2641,15 +2702,15 @@
       __Pyx_ErrRestore(__pyx_t_16, __pyx_t_15, __pyx_t_14);
       __pyx_t_16 = 0; __pyx_t_15 = 0; __pyx_t_14 = 0; __pyx_t_13 = 0; __pyx_t_12 = 0; __pyx_t_11 = 0;
       __pyx_lineno = __pyx_t_9; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_18;
       goto __pyx_L1_error;
     }
   }
 
-  /* "chorde/clients/_async.pyx":43
+  /* "chorde/clients/_async.pyx":50
  * 
  *     @cython.ccall
  *     def reraise(self, bint strip=True):             # <<<<<<<<<<<<<<
  *         exc = self.value
  *         if strip:
  */
 
@@ -2663,14 +2724,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ExceptionWrapper.reraise", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_exc);
   __Pyx_XDECREF(__pyx_v_exc_typ);
   __Pyx_XDECREF(__pyx_v_exc_obj);
   __Pyx_XDECREF(__pyx_v_exc_tb);
+  __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6chorde_7clients_6_async_16ExceptionWrapper_3reraise(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -2699,33 +2761,33 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_strip);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "reraise") < 0)) __PYX_ERR(1, 43, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "reraise") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_strip = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_strip == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 43, __pyx_L3_error)
+      __pyx_v_strip = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_strip == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L3_error)
     } else {
       __pyx_v_strip = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("reraise", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 43, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("reraise", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 50, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionWrapper.reraise", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_16ExceptionWrapper_2reraise(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_self), __pyx_v_strip);
 
@@ -2742,15 +2804,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reraise", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.strip = __pyx_v_strip;
-  __pyx_t_1 = __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper->reraise(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 43, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper->reraise(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2759,15 +2821,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":36
+/* "chorde/clients/_async.pyx":43
  * @cython.freelist(100)
  * cdef class ExceptionWrapper:
  *     cdef public object value             # <<<<<<<<<<<<<<
  *     cdef object __weakref__
  * 
  */
 
@@ -2888,19 +2950,19 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 2, __pyx_L1_error)
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -2944,19 +3006,19 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 4, __pyx_L1_error)
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -2967,15 +3029,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ExceptionWrapper.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":74
+/* "chorde/clients/_async.pyx":86
  *     cdef object me, callback, __weakref__
  * 
  *     def __cinit__(self, me, callback):             # <<<<<<<<<<<<<<
  *         self.me = wref(me)
  *         self.callback = callback
  */
 
@@ -3009,32 +3071,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_me)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(1, 74, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 86, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 74, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 86, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_me = values[0];
     __pyx_v_callback = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 74, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 86, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12WeakCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_WeakCallback *)__pyx_v_self), __pyx_v_me, __pyx_v_callback);
 
@@ -3050,15 +3112,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":75
+  /* "chorde/clients/_async.pyx":87
  * 
  *     def __cinit__(self, me, callback):
  *         self.me = wref(me)             # <<<<<<<<<<<<<<
  *         self.callback = callback
  * 
  */
   __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_wref);
@@ -3070,37 +3132,37 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_me) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_me);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 75, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->me);
   __Pyx_DECREF(__pyx_v_self->me);
   __pyx_v_self->me = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":76
+  /* "chorde/clients/_async.pyx":88
  *     def __cinit__(self, me, callback):
  *         self.me = wref(me)
  *         self.callback = callback             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self, value):
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":74
+  /* "chorde/clients/_async.pyx":86
  *     cdef object me, callback, __weakref__
  * 
  *     def __cinit__(self, me, callback):             # <<<<<<<<<<<<<<
  *         self.me = wref(me)
  *         self.callback = callback
  */
 
@@ -3114,15 +3176,15 @@
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":78
+/* "chorde/clients/_async.pyx":90
  *         self.callback = callback
  * 
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         cdef object me
  *         me = self.me()
  */
 
@@ -3151,26 +3213,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(1, 78, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 78, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 90, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12WeakCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_WeakCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -3189,15 +3251,15 @@
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":80
+  /* "chorde/clients/_async.pyx":92
  *     def __call__(self, value):
  *         cdef object me
  *         me = self.me()             # <<<<<<<<<<<<<<
  *         if me is not None:
  *             return self.callback(me)
  */
   __Pyx_INCREF(__pyx_v_self->me);
@@ -3209,32 +3271,32 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 80, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_me = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":81
+  /* "chorde/clients/_async.pyx":93
  *         cdef object me
  *         me = self.me()
  *         if me is not None:             # <<<<<<<<<<<<<<
  *             return self.callback(me)
  * 
  */
   __pyx_t_4 = (__pyx_v_me != Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "chorde/clients/_async.pyx":82
+    /* "chorde/clients/_async.pyx":94
  *         me = self.me()
  *         if me is not None:
  *             return self.callback(me)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -3247,31 +3309,31 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_me) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_me);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 82, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":81
+    /* "chorde/clients/_async.pyx":93
  *         cdef object me
  *         me = self.me()
  *         if me is not None:             # <<<<<<<<<<<<<<
  *             return self.callback(me)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":78
+  /* "chorde/clients/_async.pyx":90
  *         self.callback = callback
  * 
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         cdef object me
  *         me = self.me()
  */
 
@@ -3321,19 +3383,19 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 2, __pyx_L1_error)
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -3377,19 +3439,19 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 4, __pyx_L1_error)
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -3400,15 +3462,15 @@
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":87
+/* "chorde/clients/_async.pyx":99
  * cdef class DeferExceptionCallback:
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):             # <<<<<<<<<<<<<<
  *         self.defer = defer
  *     def __call__(self, value):
  */
 
@@ -3437,26 +3499,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_defer)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 87, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 99, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_defer = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 87, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 99, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DeferExceptionCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_22DeferExceptionCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback *)__pyx_v_self), __pyx_v_defer);
 
@@ -3466,42 +3528,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_22DeferExceptionCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback *__pyx_v_self, PyObject *__pyx_v_defer) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":88
+  /* "chorde/clients/_async.pyx":100
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):
  *         self.defer = defer             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         self.defer.set_exception(value[1] or value[0])
  */
   __Pyx_INCREF(__pyx_v_defer);
   __Pyx_GIVEREF(__pyx_v_defer);
   __Pyx_GOTREF(__pyx_v_self->defer);
   __Pyx_DECREF(__pyx_v_self->defer);
   __pyx_v_self->defer = __pyx_v_defer;
 
-  /* "chorde/clients/_async.pyx":87
+  /* "chorde/clients/_async.pyx":99
  * cdef class DeferExceptionCallback:
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):             # <<<<<<<<<<<<<<
  *         self.defer = defer
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":89
+/* "chorde/clients/_async.pyx":101
  *     def __cinit__(self, defer):
  *         self.defer = defer
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         self.defer.set_exception(value[1] or value[0])
  * 
  */
 
@@ -3530,26 +3592,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(1, 89, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 101, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 89, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 101, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DeferExceptionCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_22DeferExceptionCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -3567,35 +3629,35 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":90
+  /* "chorde/clients/_async.pyx":102
  *         self.defer = defer
  *     def __call__(self, value):
  *         self.defer.set_exception(value[1] or value[0])             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 90, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 90, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 90, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
   if (!__pyx_t_5) {
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 90, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
@@ -3606,20 +3668,20 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 90, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":89
+  /* "chorde/clients/_async.pyx":101
  *     def __cinit__(self, defer):
  *         self.defer = defer
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         self.defer.set_exception(value[1] or value[0])
  * 
  */
 
@@ -3669,19 +3731,19 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 2, __pyx_L1_error)
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -3725,19 +3787,19 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 4, __pyx_L1_error)
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -3748,15 +3810,15 @@
   __Pyx_AddTraceback("chorde.clients._async.DeferExceptionCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":95
+/* "chorde/clients/_async.pyx":107
  * cdef class ValueCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -3785,26 +3847,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 95, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 107, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 95, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 107, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ValueCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_13ValueCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_ValueCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -3814,42 +3876,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_13ValueCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_ValueCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":96
+  /* "chorde/clients/_async.pyx":108
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":95
+  /* "chorde/clients/_async.pyx":107
  * cdef class ValueCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":97
+/* "chorde/clients/_async.pyx":109
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -3878,26 +3940,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(1, 97, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 109, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 97, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 109, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ValueCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_13ValueCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_ValueCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -3916,15 +3978,15 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":98
+  /* "chorde/clients/_async.pyx":110
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   __pyx_t_2 = (__pyx_v_value != __pyx_v_6chorde_7clients_6_async_CacheMissError);
@@ -3936,15 +3998,15 @@
   }
   __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
   __pyx_t_2 = ((!(__pyx_t_3 != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":99
+    /* "chorde/clients/_async.pyx":111
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  *             return self.callback(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -3957,31 +4019,31 @@
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 99, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":98
+    /* "chorde/clients/_async.pyx":110
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":97
+  /* "chorde/clients/_async.pyx":109
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -4030,19 +4092,19 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 2, __pyx_L1_error)
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -4086,19 +4148,19 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 4, __pyx_L1_error)
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -4109,15 +4171,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ValueCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":104
+/* "chorde/clients/_async.pyx":116
  * cdef class MissCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -4146,26 +4208,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 104, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 116, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 104, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 116, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.MissCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12MissCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_MissCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -4175,42 +4237,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_12MissCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_MissCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":105
+  /* "chorde/clients/_async.pyx":117
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if value is CacheMissError:
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":104
+  /* "chorde/clients/_async.pyx":116
  * cdef class MissCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":106
+/* "chorde/clients/_async.pyx":118
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             return self.callback(value)
  */
 
@@ -4239,26 +4301,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(1, 106, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 106, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.MissCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12MissCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_MissCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -4276,26 +4338,26 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":107
+  /* "chorde/clients/_async.pyx":119
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":108
+    /* "chorde/clients/_async.pyx":120
  *     def __call__(self, value):
  *         if value is CacheMissError:
  *             return self.callback(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4308,31 +4370,31 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 108, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":107
+    /* "chorde/clients/_async.pyx":119
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":106
+  /* "chorde/clients/_async.pyx":118
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             return self.callback(value)
  */
 
@@ -4381,19 +4443,19 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 2, __pyx_L1_error)
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -4437,19 +4499,19 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 4, __pyx_L1_error)
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -4460,15 +4522,15 @@
   __Pyx_AddTraceback("chorde.clients._async.MissCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":113
+/* "chorde/clients/_async.pyx":125
  * cdef class ExceptionCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -4497,26 +4559,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 113, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 113, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 125, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_17ExceptionCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -4526,42 +4588,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_17ExceptionCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":114
+  /* "chorde/clients/_async.pyx":126
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":113
+  /* "chorde/clients/_async.pyx":125
  * cdef class ExceptionCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":115
+/* "chorde/clients/_async.pyx":127
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -4590,26 +4652,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(1, 115, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 127, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 115, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 127, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_17ExceptionCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -4627,26 +4689,26 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":116
+  /* "chorde/clients/_async.pyx":128
  *         self.callback = callback
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":117
+    /* "chorde/clients/_async.pyx":129
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):
  *             return self.callback(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4659,31 +4721,31 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 117, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":116
+    /* "chorde/clients/_async.pyx":128
  *         self.callback = callback
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":115
+  /* "chorde/clients/_async.pyx":127
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -4732,19 +4794,19 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 2, __pyx_L1_error)
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -4788,19 +4850,19 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 4, __pyx_L1_error)
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -4811,15 +4873,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ExceptionCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":122
+/* "chorde/clients/_async.pyx":134
  * cdef class AnyCallback:
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):             # <<<<<<<<<<<<<<
  *         self.on_value = on_value
  *         self.on_miss = on_miss
  */
 
@@ -4856,40 +4918,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_miss)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(1, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_exc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(1, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 134, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 122, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_on_value = values[0];
     __pyx_v_on_miss = values[1];
     __pyx_v_on_exc = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 122, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 134, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.AnyCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_11AnyCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_AnyCallback *)__pyx_v_self), __pyx_v_on_value, __pyx_v_on_miss, __pyx_v_on_exc);
 
@@ -4899,68 +4961,68 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_11AnyCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_AnyCallback *__pyx_v_self, PyObject *__pyx_v_on_value, PyObject *__pyx_v_on_miss, PyObject *__pyx_v_on_exc) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":123
+  /* "chorde/clients/_async.pyx":135
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):
  *         self.on_value = on_value             # <<<<<<<<<<<<<<
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc
  */
   __Pyx_INCREF(__pyx_v_on_value);
   __Pyx_GIVEREF(__pyx_v_on_value);
   __Pyx_GOTREF(__pyx_v_self->on_value);
   __Pyx_DECREF(__pyx_v_self->on_value);
   __pyx_v_self->on_value = __pyx_v_on_value;
 
-  /* "chorde/clients/_async.pyx":124
+  /* "chorde/clients/_async.pyx":136
  *     def __cinit__(self, on_value, on_miss, on_exc):
  *         self.on_value = on_value
  *         self.on_miss = on_miss             # <<<<<<<<<<<<<<
  *         self.on_exc = on_exc
  *     def __call__(self, value):
  */
   __Pyx_INCREF(__pyx_v_on_miss);
   __Pyx_GIVEREF(__pyx_v_on_miss);
   __Pyx_GOTREF(__pyx_v_self->on_miss);
   __Pyx_DECREF(__pyx_v_self->on_miss);
   __pyx_v_self->on_miss = __pyx_v_on_miss;
 
-  /* "chorde/clients/_async.pyx":125
+  /* "chorde/clients/_async.pyx":137
  *         self.on_value = on_value
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if value is CacheMissError:
  */
   __Pyx_INCREF(__pyx_v_on_exc);
   __Pyx_GIVEREF(__pyx_v_on_exc);
   __Pyx_GOTREF(__pyx_v_self->on_exc);
   __Pyx_DECREF(__pyx_v_self->on_exc);
   __pyx_v_self->on_exc = __pyx_v_on_exc;
 
-  /* "chorde/clients/_async.pyx":122
+  /* "chorde/clients/_async.pyx":134
  * cdef class AnyCallback:
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):             # <<<<<<<<<<<<<<
  *         self.on_value = on_value
  *         self.on_miss = on_miss
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":126
+/* "chorde/clients/_async.pyx":138
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             if self.on_miss is not None:
  */
 
@@ -4989,26 +5051,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(1, 126, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 138, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 126, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 138, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.AnyCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_11AnyCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_AnyCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -5026,37 +5088,37 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":127
+  /* "chorde/clients/_async.pyx":139
  *         self.on_exc = on_exc
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  */
   __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":128
+    /* "chorde/clients/_async.pyx":140
  *     def __call__(self, value):
  *         if value is CacheMissError:
  *             if self.on_miss is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  */
     __pyx_t_2 = (__pyx_v_self->on_miss != Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":129
+      /* "chorde/clients/_async.pyx":141
  *         if value is CacheMissError:
  *             if self.on_miss is not None:
  *                 return self.on_miss()             # <<<<<<<<<<<<<<
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5069,63 +5131,63 @@
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 129, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":128
+      /* "chorde/clients/_async.pyx":140
  *     def __call__(self, value):
  *         if value is CacheMissError:
  *             if self.on_miss is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  */
     }
 
-    /* "chorde/clients/_async.pyx":127
+    /* "chorde/clients/_async.pyx":139
  *         self.on_exc = on_exc
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":130
+  /* "chorde/clients/_async.pyx":142
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             if self.on_exc is not None:
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":131
+    /* "chorde/clients/_async.pyx":143
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  */
     __pyx_t_2 = (__pyx_v_self->on_exc != Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":132
+      /* "chorde/clients/_async.pyx":144
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:
  *                 return self.on_exc((<ExceptionWrapper>value).value)             # <<<<<<<<<<<<<<
  *         else:
  *             if self.on_value is not None:
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5138,53 +5200,53 @@
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_value)->value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_value)->value);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 132, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":131
+      /* "chorde/clients/_async.pyx":143
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":130
+    /* "chorde/clients/_async.pyx":142
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             if self.on_exc is not None:
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":134
+  /* "chorde/clients/_async.pyx":146
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  *             if self.on_value is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_value(value)
  * 
  */
   /*else*/ {
     __pyx_t_1 = (__pyx_v_self->on_value != Py_None);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "chorde/clients/_async.pyx":135
+      /* "chorde/clients/_async.pyx":147
  *         else:
  *             if self.on_value is not None:
  *                 return self.on_value(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5197,33 +5259,33 @@
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 135, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":134
+      /* "chorde/clients/_async.pyx":146
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  *             if self.on_value is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_value(value)
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "chorde/clients/_async.pyx":126
+  /* "chorde/clients/_async.pyx":138
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             if self.on_miss is not None:
  */
 
@@ -5272,19 +5334,19 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 2, __pyx_L1_error)
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -5328,19 +5390,19 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 4, __pyx_L1_error)
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -5351,15 +5413,15 @@
   __Pyx_AddTraceback("chorde.clients._async.AnyCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":140
+/* "chorde/clients/_async.pyx":152
  * cdef class DoneCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -5388,26 +5450,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 140, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 152, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 140, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 152, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DoneCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12DoneCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -5417,42 +5479,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_12DoneCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":141
+  /* "chorde/clients/_async.pyx":153
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         return self.callback()
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":140
+  /* "chorde/clients/_async.pyx":152
  * cdef class DoneCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":142
+/* "chorde/clients/_async.pyx":154
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         return self.callback()
  * 
  */
 
@@ -5481,26 +5543,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(1, 142, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 154, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 142, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 154, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DoneCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12DoneCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -5516,15 +5578,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":143
+  /* "chorde/clients/_async.pyx":155
  *         self.callback = callback
  *     def __call__(self, value):
  *         return self.callback()             # <<<<<<<<<<<<<<
  * 
  * cdef class NONE:
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5537,22 +5599,22 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 143, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":142
+  /* "chorde/clients/_async.pyx":154
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         return self.callback()
  * 
  */
 
@@ -5599,19 +5661,19 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 2, __pyx_L1_error)
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -5655,19 +5717,19 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 4, __pyx_L1_error)
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -5730,15 +5792,15 @@
   /* "(tree fragment)":6
  *     cdef bint use_setstate
  *     state = ()
  *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
  *     if _dict is not None:
  *         state += (_dict,)
  */
-  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v__dict = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "(tree fragment)":7
  *     state = ()
  *     _dict = getattr(self, '__dict__', None)
@@ -5753,20 +5815,20 @@
     /* "(tree fragment)":8
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  *         state += (_dict,)             # <<<<<<<<<<<<<<
  *         use_setstate = True
  *     else:
  */
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v__dict);
     __Pyx_GIVEREF(__pyx_v__dict);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict);
-    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 8, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 8, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_4));
     __pyx_t_4 = 0;
 
     /* "(tree fragment)":9
  *     if _dict is not None:
@@ -5813,28 +5875,28 @@
  *         use_setstate = False
  *     if use_setstate:
  *         return __pyx_unpickle_NONE, (type(self), 0xd41d8cd, None), state             # <<<<<<<<<<<<<<
  *     else:
  *         return __pyx_unpickle_NONE, (type(self), 0xd41d8cd, state)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_NONE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_NONE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_INCREF(__pyx_int_222419149);
     __Pyx_GIVEREF(__pyx_int_222419149);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_222419149);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
@@ -5859,28 +5921,28 @@
  *     else:
  *         return __pyx_unpickle_NONE, (type(self), 0xd41d8cd, state)             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_NONE__set_state(self, __pyx_state)
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_NONE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 15, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_NONE); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_INCREF(__pyx_int_222419149);
     __Pyx_GIVEREF(__pyx_int_222419149);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_222419149);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
     __pyx_t_5 = 0;
     __pyx_t_1 = 0;
@@ -5940,16 +6002,16 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_NONE, (type(self), 0xd41d8cd, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_NONE__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async___pyx_unpickle_NONE__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async___pyx_unpickle_NONE__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_NONE, (type(self), 0xd41d8cd, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
@@ -5965,15 +6027,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":150
+/* "chorde/clients/_async.pyx":162
  * @cython.freelist(100)
  * cdef class Future:
  *     def __cinit__(self, logger = None):             # <<<<<<<<<<<<<<
  *         self._cb = None
  *         self._value = NONE
  */
 
@@ -6005,29 +6067,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_logger);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 150, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 162, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_logger = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 150, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 162, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_logger);
 
@@ -6037,108 +6099,108 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_6Future___cinit__(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_logger) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":151
+  /* "chorde/clients/_async.pyx":163
  * cdef class Future:
  *     def __cinit__(self, logger = None):
  *         self._cb = None             # <<<<<<<<<<<<<<
  *         self._value = NONE
  *         self._logger = logger
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_cb);
   __Pyx_DECREF(__pyx_v_self->_cb);
   __pyx_v_self->_cb = ((PyObject*)Py_None);
 
-  /* "chorde/clients/_async.pyx":152
+  /* "chorde/clients/_async.pyx":164
  *     def __cinit__(self, logger = None):
  *         self._cb = None
  *         self._value = NONE             # <<<<<<<<<<<<<<
  *         self._logger = logger
  *         self._done_event = None
  */
   __Pyx_INCREF(((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __Pyx_GOTREF(__pyx_v_self->_value);
   __Pyx_DECREF(__pyx_v_self->_value);
   __pyx_v_self->_value = ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE);
 
-  /* "chorde/clients/_async.pyx":153
+  /* "chorde/clients/_async.pyx":165
  *         self._cb = None
  *         self._value = NONE
  *         self._logger = logger             # <<<<<<<<<<<<<<
  *         self._done_event = None
  *         self._running = 0
  */
   __Pyx_INCREF(__pyx_v_logger);
   __Pyx_GIVEREF(__pyx_v_logger);
   __Pyx_GOTREF(__pyx_v_self->_logger);
   __Pyx_DECREF(__pyx_v_self->_logger);
   __pyx_v_self->_logger = __pyx_v_logger;
 
-  /* "chorde/clients/_async.pyx":154
+  /* "chorde/clients/_async.pyx":166
  *         self._value = NONE
  *         self._logger = logger
  *         self._done_event = None             # <<<<<<<<<<<<<<
  *         self._running = 0
  *         self._cancel_pending = 0
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_done_event);
   __Pyx_DECREF(__pyx_v_self->_done_event);
   __pyx_v_self->_done_event = Py_None;
 
-  /* "chorde/clients/_async.pyx":155
+  /* "chorde/clients/_async.pyx":167
  *         self._logger = logger
  *         self._done_event = None
  *         self._running = 0             # <<<<<<<<<<<<<<
  *         self._cancel_pending = 0
  *         self._cancelled = 0
  */
   __pyx_v_self->_running = 0;
 
-  /* "chorde/clients/_async.pyx":156
+  /* "chorde/clients/_async.pyx":168
  *         self._done_event = None
  *         self._running = 0
  *         self._cancel_pending = 0             # <<<<<<<<<<<<<<
  *         self._cancelled = 0
  * 
  */
   __pyx_v_self->_cancel_pending = 0;
 
-  /* "chorde/clients/_async.pyx":157
+  /* "chorde/clients/_async.pyx":169
  *         self._running = 0
  *         self._cancel_pending = 0
  *         self._cancelled = 0             # <<<<<<<<<<<<<<
  * 
  *     cpdef _set_nothreads(self, value):
  */
   __pyx_v_self->_cancelled = 0;
 
-  /* "chorde/clients/_async.pyx":150
+  /* "chorde/clients/_async.pyx":162
  * @cython.freelist(100)
  * cdef class Future:
  *     def __cinit__(self, logger = None):             # <<<<<<<<<<<<<<
  *         self._cb = None
  *         self._value = NONE
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":159
+/* "chorde/clients/_async.pyx":171
  *         self._cancelled = 0
  * 
  *     cpdef _set_nothreads(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Like set(), but assuming no threading is involved. It won't wake waiting threads,
  */
 
@@ -6173,15 +6235,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_nothreads); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 159, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_nothreads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_6Future_3_set_nothreads)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6190,15 +6252,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 159, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -6211,236 +6273,236 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":167
+  /* "chorde/clients/_async.pyx":179
  *         cdef object old, cbs, _cb
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             # No setting twice
  *             return
  */
   __pyx_t_5 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":169
+    /* "chorde/clients/_async.pyx":181
  *         if self._value is not NONE:
  *             # No setting twice
  *             return             # <<<<<<<<<<<<<<
  * 
  *         # start atomic op
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":167
+    /* "chorde/clients/_async.pyx":179
  *         cdef object old, cbs, _cb
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             # No setting twice
  *             return
  */
   }
 
-  /* "chorde/clients/_async.pyx":172
+  /* "chorde/clients/_async.pyx":184
  * 
  *         # start atomic op
  *         old = self._value # avoid deadlocks due to finalizers             # <<<<<<<<<<<<<<
  *         _cb = self._cb
  *         if _cb is not None:
  */
   __pyx_t_1 = __pyx_v_self->_value;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_old = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":173
+  /* "chorde/clients/_async.pyx":185
  *         # start atomic op
  *         old = self._value # avoid deadlocks due to finalizers
  *         _cb = self._cb             # <<<<<<<<<<<<<<
  *         if _cb is not None:
  *             self._cb = None
  */
   __pyx_t_1 = __pyx_v_self->_cb;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v__cb = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":174
+  /* "chorde/clients/_async.pyx":186
  *         old = self._value # avoid deadlocks due to finalizers
  *         _cb = self._cb
  *         if _cb is not None:             # <<<<<<<<<<<<<<
  *             self._cb = None
  *             self._value = value
  */
   __pyx_t_6 = (__pyx_v__cb != Py_None);
   __pyx_t_5 = (__pyx_t_6 != 0);
   if (__pyx_t_5) {
 
-    /* "chorde/clients/_async.pyx":175
+    /* "chorde/clients/_async.pyx":187
  *         _cb = self._cb
  *         if _cb is not None:
  *             self._cb = None             # <<<<<<<<<<<<<<
  *             self._value = value
  *             cbs = list(_cb) # end atomic op
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_cb);
     __Pyx_DECREF(__pyx_v_self->_cb);
     __pyx_v_self->_cb = ((PyObject*)Py_None);
 
-    /* "chorde/clients/_async.pyx":176
+    /* "chorde/clients/_async.pyx":188
  *         if _cb is not None:
  *             self._cb = None
  *             self._value = value             # <<<<<<<<<<<<<<
  *             cbs = list(_cb) # end atomic op
  *         else:
  */
     __Pyx_INCREF(__pyx_v_value);
     __Pyx_GIVEREF(__pyx_v_value);
     __Pyx_GOTREF(__pyx_v_self->_value);
     __Pyx_DECREF(__pyx_v_self->_value);
     __pyx_v_self->_value = __pyx_v_value;
 
-    /* "chorde/clients/_async.pyx":177
+    /* "chorde/clients/_async.pyx":189
  *             self._cb = None
  *             self._value = value
  *             cbs = list(_cb) # end atomic op             # <<<<<<<<<<<<<<
  *         else:
  *             cbs = None
  */
-    __pyx_t_1 = PySequence_List(__pyx_v__cb); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 177, __pyx_L1_error)
+    __pyx_t_1 = PySequence_List(__pyx_v__cb); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_cbs = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "chorde/clients/_async.pyx":174
+    /* "chorde/clients/_async.pyx":186
  *         old = self._value # avoid deadlocks due to finalizers
  *         _cb = self._cb
  *         if _cb is not None:             # <<<<<<<<<<<<<<
  *             self._cb = None
  *             self._value = value
  */
     goto __pyx_L4;
   }
 
-  /* "chorde/clients/_async.pyx":179
+  /* "chorde/clients/_async.pyx":191
  *             cbs = list(_cb) # end atomic op
  *         else:
  *             cbs = None             # <<<<<<<<<<<<<<
  *             self._value = value # end atomic op
  *         self._running = 0
  */
   /*else*/ {
     __Pyx_INCREF(Py_None);
     __pyx_v_cbs = Py_None;
 
-    /* "chorde/clients/_async.pyx":180
+    /* "chorde/clients/_async.pyx":192
  *         else:
  *             cbs = None
  *             self._value = value # end atomic op             # <<<<<<<<<<<<<<
  *         self._running = 0
  *         del old, _cb
  */
     __Pyx_INCREF(__pyx_v_value);
     __Pyx_GIVEREF(__pyx_v_value);
     __Pyx_GOTREF(__pyx_v_self->_value);
     __Pyx_DECREF(__pyx_v_self->_value);
     __pyx_v_self->_value = __pyx_v_value;
   }
   __pyx_L4:;
 
-  /* "chorde/clients/_async.pyx":181
+  /* "chorde/clients/_async.pyx":193
  *             cbs = None
  *             self._value = value # end atomic op
  *         self._running = 0             # <<<<<<<<<<<<<<
  *         del old, _cb
  * 
  */
   __pyx_v_self->_running = 0;
 
-  /* "chorde/clients/_async.pyx":182
+  /* "chorde/clients/_async.pyx":194
  *             self._value = value # end atomic op
  *         self._running = 0
  *         del old, _cb             # <<<<<<<<<<<<<<
  * 
  *         if cbs is not None:
  */
   __Pyx_DECREF(__pyx_v_old);
   __pyx_v_old = NULL;
   __Pyx_DECREF(__pyx_v__cb);
   __pyx_v__cb = NULL;
 
-  /* "chorde/clients/_async.pyx":184
+  /* "chorde/clients/_async.pyx":196
  *         del old, _cb
  * 
  *         if cbs is not None:             # <<<<<<<<<<<<<<
  *             for cb in cbs:
  *                 try:
  */
   __pyx_t_5 = (__pyx_v_cbs != Py_None);
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":185
+    /* "chorde/clients/_async.pyx":197
  * 
  *         if cbs is not None:
  *             for cb in cbs:             # <<<<<<<<<<<<<<
  *                 try:
  *                     cb(value)
  */
     if (likely(PyList_CheckExact(__pyx_v_cbs)) || PyTuple_CheckExact(__pyx_v_cbs)) {
       __pyx_t_1 = __pyx_v_cbs; __Pyx_INCREF(__pyx_t_1); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_cbs); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 185, __pyx_L1_error)
+      __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_cbs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 185, __pyx_L1_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 197, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 185, __pyx_L1_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 185, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 185, __pyx_L1_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 185, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_8(__pyx_t_1);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 185, __pyx_L1_error)
+            else __PYX_ERR(0, 197, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_v_cb, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "chorde/clients/_async.pyx":186
+      /* "chorde/clients/_async.pyx":198
  *         if cbs is not None:
  *             for cb in cbs:
  *                 try:             # <<<<<<<<<<<<<<
  *                     cb(value)
  *                 except:
  */
       {
@@ -6448,15 +6510,15 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
         __Pyx_XGOTREF(__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_10);
         __Pyx_XGOTREF(__pyx_t_11);
         /*try:*/ {
 
-          /* "chorde/clients/_async.pyx":187
+          /* "chorde/clients/_async.pyx":199
  *             for cb in cbs:
  *                 try:
  *                     cb(value)             # <<<<<<<<<<<<<<
  *                 except:
  *                     if self._logger is not None:
  */
           __Pyx_INCREF(__pyx_v_cb);
@@ -6468,20 +6530,20 @@
               __Pyx_INCREF(__pyx_t_4);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_3, function);
             }
           }
           __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 187, __pyx_L8_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-          /* "chorde/clients/_async.pyx":186
+          /* "chorde/clients/_async.pyx":198
  *         if cbs is not None:
  *             for cb in cbs:
  *                 try:             # <<<<<<<<<<<<<<
  *                     cb(value)
  *                 except:
  */
         }
@@ -6490,101 +6552,101 @@
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
         goto __pyx_L15_try_end;
         __pyx_L8_error:;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "chorde/clients/_async.pyx":188
+        /* "chorde/clients/_async.pyx":200
  *                 try:
  *                     cb(value)
  *                 except:             # <<<<<<<<<<<<<<
  *                     if self._logger is not None:
  *                         error = self._logger
  */
         /*except:*/ {
           __Pyx_AddTraceback("chorde.clients._async.Future._set_nothreads", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(1, 188, __pyx_L10_except_error)
+          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 200, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_4);
 
-          /* "chorde/clients/_async.pyx":189
+          /* "chorde/clients/_async.pyx":201
  *                     cb(value)
  *                 except:
  *                     if self._logger is not None:             # <<<<<<<<<<<<<<
  *                         error = self._logger
  *                     else:
  */
           __pyx_t_6 = (__pyx_v_self->_logger != Py_None);
           __pyx_t_5 = (__pyx_t_6 != 0);
           if (__pyx_t_5) {
 
-            /* "chorde/clients/_async.pyx":190
+            /* "chorde/clients/_async.pyx":202
  *                 except:
  *                     if self._logger is not None:
  *                         error = self._logger             # <<<<<<<<<<<<<<
  *                     else:
  *                         error = logging.error
  */
             __pyx_t_12 = __pyx_v_self->_logger;
             __Pyx_INCREF(__pyx_t_12);
             __Pyx_XDECREF_SET(__pyx_v_error, __pyx_t_12);
             __pyx_t_12 = 0;
 
-            /* "chorde/clients/_async.pyx":189
+            /* "chorde/clients/_async.pyx":201
  *                     cb(value)
  *                 except:
  *                     if self._logger is not None:             # <<<<<<<<<<<<<<
  *                         error = self._logger
  *                     else:
  */
             goto __pyx_L18;
           }
 
-          /* "chorde/clients/_async.pyx":192
+          /* "chorde/clients/_async.pyx":204
  *                         error = self._logger
  *                     else:
  *                         error = logging.error             # <<<<<<<<<<<<<<
  *                     error("Error in async callback", exc_info = True)
  * 
  */
           /*else*/ {
-            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 192, __pyx_L10_except_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 204, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_12);
-            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_error); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 192, __pyx_L10_except_error)
+            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_error); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 204, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_13);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             __Pyx_XDECREF_SET(__pyx_v_error, __pyx_t_13);
             __pyx_t_13 = 0;
           }
           __pyx_L18:;
 
-          /* "chorde/clients/_async.pyx":193
+          /* "chorde/clients/_async.pyx":205
  *                     else:
  *                         error = logging.error
  *                     error("Error in async callback", exc_info = True)             # <<<<<<<<<<<<<<
  * 
  *     cpdef set(self, value):
  */
-          __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 193, __pyx_L10_except_error)
+          __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 205, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_13);
-          if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_exc_info, Py_True) < 0) __PYX_ERR(1, 193, __pyx_L10_except_error)
-          __pyx_t_12 = __Pyx_PyObject_Call(__pyx_v_error, __pyx_tuple__17, __pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 193, __pyx_L10_except_error)
+          if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_exc_info, Py_True) < 0) __PYX_ERR(0, 205, __pyx_L10_except_error)
+          __pyx_t_12 = __Pyx_PyObject_Call(__pyx_v_error, __pyx_tuple__17, __pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 205, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           goto __pyx_L9_exception_handled;
         }
         __pyx_L10_except_error:;
 
-        /* "chorde/clients/_async.pyx":186
+        /* "chorde/clients/_async.pyx":198
  *         if cbs is not None:
  *             for cb in cbs:
  *                 try:             # <<<<<<<<<<<<<<
  *                     cb(value)
  *                 except:
  */
         __Pyx_XGIVEREF(__pyx_t_9);
@@ -6596,34 +6658,34 @@
         __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_XGIVEREF(__pyx_t_11);
         __Pyx_ExceptionReset(__pyx_t_9, __pyx_t_10, __pyx_t_11);
         __pyx_L15_try_end:;
       }
 
-      /* "chorde/clients/_async.pyx":185
+      /* "chorde/clients/_async.pyx":197
  * 
  *         if cbs is not None:
  *             for cb in cbs:             # <<<<<<<<<<<<<<
  *                 try:
  *                     cb(value)
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "chorde/clients/_async.pyx":184
+    /* "chorde/clients/_async.pyx":196
  *         del old, _cb
  * 
  *         if cbs is not None:             # <<<<<<<<<<<<<<
  *             for cb in cbs:
  *                 try:
  */
   }
 
-  /* "chorde/clients/_async.pyx":159
+  /* "chorde/clients/_async.pyx":171
  *         self._cancelled = 0
  * 
  *     cpdef _set_nothreads(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Like set(), but assuming no threading is involved. It won't wake waiting threads,
  */
 
@@ -6669,15 +6731,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_nothreads", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__set_nothreads(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 159, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__set_nothreads(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6686,15 +6748,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":195
+/* "chorde/clients/_async.pyx":207
  *                     error("Error in async callback", exc_info = True)
  * 
  *     cpdef set(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Set the future's result as either a value, an exception wrappedn in ExceptionWrapper, or
  */
 
@@ -6717,15 +6779,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 195, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_6Future_5set)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6734,15 +6796,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 195, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -6755,72 +6817,72 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":200
+  /* "chorde/clients/_async.pyx":212
  *         a cache miss if given CacheMissError (the class itself)
  *         """
  *         self._set_nothreads(value)             # <<<<<<<<<<<<<<
  * 
  *         if self._done_event is not None:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":202
+  /* "chorde/clients/_async.pyx":214
  *         self._set_nothreads(value)
  * 
  *         if self._done_event is not None:             # <<<<<<<<<<<<<<
  *             # wake up waiting threads
  *             self._done_event.set()
  */
   __pyx_t_5 = (__pyx_v_self->_done_event != Py_None);
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":204
+    /* "chorde/clients/_async.pyx":216
  *         if self._done_event is not None:
  *             # wake up waiting threads
  *             self._done_event.set()             # <<<<<<<<<<<<<<
  * 
  *     def set_result(self, value):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 204, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 204, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "chorde/clients/_async.pyx":202
+    /* "chorde/clients/_async.pyx":214
  *         self._set_nothreads(value)
  * 
  *         if self._done_event is not None:             # <<<<<<<<<<<<<<
  *             # wake up waiting threads
  *             self._done_event.set()
  */
   }
 
-  /* "chorde/clients/_async.pyx":195
+  /* "chorde/clients/_async.pyx":207
  *                     error("Error in async callback", exc_info = True)
  * 
  *     cpdef set(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Set the future's result as either a value, an exception wrappedn in ExceptionWrapper, or
  */
 
@@ -6859,15 +6921,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future_set(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 195, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future_set(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6876,15 +6938,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":206
+/* "chorde/clients/_async.pyx":218
  *             self._done_event.set()
  * 
  *     def set_result(self, value):             # <<<<<<<<<<<<<<
  *         self.set(value)
  * 
  */
 
@@ -6906,26 +6968,26 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_result", 0);
 
-  /* "chorde/clients/_async.pyx":207
+  /* "chorde/clients/_async.pyx":219
  * 
  *     def set_result(self, value):
  *         self.set(value)             # <<<<<<<<<<<<<<
  * 
  *     def miss(self):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 207, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":206
+  /* "chorde/clients/_async.pyx":218
  *             self._done_event.set()
  * 
  *     def set_result(self, value):             # <<<<<<<<<<<<<<
  *         self.set(value)
  * 
  */
 
@@ -6938,15 +7000,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":209
+/* "chorde/clients/_async.pyx":221
  *         self.set(value)
  * 
  *     def miss(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result
  */
 
@@ -6970,29 +7032,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("miss", 0);
 
-  /* "chorde/clients/_async.pyx":213
+  /* "chorde/clients/_async.pyx":225
  *         Shorthand for setting a cache miss result
  *         """
  *         self.set(CacheMissError)             # <<<<<<<<<<<<<<
  * 
  *     def _miss_nothreads(self):
  */
   __pyx_t_1 = __pyx_v_6chorde_7clients_6_async_CacheMissError;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 213, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":209
+  /* "chorde/clients/_async.pyx":221
  *         self.set(value)
  * 
  *     def miss(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result
  */
 
@@ -7006,15 +7068,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":215
+/* "chorde/clients/_async.pyx":227
  *         self.set(CacheMissError)
  * 
  *     def _miss_nothreads(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result without thread safety.
  */
 
@@ -7038,29 +7100,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_miss_nothreads", 0);
 
-  /* "chorde/clients/_async.pyx":220
+  /* "chorde/clients/_async.pyx":232
  *         See _set_nothreads
  *         """
  *         self._set_nothreads(CacheMissError)             # <<<<<<<<<<<<<<
  * 
  *     def exc(self, exc_info):
  */
   __pyx_t_1 = __pyx_v_6chorde_7clients_6_async_CacheMissError;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 220, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":215
+  /* "chorde/clients/_async.pyx":227
  *         self.set(CacheMissError)
  * 
  *     def _miss_nothreads(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result without thread safety.
  */
 
@@ -7074,15 +7136,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":222
+/* "chorde/clients/_async.pyx":234
  *         self._set_nothreads(CacheMissError)
  * 
  *     def exc(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7106,35 +7168,35 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exc", 0);
 
-  /* "chorde/clients/_async.pyx":227
+  /* "chorde/clients/_async.pyx":239
  *         as returned by sys.exc_info()
  *         """
  *         self.set(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))             # <<<<<<<<<<<<<<
  * 
  *     def _exc_nothreads(self, exc_info):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 227, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_exc_info);
   __Pyx_GIVEREF(__pyx_v_exc_info);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_exc_info);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 227, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 227, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":222
+  /* "chorde/clients/_async.pyx":234
  *         self._set_nothreads(CacheMissError)
  * 
  *     def exc(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7148,15 +7210,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":229
+/* "chorde/clients/_async.pyx":241
  *         self.set(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def _exc_nothreads(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7180,35 +7242,35 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_exc_nothreads", 0);
 
-  /* "chorde/clients/_async.pyx":235
+  /* "chorde/clients/_async.pyx":247
  *         See _set_nothreads
  *         """
  *         self._set_nothreads(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))             # <<<<<<<<<<<<<<
  * 
  *     def set_exception(self, exception):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 235, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_exc_info);
   __Pyx_GIVEREF(__pyx_v_exc_info);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_exc_info);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 235, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 235, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":229
+  /* "chorde/clients/_async.pyx":241
  *         self.set(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def _exc_nothreads(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7222,15 +7284,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":237
+/* "chorde/clients/_async.pyx":249
  *         self._set_nothreads(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def set_exception(self, exception):             # <<<<<<<<<<<<<<
  *         """
  *         Set the Future's exception object.
  */
 
@@ -7260,82 +7322,82 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_exception", 0);
   __Pyx_INCREF(__pyx_v_exception);
 
-  /* "chorde/clients/_async.pyx":241
+  /* "chorde/clients/_async.pyx":253
  *         Set the Future's exception object.
  *         """
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:             # <<<<<<<<<<<<<<
  *             exception = exception.with_traceback(None)
  *         self.exc((type(exception),exception,None))
  */
   __pyx_t_2 = (__pyx_v_6chorde_7clients_6_async_strip_tracebacks != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_exception, __pyx_n_s_traceback, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 241, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_exception, __pyx_n_s_traceback, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = (__pyx_t_3 != Py_None);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = (__pyx_t_2 != 0);
   __pyx_t_1 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":242
+    /* "chorde/clients/_async.pyx":254
  *         """
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:
  *             exception = exception.with_traceback(None)             # <<<<<<<<<<<<<<
  *         self.exc((type(exception),exception,None))
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 242, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, Py_None) : __Pyx_PyObject_CallOneArg(__pyx_t_5, Py_None);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 242, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 254, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_exception, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "chorde/clients/_async.pyx":241
+    /* "chorde/clients/_async.pyx":253
  *         Set the Future's exception object.
  *         """
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:             # <<<<<<<<<<<<<<
  *             exception = exception.with_traceback(None)
  *         self.exc((type(exception),exception,None))
  */
   }
 
-  /* "chorde/clients/_async.pyx":243
+  /* "chorde/clients/_async.pyx":255
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:
  *             exception = exception.with_traceback(None)
  *         self.exc((type(exception),exception,None))             # <<<<<<<<<<<<<<
  * 
  *     def on_value(self, callback):
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_exc); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 243, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_exc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 243, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_exception)));
   __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_exception)));
   PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)Py_TYPE(__pyx_v_exception)));
   __Pyx_INCREF(__pyx_v_exception);
   __Pyx_GIVEREF(__pyx_v_exception);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_exception);
@@ -7351,20 +7413,20 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 243, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "chorde/clients/_async.pyx":237
+  /* "chorde/clients/_async.pyx":249
  *         self._set_nothreads(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def set_exception(self, exception):             # <<<<<<<<<<<<<<
  *         """
  *         Set the Future's exception object.
  */
 
@@ -7381,15 +7443,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_exception);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":245
+/* "chorde/clients/_async.pyx":257
  *         self.exc((type(exception),exception,None))
  * 
  *     def on_value(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When and if the operation completes without exception, the callback
  */
 
@@ -7413,38 +7475,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_value", 0);
 
-  /* "chorde/clients/_async.pyx":250
+  /* "chorde/clients/_async.pyx":262
  *         will be invoked with its result.
  *         """
  *         return self._on_stuff(ValueCallback.__new__(ValueCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def on_miss(self, callback):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 250, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ValueCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ValueCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 250, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ValueCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ValueCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 262, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 250, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":245
+  /* "chorde/clients/_async.pyx":257
  *         self.exc((type(exception),exception,None))
  * 
  *     def on_value(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When and if the operation completes without exception, the callback
  */
 
@@ -7456,15 +7518,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":252
+/* "chorde/clients/_async.pyx":264
  *         return self._on_stuff(ValueCallback.__new__(ValueCallback, callback))
  * 
  *     def on_miss(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in a cache miss, the callback will be invoked
  */
 
@@ -7488,38 +7550,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_miss", 0);
 
-  /* "chorde/clients/_async.pyx":257
+  /* "chorde/clients/_async.pyx":269
  *         without arugments.
  *         """
  *         return self._on_stuff(MissCallback.__new__(MissCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def on_exc(self, callback):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 257, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_MissCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_MissCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 257, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_MissCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_MissCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 257, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":252
+  /* "chorde/clients/_async.pyx":264
  *         return self._on_stuff(ValueCallback.__new__(ValueCallback, callback))
  * 
  *     def on_miss(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in a cache miss, the callback will be invoked
  */
 
@@ -7531,15 +7593,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":259
+/* "chorde/clients/_async.pyx":271
  *         return self._on_stuff(MissCallback.__new__(MissCallback, callback))
  * 
  *     def on_exc(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in an exception, the callback will be invoked
  */
 
@@ -7563,38 +7625,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_exc", 0);
 
-  /* "chorde/clients/_async.pyx":264
+  /* "chorde/clients/_async.pyx":276
  *         with an exc_info tuple as returned by sys.exc_info.
  *         """
  *         return self._on_stuff(ExceptionCallback.__new__(ExceptionCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def on_any(self, on_value = None, on_miss = None, on_exc = None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 264, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 264, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 264, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":259
+  /* "chorde/clients/_async.pyx":271
  *         return self._on_stuff(MissCallback.__new__(MissCallback, callback))
  * 
  *     def on_exc(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in an exception, the callback will be invoked
  */
 
@@ -7606,15 +7668,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":266
+/* "chorde/clients/_async.pyx":278
  *         return self._on_stuff(ExceptionCallback.__new__(ExceptionCallback, callback))
  * 
  *     def on_any(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Handy method to set callbacks for all kinds of results, and it's actually
  */
 
@@ -7667,15 +7729,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_exc);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any") < 0)) __PYX_ERR(1, 266, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any") < 0)) __PYX_ERR(0, 278, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7687,15 +7749,15 @@
     }
     __pyx_v_on_value = values[0];
     __pyx_v_on_miss = values[1];
     __pyx_v_on_exc = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("on_any", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 266, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("on_any", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 278, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.on_any", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_24on_any(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_on_value, __pyx_v_on_miss, __pyx_v_on_exc);
 
@@ -7710,44 +7772,44 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_any", 0);
 
-  /* "chorde/clients/_async.pyx":271
+  /* "chorde/clients/_async.pyx":283
  *         faster than calling on_X repeatedly. None callbacks will be ignored.
  *         """
  *         return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))             # <<<<<<<<<<<<<<
  * 
  *     def on_any_once(self, on_value = None, on_miss = None, on_exc = None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 271, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_on_value);
   __Pyx_GIVEREF(__pyx_v_on_value);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_on_value);
   __Pyx_INCREF(__pyx_v_on_miss);
   __Pyx_GIVEREF(__pyx_v_on_miss);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_on_miss);
   __Pyx_INCREF(__pyx_v_on_exc);
   __Pyx_GIVEREF(__pyx_v_on_exc);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_on_exc);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 271, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 271, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":266
+  /* "chorde/clients/_async.pyx":278
  *         return self._on_stuff(ExceptionCallback.__new__(ExceptionCallback, callback))
  * 
  *     def on_any(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Handy method to set callbacks for all kinds of results, and it's actually
  */
 
@@ -7759,15 +7821,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":273
+/* "chorde/clients/_async.pyx":285
  *         return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_any_once(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Like on_any, but will only set the callback if no other callback has been set
  */
 
@@ -7820,15 +7882,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_exc);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any_once") < 0)) __PYX_ERR(1, 273, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any_once") < 0)) __PYX_ERR(0, 285, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7840,15 +7902,15 @@
     }
     __pyx_v_on_value = values[0];
     __pyx_v_on_miss = values[1];
     __pyx_v_on_exc = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("on_any_once", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 273, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("on_any_once", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 285, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.on_any_once", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_26on_any_once(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_on_value, __pyx_v_on_miss, __pyx_v_on_exc);
 
@@ -7865,64 +7927,64 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_any_once", 0);
 
-  /* "chorde/clients/_async.pyx":277
+  /* "chorde/clients/_async.pyx":289
  *         Like on_any, but will only set the callback if no other callback has been set
  *         """
  *         if self._cb is None:             # <<<<<<<<<<<<<<
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_cb == ((PyObject*)Py_None));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":278
+    /* "chorde/clients/_async.pyx":290
  *         """
  *         if self._cb is None:
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))             # <<<<<<<<<<<<<<
  * 
  *     def on_done(self, callback):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 278, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_on_value);
     __Pyx_GIVEREF(__pyx_v_on_value);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_on_value);
     __Pyx_INCREF(__pyx_v_on_miss);
     __Pyx_GIVEREF(__pyx_v_on_miss);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_on_miss);
     __Pyx_INCREF(__pyx_v_on_exc);
     __Pyx_GIVEREF(__pyx_v_on_exc);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_on_exc);
-    __pyx_t_4 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_3, NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 278, __pyx_L1_error)
+    __pyx_t_4 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_3, NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(((PyObject *)__pyx_t_4));
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_4), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 278, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_4), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(((PyObject *)__pyx_t_4)); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":277
+    /* "chorde/clients/_async.pyx":289
  *         Like on_any, but will only set the callback if no other callback has been set
  *         """
  *         if self._cb is None:             # <<<<<<<<<<<<<<
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":273
+  /* "chorde/clients/_async.pyx":285
  *         return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_any_once(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Like on_any, but will only set the callback if no other callback has been set
  */
 
@@ -7936,15 +7998,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":280
+/* "chorde/clients/_async.pyx":292
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_done(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operation is done, the callback will be invoked without arguments,
  */
 
@@ -7968,38 +8030,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_done", 0);
 
-  /* "chorde/clients/_async.pyx":285
+  /* "chorde/clients/_async.pyx":297
  *         regardless of the outcome. If the operation is cancelled, it won't be invoked.
  *         """
  *         return self._on_stuff(DoneCallback.__new__(DoneCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def chain(self, defer):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 285, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DoneCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DoneCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 285, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DoneCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DoneCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 285, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":280
+  /* "chorde/clients/_async.pyx":292
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_done(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operation is done, the callback will be invoked without arguments,
  */
 
@@ -8011,15 +8073,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":287
+/* "chorde/clients/_async.pyx":299
  *         return self._on_stuff(DoneCallback.__new__(DoneCallback, callback))
  * 
  *     def chain(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer
  */
 
@@ -8043,29 +8105,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chain", 0);
 
-  /* "chorde/clients/_async.pyx":291
+  /* "chorde/clients/_async.pyx":303
  *         Invoke all the callbacks of the other defer
  *         """
  *         self._on_stuff(defer.set)             # <<<<<<<<<<<<<<
  * 
  *     def chain_std(self, defer):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 291, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 291, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":287
+  /* "chorde/clients/_async.pyx":299
  *         return self._on_stuff(DoneCallback.__new__(DoneCallback, callback))
  * 
  *     def chain(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer
  */
 
@@ -8079,15 +8141,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":293
+/* "chorde/clients/_async.pyx":305
  *         self._on_stuff(defer.set)
  * 
  *     def chain_std(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer, without assuming the other
  */
 
@@ -8119,58 +8181,58 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chain_std", 0);
 
-  /* "chorde/clients/_async.pyx":298
+  /* "chorde/clients/_async.pyx":310
  *         defer follows our non-standard interface.
  *         """
  *         return self.on_any(             # <<<<<<<<<<<<<<
  *             defer.set_result,
  *             functools_partial(defer.set_exception, CacheMissError()),
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_any); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 298, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 310, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "chorde/clients/_async.pyx":299
+  /* "chorde/clients/_async.pyx":311
  *         """
  *         return self.on_any(
  *             defer.set_result,             # <<<<<<<<<<<<<<
  *             functools_partial(defer.set_exception, CacheMissError()),
  *             DeferExceptionCallback.__new__(DeferExceptionCallback, defer)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 299, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "chorde/clients/_async.pyx":300
+  /* "chorde/clients/_async.pyx":312
  *         return self.on_any(
  *             defer.set_result,
  *             functools_partial(defer.set_exception, CacheMissError()),             # <<<<<<<<<<<<<<
  *             DeferExceptionCallback.__new__(DeferExceptionCallback, defer)
  *         )
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 300, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
   __pyx_t_7 = __pyx_v_6chorde_7clients_6_async_CacheMissError; __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 300, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_functools_partial);
   __pyx_t_7 = __pyx_v_6chorde_7clients_6_async_functools_partial; __pyx_t_8 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
@@ -8181,62 +8243,62 @@
       __Pyx_DECREF_SET(__pyx_t_7, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 300, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 300, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 300, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_8) {
       __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_6);
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 300, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "chorde/clients/_async.pyx":301
+  /* "chorde/clients/_async.pyx":313
  *             defer.set_result,
  *             functools_partial(defer.set_exception, CacheMissError()),
  *             DeferExceptionCallback.__new__(DeferExceptionCallback, defer)             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 301, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_v_defer);
   __Pyx_GIVEREF(__pyx_v_defer);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_defer);
-  __pyx_t_10 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DeferExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DeferExceptionCallback), __pyx_t_7, NULL)); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 301, __pyx_L1_error)
+  __pyx_t_10 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DeferExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DeferExceptionCallback), __pyx_t_7, NULL)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_10));
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -8246,58 +8308,58 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_t_10)};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 298, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(((PyObject *)__pyx_t_10)); __pyx_t_10 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_t_10)};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 298, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(((PyObject *)__pyx_t_10)); __pyx_t_10 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 298, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_9, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_9, __pyx_t_4);
     __Pyx_GIVEREF(((PyObject *)__pyx_t_10));
     PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_9, ((PyObject *)__pyx_t_10));
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_t_10 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 298, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":293
+  /* "chorde/clients/_async.pyx":305
  *         self._on_stuff(defer.set)
  * 
  *     def chain_std(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer, without assuming the other
  */
 
@@ -8316,15 +8378,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":304
+/* "chorde/clients/_async.pyx":316
  *         )
  * 
  *     cpdef _on_stuff(self, callback):             # <<<<<<<<<<<<<<
  *         if self._value is NONE:
  *             if self._cb is None:
  */
 
@@ -8348,15 +8410,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_stuff); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 304, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_stuff); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_6Future_35_on_stuff)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8365,15 +8427,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_callback) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_callback);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 304, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 316, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -8386,84 +8448,84 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":305
+  /* "chorde/clients/_async.pyx":317
  * 
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:             # <<<<<<<<<<<<<<
  *             if self._cb is None:
  *                 self._cb = list()
  */
   __pyx_t_5 = (__pyx_v_self->_value == ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":306
+    /* "chorde/clients/_async.pyx":318
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:
  *             if self._cb is None:             # <<<<<<<<<<<<<<
  *                 self._cb = list()
  *             self._cb.append(callback)
  */
     __pyx_t_6 = (__pyx_v_self->_cb == ((PyObject*)Py_None));
     __pyx_t_5 = (__pyx_t_6 != 0);
     if (__pyx_t_5) {
 
-      /* "chorde/clients/_async.pyx":307
+      /* "chorde/clients/_async.pyx":319
  *         if self._value is NONE:
  *             if self._cb is None:
  *                 self._cb = list()             # <<<<<<<<<<<<<<
  *             self._cb.append(callback)
  *         else:
  */
-      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 307, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_v_self->_cb);
       __Pyx_DECREF(__pyx_v_self->_cb);
       __pyx_v_self->_cb = ((PyObject*)__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "chorde/clients/_async.pyx":306
+      /* "chorde/clients/_async.pyx":318
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:
  *             if self._cb is None:             # <<<<<<<<<<<<<<
  *                 self._cb = list()
  *             self._cb.append(callback)
  */
     }
 
-    /* "chorde/clients/_async.pyx":308
+    /* "chorde/clients/_async.pyx":320
  *             if self._cb is None:
  *                 self._cb = list()
  *             self._cb.append(callback)             # <<<<<<<<<<<<<<
  *         else:
  *             callback(self._value)
  */
     if (unlikely(__pyx_v_self->_cb == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-      __PYX_ERR(1, 308, __pyx_L1_error)
+      __PYX_ERR(0, 320, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_self->_cb, __pyx_v_callback); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 308, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_self->_cb, __pyx_v_callback); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 320, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":305
+    /* "chorde/clients/_async.pyx":317
  * 
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:             # <<<<<<<<<<<<<<
  *             if self._cb is None:
  *                 self._cb = list()
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":310
+  /* "chorde/clients/_async.pyx":322
  *             self._cb.append(callback)
  *         else:
  *             callback(self._value)             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   /*else*/ {
@@ -8476,34 +8538,34 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_self->_value) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_self->_value);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 310, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "chorde/clients/_async.pyx":311
+  /* "chorde/clients/_async.pyx":323
  *         else:
  *             callback(self._value)
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def add_done_callback(self, callback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":304
+  /* "chorde/clients/_async.pyx":316
  *         )
  * 
  *     cpdef _on_stuff(self, callback):             # <<<<<<<<<<<<<<
  *         if self._value is NONE:
  *             if self._cb is None:
  */
 
@@ -8539,15 +8601,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_on_stuff", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__on_stuff(__pyx_v_self, __pyx_v_callback, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 304, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__on_stuff(__pyx_v_self, __pyx_v_callback, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8556,15 +8618,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":313
+/* "chorde/clients/_async.pyx":325
  *         return self
  * 
  *     def add_done_callback(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operatio is done, the callback will be invoked with the
  */
 
@@ -8588,41 +8650,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_done_callback", 0);
 
-  /* "chorde/clients/_async.pyx":318
+  /* "chorde/clients/_async.pyx":330
  *         future object as argument.
  *         """
  *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))             # <<<<<<<<<<<<<<
  * 
  *     cdef int c_done(self) except -1:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 318, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_self));
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_WeakCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_WeakCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 318, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_WeakCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_WeakCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 318, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":313
+  /* "chorde/clients/_async.pyx":325
  *         return self
  * 
  *     def add_done_callback(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operatio is done, the callback will be invoked with the
  */
 
@@ -8634,15 +8696,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":320
+/* "chorde/clients/_async.pyx":332
  *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
  * 
  *     cdef int c_done(self) except -1:             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
@@ -8650,15 +8712,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   __Pyx_RefNannySetupContext("c_done", 0);
 
-  /* "chorde/clients/_async.pyx":324
+  /* "chorde/clients/_async.pyx":336
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self._value is not NONE or self._cancelled:             # <<<<<<<<<<<<<<
  *             return 1
  *         else:
  */
   __pyx_t_2 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
@@ -8669,60 +8731,60 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = (__pyx_v_self->_cancelled != 0);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":325
+    /* "chorde/clients/_async.pyx":337
  *         """
  *         if self._value is not NONE or self._cancelled:
  *             return 1             # <<<<<<<<<<<<<<
  *         else:
  *             return 0
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":324
+    /* "chorde/clients/_async.pyx":336
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self._value is not NONE or self._cancelled:             # <<<<<<<<<<<<<<
  *             return 1
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":327
+  /* "chorde/clients/_async.pyx":339
  *             return 1
  *         else:
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     def done(self):
  */
   /*else*/ {
     __pyx_r = 0;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":320
+  /* "chorde/clients/_async.pyx":332
  *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
  * 
  *     cdef int c_done(self) except -1:             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":329
+/* "chorde/clients/_async.pyx":341
  *             return 0
  * 
  *     def done(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
@@ -8746,61 +8808,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("done", 0);
 
-  /* "chorde/clients/_async.pyx":333
+  /* "chorde/clients/_async.pyx":345
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self.c_done():             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_done(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 333, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_done(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 345, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":334
+    /* "chorde/clients/_async.pyx":346
  *         """
  *         if self.c_done():
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":333
+    /* "chorde/clients/_async.pyx":345
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self.c_done():             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":336
+  /* "chorde/clients/_async.pyx":348
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def running(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":329
+  /* "chorde/clients/_async.pyx":341
  *             return 0
  * 
  *     def done(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
@@ -8810,15 +8872,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":338
+/* "chorde/clients/_async.pyx":350
  *             return False
  * 
  *     def running(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation is running and cannot be cancelled. False if not running
  */
 
@@ -8838,75 +8900,75 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_40running(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("running", 0);
 
-  /* "chorde/clients/_async.pyx":343
+  /* "chorde/clients/_async.pyx":355
  *         (yet or done).
  *         """
  *         if self._running:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_running != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":344
+    /* "chorde/clients/_async.pyx":356
  *         """
  *         if self._running:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":343
+    /* "chorde/clients/_async.pyx":355
  *         (yet or done).
  *         """
  *         if self._running:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":346
+  /* "chorde/clients/_async.pyx":358
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def cancelled(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":338
+  /* "chorde/clients/_async.pyx":350
  *             return False
  * 
  *     def running(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation is running and cannot be cancelled. False if not running
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":348
+/* "chorde/clients/_async.pyx":360
  *             return False
  * 
  *     def cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has been cancelled successfully.
  */
 
@@ -8926,75 +8988,75 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_42cancelled(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("cancelled", 0);
 
-  /* "chorde/clients/_async.pyx":352
+  /* "chorde/clients/_async.pyx":364
  *         Return True if the operation has been cancelled successfully.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_cancelled != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":353
+    /* "chorde/clients/_async.pyx":365
  *         """
  *         if self._cancelled:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":352
+    /* "chorde/clients/_async.pyx":364
  *         Return True if the operation has been cancelled successfully.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":355
+  /* "chorde/clients/_async.pyx":367
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def cancel_pending(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":348
+  /* "chorde/clients/_async.pyx":360
  *             return False
  * 
  *     def cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has been cancelled successfully.
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":357
+/* "chorde/clients/_async.pyx":369
  *             return False
  * 
  *     def cancel_pending(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if cancel was called.
  */
 
@@ -9014,75 +9076,75 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_44cancel_pending(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("cancel_pending", 0);
 
-  /* "chorde/clients/_async.pyx":361
+  /* "chorde/clients/_async.pyx":373
  *         Return True if cancel was called.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_cancel_pending != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":362
+    /* "chorde/clients/_async.pyx":374
  *         """
  *         if self._cancel_pending:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":361
+    /* "chorde/clients/_async.pyx":373
  *         Return True if cancel was called.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":364
+  /* "chorde/clients/_async.pyx":376
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def cancel(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":357
+  /* "chorde/clients/_async.pyx":369
  *             return False
  * 
  *     def cancel_pending(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if cancel was called.
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":366
+/* "chorde/clients/_async.pyx":378
  *             return False
  * 
  *     def cancel(self):             # <<<<<<<<<<<<<<
  *         """
  *         Request cancelling of the operation. If the operation cannot be cancelled,
  */
 
@@ -9102,84 +9164,84 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_46cancel(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("cancel", 0);
 
-  /* "chorde/clients/_async.pyx":371
+  /* "chorde/clients/_async.pyx":383
  *         it will return False. Otherwise, it will return True.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return False
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_cancelled != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":372
+    /* "chorde/clients/_async.pyx":384
  *         """
  *         if self._cancelled:
  *             return False             # <<<<<<<<<<<<<<
  *         else:
  *             self._cancel_pending = 1
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":371
+    /* "chorde/clients/_async.pyx":383
  *         it will return False. Otherwise, it will return True.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return False
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":374
+  /* "chorde/clients/_async.pyx":386
  *             return False
  *         else:
  *             self._cancel_pending = 1             # <<<<<<<<<<<<<<
  *             return True
  * 
  */
   /*else*/ {
     __pyx_v_self->_cancel_pending = 1;
 
-    /* "chorde/clients/_async.pyx":375
+    /* "chorde/clients/_async.pyx":387
  *         else:
  *             self._cancel_pending = 1
  *             return True             # <<<<<<<<<<<<<<
  * 
  *     def set_running_or_notify_cancelled(self):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":366
+  /* "chorde/clients/_async.pyx":378
  *             return False
  * 
  *     def cancel(self):             # <<<<<<<<<<<<<<
  *         """
  *         Request cancelling of the operation. If the operation cannot be cancelled,
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":377
+/* "chorde/clients/_async.pyx":389
  *             return True
  * 
  *     def set_running_or_notify_cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         To be invoked by executors before executing the operation. If it returns True,
  */
 
@@ -9207,65 +9269,65 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_running_or_notify_cancelled", 0);
 
-  /* "chorde/clients/_async.pyx":384
+  /* "chorde/clients/_async.pyx":396
  *         be wakened immediately and the future will be marked as cancelled.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             self._cancelled = 1
  *             self._running = 0
  */
   __pyx_t_1 = (__pyx_v_self->_cancel_pending != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":385
+    /* "chorde/clients/_async.pyx":397
  *         """
  *         if self._cancel_pending:
  *             self._cancelled = 1             # <<<<<<<<<<<<<<
  *             self._running = 0
  * 
  */
     __pyx_v_self->_cancelled = 1;
 
-    /* "chorde/clients/_async.pyx":386
+    /* "chorde/clients/_async.pyx":398
  *         if self._cancel_pending:
  *             self._cancelled = 1
  *             self._running = 0             # <<<<<<<<<<<<<<
  * 
  *             # Notify waiters and callbacks
  */
     __pyx_v_self->_running = 0;
 
-    /* "chorde/clients/_async.pyx":389
+    /* "chorde/clients/_async.pyx":401
  * 
  *             # Notify waiters and callbacks
  *             self.set_exception(CancelledError())             # <<<<<<<<<<<<<<
  * 
  *             return False
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_exception); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 389, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_exception); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
     __pyx_t_5 = __pyx_v_6chorde_7clients_6_async_CancelledError; __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 389, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -9273,64 +9335,64 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 389, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "chorde/clients/_async.pyx":391
+    /* "chorde/clients/_async.pyx":403
  *             self.set_exception(CancelledError())
  * 
  *             return False             # <<<<<<<<<<<<<<
  *         else:
  *             self._running = 1
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":384
+    /* "chorde/clients/_async.pyx":396
  *         be wakened immediately and the future will be marked as cancelled.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             self._cancelled = 1
  *             self._running = 0
  */
   }
 
-  /* "chorde/clients/_async.pyx":393
+  /* "chorde/clients/_async.pyx":405
  *             return False
  *         else:
  *             self._running = 1             # <<<<<<<<<<<<<<
  *             return True
  * 
  */
   /*else*/ {
     __pyx_v_self->_running = 1;
 
-    /* "chorde/clients/_async.pyx":394
+    /* "chorde/clients/_async.pyx":406
  *         else:
  *             self._running = 1
  *             return True             # <<<<<<<<<<<<<<
  * 
  *     cdef c_result(self, timeout, int norecurse):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":377
+  /* "chorde/clients/_async.pyx":389
  *             return True
  * 
  *     def set_running_or_notify_cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         To be invoked by executors before executing the operation. If it returns True,
  */
 
@@ -9345,15 +9407,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":396
+/* "chorde/clients/_async.pyx":408
  *             return True
  * 
  *     cdef c_result(self, timeout, int norecurse):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -9379,84 +9441,84 @@
   PyObject *__pyx_t_15 = NULL;
   int __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("c_result", 0);
 
-  /* "chorde/clients/_async.pyx":405
+  /* "chorde/clients/_async.pyx":417
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
   __pyx_t_1 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":406
+    /* "chorde/clients/_async.pyx":418
  * 
  *         if self._value is not NONE:
  *             value = self._value             # <<<<<<<<<<<<<<
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  */
     __pyx_t_3 = __pyx_v_self->_value;
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_value = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "chorde/clients/_async.pyx":407
+    /* "chorde/clients/_async.pyx":419
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 try:
  */
     __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":408
+      /* "chorde/clients/_async.pyx":420
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value             # <<<<<<<<<<<<<<
  *                 try:
  *                     exc_value.reraise(False)
  */
       __pyx_t_3 = __pyx_v_value;
       __Pyx_INCREF(__pyx_t_3);
       __pyx_v_exc_value = ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "chorde/clients/_async.pyx":409
+      /* "chorde/clients/_async.pyx":421
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  *                 try:             # <<<<<<<<<<<<<<
  *                     exc_value.reraise(False)
  *                 finally:
  */
       /*try:*/ {
 
-        /* "chorde/clients/_async.pyx":410
+        /* "chorde/clients/_async.pyx":422
  *                 exc_value = <ExceptionWrapper>value
  *                 try:
  *                     exc_value.reraise(False)             # <<<<<<<<<<<<<<
  *                 finally:
  *                     del exc_value, value
  */
         __pyx_t_4.__pyx_n = 1;
         __pyx_t_4.strip = 0;
-        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_exc_value->__pyx_vtab)->reraise(__pyx_v_exc_value, 0, &__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 410, __pyx_L6_error)
+        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_exc_value->__pyx_vtab)->reraise(__pyx_v_exc_value, 0, &__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
 
-      /* "chorde/clients/_async.pyx":412
+      /* "chorde/clients/_async.pyx":424
  *                     exc_value.reraise(False)
  *                 finally:
  *                     del exc_value, value             # <<<<<<<<<<<<<<
  *             elif value is CacheMissError:
  *                 raise CacheMissError()
  */
       /*finally:*/ {
@@ -9501,36 +9563,36 @@
           __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0;
           __pyx_lineno = __pyx_t_5; __pyx_clineno = __pyx_t_6; __pyx_filename = __pyx_t_7;
           goto __pyx_L1_error;
         }
         __pyx_L7:;
       }
 
-      /* "chorde/clients/_async.pyx":407
+      /* "chorde/clients/_async.pyx":419
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 try:
  */
       goto __pyx_L4;
     }
 
-    /* "chorde/clients/_async.pyx":413
+    /* "chorde/clients/_async.pyx":425
  *                 finally:
  *                     del exc_value, value
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 raise CacheMissError()
  *             else:
  */
     __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "chorde/clients/_async.pyx":414
+      /* "chorde/clients/_async.pyx":426
  *                     del exc_value, value
  *             elif value is CacheMissError:
  *                 raise CacheMissError()             # <<<<<<<<<<<<<<
  *             else:
  *                 return value
  */
       __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
@@ -9542,66 +9604,66 @@
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_14, function);
         }
       }
       __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 414, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 414, __pyx_L1_error)
+      __PYX_ERR(0, 426, __pyx_L1_error)
 
-      /* "chorde/clients/_async.pyx":413
+      /* "chorde/clients/_async.pyx":425
  *                 finally:
  *                     del exc_value, value
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 raise CacheMissError()
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":416
+    /* "chorde/clients/_async.pyx":428
  *                 raise CacheMissError()
  *             else:
  *                 return value             # <<<<<<<<<<<<<<
  *         elif self._cancelled:
  *             raise CancelledError()
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_value);
       __pyx_r = __pyx_v_value;
       goto __pyx_L0;
     }
     __pyx_L4:;
 
-    /* "chorde/clients/_async.pyx":405
+    /* "chorde/clients/_async.pyx":417
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":417
+  /* "chorde/clients/_async.pyx":429
  *             else:
  *                 return value
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   __pyx_t_2 = (__pyx_v_self->_cancelled != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "chorde/clients/_async.pyx":418
+    /* "chorde/clients/_async.pyx":430
  *                 return value
  *         elif self._cancelled:
  *             raise CancelledError()             # <<<<<<<<<<<<<<
  *         else:
  *             if timeout is not None and timeout == 0:
  */
     __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
@@ -9613,54 +9675,54 @@
         __Pyx_INCREF(__pyx_t_15);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_14, function);
       }
     }
     __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
     __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 418, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 418, __pyx_L1_error)
+    __PYX_ERR(0, 430, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":417
+    /* "chorde/clients/_async.pyx":429
  *             else:
  *                 return value
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":420
+  /* "chorde/clients/_async.pyx":432
  *             raise CancelledError()
  *         else:
  *             if timeout is not None and timeout == 0:             # <<<<<<<<<<<<<<
  *                 raise TimeoutError()
  *             else:
  */
   /*else*/ {
     __pyx_t_1 = (__pyx_v_timeout != Py_None);
     __pyx_t_16 = (__pyx_t_1 != 0);
     if (__pyx_t_16) {
     } else {
       __pyx_t_2 = __pyx_t_16;
       goto __pyx_L11_bool_binop_done;
     }
-    __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_v_timeout, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_v_timeout, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_2 = __pyx_t_16;
     __pyx_L11_bool_binop_done:;
     if (unlikely(__pyx_t_2)) {
 
-      /* "chorde/clients/_async.pyx":421
+      /* "chorde/clients/_async.pyx":433
  *         else:
  *             if timeout is not None and timeout == 0:
  *                 raise TimeoutError()             # <<<<<<<<<<<<<<
  *             else:
  *                 # Wait for it
  */
       __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_TimeoutError);
@@ -9672,85 +9734,85 @@
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_14, function);
         }
       }
       __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 421, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 421, __pyx_L1_error)
+      __PYX_ERR(0, 433, __pyx_L1_error)
 
-      /* "chorde/clients/_async.pyx":420
+      /* "chorde/clients/_async.pyx":432
  *             raise CancelledError()
  *         else:
  *             if timeout is not None and timeout == 0:             # <<<<<<<<<<<<<<
  *                 raise TimeoutError()
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":424
+    /* "chorde/clients/_async.pyx":436
  *             else:
  *                 # Wait for it
  *                 if self._done_event is None:             # <<<<<<<<<<<<<<
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_self->_done_event == Py_None);
       __pyx_t_16 = (__pyx_t_2 != 0);
       if (__pyx_t_16) {
 
-        /* "chorde/clients/_async.pyx":425
+        /* "chorde/clients/_async.pyx":437
  *                 # Wait for it
  *                 if self._done_event is None:
  *                     self._done_event = threading.Event()             # <<<<<<<<<<<<<<
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_threading); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 425, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_threading); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 437, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_Event); if (unlikely(!__pyx_t_15)) __PYX_ERR(1, 425, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_Event); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 437, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_t_14 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
           __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_15);
           if (likely(__pyx_t_14)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 425, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 437, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_GIVEREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_v_self->_done_event);
         __Pyx_DECREF(__pyx_v_self->_done_event);
         __pyx_v_self->_done_event = __pyx_t_3;
         __pyx_t_3 = 0;
 
-        /* "chorde/clients/_async.pyx":424
+        /* "chorde/clients/_async.pyx":436
  *             else:
  *                 # Wait for it
  *                 if self._done_event is None:             # <<<<<<<<<<<<<<
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  */
       }
 
-      /* "chorde/clients/_async.pyx":426
+      /* "chorde/clients/_async.pyx":438
  *                 if self._done_event is None:
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):             # <<<<<<<<<<<<<<
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:
  */
       __pyx_t_2 = ((!(__pyx_v_norecurse != 0)) != 0);
@@ -9762,71 +9824,71 @@
       __pyx_t_2 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
       __pyx_t_1 = (__pyx_t_2 != 0);
       if (!__pyx_t_1) {
       } else {
         __pyx_t_16 = __pyx_t_1;
         goto __pyx_L15_bool_binop_done;
       }
-      __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_wait); if (unlikely(!__pyx_t_15)) __PYX_ERR(1, 426, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_wait); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 438, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __pyx_t_14 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
         __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_15);
         if (likely(__pyx_t_14)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
           __Pyx_INCREF(__pyx_t_14);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_15, function);
         }
       }
       __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_14, __pyx_v_timeout) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_v_timeout);
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 426, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 426, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 438, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_16 = __pyx_t_1;
       __pyx_L15_bool_binop_done:;
       if (__pyx_t_16) {
 
-        /* "chorde/clients/_async.pyx":427
+        /* "chorde/clients/_async.pyx":439
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)             # <<<<<<<<<<<<<<
  *                 elif self._cancelled:
  *                     raise CancelledError()
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_int_0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 427, __pyx_L1_error)
+        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_int_0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_r = __pyx_t_3;
         __pyx_t_3 = 0;
         goto __pyx_L0;
 
-        /* "chorde/clients/_async.pyx":426
+        /* "chorde/clients/_async.pyx":438
  *                 if self._done_event is None:
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):             # <<<<<<<<<<<<<<
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:
  */
       }
 
-      /* "chorde/clients/_async.pyx":428
+      /* "chorde/clients/_async.pyx":440
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:             # <<<<<<<<<<<<<<
  *                     raise CancelledError()
  *                 else:
  */
       __pyx_t_16 = (__pyx_v_self->_cancelled != 0);
       if (unlikely(__pyx_t_16)) {
 
-        /* "chorde/clients/_async.pyx":429
+        /* "chorde/clients/_async.pyx":441
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:
  *                     raise CancelledError()             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise TimeoutError()
  */
         __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
@@ -9838,31 +9900,31 @@
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 429, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(1, 429, __pyx_L1_error)
+        __PYX_ERR(0, 441, __pyx_L1_error)
 
-        /* "chorde/clients/_async.pyx":428
+        /* "chorde/clients/_async.pyx":440
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:             # <<<<<<<<<<<<<<
  *                     raise CancelledError()
  *                 else:
  */
       }
 
-      /* "chorde/clients/_async.pyx":431
+      /* "chorde/clients/_async.pyx":443
  *                     raise CancelledError()
  *                 else:
  *                     raise TimeoutError()             # <<<<<<<<<<<<<<
  * 
  *     def result(self, timeout=None, norecurse=False):
  */
       /*else*/ {
@@ -9875,26 +9937,26 @@
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 431, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 443, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(1, 431, __pyx_L1_error)
+        __PYX_ERR(0, 443, __pyx_L1_error)
       }
     }
   }
   __pyx_L3:;
 
-  /* "chorde/clients/_async.pyx":396
+  /* "chorde/clients/_async.pyx":408
  *             return True
  * 
  *     cdef c_result(self, timeout, int norecurse):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -9911,15 +9973,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XDECREF((PyObject *)__pyx_v_exc_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":433
+/* "chorde/clients/_async.pyx":445
  *                     raise TimeoutError()
  * 
  *     def result(self, timeout=None, norecurse=False):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -9962,15 +10024,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_norecurse);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "result") < 0)) __PYX_ERR(1, 433, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "result") < 0)) __PYX_ERR(0, 445, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -9979,15 +10041,15 @@
       }
     }
     __pyx_v_timeout = values[0];
     __pyx_v_norecurse = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("result", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 433, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("result", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 445, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.result", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_50result(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_timeout, __pyx_v_norecurse);
 
@@ -10002,30 +10064,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("result", 0);
 
-  /* "chorde/clients/_async.pyx":439
+  /* "chorde/clients/_async.pyx":451
  *         and the specified time elapses without a result available, raises TimeoutError.
  *         """
  *         return self.c_result(timeout, norecurse)             # <<<<<<<<<<<<<<
  * 
  *     def exception(self, timeout=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_norecurse); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 439, __pyx_L1_error)
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 439, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_norecurse); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 451, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":433
+  /* "chorde/clients/_async.pyx":445
  *                     raise TimeoutError()
  * 
  *     def result(self, timeout=None, norecurse=False):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -10036,15 +10098,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":441
+/* "chorde/clients/_async.pyx":453
  *         return self.c_result(timeout, norecurse)
  * 
  *     def exception(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation resulted in an exception, return the exception object.
  */
 
@@ -10077,29 +10139,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "exception") < 0)) __PYX_ERR(1, 441, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "exception") < 0)) __PYX_ERR(0, 453, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_timeout = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("exception", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 441, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("exception", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 453, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_52exception(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_timeout);
 
@@ -10125,163 +10187,163 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exception", 0);
 
-  /* "chorde/clients/_async.pyx":451
+  /* "chorde/clients/_async.pyx":463
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
   __pyx_t_1 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":452
+    /* "chorde/clients/_async.pyx":464
  * 
  *         if self._value is not NONE:
  *             value = self._value             # <<<<<<<<<<<<<<
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  */
     __pyx_t_3 = __pyx_v_self->_value;
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_value = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "chorde/clients/_async.pyx":453
+    /* "chorde/clients/_async.pyx":465
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  */
     __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":454
+      /* "chorde/clients/_async.pyx":466
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value             # <<<<<<<<<<<<<<
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:
  */
       __pyx_t_3 = __pyx_v_value;
       __Pyx_INCREF(__pyx_t_3);
       __pyx_v_exc_value = ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "chorde/clients/_async.pyx":455
+      /* "chorde/clients/_async.pyx":467
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]             # <<<<<<<<<<<<<<
  *             elif value is CacheMissError:
  *                 return CacheMissError
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 455, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 455, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 467, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else {
         __Pyx_INCREF(__pyx_t_4);
         __pyx_t_3 = __pyx_t_4;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         goto __pyx_L5_bool_binop_done;
       }
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 455, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_3 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_L5_bool_binop_done:;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":453
+      /* "chorde/clients/_async.pyx":465
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  */
     }
 
-    /* "chorde/clients/_async.pyx":456
+    /* "chorde/clients/_async.pyx":468
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 return CacheMissError
  *             else:
  */
     __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "chorde/clients/_async.pyx":457
+      /* "chorde/clients/_async.pyx":469
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:
  *                 return CacheMissError             # <<<<<<<<<<<<<<
  *             else:
  *                 return None
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
       __pyx_r = __pyx_v_6chorde_7clients_6_async_CacheMissError;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":456
+      /* "chorde/clients/_async.pyx":468
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 return CacheMissError
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":459
+    /* "chorde/clients/_async.pyx":471
  *                 return CacheMissError
  *             else:
  *                 return None             # <<<<<<<<<<<<<<
  *         elif self._cancelled:
  *             raise CancelledError()
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L0;
     }
 
-    /* "chorde/clients/_async.pyx":451
+    /* "chorde/clients/_async.pyx":463
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
   }
 
-  /* "chorde/clients/_async.pyx":460
+  /* "chorde/clients/_async.pyx":472
  *             else:
  *                 return None
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   __pyx_t_2 = (__pyx_v_self->_cancelled != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "chorde/clients/_async.pyx":461
+    /* "chorde/clients/_async.pyx":473
  *                 return None
  *         elif self._cancelled:
  *             raise CancelledError()             # <<<<<<<<<<<<<<
  *         else:
  *             try:
  */
     __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
@@ -10293,31 +10355,31 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 461, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 461, __pyx_L1_error)
+    __PYX_ERR(0, 473, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":460
+    /* "chorde/clients/_async.pyx":472
  *             else:
  *                 return None
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":463
+  /* "chorde/clients/_async.pyx":475
  *             raise CancelledError()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.c_result(timeout, 0)
  *                 return None
  */
   /*else*/ {
@@ -10326,106 +10388,106 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_8);
       /*try:*/ {
 
-        /* "chorde/clients/_async.pyx":464
+        /* "chorde/clients/_async.pyx":476
  *         else:
  *             try:
  *                 self.c_result(timeout, 0)             # <<<<<<<<<<<<<<
  *                 return None
  *             except CancelledError:
  */
-        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 464, __pyx_L7_error)
+        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 476, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "chorde/clients/_async.pyx":465
+        /* "chorde/clients/_async.pyx":477
  *             try:
  *                 self.c_result(timeout, 0)
  *                 return None             # <<<<<<<<<<<<<<
  *             except CancelledError:
  *                 raise
  */
         __Pyx_XDECREF(__pyx_r);
         __pyx_r = Py_None; __Pyx_INCREF(Py_None);
         goto __pyx_L11_try_return;
 
-        /* "chorde/clients/_async.pyx":463
+        /* "chorde/clients/_async.pyx":475
  *             raise CancelledError()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.c_result(timeout, 0)
  *                 return None
  */
       }
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "chorde/clients/_async.pyx":466
+      /* "chorde/clients/_async.pyx":478
  *                 self.c_result(timeout, 0)
  *                 return None
  *             except CancelledError:             # <<<<<<<<<<<<<<
  *                 raise
  *             except Exception as e:
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_v_6chorde_7clients_6_async_CancelledError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("chorde.clients._async.Future.exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(1, 466, __pyx_L9_except_error)
+        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 478, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GOTREF(__pyx_t_5);
 
-        /* "chorde/clients/_async.pyx":467
+        /* "chorde/clients/_async.pyx":479
  *                 return None
  *             except CancelledError:
  *                 raise             # <<<<<<<<<<<<<<
  *             except Exception as e:
  *                 try:
  */
         __Pyx_GIVEREF(__pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_4);
         __Pyx_XGIVEREF(__pyx_t_5);
         __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_4, __pyx_t_5);
         __pyx_t_3 = 0; __pyx_t_4 = 0; __pyx_t_5 = 0; 
-        __PYX_ERR(1, 467, __pyx_L9_except_error)
+        __PYX_ERR(0, 479, __pyx_L9_except_error)
       }
 
-      /* "chorde/clients/_async.pyx":468
+      /* "chorde/clients/_async.pyx":480
  *             except CancelledError:
  *                 raise
  *             except Exception as e:             # <<<<<<<<<<<<<<
  *                 try:
  *                     return e
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_9) {
         __Pyx_AddTraceback("chorde.clients._async.Future.exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_3) < 0) __PYX_ERR(1, 468, __pyx_L9_except_error)
+        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_3) < 0) __PYX_ERR(0, 480, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __pyx_v_e = __pyx_t_4;
 
-        /* "chorde/clients/_async.pyx":469
+        /* "chorde/clients/_async.pyx":481
  *                 raise
  *             except Exception as e:
  *                 try:             # <<<<<<<<<<<<<<
  *                     return e
  *                 finally:
  */
         /*try:*/ {
 
-          /* "chorde/clients/_async.pyx":470
+          /* "chorde/clients/_async.pyx":482
  *             except Exception as e:
  *                 try:
  *                     return e             # <<<<<<<<<<<<<<
  *                 finally:
  *                     del e
  */
           __Pyx_XDECREF(__pyx_r);
@@ -10433,15 +10495,15 @@
           __pyx_r = __pyx_v_e;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           goto __pyx_L19_return;
         }
 
-        /* "chorde/clients/_async.pyx":472
+        /* "chorde/clients/_async.pyx":484
  *                     return e
  *                 finally:
  *                     del e             # <<<<<<<<<<<<<<
  * 
  */
         /*finally:*/ {
           __pyx_L19_return: {
@@ -10454,15 +10516,15 @@
             goto __pyx_L10_except_return;
           }
         }
       }
       goto __pyx_L9_except_error;
       __pyx_L9_except_error:;
 
-      /* "chorde/clients/_async.pyx":463
+      /* "chorde/clients/_async.pyx":475
  *             raise CancelledError()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.c_result(timeout, 0)
  *                 return None
  */
       __Pyx_XGIVEREF(__pyx_t_6);
@@ -10481,15 +10543,15 @@
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_XGIVEREF(__pyx_t_8);
       __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
       goto __pyx_L0;
     }
   }
 
-  /* "chorde/clients/_async.pyx":441
+  /* "chorde/clients/_async.pyx":453
  *         return self.c_result(timeout, norecurse)
  * 
  *     def exception(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation resulted in an exception, return the exception object.
  */
 
@@ -10539,19 +10601,19 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 2, __pyx_L1_error)
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -10595,19 +10657,19 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 4, __pyx_L1_error)
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -10662,40 +10724,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_NONE", 1, 3, 3, 1); __PYX_ERR(0, 1, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_NONE", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_NONE", 1, 3, 3, 2); __PYX_ERR(0, 1, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_NONE", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_NONE") < 0)) __PYX_ERR(0, 1, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_NONE") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v___pyx_type = values[0];
-    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L3_error)
+    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_NONE", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_NONE", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.__pyx_unpickle_NONE", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_2__pyx_unpickle_NONE(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
@@ -10723,53 +10785,53 @@
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__20, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__20, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = NONE.__new__(__pyx_type)
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
-    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 5, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v___pyx_PickleError = __pyx_t_1;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = NONE.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 6, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
     __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_6)) {
@@ -10778,20 +10840,20 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 6, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 6, __pyx_L1_error)
+    __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
@@ -10801,29 +10863,29 @@
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = NONE.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NONE__set_state(<NONE> __pyx_result, __pyx_state)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
@@ -10839,16 +10901,16 @@
     /* "(tree fragment)":9
  *     __pyx_result = NONE.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NONE__set_state(<NONE> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_NONE__set_state(NONE __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 9, __pyx_L1_error)
-    __pyx_t_4 = __pyx_f_6chorde_7clients_6_async___pyx_unpickle_NONE__set_state(((struct __pyx_obj_6chorde_7clients_6_async_NONE *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6chorde_7clients_6_async___pyx_unpickle_NONE__set_state(((struct __pyx_obj_6chorde_7clients_6_async_NONE *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = NONE.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
@@ -10919,59 +10981,59 @@
  *     return __pyx_result
  * cdef __pyx_unpickle_NONE__set_state(NONE __pyx_result, tuple __pyx_state):
  *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
  *         __pyx_result.__dict__.update(__pyx_state[0])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 12, __pyx_L1_error)
+    __PYX_ERR(1, 12, __pyx_L1_error)
   }
-  __pyx_t_2 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 12, __pyx_L1_error)
   __pyx_t_3 = ((__pyx_t_2 > 0) != 0);
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 12, __pyx_L1_error)
   __pyx_t_4 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
     /* "(tree fragment)":13
  * cdef __pyx_unpickle_NONE__set_state(NONE __pyx_result, tuple __pyx_state):
  *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[0])             # <<<<<<<<<<<<<<
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_v___pyx_state == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 13, __pyx_L1_error)
+      __PYX_ERR(1, 13, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 13, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_NONE__set_state(NONE __pyx_result, tuple __pyx_state):
@@ -12520,14 +12582,16 @@
   {&__pyx_n_s_DeferExceptionCallback, __pyx_k_DeferExceptionCallback, sizeof(__pyx_k_DeferExceptionCallback), 0, 0, 1, 1},
   {&__pyx_n_s_DoneCallback, __pyx_k_DoneCallback, sizeof(__pyx_k_DoneCallback), 0, 0, 1, 1},
   {&__pyx_kp_s_Error_in_async_callback, __pyx_k_Error_in_async_callback, sizeof(__pyx_k_Error_in_async_callback), 0, 0, 1, 0},
   {&__pyx_n_s_Event, __pyx_k_Event, sizeof(__pyx_k_Event), 0, 0, 1, 1},
   {&__pyx_n_s_ExceptionCallback, __pyx_k_ExceptionCallback, sizeof(__pyx_k_ExceptionCallback), 0, 0, 1, 1},
   {&__pyx_n_s_ExceptionWrapper, __pyx_k_ExceptionWrapper, sizeof(__pyx_k_ExceptionWrapper), 0, 0, 1, 1},
   {&__pyx_n_s_Future, __pyx_k_Future, sizeof(__pyx_k_Future), 0, 0, 1, 1},
+  {&__pyx_n_s_HTTPError, __pyx_k_HTTPError, sizeof(__pyx_k_HTTPError), 0, 0, 1, 1},
+  {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_MissCallback, __pyx_k_MissCallback, sizeof(__pyx_k_MissCallback), 0, 0, 1, 1},
   {&__pyx_n_s_NONE, __pyx_k_NONE, sizeof(__pyx_k_NONE), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_TimeoutError, __pyx_k_TimeoutError, sizeof(__pyx_k_TimeoutError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_ValueCallback, __pyx_k_ValueCallback, sizeof(__pyx_k_ValueCallback), 0, 0, 1, 1},
@@ -12565,14 +12629,15 @@
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_NONE, __pyx_k_pyx_unpickle_NONE, sizeof(__pyx_k_pyx_unpickle_NONE), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
+  {&__pyx_n_s_reason, __pyx_k_reason, sizeof(__pyx_k_reason), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_ref, __pyx_k_ref, sizeof(__pyx_k_ref), 0, 0, 1, 1},
   {&__pyx_n_s_reraise, __pyx_k_reraise, sizeof(__pyx_k_reraise), 0, 0, 1, 1},
   {&__pyx_n_s_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
   {&__pyx_n_s_set_exception, __pyx_k_set_exception, sizeof(__pyx_k_set_exception), 0, 0, 1, 1},
@@ -12582,24 +12647,26 @@
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_strip, __pyx_k_strip, sizeof(__pyx_k_strip), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_threading, __pyx_k_threading, sizeof(__pyx_k_threading), 0, 0, 1, 1},
   {&__pyx_n_s_timeout, __pyx_k_timeout, sizeof(__pyx_k_timeout), 0, 0, 1, 1},
+  {&__pyx_n_s_tornado_web, __pyx_k_tornado_web, sizeof(__pyx_k_tornado_web), 0, 0, 1, 1},
   {&__pyx_n_s_traceback, __pyx_k_traceback, sizeof(__pyx_k_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_wait, __pyx_k_wait, sizeof(__pyx_k_wait), 0, 0, 1, 1},
   {&__pyx_n_s_weakref, __pyx_k_weakref, sizeof(__pyx_k_weakref), 0, 0, 1, 1},
   {&__pyx_n_s_with_traceback, __pyx_k_with_traceback, sizeof(__pyx_k_with_traceback), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -12607,227 +12674,227 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "chorde/clients/_async.pyx":193
+  /* "chorde/clients/_async.pyx":205
  *                     else:
  *                         error = logging.error
  *                     error("Error in async callback", exc_info = True)             # <<<<<<<<<<<<<<
  * 
  *     cpdef set(self, value):
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Error_in_async_callback); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Error_in_async_callback); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_tuple__20 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "chorde/clients/_async.pyx":22
+  /* "chorde/clients/_async.pyx":29
  * 
  * 
  * def set_strip_tracebacks(bint strip):             # <<<<<<<<<<<<<<
  *     """ Sets traceback stripping behavior for async futures
  * 
  */
-  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_strip, __pyx_n_s_strip); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 22, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_strip, __pyx_n_s_strip); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_chorde_clients__async_pyx, __pyx_n_s_set_strip_tracebacks, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 22, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_chorde_clients__async_pyx, __pyx_n_s_set_strip_tracebacks, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 29, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_NONE(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__23 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_NONE, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_NONE, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_int_228825662 = PyInt_FromLong(228825662L); if (unlikely(!__pyx_int_228825662)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_int_238750788 = PyInt_FromLong(238750788L); if (unlikely(!__pyx_int_238750788)) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_228825662 = PyInt_FromLong(228825662L); if (unlikely(!__pyx_int_228825662)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_238750788 = PyInt_FromLong(238750788L); if (unlikely(!__pyx_int_238750788)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -12842,14 +12909,15 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_global_init_code", 0);
   /*--- Global init code ---*/
   __pyx_v_6chorde_7clients_6_async_CacheMissError = Py_None; Py_INCREF(Py_None);
   __pyx_v_6chorde_7clients_6_async_CancelledError = Py_None; Py_INCREF(Py_None);
   __pyx_v_6chorde_7clients_6_async_TimeoutError = Py_None; Py_INCREF(Py_None);
   __pyx_v_6chorde_7clients_6_async_wref = Py_None; Py_INCREF(Py_None);
   __pyx_v_6chorde_7clients_6_async_functools_partial = Py_None; Py_INCREF(Py_None);
+  __pyx_v_6chorde_7clients_6_async__HTTPError = Py_None; Py_INCREF(Py_None);
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_variable_export_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_export_code", 0);
@@ -12875,126 +12943,126 @@
   /*--- Type init code ---*/
   __pyx_vtabptr_6chorde_7clients_6_async_Future = &__pyx_vtable_6chorde_7clients_6_async_Future;
   __pyx_vtable_6chorde_7clients_6_async_Future.c_done = (int (*)(struct __pyx_obj_6chorde_7clients_6_async_Future *))__pyx_f_6chorde_7clients_6_async_6Future_c_done;
   __pyx_vtable_6chorde_7clients_6_async_Future.c_result = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int))__pyx_f_6chorde_7clients_6_async_6Future_c_result;
   __pyx_vtable_6chorde_7clients_6_async_Future._set_nothreads = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6chorde_7clients_6_async_6Future__set_nothreads;
   __pyx_vtable_6chorde_7clients_6_async_Future.set = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6chorde_7clients_6_async_6Future_set;
   __pyx_vtable_6chorde_7clients_6_async_Future._on_stuff = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6chorde_7clients_6_async_6Future__on_stuff;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(1, 149, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_Future.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_Future.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_Future.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_Future.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_Future.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(1, 149, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Future, (PyObject *)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(1, 149, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_Future.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Future, (PyObject *)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_Future.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_Future.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_Future, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(1, 149, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_Future = &__pyx_type_6chorde_7clients_6_async_Future;
   __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper = &__pyx_vtable_6chorde_7clients_6_async_ExceptionWrapper;
   __pyx_vtable_6chorde_7clients_6_async_ExceptionWrapper.reraise = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *, int __pyx_skip_dispatch, struct __pyx_opt_args_6chorde_7clients_6_async_16ExceptionWrapper_reraise *__pyx_optional_args))__pyx_f_6chorde_7clients_6_async_16ExceptionWrapper_reraise;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(1, 35, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(1, 35, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionWrapper, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(1, 35, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionWrapper, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(1, 35, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper = &__pyx_type_6chorde_7clients_6_async_ExceptionWrapper;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(1, 71, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_WeakCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_WeakCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(1, 71, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_WeakCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_WeakCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_WeakCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(1, 71, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_WeakCallback = &__pyx_type_6chorde_7clients_6_async_WeakCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DeferExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DeferExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_DeferExceptionCallback = &__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(1, 93, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_ValueCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ValueCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(1, 93, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ValueCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_ValueCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_ValueCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(1, 93, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_ValueCallback = &__pyx_type_6chorde_7clients_6_async_ValueCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(1, 102, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_MissCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_MissCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_MissCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_MissCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MissCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(1, 102, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MissCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_MissCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_MissCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_MissCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(1, 102, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_MissCallback = &__pyx_type_6chorde_7clients_6_async_MissCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(1, 111, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(1, 111, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(1, 111, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_ExceptionCallback = &__pyx_type_6chorde_7clients_6_async_ExceptionCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(1, 120, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_AnyCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnyCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(1, 120, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnyCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_AnyCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_AnyCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(1, 120, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_AnyCallback = &__pyx_type_6chorde_7clients_6_async_AnyCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(1, 138, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_DoneCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DoneCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(1, 138, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DoneCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_DoneCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_DoneCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(1, 138, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_DoneCallback = &__pyx_type_6chorde_7clients_6_async_DoneCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(1, 145, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_NONE.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_NONE.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_NONE.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_NONE.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_NONE, (PyObject *)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(1, 145, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(1, 145, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_NONE, (PyObject *)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_NONE = &__pyx_type_6chorde_7clients_6_async_NONE;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -13115,14 +13183,18 @@
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec__async(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -13138,38 +13210,38 @@
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__async(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
-  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
   /*--- Module creation code ---*/
@@ -13178,247 +13250,350 @@
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_async", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
-  if (__Pyx_InitGlobals() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
-  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_chorde__clients___async) {
-    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
-    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(1, 1, __pyx_L1_error)
+    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "chorde.clients._async")) {
-      if (unlikely(PyDict_SetItemString(modules, "chorde.clients._async", __pyx_m) < 0)) __PYX_ERR(1, 1, __pyx_L1_error)
+      if (unlikely(PyDict_SetItemString(modules, "chorde.clients._async", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-  if (__Pyx_patch_abc() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "chorde/clients/_async.pyx":1
  * import functools             # <<<<<<<<<<<<<<
  * import weakref
  * import threading
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_functools, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_functools, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_functools, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_functools, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "chorde/clients/_async.pyx":2
  * import functools
  * import weakref             # <<<<<<<<<<<<<<
  * import threading
  * import logging
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_weakref, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_weakref, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_weakref, __pyx_t_1) < 0) __PYX_ERR(1, 2, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_weakref, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "chorde/clients/_async.pyx":3
  * import functools
  * import weakref
  * import threading             # <<<<<<<<<<<<<<
  * import logging
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_threading, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_threading, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_threading, __pyx_t_1) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_threading, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "chorde/clients/_async.pyx":4
  * import weakref
  * import threading
  * import logging             # <<<<<<<<<<<<<<
  * 
  * import cython
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_logging, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_logging, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logging, __pyx_t_1) < 0) __PYX_ERR(1, 4, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logging, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "chorde/clients/_async.pyx":8
  * import cython
  * 
  * from chorde.clients import base             # <<<<<<<<<<<<<<
  * 
  * cdef object CacheMissError, CancelledError, TimeoutError
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_base);
   __Pyx_GIVEREF(__pyx_n_s_base);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_base);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_chorde_clients, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 8, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_chorde_clients, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_base, __pyx_t_1) < 0) __PYX_ERR(1, 8, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_base, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "chorde/clients/_async.pyx":12
  * cdef object CacheMissError, CancelledError, TimeoutError
  * cdef object wref, functools_partial
  * CacheMissError = base.CacheMissError             # <<<<<<<<<<<<<<
  * CancelledError = base.CancelledError
  * TimeoutError = base.TimeoutError
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CacheMissError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CacheMissError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_CacheMissError, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "chorde/clients/_async.pyx":13
  * cdef object wref, functools_partial
  * CacheMissError = base.CacheMissError
  * CancelledError = base.CancelledError             # <<<<<<<<<<<<<<
  * TimeoutError = base.TimeoutError
  * wref = weakref.ref
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CancelledError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CancelledError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_CancelledError, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "chorde/clients/_async.pyx":14
  * CacheMissError = base.CacheMissError
  * CancelledError = base.CancelledError
  * TimeoutError = base.TimeoutError             # <<<<<<<<<<<<<<
  * wref = weakref.ref
  * functools_partial = functools.partial
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 14, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_TimeoutError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_TimeoutError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_TimeoutError);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_TimeoutError, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "chorde/clients/_async.pyx":15
  * CancelledError = base.CancelledError
  * TimeoutError = base.TimeoutError
  * wref = weakref.ref             # <<<<<<<<<<<<<<
  * functools_partial = functools.partial
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_weakref); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_weakref); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ref); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ref); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_wref);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_wref, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "chorde/clients/_async.pyx":16
  * TimeoutError = base.TimeoutError
  * wref = weakref.ref
  * functools_partial = functools.partial             # <<<<<<<<<<<<<<
  * 
  * cdef bint strip_tracebacks
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_functools); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_functools); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_partial); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_partial); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_functools_partial);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_functools_partial, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "chorde/clients/_async.pyx":19
  * 
  * cdef bint strip_tracebacks
  * strip_tracebacks = False             # <<<<<<<<<<<<<<
  * 
- * 
+ * cdef object _HTTPError = None
  */
   __pyx_v_6chorde_7clients_6_async_strip_tracebacks = 0;
 
-  /* "chorde/clients/_async.pyx":22
+  /* "chorde/clients/_async.pyx":21
+ * strip_tracebacks = False
+ * 
+ * cdef object _HTTPError = None             # <<<<<<<<<<<<<<
+ * 
+ * try:
+ */
+  __Pyx_INCREF(Py_None);
+  __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async__HTTPError);
+  __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async__HTTPError, Py_None);
+  __Pyx_GIVEREF(Py_None);
+
+  /* "chorde/clients/_async.pyx":23
+ * cdef object _HTTPError = None
+ * 
+ * try:             # <<<<<<<<<<<<<<
+ *     from tornado.web import HTTPError as _HTTPError
+ * except ImportError:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
+    __Pyx_XGOTREF(__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_4);
+    __Pyx_XGOTREF(__pyx_t_5);
+    /*try:*/ {
+
+      /* "chorde/clients/_async.pyx":24
+ * 
+ * try:
+ *     from tornado.web import HTTPError as _HTTPError             # <<<<<<<<<<<<<<
+ * except ImportError:
+ *     pass
+ */
+      __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L2_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_INCREF(__pyx_n_s_HTTPError);
+      __Pyx_GIVEREF(__pyx_n_s_HTTPError);
+      PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_HTTPError);
+      __pyx_t_2 = __Pyx_Import(__pyx_n_s_tornado_web, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L2_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_HTTPError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L2_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async__HTTPError);
+      __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async__HTTPError, __pyx_t_1);
+      __Pyx_GIVEREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+      /* "chorde/clients/_async.pyx":23
+ * cdef object _HTTPError = None
+ * 
+ * try:             # <<<<<<<<<<<<<<
+ *     from tornado.web import HTTPError as _HTTPError
+ * except ImportError:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    goto __pyx_L7_try_end;
+    __pyx_L2_error:;
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "chorde/clients/_async.pyx":25
+ * try:
+ *     from tornado.web import HTTPError as _HTTPError
+ * except ImportError:             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ImportError);
+    if (__pyx_t_6) {
+      __Pyx_ErrRestore(0,0,0);
+      goto __pyx_L3_exception_handled;
+    }
+    goto __pyx_L4_except_error;
+    __pyx_L4_except_error:;
+
+    /* "chorde/clients/_async.pyx":23
+ * cdef object _HTTPError = None
+ * 
+ * try:             # <<<<<<<<<<<<<<
+ *     from tornado.web import HTTPError as _HTTPError
+ * except ImportError:
+ */
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_XGIVEREF(__pyx_t_4);
+    __Pyx_XGIVEREF(__pyx_t_5);
+    __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
+    goto __pyx_L1_error;
+    __pyx_L3_exception_handled:;
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_XGIVEREF(__pyx_t_4);
+    __Pyx_XGIVEREF(__pyx_t_5);
+    __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
+    __pyx_L7_try_end:;
+  }
+
+  /* "chorde/clients/_async.pyx":29
  * 
  * 
  * def set_strip_tracebacks(bint strip):             # <<<<<<<<<<<<<<
  *     """ Sets traceback stripping behavior for async futures
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6chorde_7clients_6_async_1set_strip_tracebacks, NULL, __pyx_n_s_chorde_clients__async); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 22, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_strip_tracebacks, __pyx_t_1) < 0) __PYX_ERR(1, 22, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6chorde_7clients_6_async_1set_strip_tracebacks, NULL, __pyx_n_s_chorde_clients__async); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_strip_tracebacks, __pyx_t_2) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_NONE(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6chorde_7clients_6_async_3__pyx_unpickle_NONE, NULL, __pyx_n_s_chorde_clients__async); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_NONE, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6chorde_7clients_6_async_3__pyx_unpickle_NONE, NULL, __pyx_n_s_chorde_clients__async); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_NONE, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "chorde/clients/_async.pyx":1
  * import functools             # <<<<<<<<<<<<<<
  * import weakref
  * import threading
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
```

### Comparing `chorde-1.0.3/lib/chorde/clients/_async.pyx` & `chorde-1.0.4/lib/chorde/clients/_async.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 TimeoutError = base.TimeoutError
 wref = weakref.ref
 functools_partial = functools.partial
 
 cdef bint strip_tracebacks
 strip_tracebacks = False
 
+cdef object _HTTPError = None
+
+try:
+    from tornado.web import HTTPError as _HTTPError
+except ImportError:
+    pass
+
 
 def set_strip_tracebacks(bint strip):
     """ Sets traceback stripping behavior for async futures
 
     Async tracebacks have a tendency to cause memory leaks. Stripping them in
     production deployments is a good idea to avoid them, but keep them around
     during testing or non-production environments to get better diagnostic
@@ -47,15 +54,20 @@
         try:
             exc_typ, exc_obj, exc_tb = exc
         finally:
             # Don't leave references to the exc/tb in the frame
             del exc
         try:
             if not strip:
-                raise exc_typ(*exc_obj.args) from exc_obj
+                kwargs = {}
+                if isinstance(exc_obj, _HTTPError):
+                    # Workaround for tornado's HTTPError which does not function
+                    # correctly without a reason, and reason is given only as kwarg
+                    kwargs["reason"] = exc_obj.reason
+                raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
             elif exc_tb is not None:
                 if exc_obj is not None:
                     if getattr(exc_obj, '__traceback__') is not exc_tb:
                         exc_obj = exc_obj.with_traceback(exc_tb)
                     raise exc_obj
                 else:
                     raise exc_typ().with_traceback(exc_tb)
```

### Comparing `chorde-1.0.3/lib/chorde/clients/async.c` & `chorde-1.0.4/lib/chorde/clients/async.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/asyncache.c` & `chorde-1.0.4/lib/chorde/clients/asyncache.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/asyncache.py` & `chorde-1.0.4/lib/chorde/clients/asyncache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/base.c` & `chorde-1.0.4/lib/chorde/clients/base.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/base.py` & `chorde-1.0.4/lib/chorde/clients/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/coherent.py` & `chorde-1.0.4/lib/chorde/clients/coherent.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/elasticache.py` & `chorde-1.0.4/lib/chorde/clients/elasticache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/files.py` & `chorde-1.0.4/lib/chorde/clients/files.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/inproc.c` & `chorde-1.0.4/lib/chorde/clients/inproc.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/inproc.py` & `chorde-1.0.4/lib/chorde/clients/inproc.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/memcached.py` & `chorde-1.0.4/lib/chorde/clients/memcached.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/tiered.c` & `chorde-1.0.4/lib/chorde/clients/tiered.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/clients/tiered.py` & `chorde-1.0.4/lib/chorde/clients/tiered.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/decorators.c` & `chorde-1.0.4/lib/chorde/decorators.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/decorators.pxd` & `chorde-1.0.4/lib/chorde/decorators.pxd`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/decorators.py` & `chorde-1.0.4/lib/chorde/decorators.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/dnsutils.py` & `chorde-1.0.4/lib/chorde/dnsutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/external_integration.py` & `chorde-1.0.4/lib/chorde/external_integration.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/mq/coherence.py` & `chorde-1.0.4/lib/chorde/mq/coherence.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/mq/ipsub/base.py` & `chorde-1.0.4/lib/chorde/mq/ipsub/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/mq/ipsub/ipsub_zmq.py` & `chorde-1.0.4/lib/chorde/mq/ipsub/ipsub_zmq.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/sPickle.py` & `chorde-1.0.4/lib/chorde/sPickle.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/serialize.py` & `chorde-1.0.4/lib/chorde/serialize.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/shmemutils.py` & `chorde-1.0.4/lib/chorde/shmemutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/threadpool.py` & `chorde-1.0.4/lib/chorde/threadpool.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde/worker.py` & `chorde-1.0.4/lib/chorde/worker.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/lib/chorde.egg-info/PKG-INFO` & `chorde-1.0.4/lib/chorde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.3
+Version: 1.0.4
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.3/lib/chorde.egg-info/SOURCES.txt` & `chorde-1.0.4/lib/chorde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chorde-1.0.3/setup.py` & `chorde-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 no_pyrex = False
 try:
     from Cython.Distutils import build_ext, Extension
     from Cython.Build import cythonize
 except:
     no_pyrex = True
 
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 
 version_path = os.path.join(os.path.dirname(__file__), 'lib', 'chorde', '_version.py')
 if not os.path.exists(version_path):
     with open(version_path, "w") as version_file:
         pass
 with open(version_path, "r+") as version_file:
     version_content = "__version__ = %r" % (VERSION,)
```

