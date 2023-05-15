# Comparing `tmp/fb-python-sdk-1.1.1.tar.gz` & `tmp/fb-python-sdk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb-python-sdk-1.1.1.tar", last modified: Mon Apr 17 09:38:46 2023, max compression
+gzip compressed data, was "fb-python-sdk-1.1.2.tar", last modified: Mon May 15 14:50:11 2023, max compression
```

## Comparing `fb-python-sdk-1.1.1.tar` & `fb-python-sdk-1.1.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-17 09:38:46.785927 fb-python-sdk-1.1.1/
--rw-r--r--   0 mac        (501) staff       (20)     1064 2022-11-07 09:43:18.000000 fb-python-sdk-1.1.1/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       71 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)    10442 2023-04-17 09:38:46.785577 fb-python-sdk-1.1.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     9369 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.1/README.md
--rw-r--r--   0 mac        (501) staff       (20)      128 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/dev-requirements.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-17 09:38:46.762639 fb-python-sdk-1.1.1/fb_python_sdk.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)    10442 2023-04-17 09:38:46.000000 fb-python-sdk-1.1.1/fb_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1113 2023-04-17 09:38:46.000000 fb-python-sdk-1.1.1/fb_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-17 09:38:46.000000 fb-python-sdk-1.1.1/fb_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      218 2023-04-17 09:38:46.000000 fb-python-sdk-1.1.1/fb_python_sdk.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       34 2023-04-17 09:38:46.000000 fb-python-sdk-1.1.1/fb_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-17 09:38:46.774835 fb-python-sdk-1.1.1/fbclient/
--rw-r--r--   0 mac        (501) staff       (20)     2249 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/fbclient/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1058 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/fbclient/category.py
--rw-r--r--   0 mac        (501) staff       (20)    17864 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.1/fbclient/client.py
--rw-r--r--   0 mac        (501) staff       (20)    10775 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.1/fbclient/common_types.py
--rw-r--r--   0 mac        (501) staff       (20)     8913 2023-04-16 01:04:02.000000 fb-python-sdk-1.1.1/fbclient/config.py
--rw-r--r--   0 mac        (501) staff       (20)     3342 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/fbclient/data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)    12389 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.1/fbclient/evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     8523 2023-04-14 07:20:29.000000 fb-python-sdk-1.1.1/fbclient/event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)     4597 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/fbclient/event_types.py
--rw-r--r--   0 mac        (501) staff       (20)     9517 2023-04-16 06:51:44.000000 fb-python-sdk-1.1.1/fbclient/interfaces.py
--rw-r--r--   0 mac        (501) staff       (20)     3688 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.1/fbclient/status.py
--rw-r--r--   0 mac        (501) staff       (20)     3160 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/fbclient/status_types.py
--rw-r--r--   0 mac        (501) staff       (20)    10647 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.1/fbclient/streaming.py
--rw-r--r--   0 mac        (501) staff       (20)      629 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.1/fbclient/update_processor.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-17 09:38:46.778865 fb-python-sdk-1.1.1/fbclient/utils/
--rw-r--r--   0 mac        (501) staff       (20)     4339 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.1/fbclient/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1950 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/fbclient/utils/exponential_backoff_jitter_strategy.py
--rw-r--r--   0 mac        (501) staff       (20)     5502 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/fbclient/utils/http_client.py
--rw-r--r--   0 mac        (501) staff       (20)     1320 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/fbclient/utils/repeatable_task.py
--rw-r--r--   0 mac        (501) staff       (20)     1158 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/fbclient/utils/rwlock.py
--rw-r--r--   0 mac        (501) staff       (20)      864 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.1/fbclient/utils/variation_splitting_algorithm.py
--rw-r--r--   0 mac        (501) staff       (20)       18 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.1/fbclient/version.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-17 09:38:46.780754 fb-python-sdk-1.1.1/intergration_tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-05 10:02:17.000000 fb-python-sdk-1.1.1/intergration_tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1398 2023-04-17 09:18:29.000000 fb-python-sdk-1.1.1/intergration_tests/run_in_start_no_wait.py
--rw-------   0 mac        (501) staff       (20)     1439 2023-04-17 09:15:32.000000 fb-python-sdk-1.1.1/intergration_tests/run_in_start_wait.py
--rw-r--r--   0 mac        (501) staff       (20)       84 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       81 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-17 09:38:46.786014 fb-python-sdk-1.1.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1851 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-17 09:38:46.784835 fb-python-sdk-1.1.1/tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 15:01:21.000000 fb-python-sdk-1.1.1/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3785 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/tests/test_data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)     4435 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.1/tests/test_data_update_status_provider.py
--rw-r--r--   0 mac        (501) staff       (20)     4675 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/tests/test_evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     4475 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.1/tests/test_event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)    10823 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.1/tests/test_fbclient.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.948225 fb-python-sdk-1.1.2/
+-rw-r--r--   0 mac        (501) staff       (20)     1064 2022-11-07 09:43:18.000000 fb-python-sdk-1.1.2/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       71 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)    10444 2023-05-15 14:50:11.947834 fb-python-sdk-1.1.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     9372 2023-05-15 14:37:00.000000 fb-python-sdk-1.1.2/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      128 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/dev-requirements.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.932296 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)    10444 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1142 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      218 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       34 2023-05-15 14:50:11.000000 fb-python-sdk-1.1.2/fb_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.939515 fb-python-sdk-1.1.2/fbclient/
+-rw-r--r--   0 mac        (501) staff       (20)     2249 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1058 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/category.py
+-rw-r--r--   0 mac        (501) staff       (20)    17863 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.2/fbclient/client.py
+-rw-r--r--   0 mac        (501) staff       (20)    10775 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.2/fbclient/common_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     8913 2023-04-16 01:04:02.000000 fb-python-sdk-1.1.2/fbclient/config.py
+-rw-r--r--   0 mac        (501) staff       (20)     3342 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/data_storage.py
+-rw-r--r--   0 mac        (501) staff       (20)    12389 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/fbclient/evaluator.py
+-rw-r--r--   0 mac        (501) staff       (20)     9022 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.2/fbclient/event_processor.py
+-rw-r--r--   0 mac        (501) staff       (20)     4597 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/event_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     9517 2023-04-16 06:51:44.000000 fb-python-sdk-1.1.2/fbclient/interfaces.py
+-rw-r--r--   0 mac        (501) staff       (20)     3688 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/fbclient/status.py
+-rw-r--r--   0 mac        (501) staff       (20)     3160 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/status_types.py
+-rw-r--r--   0 mac        (501) staff       (20)    10647 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.2/fbclient/streaming.py
+-rw-r--r--   0 mac        (501) staff       (20)      629 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.2/fbclient/update_processor.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.942814 fb-python-sdk-1.1.2/fbclient/utils/
+-rw-r--r--   0 mac        (501) staff       (20)     4339 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/fbclient/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1950 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/utils/exponential_backoff_jitter_strategy.py
+-rw-r--r--   0 mac        (501) staff       (20)     5502 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/utils/http_client.py
+-rw-r--r--   0 mac        (501) staff       (20)     1320 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/utils/repeatable_task.py
+-rw-r--r--   0 mac        (501) staff       (20)     1158 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/fbclient/utils/rwlock.py
+-rw-r--r--   0 mac        (501) staff       (20)      864 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/fbclient/utils/variation_splitting_algorithm.py
+-rw-r--r--   0 mac        (501) staff       (20)       18 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.2/fbclient/version.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.944519 fb-python-sdk-1.1.2/intergration_tests/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-05 10:02:17.000000 fb-python-sdk-1.1.2/intergration_tests/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      942 2023-05-15 05:29:46.000000 fb-python-sdk-1.1.2/intergration_tests/readme.py
+-rw-r--r--   0 mac        (501) staff       (20)     1398 2023-05-15 14:42:32.000000 fb-python-sdk-1.1.2/intergration_tests/run_in_start_no_wait.py
+-rw-------   0 mac        (501) staff       (20)     1437 2023-05-15 14:42:24.000000 fb-python-sdk-1.1.2/intergration_tests/run_in_start_wait.py
+-rw-r--r--   0 mac        (501) staff       (20)       84 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       81 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-15 14:50:11.948310 fb-python-sdk-1.1.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1851 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-15 14:50:11.947298 fb-python-sdk-1.1.2/tests/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 15:01:21.000000 fb-python-sdk-1.1.2/tests/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3785 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/tests/test_data_storage.py
+-rw-r--r--   0 mac        (501) staff       (20)     4435 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.2/tests/test_data_update_status_provider.py
+-rw-r--r--   0 mac        (501) staff       (20)     4675 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/tests/test_evaluator.py
+-rw-r--r--   0 mac        (501) staff       (20)     4475 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.2/tests/test_event_processor.py
+-rw-r--r--   0 mac        (501) staff       (20)    10823 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.2/tests/test_fbclient.py
```

### Comparing `fb-python-sdk-1.1.1/LICENSE` & `fb-python-sdk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/PKG-INFO` & `fb-python-sdk-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-python-sdk
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python SDK for FeatBit plateform
 Home-page: https://github.com/featbit/featbit-python-sdk
 Author: Dian SUN
 Author-email: featbit.master@gmail.com
 Project-URL: Code, https://github.com/featbit/featbit-python-sdk
 Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,26 +58,26 @@
 
 ```python
 from fbclient import get, set_config
 from fbclient.config import Config
 
 env_secret = '<replace-with-your-env-secret>'
 event_url = 'http://localhost:5100'
-streaming_url = '"ws://localhost:5100"'
+streaming_url = 'ws://localhost:5100'
 
 set_config(Config(env_secret, event_url, streaming_url))
 client = get()
 
 if client.initialize:
     flag_key = '<replace-with-your-flag-key>'
     user_key = 'bot-id'
     user_name = 'bot'
     user = {'key': user_key, 'name': user_name}
     detail = client.variation_detail(flag_key, user, default=None)
-    print(f'flag {flag_key} returns {detail.value} for user {user_key}, reason: {detail.reason}')
+    print(f'flag {flag_key} returns {detail.variation} for user {user_key}, reason: {detail.reason}')
 
 # ensure that the SDK shuts down cleanly and has a chance to deliver events to FeatBit before the program exits
 client.stop()
 ```
 
 ### Examples
