# Comparing `tmp/pb_encoding-0.2.0.tar.gz` & `tmp/pb_encoding-0.3.0.tar.gz`

## Comparing `pb_encoding-0.2.0.tar` & `pb_encoding-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/src/pb_encoding/__init__.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/src/pb_encoding/decoder.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/src/pb_encoding/encoder.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/src/pb_encoding/typing.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/.gitignore
--rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/LICENSE
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/LICENSE_origin
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/README.md
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/src/pb_encoding/__init__.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/src/pb_encoding/decoder.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/src/pb_encoding/encoder.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/src/pb_encoding/typing.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/LICENSE_origin
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/README.md
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pb_encoding-0.3.0/PKG-INFO
```

### Comparing `pb_encoding-0.2.0/src/pb_encoding/decoder.py` & `pb_encoding-0.3.0/src/pb_encoding/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import struct
-from typing import Any, Tuple, Callable
+from typing import Any, Tuple, Callable, Union
 
 from .typing import SupportedType
 
 __all__ = (
     "DecodeField",
     "getDecoder",
+    "UnpackField",
 )
 
 
 def _VarintDecoder(mask, result_type):
     def DecodeVarint(buffer, pos):
         result = 0
         shift = 0
@@ -124,7 +125,13 @@
 
 def getDecoder(type: SupportedType) -> Callable:
     return _field_decoder_mapping[type]
 
 
 def DecodeField(type: SupportedType, buffer, pos: int) -> Tuple[Any, int]:
     return _field_decoder_mapping[type](buffer, pos)
+
+
+def UnpackField(type: SupportedType, buffer) -> Union[str, int, float, bytes]:
+    pos = 0
+    value, _ = DecodeField(type, buffer, pos)
+    return value
```

### Comparing `pb_encoding-0.2.0/src/pb_encoding/encoder.py` & `pb_encoding-0.3.0/src/pb_encoding/encoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Callable, Any
 
 from .typing import SupportedType
 
 __all__ = (
     "EncodeField",
     "getEncoder",
+    "PackField",
 )
 
 
 def EncodeVarint(write, value):
     local_int2byte = struct.Struct(">B").pack
     bits = value & 0x7F
     value >>= 7
@@ -85,7 +86,13 @@
 
 def getEncoder(type: SupportedType) -> Callable:
     return _field_encoder_mapping[type]
 
 
 def EncodeField(type: SupportedType, write: Callable[[bytes], Any], value: Any) -> None:
     return _field_encoder_mapping[type](write, value)
+
+
+def PackField(type: SupportedType, value) -> bytes:
+    b = bytearray()
+    EncodeField(type, b.__iadd__, value)
+    return bytes(b)
```

### Comparing `pb_encoding-0.2.0/.gitignore` & `pb_encoding-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pb_encoding-0.2.0/LICENSE` & `pb_encoding-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pb_encoding-0.2.0/LICENSE_origin` & `pb_encoding-0.3.0/LICENSE_origin`

 * *Files identical despite different names*

### Comparing `pb_encoding-0.2.0/pyproject.toml` & `pb_encoding-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pb_encoding-0.2.0/PKG-INFO` & `pb_encoding-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pb_encoding
-Version: 0.2.0
+Version: 0.3.0
 Summary: Some encode/decode functions extracted from google.protobuf
 Project-URL: homepage, https://github.com/Grvzard/pb_encoding
 License-File: LICENSE
 License-File: LICENSE_origin
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

