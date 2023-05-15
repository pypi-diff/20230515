# Comparing `tmp/blaster-server-0.0.429b0.tar.gz` & `tmp/blaster-server-0.0.430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.429b0.tar", last modified: Thu May 11 15:30:25 2023, max compression
+gzip compressed data, was "blaster-server-0.0.430.tar", last modified: Mon May 15 14:50:23 2023, max compression
```

## Comparing `blaster-server-0.0.429b0.tar` & `blaster-server-0.0.430.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.242540 blaster-server-0.0.429b0/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.429b0/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-05-11 15:30:25.242540 blaster-server-0.0.429b0/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.429b0/README.md
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.429b0/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.238540 blaster-server-0.0.429b0/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.429b0/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.238540 blaster-server-0.0.429b0/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.429b0/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.429b0/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.238540 blaster-server-0.0.429b0/blaster/cloud/aws/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.429b0/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-10 23:46:29.000000 blaster-server-0.0.429b0/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-06 07:07:21.000000 blaster-server-0.0.429b0/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3796 2023-03-06 12:38:58.000000 blaster-server-0.0.429b0/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.429b0/blaster/connection_pool.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.429b0/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-03-30 07:56:48.000000 blaster-server-0.0.429b0/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62877 2023-05-10 08:42:24.000000 blaster-server-0.0.429b0/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    14954 2023-03-22 22:32:18.000000 blaster-server-0.0.429b0/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36583 2023-04-18 10:02:10.000000 blaster-server-0.0.429b0/blaster/server.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46392 2023-05-11 00:33:39.000000 blaster-server-0.0.429b0/blaster/tools.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.238540 blaster-server-0.0.429b0/blaster/utils/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.238540 blaster-server-0.0.429b0/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.429b0/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.429b0/blaster/utils/data/mime_types.json
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7086 2023-04-16 20:57:56.000000 blaster-server-0.0.429b0/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.429b0/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.429b0/blaster/utils/fork.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.429b0/blaster/utils/lat_long_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5564 2023-05-09 13:55:03.000000 blaster-server-0.0.429b0/blaster/utils/phone_number_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.429b0/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.238540 blaster-server-0.0.429b0/blaster/websocket/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.429b0/blaster/websocket/_app.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_core.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_exceptions.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_handshake.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_http.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_logging.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_socket.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_ssl_compat.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_url.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.429b0/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.238540 blaster-server-0.0.429b0/blaster/websocket/tests/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/tests/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.238540 blaster-server-0.0.429b0/blaster_server.egg-info/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      851 2023-05-11 15:30:25.000000 blaster-server-0.0.429b0/blaster_server.egg-info/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-05-11 15:30:25.000000 blaster-server-0.0.429b0/blaster_server.egg-info/SOURCES.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-11 15:30:25.000000 blaster-server-0.0.429b0/blaster_server.egg-info/dependency_links.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-05-11 15:30:25.000000 blaster-server-0.0.429b0/blaster_server.egg-info/requires.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-11 15:30:25.000000 blaster-server-0.0.429b0/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.238540 blaster-server-0.0.429b0/examples/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.429b0/examples/fast_api_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/examples/gevent_wsgi_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.429b0/examples/meinheld_flask.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.429b0/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.429b0/examples/simple_examples.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.429b0/examples/test_chat_room.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.429b0/examples/tornado_hello_world.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.429b0/examples/wheezy_hello.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-11 15:30:25.242540 blaster-server-0.0.429b0/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1560 2023-05-11 15:30:22.000000 blaster-server-0.0.429b0/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-11 15:30:25.242540 blaster-server-0.0.429b0/test/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.429b0/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.429b0/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      503 2022-11-07 18:31:41.000000 blaster-server-0.0.429b0/test/test_schema.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.429b0/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.429b0/test/test_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.429b0/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.430/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.430/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-05-15 14:50:23.571991 blaster-server-0.0.430/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.430/README.md
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.430/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.567991 blaster-server-0.0.430/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.430/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.430/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.430/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/blaster/cloud/aws/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.430/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-10 23:46:29.000000 blaster-server-0.0.430/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-06 07:07:21.000000 blaster-server-0.0.430/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3828 2023-05-15 14:10:32.000000 blaster-server-0.0.430/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.430/blaster/connection_pool.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.430/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-05-15 14:09:30.000000 blaster-server-0.0.430/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62877 2023-05-10 08:42:24.000000 blaster-server-0.0.430/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15097 2023-05-15 14:49:07.000000 blaster-server-0.0.430/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36583 2023-04-18 10:02:10.000000 blaster-server-0.0.430/blaster/server.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46443 2023-05-15 14:15:15.000000 blaster-server-0.0.430/blaster/tools.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/blaster/utils/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.430/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.430/blaster/utils/data/mime_types.json
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-14 10:13:13.000000 blaster-server-0.0.430/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.430/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.430/blaster/utils/fork.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.430/blaster/utils/lat_long_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5564 2023-05-09 13:55:03.000000 blaster-server-0.0.430/blaster/utils/phone_number_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.430/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/blaster/websocket/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.430/blaster/websocket/_app.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_core.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_exceptions.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_handshake.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_http.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_logging.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_socket.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_ssl_compat.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_url.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.430/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/blaster/websocket/tests/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/tests/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.430/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/blaster_server.egg-info/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      849 2023-05-15 14:50:23.000000 blaster-server-0.0.430/blaster_server.egg-info/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-05-15 14:50:23.000000 blaster-server-0.0.430/blaster_server.egg-info/SOURCES.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-15 14:50:23.000000 blaster-server-0.0.430/blaster_server.egg-info/dependency_links.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-05-15 14:50:23.000000 blaster-server-0.0.430/blaster_server.egg-info/requires.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-15 14:50:23.000000 blaster-server-0.0.430/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/examples/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.430/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.430/examples/fast_api_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.430/examples/gevent_wsgi_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.430/examples/meinheld_flask.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.430/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.430/examples/simple_examples.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.430/examples/test_chat_room.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.430/examples/tornado_hello_world.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.430/examples/wheezy_hello.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-15 14:50:23.571991 blaster-server-0.0.430/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1559 2023-05-15 14:50:20.000000 blaster-server-0.0.430/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 14:50:23.571991 blaster-server-0.0.430/test/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.430/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.430/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      503 2022-11-07 18:31:41.000000 blaster-server-0.0.430/test/test_schema.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.430/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.430/test/test_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.430/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.429b0/LICENSE.txt` & `blaster-server-0.0.430/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/PKG-INFO` & `blaster-server-0.0.430/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.429b0
+Version: 0.0.430
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.429b0/README.md` & `blaster-server-0.0.430/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/__init__.py` & `blaster-server-0.0.430/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/cloud/analytics.py` & `blaster-server-0.0.430/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.430/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/cloud/push_tasks.py` & `blaster-server-0.0.430/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/cloud/storage.py` & `blaster-server-0.0.430/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/config.py` & `blaster-server-0.0.430/blaster/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 # default env variables
 IS_PROD = environ.get("IS_PROD") == "1"
 IS_STAGING = IS_PROD and environ.get("IS_STAGING") == "1"
 IS_DEV = 1 if not (IS_PROD or IS_STAGING) else 0
 
 # CRITICAL-50 ERROR-40  WARNING-30  INFO-20  DEBUG-10  NOTSET-0
