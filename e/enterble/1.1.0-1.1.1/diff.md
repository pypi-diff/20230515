# Comparing `tmp/enterble-1.1.0.tar.gz` & `tmp/enterble-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enterble-1.1.0.tar", last modified: Fri Oct 28 08:55:15 2022, max compression
+gzip compressed data, was "enterble-1.1.1.tar", last modified: Fri Oct 28 09:07:11 2022, max compression
```

## Comparing `enterble-1.1.0.tar` & `enterble-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 08:55:15.778220 enterble-1.1.0/
--rw-r--r--   0 chenyitao   (501) staff       (20)     1055 2022-07-12 10:05:03.000000 enterble-1.1.0/LICENSE
--rw-r--r--   0 chenyitao   (501) staff       (20)     5232 2022-10-28 08:55:15.777990 enterble-1.1.0/PKG-INFO
--rw-r--r--   0 chenyitao   (501) staff       (20)     4195 2022-07-26 06:02:13.000000 enterble-1.1.0/README.md
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 08:55:15.775502 enterble-1.1.0/enterble/
--rw-r--r--   0 chenyitao   (501) staff       (20)      205 2022-07-14 03:48:18.000000 enterble-1.1.0/enterble/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)       22 2022-07-26 10:16:15.000000 enterble-1.1.0/enterble/__version__.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 08:55:15.776593 enterble-1.1.0/enterble/adapter/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 03:49:28.000000 enterble-1.1.0/enterble/adapter/__init__.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 08:55:15.776807 enterble-1.1.0/enterble/adapter/flowtime/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-12 06:12:45.000000 enterble-1.1.0/enterble/adapter/flowtime/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     5125 2022-10-21 11:24:53.000000 enterble-1.1.0/enterble/adapter/flowtime/collector.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 08:55:15.777206 enterble-1.1.0/enterble/ble/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-08 05:57:36.000000 enterble-1.1.0/enterble/ble/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     9554 2022-10-28 08:46:30.000000 enterble-1.1.0/enterble/ble/device.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     2436 2022-10-28 08:34:28.000000 enterble-1.1.0/enterble/ble/scanner.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 08:55:15.777674 enterble-1.1.0/enterble/collector/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 03:48:57.000000 enterble-1.1.0/enterble/collector/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     6538 2022-10-28 08:49:04.000000 enterble-1.1.0/enterble/collector/collector.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 08:55:15.776459 enterble-1.1.0/enterble.egg-info/
--rw-r--r--   0 chenyitao   (501) staff       (20)     5232 2022-10-28 08:55:15.000000 enterble-1.1.0/enterble.egg-info/PKG-INFO
--rw-r--r--   0 chenyitao   (501) staff       (20)      502 2022-10-28 08:55:15.000000 enterble-1.1.0/enterble.egg-info/SOURCES.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)        1 2022-10-28 08:55:15.000000 enterble-1.1.0/enterble.egg-info/dependency_links.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)        1 2022-07-14 03:44:23.000000 enterble-1.1.0/enterble.egg-info/not-zip-safe
--rw-r--r--   0 chenyitao   (501) staff       (20)       14 2022-10-28 08:55:15.000000 enterble-1.1.0/enterble.egg-info/requires.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)        9 2022-10-28 08:55:15.000000 enterble-1.1.0/enterble.egg-info/top_level.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)       38 2022-10-28 08:55:15.778281 enterble-1.1.0/setup.cfg
--rw-r--r--   0 chenyitao   (501) staff       (20)     1523 2022-10-28 08:53:43.000000 enterble-1.1.0/setup.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 09:07:11.743636 enterble-1.1.1/
+-rw-r--r--   0 chenyitao   (501) staff       (20)     1055 2022-07-12 10:05:03.000000 enterble-1.1.1/LICENSE
+-rw-r--r--   0 chenyitao   (501) staff       (20)     5212 2022-10-28 09:07:11.743457 enterble-1.1.1/PKG-INFO
+-rw-r--r--   0 chenyitao   (501) staff       (20)     4195 2022-07-26 06:02:13.000000 enterble-1.1.1/README.md
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 09:07:11.741487 enterble-1.1.1/enterble/
+-rw-r--r--   0 chenyitao   (501) staff       (20)      205 2022-07-14 03:48:18.000000 enterble-1.1.1/enterble/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)       22 2022-07-26 10:16:15.000000 enterble-1.1.1/enterble/__version__.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 09:07:11.742427 enterble-1.1.1/enterble/adapter/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 03:49:28.000000 enterble-1.1.1/enterble/adapter/__init__.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 09:07:11.742634 enterble-1.1.1/enterble/adapter/flowtime/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-12 06:12:45.000000 enterble-1.1.1/enterble/adapter/flowtime/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     5125 2022-10-21 11:24:53.000000 enterble-1.1.1/enterble/adapter/flowtime/collector.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 09:07:11.743000 enterble-1.1.1/enterble/ble/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-08 05:57:36.000000 enterble-1.1.1/enterble/ble/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     9671 2022-10-28 09:04:15.000000 enterble-1.1.1/enterble/ble/device.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     2436 2022-10-28 08:34:28.000000 enterble-1.1.1/enterble/ble/scanner.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 09:07:11.743226 enterble-1.1.1/enterble/collector/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 03:48:57.000000 enterble-1.1.1/enterble/collector/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     6538 2022-10-28 08:49:04.000000 enterble-1.1.1/enterble/collector/collector.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2022-10-28 09:07:11.742302 enterble-1.1.1/enterble.egg-info/
+-rw-r--r--   0 chenyitao   (501) staff       (20)     5212 2022-10-28 09:07:11.000000 enterble-1.1.1/enterble.egg-info/PKG-INFO
+-rw-r--r--   0 chenyitao   (501) staff       (20)      502 2022-10-28 09:07:11.000000 enterble-1.1.1/enterble.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)        1 2022-10-28 09:07:11.000000 enterble-1.1.1/enterble.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)        1 2022-07-14 03:44:23.000000 enterble-1.1.1/enterble.egg-info/not-zip-safe
+-rw-r--r--   0 chenyitao   (501) staff       (20)       14 2022-10-28 09:07:11.000000 enterble-1.1.1/enterble.egg-info/requires.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)        9 2022-10-28 09:07:11.000000 enterble-1.1.1/enterble.egg-info/top_level.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)       38 2022-10-28 09:07:11.743687 enterble-1.1.1/setup.cfg
+-rw-r--r--   0 chenyitao   (501) staff       (20)     1523 2022-10-28 09:06:44.000000 enterble-1.1.1/setup.py
```

### Comparing `enterble-1.1.0/LICENSE` & `enterble-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enterble-1.1.0/PKG-INFO` & `enterble-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: enterble
-Version: 1.1.0
+Version: 1.1.1
 Summary: BLE device scanner and data collector for Flowtime
 Home-page: https://github.com/Entertech/Enter-Biomodule-BLE-PC-SDK.git
 Author: Lockey
 Author-email: chenyitao@entertech.cn
 License: Entertech
