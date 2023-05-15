# Comparing `tmp/touchprice-0.1.5.tar.gz` & `tmp/touchprice-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "touchprice-0.1.5.tar", max compression
+gzip compressed data, was "touchprice-0.1.6.tar", max compression
```

## Comparing `touchprice-0.1.5.tar` & `touchprice-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      478 2023-03-29 02:14:23.359548 touchprice-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      248 2023-03-29 02:14:09.531573 touchprice-0.1.5/touchprice/__init__.py
--rw-r--r--   0        0        0     3681 2023-03-29 02:14:09.531573 touchprice-0.1.5/touchprice/condition.py
--rw-r--r--   0        0        0      280 2023-03-29 02:14:09.531573 touchprice-0.1.5/touchprice/constant.py
--rw-r--r--   0        0        0     2299 2023-03-29 02:14:09.531573 touchprice-0.1.5/touchprice/core.py
--rw-r--r--   0        0        0     9780 2023-03-29 02:14:09.531573 touchprice-0.1.5/touchprice/touch_price.py
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 touchprice-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      478 2023-05-15 02:07:15.098836 touchprice-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      248 2023-05-15 02:07:02.274384 touchprice-0.1.6/touchprice/__init__.py
+-rw-r--r--   0        0        0     3681 2023-05-15 02:07:02.274384 touchprice-0.1.6/touchprice/condition.py
+-rw-r--r--   0        0        0      280 2023-05-15 02:07:02.274384 touchprice-0.1.6/touchprice/constant.py
+-rw-r--r--   0        0        0     2299 2023-05-15 02:07:02.274384 touchprice-0.1.6/touchprice/core.py
+-rw-r--r--   0        0        0     9968 2023-05-15 02:07:02.274384 touchprice-0.1.6/touchprice/touch_price.py
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 touchprice-0.1.6/PKG-INFO
```

### Comparing `touchprice-0.1.5/touchprice/condition.py` & `touchprice-0.1.6/touchprice/condition.py`

 * *Files identical despite different names*

### Comparing `touchprice-0.1.5/touchprice/core.py` & `touchprice-0.1.6/touchprice/core.py`

 * *Files identical despite different names*

### Comparing `touchprice-0.1.5/touchprice/touch_price.py` & `touchprice-0.1.6/touchprice/touch_price.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import shioaji as sj
 import typing
 import datetime
+from shioaji import TickSTKv1, Exchange, BidAskSTKv1
 from pydantic import StrictInt
 from functools import partial
 from touchprice.constant import Trend, PriceType
 from touchprice.condition import (
     Price,
     TouchOrderCond,
     OrderCmd,
@@ -32,15 +33,18 @@
     def __init__(self, api: sj.Shioaji):
         self.api: sj.Shioaji = api
         self.conditions: typing.Dict[
             str, typing.List[typing.Union[StoreLossProfit, StoreCond]]
         ] = {}
         self.infos: typing.Dict[str, StatusInfo] = {}
         self.contracts: dict = get_contracts(self.api)
-        self.api.quote.set_on_tick_stk_v1_callback(self.integration)
+        self.api.quote.set_on_tick_stk_v1_callback(self.integration_tick)
+        self.api.quote.set_on_tick_fop_v1_callback(self.integration_tick)
+        self.api.quote.set_on_bidask_stk_v1_callback(self.integration_bidask)
+        self.api.quote.set_on_bidask_fop_v1_callback(self.integration_bidask)
         self.orders: typing.Dict[str, typing.Dict[str, StoreLossProfit]] = {}
 
     def update_snapshot(self, contract: sj.contracts.Contract):
         code = contract.code
         if code not in self.infos.keys():
             snapshot = self.api.snapshots([contract])[0]
             self.infos[code] = StatusInfo(**snapshot)
@@ -159,49 +163,53 @@
                             self.conditions[code][num].excuted = True
                             self.conditions[code][num].result = self.api.place_order(
                                 order_contract,
                                 order,
                                 cb=self.conditions[code][num].excuted_cb,
                             )
 
-    def integration(self, topic: str, quote: dict):
-        if "Simtrade" in quote.keys():
+    def integration_bidask(self, exchange: Exchange, bidask: BidAskSTKv1):
+        if bidask.simtrade == 1:
             pass
-        elif topic.startswith("MKT/") or topic.startswith("L/"):
-            code = topic.split("/")[-1]
+        else:
+            code = bidask.code
+            if code in self.infos.keys():
+                info = self.infos[code]
+                if 0 not in bidask.ask_volume:
+                    info.buy_price = bidask.bid_price[0]
+                    info.sell_price = bidask.ask_price[0]
+                    self.touch(code)
+
+    def integration_tick(self, exchange: Exchange, tick: TickSTKv1):
+        if tick.simtrade == 1:
+            pass
+        else:
+            code = tick.code
             if code in self.infos.keys():
                 info = self.infos[code]
-                info.close = quote["Close"][0]
-                info.high = info.close if info.high < info.close else info.high
-                info.low = info.close if info.low > info.close else info.low
-                info.total_volume = quote["VolSum"][0]
-                info.volume = quote["Volume"][0]
-                if quote["TickType"][0] == 1:
+                info.close = tick.close
+                info.high = tick.high
+                info.low = tick.low
+                info.total_volume = tick.total_volume
+                info.volume = tick.volume
+                if tick.tick_type == 1:
                     info.ask_volume = (
                         info.ask_volume + info.volume
                         if info.ask_volume
                         else info.volume
                     )
                     info.bid_volume = 0
-                elif quote["TickType"][0] == 2:
+                elif tick.tick_type == 2:
                     info.bid_volume = (
                         info.bid_volume + info.volume
                         if info.bid_volume
                         else info.volume
                     )
                     info.ask_volume = 0
                 self.touch(code)
-        elif topic.startswith("QUT/") or topic.startswith("Q/"):
-            code = topic.split("/")[-1]
-            if code in self.infos.keys():
-                info = self.infos[code]
-                if 0 not in quote["AskVolume"]:
-                    info.buy_price = quote["BidPrice"][0]
-                    info.sell_price = quote["AskPrice"][0]
-                    self.touch(code)
 
     def show_condition(self, code: str = None):
         if not code:
             return self.conditions
         else:
             return self.conditions[code]
```

### Comparing `touchprice-0.1.5/PKG-INFO` & `touchprice-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: touchprice
-Version: 0.1.5
+Version: 0.1.6
 Summary: shioaji touchprice extentions
 Author: Sally
 Author-email: nipolikae@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

