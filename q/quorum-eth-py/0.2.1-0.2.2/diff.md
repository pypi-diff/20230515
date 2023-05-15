# Comparing `tmp/quorum_eth_py-0.2.1.tar.gz` & `tmp/quorum_eth_py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_eth_py-0.2.1.tar", last modified: Mon May 15 05:27:31 2023, max compression
+gzip compressed data, was "quorum_eth_py-0.2.2.tar", last modified: Mon May 15 07:11:24 2023, max compression
```

## Comparing `quorum_eth_py-0.2.1.tar` & `quorum_eth_py-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 05:27:31.300453 quorum_eth_py-0.2.1/
--rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      834 2023-05-15 05:27:31.299454 quorum_eth_py-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 05:27:31.272526 quorum_eth_py-0.2.1/airdrop/
--rw-rw-rw-   0        0        0       43 2023-05-14 09:31:57.000000 quorum_eth_py-0.2.1/airdrop/__init__.py
--rw-rw-rw-   0        0        0     6623 2023-05-14 14:52:16.000000 quorum_eth_py-0.2.1/airdrop/airdrop_bot.py
--rw-rw-rw-   0        0        0     3267 2023-05-14 14:40:59.000000 quorum_eth_py-0.2.1/airdrop/db_handle.py
--rw-rw-rw-   0        0        0     1054 2023-05-14 14:31:09.000000 quorum_eth_py-0.2.1/airdrop/module.py
-drwxrwxrwx   0        0        0        0 2023-05-15 05:27:31.284494 quorum_eth_py-0.2.1/quorum_eth_py/
--rw-rw-rw-   0        0        0      307 2023-05-15 04:42:31.000000 quorum_eth_py-0.2.1/quorum_eth_py/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-04-28 13:04:41.000000 quorum_eth_py-0.2.1/quorum_eth_py/_browser.py
--rw-rw-rw-   0        0        0     7483 2023-05-15 04:43:57.000000 quorum_eth_py-0.2.1/quorum_eth_py/_eth.py
--rw-rw-rw-   0        0        0      470 2023-04-28 13:05:38.000000 quorum_eth_py-0.2.1/quorum_eth_py/_gateway.py
--rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.2.1/quorum_eth_py/_http.py
-drwxrwxrwx   0        0        0        0 2023-05-15 05:27:31.297460 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/
--rw-rw-rw-   0        0        0      834 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 05:27:31.300453 quorum_eth_py-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-05-15 04:42:31.000000 quorum_eth_py-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:11:24.649458 quorum_eth_py-0.2.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-05-15 07:11:24.647486 quorum_eth_py-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 07:11:24.632503 quorum_eth_py-0.2.2/quorum_eth_py/
+-rw-rw-rw-   0        0        0      445 2023-05-15 07:10:03.000000 quorum_eth_py-0.2.2/quorum_eth_py/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-04-28 13:04:41.000000 quorum_eth_py-0.2.2/quorum_eth_py/_browser.py
+-rw-rw-rw-   0        0        0     7484 2023-05-15 07:09:49.000000 quorum_eth_py-0.2.2/quorum_eth_py/_eth.py
+-rw-rw-rw-   0        0        0      470 2023-04-28 13:05:38.000000 quorum_eth_py-0.2.2/quorum_eth_py/_gateway.py
+-rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.2.2/quorum_eth_py/_http.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:11:24.645492 quorum_eth_py-0.2.2/quorum_eth_py/contract/
+-rw-rw-rw-   0        0        0    23212 2023-05-14 05:42:29.000000 quorum_eth_py-0.2.2/quorum_eth_py/contract/RumERC20.py
+-rw-rw-rw-   0        0        0      138 2023-05-15 07:09:49.000000 quorum_eth_py-0.2.2/quorum_eth_py/contract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:11:24.641490 quorum_eth_py-0.2.2/quorum_eth_py.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-05-15 07:11:24.000000 quorum_eth_py-0.2.2/quorum_eth_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-15 07:11:24.000000 quorum_eth_py-0.2.2/quorum_eth_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 07:11:24.000000 quorum_eth_py-0.2.2/quorum_eth_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 07:11:24.000000 quorum_eth_py-0.2.2/quorum_eth_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 07:11:24.000000 quorum_eth_py-0.2.2/quorum_eth_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 07:11:24.649458 quorum_eth_py-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2023-05-15 07:10:03.000000 quorum_eth_py-0.2.2/setup.py
```

### Comparing `quorum_eth_py-0.2.1/LICENSE` & `quorum_eth_py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.2.1/PKG-INFO` & `quorum_eth_py-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_eth_py
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.2.1/quorum_eth_py/_browser.py` & `quorum_eth_py-0.2.2/quorum_eth_py/_browser.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.2.1/quorum_eth_py/_eth.py` & `quorum_eth_py-0.2.2/quorum_eth_py/_eth.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         return msg, status
 
 
 class RumERC20Instance:
     """
     https://github.com/rumsystem/rum-eth-mvm/blob/main/dapps/RumERC20/contracts/RumERC20.sol
     """
+
     def __init__(
         self, contract_address, pvtkey=None, chain: RumEthChain = None, abi=None
     ):
         abi = abi or RumERC20_abi
         self.chain = chain or RumEthChain(pvtkey)
         self.w3 = self.chain.w3
         self.account = self.chain.account
```

### Comparing `quorum_eth_py-0.2.1/quorum_eth_py/_http.py` & `quorum_eth_py-0.2.2/quorum_eth_py/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.2.1/quorum_eth_py.egg-info/PKG-INFO` & `quorum_eth_py-0.2.2/quorum_eth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-eth-py
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.2.1/setup.py` & `quorum_eth_py-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_eth_py",
-    version="0.2.1",
+    version="0.2.2",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A python sdk for quorum-eth chain",
     keywords=["rumsystem", "quorum", "eth", "sdk", "blockchain"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_eth_py",
```