-Platform: UNKNOWN
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -183,9 +182,7 @@
     loop = asyncio.get_event_loop()
     # 扫描设备
     # loop.run_until_complete(device_discover())
     # 采集数据
     loop.run_until_complete(data_collector())
 
 ```
-
-
```

### Comparing `enterble-1.1.0/README.md` & `enterble-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `enterble-1.1.0/enterble/adapter/flowtime/collector.py` & `enterble-1.1.1/enterble/adapter/flowtime/collector.py`

 * *Files identical despite different names*

### Comparing `enterble-1.1.0/enterble/ble/device.py` & `enterble-1.1.1/enterble/ble/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,22 @@
         self.disconnected_callback: Optional[Callable[["BaseBleakClient"], None]] = disconnected_callback
         self.soc_col_call: Awaitable = soc_cal_call
         self.soc: SOC = SOC(soc_cal_call)
         self._client: BleakClient = None
         self.connected: bool = False
         logger.info(f'Device initialized: {self}')
 
+    async def set_disconnected_callback(self, callback: callable):
+        """设置设备断开回调函数
+
+        Args:
+            callback (callable): 设备断开回调函数
+        """
+        self.disconnected_callback = callback
+
     async def set_soc_cal_call(self, callback: callable):
         """设置电量自定义计算回调函数
 
         Args:
             callback (callable): 电量自定义计算回调函数
         """
         self.soc.soc_cal_call = callback
@@ -99,16 +107,14 @@
         """连接设备"""
         logger.info(f'Connecting to {self}')
         self._client = BleakClient(
             address_or_ble_device=self.identify,
             disconnected_callback=self.disconnected_callback,
         )
         await self._client.connect()
-        if self.disconnected_callback:
-            await self._client.set_disconnected_callback(self.disconnected_callback)
         self.connected = True
         logger.info(f'Connected to {self}')
 
     async def disconnect(self) -> None:
         """断开设备"""
         logger.info(f'Disconnecting from {self}')
         if self._client:
```

### Comparing `enterble-1.1.0/enterble/ble/scanner.py` & `enterble-1.1.1/enterble/ble/scanner.py`

 * *Files identical despite different names*

### Comparing `enterble-1.1.0/enterble/collector/collector.py` & `enterble-1.1.1/enterble/collector/collector.py`

 * *Files identical despite different names*

### Comparing `enterble-1.1.0/enterble.egg-info/PKG-INFO` & `enterble-1.1.1/enterble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: enterble
-Version: 1.1.0
+Version: 1.1.1
 Summary: BLE device scanner and data collector for Flowtime
 Home-page: https://github.com/Entertech/Enter-Biomodule-BLE-PC-SDK.git
 Author: Lockey
 Author-email: chenyitao@entertech.cn
 License: Entertech
-Platform: UNKNOWN
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -183,9 +182,7 @@
     loop = asyncio.get_event_loop()
     # 扫描设备
     # loop.run_until_complete(device_discover())
     # 采集数据
     loop.run_until_complete(data_collector())
 
 ```
-
-
```

### Comparing `enterble-1.1.0/setup.py` & `enterble-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='enterble',
-    version='1.1.0',
+    version='1.1.1',
     description='BLE device scanner and data collector for Flowtime',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         'Natural Language :: Chinese (Simplified)',
         "Development Status :: 4 - Beta",
         "Framework :: AsyncIO",
```