+APP_NAME = ""
+APP_VERSION = "0"
 LOG_LEVEL = logging.DEBUG if IS_DEV else (logging.INFO if IS_STAGING else logging.WARN)
 DEBUG_PRINT_LEVEL = IS_DEV and int(environ.get("DEBUG_PRINT_LEVEL") or 0)
 
 
 _this_ = sys.modules[__name__]
```

### Comparing `blaster-server-0.0.429b0/blaster/connection_pool.py` & `blaster-server-0.0.430/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/logging.py` & `blaster-server-0.0.430/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/mongo_orm.py` & `blaster-server-0.0.430/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/schema.py` & `blaster-server-0.0.430/blaster/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from base64 import b64decode
 from datetime import datetime
 import ujson as json
 from typing import get_type_hints
 from functools import partial
 
-from blaster.tools import _OBJ_END_
+from blaster.tools import _OBJ_END_, _16KB_
 # bare minimum validations and schema generators
 
 
 def raise_exception(msg):
 	raise Exception(msg)
 
 
@@ -91,15 +91,15 @@
 		"date-time": lambda e: datetime.strptime(e.strip(), "%Y-%m-%dT%H:%M:%S.%fZ"),
 		"date": lambda e: datetime.strptime(e.strip(), "%Y-%m-%d"),
 		"binary": lambda e: e,
 		"byte": lambda e: b64decode(e)
 	}
 
 	def __init__(
-		self, one_of=None, minlen=0, maxlen=4294967295,
+		self, one_of=None, minlen=1, maxlen=_16KB_,
 		regex=None, default=_OBJ_END_, _name=None,
 		before=None, **kwargs
 	):
 		self.minlen = minlen
 		self.maxlen = maxlen
 		self.one_of = set(one_of) if one_of else None
 		self._default = default
