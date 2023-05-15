# Comparing `tmp/gridworks_proactor-0.1.8.tar.gz` & `tmp/gridworks_proactor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_proactor-0.1.8.tar", max compression
+gzip compressed data, was "gridworks_proactor-0.2.0.tar", max compression
```

## Comparing `gridworks_proactor-0.1.8.tar` & `gridworks_proactor-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1070 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/LICENSE
--rw-r--r--   0        0        0     2615 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/README.md
--rw-r--r--   0        0        0     2357 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2119 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/__init__.py
--rw-r--r--   0        0        0     1610 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/__init__.py
--rw-r--r--   0        0        0     4109 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/logging.py
--rw-r--r--   0        0        0      373 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/mqtt.py
--rw-r--r--   0        0        0     3107 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/paths.py
--rw-r--r--   0        0        0      596 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/proactor_settings.py
--rw-r--r--   0        0        0      107 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/link_state.py
--rw-r--r--   0        0        0     1351 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/__init__.py
--rw-r--r--   0        0        0     2763 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/acks.py
--rw-r--r--   0        0        0      514 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/asyncio_timer_manager.py
--rw-r--r--   0        0        0    16041 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/link_state.py
--rw-r--r--   0        0        0     2220 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/message_times.py
--rw-r--r--   0        0        0     1487 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/timer_interface.py
--rw-r--r--   0        0        0     5557 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/logger.py
--rw-r--r--   0        0        0     4184 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/logging_setup.py
--rw-r--r--   0        0        0     7718 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/message.py
--rw-r--r--   0        0        0    11137 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/mqtt.py
--rw-r--r--   0        0        0    13287 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/persister.py
--rw-r--r--   0        0        0    32266 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/proactor_implementation.py
--rw-r--r--   0        0        0     3448 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/proactor_interface.py
--rw-r--r--   0        0        0     2645 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/problems.py
--rw-r--r--   0        0        0        0 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/py.typed
--rw-r--r--   0        0        0     3714 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/stats.py
--rw-r--r--   0        0        0     9207 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/sync_thread.py
--rw-r--r--   0        0        0     6070 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/watchdog.py
--rw-r--r--   0        0        0     1053 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor_test/__init__.py
--rw-r--r--   0        0        0     6615 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor_test/clean.py
--rw-r--r--   0        0        0     6895 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/comm_test_helper.py
--rw-r--r--   0        0        0    20076 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/config/hardware-layout.json
--rw-r--r--   0        0        0      807 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/__init__.py
--rw-r--r--   0        0        0      187 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/child/__init__.py
--rw-r--r--   0        0        0      401 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/child/config.py
--rw-r--r--   0        0        0     2558 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/child/dummy.py
--rw-r--r--   0        0        0      195 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/names.py
--rw-r--r--   0        0        0      193 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/config.py
--rw-r--r--   0        0        0     2199 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/dummy.py
--rw-r--r--   0        0        0     2388 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/logger_guard.py
--rw-r--r--   0        0        0     9073 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor_test/proactor_recorder.py
--rw-r--r--   0        0        0    47333 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor_test/proactor_test_collections.py
--rw-r--r--   0        0        0     2936 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/wait.py
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.8/setup.py
--rw-r--r--   0        0        0     3844 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4286 2023-05-15 18:51:00.996145 gridworks_proactor-0.2.0/README.md
+-rw-r--r--   0        0        0     2390 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2304 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/__init__.py
+-rw-r--r--   0        0        0     1610 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/config/__init__.py
+-rw-r--r--   0        0        0     4109 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/config/logging.py
+-rw-r--r--   0        0        0      373 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/config/mqtt.py
+-rw-r--r--   0        0        0     3107 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/config/paths.py
+-rw-r--r--   0        0        0      677 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/config/proactor_settings.py
+-rw-r--r--   0        0        0      107 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/link_state.py
+-rw-r--r--   0        0        0     1775 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/__init__.py
+-rw-r--r--   0        0        0     2932 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/acks.py
+-rw-r--r--   0        0        0      514 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/links/asyncio_timer_manager.py
+-rw-r--r--   0        0        0    16554 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/link_manager.py
+-rw-r--r--   0        0        0    16232 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/link_state.py
+-rw-r--r--   0        0        0     2220 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/links/message_times.py
+-rw-r--r--   0        0        0    11137 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/links/mqtt.py
+-rw-r--r--   0        0        0     1487 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/links/timer_interface.py
+-rw-r--r--   0        0        0     5557 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/logger.py
+-rw-r--r--   0        0        0     4184 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/logging_setup.py
+-rw-r--r--   0        0        0     7718 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/message.py
+-rw-r--r--   0        0        0    13287 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/persister.py
+-rw-r--r--   0        0        0    23176 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor/proactor_implementation.py
+-rw-r--r--   0        0        0     3448 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/proactor_interface.py
+-rw-r--r--   0        0        0     2645 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/problems.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/py.typed
+-rw-r--r--   0        0        0     3714 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/stats.py
+-rw-r--r--   0        0        0     9207 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/sync_thread.py
+-rw-r--r--   0        0        0     6070 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor/watchdog.py
+-rw-r--r--   0        0        0     1491 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/__init__.py
+-rw-r--r--   0        0        0     6602 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/clean.py
+-rw-r--r--   0        0        0     6895 2023-05-15 18:50:40.656211 gridworks_proactor-0.2.0/src/gwproactor_test/comm_test_helper.py
+-rw-r--r--   0        0        0    20076 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/config/hardware-layout.json
+-rw-r--r--   0        0        0      807 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/__init__.py
+-rw-r--r--   0        0        0      187 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/child/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/child/config.py
+-rw-r--r--   0        0        0     2565 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/child/dummy.py
+-rw-r--r--   0        0        0      195 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/names.py
+-rw-r--r--   0        0        0      193 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/__init__.py
+-rw-r--r--   0        0        0     1021 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/config.py
+-rw-r--r--   0        0        0     2197 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/dummy.py
+-rw-r--r--   0        0        0     2388 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/logger_guard.py
+-rw-r--r--   0        0        0     9334 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/proactor_recorder.py
+-rw-r--r--   0        0        0    47306 2023-05-15 18:51:01.000145 gridworks_proactor-0.2.0/src/gwproactor_test/proactor_test_collections.py
+-rw-r--r--   0        0        0     2936 2023-05-15 18:50:40.660212 gridworks_proactor-0.2.0/src/gwproactor_test/wait.py
+-rw-r--r--   0        0        0     5515 1970-01-01 00:00:00.000000 gridworks_proactor-0.2.0/PKG-INFO
```

### Comparing `gridworks_proactor-0.1.8/LICENSE` & `gridworks_proactor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/pyproject.toml` & `gridworks_proactor-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-proactor"
-version = "0.1.8"
+version = "0.2.0"
 description = "Gridworks Proactor"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-proactor"
 repository = "https://github.com/thegridelectric/gridworks-proactor"
 documentation = "https://gridworks-proactor.readthedocs.io"
