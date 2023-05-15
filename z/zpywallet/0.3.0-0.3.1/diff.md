# Comparing `tmp/zpywallet-0.3.0.tar.gz` & `tmp/zpywallet-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpywallet-0.3.0.tar", last modified: Sun May 14 16:58:21 2023, max compression
+gzip compressed data, was "zpywallet-0.3.1.tar", last modified: Mon May 15 10:19:31 2023, max compression
```

## Comparing `zpywallet-0.3.0.tar` & `zpywallet-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:58:21.690115 zpywallet-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-14 16:58:10.000000 zpywallet-0.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-14 16:58:10.000000 zpywallet-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 16:58:10.000000 zpywallet-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-14 16:58:21.690115 zpywallet-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-14 16:58:10.000000 zpywallet-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-14 16:58:21.690115 zpywallet-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-14 16:58:10.000000 zpywallet-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:58:21.686115 zpywallet-0.3.0/zpywallet/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:58:21.690115 zpywallet-0.3.0/zpywallet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28188 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/bip32.py
--rw-r--r--   0 runner    (1001) docker     (123)    31084 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    63187 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:58:21.686115 zpywallet-0.3.0/zpywallet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:19:31.172811 zpywallet-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-15 10:19:18.000000 zpywallet-0.3.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-15 10:19:18.000000 zpywallet-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 10:19:18.000000 zpywallet-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-15 10:19:31.172811 zpywallet-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-15 10:19:18.000000 zpywallet-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 10:19:31.172811 zpywallet-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-15 10:19:18.000000 zpywallet-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:19:31.168811 zpywallet-0.3.1/zpywallet/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:19:31.172811 zpywallet-0.3.1/zpywallet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28188 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/bip32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31084 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63187 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:19:31.168811 zpywallet-0.3.1/zpywallet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/top_level.txt
```

### Comparing `zpywallet-0.3.0/LICENSE` & `zpywallet-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.0/PKG-INFO` & `zpywallet-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpywallet
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simple BIP32 (HD) wallet creation for BTC, BTX, RVN, MXT, BTG, BCH, LTC, DASH, USDT, QTUM and DOGE
 Home-page: https://github.com/ZenulAbidin/pywallet
 Author: Ali Sherief
 Author-email: ali@notatether.com
 License: MIT License
 Keywords: bitcoin,wallet,litecoin,hd-wallet,dogecoin,dashcoin,bitcore,qtum,ravencoin,martexcoin,address,crypto,python
 Platform: any
```

### Comparing `zpywallet-0.3.0/README.rst` & `zpywallet-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.0/setup.py` & `zpywallet-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.0/zpywallet/network.py` & `zpywallet-0.3.1/zpywallet/network.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.0/zpywallet/utils/bip32.py` & `zpywallet-0.3.1/zpywallet/utils/bip32.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.0/zpywallet/utils/ecdsa.py` & `zpywallet-0.3.1/zpywallet/utils/ecdsa.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.0/zpywallet/utils/keys.py` & `zpywallet-0.3.1/zpywallet/utils/keys.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.0/zpywallet/utils/ripemd160.py` & `zpywallet-0.3.1/zpywallet/utils/ripemd160.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.0/zpywallet/utils/utils.py` & `zpywallet-0.3.1/zpywallet/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.0/zpywallet.egg-info/PKG-INFO` & `zpywallet-0.3.1/zpywallet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpywallet
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simple BIP32 (HD) wallet creation for BTC, BTX, RVN, MXT, BTG, BCH, LTC, DASH, USDT, QTUM and DOGE
 Home-page: https://github.com/ZenulAbidin/pywallet
 Author: Ali Sherief
 Author-email: ali@notatether.com
 License: MIT License
 Keywords: bitcoin,wallet,litecoin,hd-wallet,dogecoin,dashcoin,bitcore,qtum,ravencoin,martexcoin,address,crypto,python
 Platform: any
```

