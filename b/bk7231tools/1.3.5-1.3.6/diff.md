# Comparing `tmp/bk7231tools-1.3.5.tar.gz` & `tmp/bk7231tools-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk7231tools-1.3.5.tar", max compression
+gzip compressed data, was "bk7231tools-1.3.6.tar", max compression
```

## Comparing `bk7231tools-1.3.5.tar` & `bk7231tools-1.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1083 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/LICENSE
--rwxr-xr-x   0        0        0       26 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/__init__.py
--rw-r--r--   0        0        0    20269 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/__main__.py
--rw-r--r--   0        0        0        0 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/analysis/__init__.py
--rw-r--r--   0        0        0      570 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/analysis/crc16.py
--rw-r--r--   0        0        0      707 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/analysis/flash.py
--rw-r--r--   0        0        0     6033 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/analysis/goto.py
--rw-r--r--   0        0        0     6209 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/analysis/rbl.py
--rw-r--r--   0        0        0    10785 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/analysis/storage.py
--rw-r--r--   0        0        0      257 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/analysis/utils.py
--rw-r--r--   0        0        0        0 2023-05-13 15:30:22.250465 bk7231tools-1.3.5/bk7231tools/crypto/__init__.py
--rw-r--r--   0        0        0     5803 2023-05-13 15:30:22.254465 bk7231tools-1.3.5/bk7231tools/crypto/code.py
--rw-r--r--   0        0        0      128 2023-05-13 15:30:22.254465 bk7231tools-1.3.5/bk7231tools/crypto/util.py
--rw-r--r--   0        0        0     5402 2023-05-13 15:30:22.254465 bk7231tools-1.3.5/bk7231tools/serial/__init__.py
--rw-r--r--   0        0        0     4946 2023-05-13 15:30:22.254465 bk7231tools-1.3.5/bk7231tools/serial/cmd_chip.py
--rw-r--r--   0        0        0     7112 2023-05-13 15:30:22.254465 bk7231tools-1.3.5/bk7231tools/serial/cmd_flash.py
--rw-r--r--   0        0        0     6068 2023-05-13 15:30:22.254465 bk7231tools-1.3.5/bk7231tools/serial/packets.py
--rw-r--r--   0        0        0     8106 2023-05-13 15:30:22.254465 bk7231tools-1.3.5/bk7231tools/serial/protocol.py
--rw-r--r--   0        0        0      140 2023-05-13 15:30:22.254465 bk7231tools-1.3.5/bk7231tools/serial/utils.py
--rw-r--r--   0        0        0      604 2023-05-13 15:30:22.254465 bk7231tools-1.3.5/pyproject.toml
--rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 bk7231tools-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/LICENSE
+-rwxr-xr-x   0        0        0       26 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/__init__.py
+-rw-r--r--   0        0        0    20269 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/analysis/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/analysis/crc16.py
+-rw-r--r--   0        0        0      707 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/analysis/flash.py
+-rw-r--r--   0        0        0     6033 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/analysis/goto.py
+-rw-r--r--   0        0        0     6209 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/analysis/rbl.py
+-rw-r--r--   0        0        0    11129 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/analysis/storage.py
+-rw-r--r--   0        0        0      257 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/analysis/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/crypto/__init__.py
+-rw-r--r--   0        0        0     5803 2023-05-15 18:26:05.879099 bk7231tools-1.3.6/bk7231tools/crypto/code.py
+-rw-r--r--   0        0        0      128 2023-05-15 18:26:05.883099 bk7231tools-1.3.6/bk7231tools/crypto/util.py
+-rw-r--r--   0        0        0     5402 2023-05-15 18:26:05.883099 bk7231tools-1.3.6/bk7231tools/serial/__init__.py
+-rw-r--r--   0        0        0     4946 2023-05-15 18:26:05.883099 bk7231tools-1.3.6/bk7231tools/serial/cmd_chip.py
+-rw-r--r--   0        0        0     7112 2023-05-15 18:26:05.883099 bk7231tools-1.3.6/bk7231tools/serial/cmd_flash.py
+-rw-r--r--   0        0        0     6068 2023-05-15 18:26:05.883099 bk7231tools-1.3.6/bk7231tools/serial/packets.py
+-rw-r--r--   0        0        0     8106 2023-05-15 18:26:05.883099 bk7231tools-1.3.6/bk7231tools/serial/protocol.py
+-rw-r--r--   0        0        0      140 2023-05-15 18:26:05.883099 bk7231tools-1.3.6/bk7231tools/serial/utils.py
+-rw-r--r--   0        0        0      604 2023-05-15 18:26:05.883099 bk7231tools-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 bk7231tools-1.3.6/PKG-INFO
```

### Comparing `bk7231tools-1.3.5/LICENSE` & `bk7231tools-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/__main__.py` & `bk7231tools-1.3.6/bk7231tools/__main__.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/analysis/crc16.py` & `bk7231tools-1.3.6/bk7231tools/analysis/crc16.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/analysis/flash.py` & `bk7231tools-1.3.6/bk7231tools/analysis/flash.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/analysis/goto.py` & `bk7231tools-1.3.6/bk7231tools/analysis/goto.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/analysis/rbl.py` & `bk7231tools-1.3.6/bk7231tools/analysis/rbl.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/analysis/storage.py` & `bk7231tools-1.3.6/bk7231tools/analysis/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,25 +123,31 @@
 
     def load(self, file: str) -> int:
         self.dumpfile = file
         with open(file, "rb") as f:
             filedata = f.read()
         return self.load_raw(filedata)
 
