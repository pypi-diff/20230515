# Comparing `tmp/tonconnect-0.1.0.tar.gz` & `tmp/tonconnect-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonconnect-0.1.0.tar", last modified: Tue Apr 25 18:15:34 2023, max compression
+gzip compressed data, was "tonconnect-0.1.1.tar", last modified: Mon May 15 14:06:44 2023, max compression
```

## Comparing `tonconnect-0.1.0.tar` & `tonconnect-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.1.0/.gitignore
--rw-r--r--   0        0        0    11350 2023-04-14 20:08:17.432870 tonconnect-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1783 2023-04-25 18:14:12.277674 tonconnect-0.1.0/README.md
--rw-r--r--   0        0        0      288 2023-04-12 09:33:18.589470 tonconnect-0.1.0/examples/address.py
--rw-r--r--   0        0        0      464 2023-04-25 17:58:46.142134 tonconnect-0.1.0/examples/async_address.py
--rw-r--r--   0        0        0      782 2023-04-21 11:32:11.563469 tonconnect-0.1.0/examples/transactions.py
--rw-r--r--   0        0        0      556 2023-04-25 18:13:07.309181 tonconnect-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.1.0/tonconnect/__init__.py
--rw-r--r--   0        0        0      261 2023-04-25 17:59:41.572138 tonconnect-0.1.0/tonconnect/apps.py
--rw-r--r--   0        0        0     3759 2023-04-25 18:07:17.059721 tonconnect-0.1.0/tonconnect/bridge.py
--rw-r--r--   0        0        0     2234 2023-04-25 17:51:46.989345 tonconnect-0.1.0/tonconnect/connector.py
--rw-r--r--   0        0        0     1202 2023-04-12 07:19:51.920373 tonconnect-0.1.0/tonconnect/crypto.py
--rw-r--r--   0        0        0     3442 2023-04-12 07:39:01.886103 tonconnect-0.1.0/tonconnect/events.py
--rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.1.0/tonconnect/exceptions.py
--rw-r--r--   0        0        0     2930 2023-04-25 18:02:37.265076 tonconnect-0.1.0/tonconnect/httpbridge.py
--rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.1.0/tonconnect/options.py
--rw-r--r--   0        0        0     1733 2023-04-24 10:38:25.387486 tonconnect-0.1.0/tonconnect/requests.py
--rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.1.0/tonconnect/static.py
--rw-r--r--   0        0        0      299 2023-04-12 07:37:03.212040 tonconnect-0.1.0/tonconnect/url.py
--rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.1.0/tonconnect/utils.py
--rw-r--r--   0        0        0      416 2023-04-25 17:06:44.302885 tonconnect-0.1.0/tonconnect/wallet.py
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 tonconnect-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11350 2023-04-14 20:08:17.432870 tonconnect-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     2479 2023-05-15 14:06:16.868138 tonconnect-0.1.1/README.md
+-rw-r--r--   0        0        0      288 2023-05-15 13:57:22.007525 tonconnect-0.1.1/examples/address.py
+-rw-r--r--   0        0        0      324 2023-05-15 13:59:35.231854 tonconnect-0.1.1/examples/all_versions_support.py
+-rw-r--r--   0        0        0      464 2023-05-15 13:57:18.790724 tonconnect-0.1.1/examples/async_address.py
+-rw-r--r--   0        0        0      782 2023-04-21 11:32:11.563469 tonconnect-0.1.1/examples/transactions.py
+-rw-r--r--   0        0        0      556 2023-05-15 13:59:54.795490 tonconnect-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.1.1/tonconnect/__init__.py
+-rw-r--r--   0        0        0      261 2023-04-25 17:59:41.572138 tonconnect-0.1.1/tonconnect/apps.py
+-rw-r--r--   0        0        0     3759 2023-04-25 18:07:17.059721 tonconnect-0.1.1/tonconnect/bridge.py
+-rw-r--r--   0        0        0     3973 2023-05-15 13:58:03.508537 tonconnect-0.1.1/tonconnect/connector.py
+-rw-r--r--   0        0        0     1202 2023-04-12 07:19:51.920373 tonconnect-0.1.1/tonconnect/crypto.py
+-rw-r--r--   0        0        0     3442 2023-04-12 07:39:01.886103 tonconnect-0.1.1/tonconnect/events.py
+-rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.1.1/tonconnect/exceptions.py
+-rw-r--r--   0        0        0     2930 2023-04-25 18:02:37.265076 tonconnect-0.1.1/tonconnect/httpbridge.py
+-rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.1.1/tonconnect/options.py
+-rw-r--r--   0        0        0     1733 2023-04-24 10:38:25.387486 tonconnect-0.1.1/tonconnect/requests.py
+-rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.1.1/tonconnect/static.py
+-rw-r--r--   0        0        0      330 2023-05-12 16:46:40.731106 tonconnect-0.1.1/tonconnect/url.py
+-rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.1.1/tonconnect/utils.py
+-rw-r--r--   0        0        0      416 2023-04-25 17:06:44.302885 tonconnect-0.1.1/tonconnect/wallet.py
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 tonconnect-0.1.1/PKG-INFO
```

### Comparing `tonconnect-0.1.0/LICENSE.md` & `tonconnect-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.0/README.md` & `tonconnect-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 ## Getting Started
 
 ### Dependencies
 
 * PyNaCl
 * tonsdk (will be removed in the future)
