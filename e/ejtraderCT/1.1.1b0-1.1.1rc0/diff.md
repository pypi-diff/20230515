# Comparing `tmp/ejtraderCT-1.1.1b0.tar.gz` & `tmp/ejtraderCT-1.1.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderCT-1.1.1b0.tar", last modified: Sun May 14 04:36:05 2023, max compression
+gzip compressed data, was "ejtraderCT-1.1.1rc0.tar", last modified: Mon May 15 21:56:39 2023, max compression
```

## Comparing `ejtraderCT-1.1.1b0.tar` & `ejtraderCT-1.1.1rc0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.959381 ejtraderCT-1.1.1b0/ejtraderCT/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/ejtraderCT/api/
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/Symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/ctrader.py
--rw-r--r--   0 runner    (1001) docker     (123)    26527 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/fix.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.959381 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-14 04:36:05.000000 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-14 04:36:05.000000 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 04:36:05.000000 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 04:36:05.000000 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/test/test_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:39.445224 ejtraderCT-1.1.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-15 21:56:39.445224 ejtraderCT-1.1.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:39.445224 ejtraderCT-1.1.1rc0/ejtraderCT/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/ejtraderCT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:39.445224 ejtraderCT-1.1.1rc0/ejtraderCT/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/ejtraderCT/api/Symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/ejtraderCT/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/ejtraderCT/api/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/ejtraderCT/api/ctrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26806 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/ejtraderCT/api/fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/ejtraderCT/api/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:39.445224 ejtraderCT-1.1.1rc0/ejtraderCT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-15 21:56:39.000000 ejtraderCT-1.1.1rc0/ejtraderCT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 21:56:39.000000 ejtraderCT-1.1.1rc0/ejtraderCT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:56:39.000000 ejtraderCT-1.1.1rc0/ejtraderCT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 21:56:39.000000 ejtraderCT-1.1.1rc0/ejtraderCT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:56:39.449225 ejtraderCT-1.1.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:39.445224 ejtraderCT-1.1.1rc0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 21:56:28.000000 ejtraderCT-1.1.1rc0/test/test_math.py
```

### Comparing `ejtraderCT-1.1.1b0/PKG-INFO` & `ejtraderCT-1.1.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: ejtraderCT
-Version: 1.1.1b0
+Version: 1.1.1rc0
 Summary: Ctrader Fix API
 Home-page: https://ejtraderCT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso & Douglas Barros
 Author-email: support@ejtrader.com
-License: GPL-3.0
-Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
-Project-URL: Source, https://github.com/traderpedroso/ejtraderCT
+License: MIT License
+Project-URL: Bug Reports, https://github.com/ejtraderLabs/ejtraderCT/issues
+Project-URL: Source, https://github.com/ejtraderLabs/ejtraderCT
 Project-URL: Documentation, https://ejtraderCT.readthedocs.io/
 Keywords: ctrader,fix-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
@@ -95,15 +93,15 @@
 from ejtraderCT import Ctrader
 ```
 
 ### Fix account login and details
 
 ```python
 server="168.205.95.20" # - Host name: (Current IP address 168.205.95.20 can be changed without notice)
-account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104928
+account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104926
 password="12345678" # - The password you configured
 
 api = Ctrader(server,account,password)
 
 ```
 ##### Check the connection status
 ```python
```

### Comparing `ejtraderCT-1.1.1b0/README.md` & `ejtraderCT-1.1.1rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 from ejtraderCT import Ctrader
 ```
 
 ### Fix account login and details
 
 ```python
 server="168.205.95.20" # - Host name: (Current IP address 168.205.95.20 can be changed without notice)
-account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104928
+account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104926
 password="12345678" # - The password you configured
 
 api = Ctrader(server,account,password)
 
 ```
 ##### Check the connection status
 ```python
```

### Comparing `ejtraderCT-1.1.1b0/ejtraderCT/api/Symbol.py` & `ejtraderCT-1.1.1rc0/ejtraderCT/api/Symbol.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.1.1b0/ejtraderCT/api/ctrader.py` & `ejtraderCT-1.1.1rc0/ejtraderCT/api/ctrader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,121 +1,192 @@
-from locale import currency
+# from locale import currency
 import logging
 import json
 import time
 import random
-import os
 from operator import itemgetter
 from .fix import FIX, Side, OrderType
 from .Symbol import SYMBOLSLIST
-class Ctrader:
 
