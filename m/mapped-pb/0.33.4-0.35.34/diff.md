# Comparing `tmp/mapped.pb-0.33.4.tar.gz` & `tmp/mapped.pb-0.35.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapped.pb-0.33.4.tar", max compression
+gzip compressed data, was "mapped.pb-0.35.34.tar", max compression
```

## Comparing `mapped.pb-0.33.4.tar` & `mapped.pb-0.35.34.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0       41 2023-01-19 17:07:48.897054 mapped.pb-0.33.4/README.md
--rw-r--r--   0        0        0        0 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/__init__.py
--rw-r--r--   0        0        0        0 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/__init__.py
--rw-r--r--   0        0        0    19776 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/types/__init__.py
--rw-r--r--   0        0        0     1540 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/types/calendar_period_pb2.py
--rw-r--r--   0        0        0     1377 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/types/date_pb2.py
--rw-r--r--   0        0        0     1554 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/types/dayofweek_pb2.py
--rw-r--r--   0        0        0     1347 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/types/geojson_pb2.py
--rw-r--r--   0        0        0     1546 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/types/interval_pb2.py
--rw-r--r--   0        0        0     1382 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/types/money_pb2.py
--rw-r--r--   0        0        0     1629 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/types/month_pb2.py
--rw-r--r--   0        0        0     1719 2023-01-19 17:08:02.981125 mapped.pb-0.33.4/mapped_pb/cloud/types/phone_number_pb2.py
--rw-r--r--   0        0        0     1909 2023-01-19 17:08:02.977125 mapped.pb-0.33.4/mapped_pb/cloud/types/postal_address_pb2.py
--rw-r--r--   0        0        0     1484 2023-01-19 17:08:02.981125 mapped.pb-0.33.4/mapped_pb/cloud/types/timeofday_pb2.py
--rw-r--r--   0        0        0     6613 2023-01-19 17:08:02.981125 mapped.pb-0.33.4/mapped_pb/cloud/types/typed_value_pb2.py
--rw-r--r--   0        0        0     5913 2023-01-19 17:08:02.981125 mapped.pb-0.33.4/mapped_pb/gateway/__init__.py
--rw-r--r--   0        0        0     3579 2023-01-19 17:08:02.981125 mapped.pb-0.33.4/mapped_pb/gateway/edgecontrol_pb2.py
--rw-r--r--   0        0        0     1856 2023-01-19 17:08:02.981125 mapped.pb-0.33.4/mapped_pb/gateway/redispoint_pb2.py
--rw-r--r--   0        0        0      616 2023-01-19 17:08:11.401165 mapped.pb-0.33.4/pyproject.toml
--rw-r--r--   0        0        0      840 2023-01-19 17:08:12.210549 mapped.pb-0.33.4/setup.py
--rw-r--r--   0        0        0      748 2023-01-19 17:08:12.210820 mapped.pb-0.33.4/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-20 12:30:15.152968 mapped.pb-0.35.34/README.md
+-rw-r--r--   0        0        0        0 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/__init__.py
+-rw-r--r--   0        0        0    20631 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/__init__.py
+-rw-r--r--   0        0        0     1540 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/calendar_period_pb2.py
+-rw-r--r--   0        0        0     1377 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/date_pb2.py
+-rw-r--r--   0        0        0     1554 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/dayofweek_pb2.py
+-rw-r--r--   0        0        0     1347 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/geojson_pb2.py
+-rw-r--r--   0        0        0     1546 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/interval_pb2.py
+-rw-r--r--   0        0        0     2209 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/metadata_pb2.py
+-rw-r--r--   0        0        0     1382 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/money_pb2.py
+-rw-r--r--   0        0        0     1629 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/month_pb2.py
+-rw-r--r--   0        0        0     1719 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/phone_number_pb2.py
+-rw-r--r--   0        0        0     1909 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/postal_address_pb2.py
+-rw-r--r--   0        0        0     1484 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/timeofday_pb2.py
+-rw-r--r--   0        0        0     6613 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/cloud/types/typed_value_pb2.py
+-rw-r--r--   0        0        0     5913 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/gateway/__init__.py
+-rw-r--r--   0        0        0     3579 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/gateway/edgecontrol_pb2.py
+-rw-r--r--   0        0        0     1856 2023-03-20 12:30:35.277069 mapped.pb-0.35.34/mapped_pb/gateway/redispoint_pb2.py
+-rw-r--r--   0        0        0      617 2023-03-20 12:30:45.781131 mapped.pb-0.35.34/pyproject.toml
+-rw-r--r--   0        0        0      841 2023-03-20 12:30:47.045638 mapped.pb-0.35.34/setup.py
+-rw-r--r--   0        0        0      749 2023-03-20 12:30:47.045964 mapped.pb-0.35.34/PKG-INFO
```

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/__init__.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: mapped/cloud/types/calendar_period.proto, mapped/cloud/types/date.proto, mapped/cloud/types/dayofweek.proto, mapped/cloud/types/geojson.proto, mapped/cloud/types/interval.proto, mapped/cloud/types/money.proto, mapped/cloud/types/month.proto, mapped/cloud/types/phone_number.proto, mapped/cloud/types/postal_address.proto, mapped/cloud/types/timeofday.proto, mapped/cloud/types/typed_value.proto
+# sources: mapped/cloud/types/calendar_period.proto, mapped/cloud/types/date.proto, mapped/cloud/types/dayofweek.proto, mapped/cloud/types/geojson.proto, mapped/cloud/types/interval.proto, mapped/cloud/types/metadata.proto, mapped/cloud/types/money.proto, mapped/cloud/types/month.proto, mapped/cloud/types/phone_number.proto, mapped/cloud/types/postal_address.proto, mapped/cloud/types/timeofday.proto, mapped/cloud/types/typed_value.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 from datetime import datetime
 from typing import (
     Dict,
     List,
 )
@@ -188,14 +188,38 @@
     """
     Optional. Exclusive end of the interval. If specified, a Timestamp matching
     this interval will have to be before the end.
     """
 
 
 @dataclass(eq=False, repr=False)
+class MetadataRecord(betterproto.Message):
+    key: str = betterproto.string_field(1)
+    value: str = betterproto.string_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class MetadataValue(betterproto.Message):
+    values: List["MetadataRecord"] = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class MetadataUpdate(betterproto.Message):
+    granular: "MetadataUpdateGranular" = betterproto.message_field(1, group="update")
+    replace: "MetadataValue" = betterproto.message_field(2, group="update")
+
+
+@dataclass(eq=False, repr=False)
+class MetadataUpdateGranular(betterproto.Message):
+    add: List["MetadataRecord"] = betterproto.message_field(1)
+    remove: List["MetadataRecord"] = betterproto.message_field(2)
+    remove_all: List[str] = betterproto.string_field(3)
+
+
+@dataclass(eq=False, repr=False)
 class Money(betterproto.Message):
     """Represents an amount of money with its currency type."""
 
     currency_code: str = betterproto.string_field(1)
     """The three-letter currency code defined in ISO 4217."""
 
     units: int = betterproto.int64_field(2)
```

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/calendar_period_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/calendar_period_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/date_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/date_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/dayofweek_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/dayofweek_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/geojson_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/geojson_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/interval_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/interval_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/money_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/money_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/month_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/month_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/phone_number_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/phone_number_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/postal_address_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/postal_address_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/timeofday_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/timeofday_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/cloud/types/typed_value_pb2.py` & `mapped.pb-0.35.34/mapped_pb/cloud/types/typed_value_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/gateway/__init__.py` & `mapped.pb-0.35.34/mapped_pb/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/gateway/edgecontrol_pb2.py` & `mapped.pb-0.35.34/mapped_pb/gateway/edgecontrol_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/mapped_pb/gateway/redispoint_pb2.py` & `mapped.pb-0.35.34/mapped_pb/gateway/redispoint_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped.pb-0.33.4/pyproject.toml` & `mapped.pb-0.35.34/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mapped.pb"
-version = "0.33.4"
+version = "0.35.34"
 description = "public Mapped Platform Service Definitions using protobuf"
 authors = ["Mapped <support@mapped.com>"]
 license = "Apache-2.0"
 homepage = "https://www.mapped.com"
 repository = "https://github.com/mapped/pb"
 keywords = ["mapped", "protobuf"]
 readme = "README.md"
```

### Comparing `mapped.pb-0.33.4/setup.py` & `mapped.pb-0.35.34/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['betterproto==2.0.0b5', 'grpclib==0.4.3']
 
 setup_kwargs = {
     'name': 'mapped.pb',
-    'version': '0.33.4',
+    'version': '0.35.34',
     'description': 'public Mapped Platform Service Definitions using protobuf',
     'long_description': '# Mapped Public Proto Package for Python\n',
     'author': 'Mapped',
     'author_email': 'support@mapped.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.mapped.com',
```

### Comparing `mapped.pb-0.33.4/PKG-INFO` & `mapped.pb-0.35.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapped.pb
-Version: 0.33.4
+Version: 0.35.34
 Summary: public Mapped Platform Service Definitions using protobuf
 Home-page: https://www.mapped.com
 License: Apache-2.0
 Keywords: mapped,protobuf
 Author: Mapped
 Author-email: support@mapped.com
 Requires-Python: >=3.8,<4.0
```

