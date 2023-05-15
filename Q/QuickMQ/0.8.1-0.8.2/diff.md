# Comparing `tmp/QuickMQ-0.8.1.tar.gz` & `tmp/QuickMQ-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickMQ-0.8.1.tar", last modified: Fri Apr 28 14:33:04 2023, max compression
+gzip compressed data, was "QuickMQ-0.8.2.tar", last modified: Mon May 15 17:20:31 2023, max compression
```

## Comparing `QuickMQ-0.8.1.tar` & `QuickMQ-0.8.2.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.749647 QuickMQ-0.8.1/
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1071 2023-02-17 21:40:50.000000 QuickMQ-0.8.1/LICENSE
--rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-04-28 14:33:04.750648 QuickMQ-0.8.1/PKG-INFO
--rw-r--r--   0 mdrexler (29089) domain users   (700)     4522 2023-03-29 21:03:07.000000 QuickMQ-0.8.1/README.md
--rw-r--r--   0 mdrexler (29089) domain users   (700)      295 2023-03-22 22:41:02.000000 QuickMQ-0.8.1/pyproject.toml
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1506 2023-04-28 14:33:04.751648 QuickMQ-0.8.1/setup.cfg
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.746647 QuickMQ-0.8.1/src/
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.747648 QuickMQ-0.8.1/src/QuickMQ.egg-info/
--rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/PKG-INFO
--rw-r--r--   0 mdrexler (29089) domain users   (700)      653 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/SOURCES.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)        1 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/dependency_links.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)       50 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/entry_points.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)      113 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/requires.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)        8 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/top_level.txt
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.749647 QuickMQ-0.8.1/src/quickmq/
--rw-r--r--   0 mdrexler (29089) domain users   (700)      511 2023-03-29 21:03:07.000000 QuickMQ-0.8.1/src/quickmq/__init__.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)       82 2023-04-28 14:32:57.000000 QuickMQ-0.8.1/src/quickmq/__version__.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1469 2023-04-28 14:26:29.000000 QuickMQ-0.8.1/src/quickmq/api.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     5111 2023-03-31 21:47:11.000000 QuickMQ-0.8.1/src/quickmq/config.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)    10394 2023-04-28 14:26:29.000000 QuickMQ-0.8.1/src/quickmq/connection.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)       39 2023-03-03 20:16:51.000000 QuickMQ-0.8.1/src/quickmq/consume.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1968 2023-04-28 14:26:29.000000 QuickMQ-0.8.1/src/quickmq/editor.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)      462 2023-03-03 21:47:49.000000 QuickMQ-0.8.1/src/quickmq/exceptions.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1193 2023-04-28 14:28:11.000000 QuickMQ-0.8.1/src/quickmq/message.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     2545 2023-04-28 14:28:41.000000 QuickMQ-0.8.1/src/quickmq/publish.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)        0 2023-01-13 22:27:07.000000 QuickMQ-0.8.1/src/quickmq/py.typed
--rw-r--r--   0 mdrexler (29089) domain users   (700)     3394 2023-04-28 14:27:52.000000 QuickMQ-0.8.1/src/quickmq/session.py
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.749647 QuickMQ-0.8.1/test/
--rw-r--r--   0 mdrexler (29089) domain users   (700)     2446 2023-04-28 14:26:29.000000 QuickMQ-0.8.1/test/test_api.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1079 2023-04-28 14:27:44.000000 QuickMQ-0.8.1/test/test_cli.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1820 2023-03-29 21:03:07.000000 QuickMQ-0.8.1/test/test_config.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     2675 2023-03-03 21:47:49.000000 QuickMQ-0.8.1/test/test_connection.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)      535 2023-03-29 21:03:07.000000 QuickMQ-0.8.1/test/test_message.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1437 2023-03-03 20:12:14.000000 QuickMQ-0.8.1/test/test_session.py
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.308718 QuickMQ-0.8.2/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1071 2023-02-17 21:40:50.000000 QuickMQ-0.8.2/LICENSE
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-05-15 17:20:31.308718 QuickMQ-0.8.2/PKG-INFO
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     4522 2023-03-29 21:03:07.000000 QuickMQ-0.8.2/README.md
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      295 2023-03-22 22:41:02.000000 QuickMQ-0.8.2/pyproject.toml
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1506 2023-05-15 17:20:31.309718 QuickMQ-0.8.2/setup.cfg
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      154 2023-04-28 15:01:45.000000 QuickMQ-0.8.2/setup.py
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.306717 QuickMQ-0.8.2/src/
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.307717 QuickMQ-0.8.2/src/QuickMQ.egg-info/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/PKG-INFO
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      686 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/SOURCES.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)        1 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/dependency_links.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)       50 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/entry_points.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      113 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/requires.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)        8 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/top_level.txt
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.308718 QuickMQ-0.8.2/src/quickmq/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      511 2023-03-29 21:03:07.000000 QuickMQ-0.8.2/src/quickmq/__init__.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     4791 2023-05-15 17:19:27.000000 QuickMQ-0.8.2/src/quickmq/__main__.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)       82 2023-05-15 17:20:27.000000 QuickMQ-0.8.2/src/quickmq/__version__.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1469 2023-04-28 14:26:29.000000 QuickMQ-0.8.2/src/quickmq/api.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     5108 2023-05-15 13:58:38.000000 QuickMQ-0.8.2/src/quickmq/config.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)    10394 2023-04-28 14:26:29.000000 QuickMQ-0.8.2/src/quickmq/connection.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)       39 2023-03-03 20:16:51.000000 QuickMQ-0.8.2/src/quickmq/consume.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1968 2023-04-28 14:26:29.000000 QuickMQ-0.8.2/src/quickmq/editor.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      462 2023-03-03 21:47:49.000000 QuickMQ-0.8.2/src/quickmq/exceptions.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1193 2023-04-28 14:28:11.000000 QuickMQ-0.8.2/src/quickmq/message.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     2545 2023-04-28 14:28:41.000000 QuickMQ-0.8.2/src/quickmq/publish.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)        0 2023-01-13 22:27:07.000000 QuickMQ-0.8.2/src/quickmq/py.typed
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     3394 2023-04-28 14:27:52.000000 QuickMQ-0.8.2/src/quickmq/session.py
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.308718 QuickMQ-0.8.2/test/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     2446 2023-04-28 14:26:29.000000 QuickMQ-0.8.2/test/test_api.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1127 2023-04-28 14:57:16.000000 QuickMQ-0.8.2/test/test_cli.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1820 2023-03-29 21:03:07.000000 QuickMQ-0.8.2/test/test_config.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     2675 2023-03-03 21:47:49.000000 QuickMQ-0.8.2/test/test_connection.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      535 2023-03-29 21:03:07.000000 QuickMQ-0.8.2/test/test_message.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1437 2023-03-03 20:12:14.000000 QuickMQ-0.8.2/test/test_session.py
```

### Comparing `QuickMQ-0.8.1/LICENSE` & `QuickMQ-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/PKG-INFO` & `QuickMQ-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickMQ
-Version: 0.8.1
+Version: 0.8.2
 Summary: A simple RabbitMQ client
 Home-page: https://gitlab.ssec.wisc.edu/mdrexler/easymq
 Author: Max Drexler
 Author-email: mndrexler@wisc.edu
 License: MIT
 Keywords: rabbitmq,message publisher,amqp message
 Classifier: Programming Language :: Python :: 3
