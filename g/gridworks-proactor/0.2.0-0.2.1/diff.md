# Comparing `tmp/gridworks_proactor-0.2.0.tar.gz` & `tmp/gridworks_proactor-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_proactor-0.2.0.tar", max compression
+gzip compressed data, was "gridworks_proactor-0.2.1.tar", max compression
```

## Comparing `gridworks_proactor-0.2.0.tar` & `gridworks_proactor-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     1070 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/LICENSE
--rw-r--r--   0        0        0     4286 2023-05-15 18:51:00.996145 gridworks_proactor-0.2.0/README.md
--rw-r--r--   0        0        0     2390 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2304 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/config/__init__.py
--rw-r--r--   0        0        0     4109 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/config/logging.py
--rw-r--r--   0        0        0      373 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/config/mqtt.py
--rw-r--r--   0        0        0     3107 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/config/paths.py
--rw-r--r--   0        0        0      677 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/config/proactor_settings.py
--rw-r--r--   0        0        0      107 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/link_state.py
--rw-r--r--   0        0        0     1775 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/__init__.py
--rw-r--r--   0        0        0     2932 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/acks.py
--rw-r--r--   0        0        0      514 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/links/asyncio_timer_manager.py
--rw-r--r--   0        0        0    16554 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/link_manager.py
--rw-r--r--   0        0        0    16232 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/link_state.py
--rw-r--r--   0        0        0     2220 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/links/message_times.py
--rw-r--r--   0        0        0    11137 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/mqtt.py
--rw-r--r--   0        0        0     1487 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/links/timer_interface.py
--rw-r--r--   0        0        0     5557 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/logger.py
--rw-r--r--   0        0        0     4184 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/logging_setup.py
--rw-r--r--   0        0        0     7718 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/message.py
--rw-r--r--   0        0        0    13287 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/persister.py
--rw-r--r--   0        0        0    23176 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/proactor_implementation.py
--rw-r--r--   0        0        0     3448 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/proactor_interface.py
--rw-r--r--   0        0        0     2645 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/problems.py
--rw-r--r--   0        0        0        0 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/py.typed
--rw-r--r--   0        0        0     3714 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/stats.py
--rw-r--r--   0        0        0     9207 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/sync_thread.py
--rw-r--r--   0        0        0     6070 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/watchdog.py
--rw-r--r--   0        0        0     1491 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/__init__.py
--rw-r--r--   0        0        0     6602 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/clean.py
--rw-r--r--   0        0        0     6895 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor_test/comm_test_helper.py
--rw-r--r--   0        0        0    20076 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/config/hardware-layout.json
--rw-r--r--   0        0        0      807 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/__init__.py
--rw-r--r--   0        0        0      187 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/child/__init__.py
--rw-r--r--   0        0        0      401 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/child/config.py
--rw-r--r--   0        0        0     2565 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/child/dummy.py
--rw-r--r--   0        0        0      195 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/names.py
--rw-r--r--   0        0        0      193 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/__init__.py
--rw-r--r--   0        0        0     1021 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/config.py
--rw-r--r--   0        0        0     2197 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/dummy.py
--rw-r--r--   0        0        0     2388 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/logger_guard.py
--rw-r--r--   0        0        0     9334 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/proactor_recorder.py
--rw-r--r--   0        0        0    47306 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/proactor_test_collections.py
--rw-r--r--   0        0        0     2936 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/wait.py
--rw-r--r--   0        0        0     5515 1970-01-01 00:00:00.000000 gridworks_proactor-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-15 19:10:11.078098 gridworks_proactor-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4286 2023-05-15 19:10:11.078098 gridworks_proactor-0.2.1/README.md
+-rw-r--r--   0        0        0     2390 2023-05-15 19:10:27.823119 gridworks_proactor-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2304 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/__init__.py
+-rw-r--r--   0        0        0     1610 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/__init__.py
+-rw-r--r--   0        0        0     4109 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/logging.py
+-rw-r--r--   0        0        0      373 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/mqtt.py
+-rw-r--r--   0        0        0     3107 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/paths.py
+-rw-r--r--   0        0        0      677 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/proactor_settings.py
+-rw-r--r--   0        0        0     1775 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/__init__.py
+-rw-r--r--   0        0        0     2932 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/acks.py
+-rw-r--r--   0        0        0      514 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/asyncio_timer_manager.py
+-rw-r--r--   0        0        0    16554 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/link_manager.py
+-rw-r--r--   0        0        0    16232 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/link_state.py
+-rw-r--r--   0        0        0     2220 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/message_times.py
+-rw-r--r--   0        0        0    11137 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/mqtt.py
+-rw-r--r--   0        0        0     1487 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/timer_interface.py
+-rw-r--r--   0        0        0     5557 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/logger.py
+-rw-r--r--   0        0        0     4184 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/logging_setup.py
+-rw-r--r--   0        0        0     7718 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/message.py
+-rw-r--r--   0        0        0    13287 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/persister.py
+-rw-r--r--   0        0        0    23176 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/proactor_implementation.py
+-rw-r--r--   0        0        0     3448 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/proactor_interface.py
+-rw-r--r--   0        0        0     2645 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/problems.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/py.typed
+-rw-r--r--   0        0        0     3714 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/stats.py
+-rw-r--r--   0        0        0     9207 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/sync_thread.py
+-rw-r--r--   0        0        0     6070 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/watchdog.py
+-rw-r--r--   0        0        0     1491 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/__init__.py
+-rw-r--r--   0        0        0     6602 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/clean.py
+-rw-r--r--   0        0        0     6895 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/comm_test_helper.py
+-rw-r--r--   0        0        0    20076 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/config/hardware-layout.json
+-rw-r--r--   0        0        0      807 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/__init__.py
+-rw-r--r--   0        0        0      187 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/child/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/child/config.py
+-rw-r--r--   0        0        0     2565 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/child/dummy.py
+-rw-r--r--   0        0        0      195 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/names.py
+-rw-r--r--   0        0        0      193 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/__init__.py
+-rw-r--r--   0        0        0     1021 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/config.py
+-rw-r--r--   0        0        0     2197 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/dummy.py
+-rw-r--r--   0        0        0     2388 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/logger_guard.py
+-rw-r--r--   0        0        0     9334 2023-05-15 19:10:11.086098 gridworks_proactor-0.2.1/src/gwproactor_test/proactor_recorder.py
+-rw-r--r--   0        0        0    47306 2023-05-15 19:10:11.086098 gridworks_proactor-0.2.1/src/gwproactor_test/proactor_test_collections.py
+-rw-r--r--   0        0        0     2936 2023-05-15 19:10:11.086098 gridworks_proactor-0.2.1/src/gwproactor_test/wait.py
+-rw-r--r--   0        0        0     5515 1970-01-01 00:00:00.000000 gridworks_proactor-0.2.1/PKG-INFO
```

### Comparing `gridworks_proactor-0.2.0/LICENSE` & `gridworks_proactor-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/README.md` & `gridworks_proactor-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/pyproject.toml` & `gridworks_proactor-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-proactor"
-version = "0.2.0"
+version = "0.2.1"
 description = "Gridworks Proactor"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-proactor"
 repository = "https://github.com/thegridelectric/gridworks-proactor"
 documentation = "https://gridworks-proactor.readthedocs.io"
