# Comparing `tmp/quorum_eth_py-0.1.1.tar.gz` & `tmp/quorum_eth_py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_eth_py-0.1.1.tar", last modified: Fri Apr 28 08:33:35 2023, max compression
+gzip compressed data, was "quorum_eth_py-0.2.1.tar", last modified: Mon May 15 05:27:31 2023, max compression
```

## Comparing `quorum_eth_py-0.1.1.tar` & `quorum_eth_py-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 08:33:35.427015 quorum_eth_py-0.1.1/
--rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      834 2023-04-28 08:33:35.426040 quorum_eth_py-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 08:33:35.415070 quorum_eth_py-0.1.1/quorum_eth_py/
--rw-rw-rw-   0        0        0      310 2023-04-28 08:32:15.000000 quorum_eth_py-0.1.1/quorum_eth_py/__init__.py
--rw-rw-rw-   0        0        0     1783 2023-04-28 07:34:33.000000 quorum_eth_py-0.1.1/quorum_eth_py/_browser.py
--rw-rw-rw-   0        0        0     2703 2023-04-28 08:28:18.000000 quorum_eth_py-0.1.1/quorum_eth_py/_eth.py
--rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.1.1/quorum_eth_py/_http.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:33:35.424046 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/
--rw-rw-rw-   0        0        0      834 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 08:33:35.428012 quorum_eth_py-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-04-28 08:32:15.000000 quorum_eth_py-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:27:31.300453 quorum_eth_py-0.2.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-05-15 05:27:31.299454 quorum_eth_py-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 05:27:31.272526 quorum_eth_py-0.2.1/airdrop/
+-rw-rw-rw-   0        0        0       43 2023-05-14 09:31:57.000000 quorum_eth_py-0.2.1/airdrop/__init__.py
+-rw-rw-rw-   0        0        0     6623 2023-05-14 14:52:16.000000 quorum_eth_py-0.2.1/airdrop/airdrop_bot.py
+-rw-rw-rw-   0        0        0     3267 2023-05-14 14:40:59.000000 quorum_eth_py-0.2.1/airdrop/db_handle.py
+-rw-rw-rw-   0        0        0     1054 2023-05-14 14:31:09.000000 quorum_eth_py-0.2.1/airdrop/module.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:27:31.284494 quorum_eth_py-0.2.1/quorum_eth_py/
+-rw-rw-rw-   0        0        0      307 2023-05-15 04:42:31.000000 quorum_eth_py-0.2.1/quorum_eth_py/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-04-28 13:04:41.000000 quorum_eth_py-0.2.1/quorum_eth_py/_browser.py
+-rw-rw-rw-   0        0        0     7483 2023-05-15 04:43:57.000000 quorum_eth_py-0.2.1/quorum_eth_py/_eth.py
+-rw-rw-rw-   0        0        0      470 2023-04-28 13:05:38.000000 quorum_eth_py-0.2.1/quorum_eth_py/_gateway.py
+-rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.2.1/quorum_eth_py/_http.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:27:31.297460 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-15 05:27:31.000000 quorum_eth_py-0.2.1/quorum_eth_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 05:27:31.300453 quorum_eth_py-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2023-05-15 04:42:31.000000 quorum_eth_py-0.2.1/setup.py
```

### Comparing `quorum_eth_py-0.1.1/LICENSE` & `quorum_eth_py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.1.1/PKG-INFO` & `quorum_eth_py-0.2.1/quorum_eth_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: quorum_eth_py
-Version: 0.1.1
+Name: quorum-eth-py
+Version: 0.2.1
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.1.1/quorum_eth_py/_browser.py` & `quorum_eth_py-0.2.1/quorum_eth_py/_browser.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 class RumEthChainBrowser:
     """the browser of rum-eth chain"""
 
     def __init__(self, contract_address=None, api_base: str = BROWSER_API_BASE):
         self.contract_address = contract_address
         self.http = HttpRequest(api_base)
-        self.api_base = api_base or BROWSER_API_BASE
         self.w3 = Web3()
 
     def _get_contract(self, action, contract_address=None):
         contract_address = contract_address or self.contract_address
         data = self.http.get(
             f"?module=token&action={action}&contractaddress={contract_address}"
         )
```

### Comparing `quorum_eth_py-0.1.1/quorum_eth_py/_http.py` & `quorum_eth_py-0.2.1/quorum_eth_py/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.1.1/quorum_eth_py.egg-info/PKG-INFO` & `quorum_eth_py-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: quorum-eth-py
-Version: 0.1.1
+Name: quorum_eth_py
+Version: 0.2.1
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.1.1/setup.py` & `quorum_eth_py-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_eth_py",
-    version="0.1.1",
+    version="0.2.1",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A python sdk for quorum-eth chain",
     keywords=["rumsystem", "quorum", "eth", "sdk", "blockchain"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_eth_py",
```

