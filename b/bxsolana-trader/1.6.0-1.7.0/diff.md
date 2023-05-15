# Comparing `tmp/bxsolana-trader-1.6.0.tar.gz` & `tmp/bxsolana-trader-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bxsolana-trader-1.6.0.tar", last modified: Thu Apr 27 20:19:29 2023, max compression
+gzip compressed data, was "bxsolana-trader-1.7.0.tar", last modified: Mon May 15 16:28:15 2023, max compression
```

## Comparing `bxsolana-trader-1.6.0.tar` & `bxsolana-trader-1.7.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.838762 bxsolana-trader-1.6.0/
--rw-r--r--   0 aspin      (501) staff       (20)     1071 2022-09-13 19:43:40.000000 bxsolana-trader-1.6.0/LICENSE
--rw-r--r--   0 aspin      (501) staff       (20)     4346 2023-04-27 20:19:29.838836 bxsolana-trader-1.6.0/PKG-INFO
--rw-r--r--   0 aspin      (501) staff       (20)     2865 2023-04-24 22:32:24.000000 bxsolana-trader-1.6.0/README.md
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.830409 bxsolana-trader-1.6.0/bxsolana/
--rw-r--r--   0 aspin      (501) staff       (20)      280 2023-01-10 20:47:33.000000 bxsolana-trader-1.6.0/bxsolana/__init__.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.832968 bxsolana-trader-1.6.0/bxsolana/examples/
--rw-r--r--   0 aspin      (501) staff       (20)      672 2023-01-10 20:47:33.000000 bxsolana-trader-1.6.0/bxsolana/examples/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)      617 2023-02-21 21:35:54.000000 bxsolana-trader-1.6.0/bxsolana/examples/constants.py
--rw-r--r--   0 aspin      (501) staff       (20)     2638 2022-12-21 21:25:04.000000 bxsolana-trader-1.6.0/bxsolana/examples/order_lifecycle.py
--rw-r--r--   0 aspin      (501) staff       (20)     6862 2023-01-10 20:47:33.000000 bxsolana-trader-1.6.0/bxsolana/examples/order_utils.py
--rw-r--r--   0 aspin      (501) staff       (20)    13092 2023-04-24 22:32:24.000000 bxsolana-trader-1.6.0/bxsolana/examples/request_utils.py
--rw-r--r--   0 aspin      (501) staff       (20)     3501 2023-04-24 22:32:24.000000 bxsolana-trader-1.6.0/bxsolana/examples/stream_utils.py
--rw-r--r--   0 aspin      (501) staff       (20)     5638 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/examples/transaction_request_utils.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.834972 bxsolana-trader-1.6.0/bxsolana/provider/
--rw-r--r--   0 aspin      (501) staff       (20)      582 2022-10-10 22:32:15.000000 bxsolana-trader-1.6.0/bxsolana/provider/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)    10174 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/provider/base.py
--rw-r--r--   0 aspin      (501) staff       (20)      970 2023-02-20 23:04:33.000000 bxsolana-trader-1.6.0/bxsolana/provider/constants.py
--rw-r--r--   0 aspin      (501) staff       (20)     2946 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/provider/grpc.py
--rw-r--r--   0 aspin      (501) staff       (20)    28223 2023-04-24 22:32:24.000000 bxsolana-trader-1.6.0/bxsolana/provider/http.py
--rw-r--r--   0 aspin      (501) staff       (20)      947 2023-03-06 23:02:29.000000 bxsolana-trader-1.6.0/bxsolana/provider/http_error.py
--rw-r--r--   0 aspin      (501) staff       (20)     3888 2023-04-27 20:19:19.000000 bxsolana-trader-1.6.0/bxsolana/provider/ws.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.835884 bxsolana-trader-1.6.0/bxsolana/transaction/
--rw-r--r--   0 aspin      (501) staff       (20)      593 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/bxsolana/transaction/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)     2361 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/transaction/memo.py
--rw-r--r--   0 aspin      (501) staff       (20)     2402 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/transaction/signing.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.836631 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/
--rw-r--r--   0 aspin      (501) staff       (20)     4346 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/PKG-INFO
--rw-r--r--   0 aspin      (501) staff       (20)     1138 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/SOURCES.txt
--rw-r--r--   0 aspin      (501) staff       (20)        1 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/dependency_links.txt
--rw-r--r--   0 aspin      (501) staff       (20)      174 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/requires.txt
--rw-r--r--   0 aspin      (501) staff       (20)       14 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/top_level.txt
--rw-r--r--   0 aspin      (501) staff       (20)      217 2022-09-07 21:30:01.000000 bxsolana-trader-1.6.0/pyproject.toml
--rw-r--r--   0 aspin      (501) staff       (20)      707 2023-04-27 20:19:29.839160 bxsolana-trader-1.6.0/setup.cfg
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.836753 bxsolana-trader-1.6.0/test/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/__init__.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.838067 bxsolana-trader-1.6.0/test/integration/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)     4020 2023-02-20 23:04:33.000000 bxsolana-trader-1.6.0/test/integration/private.py
--rw-r--r--   0 aspin      (501) staff       (20)     2192 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/public.py
--rw-r--r--   0 aspin      (501) staff       (20)      852 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/stream.py
--rw-r--r--   0 aspin      (501) staff       (20)      701 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/test_grpc.py
--rw-r--r--   0 aspin      (501) staff       (20)      544 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/test_http.py
--rw-r--r--   0 aspin      (501) staff       (20)      664 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/test_ws.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.838259 bxsolana-trader-1.6.0/test/unit/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/unit/__init__.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.838626 bxsolana-trader-1.6.0/test/unit/transaction/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/unit/transaction/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)     1386 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/test/unit/transaction/test_memo.py
--rw-r--r--   0 aspin      (501) staff       (20)     4629 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/test/unit/transaction/test_signing.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.903853 bxsolana-trader-1.7.0/
+-rw-r--r--   0 aspin      (501) staff       (20)     1071 2022-09-13 19:43:40.000000 bxsolana-trader-1.7.0/LICENSE
+-rw-r--r--   0 aspin      (501) staff       (20)     4348 2023-05-15 16:28:15.903951 bxsolana-trader-1.7.0/PKG-INFO
+-rw-r--r--   0 aspin      (501) staff       (20)     2867 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/README.md
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.870430 bxsolana-trader-1.7.0/bxsolana/
+-rw-r--r--   0 aspin      (501) staff       (20)      280 2023-01-10 20:47:33.000000 bxsolana-trader-1.7.0/bxsolana/__init__.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.894985 bxsolana-trader-1.7.0/bxsolana/examples/
+-rw-r--r--   0 aspin      (501) staff       (20)      670 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/examples/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)      617 2023-02-21 21:35:54.000000 bxsolana-trader-1.7.0/bxsolana/examples/constants.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2727 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/examples/order_lifecycle.py
+-rw-r--r--   0 aspin      (501) staff       (20)     7864 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/examples/order_utils.py
+-rw-r--r--   0 aspin      (501) staff       (20)    19151 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/examples/request_utils.py
+-rw-r--r--   0 aspin      (501) staff       (20)     4708 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/examples/stream_utils.py
+-rw-r--r--   0 aspin      (501) staff       (20)     5851 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/examples/transaction_request_utils.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.897724 bxsolana-trader-1.7.0/bxsolana/provider/
+-rw-r--r--   0 aspin      (501) staff       (20)      582 2022-10-10 22:32:15.000000 bxsolana-trader-1.7.0/bxsolana/provider/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)    11768 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/provider/base.py
+-rw-r--r--   0 aspin      (501) staff       (20)      970 2023-02-20 23:04:33.000000 bxsolana-trader-1.7.0/bxsolana/provider/constants.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2662 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/provider/grpc.py
+-rw-r--r--   0 aspin      (501) staff       (20)    30225 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/provider/http.py
+-rw-r--r--   0 aspin      (501) staff       (20)      947 2023-03-06 23:02:29.000000 bxsolana-trader-1.7.0/bxsolana/provider/http_error.py
+-rw-r--r--   0 aspin      (501) staff       (20)     4201 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.0/bxsolana/provider/ws.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.898398 bxsolana-trader-1.7.0/bxsolana/transaction/
+-rw-r--r--   0 aspin      (501) staff       (20)      593 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/bxsolana/transaction/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2361 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.0/bxsolana/transaction/memo.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2402 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.0/bxsolana/transaction/signing.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.899870 bxsolana-trader-1.7.0/bxsolana_trader.egg-info/
+-rw-r--r--   0 aspin      (501) staff       (20)     4348 2023-05-15 16:28:15.000000 bxsolana-trader-1.7.0/bxsolana_trader.egg-info/PKG-INFO
+-rw-r--r--   0 aspin      (501) staff       (20)     1138 2023-05-15 16:28:15.000000 bxsolana-trader-1.7.0/bxsolana_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 aspin      (501) staff       (20)        1 2023-05-15 16:28:15.000000 bxsolana-trader-1.7.0/bxsolana_trader.egg-info/dependency_links.txt
+-rw-r--r--   0 aspin      (501) staff       (20)      188 2023-05-15 16:28:15.000000 bxsolana-trader-1.7.0/bxsolana_trader.egg-info/requires.txt
+-rw-r--r--   0 aspin      (501) staff       (20)       14 2023-05-15 16:28:15.000000 bxsolana-trader-1.7.0/bxsolana_trader.egg-info/top_level.txt
+-rw-r--r--   0 aspin      (501) staff       (20)      217 2022-09-07 21:30:01.000000 bxsolana-trader-1.7.0/pyproject.toml
+-rw-r--r--   0 aspin      (501) staff       (20)      722 2023-05-15 16:28:15.904323 bxsolana-trader-1.7.0/setup.cfg
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.900088 bxsolana-trader-1.7.0/test/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/test/__init__.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.903102 bxsolana-trader-1.7.0/test/integration/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/test/integration/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)     4020 2023-02-20 23:04:33.000000 bxsolana-trader-1.7.0/test/integration/private.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2192 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/test/integration/public.py
+-rw-r--r--   0 aspin      (501) staff       (20)      852 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/test/integration/stream.py
+-rw-r--r--   0 aspin      (501) staff       (20)      701 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/test/integration/test_grpc.py
+-rw-r--r--   0 aspin      (501) staff       (20)      544 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/test/integration/test_http.py
+-rw-r--r--   0 aspin      (501) staff       (20)      664 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/test/integration/test_ws.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.903325 bxsolana-trader-1.7.0/test/unit/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/test/unit/__init__.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 16:28:15.903716 bxsolana-trader-1.7.0/test/unit/transaction/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.0/test/unit/transaction/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)     1386 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.0/test/unit/transaction/test_memo.py
+-rw-r--r--   0 aspin      (501) staff       (20)     4629 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.0/test/unit/transaction/test_signing.py
```

### Comparing `bxsolana-trader-1.6.0/LICENSE` & `bxsolana-trader-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/PKG-INFO` & `bxsolana-trader-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -91,15 +91,15 @@
     
     you can also push the package to pypi 
     $ rm -rf python/dist/
     $ python3 -m build
     $ python3 -m twine upload --repository pypi dist/*
     
     and install the package locally now
-    $ python -m pip install ~/solana-trader-proto/python
+    $ pip install dist/bxsolana-trader-proto-0.0.18.tar.gz
     
     now you can update the depdendency in solana-trader-client-python
     update the version of bxsolana-trader-proto in setup.cfg
     and run 
     $ pip install -r requirements.txt
```

### Comparing `bxsolana-trader-1.6.0/README.md` & `bxsolana-trader-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     
     you can also push the package to pypi 
     $ rm -rf python/dist/
     $ python3 -m build
     $ python3 -m twine upload --repository pypi dist/*
     
     and install the package locally now
-    $ python -m pip install ~/solana-trader-proto/python
+    $ pip install dist/bxsolana-trader-proto-0.0.18.tar.gz
     
     now you can update the depdendency in solana-trader-client-python
     update the version of bxsolana-trader-proto in setup.cfg
     and run 
     $ pip install -r requirements.txt
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/examples/__init__.py` & `bxsolana-trader-1.7.0/bxsolana/examples/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
     OPEN_ORDERS,
     ORDER_ID,
     MARKET,
 )
 from .order_utils import (
     cancel_order,
     cancel_all_orders,
-    replace_order_by_client_order_i_d,
+    replace_order_by_client_order_id,
 )
 from .order_lifecycle import order_lifecycle
 
 __all__ = [
     "do_requests",
     "do_transaction_requests",
     "do_stream",
     "cancel_all_orders",
     "cancel_order",
-    "replace_order_by_client_order_i_d",
+    "replace_order_by_client_order_id",
     "order_lifecycle",
     "PUBLIC_KEY",
     "USDC_WALLET",
     "OPEN_ORDERS",
     "ORDER_ID",
     "MARKET",
 ]
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/examples/constants.py` & `bxsolana-trader-1.7.0/bxsolana/examples/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/bxsolana/examples/order_lifecycle.py` & `bxsolana-trader-1.7.0/bxsolana/examples/order_lifecycle.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,17 @@
     open_orders_addr,
     base_token_wallet,
     quote_token_wallet,
 ):
     print("order lifecycle test\n")
 
     oss = p2.get_order_status_stream(
-        market=market_addr, owner_address=owner_addr
+        get_order_status_stream_request=proto.GetOrderStatusStreamRequest(
+            market=market_addr, owner_address=owner_addr
+        )
     )
 
     # pyre-ignore[6]:
     task = asyncio.create_task(oss.__anext__())
     await asyncio.sleep(10)
 
     # Place Order => `Open`
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/examples/order_utils.py` & `bxsolana-trader-1.7.0/bxsolana/examples/order_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import time
 
 from bxsolana_trader_proto import api as proto
 
 from bxsolana import provider
 from bxsolana.transaction import signing
 
-
 crank_timeout = 60
 
 
 async def place_order(
     p: provider.Provider,
     owner_addr,
     payer_addr,
@@ -21,31 +20,35 @@
     order_price,
     open_orders_addr,
 ) -> int:
     print("starting place order")
 
     client_order_id = random.randint(0, 1000000)
     post_order_response = await p.post_order(
-        owner_address=owner_addr,
-        payer_address=payer_addr,
-        market=market_addr,
-        side=order_side,
-        type=[order_type],
-        amount=order_amount,
-        price=order_price,
-        open_orders_address=open_orders_addr,
-        client_order_i_d=client_order_id,
+        post_order_request=proto.PostOrderRequest(
+            owner_address=owner_addr,
+            payer_address=payer_addr,
+            market=market_addr,
+            side=order_side,
+            type=[order_type],
+            amount=order_amount,
+            price=order_price,
+            open_orders_address=open_orders_addr,
+            client_order_id=client_order_id,
+        )
     )
     print("place order transaction created successfully")
 
     signed_tx = signing.sign_tx(post_order_response.transaction.content)
 
     post_submit_response = await p.post_submit(
-        transaction=proto.TransactionMessage(content=signed_tx),
-        skip_pre_flight=True,
+        post_submit_request=proto.PostSubmitRequest(
+            transaction=proto.TransactionMessage(content=signed_tx),
+            skip_pre_flight=True,
+        )
     )
 
     print(
         f"placing order with clientOrderID {client_order_id.__str__()},"
         f" response signature: {post_submit_response.signature}"
     )
 
@@ -57,27 +60,31 @@
     client_order_id: int,
     market_addr: str,
     owner_addr: str,
     open_orders_addr: str,
 ):
     print("starting cancel order")
 
-    cancel_order_response = await p.post_cancel_by_client_order_i_d(
-        client_order_i_d=client_order_id,
-        market_address=market_addr,
-        owner_address=owner_addr,
-        open_orders_address=open_orders_addr,
+    cancel_order_response = await p.post_cancel_by_client_order_id(
+        post_cancel_by_client_order_id_request=proto.PostCancelByClientOrderIdRequest(
+            client_order_id=client_order_id,
+            market_address=market_addr,
+            owner_address=owner_addr,
+            open_orders_address=open_orders_addr,
+        )
     )
     print("cancel order transaction created successfully")
 
     signed_tx = signing.sign_tx(cancel_order_response.transaction.content)
 
     post_submit_response = await p.post_submit(
-        transaction=proto.TransactionMessage(content=signed_tx),
-        skip_pre_flight=True,
+        post_submit_request=proto.PostSubmitRequest(
+            transaction=proto.TransactionMessage(content=signed_tx),
+            skip_pre_flight=True,
+        )
     )
     print(
         f"cancelling order with clientOrderID {client_order_id.__str__()},"
         f" response signature: {post_submit_response.signature}"
     )
 
 
@@ -88,27 +95,31 @@
     base_token_wallet: str,
     quote_token_wallet: str,
     open_orders_addr: str,
 ):
     print("starting settle funds")
 
     post_settle_response = await p.post_settle(
-        owner_address=owner_addr,
-        market=market_addr,
-        base_token_wallet=base_token_wallet,
-        quote_token_wallet=quote_token_wallet,
-        open_orders_address=open_orders_addr,
+        post_settle_request=proto.PostSettleRequest(
+            owner_address=owner_addr,
+            market=market_addr,
+            base_token_wallet=base_token_wallet,
+            quote_token_wallet=quote_token_wallet,
+            open_orders_address=open_orders_addr,
+        )
     )
     print("settle transaction created successfully")
 
     signed_settle_tx = signing.sign_tx(post_settle_response.transaction.content)
 
     post_submit_response = await p.post_submit(
-        transaction=proto.TransactionMessage(content=signed_settle_tx),
-        skip_pre_flight=True,
+        post_submit_request=proto.PostSubmitRequest(
+            transaction=proto.TransactionMessage(content=signed_settle_tx),
+            skip_pre_flight=True,
+        )
     )
 
     print(
         "settling funds, response signature: " + post_submit_response.signature
     )
 
 
@@ -152,34 +163,42 @@
         open_orders_addr,
     )
     print()
 
     print(f"waiting {crank_timeout}s for place orders to be cranked")
     time.sleep(crank_timeout)
 
-    o = await p.get_open_orders(market=market_addr, address=owner_addr)
+    o = await p.get_open_orders(
+        get_open_orders_request=proto.GetOpenOrdersRequest(
+            market=market_addr, address=owner_addr
+        )
+    )
     found1 = False
     found2 = False
 
     for order in o.orders:
-        if order.client_order_i_d == str(client_order_id_1):
+        if order.client_order_id == str(client_order_id_1):
             found1 = True
-        elif order.client_order_i_d == str(client_order_id_2):
+        elif order.client_order_id == str(client_order_id_2):
             found2 = True
 
     if not found1 or not found2:
         raise Exception("one/both orders not found in orderbook")
     print("2 orders placed successfully\n")
 
     await cancel_all(p, owner_addr, open_orders_addr, market_addr)
 
     print(f"\nwaiting {crank_timeout}s for cancel order(s) to be cranked")
     time.sleep(crank_timeout)
 
-    o = await p.get_open_orders(market=market_addr, address=owner_addr)
+    o = await p.get_open_orders(
+        get_open_orders_request=proto.GetOpenOrdersRequest(
+            market=market_addr, address=owner_addr
+        )
+    )
     if len(o.orders) != 0:
         print(f"{len(o.orders)} orders in orderbook not cancelled")
     else:
         print("orders in orderbook cancelled")
     print()
 
 
@@ -189,65 +208,73 @@
     print("starting cancel all")
 
     open_orders_addresses = [""]
     if open_orders_addresses is None:
         open_orders_addresses.append(open_orders_addr)
 
     cancel_all_response = await p.post_cancel_all(
-        market=market_addr,
-        owner_address=owner_addr,
-        open_orders_addresses=open_orders_addresses,
+        post_cancel_all_request=proto.PostCancelAllRequest(
+            market=market_addr,
+            owner_address=owner_addr,
+            open_orders_addresses=open_orders_addresses,
+        )
     )
     print("cancel all transaction created successfully")
 
     signatures = []
     for transaction in cancel_all_response.transactions:
         signed_tx = signing.sign_tx(transaction.content)
         post_submit_response = await p.post_submit(
-            transaction=proto.TransactionMessage(content=signed_tx),
-            skip_pre_flight=True,
+            post_submit_request=proto.PostSubmitRequest(
+                transaction=proto.TransactionMessage(content=signed_tx),
+                skip_pre_flight=True,
+            )
         )
         signatures.append(post_submit_response.signature)
 
     signatures_string = ", ".join(signatures)
     print(f"cancelling all orders, response signature(s): {signatures_string}")
 
 
-async def replace_order_by_client_order_i_d(
+async def replace_order_by_client_order_id(
     p: provider.Provider,
     owner_addr,
     payer_addr,
     market_addr,
     order_side,
     order_type,
     order_amount,
     order_price,
     open_orders_addr,
 ) -> int:
     print("starting replace order by client order ID")
 
     client_order_id = random.randint(0, 1000000)
-    post_order_response = await p.post_replace_by_client_order_i_d(
-        owner_address=owner_addr,
-        payer_address=payer_addr,
-        market=market_addr,
-        side=order_side,
-        type=[order_type],
-        amount=order_amount,
-        price=order_price,
-        open_orders_address=open_orders_addr,
-        client_order_i_d=client_order_id,
+    post_order_response = await p.post_replace_by_client_order_id(
+        post_order_request=proto.PostOrderRequest(
+            owner_address=owner_addr,
+            payer_address=payer_addr,
+            market=market_addr,
+            side=order_side,
+            type=[order_type],
+            amount=order_amount,
+            price=order_price,
+            open_orders_address=open_orders_addr,
+            client_order_id=client_order_id,
+        )
     )
     print("replace order transaction created successfully")
 
     signed_tx = signing.sign_tx(post_order_response.transaction.content)
 
     post_submit_response = await p.post_submit(
-        transaction=proto.TransactionMessage(content=signed_tx),
-        skip_pre_flight=True,
+        post_submit_request=proto.PostSubmitRequest(
+            transaction=proto.TransactionMessage(content=signed_tx),
+            skip_pre_flight=True,
+        )
     )
     print(
         f"replacing order with clientOrderID {client_order_id.__str__()},"
         f" response signature: {post_submit_response.signature}"
     )
 
     return client_order_id
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/examples/request_utils.py` & `bxsolana-trader-1.7.0/bxsolana/examples/request_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from bxsolana_trader_proto import api as proto
 from bxsolana_trader_proto.common import OrderType
 from bxsolana_trader_proto.common import PerpPositionSide
 from bxsolana_trader_proto.common import PerpOrderType
 from bxsolana_trader_proto.common import PerpContract
 from bxsolana_trader_proto.common import PerpCollateralType
 from bxsolana_trader_proto.common import PerpCollateralToken
+from bxsolana_trader_proto.common import PostOnlyParams
 
 from .. import provider
 
 
 async def do_requests(
     api: provider.Provider,
     public_key: str,
@@ -17,216 +18,281 @@
     usdc_wallet: str,
     sol_usdc_market: str,
 ):
     print("fetching market depth")
     print(
         (
             await api.get_market_depth(
-                limit=1, market="SOLUSDC", project=proto.Project.P_OPENBOOK
+                get_market_depth_request=proto.GetMarketDepthRequest(
+                    limit=1, market="SOLUSDC", project=proto.Project.P_OPENBOOK
+                )
             )
         ).to_json()
     )
 
     # markets API
     print("fetching all markets")
-    print((await api.get_markets()).to_json())
+    print(
+        (
+            await api.get_markets(get_markets_request=proto.GetMarketsRequest())
+        ).to_json()
+    )
 
     print("fetching SOL/USDC orderbook")
     print(
         (
             await api.get_orderbook(
-                market="SOLUSDC", project=proto.Project.P_OPENBOOK
+                get_orderbook_request=proto.GetOrderbookRequest(
+                    market="SOLUSDC", project=proto.Project.P_OPENBOOK
+                )
             )
         ).to_json()
     )
 
     print("fetching SOL/USDC ticker")
     print(
         (
             await api.get_tickers(
-                market="SOLUSDC", project=proto.Project.P_OPENBOOK
+                get_tickers_request=proto.GetTickersRequest(
+                    market="SOLUSDC", project=proto.Project.P_OPENBOOK
+                )
             )
         ).to_json()
     )
 
     print("fetching all tickers")
-    print((await api.get_tickers(project=proto.Project.P_OPENBOOK)).to_json())
+    print(
+        (
+            await api.get_tickers(
+                get_tickers_request=proto.GetTickersRequest(
+                    project=proto.Project.P_OPENBOOK
+                )
+            )
+        ).to_json()
+    )
 
     print("fetching prices")
 
     print(
         (
             await api.get_price(
-                tokens=[
-                    "So11111111111111111111111111111111111111112",
-                    "USDC",
-                    "SOL",
-                    "USDT",
-                ]
+                get_price_request=proto.GetPriceRequest(
+                    tokens=[
+                        "So11111111111111111111111111111111111111112",
+                        "USDC",
+                        "SOL",
+                        "USDT",
+                    ]
+                )
             )
         ).to_json()
     )
 
     print("fetching pools")
-    print((await api.get_pools(projects=[proto.Project.P_RAYDIUM])).to_json())
+    print(
+        (
+            await api.get_pools(
+                get_pools_request=proto.GetPoolsRequest(
+                    projects=[proto.Project.P_RAYDIUM]
+                )
+            )
+        ).to_json()
+    )
 
     print("fetching quotes")
     print(
         (
             await api.get_quotes(
-                in_token="USDC",
-                out_token="SOL",
-                in_amount=0.01,
-                slippage=10,
-                limit=1,
-                projects=[proto.Project.P_RAYDIUM],
+                get_quotes_request=proto.GetQuotesRequest(
+                    in_token="USDC",
+                    out_token="SOL",
+                    in_amount=0.01,
+                    slippage=10,
+                    limit=1,
+                    projects=[proto.Project.P_RAYDIUM],
+                )
             )
         ).to_json()
     )
 
     # trade API
     print("fetching open orders for account")
     print(
         (
             await api.get_open_orders(
-                market="SOLUSDC",
-                address=public_key,
-                project=proto.Project.P_OPENBOOK,
+                get_open_orders_request=proto.GetOpenOrdersRequest(
+                    market="SOLUSDC",
+                    address=public_key,
+                    project=proto.Project.P_OPENBOOK,
+                    limit=0,
+                )
             )
         ).to_json()
     )
 
     print("fetching unsettled amounts")
     print(
         (
             await api.get_unsettled(
-                market="SOLUSDC",
-                owner_address=public_key,
-                project=proto.Project.P_OPENBOOK,
+                get_unsettled_request=proto.GetUnsettledRequest(
+                    market="SOLUSDC",
+                    owner_address=public_key,
+                    project=proto.Project.P_OPENBOOK,
+                )
             )
         ).to_json()
     )
 
     print("fetching account balance amounts")
-    print((await api.get_account_balance(owner_address=public_key)).to_json())
+    print(
+        (
+            await api.get_account_balance(
+                get_account_balance_request=proto.GetAccountBalanceRequest(
+                    owner_address=public_key
+                )
+            )
+        ).to_json()
+    )
 
     print("fetching token accounts and balances")
-    print((await api.get_token_accounts(owner_address=public_key)).to_json())
+    print(
+        (
+            await api.get_token_accounts(
+                get_token_accounts_request=proto.GetTokenAccountsRequest(
+                    owner_address=public_key
+                )
+            )
+        ).to_json()
+    )
 
     print(
         "generating unsigned order (no sign or submission) to sell 0.1 SOL for"
         " USDC at 150_000 USD/SOL"
     )
     print(
         (
             await api.post_order(
-                owner_address=public_key,
-                payer_address=public_key,
-                market="SOLUSDC",
-                side=proto.Side.S_ASK,
-                type=[OrderType.OT_LIMIT],
-                amount=0.1,
-                price=150_000,
-                project=proto.Project.P_OPENBOOK,
-                # optional, but much faster if known
-                open_orders_address=open_orders,
-                # optional, for identification
-                client_order_i_d=0,
+                post_order_request=proto.PostOrderRequest(
+                    owner_address=public_key,
+                    payer_address=public_key,
+                    market="SOLUSDC",
+                    side=proto.Side.S_ASK,
+                    type=[OrderType.OT_LIMIT],
+                    amount=0.1,
+                    price=150_000,
+                    project=proto.Project.P_OPENBOOK,
+                    # optional, but much faster if known
+                    open_orders_address=open_orders,
+                    # optional, for identification
+                    client_order_id=0,
+                )
             )
         ).to_json()
     )
     if order_id != "":
         print("generate cancel order")
         print(
             (
                 await api.post_cancel_order(
-                    order_i_d=order_id,
-                    side=proto.Side.S_ASK,
-                    market_address="SOLUSDC",
-                    project=proto.Project.P_OPENBOOK,
-                    owner_address=public_key,
-                    open_orders_address=open_orders,
+                    post_cancel_order_request=proto.PostCancelOrderRequest(
+                        order_id=order_id,
+                        side=proto.Side.S_ASK,
+                        market_address="SOLUSDC",
+                        project=proto.Project.P_OPENBOOK,
+                        owner_address=public_key,
+                        open_orders_address=open_orders,
+                    )
                 )
             ).to_json()
         )
 
     print("generate cancel order by client ID")
     print(
-        await api.post_cancel_by_client_order_i_d(
-            client_order_i_d=123,
-            market_address=sol_usdc_market,
-            owner_address=public_key,
-            project=proto.Project.P_OPENBOOK,
-            open_orders_address=open_orders,
+        await api.post_cancel_by_client_order_id(
+            post_cancel_by_client_order_id_request=proto.PostCancelByClientOrderIdRequest(
+                client_order_id=123,
+                market_address=sol_usdc_market,
+                owner_address=public_key,
+                project=proto.Project.P_OPENBOOK,
+                open_orders_address=open_orders,
+            )
         )
     )
 
     print("generate settle order")
     print(
         await api.post_settle(
-            owner_address=public_key,
-            market="SOLUSDC",
-            base_token_wallet=public_key,
-            quote_token_wallet=usdc_wallet,
-            project=proto.Project.P_OPENBOOK,
-            open_orders_address=open_orders,
-        )
-    )
-
-    print("generate replace by client order id")
-    print(
-        (
-            await api.post_replace_by_client_order_i_d(
+            post_settle_request=proto.PostSettleRequest(
                 owner_address=public_key,
-                payer_address=public_key,
                 market="SOLUSDC",
-                side=proto.Side.S_ASK,
-                type=[OrderType.OT_LIMIT],
-                amount=0.1,
-                price=150_000,
+                base_token_wallet=public_key,
+                quote_token_wallet=usdc_wallet,
                 project=proto.Project.P_OPENBOOK,
-                # optional, but much faster if known
                 open_orders_address=open_orders,
-                # optional, for identification
-                client_order_i_d=123,
             )
-        ).to_json()
+        )
     )
-    if order_id != "":
-        print("generate replace by order id")
-        print(
-            (
-                await api.post_replace_order(
+
+    print("generate replace by client order id")
+    print(
+        (
+            await api.post_replace_by_client_order_id(
+                post_order_request=proto.PostOrderRequest(
                     owner_address=public_key,
                     payer_address=public_key,
                     market="SOLUSDC",
                     side=proto.Side.S_ASK,
                     type=[OrderType.OT_LIMIT],
                     amount=0.1,
                     price=150_000,
                     project=proto.Project.P_OPENBOOK,
                     # optional, but much faster if known
                     open_orders_address=open_orders,
                     # optional, for identification
-                    client_order_i_d=0,
-                    order_i_d=order_id,
+                    client_order_id=123,
+                )
+            )
+        ).to_json()
+    )
+    if order_id != "":
+        print("generate replace by order id")
+        print(
+            (
+                await api.post_replace_order(
+                    post_replace_order_request=proto.PostReplaceOrderRequest(
+                        owner_address=public_key,
+                        payer_address=public_key,
+                        market="SOLUSDC",
+                        side=proto.Side.S_ASK,
+                        type=[OrderType.OT_LIMIT],
+                        amount=0.1,
+                        price=150_000,
+                        project=proto.Project.P_OPENBOOK,
+                        # optional, but much faster if known
+                        open_orders_address=open_orders,
+                        # optional, for identification
+                        client_order_id=0,
+                        order_id=order_id,
+                    )
                 )
             ).to_json()
         )
 
     print("generate trade swap")
     print(
         (
             await api.post_trade_swap(
-                project=proto.Project.P_RAYDIUM,
-                owner_address=public_key,
-                in_token="SOL",
-                in_amount=0.01,
-                out_token="USDC",
-                slippage=0.01,
+                trade_swap_request=proto.TradeSwapRequest(
+                    project=proto.Project.P_RAYDIUM,
+                    owner_address=public_key,
+                    in_token="SOL",
+                    in_amount=0.01,
+                    out_token="USDC",
+                    slippage=0.01,
+                )
             )
         )
     )
 
     print("generate route swap")
     step = proto.RouteStep(
         in_token="USDC",
@@ -235,234 +301,332 @@
         out_amount=0.01,
         out_amount_min=0.01,
         project=proto.StepProject(label="Raydium"),
     )
     print(
         (
             await api.post_route_trade_swap(
-                project=proto.Project.P_RAYDIUM,
-                owner_address=public_key,
-                steps=[step],
+                route_trade_swap_request=proto.RouteTradeSwapRequest(
+                    project=proto.Project.P_RAYDIUM,
+                    owner_address=public_key,
+                    steps=[step],
+                )
             )
         ).to_json()
     )
 
     # DRIFT
+    print("post Drift margin trading flag")
+    print(
+        (
+            await api.post_drift_enable_margin_trading(
+                post_drift_enable_margin_trading_request=proto.PostDriftEnableMarginTradingRequest(
+                    owner_address=public_key, enable_margin=True
+                )
+            )
+        ).to_json()
+    )
+
+    print("post Drift Margin order")
+    print(
+        (
+            await api.post_drift_margin_order(
+                post_drift_margin_order_request=proto.PostDriftMarginOrderRequest(
+                    owner_address=public_key,
+                    market="SOL",
+                    position_side="LONG",
+                    slippage=10,
+                    type="MARKET",  # or Limit
+                    amount=10,
+                    client_order_id=12,
+                    post_only=PostOnlyParams.PO_NONE,
+                )
+            )
+        ).to_json()
+    )
+
+    print("get Drift markets")
+    print(
+        (
+            await api.get_drift_markets(
+                get_drift_markets_request=proto.GetDriftMarketsRequest(
+                    metadata=True
+                )
+            )
+        ).to_json()
+    )
+
+    print("get Drift margin orderbook")
+    print(
+        (
+            await api.get_drift_margin_orderbook(
+                get_drift_margin_orderbook_request=proto.GetDriftMarginOrderbookRequest(
+                    market="SOL", limit=2, metadata=True
+                )
+            )
+        ).to_json()
+    )
+
     print("get user")
     print(
         (
             await api.get_user(
-                project=proto.Project.P_DRIFT,
-                owner_address=public_key,
+                get_user_request=proto.GetUserRequest(
+                    project=proto.Project.P_DRIFT, owner_address=public_key
+                )
             )
         ).to_json()
     )
 
     print("get Drift orderbook")
     print(
         (
             await api.get_perp_orderbook(
-                contract=PerpContract.SOL_PERP, project=proto.Project.P_DRIFT
+                get_perp_orderbook_request=proto.GetPerpOrderbookRequest(
+                    contract=PerpContract.SOL_PERP,
+                    project=proto.Project.P_DRIFT,
+                )
             )
         ).to_json()
     )
 
     print("post perp order")
     print(
         (
             await api.post_perp_order(
-                project=proto.Project.P_DRIFT,
-                owner_address=public_key,
-                payer_address=public_key,
-                contract=PerpContract.SOL_PERP,
-                position_side=PerpPositionSide.PS_LONG,
-                slippage=0,
-                type=PerpOrderType.POT_LIMIT,
-                amount=0,
-                price=12000,
-                client_order_i_d=12,
+                post_perp_order_request=proto.PostPerpOrderRequest(
+                    project=proto.Project.P_DRIFT,
+                    owner_address=public_key,
+                    payer_address=public_key,
+                    contract=PerpContract.SOL_PERP,
+                    position_side=PerpPositionSide.PS_LONG,
+                    slippage=0,
+                    type=PerpOrderType.POT_LIMIT,
+                    amount=0,
+                    price=12000,
+                    client_order_id=12,
+                )
             )
         ).to_json()
     )
 
     print("get perp contracts")
     print(
         (
             await api.get_perp_contracts(
-                project=proto.Project.P_DRIFT,
+                get_perp_contracts_request=proto.GetPerpContractsRequest(
+                    project=proto.Project.P_DRIFT,
+                )
             )
         ).to_json()
     )
 
     print("get perp assets")
     print(
         (
             await api.get_assets(
-                owner_address=public_key,
-                project=proto.Project.P_DRIFT,
+                get_assets_request=proto.GetAssetsRequest(
+                    owner_address=public_key,
+                    project=proto.Project.P_DRIFT,
+                )
             )
         ).to_json()
     )
 
     print("get open perp order")
     print(
         (
             await api.get_open_perp_order(
-                owner_address=public_key,
-                project=proto.Project.P_DRIFT,
-                contract=PerpContract.SOL_PERP,
-                client_order_i_d=12,
+                get_open_perp_order_request=proto.GetOpenPerpOrderRequest(
+                    owner_address=public_key,
+                    project=proto.Project.P_DRIFT,
+                    contract=PerpContract.SOL_PERP,
+                    client_order_id=12,
+                )
             )
         ).to_json()
     )
 
     print("get open perp orders")
     print(
         (
             await api.get_open_perp_orders(
-                owner_address=public_key,
-                project=proto.Project.P_DRIFT,
-                contracts=[PerpContract.SOL_PERP, PerpContract.BTC_PERP],
+                get_open_perp_orders_request=proto.GetOpenPerpOrdersRequest(
+                    owner_address=public_key,
+                    project=proto.Project.P_DRIFT,
+                    contracts=[PerpContract.SOL_PERP, PerpContract.BTC_PERP],
+                )
             )
         ).to_json()
     )
 
     print("post liquidate perp")
     print(
         (
             await api.post_liquidate_perp(
-                project=proto.Project.P_DRIFT,
-                owner_address=public_key,
-                settlee_account_address=(
-                    "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
-                ),
-                contract=PerpContract.SOL_PERP,
-                amount=1,
+                post_liquidate_perp_request=proto.PostLiquidatePerpRequest(
+                    project=proto.Project.P_DRIFT,
+                    owner_address=public_key,
+                    settlee_account_address=(
+                        "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
+                    ),
+                    contract=PerpContract.SOL_PERP,
+                    amount=1,
+                )
             )
         ).to_json()
     )
 
     print("post settle pnl")
     print(
         (
-            await api.post_settle_p_n_l(
-                project=proto.Project.P_DRIFT,
-                owner_address=public_key,
-                settlee_account_address=(
-                    "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
-                ),
-                contract=PerpContract.SOL_PERP,
+            await api.post_settle_pnl(
+                post_settle_pnl_request=proto.PostSettlePnlRequest(
+                    project=proto.Project.P_DRIFT,
+                    owner_address=public_key,
+                    settlee_account_address=(
+                        "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
+                    ),
+                    contract=PerpContract.SOL_PERP,
+                )
             )
         ).to_json()
     )
 
     print("post settle pnls")
     print(
         (
-            await api.post_settle_p_n_ls(
-                project=proto.Project.P_DRIFT,
-                owner_address=public_key,
-                settlee_account_addresses=[
-                    "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
-                ],
-                contract=PerpContract.SOL_PERP,
+            await api.post_settle_pn_ls(
+                post_settle_pn_ls_request=proto.PostSettlePnLsRequest(
+                    project=proto.Project.P_DRIFT,
+                    owner_address=public_key,
+                    settlee_account_addresses=[
+                        "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
+                    ],
+                    contract=PerpContract.SOL_PERP,
+                )
             )
         ).to_json()
     )
 
     print("post cancel perp order")
     print(
         (
             await api.post_cancel_perp_order(
-                project=proto.Project.P_DRIFT,
-                owner_address=public_key,
-                client_order_i_d=12,
-                order_i_d=0,
-                contract=PerpContract.SOL_PERP,
+                post_cancel_perp_order_request=proto.PostCancelPerpOrderRequest(
+                    project=proto.Project.P_DRIFT,
+                    owner_address=public_key,
+                    client_order_id=12,
+                    order_id=0,
+                    contract=PerpContract.SOL_PERP,
+                )
             )
         ).to_json()
     )
 
     print("post close perp orders")
     print(
         (
             await api.post_close_perp_positions(
-                project=proto.Project.P_DRIFT,
-                owner_address=public_key,
-                contracts=[PerpContract.SOL_PERP],
+                post_close_perp_positions_request=proto.PostClosePerpPositionsRequest(
+                    project=proto.Project.P_DRIFT,
+                    owner_address=public_key,
+                    contracts=[PerpContract.SOL_PERP],
+                )
             )
         ).to_json()
     )
 
     print("post cancel perp orders")
     print(
         (
             await api.post_cancel_perp_orders(
-                project=proto.Project.P_DRIFT,
-                contract=PerpContract.SOL_PERP,
-                owner_address=public_key,
+                post_cancel_perp_orders_request=proto.PostCancelPerpOrdersRequest(
+                    project=proto.Project.P_DRIFT,
+                    contract=PerpContract.SOL_PERP,
+                    owner_address=public_key,
+                )
             )
         ).to_json()
     )
 
     print("post create user")
     print(
         (
             await api.post_create_user(
-                project=proto.Project.P_DRIFT,
-                owner_address="BgJ8uyf9yhLJaUVESRrqffzwVyQgRi9YvWmpEFaH14kx",
+                post_create_user_request=proto.PostCreateUserRequest(
+                    project=proto.Project.P_DRIFT,
+                    action="CREATE",
+                    owner_address=(
+                        "BgJ8uyf9yhLJaUVESRrqffzwVyQgRi9YvWmpEFaH14kx"
+                    ),
+                )
             )
         ).to_json()
     )
 
     print("post deposit collateral")
     print(
         (
             await api.post_manage_collateral(
-                project=proto.Project.P_DRIFT,
-                account_address="9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS",
-                amount=0.1,
-                token=PerpCollateralToken.PCTK_USDC,
-                type=PerpCollateralType.PCT_DEPOSIT,
+                post_manage_collateral_request=proto.PostManageCollateralRequest(
+                    project=proto.Project.P_DRIFT,
+                    account_address=(
+                        "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
+                    ),
+                    amount=0.1,
+                    token=PerpCollateralToken.PCTK_USDC,
+                    type=PerpCollateralType.PCT_DEPOSIT,
+                )
             )
         ).to_json()
     )
 
     print("post withdraw collateral")
     print(
         (
             await api.post_manage_collateral(
-                project=proto.Project.P_DRIFT,
-                account_address="9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS",
-                amount=0.1,
-                token=PerpCollateralToken.PCTK_SOL,
-                type=PerpCollateralType.PCT_WITHDRAWAL,
+                post_manage_collateral_request=proto.PostManageCollateralRequest(
+                    project=proto.Project.P_DRIFT,
+                    account_address=(
+                        "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
+                    ),
+                    amount=0.1,
+                    token=PerpCollateralToken.PCTK_SOL,
+                    type=PerpCollateralType.PCT_WITHDRAWAL,
+                )
             )
         ).to_json()
     )
 
     print("post transfer collateral")
     print(
         (
             await api.post_manage_collateral(
-                project=proto.Project.P_DRIFT,
-                account_address="9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS",
-                amount=0.1,
-                token=PerpCollateralToken.PCTK_SOL,
-                type=PerpCollateralType.PCT_TRANSFER,
-                to_account_address=(
-                    "AbnwAQGrYnvktT4ihhX5np8RbgtfXJfPwpgMJnCFa4MT"
-                ),
+                post_manage_collateral_request=proto.PostManageCollateralRequest(
+                    project=proto.Project.P_DRIFT,
+                    account_address=(
+                        "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
+                    ),
+                    amount=0.1,
+                    token=PerpCollateralToken.PCTK_SOL,
+                    type=PerpCollateralType.PCT_TRANSFER,
+                    to_account_address=(
+                        "AbnwAQGrYnvktT4ihhX5np8RbgtfXJfPwpgMJnCFa4MT"
+                    ),
+                )
             )
         ).to_json()
     )
 
     print("get perp positions")
     print(
         (
             await api.get_perp_positions(
-                project=proto.Project.P_DRIFT,
-                owner_address=public_key,
-                contracts=[PerpContract.SOL_PERP],
+                get_perp_positions_request=proto.GetPerpPositionsRequest(
+                    project=proto.Project.P_DRIFT,
+                    owner_address=public_key,
+                    contracts=[PerpContract.SOL_PERP],
+                )
             )
         ).to_json()
     )
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/examples/stream_utils.py` & `bxsolana-trader-1.7.0/bxsolana/examples/stream_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,105 +6,134 @@
 
 async def do_stream(api: provider.Provider, run_slow: bool = False):
     item_count = 0
 
     if run_slow:
         print("streaming orderbook updates...")
         async for response in api.get_orderbooks_stream(
-            markets=["SOLUSDC"], project=proto.Project.P_OPENBOOK
+            get_orderbooks_request=proto.GetOrderbooksRequest(
+                markets=["SOLUSDC"], project=proto.Project.P_OPENBOOK
+            )
         ):
             print(response.to_json())
             item_count += 1
-            if item_count == 5:
+            if item_count == 1:
                 item_count = 0
                 break
 
     if run_slow:
         print("streaming ticker updates...")
         async for response in api.get_tickers_stream(
-            market="SOLUSDC", project=proto.Project.P_OPENBOOK
+            get_tickers_request=proto.GetTickersRequest(
+                market="SOLUSDC", project=proto.Project.P_OPENBOOK
+            )
         ):
             print(response.to_json())
             item_count += 1
-            if item_count == 5:
+            if item_count == 1:
                 item_count = 0
                 break
 
     if run_slow:
         print("streaming trade updates...")
         async for response in api.get_trades_stream(
-            market="SOLUSDC", project=proto.Project.P_OPENBOOK
+            get_trades_request=proto.GetTradesRequest(
+                market="SOLUSDC", project=proto.Project.P_OPENBOOK
+            )
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 1:
                 item_count = 0
                 break
 
     if run_slow:
         print("streaming swap events...")
         async for response in api.get_swaps_stream(
-            projects=[proto.Project.P_RAYDIUM],
-            # RAY-SOL , ETH-SOL, SOL-USDC, SOL-USDT
-            pools=[
-                "AVs9TA4nWDzfPJE9gGVNJMVhcQy3V9PGazuz33BfG2RA",
-                "9Hm8QX7ZhE9uB8L2arChmmagZZBtBmnzBbpfxzkQp85D",
-                "58oQChx4yWmvKdwLLZzBi4ChoCc2fqCUWBkwMihLYQo2",
-                "7XawhbbxtsRcQA8KTkHT9f9nc6d69UwqCDh6U5EEbEmX",
-            ],
-            include_failed=True,
+            get_swaps_stream_request=proto.GetSwapsStreamRequest(
+                projects=[proto.Project.P_RAYDIUM],
+                # RAY-SOL , ETH-SOL, SOL-USDC, SOL-USDT
+                pools=[
+                    "AVs9TA4nWDzfPJE9gGVNJMVhcQy3V9PGazuz33BfG2RA",
+                    "9Hm8QX7ZhE9uB8L2arChmmagZZBtBmnzBbpfxzkQp85D",
+                    "58oQChx4yWmvKdwLLZzBi4ChoCc2fqCUWBkwMihLYQo2",
+                    "7XawhbbxtsRcQA8KTkHT9f9nc6d69UwqCDh6U5EEbEmX",
+                ],
+                include_failed=True,
+            )
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 1:
                 item_count = 0
                 break
 
     if run_slow:
         print("streaming pool reserves...")
         async for response in api.get_pool_reserves_stream(
-            projects=[proto.Project.P_RAYDIUM]
+            get_pool_reserves_stream_request=proto.GetPoolReservesStreamRequest(
+                projects=[proto.Project.P_RAYDIUM]
+            )
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 1:
                 item_count = 0
                 break
 
     if run_slow:
         print("streaming price streams...")
         async for response in api.get_prices_stream(
-            projects=[proto.Project.P_RAYDIUM],
-            tokens=[
-                "So11111111111111111111111111111111111111112",
-                "USDC",
-                "SOL",
-                "USDT",
-            ],
+            get_prices_stream_request=proto.GetPricesStreamRequest(
+                projects=[proto.Project.P_RAYDIUM],
+                tokens=[
+                    "So11111111111111111111111111111111111111112",
+                    "USDC",
+                    "SOL",
+                    "USDT",
+                ],
+            )
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 1:
                 item_count = 0
                 break
 
     if run_slow:
         print("streaming Drift orderbook updates...")
         async for response in api.get_perp_orderbooks_stream(
-            contracts=[PerpContract.ALL], project=proto.Project.P_DRIFT
+            get_perp_orderbooks_request=proto.GetPerpOrderbooksRequest(
+                contracts=[PerpContract.ALL], project=proto.Project.P_DRIFT
+            )
         ):
             print(response.to_json())
             item_count += 1
-            if item_count == 5:
+            if item_count == 1:
                 item_count = 0
                 break
 
     if run_slow:
         print("streaming Drift trade updates...")
         async for response in api.get_perp_trades_stream(
-            contracts=[PerpContract.ALL], project=proto.Project.P_DRIFT
+            get_perp_trades_stream_request=proto.GetPerpTradesStreamRequest(
+                contracts=[PerpContract.ALL], project=proto.Project.P_DRIFT
+            )
+        ):
+            print(response.to_json())
+            item_count += 1
+            if item_count == 1:
+                item_count = 0
+                break
+
+    if run_slow:
+        print("streaming Drift margin orderbook updates...")
+        async for response in api.get_drift_margin_orderbooks_stream(
+            get_drift_margin_orderbooks_request=proto.GetDriftMarginOrderbooksRequest(
+                markets=["SOL"], metadata=True, limit=1
+            )
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 1:
                 item_count = 0
                 break
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/examples/transaction_request_utils.py` & `bxsolana-trader-1.7.0/bxsolana/examples/transaction_request_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,27 +56,27 @@
     print(signature)
 
     print(
         "submitting replace order by client ID (generate + sign) to sell 0.1"
         " SOL for USDC at 150_000 USD/SOL"
     )
     print(
-        await api.submit_replace_by_client_order_i_d(
+        await api.submit_replace_by_client_order_id(
             owner_address=owner_addr,
             payer_address=payer_addr,
             market=market,
             side=proto.Side.S_ASK,
             types=[OrderType.OT_LIMIT],
             amount=0.1,
             price=150_000,
             project=proto.Project.P_SERUM,
             # optional, but much faster if known
             open_orders_address=open_orders_addr,
             # optional, for identification
-            client_order_i_d=client_order_id,
+            client_order_id=client_order_id,
             skip_pre_flight=True,
         )
     )
 
     print(
         "submitting replace order (generate + sign) to sell 0.1 SOL for USDC at"
         " 150_000 USD/SOL"
@@ -91,36 +91,36 @@
             amount=0.1,
             price=150_000,
             project=proto.Project.P_SERUM,
             # optional, but much faster if known
             open_orders_address=open_orders_addr,
             # optional, for identification
             client_order_id=0,
-            order_i_d=order_id,
+            order_id=order_id,
         )
     )
 
     # cancel order example: comment out if want to try replace example
     print("submit cancel order")
     print(
         await api.submit_cancel_order(
-            order_i_d=order_id,
+            order_id=order_id,
             side=proto.Side.S_ASK,
             market_address=market,
             owner_address=owner_addr,
             project=proto.Project.P_SERUM,
             open_orders_address=open_orders_addr,
         )
     )
 
     # cancel by client order ID example: comment out if want to try replace example
     print("submit cancel order by client ID")
     print(
-        await api.submit_cancel_by_client_order_i_d(
-            client_order_i_d=client_order_id,
+        await api.submit_cancel_by_client_order_id(
+            client_order_id=client_order_id,
             market_address=market,
             owner_address=owner_addr,
             project=proto.Project.P_SERUM,
             open_orders_address=open_orders_addr,
             skip_pre_flight=True,
         )
     )
@@ -142,32 +142,38 @@
 
 
 async def create_transaction_with_memo(api: provider.Provider):
     private_key = transaction.load_private_key_from_env()
 
     instruction = transaction.create_trader_api_memo_instruction("hi from dev")
 
-    recent_block_hash_resp = await api.get_recent_block_hash()
+    recent_block_hash_resp = await api.get_recent_block_hash(
+        get_recent_block_hash_request=proto.GetRecentBlockHashRequest()
+    )
     recent_block_hash = hs.Hash.from_string(recent_block_hash_resp.block_hash)
     instructions = [instruction]
 
     tx_serialized = transaction.build_fully_signed_txn(
         recent_block_hash, private_key.pubkey(), instructions, private_key
     )
     single_memo_txn = base64.b64encode(tx_serialized).decode("utf-8")
     print("serialized memo single_memo_txn", single_memo_txn)
 
     post_submit_response = await api.post_submit(
-        transaction=proto.TransactionMessage(single_memo_txn),
-        skip_pre_flight=True,
+        post_submit_request=proto.PostSubmitRequest(
+            transaction=proto.TransactionMessage(single_memo_txn),
+            skip_pre_flight=True,
+        )
     )
     print("signature for single memo txn", post_submit_response.signature)
 
     double_memo_txn_signed = transaction.add_memo_to_serialized_txn(
         single_memo_txn, "hi from dev2", private_key.pubkey(), private_key
     )
     print("double_memo_txn_signed", double_memo_txn_signed)
     post_submit_response = await api.post_submit(
-        transaction=proto.TransactionMessage(double_memo_txn_signed),
-        skip_pre_flight=True,
+        post_submit_request=proto.PostSubmitRequest(
+            transaction=proto.TransactionMessage(double_memo_txn_signed),
+            skip_pre_flight=True,
+        )
     )
     print("signature for double memo tx", post_submit_response.signature)
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/provider/__init__.py` & `bxsolana-trader-1.7.0/bxsolana/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/bxsolana/provider/base.py` & `bxsolana-trader-1.7.0/bxsolana/provider/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,82 +46,94 @@
         open_orders_address: str = "",
         client_order_id: int = 0,
         project: api.Project = api.Project.P_UNKNOWN,
         skip_pre_flight: bool = False,
     ) -> str:
         pk = self.require_private_key()
         order = await self.post_order(
-            owner_address=owner_address,
-            payer_address=payer_address,
-            market=market,
-            side=side,
-            type=types,
-            amount=amount,
-            price=price,
-            open_orders_address=open_orders_address,
-            client_order_i_d=client_order_id,
-            project=project,
+            post_order_request=api.PostOrderRequest(
+                owner_address=owner_address,
+                payer_address=payer_address,
+                market=market,
+                side=side,
+                type=types,
+                amount=amount,
+                price=price,
+                open_orders_address=open_orders_address,
+                client_order_id=client_order_id,
+                project=project,
+            )
         )
         signed_tx = transaction.sign_tx_message_with_private_key(
             order.transaction, pk
         )
         result = await self.post_submit(
-            transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            post_submit_request=api.PostSubmitRequest(
+                transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            )
         )
         return result.signature
 
     async def submit_cancel_order(
         self,
-        order_i_d: str = "",
+        order_id: str = "",
         side: api.Side = api.Side.S_UNKNOWN,
         market_address: str = "",
         owner_address: str = "",
         open_orders_address: str = "",
         project: api.Project = api.Project.P_UNKNOWN,
         skip_pre_flight: bool = True,
     ) -> str:
         pk = self.require_private_key()
         order = await self.post_cancel_order(
-            order_i_d=order_i_d,
-            side=side,
-            market_address=market_address,
-            owner_address=owner_address,
-            open_orders_address=open_orders_address,
-            project=project,
+            post_cancel_order_request=api.PostCancelOrderRequest(
+                order_id=order_id,
+                side=side,
+                market_address=market_address,
+                owner_address=owner_address,
+                open_orders_address=open_orders_address,
+                project=project,
+            )
         )
         signed_tx = transaction.sign_tx_message_with_private_key(
             order.transaction, pk
         )
         result = await self.post_submit(
-            transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            post_submit_request=api.PostSubmitRequest(
+                transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            )
         )
         return result.signature
 
-    async def submit_cancel_by_client_order_i_d(
+    async def submit_cancel_by_client_order_id(
         self,
-        client_order_i_d: int = 0,
+        client_order_id: int = 0,
         market_address: str = "",
         owner_address: str = "",
         open_orders_address: str = "",
         project: api.Project = api.Project.P_UNKNOWN,
         skip_pre_flight: bool = True,
     ) -> str:
         pk = self.require_private_key()
-        order = await self.post_cancel_by_client_order_i_d(
-            client_order_i_d=client_order_i_d,
-            market_address=market_address,
-            owner_address=owner_address,
-            open_orders_address=open_orders_address,
-            project=project,
+        order = await self.post_cancel_by_client_order_id(
+            post_cancel_by_client_order_id_request=api.PostCancelByClientOrderIdRequest(
+                client_order_id=client_order_id,
+                market_address=market_address,
+                owner_address=owner_address,
+                open_orders_address=open_orders_address,
+                project=project,
+            )
         )
         signed_tx = transaction.sign_tx_message_with_private_key(
             order.transaction, pk
         )
         result = await self.post_submit(
-            transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            post_submit_request=api.PostSubmitRequest(
+                transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            )
         )
         return result.signature
 
     async def submit_cancel_all(
         self,
         market: str = "",
         owner_address: str = "",
@@ -130,25 +142,29 @@
         skip_pre_flight: bool = True,
     ) -> List[str]:
         if open_orders_addresses is None:
             open_orders_addresses = []
 
         pk = self.require_private_key()
         response = await self.post_cancel_all(
-            market=market,
-            owner_address=owner_address,
-            open_orders_addresses=open_orders_addresses,
-            project=project,
+            post_cancel_all_request=api.PostCancelAllRequest(
+                market=market,
+                owner_address=owner_address,
+                open_orders_addresses=open_orders_addresses,
+                project=project,
+            )
         )
 
         signatures = []
         for tx in response.transactions:
             signed_tx = transaction.sign_tx_message_with_private_key(tx, pk)
             result = await self.post_submit(
-                transaction=signed_tx, skip_pre_flight=skip_pre_flight
+                post_submit_request=api.PostSubmitRequest(
+                    transaction=signed_tx, skip_pre_flight=skip_pre_flight
+                )
             )
             signatures.append(result.signature)
 
         return signatures
 
     async def submit_settle(
         self,
@@ -158,98 +174,110 @@
         quote_token_wallet: str = "",
         open_orders_address: str = "",
         project: api.Project = api.Project.P_UNKNOWN,
         skip_pre_flight: bool = False,
     ) -> str:
         pk = self.require_private_key()
         response = await self.post_settle(
-            owner_address=owner_address,
-            market=market,
-            base_token_wallet=base_token_wallet,
-            quote_token_wallet=quote_token_wallet,
-            open_orders_address=open_orders_address,
-            project=project,
+            post_settle_request=api.PostSettleRequest(
+                owner_address=owner_address,
+                market=market,
+                base_token_wallet=base_token_wallet,
+                quote_token_wallet=quote_token_wallet,
+                open_orders_address=open_orders_address,
+                project=project,
+            )
         )
         signed_tx = transaction.sign_tx_message_with_private_key(
             response.transaction, pk
         )
         result = await self.post_submit(
-            transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            post_submit_request=api.PostSubmitRequest(
+                transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            )
         )
         return result.signature
 
-    async def submit_replace_by_client_order_i_d(
+    async def submit_replace_by_client_order_id(
         self,
         owner_address: str,
         payer_address: str,
         market: str,
         side: "api.Side",
         types: List["OrderType"],
         amount: float,
         price: float,
         open_orders_address: str = "",
-        client_order_i_d: int = 0,
+        client_order_id: int = 0,
         project: api.Project = api.Project.P_UNKNOWN,
         skip_pre_flight: bool = False,
     ) -> str:
         pk = self.require_private_key()
-        order = await self.post_replace_by_client_order_i_d(
-            owner_address=owner_address,
-            payer_address=payer_address,
-            market=market,
-            side=side,
-            type=types,
-            amount=amount,
-            price=price,
-            open_orders_address=open_orders_address,
-            client_order_i_d=client_order_i_d,
-            project=project,
+        order = await self.post_replace_by_client_order_id(
+            post_order_request=api.PostOrderRequest(
+                owner_address=owner_address,
+                payer_address=payer_address,
+                market=market,
+                side=side,
+                type=types,
+                amount=amount,
+                price=price,
+                open_orders_address=open_orders_address,
+                client_order_id=client_order_id,
+                project=project,
+            )
         )
         signed_tx = transaction.sign_tx_message_with_private_key(
             order.transaction, pk
         )
         result = await self.post_submit(
-            transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            post_submit_request=api.PostSubmitRequest(
+                transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            )
         )
         return result.signature
 
     async def submit_replace_order(
         self,
-        order_i_d: str,
+        order_id: str,
         owner_address: str,
         payer_address: str,
         market: str,
         side: "api.Side",
         types: List["OrderType"],
         amount: float,
         price: float,
         open_orders_address: str = "",
         client_order_id: int = 0,
         project: api.Project = api.Project.P_UNKNOWN,
         skip_pre_flight: bool = False,
     ) -> str:
         pk = self.require_private_key()
         order = await self.post_replace_order(
-            owner_address=owner_address,
-            payer_address=payer_address,
-            market=market,
-            side=side,
-            type=types,
-            amount=amount,
-            price=price,
-            open_orders_address=open_orders_address,
-            client_order_i_d=client_order_id,
-            order_i_d=order_i_d,
-            project=project,
+            post_replace_order_request=api.PostReplaceOrderRequest(
+                owner_address=owner_address,
+                payer_address=payer_address,
+                market=market,
+                side=side,
+                type=types,
+                amount=amount,
+                price=price,
+                open_orders_address=open_orders_address,
+                client_order_id=client_order_id,
+                order_id=order_id,
+                project=project,
+            )
         )
         signed_tx = transaction.sign_tx_message_with_private_key(
             order.transaction, pk
         )
         result = await self.post_submit(
-            transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            post_submit_request=api.PostSubmitRequest(
+                transaction=signed_tx, skip_pre_flight=skip_pre_flight
+            )
         )
         return result.signature
 
     async def submit_post_trade_swap(
         self,
         *,
         project: api.Project = api.Project.P_UNKNOWN,
@@ -259,58 +287,66 @@
         in_amount: float = 0,
         slippage: float = 0,
         skip_pre_flight: bool = False,
         submit_strategy: api.SubmitStrategy = api.SubmitStrategy.P_ABORT_ON_FIRST_ERROR,
     ) -> api.PostSubmitBatchResponse:
         pk = self.require_private_key()
         result = await self.post_trade_swap(
-            project=project,
-            owner_address=owner_address,
-            in_token=in_token,
-            out_token=out_token,
-            in_amount=in_amount,
-            slippage=slippage,
+            trade_swap_request=api.TradeSwapRequest(
+                project=project,
+                owner_address=owner_address,
+                in_token=in_token,
+                out_token=out_token,
+                in_amount=in_amount,
+                slippage=slippage,
+            )
         )
 
         signed_txs: List[api.PostSubmitRequestEntry] = []
         for tx in result.transactions:
             signed_tx = transaction.sign_tx_message_with_private_key(tx, pk)
             signed_txs.append(
                 api.PostSubmitRequestEntry(
                     transaction=signed_tx, skip_pre_flight=skip_pre_flight
                 )
             )
 
         return await self.post_submit_batch(
-            entries=signed_txs, submit_strategy=submit_strategy
+            post_submit_batch_request=api.PostSubmitBatchRequest(
+                entries=signed_txs, submit_strategy=submit_strategy
+            )
         )
 
     async def submit_post_route_trade_swap(
         self,
         *,
         project: api.Project = api.Project.P_UNKNOWN,
         owner_address: str = "",
         steps: List["api.RouteStep"] = [],
         skip_pre_flight: bool = False,
         submit_strategy: api.SubmitStrategy = api.SubmitStrategy.P_ABORT_ON_FIRST_ERROR,
     ) -> api.PostSubmitBatchResponse:
         pk = self.require_private_key()
         result = await self.post_route_trade_swap(
-            project=project, owner_address=owner_address, steps=steps
+            route_trade_swap_request=api.RouteTradeSwapRequest(
+                project=project, owner_address=owner_address, steps=steps
+            )
         )
 
         signed_txs: List[api.PostSubmitRequestEntry] = []
         for tx in result.transactions:
             signed_tx = transaction.sign_tx_message_with_private_key(tx, pk)
             signed_txs.append(
                 api.PostSubmitRequestEntry(
                     transaction=signed_tx, skip_pre_flight=skip_pre_flight
                 )
             )
 
         return await self.post_submit_batch(
-            entries=signed_txs, submit_strategy=submit_strategy
+            post_submit_batch_request=api.PostSubmitBatchRequest(
+                entries=signed_txs, submit_strategy=submit_strategy
+            )
         )
 
 
 class NotConnectedException(Exception):
     pass
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/provider/constants.py` & `bxsolana-trader-1.7.0/bxsolana/provider/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/bxsolana/provider/grpc.py` & `bxsolana-trader-1.7.0/bxsolana/provider/grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import os
-from typing import TYPE_CHECKING, Optional
+from typing import Optional
 
 from grpclib import client
 from solders import keypair as kp
 
 from .. import transaction
 from . import constants
 from .base import Provider
 
-if TYPE_CHECKING:
-    # noinspection PyProtectedMember
-    from betterproto import _MetadataLike, Deadline
-
 
 class GrpcProvider(Provider):
     # pyre-ignore[15]: overriding to force context manager hooks
     channel: Optional[client.Channel] = None
 
     _host: str
     _port: int
@@ -28,16 +24,14 @@
         host: str = constants.MAINNET_API_GRPC_HOST,
         port: int = constants.MAINNET_API_GRPC_PORT,
         private_key: Optional[str] = None,
         auth_header: Optional[str] = None,
         use_ssl: bool = False,
         *,
         timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["_MetadataLike"] = None,
     ):
         self._host = host
         self._port = port
         self._use_ssl = use_ssl
 
         if private_key is None:
             try:
@@ -52,16 +46,14 @@
         else:
             self._auth_header = auth_header
 
         super().__init__(
             # pyre-ignore[6]: overriding to force context manager hooks
             None,
             timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
         )
 
     async def connect(self):
         if self.channel is None:
             self.channel = client.Channel(
                 self._host, self._port, ssl=self._use_ssl
             )
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/provider/http_error.py` & `bxsolana-trader-1.7.0/bxsolana/provider/http_error.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/bxsolana/provider/ws.py` & `bxsolana-trader-1.7.0/bxsolana/provider/ws.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 import jsonrpc
 from solders import keypair as kp
 from stringcase import camelcase
 
 from . import Provider, constants
 from .. import transaction
 
+from grpclib.metadata import Deadline
+from grpclib.metadata import _MetadataLike as MetadataLike
+
 if TYPE_CHECKING:
     # noinspection PyUnresolvedReferences,PyProtectedMember
     # pyre-ignore[21]: module is too hard to find
     from grpclib._protocols import IProtoMessage
 
     # noinspection PyProtectedMember
-    from betterproto import _MetadataLike, Deadline, T
+    from betterproto import T
 
 
 class WsProvider(Provider):
     _ws: jsonrpc.WsRpcConnection
 
     _endpoint: str
     _private_key: Optional[kp.Keypair]
@@ -65,31 +68,36 @@
         route: str,
         # pyre-ignore[11]: type is too hard to find
         request: "IProtoMessage",
         response_type: Type["T"],
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["_MetadataLike"] = None,
+        metadata: Optional["MetadataLike"] = None,
     ) -> "T":
-        result = await self._ws.call(
-            _ws_endpoint(route), request.to_dict(include_default_values=False)
-        )
+        request_dict = request.to_dict(include_default_values=False)
+        if "clientOrderId" in request_dict:
+            request_dict["clientOrderID"] = request_dict.pop("clientOrderId")
+
+        if "orderId" in request_dict:
+            request_dict["orderID"] = request_dict.pop("orderId")
+
+        result = await self._ws.call(_ws_endpoint(route), request_dict)
         response = _validated_response(result, response_type)
         return response
 
     async def _unary_stream(
         self,
         route: str,
         request: "IProtoMessage",
         response_type: Type["T"],
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["_MetadataLike"] = None,
+        metadata: Optional["MetadataLike"] = None,
     ) -> AsyncGenerator["T", None]:
         subscription_id = await self._ws.subscribe(
             _ws_endpoint(route), request.to_dict()
         )
         async for update in self._ws.notifications_for_id(subscription_id):
             response = _validated_response(update, response_type)
             yield response
```

### Comparing `bxsolana-trader-1.6.0/bxsolana/transaction/__init__.py` & `bxsolana-trader-1.7.0/bxsolana/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/bxsolana/transaction/memo.py` & `bxsolana-trader-1.7.0/bxsolana/transaction/memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/bxsolana/transaction/signing.py` & `bxsolana-trader-1.7.0/bxsolana/transaction/signing.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/bxsolana_trader.egg-info/PKG-INFO` & `bxsolana-trader-1.7.0/bxsolana_trader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -91,15 +91,15 @@
     
     you can also push the package to pypi 
     $ rm -rf python/dist/
     $ python3 -m build
     $ python3 -m twine upload --repository pypi dist/*
     
     and install the package locally now
-    $ python -m pip install ~/solana-trader-proto/python
+    $ pip install dist/bxsolana-trader-proto-0.0.18.tar.gz
     
     now you can update the depdendency in solana-trader-client-python
     update the version of bxsolana-trader-proto in setup.cfg
     and run 
     $ pip install -r requirements.txt
```

### Comparing `bxsolana-trader-1.6.0/bxsolana_trader.egg-info/SOURCES.txt` & `bxsolana-trader-1.7.0/bxsolana_trader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/setup.cfg` & `bxsolana-trader-1.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [metadata]
 name = bxsolana-trader
-version = 1.6.0
+version = 1.7.0
 description = Python SDK for bloXroute's Solana Trader API
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = bloXroute Labs
 author_email = support@bloxroute.com
 url = https://github.com/bloXroute-Labs/solana-trader-client-python
 keywords = serum, solana, blockchain, trader, grpc, stream
 classifiers = Programming Language :: Python :: 3
 
 [options]
 packages = find:
 install_requires = 
 	aiohttp==3.8.1
-	betterproto[compiler]==1.2.5
 	grpclib==0.4.3
 	aiounittest==1.4.1
 	base58==2.1.1
 	solana==0.29.1
 	solders==0.14.4
 	bx-jsonrpc-py==0.2.0
-	bxsolana-trader-proto==0.0.18
+	protobuf==4.21.8
+	betterproto==v2.0.0-beta5
+	bxsolana-trader-proto==0.0.24
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `bxsolana-trader-1.6.0/test/integration/private.py` & `bxsolana-trader-1.7.0/test/integration/private.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/test/integration/public.py` & `bxsolana-trader-1.7.0/test/integration/public.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/test/integration/stream.py` & `bxsolana-trader-1.7.0/test/integration/stream.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/test/integration/test_grpc.py` & `bxsolana-trader-1.7.0/test/integration/test_grpc.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/test/integration/test_http.py` & `bxsolana-trader-1.7.0/test/integration/test_http.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/test/integration/test_ws.py` & `bxsolana-trader-1.7.0/test/integration/test_ws.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/test/unit/transaction/test_memo.py` & `bxsolana-trader-1.7.0/test/unit/transaction/test_memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.6.0/test/unit/transaction/test_signing.py` & `bxsolana-trader-1.7.0/test/unit/transaction/test_signing.py`

 * *Files identical despite different names*