-    def __init__(self,server,account,password,debug=False):
+
+class Ctrader:
+    def __init__(
+        self,
+        server=None,
+        account=None,
+        password=None,
+        currency="EUR",
+        client_id=1,
+        debug=False,
+    ):
         """AI is creating summary for __init__
 
         Args:
             server ([str]): [example h8.p.c-trader.cn]
             account ([str]): [live.icmarkets.1104926 or demo.icmarkets.1104926]
             password ([str]): [example 12345678 need to setup when you create api on ctrader platform]
         """
         if debug:
             logging.getLogger().setLevel(logging.INFO)
         split_string = account.split(".")
         broker = split_string[0] + "." + split_string[1]
         login = split_string[2]
-        currency = "EUR"
+
         self.client = c = {
-            '_id': '1',
-            'server': server,
-            'broker': broker,
-            'login': login,
-            'password': password,
-            'currency': currency,
-            'fix_status': 0,
-            'positions': [],
-            'orders': []
+            "_id": client_id,
+            "server": server,
+            "broker": broker,
+            "login": login,
+            "password": password,
+            "currency": currency,
+            "fix_status": 0,
+            "positions": [],
+            "orders": [],
         }
-        self.fix = FIX(c['server'], c['broker'], c['login'], c['password'], c['currency'], c['_id'], self.position_list_callback, self.order_list_callback)
+        self.fix = FIX(
+            c["server"],
+            c["broker"],
+            c["login"],
+            c["password"],
+            c["currency"],
+            c["_id"],
+            self.position_list_callback,
+            self.order_list_callback,
+        )
         self.market_data_list = {}
-        self.symbol_table = SYMBOLSLIST['default']
+        self.symbol_table = SYMBOLSLIST["default"]
 
-    def trade(self, symbol, action, type, actionType, volume, stoploss, takeprofit, price, deviation, id):
-        #"1 OPEN|EURUSD|1234567890|1|1.2|1.3|0.01|0|0"
-        # OPEN CLOSED PCLOSED MODIFY
+    def trade(
+        self,
+        symbol,
+        action,
+        type,
+        actionType,
+        volume,
+        stoploss,
+        takeprofit,
+        price,
+        deviation,
+        id,
+    ):
         v_action = action
         v_symbol = symbol
-        v_ticket = id if id != None else '{:.7f}'.format(time.time()).replace('.', '') + str(random.randint(10000, 99999))
+        v_ticket = (
+            id
+            if id
+            else "{:.7f}".format(time.time()).replace(".", "")
+            + str(random.randint(10000, 99999))
+        )
         v_type = str(type)
         v_openprice = price
         v_lots = volume
         v_sl = stoploss
         v_tp = takeprofit
 
-        logging.info("Action: %s, Symbol: %s, Lots: %s, Ticket: %s", v_action, v_symbol, v_lots, v_ticket)
+        logging.info(
+            "Action: %s, Symbol: %s, Lots: %s, Ticket: %s, price: %s, takeprofit: %s, stoploss: %s, type: %s",
+            v_action,
+            v_symbol,
+            v_lots,
+            v_ticket,
+            v_openprice,
+            v_sl,
+            v_tp,
+            v_type,
+        )
 
         otype = actionType
         symbol = v_symbol[:6]
         size = int(float(v_lots) * 100000)
-        
-        client_id = str(self.client['_id'])
-        command = ''
-        if v_action == 'OPEN':
+        global ticket
+        client_id = str(self.client["_id"])
+        command = ""
+        if v_action == "OPEN":
             if int(v_type) > 1:
                 # abre ordem pendente
-                command = '{0} {1} {2} {3} {4}'.format(otype, symbol, size, v_openprice, v_ticket)
+                command = "{0} {1} {2} {3} {4}".format(
+                    otype, symbol, size, v_openprice, v_ticket
+                )
+                self.parse_command(command, client_id)
             else:
                 # abre posicao a mercado