-    def load_raw(self, filedata: bytes) -> int:
+    def load_raw(self, filedata: bytes, allow_incomplete: bool = False) -> int:
         magic = bytes.fromhex(KEY_MAGIC) * 4
         try:
             pos = filedata.index(magic)
             pos -= 32  # rewind to block start
         except ValueError:
             return None
         self.data = filedata[pos: pos + self.flash_sz + self.swap_flash_sz]
         self.data = bytearray(self.data)
         if len(self.data) != self.flash_sz + self.swap_flash_sz:
-            return None
+            if len(self.data) & 0xFFF:
+                return None
+            if allow_incomplete and len(self.data) >= 0x2000:
+                flash_sz = min(self.flash_sz, len(self.data) - 0x1000)
+                self.__init__(flash_sz=flash_sz, swap_flash_sz=len(self.data) - flash_sz)
+            else:
+                return None
         return pos
 
     def save(self, file: str):
         with open(file, "wb") as f:
             f.write(self.data)
 
     def block(self, i: int, new: bytearray = None) -> bytearray:
```

### Comparing `bk7231tools-1.3.5/bk7231tools/crypto/code.py` & `bk7231tools-1.3.6/bk7231tools/crypto/code.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/serial/__init__.py` & `bk7231tools-1.3.6/bk7231tools/serial/__init__.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/serial/cmd_chip.py` & `bk7231tools-1.3.6/bk7231tools/serial/cmd_chip.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/serial/cmd_flash.py` & `bk7231tools-1.3.6/bk7231tools/serial/cmd_flash.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/serial/packets.py` & `bk7231tools-1.3.6/bk7231tools/serial/packets.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/bk7231tools/serial/protocol.py` & `bk7231tools-1.3.6/bk7231tools/serial/protocol.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.5/pyproject.toml` & `bk7231tools-1.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bk7231tools"
-version = "1.3.5"
+version = "1.3.6"
 description = "Tools to interact with and analyze artifacts for BK7231 MCUs"
 authors = ["Khaled Nassar <kmhnassar@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyserial = "^3.5"
```

### Comparing `bk7231tools-1.3.5/PKG-INFO` & `bk7231tools-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bk7231tools
-Version: 1.3.5
+Version: 1.3.6
 Summary: Tools to interact with and analyze artifacts for BK7231 MCUs
 License: MIT
 Author: Khaled Nassar
 Author-email: kmhnassar@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