```

### Comparing `fb-python-sdk-1.1.1/README.md` & `fb-python-sdk-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 ```python
 from fbclient import get, set_config
 from fbclient.config import Config
 
 env_secret = '<replace-with-your-env-secret>'
 event_url = 'http://localhost:5100'
-streaming_url = '"ws://localhost:5100"'
+streaming_url = 'ws://localhost:5100'
 
 set_config(Config(env_secret, event_url, streaming_url))
 client = get()
 
 if client.initialize:
     flag_key = '<replace-with-your-flag-key>'
     user_key = 'bot-id'
     user_name = 'bot'
     user = {'key': user_key, 'name': user_name}
     detail = client.variation_detail(flag_key, user, default=None)
-    print(f'flag {flag_key} returns {detail.value} for user {user_key}, reason: {detail.reason}')
+    print(f'flag {flag_key} returns {detail.variation} for user {user_key}, reason: {detail.reason}')
 
 # ensure that the SDK shuts down cleanly and has a chance to deliver events to FeatBit before the program exits
 client.stop()
 ```
 
 ### Examples
 
@@ -181,8 +181,8 @@
 
 - If you have a specific question about using this sdk, we encourage you
   to [ask it in our slack](https://join.slack.com/t/featbit/shared_invite/zt-1ew5e2vbb-x6Apan1xZOaYMnFzqZkGNQ).
 - If you encounter a bug or would like to request a
   feature, [submit an issue](https://github.com/featbit/featbit-python-sdk/issues/new).
 
 ## See Also
-- [Connect To Python Sdk](https://docs.featbit.co/docs/getting-started/4.-connect-an-sdk/server-side-sdks/python-sdk)
+- [Connect To Python Sdk](https://docs.featbit.co/docs/getting-started/4.-connect-an-sdk/server-side-sdks/python-sdk)
```

### Comparing `fb-python-sdk-1.1.1/fb_python_sdk.egg-info/PKG-INFO` & `fb-python-sdk-1.1.2/fb_python_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-python-sdk
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python SDK for FeatBit plateform
 Home-page: https://github.com/featbit/featbit-python-sdk
 Author: Dian SUN
 Author-email: featbit.master@gmail.com
 Project-URL: Code, https://github.com/featbit/featbit-python-sdk
 Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,26 +58,26 @@
 
 ```python
 from fbclient import get, set_config
 from fbclient.config import Config
 
 env_secret = '<replace-with-your-env-secret>'
 event_url = 'http://localhost:5100'
-streaming_url = '"ws://localhost:5100"'
+streaming_url = 'ws://localhost:5100'
 
 set_config(Config(env_secret, event_url, streaming_url))
 client = get()
 
 if client.initialize:
     flag_key = '<replace-with-your-flag-key>'
     user_key = 'bot-id'
     user_name = 'bot'
     user = {'key': user_key, 'name': user_name}
     detail = client.variation_detail(flag_key, user, default=None)
-    print(f'flag {flag_key} returns {detail.value} for user {user_key}, reason: {detail.reason}')
+    print(f'flag {flag_key} returns {detail.variation} for user {user_key}, reason: {detail.reason}')
 
 # ensure that the SDK shuts down cleanly and has a chance to deliver events to FeatBit before the program exits
 client.stop()
 ```
 
 ### Examples
```

### Comparing `fb-python-sdk-1.1.1/fb_python_sdk.egg-info/SOURCES.txt` & `fb-python-sdk-1.1.2/fb_python_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 fbclient/utils/__init__.py
 fbclient/utils/exponential_backoff_jitter_strategy.py
 fbclient/utils/http_client.py
 fbclient/utils/repeatable_task.py
 fbclient/utils/rwlock.py
 fbclient/utils/variation_splitting_algorithm.py
 intergration_tests/__init__.py
+intergration_tests/readme.py
 intergration_tests/run_in_start_no_wait.py
 intergration_tests/run_in_start_wait.py
 tests/__init__.py
 tests/test_data_storage.py
 tests/test_data_update_status_provider.py
 tests/test_evaluator.py
 tests/test_event_processor.py
```

### Comparing `fb-python-sdk-1.1.1/fbclient/__init__.py` & `fb-python-sdk-1.1.2/fbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/category.py` & `fb-python-sdk-1.1.2/fbclient/category.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/client.py` & `fb-python-sdk-1.1.2/fbclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,18 +88,17 @@
                                                               update_processor_ready)
         self._update_processor.start()
 
         if start_wait > 0:
             if not isinstance(self._update_processor, NullUpdateProcessor):
                 log.info("FB Python SDK: Waiting for Client initialization in %s seconds" % str(start_wait))
 
+            update_processor_ready.wait(start_wait)
             if isinstance(self._data_storage, NullDataStorage) or (not self._data_storage.initialized and not self._config.is_offline):
                 log.warning("FB Python SDK: SDK just returns default variation because of no data found in the given environment")
-
-            update_processor_ready.wait(start_wait)
             if not self._update_processor.initialized:
                 log.warning("FB Python SDK: SDK was not successfully initialized")
         else:
             log.info("FB Python SDK: SDK starts in asynchronous mode")
 
     def _build_event_processor(self, config: Config):
         if config.event_processor_imp:
```

### Comparing `fb-python-sdk-1.1.1/fbclient/common_types.py` & `fb-python-sdk-1.1.2/fbclient/common_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/config.py` & `fb-python-sdk-1.1.2/fbclient/config.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/data_storage.py` & `fb-python-sdk-1.1.2/fbclient/data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/evaluator.py` & `fb-python-sdk-1.1.2/fbclient/evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/event_processor.py` & `fb-python-sdk-1.1.2/fbclient/event_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from concurrent.futures import ThreadPoolExecutor
 from queue import Empty, Queue
-from threading import BoundedSemaphore, Lock, Thread
+from threading import BoundedSemaphore, Condition, Lock, Thread
 from typing import List, Optional
 
 from fbclient.common_types import FBEvent
 from fbclient.config import Config
 from fbclient.event_types import (EventMessage, FlagEvent, MessageType,
                                   MetricEvent, UserEvent)
 from fbclient.interfaces import EventProcessor, Sender
@@ -72,15 +72,15 @@
 
     def stop(self):
         with self.__lock:
             if not self.__closed:
                 log.info('FB Python SDK: event processor is stopping')
                 self.__closed = True
                 self.__flush_task.stop()
-                self.flush()
+                self.__put_message_async(MessageType.FLUSH)
                 self.__put_message_and_wait_terminate(MessageType.SHUTDOWN)
 
 
 class EventDispatcher(Thread):
 
     __MAX_FLUSH_WORKERS_NUMBER = 5
     __BATCH_SIZE = 50
@@ -90,14 +90,15 @@
         self.__config = config
         self.__inbox = inbox
         self.__closed = False
         self.__sender = sender
         self.__events_buffer_to_next_flush = []
         self.__flush_workers = ThreadPoolExecutor(max_workers=self.__MAX_FLUSH_WORKERS_NUMBER)
         self.__permits = BoundedSemaphore(value=self.__MAX_FLUSH_WORKERS_NUMBER)
+        self.__lock = Condition(Lock())
 
     # blocks until at least one message is available and then:
     # 1: transfer the events to event buffer
     # 2: try to flush events to featureflag if a flush message arrives
     # 3: wait for releasing resources if a shutdown arrives
     def run(self):
         log.debug('event dispatcher is working...')
@@ -133,38 +134,49 @@
 
     def __put_events_to_buffer(self, event: FBEvent):
         if not self.__closed and event.is_send_event:
             log.debug('put event to buffer')
             self.__events_buffer_to_next_flush.append(event)
 
     def __trigger_flush(self):
+        def flush_payload_done(fn):
+            self.__permits.release()
+            with self.__lock:
+                self.__lock.notify_all()
+
         if not self.__closed and len(self.__events_buffer_to_next_flush) > 0:
             log.debug('trigger flush')
             # get all the current events from event buffer
             if self.__permits.acquire(blocking=False):
                 payloads = []
                 payloads.extend(self.__events_buffer_to_next_flush)
                 # get an available flush worker to send events
                 self.__flush_workers \
                     .submit(FlushPayloadRunner(self.__config, self.__sender, payloads).run) \
-                    .add_done_callback(lambda x: self.__permits.release())
+                    .add_done_callback(flush_payload_done)
                 # clear the buffer for the next flush
                 self.__events_buffer_to_next_flush.clear()
             # if no available flush worker, keep the events in the buffer
 
     def __shutdown(self):
         if not self.__closed:
-            try:
-                log.debug('event dispatcher is cleaning up thread and conn pool')
-                self.__closed = True
-                log.debug('flush worker pool is stopping...')
-                self.__flush_workers.shutdown(wait=True)
-                self.__sender.stop()
-            except Exception as e:
-                log.exception('FB Python SDK: unexpected error when closing event dispatcher: %s' % str(e))
+            with self.__lock:
+                try:
+                    log.debug('event dispatcher is cleaning up thread and conn pool')
+                    self.__wait_until_flush_playload_worker_down()
+                    self.__closed = True
+                    log.debug('flush worker pool is stopping...')
+                    self.__flush_workers.shutdown(wait=True)
+                    self.__sender.stop()
+                except Exception as e:
+                    log.exception('FB Python SDK: unexpected error when closing event dispatcher: %s' % str(e))
+
+    def __wait_until_flush_playload_worker_down(self):
+        while self.__permits._value != self.__MAX_FLUSH_WORKERS_NUMBER:
+            self.__lock.wait()
 
 
 class FlushPayloadRunner:
     __MAX_EVENT_SIZE_PER_REQUEST = 50
 
     def __init__(self, config: Config, sender: Sender, payloads: List[FBEvent]):
         self.__config = config
```

### Comparing `fb-python-sdk-1.1.1/fbclient/event_types.py` & `fb-python-sdk-1.1.2/fbclient/event_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/interfaces.py` & `fb-python-sdk-1.1.2/fbclient/interfaces.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/status.py` & `fb-python-sdk-1.1.2/fbclient/status.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/status_types.py` & `fb-python-sdk-1.1.2/fbclient/status_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/streaming.py` & `fb-python-sdk-1.1.2/fbclient/streaming.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/update_processor.py` & `fb-python-sdk-1.1.2/fbclient/update_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/utils/__init__.py` & `fb-python-sdk-1.1.2/fbclient/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/utils/exponential_backoff_jitter_strategy.py` & `fb-python-sdk-1.1.2/fbclient/utils/exponential_backoff_jitter_strategy.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/utils/http_client.py` & `fb-python-sdk-1.1.2/fbclient/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/utils/repeatable_task.py` & `fb-python-sdk-1.1.2/fbclient/utils/repeatable_task.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/utils/rwlock.py` & `fb-python-sdk-1.1.2/fbclient/utils/rwlock.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/fbclient/utils/variation_splitting_algorithm.py` & `fb-python-sdk-1.1.2/fbclient/utils/variation_splitting_algorithm.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/intergration_tests/run_in_start_no_wait.py` & `fb-python-sdk-1.1.2/intergration_tests/run_in_start_no_wait.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fbclient.config import Config
 from fbclient.utils import log
 
 logging.basicConfig(level=logging.DEBUG,
                     format='%(asctime)s,%(msecs)d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
                     datefmt='%m-%d %H:%M')
 
-env_secret = '9T0GABTXokagxhUZ81hUnws9_E2uOpIEyTjScBRr6JKA'
+env_secret = 'fXWjg00OTEa-M_iBCyYiBwFPfdBisjAkiY3ycIMOWw1Q'
 
 config = Config(env_secret, event_url='http://localhost:5100', streaming_url='ws://localhost:5100')
 client = FBClient(config, start_wait=0)
 
 if client.update_status_provider.wait_for_OKState(timeout=15.):
     while True:
         line = input('input user key and flag key seperated by / \n')
```

### Comparing `fb-python-sdk-1.1.1/intergration_tests/run_in_start_wait.py` & `fb-python-sdk-1.1.2/intergration_tests/run_in_start_wait.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from fbclient.config import Config
 from fbclient.utils import log
 
 logging.basicConfig(level=logging.DEBUG,
                     format='%(asctime)s,%(msecs)d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
                     datefmt='%m-%d %H:%M')
 
-env_secret = '9T0GABTXokagxhUZ81hUnws9_E2uOpIEyTjScBRr6JKA'
+env_secret = 'fXWjg00OTEa-M_iBCyYiBwFPfdBisjAkiY3ycIMOWw1Q'
 
 config = Config(env_secret, event_url='http://localhost:5100', streaming_url='ws://localhost:5100')
 
 set_config(config)
 
 client = get()
 
 if client.initialize:
-    # client.identify({'key': 'test-python-sdk-user', 'name': 'test-python-sdk-user'})
+    client.identify({'key': 'test-python-sdk-user', 'name': 'test-python-sdk-user'})
     while True:
         line = input('input user key and flag key seperated by / \n')
         if 'exit' == line.strip():
             break
         try:
             user_key, flag_key, *_ = tuple(line.split('/'))
             user = {'key': user_key, 'name': user_key, 'country': 'cn'}
```

### Comparing `fb-python-sdk-1.1.1/setup.py` & `fb-python-sdk-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/tests/test_data_storage.py` & `fb-python-sdk-1.1.2/tests/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/tests/test_data_update_status_provider.py` & `fb-python-sdk-1.1.2/tests/test_data_update_status_provider.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/tests/test_evaluator.py` & `fb-python-sdk-1.1.2/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/tests/test_event_processor.py` & `fb-python-sdk-1.1.2/tests/test_event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.1/tests/test_fbclient.py` & `fb-python-sdk-1.1.2/tests/test_fbclient.py`

 * *Files identical despite different names*