-                command = '{0} {1} {2} {3}'.format(otype, symbol, size, v_ticket)
-        elif v_action in ['CLOSED', 'PCLOSED']:
-            if int(v_type) > 1:
-                # ORDEM
-                # cancela ordens pendentes
-                self.fix.cancel_order(v_ticket)
-                ticket_orders = self.getOrdersIdByOriginId(v_ticket, client_id)
-                self.cancelOrdersByOriginId(ticket_orders, client_id)
-                return
-            else:
-                # POSICAO
-                self.fix.close_position(v_ticket, size)
-                # cancela ordens pendentes abertas de TP e SL
-                ticket_orders = self.getOrdersIdByOriginId(v_ticket, client_id)
-                self.cancelOrdersByOriginId(ticket_orders, client_id)
-                return
-            
-        elif v_action == 'MODIFY':
+                command = "{0} {1} {2} {3}".format(otype, symbol, size, v_ticket)
+                self.parse_command(command, client_id)
+
+                while True:
+                    try:
+                        ticket = self.fix.origin_to_pos_id[v_ticket]
+                        if ticket:  # Verifica se a variável ticket não está vazia
+                            break
+                    except Exception as e:
+                        logging.info(e)
+                        continue
+
+                if ticket:
+                    if float(v_sl) > 0:
+                        # abre posicao pendente SL
+                        otype = "sell stop" if v_type == "0" else "buy stop"
+                        command = "{0} {1} {2} {3} {4} {5}".format(
+                            otype, symbol, size, v_sl, v_ticket, ticket
+                        )
+                        self.parse_command(command, client_id)
+                    if float(v_tp) > 0:
+                        # cancela ordens pendentes abertas de TP e SL
+                        ticket_orders = self.getOrdersIdByOriginId(v_ticket, client_id)
+                        # abre posicao pendente TP
+                        otype = "sell limit" if v_type == "0" else "buy limit"
+                        command = "{0} {1} {2} {3} {4} {5}".format(
+                            otype, symbol, size, v_tp, v_ticket, ticket
+                        )
+                        self.parse_command(command, client_id)
+        elif v_action == "MODIFY":
             # POSICAO: verifica qual o ticket do client pelo ticket do server
             ticket = self.getPositionIdByOriginId(v_ticket, client_id)
-            if ticket != None:
+            if ticket:
                 # cancela ordens pendentes abertas de TP e SL
                 ticket_orders = self.getOrdersIdByOriginId(v_ticket, client_id)
                 self.cancelOrdersByOriginId(ticket_orders, client_id)
                 if float(v_sl) > 0:
                     # cancela ordens pendentes abertas de TP e SL
                     ticket_orders = self.getOrdersIdByOriginId(v_ticket, client_id)
                     self.cancelOrdersByOriginId(ticket_orders, client_id)
-                    # abre posicao pendente SL
-                    otype = 'sell stop' if v_type == '0' else 'buy stop'
-                    command = '{0} {1} {2} {3} {4} {5}'.format(otype, symbol, size, v_sl, v_ticket, ticket)
+                    otype = "sell stop" if v_type == "0" else "buy stop"
+                    command = "{0} {1} {2} {3} {4} {5}".format(
+                        otype, symbol, size, v_sl, v_ticket, ticket
+                    )
+                    self.parse_command(command, client_id)
                 if float(v_tp) > 0:
                     # cancela ordens pendentes abertas de TP e SL
                     ticket_orders = self.getOrdersIdByOriginId(v_ticket, client_id)
                     self.cancelOrdersByOriginId(ticket_orders, client_id)
                     # abre posicao pendente TP
-                    otype = 'sell limit' if v_type == '0' else 'buy limit'
-                    command = '{0} {1} {2} {3} {4} {5}'.format(otype, symbol, size, v_tp, v_ticket, ticket)
-            # ORDEM: verifica qual o ticket do client pelo ticket do server
-            tickets = self.getOrdersIdByOriginId(v_ticket, client_id)
-            if tickets != None and len(tickets) > 0:
-                # cancela ordens pendentes abertas
+                    otype = "sell limit" if v_type == "0" else "buy limit"
+                    command = "{0} {1} {2} {3} {4} {5}".format(
+                        otype, symbol, size, v_tp, v_ticket, ticket
+                    )
+                    self.parse_command(command, client_id)
+
+        elif v_action in ["CLOSED", "PCLOSED"]:
+            if int(v_type) > 1:
+                # ORDEM
+                # cancela ordens pendentes
+                self.fix.cancel_order(v_ticket)
                 ticket_orders = self.getOrdersIdByOriginId(v_ticket, client_id)
                 self.cancelOrdersByOriginId(ticket_orders, client_id)
-                # abre ordem pendente
-                command = '{0} {1} {2} {3} {4}'.format(otype, symbol, size, v_openprice, v_ticket)
+                self.parse_command(command, client_id)
+                return
+            else:
+                # POSICAO
+                self.fix.close_position(v_ticket, size)
+                # cancela ordens pendentes abertas de TP e SL
+                ticket_orders = self.getOrdersIdByOriginId(v_ticket, client_id)
+                self.cancelOrdersByOriginId(ticket_orders, client_id)
+                self.parse_command(command, client_id)
+                return
 
