# Comparing `tmp/eth-address-index-0.7.2.tar.gz` & `tmp/eth-address-index-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-address-index-0.7.2.tar", last modified: Sun Mar 26 07:19:37 2023, max compression
+gzip compressed data, was "eth-address-index-0.7.3.tar", last modified: Mon May 15 14:04:24 2023, max compression
```

## Comparing `eth-address-index-0.7.2.tar` & `eth-address-index-0.7.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:19:37.639990 eth-address-index-0.7.2/
--rw-r--r--   0 lash      (1000) lash      (1000)       55 2021-08-24 19:43:26.000000 eth-address-index-0.7.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      713 2023-03-26 07:19:37.639990 eth-address-index-0.7.2/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:19:37.639990 eth-address-index-0.7.2/eth_address_declarator/
--rw-r--r--   0 lash      (1000) lash      (1000)       34 2023-03-23 12:34:17.000000 eth-address-index-0.7.2/eth_address_declarator/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:19:37.639990 eth-address-index-0.7.2/eth_address_declarator/data/
--rw-r--r--   0 lash      (1000) lash      (1000)    16494 2023-03-26 07:19:24.000000 eth-address-index-0.7.2/eth_address_declarator/data/AddressDeclarator.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     2880 2023-03-26 07:19:24.000000 eth-address-index-0.7.2/eth_address_declarator/data/AddressDeclarator.json
--rw-r--r--   0 lash      (1000) lash      (1000)     3587 2023-03-26 07:19:24.000000 eth-address-index-0.7.2/eth_address_declarator/data/AddressDeclarator.metadata.json
--rw-r--r--   0 lash      (1000) lash      (1000)     2069 2023-03-24 10:40:22.000000 eth-address-index-0.7.2/eth_address_declarator/declarator.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5325 2023-03-24 10:40:22.000000 eth-address-index-0.7.2/eth_address_declarator/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:19:37.639990 eth-address-index-0.7.2/eth_address_declarator/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2894 2023-02-12 08:14:47.000000 eth-address-index-0.7.2/eth_address_declarator/runnable/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3085 2023-02-12 08:14:47.000000 eth-address-index-0.7.2/eth_address_declarator/runnable/publish.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2899 2023-02-25 20:12:23.000000 eth-address-index-0.7.2/eth_address_declarator/runnable/view.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:19:37.639990 eth-address-index-0.7.2/eth_address_declarator/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       33 2021-10-04 10:02:49.000000 eth-address-index-0.7.2/eth_address_declarator/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1625 2023-03-24 10:40:22.000000 eth-address-index-0.7.2/eth_address_declarator/unittest/addressdeclarator.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:19:37.639990 eth-address-index-0.7.2/eth_address_index.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      713 2023-03-26 07:19:37.000000 eth-address-index-0.7.2/eth_address_index.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      837 2023-03-26 07:19:37.000000 eth-address-index-0.7.2/eth_address_index.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-26 07:19:37.000000 eth-address-index-0.7.2/eth_address_index.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      238 2023-03-26 07:19:37.000000 eth-address-index-0.7.2/eth_address_index.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      140 2023-03-26 07:19:37.000000 eth-address-index-0.7.2/eth_address_index.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       23 2023-03-26 07:19:37.000000 eth-address-index-0.7.2/eth_address_index.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       53 2023-02-25 20:24:41.000000 eth-address-index-0.7.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1194 2023-03-26 07:19:37.639990 eth-address-index-0.7.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      545 2021-10-24 13:34:28.000000 eth-address-index-0.7.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       80 2023-02-12 08:14:47.000000 eth-address-index-0.7.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:19:37.639990 eth-address-index-0.7.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     9816 2023-03-26 07:19:24.000000 eth-address-index-0.7.2/tests/test_addressdeclarator.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:04:24.229990 eth-address-index-0.7.3/
+-rw-r--r--   0 lash      (1000) lash      (1000)       55 2021-08-24 19:43:26.000000 eth-address-index-0.7.3/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      713 2023-05-15 14:04:24.229990 eth-address-index-0.7.3/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:04:24.226657 eth-address-index-0.7.3/eth_address_declarator/
+-rw-r--r--   0 lash      (1000) lash      (1000)       34 2023-03-23 12:34:17.000000 eth-address-index-0.7.3/eth_address_declarator/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:04:24.226657 eth-address-index-0.7.3/eth_address_declarator/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)    16494 2023-03-26 07:19:24.000000 eth-address-index-0.7.3/eth_address_declarator/data/AddressDeclarator.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     2880 2023-03-26 07:19:24.000000 eth-address-index-0.7.3/eth_address_declarator/data/AddressDeclarator.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     3587 2023-03-26 07:19:24.000000 eth-address-index-0.7.3/eth_address_declarator/data/AddressDeclarator.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     2069 2023-03-24 10:40:22.000000 eth-address-index-0.7.3/eth_address_declarator/declarator.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5325 2023-03-24 10:40:22.000000 eth-address-index-0.7.3/eth_address_declarator/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:04:24.229990 eth-address-index-0.7.3/eth_address_declarator/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2894 2023-02-12 08:14:47.000000 eth-address-index-0.7.3/eth_address_declarator/runnable/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3085 2023-02-12 08:14:47.000000 eth-address-index-0.7.3/eth_address_declarator/runnable/publish.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2899 2023-02-25 20:12:23.000000 eth-address-index-0.7.3/eth_address_declarator/runnable/view.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:04:24.229990 eth-address-index-0.7.3/eth_address_declarator/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       33 2021-10-04 10:02:49.000000 eth-address-index-0.7.3/eth_address_declarator/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1625 2023-03-24 10:40:22.000000 eth-address-index-0.7.3/eth_address_declarator/unittest/addressdeclarator.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:04:24.229990 eth-address-index-0.7.3/eth_address_index.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      713 2023-05-15 14:04:24.000000 eth-address-index-0.7.3/eth_address_index.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      872 2023-05-15 14:04:24.000000 eth-address-index-0.7.3/eth_address_index.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-15 14:04:24.000000 eth-address-index-0.7.3/eth_address_index.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      238 2023-05-15 14:04:24.000000 eth-address-index-0.7.3/eth_address_index.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      140 2023-05-15 14:04:24.000000 eth-address-index-0.7.3/eth_address_index.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       23 2023-05-15 14:04:24.000000 eth-address-index-0.7.3/eth_address_index.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       53 2023-05-15 14:04:00.000000 eth-address-index-0.7.3/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1194 2023-05-15 14:04:24.229990 eth-address-index-0.7.3/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      545 2021-10-24 13:34:28.000000 eth-address-index-0.7.3/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       80 2023-02-12 08:14:47.000000 eth-address-index-0.7.3/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-15 14:04:24.229990 eth-address-index-0.7.3/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     9816 2023-03-26 07:19:24.000000 eth-address-index-0.7.3/tests/test_addressdeclarator.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    11196 2023-03-24 10:40:22.000000 eth-address-index-0.7.3/tests/test_addressdeclarator_kv.py
```

### Comparing `eth-address-index-0.7.2/PKG-INFO` & `eth-address-index-0.7.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-address-index
-Version: 0.7.2
+Version: 0.7.3
 Summary: Signed metadata declarations for ethereum addresses
 Home-page: https://holbrook.no/src/eth-address-index/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-address-index-0.7.2/eth_address_declarator/data/AddressDeclarator.bin` & `eth-address-index-0.7.3/eth_address_declarator/data/AddressDeclarator.bin`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/eth_address_declarator/data/AddressDeclarator.json` & `eth-address-index-0.7.3/eth_address_declarator/data/AddressDeclarator.json`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/eth_address_declarator/data/AddressDeclarator.metadata.json` & `eth-address-index-0.7.3/eth_address_declarator/data/AddressDeclarator.metadata.json`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/eth_address_declarator/declarator.py` & `eth-address-index-0.7.3/eth_address_declarator/declarator.py`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/eth_address_declarator/interface.py` & `eth-address-index-0.7.3/eth_address_declarator/interface.py`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/eth_address_declarator/runnable/add.py` & `eth-address-index-0.7.3/eth_address_declarator/runnable/add.py`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/eth_address_declarator/runnable/publish.py` & `eth-address-index-0.7.3/eth_address_declarator/runnable/publish.py`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/eth_address_declarator/runnable/view.py` & `eth-address-index-0.7.3/eth_address_declarator/runnable/view.py`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/eth_address_declarator/unittest/addressdeclarator.py` & `eth-address-index-0.7.3/eth_address_declarator/unittest/addressdeclarator.py`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/eth_address_index.egg-info/PKG-INFO` & `eth-address-index-0.7.3/eth_address_index.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-address-index