```

### Comparing `QuickMQ-0.8.1/README.md` & `QuickMQ-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/setup.cfg` & `QuickMQ-0.8.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 	platformdirs
 	dataclasses;python_version<'3.7'
 package_dir = 
 	=src
 
 [options.entry_points]
 console_scripts = 
-	quickmq = quickmq.cli.main:main
+	quickmq = quickmq.__main__:main
 
 [options.extras_require]
 testing = 
 	pytest
 	pytest-cov
 	mypy
 	flake8
```

### Comparing `QuickMQ-0.8.1/src/QuickMQ.egg-info/PKG-INFO` & `QuickMQ-0.8.2/src/QuickMQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickMQ
-Version: 0.8.1
+Version: 0.8.2
 Summary: A simple RabbitMQ client
 Home-page: https://gitlab.ssec.wisc.edu/mdrexler/easymq
 Author: Max Drexler
 Author-email: mndrexler@wisc.edu
 License: MIT
 Keywords: rabbitmq,message publisher,amqp message
 Classifier: Programming Language :: Python :: 3
```

### Comparing `QuickMQ-0.8.1/src/QuickMQ.egg-info/SOURCES.txt` & `QuickMQ-0.8.2/src/QuickMQ.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
+setup.py
 src/QuickMQ.egg-info/PKG-INFO
 src/QuickMQ.egg-info/SOURCES.txt
 src/QuickMQ.egg-info/dependency_links.txt
 src/QuickMQ.egg-info/entry_points.txt
 src/QuickMQ.egg-info/requires.txt
 src/QuickMQ.egg-info/top_level.txt
 src/quickmq/__init__.py