-        self.parse_command(command, client_id)
         return v_ticket
 
     def buy(self, symbol, volume, stoploss, takeprofit, price=0, deviation=5):
         """summary for buy
 
         Args:
             symbol ([str]): ["EURUSD"]
@@ -124,172 +195,257 @@
             takeprofit ([float]): [1.19]
             price (int, optional): [on the price]. Defaults to 0.
             deviation (int, optional): [5].standard deviation Defaults to 5.
 
         Returns:
             [int]: [order ID]
         """
-        return self.trade(symbol, "OPEN", 0, "buy", volume, stoploss, takeprofit, price, deviation, None)
+        return self.trade(
+            symbol,
+            "OPEN",
+            0,
+            "buy",
+            volume,
+            stoploss,
+            takeprofit,
+            price,
+            deviation,
+            None,
+        )
 
-    def sell(self, symbol, volume, stoploss, takeprofit, price=0, deviation=5):
+    def sell(self, symbol, volume, stoploss=0, takeprofit=9, price=0, deviation=5):
         """summary for sell
 
         Args:
             symbol ([str]): ["EURUSD"]
             volume ([float]): [0.01]
             stoploss ([float]): [1.19]
             takeprofit ([float]): [1.18]
             price (int, optional): [on the price]. Defaults to 0.
             deviation (int, optional): [5]. standard deviation Defaults to 5.
 
         Returns:
             [int]: [Order ID]
         """
-        return self.trade(symbol, "OPEN", 1, "sell", volume, stoploss, takeprofit, price, deviation, None)
+        return self.trade(
+            symbol,
+            "OPEN",
+            1,
+            "sell",
+            volume,
+            stoploss,
+            takeprofit,
+            price,
+            deviation,
+            None,
+        )
 
-    def buyLimit(self, symbol, volume, stoploss, takeprofit, price=0, deviation=5):
+    def buyLimit(self, symbol, volume, stoploss=0, takeprofit=0, price=0, deviation=5):
         """summary for buy Limit
 
         Args:
             symbol ([str]): ["EURUSD"]
             volume ([float]): [0.01]
             stoploss ([float]): [1.17]
             takeprofit ([float]): [1.19]
             price ([float]): [1.8]. Defaults to 0.
             deviation (int, optional): [5]. standard deviation Defaults to 5.
 
         Returns:
             [int]: [order ID]
         """
-        return self.trade(symbol, "OPEN", 2, "buy limit", volume, stoploss, takeprofit, price, deviation, None)
+        return self.trade(
+            symbol,
+            "OPEN",
+            2,
+            "buy limit",
+            volume,
+            stoploss,
+            takeprofit,
+            price,
+            deviation,
+            None,
+        )
 
-    def sellLimit(self, symbol, volume, stoploss, takeprofit, price=0, deviation=5):
+    def sellLimit(self, symbol, volume, stoploss=0, takeprofit=0, price=0, deviation=5):
         """summary for sellLimit
 
         Args:
             symbol ([str]): ["EURUSD"]
             volume ([float]): [0.01]
             stoploss ([type]): [1.23]
             takeprofit ([type]): [1.17]
             price (int, optional): [1.22]. Defaults to 0.
             deviation (int, optional): [description]. standard deviation Defaults to 5.
 
         Returns:
             [type]: [description]
         """
-        return self.trade(symbol, "OPEN", 3, "sell limit", volume, stoploss, takeprofit, price, deviation, None)
-
-    def buyStop(self, symbol, volume, stoploss, takeprofit, price=0, deviation=5):
-        return self.trade(symbol, "OPEN", 4, "buy stop", volume, stoploss, takeprofit, price, deviation, None)
+        return self.trade(
+            symbol,
+            "OPEN",
+            3,
+            "sell limit",
+            volume,
+            stoploss,
+            takeprofit,
+            price,
+            deviation,
+            None,
+        )
+
+    def buyStop(self, symbol, volume, stoploss=0, takeprofit=0, price=0, deviation=5):
+        return self.trade(
+            symbol,
+            "OPEN",
+            4,
+            "buy stop",
+            volume,
+            stoploss,
+            takeprofit,
+            price,
+            deviation,
+            None,
+        )
+
+    def sellStop(self, symbol, volume, stoploss=0, takeprofit=0, price=0, deviation=5):
+        return self.trade(
+            symbol,
+            "OPEN",
+            5,
+            "sell stop",
+            volume,
+            stoploss,
+            takeprofit,
+            price,
+            deviation,
+            None,
+        )
 