@@ -51,14 +51,15 @@
 safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
+sphinxcontrib-mermaid = "^0.8.1"
 
 [tool.poetry.extras]
 tests = ["pytest", "pytest-asyncio"]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/__init__.py` & `gridworks_proactor-0.2.0/src/gwproactor/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 
 This packages is not GridWorks-aware (except that it links actors with multiple mqtt clients). This separation between
 communication / action infrastructure and GridWorks semantics is intended to allow the latter to be more focussed.
 
 This package is not polished and the separation is up for debate.
 
 Particular questions:
+
 * Is the programming model still clean after more concrete actors are implemented and more infrastructure are added.
 * Does the separation add value or just complicate analysis.
 * MQTTClients should be made async.
 * Semantics of building message type namespaces should be spelled out / further worked out.
 * Test support should be implemented / cleaner.
 """
 
 from gwproactor.config import ProactorSettings
+from gwproactor.links.mqtt import QOS
+from gwproactor.links.mqtt import MQTTClients
+from gwproactor.links.mqtt import MQTTClientWrapper
+from gwproactor.links.mqtt import Subscription
 from gwproactor.logger import ProactorLogger
 from gwproactor.logging_setup import format_exceptions
 from gwproactor.logging_setup import setup_logging
-from gwproactor.proactor_implementation import MQTTCodec
 from gwproactor.proactor_implementation import Proactor
 from gwproactor.proactor_interface import Communicator
 from gwproactor.proactor_interface import CommunicatorInterface
 from gwproactor.proactor_interface import MonitoredName
 from gwproactor.proactor_interface import Runnable
 from gwproactor.proactor_interface import ServicesInterface
 from gwproactor.problems import Problems
@@ -34,19 +38,22 @@
 
 __all__ = [
     "AsyncQueueWriter",
     "Communicator",
     "CommunicatorInterface",
     "format_exceptions",
     "MonitoredName",
-    "MQTTCodec",
+    "MQTTClients",
+    "MQTTClientWrapper",
     "Proactor",
     "ProactorLogger",
     "ProactorSettings",
     "Problems",
+    "QOS",
     "responsive_sleep",
     "Runnable",
     "ServicesInterface",
     "setup_logging",
+    "Subscription",
     "SyncAsyncInteractionThread",
     "SyncAsyncQueueWriter",
 ]
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/config/__init__.py` & `gridworks_proactor-0.2.0/src/gwproactor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/config/logging.py` & `gridworks_proactor-0.2.0/src/gwproactor/config/logging.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/config/paths.py` & `gridworks_proactor-0.2.0/src/gwproactor/config/paths.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/config/proactor_settings.py` & `gridworks_proactor-0.2.0/src/gwproactor/config/proactor_settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from pydantic import BaseSettings
 from pydantic import validator
 
 from gwproactor.config.logging import LoggingSettings
 from gwproactor.config.paths import Paths
 
 
-MQTT_LINK_POLL_SECONDS = 60
+MQTT_LINK_POLL_SECONDS = 60.0
+ACK_TIMEOUT_SECONDS = 5.0
 
 
 class ProactorSettings(BaseSettings):
     paths: Paths = None
     logging: LoggingSettings = LoggingSettings()
     mqtt_link_poll_seconds: float = MQTT_LINK_POLL_SECONDS
+    ack_timeout_seconds: float = ACK_TIMEOUT_SECONDS
 
     class Config:
         env_prefix = "PROACTOR_"
         env_nested_delimiter = "__"
 
     @validator("paths", always=True)
     def get_paths(cls, v: Paths) -> Paths:
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/links/__init__.py` & `gridworks_proactor-0.2.0/src/gwproactor/links/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 from gwproactor.links.acks import DEFAULT_ACK_DELAY
 from gwproactor.links.acks import AckManager
 from gwproactor.links.acks import AckTimerCallback
 from gwproactor.links.acks import AckWaitInfo
 from gwproactor.links.asyncio_timer_manager import AsyncioTimerManager
+from gwproactor.links.link_manager import LinkManager
+from gwproactor.links.link_manager import LinkManagerTransition
 from gwproactor.links.link_state import CommLinkAlreadyExists
 from gwproactor.links.link_state import CommLinkMissing
 from gwproactor.links.link_state import InvalidCommStateInput
 from gwproactor.links.link_state import LinkState
 from gwproactor.links.link_state import LinkStates
 from gwproactor.links.link_state import RuntimeLinkStateError
 from gwproactor.links.link_state import StateName
 from gwproactor.links.link_state import Transition
 from gwproactor.links.link_state import TransitionName
 from gwproactor.links.message_times import LinkMessageTimes
 from gwproactor.links.message_times import MessageTimes
+from gwproactor.links.mqtt import QOS
+from gwproactor.links.mqtt import MQTTClients
+from gwproactor.links.mqtt import MQTTClientWrapper
+from gwproactor.links.mqtt import Subscription
 from gwproactor.links.timer_interface import TimerManagerInterface
 
 
 __all__ = [
     "DEFAULT_ACK_DELAY",
     "AckManager",
     "AckTimerCallback",
     "AckWaitInfo",
     "AsyncioTimerManager",
     "CommLinkAlreadyExists",
     "CommLinkMissing",
     "InvalidCommStateInput",
+    "LinkManager",
+    "LinkManagerTransition",
     "LinkState",
     "LinkStates",
     "RuntimeLinkStateError",
     "Transition",
     "TransitionName",
     "StateName",
     "LinkMessageTimes",
     "MessageTimes",
+    "MQTTClients",
+    "MQTTClientWrapper",
+    "QOS",
+    "Subscription",
     "TimerManagerInterface",
 ]
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/links/acks.py` & `gridworks_proactor-0.2.0/src/gwproactor/links/acks.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,27 +59,33 @@
             context=context,
         )
         if link_name not in self._acks:
             self._acks[link_name] = dict()
         self._acks[link_name][message_id] = wait_info
         return wait_info
 
+    def add_link(self, link_name: str) -> None:
+        self._acks[link_name] = dict()
+
     def _pop_wait_info(self, link_name: str, message_id: str) -> Optional[AckWaitInfo]:
         if (client_acks := self._acks.get(link_name, None)) is not None:
             return client_acks.pop(message_id, None)
         return None
 
     def _timeout(self, link_name: str, message_id: str) -> None:
         if (wait_info := self._pop_wait_info(link_name, message_id)) is not None:
             self._user_callback(wait_info)
 
     def cancel_ack_timer(self, link_name: str, message_id: str) -> AckWaitInfo:
         if (wait_info := self._pop_wait_info(link_name, message_id)) is not None:
             self._timer_mgr.cancel_timer(wait_info.timer_handle)
         return wait_info
 
-    def cancel_ack_timers(self, link_name: str) -> None:
+    def cancel_ack_timers(self, link_name: str) -> list[AckWaitInfo]:
         if link_name in self._acks:
             wait_infos = self._acks[link_name]
             self._acks[link_name] = dict()
             for wait_info in wait_infos.values():
                 self._timer_mgr.cancel_timer(wait_info.timer_handle)
+        else:
+            wait_infos = []
+        return wait_infos
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/links/asyncio_timer_manager.py` & `gridworks_proactor-0.2.0/src/gwproactor/links/asyncio_timer_manager.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/links/link_state.py` & `gridworks_proactor-0.2.0/src/gwproactor/links/link_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,31 +433,37 @@
 
     def __init__(self, names: Optional[Sequence[str]] = None):
         self._links = dict()
         if names is not None:
             for name in names:
                 self.add(name)
 
-    def link(self, name) -> Optional[LinkState]:
+    def link(self, name: str) -> Optional[LinkState]:
         return self._links.get(name, None)
 
-    def link_state(self, name) -> Optional[StateName]:
+    def link_state(self, name: str) -> Optional[StateName]:
         if name in self._links:
             return self._links[name].curr_state.name
         return None
 
+    def stopped(self, name: str) -> bool:
+        return self.link_state(name) == StateName.stopped
+
     def __contains__(self, name: str) -> bool:
         return name in self._links
 
     def __getitem__(self, name: str) -> LinkState:
         try:
             return self._links[name]
         except KeyError:
             raise CommLinkMissing(name)
 
+    def link_names(self) -> list[str]:
+        return list(self._links.keys())
+
     def add(self, name: str, state: StateName = StateName.not_started) -> LinkState:
         if name in self._links:
             raise CommLinkAlreadyExists(
                 name, current_state=self._links[name].curr_state.name
             )
         self._links[name] = LinkState(name, state)
         return self._links[name]
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/links/message_times.py` & `gridworks_proactor-0.2.0/src/gwproactor/links/message_times.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/links/timer_interface.py` & `gridworks_proactor-0.2.0/src/gwproactor/links/timer_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/logger.py` & `gridworks_proactor-0.2.0/src/gwproactor/logger.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/logging_setup.py` & `gridworks_proactor-0.2.0/src/gwproactor/logging_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/message.py` & `gridworks_proactor-0.2.0/src/gwproactor/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/mqtt.py` & `gridworks_proactor-0.2.0/src/gwproactor/links/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/persister.py` & `gridworks_proactor-0.2.0/src/gwproactor/persister.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/proactor_interface.py` & `gridworks_proactor-0.2.0/src/gwproactor/proactor_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/problems.py` & `gridworks_proactor-0.2.0/src/gwproactor/problems.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/stats.py` & `gridworks_proactor-0.2.0/src/gwproactor/stats.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/sync_thread.py` & `gridworks_proactor-0.2.0/src/gwproactor/sync_thread.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor/watchdog.py` & `gridworks_proactor-0.2.0/src/gwproactor/watchdog.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/clean.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,20 +132,21 @@
 
     Note that this fixture is run before _every_ test.
 
     The behavior of this fixture can be customized by:
         1. Modifying the contents of tests/.env-gwproactor-test.
         2. Changing the the path to the test dotenv file via the GWPROACTOR_TEST_DOTENV_PATH environment variable.
         3. Explicitly passing and parametrizing this fixture. For example, to run a test with a different hardware
-          layout file, such as DUMMY_TEST_HARDWARE_LAYOUT_PATH:
+            layout file, such as DUMMY_TEST_HARDWARE_LAYOUT_PATH:
+
+        >>> from gwproactor_test.clean import DUMMY_TEST_HARDWARE_LAYOUT_PATH
+        >>> @pytest.mark.parametrize("default_test_env", [(DefaultTestEnv(src_test_layout=DUMMY_TEST_HARDWARE_LAYOUT_PATH)], indirect=True)
+        >>> def test_something(default_test_env):
+        >>>    assert Paths().hardware_layout.open().read() == DUMMY_TEST_HARDWARE_LAYOUT_PATH.open().read()
 
-            >>> from gwproactor_test.clean import DUMMY_TEST_HARDWARE_LAYOUT_PATH
-            >>> @pytest.mark.parametrize("default_test_env", [(DefaultTestEnv(src_test_layout=DUMMY_TEST_HARDWARE_LAYOUT_PATH)], indirect=True)
-            >>> def test_something(default_test_env):
-            >>>    assert Paths().hardware_layout.open().read() == DUMMY_TEST_HARDWARE_LAYOUT_PATH.open().read()
 
     """
     test_env = getattr(request, "param", DefaultTestEnv())
     if test_env.xdg_home is None:
         test_env.xdg_home = tmp_path
     with test_env.context() as mpatch:
         yield mpatch
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/comm_test_helper.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/comm_test_helper.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/config/hardware-layout.json` & `gridworks_proactor-0.2.0/src/gwproactor_test/config/hardware-layout.json`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/dummies/__init__.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/dummies/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/dummies/child/dummy.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/dummies/child/dummy.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from gwproto import Decoders
 from gwproto import Message
 from gwproto import MQTTCodec
 from gwproto import MQTTTopic
 from gwproto import create_message_payload_discriminator
 
 from gwproactor import ProactorSettings
-from gwproactor.mqtt import QOS
+from gwproactor.links import QOS
 from gwproactor.persister import TimedRollingFilePersister
 from gwproactor.proactor_implementation import Proactor
 from gwproactor_test.dummies.child.config import DummyChildSettings
 from gwproactor_test.dummies.names import DUMMY_CHILD_NAME
 from gwproactor_test.dummies.names import DUMMY_PARENT_NAME
 
 
@@ -20,15 +20,15 @@
     [
         "gwproto.messages",
         "gwproactor.message",
     ],
 )
 
 
-class ChildMQTTCode(MQTTCodec):
+class ChildMQTTCodec(MQTTCodec):
     def __init__(self):
         super().__init__(
             Decoders.from_objects(message_payload_discriminator=ChildMessageDecoder)
         )
 
     def validate_source_alias(self, source_alias: str):
         if source_alias != DUMMY_PARENT_NAME:
@@ -45,30 +45,30 @@
         name: str = "",
         settings: Optional[DummyChildSettings] = None,
     ):
         super().__init__(
             name=name if name else DUMMY_CHILD_NAME,
             settings=DummyChildSettings() if settings is None else settings,
         )
-        self._add_mqtt_client(
+        self._links.add_mqtt_link(
             DummyChild.PARENT_MQTT,
             settings.parent_mqtt,
-            ChildMQTTCode(),
+            ChildMQTTCodec(),
             upstream=True,
             primary_peer=True,
         )
         for topic in [
             MQTTTopic.encode_subscription(Message.type_name(), DUMMY_PARENT_NAME),
             # Enable awaiting_setup edge case testing, which depends on receiving multiple, separate
             # MQTT topic subscription acks:
             MQTTTopic.encode_subscription(Message.type_name(), "1"),
             MQTTTopic.encode_subscription(Message.type_name(), "2"),
         ]:
-            self._mqtt_clients.subscribe(self.PARENT_MQTT, topic, QOS.AtMostOnce)
-        self.log_subscriptions("construction")
+            self._links.subscribe(self.PARENT_MQTT, topic, QOS.AtMostOnce)
+        self._links.log_subscriptions("construction")
 
     @classmethod
     def make_event_persister(
         cls, settings: ProactorSettings
     ) -> TimedRollingFilePersister:
         return TimedRollingFilePersister(settings.paths.event_dir)
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/config.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/dummy.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/dummies/parent/dummy.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import cast
 
 from gwproto import Decoders
 from gwproto import MQTTCodec
 from gwproto import MQTTTopic
 from gwproto import create_message_payload_discriminator
 
+from gwproactor.links import QOS
 from gwproactor.message import Message
-from gwproactor.mqtt import QOS
 from gwproactor.persister import SimpleDirectoryWriter
 from gwproactor.proactor_implementation import Proactor
 from gwproactor_test.dummies.names import DUMMY_CHILD_NAME
 from gwproactor_test.dummies.names import DUMMY_PARENT_NAME
 from gwproactor_test.dummies.parent.config import DummyParentSettings
 
 
@@ -41,21 +41,21 @@
         name: str = "",
         settings: Optional[DummyParentSettings] = None,
     ):
         super().__init__(
             name=name if name else DUMMY_PARENT_NAME,
             settings=DummyParentSettings() if settings is None else settings,
         )
-        self._add_mqtt_client(
+        self._links.add_mqtt_link(
             self.CHILD_MQTT,
             self.settings.child_mqtt,
             ParentMQTTCodec(),
             primary_peer=True,
         )
-        self._mqtt_clients.subscribe(
+        self._links.subscribe(
             self.CHILD_MQTT,
             MQTTTopic.encode_subscription(Message.type_name(), DUMMY_CHILD_NAME),
             QOS.AtMostOnce,
         )
 
     @classmethod
     def make_event_persister(
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/logger_guard.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/logger_guard.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/proactor_recorder.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/proactor_recorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 from paho.mqtt.client import MQTTMessageInfo
 
 from gwproactor import Proactor
 from gwproactor import ProactorSettings
 from gwproactor import Runnable
 from gwproactor import ServicesInterface
 from gwproactor.config import LoggerLevels
+from gwproactor.links import LinkManager
+from gwproactor.links import MQTTClients
+from gwproactor.links import MQTTClientWrapper
 from gwproactor.message import DBGCommands
 from gwproactor.message import DBGPayload
 from gwproactor.message import MQTTReceiptPayload
 from gwproactor.message import MQTTSubackPayload
-from gwproactor.mqtt import MQTTClients
-from gwproactor.mqtt import MQTTClientWrapper
 from gwproactor.stats import LinkStats
 from gwproactor.stats import ProactorStats
 
 
 def split_subscriptions(client_wrapper: MQTTClientWrapper) -> Tuple[int, Optional[int]]:
     for i, (topic, qos) in enumerate(client_wrapper.subscription_items()):
         MQTTClientWrapper.subscribe(client_wrapper, topic, qos)
@@ -112,54 +113,85 @@
 class _PausedAck:
     client: str
     message: Message
     qos: int
     context: Optional[Any]
 
 
+class RecorderLinks(LinkManager):
+
+    acks_paused: bool
+    needs_ack: list[_PausedAck]
+
+    # noinspection PyMissingConstructor
+    def __init__(self, other: LinkManager):
+        self.__dict__ = other.__dict__
+        self.acks_paused = False
+        self.needs_ack = []
+
+    def publish_message(
+        self, client, message: Message, qos: int = 0, context: Any = None
+    ) -> MQTTMessageInfo:
+        if self.acks_paused:
+            self.needs_ack.append(_PausedAck(client, message, qos, context))
+            return MQTTMessageInfo(-1)
+        else:
+            # noinspection PyProtectedMember
+            return super().publish_message(client, message, qos=qos, context=context)
+
+    def release_acks(self, clear: bool = False):
+        self.acks_paused = False
+        needs_ack = self.needs_ack
+        self.needs_ack = []
+        if not clear:
+            for paused_ack in needs_ack:
+                self.publish_message(**dataclasses.asdict(paused_ack))
+
+    def generate_event(self, event: EventT) -> None:
+        if isinstance(event, CommEvent):
+            cast(
+                RecorderLinkStats, self._stats.link(event.PeerName)
+            ).comm_events.append(event)
+        super().generate_event(event)
+
+
 def make_recorder_class(
     proactor_type: Type[ProactorT],
 ) -> Callable[..., RecorderInterface]:
     class Recorder(proactor_type):
 
         subacks_paused: bool
         pending_subacks: list[Message]
-        acks_paused: bool
-        needs_ack: list[_PausedAck]
         mqtt_messages_dropped: bool
 
         def __init__(self, name: str, settings: ProactorSettings, **kwargs_):
             super().__init__(name=name, settings=settings, **kwargs_)
             self.subacks_paused = False
             self.pending_subacks = []
-            self.acks_paused = False
-            self.needs_ack = []
             self.mqtt_messages_dropped = False
+            self._links = RecorderLinks(self._links)
 
         @classmethod
         def make_stats(cls) -> RecorderStats:
             return RecorderStats()
 
-        def generate_event(self: ProactorT, event: EventT) -> None:
-            if isinstance(event, CommEvent):
-                cast(
-                    RecorderLinkStats, self.stats.link(event.PeerName)
-                ).comm_events.append(event)
-            super().generate_event(event)
+        @property
+        def needs_ack(self) -> list[_PausedAck]:
+            return self._links.needs_ack
 
         def split_client_subacks(self: ProactorT, client_name: str):
-            client_wrapper = self._mqtt_clients.client_wrapper(client_name)
+            client_wrapper = self.mqtt_client_wrapper(client_name)
 
             def member_split_subscriptions():
                 return split_subscriptions(client_wrapper)
 
             client_wrapper.subscribe_all = member_split_subscriptions
 
         def restore_client_subacks(self: ProactorT, client_name: str):
-            client_wrapper = self._mqtt_clients.client_wrapper(client_name)
+            client_wrapper = self.mqtt_client_wrapper(client_name)
             client_wrapper.subscribe_all = MQTTClientWrapper.subscribe_all
 
         def pause_subacks(self):
             self.subacks_paused = True
 
         def release_subacks(self: ProactorT, num_released: int = -1):
             self.subacks_paused = False
@@ -173,76 +205,57 @@
         async def process_message(self, message: Message):
             if self.subacks_paused and isinstance(message.Payload, MQTTSubackPayload):
                 self.pending_subacks.append(message)
             else:
                 await super().process_message(message)
 
         def pause_acks(self):
-            self.acks_paused = True
+            self._links.acks_paused = True
 
         def release_acks(self, clear: bool = False):
-            self.acks_paused = False
-            needs_ack = self.needs_ack
-            self.needs_ack = []
-            if not clear:
-                for paused_ack in needs_ack:
-                    self._publish_message(**dataclasses.asdict(paused_ack))
-
-        def _publish_message(
-            self, client, message: Message, qos: int = 0, context: Any = None
-        ) -> MQTTMessageInfo:
-            if self.acks_paused:
-                self.needs_ack.append(_PausedAck(client, message, qos, context))
-                return MQTTMessageInfo(-1)
-            else:
-                # noinspection PyProtectedMember
-                return super()._publish_message(
-                    client, message, qos=qos, context=context
-                )
+            self._links.release_acks(clear)
+
+        def set_ack_timeout_seconds(self, delay: float) -> None:
+            self._links._acks._default_delay_seconds = delay  # noqa
 
         def drop_mqtt(self, drop: bool):
             self.mqtt_messages_dropped = drop
 
         def _process_mqtt_message(self, message: Message[MQTTReceiptPayload]):
             if not self.mqtt_messages_dropped:
                 # noinspection PyProtectedMember
                 super()._process_mqtt_message(message)
 
         def summary_str(self: ProactorT):
             s = str(self.stats)
             s += f"\nsubacks_paused: {self.subacks_paused}  pending_subacks: {len(self.pending_subacks)}\n"
             s += "Link states:\n"
             for link_name in self.stats.links:
-                s += f"  {link_name:10s}  {self._link_states.link_state(link_name).value}\n"
+                s += f"  {link_name:10s}  {self._links.link_state(link_name).value}\n"
             return s
 
-        def set_ack_timeout_seconds(self, timeout_seconds: float):
-            self._link_acks._default_delay_seconds = timeout_seconds
-
         def summarize(self: ProactorT):
             self._logger.info(self.summary_str())
 
         def ping_peer(self):
-            self._publish_message(
+            self._links.publish_message(
                 self.primary_peer_client, PingMessage(Src=self.publication_name)
             )
 
         @property
         def mqtt_clients(self) -> MQTTClients:
-            return self._mqtt_clients
+            return self._links.mqtt_clients()
 
         def mqtt_client_wrapper(self, client_name: str) -> MQTTClientWrapper:
-            return self._mqtt_clients.client_wrapper(client_name)
+            return self._links.mqtt_client_wrapper(client_name)
 
         def mqtt_subscriptions(self, client_name: str) -> list[str]:
             return [
                 item[0]
-                for item in self._mqtt_clients.client_wrapper(
-                    client_name
-                ).subscription_items()
+                for item in self.mqtt_client_wrapper(client_name).subscription_items()
             ]
 
         def send_dbg_to_peer(
             self,
             message_summary: int = -1,
             lifecycle: int = -1,
             comm_event: int = -1,
@@ -266,13 +279,13 @@
             )
 
         def _derived_process_message(self, message: Message):
             match message.Payload:
                 case DBGPayload():
                     message.Header.Src = self.publication_name
                     message.Header.Dst = self.primary_peer_client
-                    self._publish_message(self.primary_peer_client, message)
+                    self._links.publish_message(self.primary_peer_client, message)
                 case _:
                     # noinspection PyProtectedMember
                     super()._derived_process_message(message)
 
     return Recorder
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/proactor_test_collections.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/proactor_test_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 import warnings
 from typing import Type
 
 import pytest
 from gwproto import MQTTTopic
 from paho.mqtt.client import MQTT_ERR_CONN_LOST
 
-from gwproactor.config import MQTTClient
 from gwproactor.links import StateName
 from gwproactor.message import DBGPayload
 from gwproactor_test.comm_test_helper import CommTestHelper
-from gwproactor_test.dummies import DummyChildSettings
 from gwproactor_test.wait import await_for
 
 
 @pytest.mark.asyncio
 class ProactorCommTests:
     CTH: Type[CommTestHelper]
 
     async def test_no_parent(self):
         async with self.CTH(add_child=True) as h:
             child = h.child
             stats = child.stats.link(child.upstream_client)
             comm_event_counts = stats.comm_event_counts
-            link = child._link_states.link(child.upstream_client)
+            link = child._links.link(child.upstream_client)
 
             # unstarted child
             assert stats.num_received == 0
             assert link.state == StateName.not_started
 
             # start child
             h.start_child()
@@ -44,15 +42,15 @@
             assert comm_event_counts["gridworks.event.comm.mqtt.fully.subscribed"] == 1
             assert comm_event_counts["gridworks.event.comm.mqtt.disconnect"] == 0
             assert len(stats.comm_events) == 2
             for comm_event in stats.comm_events:
                 assert comm_event.MessageId in child._event_persister
 
             # Tell client we lost comm.
-            child._mqtt_clients.clients["gridworks"]._client._loop_rc_handle(
+            child.mqtt_client_wrapper("gridworks")._client._loop_rc_handle(
                 MQTT_ERR_CONN_LOST
             )
 
             # Wait for reconnect
             await await_for(
                 lambda: stats.comm_event_counts[
                     "gridworks.event.comm.mqtt.fully.subscribed"
@@ -76,15 +74,15 @@
     async def test_basic_comm_child_first(self):
         async with self.CTH(
             add_child=True, add_parent=True, verbose=True, parent_on_screen=True
         ) as h:
             child = h.child
             child_stats = child.stats.link(child.upstream_client)
             child_comm_event_counts = child_stats.comm_event_counts
-            child_link = child._link_states.link(child.upstream_client)
+            child_link = child._links.link(child.upstream_client)
 
             # unstarted child, parent
             assert child_stats.num_received == 0
             assert child_link.state == StateName.not_started
 
             # start child
             h.start_child()
@@ -135,15 +133,15 @@
                 lambda: child._event_persister.num_pending == 0,
                 1,
                 "ERROR waiting for events to be acked",
                 err_str_f=child.summary_str,
             )
 
             # Tell client we lost comm.
-            child._mqtt_clients.clients["gridworks"]._client._loop_rc_handle(
+            child.mqtt_client_wrapper("gridworks")._client._loop_rc_handle(
                 MQTT_ERR_CONN_LOST
             )
 
             # Wait for reconnect
             await await_for(
                 lambda: child_stats.comm_event_counts[
                     "gridworks.event.comm.peer.active"
@@ -170,51 +168,50 @@
             await await_for(
                 lambda: child._event_persister.num_pending == 0,
                 1,
                 "ERROR waiting for events to be acked",
                 err_str_f=child.summary_str,
             )
 
-    @pytest.mark.skip()
-    @pytest.mark.asyncio
-    async def test_broker_dns_failure(self):
-        """Verify proactor does not crash in presence of bad host.
-
-        This test skipped because it's currently very slow - 4 seconds
-        before mqtt client thread reports first problem.
-
-        A better test would:
-            - be faster
-            - verify client thread continues
-            - verify problem reports occur
-            - possibly verify that eventually child requests device restart since pi's are
-              having DNS failures on network comm loss that seem to be undone by pi restart
-        """
-        no_broker = MQTTClient(host="www.foo.com")
-        async with self.CTH(
-            child_settings=DummyChildSettings(
-                parent_mqtt=no_broker,
-            ),
-            start_child=True,
-            verbose=True,
-        ):
-            for i in range(20):
-                print(f"{i}...")
-                await asyncio.sleep(1)
+    # @pytest.mark.asyncio
+    # async def test_broker_dns_failure(self):
+    #     """Verify proactor does not crash in presence of bad host.
+    #
+    #     This test commented out because it's very slow - 4 seconds before mqtt client thread
+    #     reports first problem.
+    #
+    #     A better test would:
+    #         - be faster
+    #         - verify client thread continues
+    #         - verify problem reports occur
+    #         - possibly verify that eventually child requests device restart since pi's are
+    #           having DNS failures on network comm loss that seem to be undone by pi restart
+    #     """
+    #     no_broker = MQTTClient(host="www.foo.com")
+    #     async with self.CTH(
+    #         child_settings=DummyChildSettings(
+    #             parent_mqtt=no_broker,
+    #         ),
+    #         start_child=True,
+    #         verbose=True,
+    #     ):
+    #         for i in range(20):
+    #             print(f"{i}...")
+    #             await asyncio.sleep(1)
 
     @pytest.mark.asyncio
     async def test_basic_comm_parent_first(self):
         async with self.CTH(add_child=True, add_parent=True, verbose=True) as h:
             child = h.child
             child_stats = child.stats.link(child.upstream_client)
             child_comm_event_counts = child_stats.comm_event_counts
-            child_link = child._link_states.link(child.upstream_client)
+            child_link = child._links.link(child.upstream_client)
             parent = h.parent
             # TODO: hack
-            parent_link = parent._link_states.link(parent.primary_peer_client)
+            parent_link = parent._links.link(parent.primary_peer_client)
 
             # unstarted parent
             assert parent_link.state == StateName.not_started
 
             # start parent
             h.start_parent()
             await await_for(
@@ -259,17 +256,17 @@
 
     @pytest.mark.asyncio
     async def test_basic_parent_comm_loss(self):
         async with self.CTH(add_child=True, add_parent=True, verbose=False) as h:
             child = h.child
             child_stats = child.stats.link(child.upstream_client)
             child_comm_event_counts = child_stats.comm_event_counts
-            child_link = child._link_states.link(child.upstream_client)
+            child_link = child._links.link(child.upstream_client)
             parent = h.parent
-            parent_link = parent._link_states.link(parent.primary_peer_client)
+            parent_link = parent._links.link(parent.primary_peer_client)
 
             # unstarted child, parent
             assert parent_link.state == StateName.not_started
             assert child_stats.num_received == 0
             assert child_link.state == StateName.not_started
 
             # start child, parent
@@ -298,15 +295,15 @@
                 lambda: child._event_persister.num_pending == 0,
                 1,
                 "ERROR waiting for events to be acked",
                 err_str_f=child.summary_str,
             )
 
             # Tell *child* client we lost comm.
-            child._mqtt_clients.clients[child.upstream_client]._client._loop_rc_handle(
+            child.mqtt_client_wrapper(child.upstream_client)._client._loop_rc_handle(
                 MQTT_ERR_CONN_LOST
             )
 
             # Wait for reconnect
             await await_for(
                 lambda: child_stats.comm_event_counts[
                     "gridworks.event.comm.peer.active"
@@ -334,17 +331,17 @@
                 lambda: child._event_persister.num_pending == 0,
                 1,
                 "ERROR waiting for events to be acked",
                 err_str_f=child.summary_str,
             )
 
             # Tell *parent* client we lost comm.
-            parent._mqtt_clients.clients[
+            parent.mqtt_client_wrapper(
                 parent.primary_peer_client
-            ]._client._loop_rc_handle(MQTT_ERR_CONN_LOST)
+            )._client._loop_rc_handle(MQTT_ERR_CONN_LOST)
             # wait for child to get ping from parent when parent reconnects to mqtt
             parent_ping_topic = MQTTTopic.encode(
                 "gw", parent.publication_name, "gridworks-ping"
             )
             num_parent_pings = child_stats.num_received_by_topic[parent_ping_topic]
             await await_for(
                 lambda: child_stats.num_received_by_topic[parent_ping_topic]
@@ -365,18 +362,18 @@
             )
             assert child_comm_event_counts["gridworks.event.comm.mqtt.disconnect"] == 1
             assert child_comm_event_counts["gridworks.event.comm.peer.active"] == 2
             assert len(child_stats.comm_events) == 7
             assert child._event_persister.num_pending == 0
 
             # Tell *both* clients we lost comm.
-            parent._mqtt_clients.clients[
+            parent.mqtt_client_wrapper(
                 parent.primary_peer_client
-            ]._client._loop_rc_handle(MQTT_ERR_CONN_LOST)
-            child._mqtt_clients.clients[child.upstream_client]._client._loop_rc_handle(
+            )._client._loop_rc_handle(MQTT_ERR_CONN_LOST)
+            child.mqtt_client_wrapper(child.upstream_client)._client._loop_rc_handle(
                 MQTT_ERR_CONN_LOST
             )
 
             # Wait for reconnect
             await await_for(
                 lambda: child_stats.comm_event_counts[
                     "gridworks.event.comm.peer.active"
@@ -415,15 +412,15 @@
          (awaiting_setup_and_peer -> mqtt_suback -> awaiting_peer)
          (awaiting_setup_and_peer -> disconnected -> connecting)
         """
         async with self.CTH(add_child=True, verbose=True) as h:
             child = h.child
             stats = child.stats.link(child.upstream_client)
             comm_event_counts = stats.comm_event_counts
-            link = child._link_states.link(child.upstream_client)
+            link = child._links.link(child.upstream_client)
 
             # unstarted child
             assert stats.num_received == 0
             assert link.state == StateName.not_started
 
             # start child
             child.pause_subacks()
@@ -461,15 +458,15 @@
             assert comm_event_counts["gridworks.event.comm.mqtt.disconnect"] == 0
             assert len(stats.comm_events) == 2
             for comm_event in stats.comm_events:
                 assert comm_event.MessageId in child._event_persister
 
             # Tell client we lost comm
             child.pause_subacks()
-            child._mqtt_clients.clients[child.upstream_client]._client._loop_rc_handle(
+            child.mqtt_client_wrapper(child.upstream_client)._client._loop_rc_handle(
                 MQTT_ERR_CONN_LOST
             )
             await await_for(
                 lambda: len(child.pending_subacks) == 1,
                 3,
                 "ERROR waiting suback pending",
                 err_str_f=child.summary_str,
@@ -483,15 +480,15 @@
             assert comm_event_counts["gridworks.event.comm.mqtt.disconnect"] == 1
             assert len(stats.comm_events) == 4
             for comm_event in stats.comm_events:
                 assert comm_event.MessageId in child._event_persister
 
             # Tell client we lost comm
             child.pending_subacks = []
-            child._mqtt_clients.clients[child.upstream_client]._client._loop_rc_handle(
+            child.mqtt_client_wrapper(child.upstream_client)._client._loop_rc_handle(
                 MQTT_ERR_CONN_LOST
             )
             await await_for(
                 lambda: len(stats.comm_events) > 4,
                 1,
                 "ERROR waiting comm fail",
                 err_str_f=child.summary_str,
@@ -555,15 +552,15 @@
                     warnings.warn(
                         f"Skipping <{request.node.name}> because configured child proactor <{child.name}> "
                         f"has < 2 subscriptions. Subscriptions: {child_subscriptions}"
                     )
                 return
             stats = child.stats.link(child.upstream_client)
             comm_event_counts = stats.comm_event_counts
-            link = child._link_states.link(child.upstream_client)
+            link = child._links.link(child.upstream_client)
 
             # unstarted child
             assert stats.num_received == 0
             assert link.state == StateName.not_started
 
             # start child
             child.split_client_subacks(child.upstream_client)
@@ -631,15 +628,15 @@
             assert len(stats.comm_events) == 2
             for comm_event in stats.comm_events:
                 assert comm_event.MessageId in child._event_persister
 
             # (message_from_peer -> awaiting_setup)
             # Tell client we lost comm
             child.pause_subacks()
-            child._mqtt_clients.clients[child.upstream_client]._client._loop_rc_handle(
+            child.mqtt_client_wrapper(child.upstream_client)._client._loop_rc_handle(
                 MQTT_ERR_CONN_LOST
             )
             await await_for(
                 lambda: len(child.pending_subacks) == 3,
                 3,
                 "ERROR waiting suback pending",
                 err_str_f=child.summary_str,
@@ -716,15 +713,15 @@
                     warnings.warn(
                         f"Skipping <{request.node.name}> because configured child proactor <{child.name}> "
                         f"has < 2 subscriptions. Subscriptions: {child_subscriptions}"
                     )
                 return
             stats = child.stats.link(child.upstream_client)
             comm_event_counts = stats.comm_event_counts
-            link = child._link_states.link(child.upstream_client)
+            link = child._links.link(child.upstream_client)
 
             # unstarted child
             assert stats.num_received == 0
             assert link.state == StateName.not_started
 
             # start child
             # (not_started -> started -> connecting)
@@ -810,15 +807,15 @@
             )
             assert link.state == StateName.awaiting_setup
 
             # (awaiting_setup -> disconnected -> connecting)
             # Tell client we lost comm
             child.pending_subacks.clear()
             child.pause_subacks()
-            child._mqtt_clients.clients[child.upstream_client]._client._loop_rc_handle(
+            child.mqtt_client_wrapper(child.upstream_client)._client._loop_rc_handle(
                 MQTT_ERR_CONN_LOST
             )
             await await_for(
                 lambda: len(child.pending_subacks) == 3,
                 3,
                 "ERROR waiting suback pending",
                 err_str_f=child.summary_str,
@@ -843,17 +840,17 @@
                 f"ERROR waiting mqtt_suback {exp_subacks} (1/3)",
                 err_str_f=child.summary_str,
             )
             assert link.state == StateName.awaiting_setup_and_peer
 
             # (awaiting_setup_and_peer -> message_from_peer -> awaiting_setup)
             # Force parent to restore comm, delivering a message, sending us to awaiting_setup
-            parent._mqtt_clients.clients[
+            parent.mqtt_client_wrapper(
                 parent.primary_peer_client
-            ]._client._loop_rc_handle(MQTT_ERR_CONN_LOST)
+            )._client._loop_rc_handle(MQTT_ERR_CONN_LOST)
             await await_for(
                 lambda: link.in_state(StateName.awaiting_setup),
                 3,
                 f"ERROR waiting for message from peer",
                 err_str_f=child.summary_str,
             )
 
@@ -871,20 +868,23 @@
     async def test_response_timeout(self):
         """
         Test:
             (awaiting_peer -> response_timeout -> awaiting_peer)
             (active -> response_timeout -> awaiting_peer)
         """
 
-        async with self.CTH(add_child=True, add_parent=True, verbose=True) as h:
+        async with self.CTH(
+            add_child=True,
+            add_parent=True,
+        ) as h:
             child = h.child
-            link = child._link_states.link(child.upstream_client)
+            link = child._links.link(child.upstream_client)
             stats = child.stats.link(child.upstream_client)
             parent = h.parent
-            parent_link = parent._link_states.link(parent.primary_peer_client)
+            parent_link = parent._links.link(parent.primary_peer_client)
 
             # Timeout while awaiting setup
             # (awaiting_peer -> response_timeout -> awaiting_peer)
 
             # start parent
             parent.pause_acks()
             h.start_parent()
@@ -933,15 +933,15 @@
             )
 
             # Timeout while active
             # (active -> response_timeout -> awaiting_peer)
             parent.pause_acks()
             child.ping_peer()
             exp_timeouts = stats.timeouts + len(
-                child._link_acks._acks[child.upstream_client]
+                child._links._acks._acks[child.upstream_client]
             )
             await await_for(
                 lambda: stats.timeouts == exp_timeouts,
                 1,
                 "ERROR waiting for child to timeout",
                 err_str_f=child.summary_str,
             )
@@ -959,15 +959,14 @@
             await await_for(
                 lambda: link.in_state(StateName.active),
                 1,
                 "ERROR waiting for parent to restore link #1",
                 err_str_f=parent.summary_str,
             )
 
-    @pytest.mark.skip
     @pytest.mark.asyncio
     async def test_ping(self):
         """
         Test:
             ping sent peridoically if no messages sent
             ping not sent if messages are sent
             ping restores comm
@@ -978,26 +977,26 @@
             parent_settings.mqtt_link_poll_seconds
         ) = 0.1
         async with self.CTH(
             add_child=True,
             add_parent=True,
             child_settings=child_settings,
             parent_settings=parent_settings,
-            verbose=True,
+            verbose=False,
         ) as h:
             parent = h.parent
             parent_stats = parent.stats.link(parent.primary_peer_client)
             parent_ping_topic = MQTTTopic.encode(
                 "gw", parent.publication_name, "gridworks-ping"
             )
 
             child = h.child
             child.suppress_status = True
             child.set_ack_timeout_seconds(0.1)
-            link = child._link_states.link(child.upstream_client)
+            link = child._links.link(child.upstream_client)
             stats = child.stats.link(child.upstream_client)
             child_ping_topic = MQTTTopic.encode(
                 "gw", child.publication_name, "gridworks-ping"
             )
 
             # start parent and child
             h.start_parent()
@@ -1063,20 +1062,20 @@
             err_str = (
                 f"pings_from_parent: {pings_from_parent}\n"
                 f"messages_from_parent: {messages_from_parent}\n"
                 f"pings_from_child: {pings_from_child}\n"
                 f"messages_from_child: {messages_from_child}\n"
                 f"exp_pings_nominal: {exp_pings_nominal}\n"
             )
-            print(err_str)
-            print(parent.summary_str())
             assert pings_from_parent <= exp_pings_nominal, err_str
             assert pings_from_child <= exp_pings_nominal, err_str
-            assert messages_from_parent >= reps, err_str
-            assert messages_from_child >= 2 * reps, err_str
+            # Allow wide variance in number of messages exchanged - we are really testing pings, which
+            # Should be should be close to 0 when a lot of messages are being exchanged.
+            assert messages_from_parent >= reps * 0.5, err_str
+            assert messages_from_child >= reps * 0.5, err_str
 
             parent.pause_acks()
             await await_for(
                 lambda: link.in_state(StateName.awaiting_peer),
                 1,
                 "ERROR waiting for for parent to be slow",
                 err_str_f=child.summary_str,
```

