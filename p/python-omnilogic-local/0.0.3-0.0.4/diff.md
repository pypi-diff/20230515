# Comparing `tmp/python_omnilogic_local-0.0.3.tar.gz` & `tmp/python_omnilogic_local-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.0.3.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.0.4.tar", max compression
```

## Comparing `python_omnilogic_local-0.0.3.tar` & `python_omnilogic_local-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1697 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.3/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    30393 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.3/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     1763 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.3/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0     1674 2023-05-10 23:14:12.231775 python_omnilogic_local-0.0.3/pyomnilogic_local/types.py
--rw-r--r--   0        0        0     1414 2023-05-15 14:56:48.568207 python_omnilogic_local-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 python_omnilogic_local-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1697 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.4/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    31758 2023-05-15 17:24:18.872678 python_omnilogic_local-0.0.4/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     1763 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.4/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0     1674 2023-05-10 23:14:12.231775 python_omnilogic_local-0.0.4/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0     1414 2023-05-15 17:24:38.628964 python_omnilogic_local-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 python_omnilogic_local-0.0.4/PKG-INFO
```

### Comparing `python_omnilogic_local-0.0.3/README.md` & `python_omnilogic_local-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.0.3/pyomnilogic_local/api.py` & `python_omnilogic_local-0.0.4/pyomnilogic_local/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import time
 from typing import Union
 import xml.etree.ElementTree as ET
 import zlib
 
 from .types import ColorLogicBrightness, ColorLogicShow, ColorLogicSpeed, MessageType
 
+_LOGGER = logging.getLogger(__name__)
+
 
 class OmniLogicRequest:
     HEADER_FORMAT = "!LQ4sLBBBB"
 
     def __init__(self, msg_id, msg_type: MessageType, extra_data="", client_type=1):
         self.msg_id = msg_id
         self.msg_type = msg_type
@@ -30,15 +32,15 @@
             bytes(self.version),  # version string
             self.msg_type.value,  # OpID/msgType
             self.client_type,  # Client type
             0,  # reserved
             0,  # compressed
             0,  # reserved
         )
-        # logging.debug(retval+self.extra_data)
+        # _LOGGER.debug(retval+self.extra_data)
         return retval + self.extra_data
 
     @staticmethod
     def from_bytes(data):
         # split the header and data
         header = data[0:24]
         rdata = data[24:]
@@ -289,20 +291,20 @@
         msg_id, _, _, msg_type, _, _, compressed, _, data = OmniLogicRequest.from_bytes(data)
         self.data_queue.put_nowait((msg_id, msg_type, compressed, data))
 
     def error_received(self, exc):
         raise exc
 
     async def _send_request(self, msg_type, extra_data="", msg_id=None):
-        logging.debug("Sending Message Type: %s, Request Body: %s", msg_type.name, extra_data)
-
         # If we aren't sending a specific msg_id, lets randomize it
         if not msg_id:
             msg_id = random.randrange(2**32)
 
+        _LOGGER.debug("Sending Message ID: %s, Message Type: %s, Request Body: %s", msg_id, msg_type.name, extra_data)
+
         # If we are speaking the XML API, it seems like we need client_type 0, otherwise we need client_type 1
         client_type = 0 if extra_data != "" else 1
 
         # The Hayward API terminates it's messages with a null character
         extra_data += "\x00" if extra_data != "" else ""
 
         request = OmniLogicRequest(msg_id, msg_type, extra_data, client_type)
@@ -322,21 +324,44 @@
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
         await self._send_request(MessageType.XML_ACK, req_body, msg_id)
 
     async def _receive_file(self):
         # wait for the initial packet.
         msg_id, msg_type, compressed, data = await self.data_queue.get()
+        if compressed:
+            _LOGGER.debug("Received compressed message ID: %s, Type: %s", msg_id, msg_type)
+        else:
+            _LOGGER.debug("Received Message ID: %s, Type: %s", msg_id, msg_type)
 
         await self._send_ack(msg_id)
 
         # Check if the 23rd bit of the header (compressed bit) was a 1
         # There are also some messages that are ALWAYS compressed although they do not return a 1 in their LeadMessage
         msg_compressed = compressed == 1 or msg_type in [MessageType.MSP_TELEMETRY_UPDATE]
 
+        # # If the response is too large, the controller will send a LeadMessage indicating how many follow-up messages will be sent
+        # if msg_type == MessageType.MSP_LEADMESSAGE:
+        #     # Parse XML
+        #     root = ET.fromstring(data[:-1])  # strip trailing \x00
+        #     block_count = int(root.findall(".//*[@name='MsgBlockCount']")[0].text)
+
+        #     # Wait for the block data data
+        #     retval = b""
+        #     # If we received a LeadMessage, continue to receive messages until we have all of our data
+        #     # Chunks of data may arrive out of order, so we store them in a buffer as they arrive and sort them after
+        #     data_chunks: dict = {}
+        #     for _ in range(block_count):
+        #         msg_id, msg_type, compressed, data = await self.data_queue.get()
+        #         await self._send_ack(msg_id)
+        #         # remove an 8 byte header to get to the payload data
+        #         data_chunks[msg_id] = data[8:]
+        #     for msg_id, data in sorted(data_chunks.items()):
+        #         retval += data
+
         # If the response is too large, the controller will send a LeadMessage indicating how many follow-up messages will be sent
         if msg_type == MessageType.MSP_LEADMESSAGE:
             # Parse XML
             root = ET.fromstring(data[:-1])  # strip trailing \x00
             block_count = int(root.findall(".//*[@name='MsgBlockCount']")[0].text)
 
             # Wait for the block data data
```

### Comparing `python_omnilogic_local-0.0.3/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.0.4/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.0.3/pyomnilogic_local/types.py` & `python_omnilogic_local-0.0.4/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.0.3/pyproject.toml` & `python_omnilogic_local-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.0.3"
+version = "0.0.4"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.0.3/PKG-INFO` & `python_omnilogic_local-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.0.3 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.0.4 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