-    def sellStop(self, symbol, volume, stoploss, takeprofit, price=0, deviation=5):
-        return self.trade(symbol, "OPEN", 5, "sell stop", volume, stoploss, takeprofit, price, deviation, None)
-
-    def positionModify(self, id, stoploss, takeprofit):
+    def positionModify(self, id, symbol, volume, stoploss=0, takeprofit=0):
         buy = True
         if buy:
-            return self.trade("", "MODIFY", 0, "", 0, stoploss, takeprofit, 0, 5, id)
+            return self.trade(
+                "", "MODIFY", 0, symbol, volume, stoploss, takeprofit, 0, 5, id
+            )
         else:
             return self.trade("", "MODIFY", 1, "", 0, stoploss, takeprofit, 0, 5, id)
 
     def positionClosePartial(self, id, volume):
         return self.trade("", "PCLOSED", 0, "", volume, 0, 0, 0, 5, id)
 
     def positionCloseById(self, id, amount):
         try:
-           action= self.trade("", "CLOSED", 0, "", amount/100000, 0, 0, 0, 5, id)
-        except:
+            action = self.trade("", "CLOSED", 0, "", amount / 100000, 0, 0, 0, 5, id)
+        except Exception as e:
+            logging.info(e)
             action = None
             pass
         return action
 
     def orderModify(self, id, stoploss, takeprofit, price):
+        """_summary_
+
+        Args:
+            id (_type_): _description_
+            stoploss (_type_): _description_
+            takeprofit (_type_): _description_
+            price (_type_): _description_
+
+        Returns:
+            _type_: _description_
+        """
         buy = True
         if buy:
             return self.trade("", "MODIFY", 0, "", 0, stoploss, takeprofit, 0, 5, id)
         else:
             return self.trade("", "MODIFY", 1, "", 0, stoploss, takeprofit, 0, 5, id)
 
     def orderCancelById(self, id):
         try:
             action = self.trade("", "CLOSED", 2, "", 0, 0, 0, 0, 5, id)
-        except:
+        except Exception as e:
+            logging.info(e)
             action = None
             pass
         return action
-    
-    def accountInfo(self):
-        return json.loads(json.dumps(self.api.Command(action="ACCOUNT")))
 
     def positions(self):
-        return json.loads(json.dumps(self.client['positions']))
+        return json.loads(json.dumps(self.client["positions"]))
 
     def orders(self):
-        return json.loads(json.dumps(self.client['orders']))
+        return json.loads(json.dumps(self.client["orders"]))
 
-    
     def parse_command(self, command: str, client_id: str):
         parts = command.split(" ")
-        logging.debug(parts)
-        logging.info("Command: %s - client_id: %s", command, client_id)
+        logging.info(parts)
+        logging.info(f"Command: {command} ")
 
-        if self.fix.logged == False:
+        if not self.fix.logged:
             logging.info("waiting logging...")
             return
 
         if parts[0] == "sub":
             try:
                 subid = int(parts[1])
-                self.fix.market_request(subid - 1, parts[2].upper(), self.quote_callback)
+                self.fix.market_request(
+                    subid - 1, parts[2].upper(), self.quote_callback
+                )
             except ValueError:
                 logging.error("Invalid subscription ID")
         if parts[0] in ["buy", "sell"]:
             if parts[1] in ["stop", "limit"]:
                 self.fix.new_limit_order(
                     parts[2].upper(),
                     Side.Buy if parts[0] == "buy" else Side.Sell,
                     OrderType.Limit if parts[1] == "limit" else OrderType.Stop,
                     float(parts[3]),
                     float(parts[4]),
                     parts[5] if len(parts) >= 6 else None,
-                    parts[6] if len(parts) >= 7 else None
+                    parts[6] if len(parts) >= 7 else None,
                 )
             else:
                 self.fix.new_market_order(
                     parts[1].upper(),
                     Side.Buy if parts[0] == "buy" else Side.Sell,
                     float(parts[2]),
                     parts[3] if len(parts) >= 4 else None,
-                    parts[4] if len(parts) >= 5 else None
+                    parts[4] if len(parts) >= 5 else None,
                 )
         if parts[0] == "close":
             if parts[1] == "all":
                 self.fix.close_all()
             else:
                 if len(parts) == 3:
                     self.fix.close_position(parts[1], parts[2])
                 else:
                     self.fix.close_position(parts[1])
         if parts[0] == "cancel":
             if parts[1] == "all":
                 self.fix.cancel_all()
             else:
                 self.fix.cancel_order(parts[1])
