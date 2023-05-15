# Comparing `tmp/python_omnilogic_local-0.0.2.tar.gz` & `tmp/python_omnilogic_local-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.0.2.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.0.3.tar", max compression
```

## Comparing `python_omnilogic_local-0.0.2.tar` & `python_omnilogic_local-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1700 2023-05-10 16:33:48.289849 python_omnilogic_local-0.0.2/README.md
--rw-r--r--   0        0        0       74 2023-05-09 17:43:23.661025 python_omnilogic_local-0.0.2/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    30567 2023-05-10 23:24:06.608502 python_omnilogic_local-0.0.2/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     1612 2023-05-09 21:52:03.533845 python_omnilogic_local-0.0.2/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0     1674 2023-05-10 23:14:12.231775 python_omnilogic_local-0.0.2/pyomnilogic_local/types.py
--rw-r--r--   0        0        0     1383 2023-05-10 23:42:46.960875 python_omnilogic_local-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 python_omnilogic_local-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1697 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.3/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    30393 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.3/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     1763 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.3/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0     1674 2023-05-10 23:14:12.231775 python_omnilogic_local-0.0.3/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0     1414 2023-05-15 14:56:48.568207 python_omnilogic_local-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 python_omnilogic_local-0.0.3/PKG-INFO
```

### Comparing `python_omnilogic_local-0.0.2/README.md` & `python_omnilogic_local-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 - Setting filter/pump speed
 - Controlling ColorLogic lights including brightness, speed, and selected shows, with support for countdown timers
 
 If your controller has functionality outside of this list, please do not hesitate to [Open an Issue](https://github.com/cryptk/python-omnilogic-local/issues)
 
 ## Credits
 
-The work on this library would not have been possible without the efforts of [djtimca](https://github.com/djtimca/) and [garionphx](https://github.com/garionphx/)
+The work on this library would not have been possible without the efforts of [djtimca](https://github.com/djtimca/) and [John Sutherland](garionphx@gmail.com)
```

#### html2text {}

```diff
@@ -10,9 +10,9 @@
 Polling the logging configuration - Setting pool heater temperature - Turning
 pool heaters on/off - Turning other pool equipment on/off, including countdown
 timers - Setting filter/pump speed - Controlling ColorLogic lights including
 brightness, speed, and selected shows, with support for countdown timers If
 your controller has functionality outside of this list, please do not hesitate
 to [Open an Issue](https://github.com/cryptk/python-omnilogic-local/issues) ##
 Credits The work on this library would not have been possible without the
-efforts of [djtimca](https://github.com/djtimca/) and [garionphx](https://
-github.com/garionphx/)
+efforts of [djtimca](https://github.com/djtimca/) and [John Sutherland]
+(garionphx@gmail.com)
```

### Comparing `python_omnilogic_local-0.0.2/pyomnilogic_local/api.py` & `python_omnilogic_local-0.0.3/pyomnilogic_local/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,45 +118,36 @@
         Returns:
             _type_: _description_
         """
         transport, protocol = await self._get_endpoint()
 
         try:
             return await asyncio.wait_for(
-                protocol.set_heater(
-                    pool_id,
-                    equipment_id,
-                    temperature,
-                    unit
-                ),
+                protocol.set_heater(pool_id, equipment_id, temperature, unit),
                 self.response_timeout,
             )
         finally:
             transport.close()
 
-    async def async_set_heater_enable(self, pool_id: int, equipment_id: int, enabled:Union[int, bool]):
+    async def async_set_heater_enable(self, pool_id: int, equipment_id: int, enabled: Union[int, bool]):
         """async_set_heater_enable handles sending a SetHeaterEnable XML API call to the Hayward Omni pool controller
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
             enabled (bool, optional): Turn the heater on (True) or off (False)
 
         Returns:
             _type_: _description_
         """
         transport, protocol = await self._get_endpoint()
 
         try:
             return await asyncio.wait_for(
-                protocol.set_heater_enable(
-                    pool_id,
-                    equipment_id,
-                    enabled
-                ),
+                protocol.set_heater_enable(pool_id, equipment_id, enabled),
                 self.response_timeout,
             )
         finally:
             transport.close()
 
     # pylint: disable=too-many-arguments,too-many-locals
     async def async_set_equipment(
@@ -440,15 +431,15 @@
         data = await self._receive_file()
         return data
 
     async def set_heater_enable(
         self,
         pool_id: int,
         equipment_id: int,
-        enabled: Union[int,bool],
+        enabled: Union[int, bool],
     ):
         """set_heater_enabled handles sending a SetHeaterEnable XML API call to the Hayward Omni pool controller
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
             enabled (bool, optional): Turn the heater on (True) or off (False)
```

### Comparing `python_omnilogic_local-0.0.2/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.0.3/pyomnilogic_local/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 #!/usr/bin/env python3
 
 import asyncio
 import logging
 import os
 
-from pyomnilogic_local import OmniLogicAPI
+from pyomnilogic_local.api import OmniLogicAPI
+
+pool_id = 7  # pylint: disable=unused-variable
+pump_equipment_id = 8  # pylint: disable=unused-variable
+light_equipment_id = 10  # pylint: disable=unused-variable
 
 
 async def async_main():
-    omni = OmniLogicAPI((os.environ.get("OMNILOGIC_HOST"), 10444), 5.0)
+    omni = OmniLogicAPI((os.environ.get("OMNILOGIC_HOST"), 10444), 15.0)
 
     # Some basic calls to run some testing against the library
-    pool_id = 7  # pylint: disable=unused-variable
-    pump_equipment_id = 8  # pylint: disable=unused-variable
-    light_equipment_id = 10  # pylint: disable=unused-variable
-
-    print(await omni.async_get_config())
+    # Fetch the MSPConfig data
+    # print(await omni.async_get_config())
+    # Fetch the current telemetry data
     print(await omni.async_get_telemetry())
-
-    print(await omni.async_get_log_config())
-    print(await omni.async_get_alarm_list())
+    # Fetch the current log configuration
+    # print(await omni.async_get_log_config())
+    # Fetch a list of current alarms
+    # print(await omni.async_get_alarm_list())
+    # Fetch diagnostic data for a filter pump
+    # print(await omni.async_get_filter_diagnostics(pool_id, pump_equipment_id))
 
     # Turn a variable speed pump on to 50%
     # print(await omni.async_set_equipment(pool_id, pump_equipment_id, 50))
     # Turn a variable speed pump on to 75%
     # print(await omni.async_set_filter_speed(pool_id, pump_equipment_id, 75))
     # Turn the pump off
-    # print(await omni.async_set_equipment(pool_id, pump_equipment_id, 50))
+    # print(await omni.async_set_equipment(pool_id, pump_equipment_id, False))
 
     # Activate a light show
-    # print(await omni.async_set_light_show(
-    #   pool_id,
-    #   light_equipment_id,
-    #   ColorLogicShow.VOODOO_LOUNGE,
-    #   ColorLogicSpeed.ONE_HALF,
-    #   ColorLogicBrightness.SIXTY_PERCENT
-    # ))
+    # print(
+    #     await omni.async_set_light_show(
+    #         pool_id, light_equipment_id, ColorLogicShow.VOODOO_LOUNGE, ColorLogicSpeed.ONE_HALF, ColorLogicBrightness.SIXTY_PERCENT
+    #     )
+    # )
     # Turn off the light
-    # print(await omni.async_set_equipment(pool_id, light_equipment_id, 1))
-    # print(await omni.async_get_telemetry())
-
-    print(await omni.async_get_filter_diagnostics(pool_id, pump_equipment_id))
+    # print(await omni.async_set_equipment(pool_id, light_equipment_id, False))
 
 
 def main():
     logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", level=logging.DEBUG)
     asyncio.run(async_main())
```

### Comparing `python_omnilogic_local-0.0.2/pyomnilogic_local/types.py` & `python_omnilogic_local-0.0.3/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.0.2/pyproject.toml` & `python_omnilogic_local-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -45,7 +45,10 @@
 [tool.pylint."FORMAT"]
 # Maximum number of characters on a single line.
 max-line-length=140
 
 [tool.pylint."MESSAGES CONTROL"]
 #For now, we have a lot of thing missing docstrings, this is ok for now
 disable="missing-docstring"
+
+[tool.ruff]
+line-length = 140
```

### Comparing `python_omnilogic_local-0.0.2/PKG-INFO` & `python_omnilogic_local-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -54,8 +54,9 @@
 - Setting filter/pump speed
 - Controlling ColorLogic lights including brightness, speed, and selected shows, with support for countdown timers
 
 If your controller has functionality outside of this list, please do not hesitate to [Open an Issue](https://github.com/cryptk/python-omnilogic-local/issues)
 
 ## Credits
 
-The work on this library would not have been possible without the efforts of [djtimca](https://github.com/djtimca/) and [garionphx](https://github.com/garionphx/)
+The work on this library would not have been possible without the efforts of [djtimca](https://github.com/djtimca/) and [John Sutherland](garionphx@gmail.com)
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.0.3 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
@@ -23,9 +23,9 @@
 Polling the logging configuration - Setting pool heater temperature - Turning
 pool heaters on/off - Turning other pool equipment on/off, including countdown
 timers - Setting filter/pump speed - Controlling ColorLogic lights including
 brightness, speed, and selected shows, with support for countdown timers If
 your controller has functionality outside of this list, please do not hesitate
 to [Open an Issue](https://github.com/cryptk/python-omnilogic-local/issues) ##
 Credits The work on this library would not have been possible without the
-efforts of [djtimca](https://github.com/djtimca/) and [garionphx](https://
-github.com/garionphx/)
+efforts of [djtimca](https://github.com/djtimca/) and [John Sutherland]
+(garionphx@gmail.com)
```