### Comparing `gridworks_proactor-0.1.8/src/gwproactor_test/wait.py` & `gridworks_proactor-0.2.0/src/gwproactor_test/wait.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.8/PKG-INFO` & `gridworks_proactor-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: gridworks-proactor
-Version: 0.1.8
-Summary: Gridworks Proactor
-Home-page: https://github.com/thegridelectric/gridworks-proactor
-License: MIT
-Author: Jessica Millar
-Author-email: jmillar@gridworks-consulting.com
-Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: tests
-Requires-Dist: gridworks-protocol (>=0.3.6)
-Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
-Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
-Requires-Dist: pytest (>=7.2.0,<8.0.0) ; extra == "tests"
-Requires-Dist: pytest-asyncio (>=0.20.3,<0.21.0) ; extra == "tests"
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: result (>=0.9.0,<0.10.0)
-Requires-Dist: xdg (>=6.0.0,<7.0.0)
-Project-URL: Changelog, https://github.com/thegridelectric/gridworks-proactor/releases
-Project-URL: Documentation, https://gridworks-proactor.readthedocs.io
-Project-URL: Repository, https://github.com/thegridelectric/gridworks-proactor
-Description-Content-Type: text/markdown
-
 # Gridworks Proactor
 
 [![PyPI](https://img.shields.io/pypi/v/gridworks-proactor.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/gridworks-proactor.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/gridworks-proactor)][pypi status]
 [![License](https://img.shields.io/pypi/l/gridworks-proactor)][license]
 
@@ -44,34 +15,53 @@
 [pypi status]: https://pypi.org/project/gridworks-proactor/
 [read the docs]: https://gridworks-proactor.readthedocs.io/
 [tests]: https://github.com/thegridelectric/gridworks-proactor/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-proactor
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
+This packages provides "live actor" and "application monitored communication" infrastructure for the
+[GridWorks SpaceHeat SCADA](https://github.com/thegridelectric/gw-scada-spaceheat-python) project. This separation
+allows the scada code to be more focussed on on application specific details and provides the potential to re-use the
+"live actor" and "application monitored" infrastructure.
+
 ## Features
 
-- TODO
+- [](Proactor), a single threaded event loop running on asyncio, for exchanging messages between the main application
+  object, "live actor" subobjects and MQTT clients.
+- A [communication state] ("active" or not) for each external communications link is available to the proactor and
+  sub-objects. "Active" communications is defined as ALL of the following:
+  - The underlying communications mechanism (MQTT) is connected.
+  - All input channels of underlying mechanism (MQTT topics) are established.
+  - A application messages requiring acknowledgement have been ACKed in timely fashion (by default 5 seconds).
+  - A message has been received "recently" (by default within 1 minute).
+- Reliable delievery of "Events" generated locally. Generated Events are stored locally until they are acknowledged
+  and unacknowledged Events are retransmitted when the "Active" communication state is restored.
+- [](gwproactor_test), a test package for development and test environments of projects that implement a class derived
+  from [](Proactor), allowing the derived class to be tested with the base-class tests.
 
 ## Requirements
 
-- TODO
+Testing requires an MQTT broker. This can be installed on a mac with:
+
+```shell
+brew install mosquitto
+brew services restart mosquitto
+```
+
+Alternatively, the MQTT broker used by tests be controlled by .env file as described in [](DefaultTestEnv).
 
 ## Installation
 
 You can install _Gridworks Proactor_ via [pip] from [PyPI]:
 
 ```console
 $ pip install gridworks-proactor
 ```
 
-## Usage
-
-Please see the [Command-line Reference] for details.
-
 ## Contributing
 
 Contributions are very welcome. In order to develop, do this:
 
 ```console
 $ poetry install --all-extras
 ```
@@ -98,9 +88,8 @@
 [file an issue]: https://github.com/thegridelectric/gridworks-proactor/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
 [license]: https://github.com/thegridelectric/gridworks-proactor/blob/main/LICENSE
 [contributor guide]: https://github.com/thegridelectric/gridworks-proactor/blob/main/CONTRIBUTING.md
-[command-line reference]: https://gridworks-proactor.readthedocs.io/en/latest/usage.html
-
+[communication state]: https://gridworks-proactor.readthedocs.io/en/latest/comm_state.html
```