-    
-    def float_format(self, fmt: str, num: float, force_sign = True):
-        return max(('{:+}' if force_sign else "{}").format(round(num, 6)), fmt.format(num), key=len)
-    
+
+    def float_format(self, fmt: str, num: float, force_sign=True):
+        return max(
+            ("{:+}" if force_sign else "{}").format(round(num, 6)),
+            fmt.format(num),
+            key=len,
+        )
+
     def position_list_callback(self, data: dict, price_data: dict, client_id: str):
         positions = []
         for i, kv in enumerate(data.items()):
             pos_id = kv[0]
             name = kv[1]["name"]
             side = "Buy" if kv[1]["long"] > 0 else "Sell"
             amount = kv[1]["long"] if kv[1]["long"] > 0 else kv[1]["short"]
-            price_str = self.float_format("{:.%df}" % kv[1]["digits"], kv[1]["price"], False)
+            price_str = self.float_format(
+                "{:.%df}" % kv[1]["digits"], kv[1]["price"], False
+            )
             price = price_data.get(name, None)
             actual_price = ""
             diff_str = ""
             pl_str = ""
             gain_str = ""
             if price:
                 if side == "Buy":
@@ -310,126 +466,132 @@
                     if convert_dir:
                         rate = 1 / price["ask"]
                     else:
                         rate = price["bid"]
                     pl_base = pl * rate
                     gain_str = "{:+.2f}".format(round(pl_base, 2))
             # adiciona informacoes de posicoes no client
-            positions.append({
-                "pos_id" : pos_id,
-                "name" : name,
-                "side" : side,
-                "amount" : amount,
-                "price" : price_str,
-                "actual_price" : actual_price,
-                "diff" : diff_str,
-                "pl" : pl_str,
-                "gain" : gain_str
-            })
-        self.client.update(positions = positions)
+            positions.append(
+                {
+                    "pos_id": pos_id,
+                    "name": name,
+                    "side": side,
+                    "amount": amount,
+                    "price": price_str,
+                    "actual_price": actual_price,
+                    "diff": diff_str,
+                    "pl": pl_str,
+                    "gain": gain_str,
+                }
+            )
+        self.client.update(positions=positions)
         logging.debug("client_id %s positions: %s", client_id, positions)
 
     def getPositionIdByOriginId(self, posId: str, client_id: str):
         if posId in self.fix.origin_to_pos_id:
             return self.fix.position_list[self.fix.origin_to_pos_id[posId]]
 
     def getOrdersIdByOriginId(self, ordId: str, client_id: str):
-        if ordId in self.fix.origin_to_ord_id:  # Verifique se a chave existe antes de acessá-la
+        if (
+            ordId in self.fix.origin_to_ord_id
+        ):  # Verifique se a chave existe antes de acessá-la
             return self.fix.origin_to_ord_id[ordId]
         else:
             return None  # Retorne None ou outro valor padrão quando a chave não existir
 
     def cancelOrdersByOriginId(self, clIdArr, client_id: str):
-        if clIdArr == None:
+        if not clIdArr:
             return
         for clId in clIdArr:
             self.fix.cancel_order(clId)
-            
-    def subscribe(self, *symbol): 
+
+    def subscribe(self, *symbol):
         symbol = list(symbol)
         for symbols in symbol:
-            self.fix.spot_market_request(symbols) 
- 
-    def quote(self, symbol=None): 
-        if symbol and symbol not in self.fix.spot_price_list: 
+            self.fix.spot_market_request(symbols)
+
+    def quote(self, symbol=None):
+        if symbol and symbol not in self.fix.spot_price_list:
             return "Symbol not Subscribed"
         elif symbol:
-            return self.fix.spot_price_list[symbol]     
+            return self.fix.spot_price_list[symbol]
         return self.fix.spot_price_list
-    
+
     def order_list_callback(self, data: dict, price_data: dict, client_id: str):
         orders = []
         for i, kv in enumerate(data.items()):
             ord_id = kv[0]
             name = kv[1]["name"]
             side = "Buy" if kv[1]["side"] == Side.Buy else "Sell"
             amount = kv[1]["amount"]
             order_type = kv[1]["type"]
             price_str = ""
             if order_type > 1:
-                price_str = self.float_format("{:.%df}" % kv[1]["digits"], kv[1]["price"], False)
+                price_str = self.float_format(
+                    "{:.%df}" % kv[1]["digits"], kv[1]["price"], False
+                )
             price = price_data.get(name, None)
             actual_price = ""
             if price:
                 if side == "Buy":
                     price = price["ask"]
                 else:
                     price = price["bid"]