+src/quickmq/__main__.py
 src/quickmq/__version__.py
 src/quickmq/api.py
 src/quickmq/config.py
 src/quickmq/connection.py
 src/quickmq/consume.py
 src/quickmq/editor.py
 src/quickmq/exceptions.py
```

### Comparing `QuickMQ-0.8.1/src/quickmq/api.py` & `QuickMQ-0.8.2/src/quickmq/api.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/src/quickmq/config.py` & `QuickMQ-0.8.2/src/quickmq/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         return rep.__eq__(__obj)
 
     def __str__(self) -> str:
         return f"Config variable: {self.name}"
 
 
 class Configuration:
-
     DEFAULT_VARIABLES: List[Tuple[str, CFG_VALS, Callable]] = [
         ("RECONNECT_DELAY", 5.0, verify_pos_float),
         ("RECONNECT_TRIES", 3, int),
         ("DEFAULT_SERVER", "localhost", str),
         ("DEFAULT_EXCHANGE", "", str),
         ("DEFAULT_USER", "guest", str),
         ("DEFAULT_PASS", "guest", str),
@@ -106,15 +105,15 @@
             if file_path != CFG_FILE_PATH:
                 LOGGER.warning(f"IOError loading file {file_path}. {e.strerror}")
                 warnings.warn(
                     f"Couldn't load config from '{file_path}' because of {e} using default values"
                 )
             return new_configuration
 
-        for (k, v) in new_cfg_file.items():
+        for k, v in new_cfg_file.items():
             try:
                 new_configuration.set(k, v)
             except (AttributeError, ValueError) as e:
                 LOGGER.warning(f"Error with variable {k}: {e}")
                 warnings.warn(f"Couldn't set variable '{k}' because '{e}'")
         return new_configuration
```

### Comparing `QuickMQ-0.8.1/src/quickmq/connection.py` & `QuickMQ-0.8.2/src/quickmq/connection.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/src/quickmq/editor.py` & `QuickMQ-0.8.2/src/quickmq/editor.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/src/quickmq/message.py` & `QuickMQ-0.8.2/src/quickmq/message.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/src/quickmq/publish.py` & `QuickMQ-0.8.2/src/quickmq/publish.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/src/quickmq/session.py` & `QuickMQ-0.8.2/src/quickmq/session.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/test/test_api.py` & `QuickMQ-0.8.2/test/test_api.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/test/test_cli.py` & `QuickMQ-0.8.2/test/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,8 +27,10 @@
 def test_publish_from_stdin(create_listener):
     proc = subprocess.Popen(['quickmq', 'publish', '-s=localhost', '-e=amq.fanout'], stdin=subprocess.PIPE)
     try:
         proc.communicate(input=b'Hello', timeout=.1)
     except subprocess.TimeoutExpired:
         proc.kill()
     rcvd_bytes = create_listener.get_message(block=False)
+    if rcvd_bytes is None:
+        assert False
     assert loads(rcvd_bytes) == 'Hello'
```

### Comparing `QuickMQ-0.8.1/test/test_config.py` & `QuickMQ-0.8.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/test/test_connection.py` & `QuickMQ-0.8.2/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/test/test_message.py` & `QuickMQ-0.8.2/test/test_message.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.1/test/test_session.py` & `QuickMQ-0.8.2/test/test_session.py`

 * *Files identical despite different names*

