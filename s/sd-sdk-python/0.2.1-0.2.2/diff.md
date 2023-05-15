# Comparing `tmp/sd_sdk_python-0.2.1.tar.gz` & `tmp/sd_sdk_python-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_sdk_python-0.2.1.tar", max compression
+gzip compressed data, was "sd_sdk_python-0.2.2.tar", max compression
```

## Comparing `sd_sdk_python-0.2.1.tar` & `sd_sdk_python-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/LICENSE
--rw-r--r--   0        0        0      636 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/README.md
--rw-r--r--   0        0        0     1080 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2783 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/sd_sdk_python/__init__.py
--rw-r--r--   0        0        0    12488 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/sd_sdk_python/sd_sdk.py
--rw-r--r--   0        0        0    13130 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/sd_sdk_python/sd_sdk_wireless.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 sd_sdk_python-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-15 21:02:02.654724 sd_sdk_python-0.2.2/LICENSE
+-rw-r--r--   0        0        0      636 2023-05-15 21:02:02.654724 sd_sdk_python-0.2.2/README.md
+-rw-r--r--   0        0        0     1080 2023-05-15 21:02:02.654724 sd_sdk_python-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2783 2023-05-15 21:02:02.654724 sd_sdk_python-0.2.2/sd_sdk_python/__init__.py
+-rw-r--r--   0        0        0    12568 2023-05-15 21:02:02.658723 sd_sdk_python-0.2.2/sd_sdk_python/sd_sdk.py
+-rw-r--r--   0        0        0    13130 2023-05-15 21:02:02.658723 sd_sdk_python-0.2.2/sd_sdk_python/sd_sdk_wireless.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 sd_sdk_python-0.2.2/PKG-INFO
```

### Comparing `sd_sdk_python-0.2.1/LICENSE` & `sd_sdk_python-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.1/README.md` & `sd_sdk_python-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.1/pyproject.toml` & `sd_sdk_python-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sd-sdk-python"
 homepage = "https://github.com/markmelvin-onsemi/sd-sdk-python"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python helper module for the Sound Designer SDK"
 authors = ["Mark Melvin <mark.melvin@onsemi.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `sd_sdk_python-0.2.1/sd_sdk_python/__init__.py` & `sd_sdk_python-0.2.2/sd_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.1/sd_sdk_python/sd_sdk.py` & `sd_sdk_python-0.2.2/sd_sdk_python/sd_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     valid: bool = False
     locked: bool = False
     radio_application_version: str = ""
     radio_bootloader_version: str = ""
     radio_soft_device_version: str = ""
     hybrid_serial: int = 0
     hybrid_revision: int = 0
+    hybrid_tester: int = 0
 
     def __post_init__(self):
         assert self._info is not None
         self.library_id = self._info.LibraryId
         self.product_id = self._info.ProductId
         self.chip_id = self._info.ChipId
         self.chip_version = self._info.ChipVersion
@@ -66,14 +67,15 @@
         self.valid = self._info.IsValid
         self.locked = self._info.ParameterLockState
         self.radio_application_version = self._info.RadioApplicationVersion
         self.radio_bootloader_version = self._info.RadioBootloaderVersion
         self.radio_soft_device_version = self._info.RadioSoftDeviceVersion
         self.hybrid_serial = self._info.HybridSerial
         self.hybrid_revision = self._info.HybridRevision
+        self.hybrid_tester = self._info.HybridTester
 
     def to_dict(self,) -> dict:
         return {k:v for k,v in self.__dict__.items() if not k.startswith('_')}
 
 @dataclass
 class Ezairo:
     sd: object
```

### Comparing `sd_sdk_python-0.2.1/sd_sdk_python/sd_sdk_wireless.py` & `sd_sdk_python-0.2.2/sd_sdk_python/sd_sdk_wireless.py`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.1/PKG-INFO` & `sd_sdk_python-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-sdk-python
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python helper module for the Sound Designer SDK
 Home-page: https://github.com/markmelvin-onsemi/sd-sdk-python
 License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@onsemi.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