@@ -225,15 +225,15 @@
 		return e
 
 	def __getitem__(self, *kv):
 		return _Dict(
 			str if len(kv) < 2 else kv[-2], 
 			str if len(kv) < 1 else kv[-1]
 		)
-				
+
 class Object:
 	def __init__(self, default=_OBJ_END_, _required_=None, _name=None, **keys):
 		self._default = default
 		self._required = set(_required_) if _required_ else set()
 		self._name = _name
 
 		# instance specific: Ex: Object(a=Int, b=Str)
@@ -299,27 +299,30 @@
 	def from_dict(self, _dict: dict, default=_OBJ_END_):
 		return self.__class__.from_dict(_dict, default=default)
 
 	@classmethod
 	def from_dict(cls, _dict: dict, default=_OBJ_END_):
 		ret = cls()
 		for _k, (k, _validator, _default) in cls._dict_key_to_object_key.items():
-			if((_v:= _dict.get(_k, _OBJ_END_)) != _OBJ_END_):
+			if((_v := _dict.get(_k, _OBJ_END_)) != _OBJ_END_):
 				# value exists
-				setattr(ret, k, _validator(_v))  
+				try:
+					setattr(ret, k, _validator(_v))
+				except Exception as ex:
+					raise Exception(f"key: {_k}/{k} failed validation: {_v} -> {ex}")
 			elif(_default != _OBJ_END_):
 				# key doesn't exists, if default exists it's set,
 				# else raises error with missing key
 				setattr(ret, k, _default)
 			elif(default != _OBJ_END_):
 				return default
 			else:
 				raise Exception(f"missing key: {_k}/{k}")
 		return ret
-		
+
 	def to_dict(self):
 		ret = {}
 		for k, attr_validation in self.__class__._validations.items():
 			ret[k] = getattr(self, k, None)
 		return ret
 
 
@@ -428,15 +431,15 @@
 		if(ret):
 			return {"schema": {"$ref": "#/definitions/" + x.__name__}}, x.validate
 
 		x._validations = _validations = {}
 		x._properties = _properties = {}
 		x._property_types = {}
 		x._required = _required = set()
