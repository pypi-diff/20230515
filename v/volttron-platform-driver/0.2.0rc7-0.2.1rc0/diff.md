# Comparing `tmp/volttron_platform_driver-0.2.0rc7.tar.gz` & `tmp/volttron_platform_driver-0.2.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_platform_driver-0.2.0rc7.tar", max compression
+gzip compressed data, was "volttron_platform_driver-0.2.1rc0.tar", max compression
```

## Comparing `volttron_platform_driver-0.2.0rc7.tar` & `volttron_platform_driver-0.2.1rc0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10255 2023-05-11 21:09:03.201087 volttron_platform_driver-0.2.0rc7/LICENSE
--rw-r--r--   0        0        0     2777 2023-05-11 21:09:03.201087 volttron_platform_driver-0.2.0rc7/README.md
--rw-r--r--   0        0        0     2111 2023-05-11 21:09:59.649289 volttron_platform_driver-0.2.0rc7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 21:09:03.205087 volttron_platform_driver-0.2.0rc7/src/platform_driver/__init__.py
--rw-r--r--   0        0        0    34550 2023-05-11 21:09:03.205087 volttron_platform_driver-0.2.0rc7/src/platform_driver/agent.py
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 volttron_platform_driver-0.2.0rc7/PKG-INFO
+-rw-r--r--   0        0        0    10255 2023-05-15 18:07:23.404584 volttron_platform_driver-0.2.1rc0/LICENSE
+-rw-r--r--   0        0        0     2777 2023-05-15 18:08:16.973508 volttron_platform_driver-0.2.1rc0/README.md
+-rw-r--r--   0        0        0     2137 2023-05-15 18:09:45.550815 volttron_platform_driver-0.2.1rc0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 18:07:23.404584 volttron_platform_driver-0.2.1rc0/src/platform_driver/__init__.py
+-rw-r--r--   0        0        0    34550 2023-05-15 18:07:23.404584 volttron_platform_driver-0.2.1rc0/src/platform_driver/agent.py
+-rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 volttron_platform_driver-0.2.1rc0/PKG-INFO
```

### Comparing `volttron_platform_driver-0.2.0rc7/LICENSE` & `volttron_platform_driver-0.2.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_platform_driver-0.2.0rc7/README.md` & `volttron_platform_driver-0.2.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `volttron_platform_driver-0.2.0rc7/pyproject.toml` & `volttron_platform_driver-0.2.1rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 exclude = ['docs/']
 
 [tool.poetry]
 name = "volttron-platform-driver"
-version = "0.2.0rc7"
+version = "0.2.1rc0"
 description = "The Platform Driver agent is a special purpose agent that manages communication between the Volttron platform and devices. The Platform driver features a number of endpoints for collecting data and sending control signals using the message bus and automatically publishes data to the bus on a specified interval."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/platform-driver-agent"
 homepage = "https://github.com/eclipse-volttron/platform-driver-agent"
 keywords = []
@@ -46,14 +46,15 @@
 yapf = "^0.32.0"
 toml = "^0.10.2"
 isort = "^5.10.1"
 safety = "^1.10.3"
 mypy = "^0.942"
 coverage = "^6.3.2"
 volttron-testing = "^0.4.1rc3"
+pytest-timeout = "^2.1.0"
 
 [tool.poetry.group.documentation.dependencies]
 Sphinx = "^4.5.0"
 sphinx-rtd-theme = "^1.0.0"
 
 [tool.poetry.scripts]
 volttron-platform-driver = "platform_driver.agent:main"
```

### Comparing `volttron_platform_driver-0.2.0rc7/src/platform_driver/agent.py` & `volttron_platform_driver-0.2.1rc0/src/platform_driver/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_platform_driver-0.2.0rc7/PKG-INFO` & `volttron_platform_driver-0.2.1rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-platform-driver
-Version: 0.2.0rc7
+Version: 0.2.1rc0
 Summary: The Platform Driver agent is a special purpose agent that manages communication between the Volttron platform and devices. The Platform driver features a number of endpoints for collecting data and sending control signals using the message bus and automatically publishes data to the bus on a specified interval.
 Home-page: https://github.com/eclipse-volttron/platform-driver-agent
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