-Version: 0.7.2
+Version: 0.7.3
 Summary: Signed metadata declarations for ethereum addresses
 Home-page: https://holbrook.no/src/eth-address-index/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-address-index-0.7.2/eth_address_index.egg-info/SOURCES.txt` & `eth-address-index-0.7.3/eth_address_index.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 eth_address_declarator/unittest/addressdeclarator.py
 eth_address_index.egg-info/PKG-INFO
 eth_address_index.egg-info/SOURCES.txt
 eth_address_index.egg-info/dependency_links.txt
 eth_address_index.egg-info/entry_points.txt
 eth_address_index.egg-info/requires.txt
 eth_address_index.egg-info/top_level.txt
-tests/test_addressdeclarator.py
+tests/test_addressdeclarator.py
+tests/test_addressdeclarator_kv.py
```

### Comparing `eth-address-index-0.7.2/setup.cfg` & `eth-address-index-0.7.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-address-index
-version = 0.7.2
+version = 0.7.3
 description = Signed metadata declarations for ethereum addresses
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/eth-address-index/log.html
 keywords = 
 	ethereum
 classifiers =
```

### Comparing `eth-address-index-0.7.2/setup.py` & `eth-address-index-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `eth-address-index-0.7.2/tests/test_addressdeclarator.py` & `eth-address-index-0.7.3/tests/test_addressdeclarator.py`

 * *Files identical despite different names*