-                actual_price = self.float_format("{:.%df}" % kv[1]["digits"], price, False)
+                actual_price = self.float_format(
+                    "{:.%df}" % kv[1]["digits"], price, False
+                )
             pos_id = kv[1]["pos_id"]
             # adiciona informacoes de ordens no client
-            orders.append({
-                "ord_id" : ord_id,
-                "name" : name,
-                "side" : side,
-                "amount" : amount,
-                "price" : price_str,
-                "actual_price" : actual_price,
-                "pos_id" : pos_id,
-                "clid" : kv[1]["clid"]
-            })
-        self.client.update(orders = orders)
+            orders.append(
+                {
+                    "ord_id": ord_id,
+                    "name": name,
+                    "side": side,
+                    "amount": amount,
+                    "price": price_str,
+                    "actual_price": actual_price,
+                    "pos_id": pos_id,
+                    "clid": kv[1]["clid"],
+                }
+            )
+        self.client.update(orders=orders)
         logging.debug("client_id %s orders: %s", client_id, orders)
 
     def quote_callback(self, name: str, digits: int, data: dict):
         if len(data) == 0:
             return
         ask = []
         bid = []
         for e in data.values():
             if e["type"] == 0:
                 bid.append(e)
             else:
                 ask.append(e)
         ask.sort(key=itemgetter("price"))
         bid.sort(key=itemgetter("price"), reverse=True)
-        for i, e in enumerate(bid):
-            p = ("{:.%df}" % digits).format(e["price"])
-            if "size" in e.keys():
-                a = str(e["size"])
-        for i, e in enumerate(ask):
-            p = ("{:.%df}" % digits).format(e["price"])
-            if "size" in e.keys():
-                a = str(e["size"])
+
         bid_str = ("{:.%df}" % digits).format(bid[0]["price"])
         offer_str = ("{:.%df}" % digits).format(ask[0]["price"])
         spread_str = ("{:.%df}" % digits).format(ask[0]["price"] - bid[0]["price"])
-        self.market_data_list[name] = { "bid": bid_str, "ask": offer_str, "spread": spread_str, "time": time.time()}
-    
+        self.market_data_list[name] = {
+            "bid": bid_str,
+            "ask": offer_str,
+            "spread": spread_str,
+            "time": time.time(),
+        }
+
     def close_all(self):
         self.fix.close_all()
-    
+
     def cancel_all(self):
         self.fix.cancel_all()
-        
+
     def logout(self):
         if self.isconnected():
             self.fix.logout()
             logout = "Logged out"
         else:
             logout = "Not logged in"
         return logout
-    
-    
+
     def isconnected(self):
         return self.fix.logged
-
```

### Comparing `ejtraderCT-1.1.1b0/ejtraderCT/api/fix.py` & `ejtraderCT-1.1.1rc0/ejtraderCT/api/fix.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,59 +623,62 @@
         self.subscribed_symbol[subid] = msg[Field.Symbol]
         self.market_callback = callback
         self.send_message(msg)
         self.market_seq += 1
 
     def spot_market_request(self, symbol):
         msg = FIX.Message(SubID.QUOTE, "V", self)
-        msg[Field.MDReqID] = -1
+        msg[Field.MDReqID] = self.client_id
         msg[Field.SubscriptionRequestType] = 1
         msg[Field.MarketDepth] = 1
         msg[Field.NoMDEntryTypes] = 2
         msg[Field.MDEntryType] = 0
         msg[Field.MDEntryType] = 1
         msg[Field.NoRelatedSym] = 1
         msg[Field.Symbol] = self.sec_name_table[symbol]["id"]
         self.spot_request_list.add(symbol)
         self.send_message(msg)
 
     def position_request(self):
         msg = FIX.Message(SubID.TRADE, "AN", self)
-        msg[Field.PosReqID] = 16336345
+        msg[Field.PosReqID] = self.client_id
         self.send_message(msg)
 
     def order_request(self):
         msg = FIX.Message(SubID.TRADE, "AF", self)
-        msg[Field.MassStatusReqID] = 1
+        msg[Field.MassStatusReqID] = self.client_id
         msg[Field.MassStatusReqType] = 7
         self.send_message(msg)
 
     def sec_list(self, callback=None):
         msg = FIX.Message(SubID.QUOTE, "x", self)
-        msg[Field.SecurityReqID] = 1
+        msg[Field.SecurityReqID] = self.client_id
         msg[Field.SecurityListRequestType] = 0
         self.sec_list_callback = callback
         self.send_message(msg)
 
     def new_market_order(
         self, symbol, side: Side, size: float, originId=None, pos_id=None
     ):