```

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/__init__.py` & `gridworks_proactor-0.2.1/src/gwproactor/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/config/__init__.py` & `gridworks_proactor-0.2.1/src/gwproactor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/config/logging.py` & `gridworks_proactor-0.2.1/src/gwproactor/config/logging.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/config/paths.py` & `gridworks_proactor-0.2.1/src/gwproactor/config/paths.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/config/proactor_settings.py` & `gridworks_proactor-0.2.1/src/gwproactor/config/proactor_settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/links/__init__.py` & `gridworks_proactor-0.2.1/src/gwproactor/links/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/links/acks.py` & `gridworks_proactor-0.2.1/src/gwproactor/links/acks.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/links/asyncio_timer_manager.py` & `gridworks_proactor-0.2.1/src/gwproactor/links/asyncio_timer_manager.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/links/link_manager.py` & `gridworks_proactor-0.2.1/src/gwproactor/links/link_manager.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/links/link_state.py` & `gridworks_proactor-0.2.1/src/gwproactor/links/link_state.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/links/message_times.py` & `gridworks_proactor-0.2.1/src/gwproactor/links/message_times.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/links/mqtt.py` & `gridworks_proactor-0.2.1/src/gwproactor/links/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/links/timer_interface.py` & `gridworks_proactor-0.2.1/src/gwproactor/links/timer_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/logger.py` & `gridworks_proactor-0.2.1/src/gwproactor/logger.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/logging_setup.py` & `gridworks_proactor-0.2.1/src/gwproactor/logging_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/message.py` & `gridworks_proactor-0.2.1/src/gwproactor/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/persister.py` & `gridworks_proactor-0.2.1/src/gwproactor/persister.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/proactor_implementation.py` & `gridworks_proactor-0.2.1/src/gwproactor/proactor_implementation.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/proactor_interface.py` & `gridworks_proactor-0.2.1/src/gwproactor/proactor_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/problems.py` & `gridworks_proactor-0.2.1/src/gwproactor/problems.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/stats.py` & `gridworks_proactor-0.2.1/src/gwproactor/stats.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/sync_thread.py` & `gridworks_proactor-0.2.1/src/gwproactor/sync_thread.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor/watchdog.py` & `gridworks_proactor-0.2.1/src/gwproactor/watchdog.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/__init__.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/clean.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/clean.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/comm_test_helper.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/comm_test_helper.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/config/hardware-layout.json` & `gridworks_proactor-0.2.1/src/gwproactor_test/config/hardware-layout.json`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/dummies/__init__.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/dummies/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/dummies/child/dummy.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/dummies/child/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/config.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/dummy.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/logger_guard.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/logger_guard.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/proactor_recorder.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/proactor_recorder.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/proactor_test_collections.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/proactor_test_collections.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/src/gwproactor_test/wait.py` & `gridworks_proactor-0.2.1/src/gwproactor_test/wait.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.0/PKG-INFO` & `gridworks_proactor-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-proactor
-Version: 0.2.0
+Version: 0.2.1
 Summary: Gridworks Proactor
 Home-page: https://github.com/thegridelectric/gridworks-proactor
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