-		x._dict_key_to_object_key = {} # used when converting json/dict to object
+		x._dict_key_to_object_key = {}  # used when converting json/dict to object
 
 		for k, _type in get_type_hints(x).items():
 			is_required = True
 			if(
 				_type.__module__ == 'typing'
 				and getattr(_type, "__origin__", None) == typing.Union
 				and getattr(_type, "__args__", None)
@@ -451,27 +454,27 @@
 
 			elif(isinstance(_type, _Required)):
 				# required
 				_type = _type._types[0]
 
 			# pure type to instance of schema types
 			_default = x.__dict__.get(k, _OBJ_END_)  # declaration default
-			if(x == int or x == Int):
+			if(_type == int or _type == Int):
 				_type = Int(default=_default)
 
-			elif(x == float):
+			elif(_type == float):
 				_type = Float(default=_default)
 
-			elif(x == str or x == Str):
+			elif(_type == str or _type == Str):
 				_type = Str(default=_default)
 
-			elif(x == Array or x == list):  # genric
+			elif(_type == Array or _type == list):  # genric
 				_type = Array(default=list(_default))
 
-			elif(x == dict or x == Dict):  # generic without any attributes
+			elif(_type == dict or _type == Dict):  # generic without any attributes
 				_type = _Dict(default=dict(_default))
 
 			_schema_and_validation = schema(_type)
 			if(_schema_and_validation):
 				_properties[k], _validations[k] = _schema_and_validation
 				if(_default != _OBJ_END_):  # ? and not isinstance(_type, type)):
 					is_required = False
```

### Comparing `blaster-server-0.0.429b0/blaster/server.py` & `blaster-server-0.0.430/blaster/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/tools.py` & `blaster-server-0.0.430/blaster/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 SECONDS_IN_HOUR = 60 * 60
 SECONDS_IN_DAY = 24 * 60 * 60
 
 EPOCH = datetime.utcfromtimestamp(0)
 
 
 _OBJ_END_ = object()
+_1KB_ = 1024
+_16KB_ = _1KB_ * 16
 
 
 def cur_ms():
 	return int(1000 * time.time())
 
 
 # genetic LRU cache
@@ -714,23 +716,23 @@
 
 def utf8(value) -> bytes:
 	if(isinstance(value, bytes)):
 		return value
 	return value.encode("utf-8")
 
 
-def create_signed_value(name, value, secret, expires_in=31 * SECONDS_IN_DAY):
+def create_signed_value(name, value, secret, expires_in=31 * SECONDS_IN_DAY) -> bytes:
 	timestamp = utf8(str(int(time.time() + expires_in)))
 	value = base64.b64encode(utf8(value))  # hide value
 	signature = hmac_hexdigest(secret, name, value, b"~", timestamp)
 	signed_value = b"|".join([value, b"~", timestamp, signature])
 	return signed_value
 
 
-def decode_signed_value(name, value, secret, expiry_check=True):
+def decode_signed_value(name, value, secret, expiry_check=True) -> bytes:
 	if not value:
 		return None
 	_value, *parts, _timestamp, _signature = utf8(value).split(b"|")
 	# check signature matches or not
 	signature = hmac_hexdigest(secret, name, _value, *parts, _timestamp)
 	if not hmac_compare_digest(_signature, signature):
 		return None
```

### Comparing `blaster-server-0.0.429b0/blaster/utils/data/countries.json` & `blaster-server-0.0.430/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/utils/data/mime_types.json` & `blaster-server-0.0.430/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/utils/data_utils.py` & `blaster-server-0.0.430/blaster/utils/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 COUNTRY_DATA = json.loads(open(os.path.join(os.path.dirname(__file__), "data/countries.json")).read())
 
 # use this with caution, please check before using this
 PHONE_CODE_TO_COUNTRY_CODE = {v["phone_code"]: k for k, v in COUNTRY_DATA.items()}
 
 
 # currencies data
-_currency_aliases = {"RS" : "INR", "KSH": "KES"}
+_currency_aliases = {"RS": "INR", "KSH": "KES"}
 INR_EXCHANGE_RATE = {
 	'USD': 0.012183438191392, 'EUR': 0.012422414249388, 'GBP': 0.010834394013173, 'JPY': 1.7987256393607, 'AUD': 0.018918695391527, 'CHF': 0.012264650860763, 'CAD': 0.016475260651803, 'ERN': 0.18138325525675, 'WST': 0.033606866950932, 'BRL': 0.061575865015267, 'NPR': 1.6002818984603, 'ZAR': 0.21904097072182, 'AZN': 0.020548978744206, 'PYG': 87.698105901714, 'GYD': 2.5174813763509, 'RWF': 12.847640911669, 'MOP': 0.097330612967188, 'BAM': 0.023829610727296, 'DKK': 0.091520558147964, 'LKR': 4.4253369648097, 'TND': 0.039426152317367, 'TWD': 0.3904224223879, 'IQD': 17.67608659105, 'AFN': 1.0633090696497, 'NAD': 0.21804729998828, 'SYP': 30.090527398382, 'LAK': 208.6569418136, 'GTQ': 0.094094802595334, 'PKR': 2.6891007125432, 'BGN': 0.024025334618917, 'PEN': 0.048222592843438, 'TMT': 0.042347807393353, 'SVC': 0.10534734117731, 'XCD': 0.032572927334165, 'AOA': 5.8338777609108, 'MVR': 0.18604621560991, 'SAR': 0.045747954133748, 'PLN': 0.057555274399256, 'GIP': 0.010615125834899, 'GEL': 0.033448488915627, 'MKD': 0.74888335612859, 'AWG': 0.021780640046069, 'HNL': 0.29746098884978, 'KES': 1.4619751970779, 'BHD': 0.0045697582094003, 'EGP': 0.29597397827042, 'HRK': 0.092572586150074, 'MRO': 0.46205975580038, 'COP': 61.045485173549, 'BBD': 0.024295428377073, 'DJF': 2.142075760844, 'MZN': 0.77155198457389, 'UGX': 45.737601645542, 'HKD': 0.095637705566837, 'MAD': 0.13281872006941, 'MYR': 0.057808842145032, 'MDL': 0.231466653616, 'PAB': 0.012111725630068, 'FJD': 0.027507699219076, 'CDF': 24.717683552498, 'TOP': 0.028683525013509, 'VUV': 1.4613772827802, 'KWD': 0.0037577233608513, 'THB': 0.45571957269225, 'XOF': 8.0978306511739, 'IRR': 508.82594230842, 'BOB': 0.083453674891916, 'LRD': 1.8502266037841, 'SDG': 6.9721953727962, 'PGK': 0.042396738640658, 'BWP': 0.16086663493789, 'OMR': 0.0046684705199891, 'ILS': 0.0432693372504, 'NGN': 5.3171962841669, 'UZS': 135.05352448274, 'ETB': 0.64238204558346, 'TTD': 0.081557777541978, 'ZMW': 0.19505971360262, 'KHR': 49.8448143478, 'SEK': 0.13334849790674, 'SGD': 0.01714093842782, 'HUF': 4.9317152140234, 'BYN': 0.036140191195114, 'TJS': 0.12333235182038, 'GMD': 0.75524441290526, 'CVE': 1.34522357781, 'ALL': 1.4339963895992, 'SCR': 0.15912051783169, 'DOP': 0.65633142833622, 'CNY': 0.087777573416397, 'ISK': 1.7941283265918, 'LYD': 0.060637696688727, 'CLP': 11.29324809433, 'BSD': 0.012040013068743, 'XPF': 1.4503666266756, 'LSL': 0.21788110539988, 'TZS': 28.066765860052, 'ANG': 0.021747410910516, 'LBP': 18.359279806714, 'MXN': 0.23771601585986, 'KZT': 5.6065613522336, 'HTG': 1.5472110658854, 'BND': 0.016981614654388, 'KMF': 5.967227017736, 'MRU': 0.45701040812891, 'MNT': 41.071840558137, 'JOD': 0.008611275201891, 'PHP': 0.71215375291958, 'XAF': 8.0977363153449, 'AMD': 4.8273157990942, 'UYU': 0.48746899128935, 'JMD': 1.8442581308686, 'SSP': 7.3400952698581, 'CUP': 0.012040013068743, 'NZD': 0.020664124312008, 'TRY': 0.2266941970772, 'VND': 302.6775993976, 'KGS': 1.0110804368492, 'MGA': 51.459947846019, 'SRD': 0.35599005016766, 'GHS': 0.1684502123068, 'MWK': 12.358841776249, 'YER': 3.0106372857781, 'NOK': 0.12560943375401, 'QAR': 0.044393720562668, 'CZK': 0.29969962628925, 'RUB': 0.78333676549317, 'RSD': 1.4310703139363, 'NIO': 0.433121227704, 'SBD': 0.099050592614216, 'MMK': 25.263810011899, 'MUR': 0.53332091471014, 'VES': 0.10313041241555, 'BDT': 1.2562816787422, 'RON': 0.06004767821541, 'DZD': 1.7031267545841, 'ARS': 1.9109965053783, 'STN': 0.30074698609641, 'BIF': 24.889857229834, 'SZL': 0.21804729998828, 'SOS': 6.8403926844849, 'AED': 0.044710920816339, 'IDR': 191.24754830074, 'KRW': 17.128153864145, 'UAH': 0.44986965813791, 'CRC': 7.5351414066391, 'BZD': 0.024254200770799, 'GNF': 103.76043930477
 }
 
 INR_EXCHANGE_RATE["INR"] = 1  # this is the base
 INR_EXCHANGE_RATE["APP_CURRENCY"] = 1  # this is the base
 INR_EXCHANGE_RATE["ROUTE"] = 1  # legacy
```

### Comparing `blaster-server-0.0.429b0/blaster/utils/events.py` & `blaster-server-0.0.430/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/utils/fork.py` & `blaster-server-0.0.430/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.430/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.430/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/utils/xss_html.py` & `blaster-server-0.0.430/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/__init__.py` & `blaster-server-0.0.430/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_abnf.py` & `blaster-server-0.0.430/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_app.py` & `blaster-server-0.0.430/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_core.py` & `blaster-server-0.0.430/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_exceptions.py` & `blaster-server-0.0.430/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_handshake.py` & `blaster-server-0.0.430/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_http.py` & `blaster-server-0.0.430/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_logging.py` & `blaster-server-0.0.430/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_socket.py` & `blaster-server-0.0.430/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.430/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_url.py` & `blaster-server-0.0.430/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/_utils.py` & `blaster-server-0.0.430/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/server.py` & `blaster-server-0.0.430/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.430/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.430/blaster_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.429b0
+Version: 0.0.430
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.429b0/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.430/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/examples/gevent_wsgi_test.py` & `blaster-server-0.0.430/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/examples/mongo_ormexample.py` & `blaster-server-0.0.430/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/examples/simple_examples.py` & `blaster-server-0.0.430/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/examples/test_chat_room.py` & `blaster-server-0.0.430/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/examples/tornado_hello_world.py` & `blaster-server-0.0.430/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/examples/wheezy_hello.py` & `blaster-server-0.0.430/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/setup.py` & `blaster-server-0.0.430/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.429b',
+	version='0.0.430',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.429b0/test/test_mongo_orm.py` & `blaster-server-0.0.430/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/test/test_tools.py` & `blaster-server-0.0.430/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/test/test_utils.py` & `blaster-server-0.0.430/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.429b0/test/timeit_snippets.py` & `blaster-server-0.0.430/test/timeit_snippets.py`

 * *Files identical despite different names*