+        logging.info(f"error ORIGINAL ID: {originId}")
+        logging.info(f"error POS ID: {pos_id}")
         if symbol not in self.sec_name_table:
             return
 
         msg = FIX.Message(SubID.TRADE, "D", self)
         msg[Field.ClOrdId] = originId if originId else "dt" + get_time()
         msg[Field.Symbol] = self.sec_name_table[symbol]["id"]
         msg[Field.Side] = side.value
         msg[Field.TransactTime] = get_time()
         msg[Field.OrderQty] = size
         msg[Field.OrdType] = OrderType.Market.value
-        msg[Field.Designation] = "test label"
+        msg[Field.Designation] = f"EjtraderCT ClientID: {self.client_id}"
         if pos_id:
             msg[Field.PosMaintRptID] = pos_id
+
         self.send_message(msg)
 
     def close_position(self, pos_id: str, lots):
         if pos_id not in self.position_list:
             return
 
         # remove referencia ao server ord_id da tabela de-para
@@ -720,14 +723,16 @@
         side: Side,
         order_type: OrderType,
         size: float,
         price: float,
         originId=None,
         pos_id=None,
     ):
+        logging.info(f"error ORIGINAL ID: {originId}")
+        logging.info(f"error POS ID: {pos_id}")
         if symbol not in self.sec_name_table:
             return
 
         msg = FIX.Message(SubID.TRADE, "D", self)
         msg[Field.ClOrdId] = originId if originId else "dt" + get_time()
         msg[Field.Symbol] = self.sec_name_table[symbol]["id"]
         msg[Field.Side] = side.value
```

### Comparing `ejtraderCT-1.1.1b0/ejtraderCT/api/math.py` & `ejtraderCT-1.1.1rc0/ejtraderCT/api/math.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.1.1b0/ejtraderCT.egg-info/PKG-INFO` & `ejtraderCT-1.1.1rc0/ejtraderCT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: ejtraderCT
-Version: 1.1.1b0
+Version: 1.1.1rc0
 Summary: Ctrader Fix API
 Home-page: https://ejtraderCT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso & Douglas Barros
 Author-email: support@ejtrader.com
-License: GPL-3.0
-Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
-Project-URL: Source, https://github.com/traderpedroso/ejtraderCT
+License: MIT License
+Project-URL: Bug Reports, https://github.com/ejtraderLabs/ejtraderCT/issues
+Project-URL: Source, https://github.com/ejtraderLabs/ejtraderCT
 Project-URL: Documentation, https://ejtraderCT.readthedocs.io/
 Keywords: ctrader,fix-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
@@ -95,15 +93,15 @@
 from ejtraderCT import Ctrader
 ```
 
 ### Fix account login and details
 
 ```python
 server="168.205.95.20" # - Host name: (Current IP address 168.205.95.20 can be changed without notice)
-account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104928
+account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104926
 password="12345678" # - The password you configured
 
 api = Ctrader(server,account,password)
 
 ```
 ##### Check the connection status
 ```python
```

### Comparing `ejtraderCT-1.1.1b0/setup.py` & `ejtraderCT-1.1.1rc0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,34 +14,32 @@
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
     name="ejtraderCT",
-    version="1.1.1b0",
+    version="1.1.1rc0",
     packages=find_packages(),
     url="https://ejtraderCT.readthedocs.io/",
     download_url="https://ejtrader.com",
-    license="GPL-3.0",
+    license="MIT License",
     author="Emerson Pedroso & Douglas Barros",
     author_email="support@ejtrader.com",
     description="Ctrader Fix API",
     long_description=readme(),
     long_description_content_type="text/markdown",
     install_requires=requirements(filename="requirements.txt"),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Topic :: Office/Business :: Financial",
         "Topic :: Office/Business :: Financial :: Investment",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Software Development :: Libraries",
     ],
@@ -59,12 +57,12 @@
             "currency crosses",
             "bonds",
             "commodities",
             "crypto currencies",
         ]
     ),
     project_urls={
-        "Bug Reports": "https://github.com/traderpedroso/ejtraderCT/issues",
-        "Source": "https://github.com/traderpedroso/ejtraderCT",
+        "Bug Reports": "https://github.com/ejtraderLabs/ejtraderCT/issues",
+        "Source": "https://github.com/ejtraderLabs/ejtraderCT",
         "Documentation": "https://ejtraderCT.readthedocs.io/",
     },
 )
```

### Comparing `ejtraderCT-1.1.1b0/test/test_math.py` & `ejtraderCT-1.1.1rc0/test/test_math.py`

 * *Files identical despite different names*