+* aiohttp
+* requests
 
 ### Installing
 
 ```
 git clone https://github.com/ClickoTON-Foundation/tonconnect.git
 pip install -e tonconnect
 ```
@@ -33,14 +35,31 @@
 
 print(f'Universal connect url for Tonkeeper: {url}')
 
 address = connector.get_address()
 print(f'Successfuly connected {address}.')
 ```
 
+Example of connecting wallet with help of tonapi.io.
+tonapi.io it's used to obtain a public key, which adds support for all versions of the wallet that have the get_public_key method. (These are all versions except v3r1).
+But if the wallet isn't already deployed, user will not be able to log in.
+
+```python
+from tonconnect.connector import Connector
+
+
+connector = Connector('https://tonclick.online/ton-connect.json', use_tonapi=True, tonapi_token=None)
+url = connector.connect('tonkeeper', 'test')
+
+print(f'Universal connect url for Tonkeeper: {url}')
+
+address = connector.get_address()
+print(f'Successfuly connected {address}.')
+```
+
 Example of asynchronous connecting wallet.
 
 ```python
 import asyncio
 from tonconnect.connector import AsyncConnector
 
 
@@ -61,14 +80,16 @@
 
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.1.1
+    * Added tonapi.io support
 * 0.1.0
     * Async wrapper
 * 0.0.2 & 0.0.3
     * pyproject.toml fix
 * 0.0.1
     * Initial Beta
```

### Comparing `tonconnect-0.1.0/examples/transactions.py` & `tonconnect-0.1.1/examples/transactions.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.0/pyproject.toml` & `tonconnect-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "tonconnect"
 description = "TON Connect - Python library for using TON Connect 2."
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Vlad100"}
 ]
 dependencies = [
     "pynacl",
     "requests",
     "tonsdk",
```

### Comparing `tonconnect-0.1.0/tonconnect/bridge.py` & `tonconnect-0.1.1/tonconnect/bridge.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.0/tonconnect/crypto.py` & `tonconnect-0.1.1/tonconnect/crypto.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.0/tonconnect/events.py` & `tonconnect-0.1.1/tonconnect/events.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.0/tonconnect/httpbridge.py` & `tonconnect-0.1.1/tonconnect/httpbridge.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.0/tonconnect/requests.py` & `tonconnect-0.1.1/tonconnect/requests.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.0/PKG-INFO` & `tonconnect-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonconnect
-Version: 0.1.0
+Version: 0.1.1
 Summary: TON Connect - Python library for using TON Connect 2.
 Author: Vlad100
 Description-Content-Type: text/markdown
 Requires-Dist: pynacl
 Requires-Dist: requests
 Requires-Dist: tonsdk
 Requires-Dist: aiohttp
@@ -22,14 +22,16 @@
 
 ## Getting Started
 
 ### Dependencies
 
 * PyNaCl
 * tonsdk (will be removed in the future)
+* aiohttp
+* requests
 
 ### Installing
 
 ```
 git clone https://github.com/ClickoTON-Foundation/tonconnect.git
 pip install -e tonconnect
 ```
@@ -47,14 +49,31 @@
 
 print(f'Universal connect url for Tonkeeper: {url}')
 
 address = connector.get_address()
 print(f'Successfuly connected {address}.')
 ```
 
+Example of connecting wallet with help of tonapi.io.
+tonapi.io it's used to obtain a public key, which adds support for all versions of the wallet that have the get_public_key method. (These are all versions except v3r1).
+But if the wallet isn't already deployed, user will not be able to log in.
+
+```python
+from tonconnect.connector import Connector
+
+
+connector = Connector('https://tonclick.online/ton-connect.json', use_tonapi=True, tonapi_token=None)
+url = connector.connect('tonkeeper', 'test')
+
+print(f'Universal connect url for Tonkeeper: {url}')
+
+address = connector.get_address()
+print(f'Successfuly connected {address}.')
+```
+
 Example of asynchronous connecting wallet.
 
 ```python
 import asyncio
 from tonconnect.connector import AsyncConnector
 
 
@@ -75,14 +94,16 @@
 
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.1.1
+    * Added tonapi.io support
 * 0.1.0
     * Async wrapper
 * 0.0.2 & 0.0.3
     * pyproject.toml fix
 * 0.0.1
     * Initial Beta
```

