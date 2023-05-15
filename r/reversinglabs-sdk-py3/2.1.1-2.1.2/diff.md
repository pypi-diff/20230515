# Comparing `tmp/reversinglabs-sdk-py3-2.1.1.tar.gz` & `tmp/reversinglabs-sdk-py3-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reversinglabs-sdk-py3-2.1.1.tar", last modified: Wed Apr  5 12:47:33 2023, max compression
+gzip compressed data, was "reversinglabs-sdk-py3-2.1.2.tar", last modified: Mon May 15 12:49:20 2023, max compression
```

## Comparing `reversinglabs-sdk-py3-2.1.1.tar` & `reversinglabs-sdk-py3-2.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-04-05 12:47:33.041742 reversinglabs-sdk-py3-2.1.1/
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     5573 2023-04-04 23:44:46.000000 reversinglabs-sdk-py3-2.1.1/CHANGELOG.md
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     1056 2023-01-01 19:35:25.000000 reversinglabs-sdk-py3-2.1.1/LICENSE
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       53 2022-10-18 22:24:54.000000 reversinglabs-sdk-py3-2.1.1/MANIFEST.in
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    36594 2023-04-05 12:47:33.042742 reversinglabs-sdk-py3-2.1.1/PKG-INFO
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    35342 2023-04-05 12:43:55.000000 reversinglabs-sdk-py3-2.1.1/README.md
-drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-04-05 12:47:33.039742 reversinglabs-sdk-py3-2.1.1/ReversingLabs/
-drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-04-05 12:47:33.041742 reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/__init__.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)   103704 2023-03-30 16:30:46.000000 reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/a1000.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    19593 2023-02-27 14:28:49.000000 reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/clouddeepscan.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     4776 2023-03-30 13:23:32.000000 reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/helper.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)   171456 2023-04-05 12:27:16.000000 reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/ticloud.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    16840 2023-03-31 17:23:41.000000 reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/tiscale.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.1.1/ReversingLabs/__init__.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    41623 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.1.1/logo.jpg
-drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-04-05 12:47:33.041742 reversinglabs-sdk-py3-2.1.1/reversinglabs_sdk_py3.egg-info/
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    36594 2023-04-05 12:47:32.000000 reversinglabs-sdk-py3-2.1.1/reversinglabs_sdk_py3.egg-info/PKG-INFO
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)      542 2023-04-05 12:47:33.000000 reversinglabs-sdk-py3-2.1.1/reversinglabs_sdk_py3.egg-info/SOURCES.txt
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        1 2023-04-05 12:47:32.000000 reversinglabs-sdk-py3-2.1.1/reversinglabs_sdk_py3.egg-info/dependency_links.txt
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        1 2023-04-05 12:47:32.000000 reversinglabs-sdk-py3-2.1.1/reversinglabs_sdk_py3.egg-info/not-zip-safe
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       34 2023-04-05 12:47:32.000000 reversinglabs-sdk-py3-2.1.1/reversinglabs_sdk_py3.egg-info/requires.txt
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       14 2023-04-05 12:47:32.000000 reversinglabs-sdk-py3-2.1.1/reversinglabs_sdk_py3.egg-info/top_level.txt
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       74 2023-04-05 12:47:33.042742 reversinglabs-sdk-py3-2.1.1/setup.cfg
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     1645 2023-04-03 15:10:58.000000 reversinglabs-sdk-py3-2.1.1/setup.py
+drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-05-15 12:49:20.209660 reversinglabs-sdk-py3-2.1.2/
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     5969 2023-05-15 12:14:56.000000 reversinglabs-sdk-py3-2.1.2/CHANGELOG.md
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     1056 2023-01-01 19:35:25.000000 reversinglabs-sdk-py3-2.1.2/LICENSE
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       53 2022-10-18 22:24:54.000000 reversinglabs-sdk-py3-2.1.2/MANIFEST.in
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    37303 2023-05-15 12:49:20.210660 reversinglabs-sdk-py3-2.1.2/PKG-INFO
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    36051 2023-05-15 12:44:26.000000 reversinglabs-sdk-py3-2.1.2/README.md
+drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-05-15 12:49:20.207660 reversinglabs-sdk-py3-2.1.2/ReversingLabs/
+drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-05-15 12:49:20.209660 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/__init__.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)   110651 2023-05-15 12:44:26.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/a1000.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    19593 2023-02-27 14:28:49.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/clouddeepscan.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     4776 2023-03-30 13:23:32.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/helper.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)   171456 2023-04-05 12:27:16.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/ticloud.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    16840 2023-04-05 21:30:12.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/tiscale.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/__init__.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    41623 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.1.2/logo.jpg
+drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-05-15 12:49:20.209660 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    37303 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/PKG-INFO
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)      542 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        1 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        1 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/not-zip-safe
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       34 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/requires.txt
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       14 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/top_level.txt
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       74 2023-05-15 12:49:20.210660 reversinglabs-sdk-py3-2.1.2/setup.cfg
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     1645 2023-05-15 12:00:53.000000 reversinglabs-sdk-py3-2.1.2/setup.py
```

### Comparing `reversinglabs-sdk-py3-2.1.1/CHANGELOG.md` & `reversinglabs-sdk-py3-2.1.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -99,12 +99,26 @@
 
 - **ticloud** module:
   - Added the `FileAnalysisNonMalicious` and `DataChangeSubscription` classes.
   - The `FileUpload` class methods now also use `subscribe`, `archive_type` and `archive_passoword` parameters.
 
 ---
 
+
+
+v2.1.2 (2023-05-15)
+-------------------
+
+#### Improvements
+
+- **a1000** module:
+  - Added paging parameters to the Network Threat Intelligence methods: `network_ip_to_domain`, `network_urls_from_ip` and `network_files_from_ip`
+  - Added auto paging versions of the same methods: `network_ip_to_domain_aggregated`, `network_urls_from_ip_aggregated` and `network_files_from_ip_aggregated`
+
+---
+
+
 ### Scheduled removals
 - **June 2023.**:
   - `a1000.A1000.get_results`, `a1000.A1000.upload_sample_and_get_results`, `a1000.A1000.get_classification`, `a1000.A1000.reanalyze_samples`, `a1000.A1000.get_extracted_files`, `a1000.A1000.advanced_search`, `a1000.A1000.advanced_search_aggregated`
 - **September 2023.**:
   - `ticloud.ReanalyzeFile.ranalyze_samples`
```

### Comparing `reversinglabs-sdk-py3-2.1.1/LICENSE` & `reversinglabs-sdk-py3-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.1/PKG-INFO` & `reversinglabs-sdk-py3-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python SDK for using ReversingLabs services - Python 3 version.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -170,15 +170,15 @@
 - `create_or_update_yara_ruleset`
   - Creates a new YARA ruleset if it doesn’t exist
   - If a ruleset with the specified name already exists, a new revision (update) of the ruleset is created
 - `delete_yara_ruleset`
   - Deletes the specified YARA ruleset and its matches from the appliance
 - `enable_or_disable_yara_ruleset`
   - Enables/disables ruleset on the appliance
-  - Administrators can manage any ruleset while regular A1000 users can only menage their own rulesets
+  - Administrators can manage any ruleset while regular A1000 users can only manage their own rulesets
 - `get_yara_ruleset_synchronization_time`
   - Gets information about the current synchronization status for TitaniumCloud-enabled rulesets
 - `update_yara_ruleset_synchronization_time`
   - Updates the TitaniumCloud synchronization time for TitaniumCloud-enabled YARA rulesets
 - `start_or_stop_yara_local_retro_scan`
   - Allows users to initiate the Local Retro scan on the A1000 appliance, and stop the Local Retro scan that is
         in progress on the appliance
@@ -204,18 +204,27 @@
   - Accepts a URL string and returns a report about the requested URL
 - `network_domain_report`
   - Accepts a domain string and returns a report about the requested domain
 - `network_ip_addr_report`
   - Accepts an IP address string and returns a report about the requested IP address
 - `network_ip_to_domain`
   - Accepts an IP address string and returns a list of IP-to-domain mappings
+- `network_ip_to_domain_aggregated`
+  - Accepts an IP address string and returns a list of IP-to-domain mappings. 
+  - This method performs the paging automatically and returns a specified maximum number of records
 - `network_urls_from_ip`
   - Accepts an IP address string and returns a list of URLs hosted on the requested IP address
+- `network_urls_from_ip_aggregated`
+  - Accepts an IP address string and returns a list of URLs hosted on the requested IP address
+  - This method performs the paging automatically and returns a specified maximum number of records
 - `network_files_from_ip`
   - Accepts an IP address string and returns a list of hashes and classifications for files found on the requested IP address
+- `network_files_from_ip_aggregated`
+  - Accepts an IP address string and returns a list of hashes and classifications for files found on the requested IP address
+  - This method performs the paging automatically and returns a specified maximum number of records
 
 ***
 
 
 ## Module: ticloud
 A Python module representing the ReversingLabs TitaniumCloud API-s.
```

### Comparing `reversinglabs-sdk-py3-2.1.1/README.md` & `reversinglabs-sdk-py3-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 - `create_or_update_yara_ruleset`
   - Creates a new YARA ruleset if it doesn’t exist
   - If a ruleset with the specified name already exists, a new revision (update) of the ruleset is created
 - `delete_yara_ruleset`
   - Deletes the specified YARA ruleset and its matches from the appliance
 - `enable_or_disable_yara_ruleset`
   - Enables/disables ruleset on the appliance
-  - Administrators can manage any ruleset while regular A1000 users can only menage their own rulesets
+  - Administrators can manage any ruleset while regular A1000 users can only manage their own rulesets
 - `get_yara_ruleset_synchronization_time`
   - Gets information about the current synchronization status for TitaniumCloud-enabled rulesets
 - `update_yara_ruleset_synchronization_time`
   - Updates the TitaniumCloud synchronization time for TitaniumCloud-enabled YARA rulesets
 - `start_or_stop_yara_local_retro_scan`
   - Allows users to initiate the Local Retro scan on the A1000 appliance, and stop the Local Retro scan that is
         in progress on the appliance
@@ -176,18 +176,27 @@
   - Accepts a URL string and returns a report about the requested URL
 - `network_domain_report`
   - Accepts a domain string and returns a report about the requested domain
 - `network_ip_addr_report`
   - Accepts an IP address string and returns a report about the requested IP address
 - `network_ip_to_domain`
   - Accepts an IP address string and returns a list of IP-to-domain mappings
+- `network_ip_to_domain_aggregated`
+  - Accepts an IP address string and returns a list of IP-to-domain mappings. 
+  - This method performs the paging automatically and returns a specified maximum number of records
 - `network_urls_from_ip`
   - Accepts an IP address string and returns a list of URLs hosted on the requested IP address
+- `network_urls_from_ip_aggregated`
+  - Accepts an IP address string and returns a list of URLs hosted on the requested IP address
+  - This method performs the paging automatically and returns a specified maximum number of records
 - `network_files_from_ip`
   - Accepts an IP address string and returns a list of hashes and classifications for files found on the requested IP address
+- `network_files_from_ip_aggregated`
+  - Accepts an IP address string and returns a list of hashes and classifications for files found on the requested IP address
+  - This method performs the paging automatically and returns a specified maximum number of records
 
 ***
 
 
 ## Module: ticloud
 A Python module representing the ReversingLabs TitaniumCloud API-s.
```

### Comparing `reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/a1000.py` & `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/a1000.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,6464 +19,6898 @@
 00000120: 5245 5350 4f4e 5345 5f43 4f44 455f 4552  RESPONSE_CODE_ER
 00000130: 524f 525f 4d41 502c 205c 0a20 2020 204d  ROR_MAP, \.    M
 00000140: 4435 2c20 5348 4131 2c20 5348 4132 3536  D5, SHA1, SHA256
 00000150: 2c20 5348 4135 3132 2c20 5c0a 2020 2020  , SHA512, \.    
 00000160: 5265 7175 6573 7454 696d 656f 7574 4572  RequestTimeoutEr
 00000170: 726f 722c 2057 726f 6e67 496e 7075 7445  ror, WrongInputE
 00000180: 7272 6f72 2c20 5c0a 2020 2020 7661 6c69  rror, \.    vali
-00000190: 6461 7465 5f68 6173 6865 730a 0a0a 4156  date_hashes...AV
-000001a0: 4149 4c41 424c 455f 504c 4154 464f 524d  AILABLE_PLATFORM
-000001b0: 5320 3d20 2822 7769 6e64 6f77 7337 222c  S = ("windows7",
-000001c0: 2022 7769 6e64 6f77 7331 3022 2c20 226d   "windows10", "m
-000001d0: 6163 6f73 5f31 3122 290a 0a0a 636c 6173  acos_11")...clas
-000001e0: 7320 4131 3030 3028 6f62 6a65 6374 293a  s A1000(object):
-000001f0: 0a0a 2020 2020 5f5f 544f 4b45 4e5f 454e  ..    __TOKEN_EN
-00000200: 4450 4f49 4e54 203d 2022 2f61 7069 2d74  DPOINT = "/api-t
-00000210: 6f6b 656e 2d61 7574 682f 220a 2020 2020  oken-auth/".    
-00000220: 5f5f 5550 4c4f 4144 5f45 4e44 504f 494e  __UPLOAD_ENDPOIN
-00000230: 5420 3d20 222f 6170 692f 7570 6c6f 6164  T = "/api/upload
-00000240: 732f 220a 2020 2020 5f5f 4348 4543 4b5f  s/".    __CHECK_
-00000250: 5354 4154 5553 5f45 4e44 504f 494e 5420  STATUS_ENDPOINT 
-00000260: 3d20 222f 6170 692f 7361 6d70 6c65 732f  = "/api/samples/
-00000270: 7374 6174 7573 2f22 0a20 2020 205f 5f43  status/".    __C
-00000280: 4845 434b 5f55 524c 5f53 5441 5455 535f  HECK_URL_STATUS_
-00000290: 454e 4450 4f49 4e54 203d 2022 2f61 7069  ENDPOINT = "/api
-000002a0: 2f75 706c 6f61 6473 2f76 322f 7572 6c2d  /uploads/v2/url-
-000002b0: 7361 6d70 6c65 732f 7b74 6173 6b5f 6964  samples/{task_id
-000002c0: 7d22 0a20 2020 205f 5f52 4553 554c 5453  }".    __RESULTS
-000002d0: 5f45 4e44 504f 494e 5420 3d20 222f 6170  _ENDPOINT = "/ap
-000002e0: 692f 7361 6d70 6c65 732f 6c69 7374 2f22  i/samples/list/"
-000002f0: 0a20 2020 205f 5f53 554d 4d41 5259 5f52  .    __SUMMARY_R
-00000300: 4550 4f52 545f 454e 4450 4f49 4e54 5f56  EPORT_ENDPOINT_V
-00000310: 3220 3d20 222f 6170 692f 7361 6d70 6c65  2 = "/api/sample
-00000320: 732f 7632 2f6c 6973 742f 220a 2020 2020  s/v2/list/".    
-00000330: 5f5f 4445 5441 494c 4544 5f52 4550 4f52  __DETAILED_REPOR
-00000340: 545f 454e 4450 4f49 4e54 5f56 3220 3d20  T_ENDPOINT_V2 = 
-00000350: 222f 6170 692f 7361 6d70 6c65 732f 7632  "/api/samples/v2
-00000360: 2f6c 6973 742f 6465 7461 696c 732f 220a  /list/details/".
-00000370: 2020 2020 5f5f 434c 4153 5349 4659 5f45      __CLASSIFY_E
-00000380: 4e44 504f 494e 545f 5632 203d 2022 2f61  NDPOINT_V2 = "/a
-00000390: 7069 2f76 322f 7361 6d70 6c65 732f 7b68  pi/v2/samples/{h
-000003a0: 6173 685f 7661 6c75 657d 2f63 6c61 7373  ash_value}/class
-000003b0: 6966 6963 6174 696f 6e2f 3f6c 6f63 616c  ification/?local
-000003c0: 6f6e 6c79 3d7b 6c6f 6361 6c6f 6e6c 797d  only={localonly}
-000003d0: 220a 2020 2020 5f5f 434c 4153 5349 4659  ".    __CLASSIFY
-000003e0: 5f45 4e44 504f 494e 545f 5633 203d 2022  _ENDPOINT_V3 = "
-000003f0: 2f61 7069 2f73 616d 706c 6573 2f76 332f  /api/samples/v3/
-00000400: 7b68 6173 685f 7661 6c75 657d 2f63 6c61  {hash_value}/cla
-00000410: 7373 6966 6963 6174 696f 6e2f 220a 2020  ssification/".  
-00000420: 2020 5f5f 5245 414e 414c 595a 455f 454e    __REANALYZE_EN
-00000430: 4450 4f49 4e54 203d 2022 2f61 7069 2f73  DPOINT = "/api/s
-00000440: 616d 706c 6573 2f7b 6861 7368 5f76 616c  amples/{hash_val
-00000450: 7565 7d2f 616e 616c 797a 652f 220a 2020  ue}/analyze/".  
-00000460: 2020 5f5f 5245 414e 414c 595a 455f 4255    __REANALYZE_BU
-00000470: 4c4b 5f45 4e44 504f 494e 5420 3d20 222f  LK_ENDPOINT = "/
-00000480: 6170 692f 7361 6d70 6c65 732f 616e 616c  api/samples/anal
-00000490: 797a 655f 6275 6c6b 2f22 0a20 2020 205f  yze_bulk/".    _
-000004a0: 5f52 4541 4e41 4c59 5a45 5f42 554c 4b5f  _REANALYZE_BULK_
-000004b0: 454e 4450 4f49 4e54 5f56 3220 3d20 222f  ENDPOINT_V2 = "/
-000004c0: 6170 692f 7361 6d70 6c65 732f 7632 2f61  api/samples/v2/a
-000004d0: 6e61 6c79 7a65 5f62 756c 6b2f 220a 2020  nalyze_bulk/".  
-000004e0: 2020 5f5f 4c49 5354 5f45 5854 5241 4354    __LIST_EXTRACT
-000004f0: 4544 5f46 494c 4553 5f45 4e44 504f 494e  ED_FILES_ENDPOIN
-00000500: 5420 3d20 222f 6170 692f 7361 6d70 6c65  T = "/api/sample
-00000510: 732f 7b68 6173 685f 7661 6c75 657d 2f65  s/{hash_value}/e
-00000520: 7874 7261 6374 6564 2d66 696c 6573 2f22  xtracted-files/"
-00000530: 0a20 2020 205f 5f4c 4953 545f 4558 5452  .    __LIST_EXTR
-00000540: 4143 5445 445f 4649 4c45 535f 454e 4450  ACTED_FILES_ENDP
-00000550: 4f49 4e54 5f56 3220 3d20 222f 6170 692f  OINT_V2 = "/api/
-00000560: 7361 6d70 6c65 732f 7632 2f7b 6861 7368  samples/v2/{hash
-00000570: 5f76 616c 7565 7d2f 6578 7472 6163 7465  _value}/extracte
-00000580: 642d 6669 6c65 732f 220a 2020 2020 5f5f  d-files/".    __
-00000590: 444f 574e 4c4f 4144 5f45 5854 5241 4354  DOWNLOAD_EXTRACT
-000005a0: 4544 5f46 494c 4553 5f45 4e44 504f 494e  ED_FILES_ENDPOIN
-000005b0: 5420 3d20 222f 6170 692f 7361 6d70 6c65  T = "/api/sample
-000005c0: 732f 7b68 6173 685f 7661 6c75 657d 2f75  s/{hash_value}/u
-000005d0: 6e70 6163 6b65 642f 220a 2020 2020 5f5f  npacked/".    __
-000005e0: 444f 574e 4c4f 4144 5f53 414d 504c 455f  DOWNLOAD_SAMPLE_
-000005f0: 454e 4450 4f49 4e54 203d 2022 2f61 7069  ENDPOINT = "/api
-00000600: 2f73 616d 706c 6573 2f7b 6861 7368 5f76  /samples/{hash_v
-00000610: 616c 7565 7d2f 646f 776e 6c6f 6164 2f22  alue}/download/"
-00000620: 0a20 2020 205f 5f44 454c 4554 455f 5341  .    __DELETE_SA
+00000190: 6461 7465 5f68 6173 6865 730a 0a0a 434c  date_hashes...CL
+000001a0: 4153 5349 4649 4341 5449 4f4e 5320 3d20  ASSIFICATIONS = 
+000001b0: 2822 4d41 4c49 4349 4f55 5322 2c20 2253  ("MALICIOUS", "S
+000001c0: 5553 5049 4349 4f55 5322 2c20 2247 4f4f  USPICIOUS", "GOO
+000001d0: 4457 4152 4522 2c20 2255 4e4b 4e4f 574e  DWARE", "UNKNOWN
+000001e0: 2229 0a41 5641 494c 4142 4c45 5f50 4c41  ").AVAILABLE_PLA
+000001f0: 5446 4f52 4d53 203d 2028 2277 696e 646f  TFORMS = ("windo
+00000200: 7773 3722 2c20 2277 696e 646f 7773 3130  ws7", "windows10
+00000210: 222c 2022 6d61 636f 735f 3131 2229 0a0a  ", "macos_11")..
+00000220: 0a63 6c61 7373 2041 3130 3030 286f 626a  .class A1000(obj
+00000230: 6563 7429 3a0a 0a20 2020 205f 5f54 4f4b  ect):..    __TOK
+00000240: 454e 5f45 4e44 504f 494e 5420 3d20 222f  EN_ENDPOINT = "/
+00000250: 6170 692d 746f 6b65 6e2d 6175 7468 2f22  api-token-auth/"
+00000260: 0a20 2020 205f 5f55 504c 4f41 445f 454e  .    __UPLOAD_EN
+00000270: 4450 4f49 4e54 203d 2022 2f61 7069 2f75  DPOINT = "/api/u
+00000280: 706c 6f61 6473 2f22 0a20 2020 205f 5f43  ploads/".    __C
+00000290: 4845 434b 5f53 5441 5455 535f 454e 4450  HECK_STATUS_ENDP
+000002a0: 4f49 4e54 203d 2022 2f61 7069 2f73 616d  OINT = "/api/sam
+000002b0: 706c 6573 2f73 7461 7475 732f 220a 2020  ples/status/".  
+000002c0: 2020 5f5f 4348 4543 4b5f 5552 4c5f 5354    __CHECK_URL_ST
+000002d0: 4154 5553 5f45 4e44 504f 494e 5420 3d20  ATUS_ENDPOINT = 
+000002e0: 222f 6170 692f 7570 6c6f 6164 732f 7632  "/api/uploads/v2
+000002f0: 2f75 726c 2d73 616d 706c 6573 2f7b 7461  /url-samples/{ta
+00000300: 736b 5f69 647d 220a 2020 2020 5f5f 5245  sk_id}".    __RE
+00000310: 5355 4c54 535f 454e 4450 4f49 4e54 203d  SULTS_ENDPOINT =
+00000320: 2022 2f61 7069 2f73 616d 706c 6573 2f6c   "/api/samples/l
+00000330: 6973 742f 220a 2020 2020 5f5f 5355 4d4d  ist/".    __SUMM
+00000340: 4152 595f 5245 504f 5254 5f45 4e44 504f  ARY_REPORT_ENDPO
+00000350: 494e 545f 5632 203d 2022 2f61 7069 2f73  INT_V2 = "/api/s
+00000360: 616d 706c 6573 2f76 322f 6c69 7374 2f22  amples/v2/list/"
+00000370: 0a20 2020 205f 5f44 4554 4149 4c45 445f  .    __DETAILED_
+00000380: 5245 504f 5254 5f45 4e44 504f 494e 545f  REPORT_ENDPOINT_
+00000390: 5632 203d 2022 2f61 7069 2f73 616d 706c  V2 = "/api/sampl
+000003a0: 6573 2f76 322f 6c69 7374 2f64 6574 6169  es/v2/list/detai
+000003b0: 6c73 2f22 0a20 2020 205f 5f43 4c41 5353  ls/".    __CLASS
+000003c0: 4946 595f 454e 4450 4f49 4e54 5f56 3220  IFY_ENDPOINT_V2 
+000003d0: 3d20 222f 6170 692f 7632 2f73 616d 706c  = "/api/v2/sampl
+000003e0: 6573 2f7b 6861 7368 5f76 616c 7565 7d2f  es/{hash_value}/
+000003f0: 636c 6173 7369 6669 6361 7469 6f6e 2f3f  classification/?
+00000400: 6c6f 6361 6c6f 6e6c 793d 7b6c 6f63 616c  localonly={local
+00000410: 6f6e 6c79 7d22 0a20 2020 205f 5f43 4c41  only}".    __CLA
+00000420: 5353 4946 595f 454e 4450 4f49 4e54 5f56  SSIFY_ENDPOINT_V
+00000430: 3320 3d20 222f 6170 692f 7361 6d70 6c65  3 = "/api/sample
+00000440: 732f 7633 2f7b 6861 7368 5f76 616c 7565  s/v3/{hash_value
+00000450: 7d2f 636c 6173 7369 6669 6361 7469 6f6e  }/classification
+00000460: 2f22 0a20 2020 205f 5f52 4541 4e41 4c59  /".    __REANALY
+00000470: 5a45 5f45 4e44 504f 494e 5420 3d20 222f  ZE_ENDPOINT = "/
+00000480: 6170 692f 7361 6d70 6c65 732f 7b68 6173  api/samples/{has
+00000490: 685f 7661 6c75 657d 2f61 6e61 6c79 7a65  h_value}/analyze
+000004a0: 2f22 0a20 2020 205f 5f52 4541 4e41 4c59  /".    __REANALY
+000004b0: 5a45 5f42 554c 4b5f 454e 4450 4f49 4e54  ZE_BULK_ENDPOINT
+000004c0: 203d 2022 2f61 7069 2f73 616d 706c 6573   = "/api/samples
+000004d0: 2f61 6e61 6c79 7a65 5f62 756c 6b2f 220a  /analyze_bulk/".
+000004e0: 2020 2020 5f5f 5245 414e 414c 595a 455f      __REANALYZE_
+000004f0: 4255 4c4b 5f45 4e44 504f 494e 545f 5632  BULK_ENDPOINT_V2
+00000500: 203d 2022 2f61 7069 2f73 616d 706c 6573   = "/api/samples
+00000510: 2f76 322f 616e 616c 797a 655f 6275 6c6b  /v2/analyze_bulk
+00000520: 2f22 0a20 2020 205f 5f4c 4953 545f 4558  /".    __LIST_EX
+00000530: 5452 4143 5445 445f 4649 4c45 535f 454e  TRACTED_FILES_EN
+00000540: 4450 4f49 4e54 203d 2022 2f61 7069 2f73  DPOINT = "/api/s
+00000550: 616d 706c 6573 2f7b 6861 7368 5f76 616c  amples/{hash_val
+00000560: 7565 7d2f 6578 7472 6163 7465 642d 6669  ue}/extracted-fi
+00000570: 6c65 732f 220a 2020 2020 5f5f 4c49 5354  les/".    __LIST
+00000580: 5f45 5854 5241 4354 4544 5f46 494c 4553  _EXTRACTED_FILES
+00000590: 5f45 4e44 504f 494e 545f 5632 203d 2022  _ENDPOINT_V2 = "
+000005a0: 2f61 7069 2f73 616d 706c 6573 2f76 322f  /api/samples/v2/
+000005b0: 7b68 6173 685f 7661 6c75 657d 2f65 7874  {hash_value}/ext
+000005c0: 7261 6374 6564 2d66 696c 6573 2f22 0a20  racted-files/". 
+000005d0: 2020 205f 5f44 4f57 4e4c 4f41 445f 4558     __DOWNLOAD_EX
+000005e0: 5452 4143 5445 445f 4649 4c45 535f 454e  TRACTED_FILES_EN
+000005f0: 4450 4f49 4e54 203d 2022 2f61 7069 2f73  DPOINT = "/api/s
+00000600: 616d 706c 6573 2f7b 6861 7368 5f76 616c  amples/{hash_val
+00000610: 7565 7d2f 756e 7061 636b 6564 2f22 0a20  ue}/unpacked/". 
+00000620: 2020 205f 5f44 4f57 4e4c 4f41 445f 5341     __DOWNLOAD_SA
 00000630: 4d50 4c45 5f45 4e44 504f 494e 5420 3d20  MPLE_ENDPOINT = 
 00000640: 222f 6170 692f 7361 6d70 6c65 732f 7b68  "/api/samples/{h
-00000650: 6173 685f 7661 6c75 657d 2f22 0a20 2020  ash_value}/".   
-00000660: 205f 5f44 454c 4554 455f 5341 4d50 4c45   __DELETE_SAMPLE
-00000670: 535f 4255 4c4b 5f45 4e44 504f 494e 545f  S_BULK_ENDPOINT_
-00000680: 5632 203d 2022 2f61 7069 2f73 616d 706c  V2 = "/api/sampl
-00000690: 6573 2f76 322f 6465 6c65 7465 5f62 756c  es/v2/delete_bul
-000006a0: 6b2f 220a 2020 2020 5f5f 4348 4543 4b5f  k/".    __CHECK_
-000006b0: 5341 4d50 4c45 5f52 454d 4f56 414c 5f53  SAMPLE_REMOVAL_S
-000006c0: 5441 5455 535f 454e 4450 4f49 4e54 5f56  TATUS_ENDPOINT_V
-000006d0: 3220 3d20 222f 6170 692f 7361 6d70 6c65  2 = "/api/sample
-000006e0: 732f 7632 2f64 656c 6574 655f 6275 6c6b  s/v2/delete_bulk
-000006f0: 2f73 7461 7475 732f 3f69 643d 7b74 6173  /status/?id={tas
-00000700: 6b5f 6964 7d22 0a20 2020 205f 5f50 4446  k_id}".    __PDF
-00000710: 5f52 4550 4f52 545f 4352 4541 5445 5f45  _REPORT_CREATE_E
-00000720: 4e44 504f 494e 5420 3d20 222f 6170 692f  NDPOINT = "/api/
-00000730: 7064 662f 7b68 6173 685f 7661 6c75 657d  pdf/{hash_value}
-00000740: 2f63 7265 6174 6522 0a20 2020 205f 5f50  /create".    __P
-00000750: 4446 5f52 4550 4f52 545f 5354 4154 5553  DF_REPORT_STATUS
-00000760: 5f45 4e44 504f 494e 5420 3d20 222f 6170  _ENDPOINT = "/ap
-00000770: 692f 7064 662f 7b68 6173 685f 7661 6c75  i/pdf/{hash_valu
-00000780: 657d 2f73 7461 7475 7322 0a20 2020 205f  e}/status".    _
-00000790: 5f50 4446 5f52 4550 4f52 545f 444f 574e  _PDF_REPORT_DOWN
-000007a0: 4c4f 4144 5f45 4e44 504f 494e 5420 3d20  LOAD_ENDPOINT = 
-000007b0: 222f 6170 692f 7064 662f 7b68 6173 685f  "/api/pdf/{hash_
-000007c0: 7661 6c75 657d 2f64 6f77 6e6c 6f61 6422  value}/download"
-000007d0: 0a20 2020 205f 5f54 4954 414e 4955 4d5f  .    __TITANIUM_
-000007e0: 434f 5245 5f52 4550 4f52 545f 454e 4450  CORE_REPORT_ENDP
-000007f0: 4f49 4e54 5f56 3220 3d20 222f 6170 692f  OINT_V2 = "/api/
-00000800: 7632 2f73 616d 706c 6573 2f7b 6861 7368  v2/samples/{hash
-00000810: 5f76 616c 7565 7d2f 7469 636f 7265 2f3f  _value}/ticore/?
-00000820: 6669 656c 6473 3d7b 6669 656c 6473 7d22  fields={fields}"
-00000830: 0a20 2020 205f 5f44 594e 414d 4943 5f41  .    __DYNAMIC_A
-00000840: 4e41 4c59 5349 535f 5245 504f 5254 5f43  NALYSIS_REPORT_C
-00000850: 5245 4154 455f 454e 4450 4f49 4e54 203d  REATE_ENDPOINT =
-00000860: 2022 2f61 7069 2f72 6c5f 6479 6e61 6d69   "/api/rl_dynami
-00000870: 635f 616e 616c 7973 6973 2f65 7870 6f72  c_analysis/expor
-00000880: 742f 7375 6d6d 6172 792f 7b68 6173 685f  t/summary/{hash_
-00000890: 7661 6c75 657d 2f7b 666f 726d 6174 7d2f  value}/{format}/
-000008a0: 6372 6561 7465 2f22 0a20 2020 205f 5f44  create/".    __D
-000008b0: 594e 414d 4943 5f41 4e41 4c59 5349 535f  YNAMIC_ANALYSIS_
-000008c0: 5245 504f 5254 5f53 5441 5455 535f 454e  REPORT_STATUS_EN
-000008d0: 4450 4f49 4e54 203d 2022 2f61 7069 2f72  DPOINT = "/api/r
-000008e0: 6c5f 6479 6e61 6d69 635f 616e 616c 7973  l_dynamic_analys
-000008f0: 6973 2f65 7870 6f72 742f 7375 6d6d 6172  is/export/summar
-00000900: 792f 7b68 6173 685f 7661 6c75 657d 2f7b  y/{hash_value}/{
-00000910: 666f 726d 6174 7d2f 7374 6174 7573 2f22  format}/status/"
-00000920: 0a20 2020 205f 5f44 594e 414d 4943 5f41  .    __DYNAMIC_A
-00000930: 4e41 4c59 5349 535f 5245 504f 5254 5f44  NALYSIS_REPORT_D
-00000940: 4f57 4e4c 4f41 445f 454e 4450 4f49 4e54  OWNLOAD_ENDPOINT
-00000950: 203d 2022 2f61 7069 2f72 6c5f 6479 6e61   = "/api/rl_dyna
-00000960: 6d69 635f 616e 616c 7973 6973 2f65 7870  mic_analysis/exp
-00000970: 6f72 742f 7375 6d6d 6172 792f 7b68 6173  ort/summary/{has
-00000980: 685f 7661 6c75 657d 2f7b 666f 726d 6174  h_value}/{format
-00000990: 7d22 205c 0a20 2020 2020 2020 2020 2020  }" \.           
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 2020 2020 2022 2f64 6f77 6e6c 6f61         "/downloa
-000009d0: 642f 220a 2020 2020 5f5f 5345 545f 4f52  d/".    __SET_OR
-000009e0: 5f44 454c 4554 455f 434c 4153 5349 4649  _DELETE_CLASSIFI
-000009f0: 4341 5449 4f4e 5f45 4e44 504f 494e 5420  CATION_ENDPOINT 
-00000a00: 3d20 222f 6170 692f 7361 6d70 6c65 732f  = "/api/samples/
-00000a10: 7b68 6173 685f 7661 6c75 657d 2f73 6574  {hash_value}/set
-00000a20: 636c 6173 7369 6669 6361 7469 6f6e 2f7b  classification/{
-00000a30: 7379 7374 656d 7d2f 220a 2020 2020 5f5f  system}/".    __
-00000a40: 5441 4753 5f45 4e44 504f 494e 5420 3d20  TAGS_ENDPOINT = 
-00000a50: 222f 6170 692f 7461 672f 7b68 6173 685f  "/api/tag/{hash_
-00000a60: 7661 6c75 657d 2f22 0a20 2020 205f 5f52  value}/".    __R
-00000a70: 4554 5249 4556 455f 5941 5241 5f52 554c  ETRIEVE_YARA_RUL
-00000a80: 4553 4554 535f 454e 4450 4f49 4e54 5f56  ESETS_ENDPOINT_V
-00000a90: 3220 3d20 222f 6170 692f 7961 7261 2f76  2 = "/api/yara/v
-00000aa0: 322f 7275 6c65 7365 7473 2f22 0a20 2020  2/rulesets/".   
-00000ab0: 205f 5f52 4554 5249 4556 455f 5941 5241   __RETRIEVE_YARA
-00000ac0: 5f52 554c 4553 4554 5f43 4f4e 5445 4e54  _RULESET_CONTENT
-00000ad0: 535f 454e 4450 4f49 4e54 203d 2022 2f61  S_ENDPOINT = "/a
-00000ae0: 7069 2f79 6172 612f 7275 6c65 7365 742f  pi/yara/ruleset/
-00000af0: 636f 6e74 656e 742f 3f6e 616d 653d 7b72  content/?name={r
-00000b00: 756c 6573 6574 5f6e 616d 657d 220a 2020  uleset_name}".  
-00000b10: 2020 5f5f 5245 5452 4945 5645 5f4d 4154    __RETRIEVE_MAT
-00000b20: 4348 4553 5f46 4f52 5f41 5f59 4152 415f  CHES_FOR_A_YARA_
-00000b30: 5255 4c45 5345 545f 454e 4450 4f49 4e54  RULESET_ENDPOINT
-00000b40: 5f56 3220 3d20 222f 6170 692f 7961 7261  _V2 = "/api/yara
-00000b50: 2f76 322f 7275 6c65 7365 742f 6d61 7463  /v2/ruleset/matc
-00000b60: 6865 732f 220a 2020 2020 5f5f 5941 5241  hes/".    __YARA
-00000b70: 5f52 554c 4553 4554 5f45 4e44 504f 494e  _RULESET_ENDPOIN
-00000b80: 5420 3d20 222f 6170 692f 7961 7261 2f72  T = "/api/yara/r
-00000b90: 756c 6573 6574 2f22 0a20 2020 205f 5f45  uleset/".    __E
-00000ba0: 4e41 424c 455f 4f52 5f44 4953 4142 4c45  NABLE_OR_DISABLE
+00000650: 6173 685f 7661 6c75 657d 2f64 6f77 6e6c  ash_value}/downl
+00000660: 6f61 642f 220a 2020 2020 5f5f 4445 4c45  oad/".    __DELE
+00000670: 5445 5f53 414d 504c 455f 454e 4450 4f49  TE_SAMPLE_ENDPOI
+00000680: 4e54 203d 2022 2f61 7069 2f73 616d 706c  NT = "/api/sampl
+00000690: 6573 2f7b 6861 7368 5f76 616c 7565 7d2f  es/{hash_value}/
+000006a0: 220a 2020 2020 5f5f 4445 4c45 5445 5f53  ".    __DELETE_S
+000006b0: 414d 504c 4553 5f42 554c 4b5f 454e 4450  AMPLES_BULK_ENDP
+000006c0: 4f49 4e54 5f56 3220 3d20 222f 6170 692f  OINT_V2 = "/api/
+000006d0: 7361 6d70 6c65 732f 7632 2f64 656c 6574  samples/v2/delet
+000006e0: 655f 6275 6c6b 2f22 0a20 2020 205f 5f43  e_bulk/".    __C
+000006f0: 4845 434b 5f53 414d 504c 455f 5245 4d4f  HECK_SAMPLE_REMO
+00000700: 5641 4c5f 5354 4154 5553 5f45 4e44 504f  VAL_STATUS_ENDPO
+00000710: 494e 545f 5632 203d 2022 2f61 7069 2f73  INT_V2 = "/api/s
+00000720: 616d 706c 6573 2f76 322f 6465 6c65 7465  amples/v2/delete
+00000730: 5f62 756c 6b2f 7374 6174 7573 2f3f 6964  _bulk/status/?id
+00000740: 3d7b 7461 736b 5f69 647d 220a 2020 2020  ={task_id}".    
+00000750: 5f5f 5044 465f 5245 504f 5254 5f43 5245  __PDF_REPORT_CRE
+00000760: 4154 455f 454e 4450 4f49 4e54 203d 2022  ATE_ENDPOINT = "
+00000770: 2f61 7069 2f70 6466 2f7b 6861 7368 5f76  /api/pdf/{hash_v
+00000780: 616c 7565 7d2f 6372 6561 7465 220a 2020  alue}/create".  
+00000790: 2020 5f5f 5044 465f 5245 504f 5254 5f53    __PDF_REPORT_S
+000007a0: 5441 5455 535f 454e 4450 4f49 4e54 203d  TATUS_ENDPOINT =
+000007b0: 2022 2f61 7069 2f70 6466 2f7b 6861 7368   "/api/pdf/{hash
+000007c0: 5f76 616c 7565 7d2f 7374 6174 7573 220a  _value}/status".
+000007d0: 2020 2020 5f5f 5044 465f 5245 504f 5254      __PDF_REPORT
+000007e0: 5f44 4f57 4e4c 4f41 445f 454e 4450 4f49  _DOWNLOAD_ENDPOI
+000007f0: 4e54 203d 2022 2f61 7069 2f70 6466 2f7b  NT = "/api/pdf/{
+00000800: 6861 7368 5f76 616c 7565 7d2f 646f 776e  hash_value}/down
+00000810: 6c6f 6164 220a 2020 2020 5f5f 5449 5441  load".    __TITA
+00000820: 4e49 554d 5f43 4f52 455f 5245 504f 5254  NIUM_CORE_REPORT
+00000830: 5f45 4e44 504f 494e 545f 5632 203d 2022  _ENDPOINT_V2 = "
+00000840: 2f61 7069 2f76 322f 7361 6d70 6c65 732f  /api/v2/samples/
+00000850: 7b68 6173 685f 7661 6c75 657d 2f74 6963  {hash_value}/tic
+00000860: 6f72 652f 3f66 6965 6c64 733d 7b66 6965  ore/?fields={fie
+00000870: 6c64 737d 220a 2020 2020 5f5f 4459 4e41  lds}".    __DYNA
+00000880: 4d49 435f 414e 414c 5953 4953 5f52 4550  MIC_ANALYSIS_REP
+00000890: 4f52 545f 4352 4541 5445 5f45 4e44 504f  ORT_CREATE_ENDPO
+000008a0: 494e 5420 3d20 222f 6170 692f 726c 5f64  INT = "/api/rl_d
+000008b0: 796e 616d 6963 5f61 6e61 6c79 7369 732f  ynamic_analysis/
+000008c0: 6578 706f 7274 2f73 756d 6d61 7279 2f7b  export/summary/{
+000008d0: 6861 7368 5f76 616c 7565 7d2f 7b66 6f72  hash_value}/{for
+000008e0: 6d61 747d 2f63 7265 6174 652f 220a 2020  mat}/create/".  
+000008f0: 2020 5f5f 4459 4e41 4d49 435f 414e 414c    __DYNAMIC_ANAL
+00000900: 5953 4953 5f52 4550 4f52 545f 5354 4154  YSIS_REPORT_STAT
+00000910: 5553 5f45 4e44 504f 494e 5420 3d20 222f  US_ENDPOINT = "/
+00000920: 6170 692f 726c 5f64 796e 616d 6963 5f61  api/rl_dynamic_a
+00000930: 6e61 6c79 7369 732f 6578 706f 7274 2f73  nalysis/export/s
+00000940: 756d 6d61 7279 2f7b 6861 7368 5f76 616c  ummary/{hash_val
+00000950: 7565 7d2f 7b66 6f72 6d61 747d 2f73 7461  ue}/{format}/sta
+00000960: 7475 732f 220a 2020 2020 5f5f 4459 4e41  tus/".    __DYNA
+00000970: 4d49 435f 414e 414c 5953 4953 5f52 4550  MIC_ANALYSIS_REP
+00000980: 4f52 545f 444f 574e 4c4f 4144 5f45 4e44  ORT_DOWNLOAD_END
+00000990: 504f 494e 5420 3d20 222f 6170 692f 726c  POINT = "/api/rl
+000009a0: 5f64 796e 616d 6963 5f61 6e61 6c79 7369  _dynamic_analysi
+000009b0: 732f 6578 706f 7274 2f73 756d 6d61 7279  s/export/summary
+000009c0: 2f7b 6861 7368 5f76 616c 7565 7d2f 7b66  /{hash_value}/{f
+000009d0: 6f72 6d61 747d 2220 5c0a 2020 2020 2020  ormat}" \.      
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 2020 2020 2020 2020 2020 2020 222f 646f              "/do
+00000a10: 776e 6c6f 6164 2f22 0a20 2020 205f 5f53  wnload/".    __S
+00000a20: 4554 5f4f 525f 4445 4c45 5445 5f43 4c41  ET_OR_DELETE_CLA
+00000a30: 5353 4946 4943 4154 494f 4e5f 454e 4450  SSIFICATION_ENDP
+00000a40: 4f49 4e54 203d 2022 2f61 7069 2f73 616d  OINT = "/api/sam
+00000a50: 706c 6573 2f7b 6861 7368 5f76 616c 7565  ples/{hash_value
+00000a60: 7d2f 7365 7463 6c61 7373 6966 6963 6174  }/setclassificat
+00000a70: 696f 6e2f 7b73 7973 7465 6d7d 2f22 0a20  ion/{system}/". 
+00000a80: 2020 205f 5f54 4147 535f 454e 4450 4f49     __TAGS_ENDPOI
+00000a90: 4e54 203d 2022 2f61 7069 2f74 6167 2f7b  NT = "/api/tag/{
+00000aa0: 6861 7368 5f76 616c 7565 7d2f 220a 2020  hash_value}/".  
+00000ab0: 2020 5f5f 5245 5452 4945 5645 5f59 4152    __RETRIEVE_YAR
+00000ac0: 415f 5255 4c45 5345 5453 5f45 4e44 504f  A_RULESETS_ENDPO
+00000ad0: 494e 545f 5632 203d 2022 2f61 7069 2f79  INT_V2 = "/api/y
+00000ae0: 6172 612f 7632 2f72 756c 6573 6574 732f  ara/v2/rulesets/
+00000af0: 220a 2020 2020 5f5f 5245 5452 4945 5645  ".    __RETRIEVE
+00000b00: 5f59 4152 415f 5255 4c45 5345 545f 434f  _YARA_RULESET_CO
+00000b10: 4e54 454e 5453 5f45 4e44 504f 494e 5420  NTENTS_ENDPOINT 
+00000b20: 3d20 222f 6170 692f 7961 7261 2f72 756c  = "/api/yara/rul
+00000b30: 6573 6574 2f63 6f6e 7465 6e74 2f3f 6e61  eset/content/?na
+00000b40: 6d65 3d7b 7275 6c65 7365 745f 6e61 6d65  me={ruleset_name
+00000b50: 7d22 0a20 2020 205f 5f52 4554 5249 4556  }".    __RETRIEV
+00000b60: 455f 4d41 5443 4845 535f 464f 525f 415f  E_MATCHES_FOR_A_
+00000b70: 5941 5241 5f52 554c 4553 4554 5f45 4e44  YARA_RULESET_END
+00000b80: 504f 494e 545f 5632 203d 2022 2f61 7069  POINT_V2 = "/api
+00000b90: 2f79 6172 612f 7632 2f72 756c 6573 6574  /yara/v2/ruleset
+00000ba0: 2f6d 6174 6368 6573 2f22 0a20 2020 205f  /matches/".    _
 00000bb0: 5f59 4152 415f 5255 4c45 5345 545f 454e  _YARA_RULESET_EN
 00000bc0: 4450 4f49 4e54 203d 2022 2f61 7069 2f79  DPOINT = "/api/y
-00000bd0: 6172 612f 7275 6c65 7365 742f 7b6f 7065  ara/ruleset/{ope
-00000be0: 7261 7469 6f6e 7d2f 220a 2020 2020 5f5f  ration}/".    __
-00000bf0: 4745 545f 4f52 5f53 4554 5f59 4152 415f  GET_OR_SET_YARA_
-00000c00: 5255 4c45 5345 545f 5359 4e43 4852 4f4e  RULESET_SYNCHRON
-00000c10: 495a 4154 494f 4e5f 5449 4d45 5f45 4e44  IZATION_TIME_END
-00000c20: 504f 494e 5420 3d20 222f 6170 692f 7961  POINT = "/api/ya
-00000c30: 7261 2f74 6963 6c6f 7564 2f74 696d 652f  ra/ticloud/time/
-00000c40: 220a 2020 2020 5f5f 5941 5241 5f4c 4f43  ".    __YARA_LOC
-00000c50: 414c 5f52 4554 524f 5343 414e 5f45 4e44  AL_RETROSCAN_END
-00000c60: 504f 494e 5420 3d20 222f 6170 692f 7570  POINT = "/api/up
-00000c70: 6c6f 6164 732f 6c6f 6361 6c2d 7265 7472  loads/local-retr
-00000c80: 6f2d 6875 6e74 2f22 0a20 2020 205f 5f59  o-hunt/".    __Y
-00000c90: 4152 415f 434c 4f55 445f 5245 5452 4f53  ARA_CLOUD_RETROS
-00000ca0: 4341 4e53 5f45 4e44 504f 494e 5420 3d20  CANS_ENDPOINT = 
-00000cb0: 222f 6170 692f 7961 7261 2f72 756c 6573  "/api/yara/rules
-00000cc0: 6574 2f7b 7275 6c65 7365 745f 6e61 6d65  et/{ruleset_name
-00000cd0: 7d2f 636c 6f75 642d 7265 7472 6f2d 6875  }/cloud-retro-hu
-00000ce0: 6e74 2f22 0a20 2020 205f 5f41 4456 414e  nt/".    __ADVAN
-00000cf0: 4345 445f 5345 4152 4348 5f45 4e44 504f  CED_SEARCH_ENDPO
-00000d00: 494e 5420 3d20 222f 6170 692f 7361 6d70  INT = "/api/samp
-00000d10: 6c65 732f 7365 6172 6368 2f22 0a20 2020  les/search/".   
-00000d20: 205f 5f41 4456 414e 4345 445f 5345 4152   __ADVANCED_SEAR
-00000d30: 4348 5f45 4e44 504f 494e 545f 5632 203d  CH_ENDPOINT_V2 =
-00000d40: 2022 2f61 7069 2f73 616d 706c 6573 2f76   "/api/samples/v
-00000d50: 322f 7365 6172 6368 2f22 0a20 2020 205f  2/search/".    _
-00000d60: 5f4c 4953 545f 434f 4e54 4149 4e45 5253  _LIST_CONTAINERS
-00000d70: 5f45 4e44 504f 494e 5420 3d20 222f 6170  _ENDPOINT = "/ap
-00000d80: 692f 7361 6d70 6c65 732f 636f 6e74 6169  i/samples/contai
-00000d90: 6e65 7273 2f22 0a20 2020 205f 5f55 524c  ners/".    __URL
-00000da0: 5f52 4550 4f52 545f 454e 4450 4f49 4e54  _REPORT_ENDPOINT
-00000db0: 203d 2022 2f61 7069 2f6e 6574 776f 726b   = "/api/network
-00000dc0: 2d74 6872 6561 742d 696e 7465 6c2f 7572  -threat-intel/ur
-00000dd0: 6c2f 220a 2020 2020 5f5f 444f 4d41 494e  l/".    __DOMAIN
-00000de0: 5f52 4550 4f52 545f 454e 4450 4f49 4e54  _REPORT_ENDPOINT
-00000df0: 203d 2022 2f61 7069 2f6e 6574 776f 726b   = "/api/network
-00000e00: 2d74 6872 6561 742d 696e 7465 6c2f 646f  -threat-intel/do
-00000e10: 6d61 696e 2f7b 646f 6d61 696e 7d2f 220a  main/{domain}/".
-00000e20: 2020 2020 5f5f 4950 5f52 4550 4f52 545f      __IP_REPORT_
-00000e30: 454e 4450 4f49 4e54 203d 2022 2f61 7069  ENDPOINT = "/api
-00000e40: 2f6e 6574 776f 726b 2d74 6872 6561 742d  /network-threat-
-00000e50: 696e 7465 6c2f 6970 2f7b 6970 7d2f 7265  intel/ip/{ip}/re
-00000e60: 706f 7274 2f22 0a20 2020 205f 5f49 505f  port/".    __IP_
-00000e70: 544f 5f44 4f4d 4149 4e5f 454e 4450 4f49  TO_DOMAIN_ENDPOI
-00000e80: 4e54 203d 2022 2f61 7069 2f6e 6574 776f  NT = "/api/netwo
-00000e90: 726b 2d74 6872 6561 742d 696e 7465 6c2f  rk-threat-intel/
-00000ea0: 6970 2f7b 6970 7d2f 7265 736f 6c75 7469  ip/{ip}/resoluti
-00000eb0: 6f6e 732f 220a 2020 2020 5f5f 5552 4c53  ons/".    __URLS
-00000ec0: 5f46 524f 4d5f 4950 5f45 4e44 504f 494e  _FROM_IP_ENDPOIN
-00000ed0: 5420 3d20 222f 6170 692f 6e65 7477 6f72  T = "/api/networ
-00000ee0: 6b2d 7468 7265 6174 2d69 6e74 656c 2f69  k-threat-intel/i
-00000ef0: 702f 7b69 707d 2f75 726c 732f 220a 2020  p/{ip}/urls/".  
-00000f00: 2020 5f5f 4649 4c45 535f 4652 4f4d 5f49    __FILES_FROM_I
-00000f10: 505f 454e 4450 4f49 4e54 203d 2022 2f61  P_ENDPOINT = "/a
-00000f20: 7069 2f6e 6574 776f 726b 2d74 6872 6561  pi/network-threa
-00000f30: 742d 696e 7465 6c2f 6970 2f7b 6970 7d2f  t-intel/ip/{ip}/
-00000f40: 646f 776e 6c6f 6164 6564 5f66 696c 6573  downloaded_files
-00000f50: 2f22 0a0a 0a20 2020 2023 2055 7365 6420  /"...    # Used 
-00000f60: 6279 2074 6865 2064 6570 7265 6361 7465  by the deprecate
-00000f70: 6420 6765 745f 7265 7375 6c74 7320 6d65  d get_results me
-00000f80: 7468 6f64 0a20 2020 205f 5f46 4945 4c44  thod.    __FIELD
-00000f90: 5320 3d20 2822 6964 222c 2022 7368 6131  S = ("id", "sha1
-00000fa0: 222c 2022 7368 6132 3536 222c 2022 7368  ", "sha256", "sh
-00000fb0: 6135 3132 222c 2022 6d64 3522 2c20 2263  a512", "md5", "c
-00000fc0: 6174 6567 6f72 7922 2c20 2266 696c 655f  ategory", "file_
-00000fd0: 7479 7065 222c 2022 6669 6c65 5f73 7562  type", "file_sub
-00000fe0: 7479 7065 222c 2022 6964 656e 7469 6669  type", "identifi
-00000ff0: 6361 7469 6f6e 5f6e 616d 6522 2c0a 2020  cation_name",.  
-00001000: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00001010: 6465 6e74 6966 6963 6174 696f 6e5f 7665  dentification_ve
-00001020: 7273 696f 6e22 2c20 2266 696c 655f 7369  rsion", "file_si
-00001030: 7a65 222c 2022 6578 7472 6163 7465 645f  ze", "extracted_
-00001040: 6669 6c65 5f63 6f75 6e74 222c 2022 6c6f  file_count", "lo
-00001050: 6361 6c5f 6669 7273 745f 7365 656e 222c  cal_first_seen",
-00001060: 2022 6c6f 6361 6c5f 6c61 7374 5f73 6565   "local_last_see
-00001070: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-00001080: 2020 2020 2263 6c61 7373 6966 6963 6174      "classificat
-00001090: 696f 6e5f 6f72 6967 696e 222c 2022 636c  ion_origin", "cl
-000010a0: 6173 7369 6669 6361 7469 6f6e 5f72 6561  assification_rea
-000010b0: 736f 6e22 2c20 2274 6872 6561 745f 7374  son", "threat_st
-000010c0: 6174 7573 222c 2022 7472 7573 745f 6661  atus", "trust_fa
-000010d0: 6374 6f72 222c 2022 7468 7265 6174 5f6c  ctor", "threat_l
-000010e0: 6576 656c 222c 0a20 2020 2020 2020 2020  evel",.         
-000010f0: 2020 2020 2020 2022 7468 7265 6174 5f6e         "threat_n
-00001100: 616d 6522 2c20 2274 6963 6f72 6522 2c20  ame", "ticore", 
-00001110: 2273 756d 6d61 7279 222c 2022 7469 636c  "summary", "ticl
-00001120: 6f75 6422 2c20 2261 6c69 6173 6573 220a  oud", "aliases".
-00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001140: 290a 0a20 2020 205f 5f46 4945 4c44 535f  )..    __FIELDS_
-00001150: 5632 203d 2028 2269 6422 2c20 2273 6861  V2 = ("id", "sha
-00001160: 3122 2c20 2273 6861 3235 3622 2c20 2273  1", "sha256", "s
-00001170: 6861 3531 3222 2c20 226d 6435 222c 2022  ha512", "md5", "
-00001180: 6361 7465 676f 7279 222c 2022 6669 6c65  category", "file
-00001190: 5f74 7970 6522 2c20 2266 696c 655f 7375  _type", "file_su
-000011a0: 6274 7970 6522 2c0a 2020 2020 2020 2020  btype",.        
-000011b0: 2020 2020 2020 2020 2020 2022 6964 656e             "iden
-000011c0: 7469 6669 6361 7469 6f6e 5f6e 616d 6522  tification_name"
-000011d0: 2c20 2269 6465 6e74 6966 6963 6174 696f  , "identificatio
-000011e0: 6e5f 7665 7273 696f 6e22 2c20 2266 696c  n_version", "fil
-000011f0: 655f 7369 7a65 222c 2022 6578 7472 6163  e_size", "extrac
-00001200: 7465 645f 6669 6c65 5f63 6f75 6e74 222c  ted_file_count",
-00001210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001220: 2020 2020 226c 6f63 616c 5f66 6972 7374      "local_first
-00001230: 5f73 6565 6e22 2c20 226c 6f63 616c 5f6c  _seen", "local_l
-00001240: 6173 745f 7365 656e 222c 2022 636c 6173  ast_seen", "clas
-00001250: 7369 6669 6361 7469 6f6e 5f6f 7269 6769  sification_origi
-00001260: 6e22 2c20 2263 6c61 7373 6966 6963 6174  n", "classificat
-00001270: 696f 6e5f 7265 6173 6f6e 222c 0a20 2020  ion_reason",.   
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 6172 612f 7275 6c65 7365 742f 220a 2020  ara/ruleset/".  
+00000be0: 2020 5f5f 454e 4142 4c45 5f4f 525f 4449    __ENABLE_OR_DI
+00000bf0: 5341 424c 455f 5941 5241 5f52 554c 4553  SABLE_YARA_RULES
+00000c00: 4554 5f45 4e44 504f 494e 5420 3d20 222f  ET_ENDPOINT = "/
+00000c10: 6170 692f 7961 7261 2f72 756c 6573 6574  api/yara/ruleset
+00000c20: 2f7b 6f70 6572 6174 696f 6e7d 2f22 0a20  /{operation}/". 
+00000c30: 2020 205f 5f47 4554 5f4f 525f 5345 545f     __GET_OR_SET_
+00000c40: 5941 5241 5f52 554c 4553 4554 5f53 594e  YARA_RULESET_SYN
+00000c50: 4348 524f 4e49 5a41 5449 4f4e 5f54 494d  CHRONIZATION_TIM
+00000c60: 455f 454e 4450 4f49 4e54 203d 2022 2f61  E_ENDPOINT = "/a
+00000c70: 7069 2f79 6172 612f 7469 636c 6f75 642f  pi/yara/ticloud/
+00000c80: 7469 6d65 2f22 0a20 2020 205f 5f59 4152  time/".    __YAR
+00000c90: 415f 4c4f 4341 4c5f 5245 5452 4f53 4341  A_LOCAL_RETROSCA
+00000ca0: 4e5f 454e 4450 4f49 4e54 203d 2022 2f61  N_ENDPOINT = "/a
+00000cb0: 7069 2f75 706c 6f61 6473 2f6c 6f63 616c  pi/uploads/local
+00000cc0: 2d72 6574 726f 2d68 756e 742f 220a 2020  -retro-hunt/".  
+00000cd0: 2020 5f5f 5941 5241 5f43 4c4f 5544 5f52    __YARA_CLOUD_R
+00000ce0: 4554 524f 5343 414e 535f 454e 4450 4f49  ETROSCANS_ENDPOI
+00000cf0: 4e54 203d 2022 2f61 7069 2f79 6172 612f  NT = "/api/yara/
+00000d00: 7275 6c65 7365 742f 7b72 756c 6573 6574  ruleset/{ruleset
+00000d10: 5f6e 616d 657d 2f63 6c6f 7564 2d72 6574  _name}/cloud-ret
+00000d20: 726f 2d68 756e 742f 220a 2020 2020 5f5f  ro-hunt/".    __
+00000d30: 4144 5641 4e43 4544 5f53 4541 5243 485f  ADVANCED_SEARCH_
+00000d40: 454e 4450 4f49 4e54 203d 2022 2f61 7069  ENDPOINT = "/api
+00000d50: 2f73 616d 706c 6573 2f73 6561 7263 682f  /samples/search/
+00000d60: 220a 2020 2020 5f5f 4144 5641 4e43 4544  ".    __ADVANCED
+00000d70: 5f53 4541 5243 485f 454e 4450 4f49 4e54  _SEARCH_ENDPOINT
+00000d80: 5f56 3220 3d20 222f 6170 692f 7361 6d70  _V2 = "/api/samp
+00000d90: 6c65 732f 7632 2f73 6561 7263 682f 220a  les/v2/search/".
+00000da0: 2020 2020 5f5f 4c49 5354 5f43 4f4e 5441      __LIST_CONTA
+00000db0: 494e 4552 535f 454e 4450 4f49 4e54 203d  INERS_ENDPOINT =
+00000dc0: 2022 2f61 7069 2f73 616d 706c 6573 2f63   "/api/samples/c
+00000dd0: 6f6e 7461 696e 6572 732f 220a 2020 2020  ontainers/".    
+00000de0: 5f5f 5552 4c5f 5245 504f 5254 5f45 4e44  __URL_REPORT_END
+00000df0: 504f 494e 5420 3d20 222f 6170 692f 6e65  POINT = "/api/ne
+00000e00: 7477 6f72 6b2d 7468 7265 6174 2d69 6e74  twork-threat-int
+00000e10: 656c 2f75 726c 2f22 0a20 2020 205f 5f44  el/url/".    __D
+00000e20: 4f4d 4149 4e5f 5245 504f 5254 5f45 4e44  OMAIN_REPORT_END
+00000e30: 504f 494e 5420 3d20 222f 6170 692f 6e65  POINT = "/api/ne
+00000e40: 7477 6f72 6b2d 7468 7265 6174 2d69 6e74  twork-threat-int
+00000e50: 656c 2f64 6f6d 6169 6e2f 7b64 6f6d 6169  el/domain/{domai
+00000e60: 6e7d 2f22 0a20 2020 205f 5f49 505f 5245  n}/".    __IP_RE
+00000e70: 504f 5254 5f45 4e44 504f 494e 5420 3d20  PORT_ENDPOINT = 
+00000e80: 222f 6170 692f 6e65 7477 6f72 6b2d 7468  "/api/network-th
+00000e90: 7265 6174 2d69 6e74 656c 2f69 702f 7b69  reat-intel/ip/{i
+00000ea0: 707d 2f72 6570 6f72 742f 220a 2020 2020  p}/report/".    
+00000eb0: 5f5f 4950 5f54 4f5f 444f 4d41 494e 5f45  __IP_TO_DOMAIN_E
+00000ec0: 4e44 504f 494e 5420 3d20 222f 6170 692f  NDPOINT = "/api/
+00000ed0: 6e65 7477 6f72 6b2d 7468 7265 6174 2d69  network-threat-i
+00000ee0: 6e74 656c 2f69 702f 7b69 707d 2f72 6573  ntel/ip/{ip}/res
+00000ef0: 6f6c 7574 696f 6e73 2f22 0a20 2020 205f  olutions/".    _
+00000f00: 5f55 524c 535f 4652 4f4d 5f49 505f 454e  _URLS_FROM_IP_EN
+00000f10: 4450 4f49 4e54 203d 2022 2f61 7069 2f6e  DPOINT = "/api/n
+00000f20: 6574 776f 726b 2d74 6872 6561 742d 696e  etwork-threat-in
+00000f30: 7465 6c2f 6970 2f7b 6970 7d2f 7572 6c73  tel/ip/{ip}/urls
+00000f40: 2f22 0a20 2020 205f 5f46 494c 4553 5f46  /".    __FILES_F
+00000f50: 524f 4d5f 4950 5f45 4e44 504f 494e 5420  ROM_IP_ENDPOINT 
+00000f60: 3d20 222f 6170 692f 6e65 7477 6f72 6b2d  = "/api/network-
+00000f70: 7468 7265 6174 2d69 6e74 656c 2f69 702f  threat-intel/ip/
+00000f80: 7b69 707d 2f64 6f77 6e6c 6f61 6465 645f  {ip}/downloaded_
+00000f90: 6669 6c65 732f 220a 0a0a 2020 2020 2320  files/"...    # 
+00000fa0: 5573 6564 2062 7920 7468 6520 6465 7072  Used by the depr
+00000fb0: 6563 6174 6564 2067 6574 5f72 6573 756c  ecated get_resul
+00000fc0: 7473 206d 6574 686f 640a 2020 2020 5f5f  ts method.    __
+00000fd0: 4649 454c 4453 203d 2028 2269 6422 2c20  FIELDS = ("id", 
+00000fe0: 2273 6861 3122 2c20 2273 6861 3235 3622  "sha1", "sha256"
+00000ff0: 2c20 2273 6861 3531 3222 2c20 226d 6435  , "sha512", "md5
+00001000: 222c 2022 6361 7465 676f 7279 222c 2022  ", "category", "
+00001010: 6669 6c65 5f74 7970 6522 2c20 2266 696c  file_type", "fil
+00001020: 655f 7375 6274 7970 6522 2c20 2269 6465  e_subtype", "ide
+00001030: 6e74 6966 6963 6174 696f 6e5f 6e61 6d65  ntification_name
+00001040: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001050: 2020 2022 6964 656e 7469 6669 6361 7469     "identificati
+00001060: 6f6e 5f76 6572 7369 6f6e 222c 2022 6669  on_version", "fi
+00001070: 6c65 5f73 697a 6522 2c20 2265 7874 7261  le_size", "extra
+00001080: 6374 6564 5f66 696c 655f 636f 756e 7422  cted_file_count"
+00001090: 2c20 226c 6f63 616c 5f66 6972 7374 5f73  , "local_first_s
+000010a0: 6565 6e22 2c20 226c 6f63 616c 5f6c 6173  een", "local_las
+000010b0: 745f 7365 656e 222c 0a20 2020 2020 2020  t_seen",.       
+000010c0: 2020 2020 2020 2020 2022 636c 6173 7369           "classi
+000010d0: 6669 6361 7469 6f6e 5f6f 7269 6769 6e22  fication_origin"
+000010e0: 2c20 2263 6c61 7373 6966 6963 6174 696f  , "classificatio
+000010f0: 6e5f 7265 6173 6f6e 222c 2022 7468 7265  n_reason", "thre
+00001100: 6174 5f73 7461 7475 7322 2c20 2274 7275  at_status", "tru
+00001110: 7374 5f66 6163 746f 7222 2c20 2274 6872  st_factor", "thr
+00001120: 6561 745f 6c65 7665 6c22 2c0a 2020 2020  eat_level",.    
+00001130: 2020 2020 2020 2020 2020 2020 2274 6872              "thr
+00001140: 6561 745f 6e61 6d65 222c 2022 7469 636f  eat_name", "tico
+00001150: 7265 222c 2022 7375 6d6d 6172 7922 2c20  re", "summary", 
+00001160: 2274 6963 6c6f 7564 222c 2022 616c 6961  "ticloud", "alia
+00001170: 7365 7322 0a20 2020 2020 2020 2020 2020  ses".           
+00001180: 2020 2020 2029 0a0a 2020 2020 5f5f 4649       )..    __FI
+00001190: 454c 4453 5f56 3220 3d20 2822 6964 222c  ELDS_V2 = ("id",
+000011a0: 2022 7368 6131 222c 2022 7368 6132 3536   "sha1", "sha256
+000011b0: 222c 2022 7368 6135 3132 222c 2022 6d64  ", "sha512", "md
+000011c0: 3522 2c20 2263 6174 6567 6f72 7922 2c20  5", "category", 
+000011d0: 2266 696c 655f 7479 7065 222c 2022 6669  "file_type", "fi
+000011e0: 6c65 5f73 7562 7479 7065 222c 0a20 2020  le_subtype",.   
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001200: 2269 6465 6e74 6966 6963 6174 696f 6e5f  "identification_
+00001210: 6e61 6d65 222c 2022 6964 656e 7469 6669  name", "identifi
+00001220: 6361 7469 6f6e 5f76 6572 7369 6f6e 222c  cation_version",
+00001230: 2022 6669 6c65 5f73 697a 6522 2c20 2265   "file_size", "e
+00001240: 7874 7261 6374 6564 5f66 696c 655f 636f  xtracted_file_co
+00001250: 756e 7422 2c0a 2020 2020 2020 2020 2020  unt",.          
+00001260: 2020 2020 2020 2020 2022 6c6f 6361 6c5f           "local_
+00001270: 6669 7273 745f 7365 656e 222c 2022 6c6f  first_seen", "lo
+00001280: 6361 6c5f 6c61 7374 5f73 6565 6e22 2c20  cal_last_seen", 
 00001290: 2263 6c61 7373 6966 6963 6174 696f 6e5f  "classification_
-000012a0: 736f 7572 6365 222c 2022 636c 6173 7369  source", "classi
-000012b0: 6669 6361 7469 6f6e 222c 2022 7269 736b  fication", "risk
-000012c0: 7363 6f72 6522 2c20 2263 6c61 7373 6966  score", "classif
-000012d0: 6963 6174 696f 6e5f 7265 7375 6c74 222c  ication_result",
-000012e0: 2022 7469 636f 7265 222c 2022 7461 6773   "ticore", "tags
-000012f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001300: 2020 2020 2020 2273 756d 6d61 7279 222c        "summary",
-00001310: 2022 7469 636c 6f75 6422 2c20 2261 6c69   "ticloud", "ali
-00001320: 6173 6573 222c 2022 6e65 7477 6f72 6b74  ases", "networkt
-00001330: 6872 6561 7469 6e74 656c 6c69 6765 6e63  hreatintelligenc
-00001340: 6522 2c20 2264 6f6d 6169 6e74 6872 6561  e", "domainthrea
-00001350: 7469 6e74 656c 6c69 6765 6e63 6522 0a20  tintelligence". 
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 290a 0a20 2020 205f 5f54 4954 414e    )..    __TITAN
-00001380: 4955 4d5f 434f 5245 5f46 4945 4c44 5320  IUM_CORE_FIELDS 
-00001390: 3d20 2273 6861 312c 2073 6861 3235 362c  = "sha1, sha256,
-000013a0: 2073 6861 3531 322c 206d 6435 2c20 696d   sha512, md5, im
-000013b0: 7068 6173 682c 2069 6e66 6f2c 2061 7070  phash, info, app
-000013c0: 6c69 6361 7469 6f6e 2c20 7072 6f74 6563  lication, protec
-000013d0: 7469 6f6e 2c20 7365 6375 7269 7479 2c20  tion, security, 
-000013e0: 6265 6861 7669 6f75 722c 2220 5c0a 2020  behaviour," \.  
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 2020 2020 2020 2020 2020 2022 2063 6572             " cer
-00001410: 7469 6669 6361 7465 2c20 646f 6375 6d65  tificate, docume
-00001420: 6e74 2c20 6d6f 6269 6c65 2c20 6d65 6469  nt, mobile, medi
-00001430: 612c 2077 6562 2c20 656d 6169 6c2c 2073  a, web, email, s
-00001440: 7472 696e 6773 2c20 696e 7465 7265 7374  trings, interest
-00001450: 696e 675f 7374 7269 6e67 732c 2220 5c0a  ing_strings," \.
-00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001470: 2020 2020 2020 2020 2020 2020 2022 2063               " c
-00001480: 6c61 7373 6966 6963 6174 696f 6e2c 2069  lassification, i
-00001490: 6e64 6963 6174 6f72 732c 2074 6167 732c  ndicators, tags,
-000014a0: 2061 7474 6163 6b2c 2073 746f 7279 220a   attack, story".
-000014b0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000014c0: 5f28 7365 6c66 2c20 686f 7374 2c20 7573  _(self, host, us
-000014d0: 6572 6e61 6d65 3d4e 6f6e 652c 2070 6173  ername=None, pas
-000014e0: 7377 6f72 643d 4e6f 6e65 2c20 746f 6b65  sword=None, toke
-000014f0: 6e3d 4e6f 6e65 2c20 6669 656c 6473 3d5f  n=None, fields=_
-00001500: 5f46 4945 4c44 532c 2066 6965 6c64 735f  _FIELDS, fields_
-00001510: 7632 3d5f 5f46 4945 4c44 535f 5632 2c0a  v2=__FIELDS_V2,.
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2074 6963 6f72 655f 6669 656c 6473 3d5f   ticore_fields=_
-00001540: 5f54 4954 414e 4955 4d5f 434f 5245 5f46  _TITANIUM_CORE_F
-00001550: 4945 4c44 532c 2077 6169 745f 7469 6d65  IELDS, wait_time
-00001560: 5f73 6563 6f6e 6473 3d32 2c20 7265 7472  _seconds=2, retr
-00001570: 6965 733d 3130 2c20 7665 7269 6679 3d54  ies=10, verify=T
-00001580: 7275 652c 2070 726f 7869 6573 3d4e 6f6e  rue, proxies=Non
-00001590: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000015a0: 2020 2020 7573 6572 5f61 6765 6e74 3d44      user_agent=D
-000015b0: 4546 4155 4c54 5f55 5345 525f 4147 454e  EFAULT_USER_AGEN
-000015c0: 5429 3a0a 0a20 2020 2020 2020 2073 656c  T):..        sel
-000015d0: 662e 5f68 6f73 7420 3d20 7365 6c66 2e5f  f._host = self._
-000015e0: 5f76 616c 6964 6174 655f 686f 7374 2868  _validate_host(h
-000015f0: 6f73 7429 0a20 2020 2020 2020 2073 656c  ost).        sel
-00001600: 662e 5f75 726c 203d 2022 7b68 6f73 747d  f._url = "{host}
-00001610: 7b7b 656e 6470 6f69 6e74 7d7d 222e 666f  {{endpoint}}".fo
-00001620: 726d 6174 2868 6f73 743d 7365 6c66 2e5f  rmat(host=self._
-00001630: 686f 7374 290a 2020 2020 2020 2020 7365  host).        se
-00001640: 6c66 2e5f 7665 7269 6679 203d 2076 6572  lf._verify = ver
-00001650: 6966 790a 2020 2020 2020 2020 7365 6c66  ify.        self
-00001660: 2e5f 7573 6572 5f61 6765 6e74 203d 2075  ._user_agent = u
-00001670: 7365 725f 6167 656e 740a 0a20 2020 2020  ser_agent..     
-00001680: 2020 2069 6620 7072 6f78 6965 733a 0a20     if proxies:. 
-00001690: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000016a0: 7420 6973 696e 7374 616e 6365 2870 726f  t isinstance(pro
-000016b0: 7869 6573 2c20 6469 6374 293a 0a20 2020  xies, dict):.   
-000016c0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-000016d0: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-000016e0: 6f72 2822 7072 6f78 6965 7320 7061 7261  or("proxies para
-000016f0: 6d65 7465 7220 6d75 7374 2062 6520 6120  meter must be a 
-00001700: 6469 6374 696f 6e61 7279 2e22 290a 2020  dictionary.").  
-00001710: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00001720: 2870 726f 7869 6573 2920 3d3d 2030 3a0a  (proxies) == 0:.
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
-00001750: 4572 726f 7228 2270 726f 7869 6573 2070  Error("proxies p
-00001760: 6172 616d 6574 6572 2063 616e 206e 6f74  arameter can not
-00001770: 2062 6520 616e 2065 6d70 7479 2064 6963   be an empty dic
-00001780: 7469 6f6e 6172 792e 2229 0a20 2020 2020  tionary.").     
-00001790: 2020 2073 656c 662e 5f70 726f 7869 6573     self._proxies
-000017a0: 203d 2070 726f 7869 6573 0a0a 2020 2020   = proxies..    
-000017b0: 2020 2020 6966 206e 6f74 2074 6f6b 656e      if not token
-000017c0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000017d0: 206e 6f74 2075 7365 726e 616d 6520 6f72   not username or
-000017e0: 206e 6f74 2070 6173 7377 6f72 643a 0a20   not password:. 
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001800: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
-00001810: 7272 6f72 2822 4966 2074 6f6b 656e 2069  rror("If token i
-00001820: 7320 6e6f 7420 7072 6f76 6964 6564 2075  s not provided u
-00001830: 7365 726e 616d 6520 616e 6420 7061 7373  sername and pass
-00001840: 776f 7264 2061 7265 2072 6571 7569 7265  word are require
-00001850: 642e 2229 0a20 2020 2020 2020 2020 2020  d.").           
-00001860: 2074 6f6b 656e 203d 2073 656c 662e 5f5f   token = self.__
-00001870: 6765 745f 746f 6b65 6e28 7573 6572 6e61  get_token(userna
-00001880: 6d65 2c20 7061 7373 776f 7264 290a 0a20  me, password).. 
-00001890: 2020 2020 2020 2073 656c 662e 5f68 6561         self._hea
-000018a0: 6465 7273 203d 207b 0a20 2020 2020 2020  ders = {.       
-000018b0: 2020 2020 2022 5573 6572 2d41 6765 6e74       "User-Agent
-000018c0: 223a 2073 656c 662e 5f75 7365 725f 6167  ": self._user_ag
-000018d0: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
-000018e0: 2022 4175 7468 6f72 697a 6174 696f 6e22   "Authorization"
-000018f0: 3a20 2254 6f6b 656e 207b 746f 6b65 6e7d  : "Token {token}
-00001900: 222e 666f 726d 6174 2874 6f6b 656e 3d74  ".format(token=t
-00001910: 6f6b 656e 290a 2020 2020 2020 2020 7d0a  oken).        }.
-00001920: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
-00001930: 656c 6473 203d 2066 6965 6c64 730a 2020  elds = fields.  
-00001940: 2020 2020 2020 7365 6c66 2e5f 6669 656c        self._fiel
-00001950: 6473 5f76 3220 3d20 6669 656c 6473 5f76  ds_v2 = fields_v
-00001960: 320a 2020 2020 2020 2020 7365 6c66 2e5f  2.        self._
-00001970: 7469 636f 7265 5f66 6965 6c64 7320 3d20  ticore_fields = 
-00001980: 7469 636f 7265 5f66 6965 6c64 730a 0a20  ticore_fields.. 
-00001990: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-000019a0: 696e 7374 616e 6365 2877 6169 745f 7469  instance(wait_ti
-000019b0: 6d65 5f73 6563 6f6e 6473 2c20 696e 7429  me_seconds, int)
-000019c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000019d0: 6973 6520 5772 6f6e 6749 6e70 7574 4572  ise WrongInputEr
-000019e0: 726f 7228 2277 6169 745f 7469 6d65 5f73  ror("wait_time_s
-000019f0: 6563 6f6e 6473 206d 7573 7420 6265 2061  econds must be a
-00001a00: 6e20 696e 7465 6765 722e 2229 0a20 2020  n integer.").   
-00001a10: 2020 2020 2073 656c 662e 5f77 6169 745f       self._wait_
-00001a20: 7469 6d65 5f73 6563 6f6e 6473 203d 2077  time_seconds = w
-00001a30: 6169 745f 7469 6d65 5f73 6563 6f6e 6473  ait_time_seconds
-00001a40: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00001a50: 2069 7369 6e73 7461 6e63 6528 7265 7472   isinstance(retr
-00001a60: 6965 732c 2069 6e74 293a 0a20 2020 2020  ies, int):.     
-00001a70: 2020 2020 2020 2072 6169 7365 2057 726f         raise Wro
-00001a80: 6e67 496e 7075 7445 7272 6f72 2822 7265  ngInputError("re
-00001a90: 7472 6965 7320 6d75 7374 2062 6520 616e  tries must be an
-00001aa0: 2069 6e74 6567 6572 2e22 290a 2020 2020   integer.").    
-00001ab0: 2020 2020 7365 6c66 2e5f 7265 7472 6965      self._retrie
-00001ac0: 7320 3d20 7265 7472 6965 730a 0a20 2020  s = retries..   
-00001ad0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-00001ae0: 2020 2064 6566 205f 5f76 616c 6964 6174     def __validat
-00001af0: 655f 686f 7374 2868 6f73 7429 3a0a 2020  e_host(host):.  
-00001b00: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
-00001b10: 2061 2066 6f72 6d61 7474 6564 2068 6f73   a formatted hos
-00001b20: 7420 5552 4c20 696e 636c 7564 696e 6720  t URL including 
-00001b30: 7468 6520 7072 6f74 6f63 6f6c 2070 7265  the protocol pre
-00001b40: 6669 782e 0a20 2020 2020 2020 2020 2020  fix..           
-00001b50: 203a 7061 7261 6d20 686f 7374 3a20 5552   :param host: UR
-00001b60: 4c20 7374 7269 6e67 0a20 2020 2020 2020  L string.       
-00001b70: 2020 2020 203a 7479 7065 2068 6f73 743a       :type host:
-00001b80: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
-00001b90: 203a 7265 7475 726e 733a 2066 6f72 6d61   :returns: forma
-00001ba0: 7474 6564 2055 524c 2073 7472 696e 670a  tted URL string.
-00001bb0: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
-00001bc0: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-00001bd0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-00001be0: 6f74 2069 7369 6e73 7461 6e63 6528 686f  ot isinstance(ho
-00001bf0: 7374 2c20 7374 7229 3a0a 2020 2020 2020  st, str):.      
-00001c00: 2020 2020 2020 7261 6973 6520 5772 6f6e        raise Wron
-00001c10: 6749 6e70 7574 4572 726f 7228 2268 6f73  gInputError("hos
-00001c20: 7420 7061 7261 6d65 7465 7220 6d75 7374  t parameter must
-00001c30: 2062 6520 7374 7269 6e67 2e22 290a 0a20   be string.").. 
-00001c40: 2020 2020 2020 2069 6620 6e6f 7420 686f         if not ho
-00001c50: 7374 2e73 7461 7274 7377 6974 6828 2822  st.startswith(("
-00001c60: 6874 7470 3a2f 2f22 2c20 2268 7474 7073  http://", "https
-00001c70: 3a2f 2f22 2929 3a0a 2020 2020 2020 2020  ://")):.        
-00001c80: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00001c90: 6e70 7574 4572 726f 7228 2268 6f73 7420  nputError("host 
-00001ca0: 7061 7261 6d65 7465 7220 6d75 7374 2063  parameter must c
-00001cb0: 6f6e 7461 696e 2061 2070 726f 746f 636f  ontain a protoco
-00001cc0: 6c20 6465 6669 6e69 7469 6f6e 2061 7420  l definition at 
-00001cd0: 7468 6520 6265 6769 6e6e 696e 672e 2229  the beginning.")
-00001ce0: 0a0a 2020 2020 2020 2020 686f 7374 203d  ..        host =
-00001cf0: 2068 6f73 742e 7273 7472 6970 2822 2f22   host.rstrip("/"
-00001d00: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00001d10: 6e20 686f 7374 0a0a 2020 2020 6465 6620  n host..    def 
-00001d20: 636f 6e66 6967 7572 6174 696f 6e5f 6475  configuration_du
-00001d30: 6d70 2873 656c 6629 3a0a 2020 2020 2020  mp(self):.      
-00001d40: 2020 2222 2252 6574 7572 6e73 2074 6865    """Returns the
-00001d50: 2063 6f6e 6669 6775 7261 7469 6f6e 206f   configuration o
-00001d60: 6620 7468 6520 696e 7374 616e 7469 6174  f the instantiat
-00001d70: 6564 2041 3130 3030 206f 626a 6563 742e  ed A1000 object.
-00001d80: 0a20 2020 2020 2020 2020 2020 203a 7265  .            :re
-00001d90: 7475 726e 3a20 636f 6e66 6967 7572 6174  turn: configurat
-00001da0: 696f 6e20 7374 7269 6e67 0a20 2020 2020  ion string.     
-00001db0: 2020 2020 2020 203a 7274 7970 653a 2073         :rtype: s
-00001dc0: 7472 0a20 2020 2020 2020 2022 2222 0a20  tr.        """. 
-00001dd0: 2020 2020 2020 2063 6f6e 6669 6775 7261         configura
-00001de0: 7469 6f6e 203d 2022 2222 0a20 2020 2020  tion = """.     
-00001df0: 2020 2020 2020 2048 6f73 743a 207b 686f         Host: {ho
-00001e00: 7374 7d0a 2020 2020 2020 2020 2020 2020  st}.            
-00001e10: 5265 706f 7274 2073 756d 6d61 7279 2066  Report summary f
-00001e20: 6965 6c64 733a 207b 6669 656c 6473 7d0a  ields: {fields}.
-00001e30: 2020 2020 2020 2020 2020 2020 5761 6974              Wait
-00001e40: 2074 696d 6520 696e 2073 6563 6f6e 6473   time in seconds
-00001e50: 3a20 7b77 6169 745f 7469 6d65 5f73 6563  : {wait_time_sec
-00001e60: 6f6e 6473 7d0a 2020 2020 2020 2020 2020  onds}.          
-00001e70: 2020 4e75 6d62 6572 206f 6620 7265 7472    Number of retr
-00001e80: 6965 733a 207b 7265 7472 6965 737d 0a20  ies: {retries}. 
-00001e90: 2020 2020 2020 2020 2020 2055 7365 7220             User 
-00001ea0: 6167 656e 743a 207b 7573 6572 5f61 6765  agent: {user_age
-00001eb0: 6e74 7d0a 2020 2020 2020 2020 2020 2020  nt}.            
-00001ec0: 5353 4c20 7665 7269 6679 3a20 7b76 6572  SSL verify: {ver
-00001ed0: 6966 797d 0a20 2020 2020 2020 2022 2222  ify}.        """
-00001ee0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00001ef0: 2020 2020 2068 6f73 743d 7365 6c66 2e5f       host=self._
-00001f00: 686f 7374 2c0a 2020 2020 2020 2020 2020  host,.          
-00001f10: 2020 6669 656c 6473 3d73 656c 662e 5f66    fields=self._f
-00001f20: 6965 6c64 735f 7632 2c0a 2020 2020 2020  ields_v2,.      
-00001f30: 2020 2020 2020 7761 6974 5f74 696d 655f        wait_time_
-00001f40: 7365 636f 6e64 733d 7365 6c66 2e5f 7761  seconds=self._wa
-00001f50: 6974 5f74 696d 655f 7365 636f 6e64 732c  it_time_seconds,
-00001f60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001f70: 7269 6573 3d73 656c 662e 5f72 6574 7269  ries=self._retri
-00001f80: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00001f90: 7573 6572 5f61 6765 6e74 3d73 656c 662e  user_agent=self.
-00001fa0: 5f75 7365 725f 6167 656e 742c 0a20 2020  _user_agent,.   
-00001fb0: 2020 2020 2020 2020 2076 6572 6966 793d           verify=
-00001fc0: 7365 6c66 2e5f 7665 7269 6679 0a20 2020  self._verify.   
-00001fd0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00001fe0: 7265 7475 726e 2063 6f6e 6669 6775 7261  return configura
-00001ff0: 7469 6f6e 0a0a 2020 2020 6465 6620 7465  tion..    def te
-00002000: 7374 5f63 6f6e 6e65 6374 696f 6e28 7365  st_connection(se
-00002010: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00002020: 4372 6561 7465 7320 6120 7265 7175 6573  Creates a reques
-00002030: 7420 746f 7761 7264 7320 7468 6520 4131  t towards the A1
-00002040: 3030 3020 4368 6563 6b20 5374 6174 7573  000 Check Status
-00002050: 2041 5049 2074 6f20 7465 7374 2074 6865   API to test the
-00002060: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
-00002070: 2020 2020 7769 7468 2041 3130 3030 2e0a      with A1000..
-00002080: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00002090: 2020 2020 5f20 3d20 7365 6c66 2e5f 5f61      _ = self.__a
-000020a0: 6e61 6c79 7369 735f 6973 5f66 696e 6973  nalysis_is_finis
-000020b0: 6865 6428 0a20 2020 2020 2020 2020 2020  hed(.           
-000020c0: 2073 616d 706c 655f 6861 7368 6573 3d5b   sample_hashes=[
-000020d0: 2230 3030 3030 3030 3030 3030 3030 3030  "000000000000000
-000020e0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
-000020f0: 3030 3030 3030 3030 3022 5d0a 2020 2020  000000000"].    
-00002100: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
-00002110: 6574 7572 6e0a 0a20 2020 2064 6566 2075  eturn..    def u
-00002120: 706c 6f61 645f 7361 6d70 6c65 5f66 726f  pload_sample_fro
-00002130: 6d5f 7061 7468 2873 656c 662c 2066 696c  m_path(self, fil
-00002140: 655f 7061 7468 2c20 6375 7374 6f6d 5f66  e_path, custom_f
-00002150: 696c 656e 616d 653d 4e6f 6e65 2c20 6172  ilename=None, ar
-00002160: 6368 6976 655f 7061 7373 776f 7264 3d4e  chive_password=N
-00002170: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002190: 2020 2020 2072 6c5f 636c 6f75 645f 7361       rl_cloud_sa
-000021a0: 6e64 626f 785f 706c 6174 666f 726d 3d4e  ndbox_platform=N
-000021b0: 6f6e 652c 2074 6167 733d 4e6f 6e65 2c20  one, tags=None, 
-000021c0: 636f 6d6d 656e 743d 4e6f 6e65 2c20 636c  comment=None, cl
-000021d0: 6f75 645f 616e 616c 7973 6973 3d54 7275  oud_analysis=Tru
-000021e0: 6529 3a0a 2020 2020 2020 2020 2222 2241  e):.        """A
-000021f0: 6363 6570 7473 2061 2066 696c 6520 7061  ccepts a file pa
-00002200: 7468 2073 7472 696e 6720 666f 7220 6669  th string for fi
-00002210: 6c65 2075 706c 6f61 6420 616e 6420 7265  le upload and re
-00002220: 7475 726e 7320 6120 7265 7370 6f6e 7365  turns a response
-00002230: 2e0a 2020 2020 2020 2020 4164 6469 7469  ..        Additi
-00002240: 6f6e 616c 2070 6172 616d 6574 6572 7320  onal parameters 
-00002250: 6361 6e20 6265 2070 726f 7669 6465 642e  can be provided.
-00002260: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-00002270: 7261 6d20 6669 6c65 5f70 6174 683a 2070  ram file_path: p
-00002280: 6174 6820 746f 2066 696c 650a 2020 2020  ath to file.    
-00002290: 2020 2020 2020 2020 3a74 7970 6520 6669          :type fi
-000022a0: 6c65 5f70 6174 683a 2073 7472 0a20 2020  le_path: str.   
-000022b0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-000022c0: 6375 7374 6f6d 5f66 696c 656e 616d 653a  custom_filename:
-000022d0: 2063 7573 746f 6d20 6669 6c65 206e 616d   custom file nam
-000022e0: 6520 666f 7220 7570 6c6f 6164 0a20 2020  e for upload.   
-000022f0: 2020 2020 2020 2020 203a 7479 7065 2063           :type c
-00002300: 7573 746f 6d5f 6669 6c65 6e61 6d65 3a20  ustom_filename: 
-00002310: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-00002320: 3a70 6172 616d 2061 7263 6869 7665 5f70  :param archive_p
-00002330: 6173 7377 6f72 643a 2070 6173 7377 6f72  assword: passwor
-00002340: 642c 2069 6620 6669 6c65 2069 7320 6120  d, if file is a 
-00002350: 7061 7373 776f 7264 2d70 726f 7465 6374  password-protect
-00002360: 6564 2061 7263 6869 7665 0a20 2020 2020  ed archive.     
-00002370: 2020 2020 2020 203a 7479 7065 2061 7263         :type arc
-00002380: 6869 7665 5f70 6173 7377 6f72 643a 2073  hive_password: s
-00002390: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
-000023a0: 7061 7261 6d20 726c 5f63 6c6f 7564 5f73  param rl_cloud_s
-000023b0: 616e 6462 6f78 5f70 6c61 7466 6f72 6d3a  andbox_platform:
-000023c0: 2043 6c6f 7564 2053 616e 6462 6f78 2070   Cloud Sandbox p
-000023d0: 6c61 7466 6f72 6d20 2877 696e 646f 7773  latform (windows
-000023e0: 372c 2077 696e 646f 7773 3130 206f 7220  7, windows10 or 
-000023f0: 6d61 636f 735f 3131 290a 2020 2020 2020  macos_11).      
-00002400: 2020 2020 2020 3a74 7970 6520 726c 5f63        :type rl_c
-00002410: 6c6f 7564 5f73 616e 6462 6f78 5f70 6c61  loud_sandbox_pla
-00002420: 7466 6f72 6d3a 2073 7472 0a20 2020 2020  tform: str.     
-00002430: 2020 2020 2020 203a 7061 7261 6d20 7461         :param ta
-00002440: 6773 3a20 6120 7374 7269 6e67 206f 6620  gs: a string of 
-00002450: 636f 6d6d 6120 7365 7061 7261 7465 6420  comma separated 
-00002460: 7461 6773 0a20 2020 2020 2020 2020 2020  tags.           
-00002470: 203a 7479 7065 2074 6167 733a 2073 7472   :type tags: str
-00002480: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-00002490: 7261 6d20 636f 6d6d 656e 743a 2063 6f6d  ram comment: com
-000024a0: 6d65 6e74 2073 7472 696e 670a 2020 2020  ment string.    
-000024b0: 2020 2020 2020 2020 3a74 7970 6520 636f          :type co
-000024c0: 6d6d 656e 743a 2073 7472 0a20 2020 2020  mment: str.     
-000024d0: 2020 2020 2020 203a 7061 7261 6d20 636c         :param cl
-000024e0: 6f75 645f 616e 616c 7973 6973 3a20 7573  oud_analysis: us
-000024f0: 6520 636c 6f75 6420 616e 616c 7973 6973  e cloud analysis
-00002500: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00002510: 7065 2063 6c6f 7564 5f61 6e61 6c79 7369  pe cloud_analysi
-00002520: 733a 2062 6f6f 6c0a 2020 2020 2020 2020  s: bool.        
-00002530: 2020 2020 3a72 6574 7572 6e3a 203a 636c      :return: :cl
-00002540: 6173 733a 6052 6573 706f 6e73 6520 3c52  ass:`Response <R
-00002550: 6573 706f 6e73 653e 6020 6f62 6a65 6374  esponse>` object
-00002560: 0a20 2020 2020 2020 2020 2020 203a 7274  .            :rt
-00002570: 7970 653a 2072 6571 7565 7374 732e 5265  ype: requests.Re
-00002580: 7370 6f6e 7365 0a20 2020 2020 2020 2022  sponse.        "
-00002590: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-000025a0: 7420 6973 696e 7374 616e 6365 2866 696c  t isinstance(fil
-000025b0: 655f 7061 7468 2c20 7374 7229 3a0a 2020  e_path, str):.  
-000025c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000025d0: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
-000025e0: 2266 696c 655f 7061 7468 206d 7573 7420  "file_path must 
-000025f0: 6265 2061 2073 7472 696e 672e 2229 0a0a  be a string.")..
-00002600: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
-00002610: 656c 662e 5f5f 6372 6561 7465 5f70 6f73  elf.__create_pos
-00002620: 745f 7061 796c 6f61 6428 0a20 2020 2020  t_payload(.     
-00002630: 2020 2020 2020 2063 7573 746f 6d5f 6669         custom_fi
-00002640: 6c65 6e61 6d65 3d63 7573 746f 6d5f 6669  lename=custom_fi
-00002650: 6c65 6e61 6d65 2c0a 2020 2020 2020 2020  lename,.        
-00002660: 2020 2020 6172 6368 6976 655f 7061 7373      archive_pass
-00002670: 776f 7264 3d61 7263 6869 7665 5f70 6173  word=archive_pas
-00002680: 7377 6f72 642c 0a20 2020 2020 2020 2020  sword,.         
-00002690: 2020 2072 6c5f 636c 6f75 645f 7361 6e64     rl_cloud_sand
-000026a0: 626f 785f 706c 6174 666f 726d 3d72 6c5f  box_platform=rl_
-000026b0: 636c 6f75 645f 7361 6e64 626f 785f 706c  cloud_sandbox_pl
-000026c0: 6174 666f 726d 2c0a 2020 2020 2020 2020  atform,.        
-000026d0: 2020 2020 7461 6773 3d74 6167 732c 0a20      tags=tags,. 
-000026e0: 2020 2020 2020 2020 2020 2063 6f6d 6d65             comme
-000026f0: 6e74 3d63 6f6d 6d65 6e74 2c0a 2020 2020  nt=comment,.    
-00002700: 2020 2020 2020 2020 636c 6f75 645f 616e          cloud_an
-00002710: 616c 7973 6973 3d63 6c6f 7564 5f61 6e61  alysis=cloud_ana
-00002720: 6c79 7369 730a 2020 2020 2020 2020 290a  lysis.        ).
-00002730: 0a20 2020 2020 2020 2075 726c 203d 2073  .        url = s
-00002740: 656c 662e 5f75 726c 2e66 6f72 6d61 7428  elf._url.format(
-00002750: 656e 6470 6f69 6e74 3d73 656c 662e 5f5f  endpoint=self.__
-00002760: 5550 4c4f 4144 5f45 4e44 504f 494e 5429  UPLOAD_ENDPOINT)
-00002770: 0a0a 2020 2020 2020 2020 7472 793a 0a20  ..        try:. 
-00002780: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-00002790: 6861 6e64 6c65 203d 206f 7065 6e28 6669  handle = open(fi
-000027a0: 6c65 5f70 6174 682c 2022 7262 2229 0a20  le_path, "rb"). 
-000027b0: 2020 2020 2020 2065 7863 6570 7420 494f         except IO
-000027c0: 4572 726f 7220 6173 2065 7272 6f72 3a0a  Error as error:.
-000027d0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000027e0: 6520 5772 6f6e 6749 6e70 7574 4572 726f  e WrongInputErro
-000027f0: 7228 2245 7272 6f72 2077 6869 6c65 206f  r("Error while o
-00002800: 7065 6e69 6e67 2066 696c 6520 696e 2027  pening file in '
-00002810: 7262 2720 6d6f 6465 202d 207b 6572 726f  rb' mode - {erro
-00002820: 727d 222e 666f 726d 6174 2865 7272 6f72  r}".format(error
-00002830: 3d73 7472 2865 7272 6f72 2929 290a 0a20  =str(error))).. 
-00002840: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00002850: 3d20 7365 6c66 2e5f 5f70 6f73 745f 7265  = self.__post_re
-00002860: 7175 6573 7428 0a20 2020 2020 2020 2020  quest(.         
-00002870: 2020 2075 726c 3d75 726c 2c0a 2020 2020     url=url,.    
-00002880: 2020 2020 2020 2020 6669 6c65 733d 7b22          files={"
-00002890: 6669 6c65 223a 2066 696c 655f 6861 6e64  file": file_hand
-000028a0: 6c65 7d2c 0a20 2020 2020 2020 2020 2020  le},.           
-000028b0: 2064 6174 613d 6461 7461 0a20 2020 2020   data=data.     
-000028c0: 2020 2029 0a0a 2020 2020 2020 2020 7365     )..        se
-000028d0: 6c66 2e5f 5f72 6169 7365 5f6f 6e5f 6572  lf.__raise_on_er
-000028e0: 726f 7228 7265 7370 6f6e 7365 290a 0a20  ror(response).. 
-000028f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00002900: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
-00002910: 7570 6c6f 6164 5f73 616d 706c 655f 6672  upload_sample_fr
-00002920: 6f6d 5f66 696c 6528 7365 6c66 2c20 6669  om_file(self, fi
-00002930: 6c65 5f73 6f75 7263 652c 2063 7573 746f  le_source, custo
-00002940: 6d5f 6669 6c65 6e61 6d65 3d4e 6f6e 652c  m_filename=None,
-00002950: 2061 7263 6869 7665 5f70 6173 7377 6f72   archive_passwor
-00002960: 643d 4e6f 6e65 2c0a 2020 2020 2020 2020  d=None,.        
-00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002980: 2020 2020 2020 2020 726c 5f63 6c6f 7564          rl_cloud
-00002990: 5f73 616e 6462 6f78 5f70 6c61 7466 6f72  _sandbox_platfor
-000029a0: 6d3d 4e6f 6e65 2c20 7461 6773 3d4e 6f6e  m=None, tags=Non
-000029b0: 652c 2063 6f6d 6d65 6e74 3d4e 6f6e 652c  e, comment=None,
-000029c0: 2063 6c6f 7564 5f61 6e61 6c79 7369 733d   cloud_analysis=
-000029d0: 5472 7565 293a 0a20 2020 2020 2020 2022  True):.        "
-000029e0: 2222 4163 6365 7074 7320 616e 206f 7065  ""Accepts an ope
-000029f0: 6e20 6669 6c65 2069 6e20 2772 6227 206d  n file in 'rb' m
-00002a00: 6f64 6520 666f 7220 6669 6c65 2075 706c  ode for file upl
-00002a10: 6f61 6420 616e 6420 7265 7475 726e 7320  oad and returns 
-00002a20: 6120 7265 7370 6f6e 7365 2e0a 2020 2020  a response..    
-00002a30: 2020 2020 4164 6469 7469 6f6e 616c 2070      Additional p
-00002a40: 6172 616d 6574 6572 7320 6361 6e20 6265  arameters can be
-00002a50: 2070 726f 7669 6465 642e 0a20 2020 2020   provided..     
-00002a60: 2020 2020 2020 203a 7061 7261 6d20 6669         :param fi
-00002a70: 6c65 5f73 6f75 7263 653a 206f 7065 6e20  le_source: open 
-00002a80: 6669 6c65 0a20 2020 2020 2020 2020 2020  file.           
-00002a90: 203a 7479 7065 2066 696c 655f 736f 7572   :type file_sour
-00002aa0: 6365 3a20 6669 6c65 206f 7220 4269 6e61  ce: file or Bina
-00002ab0: 7279 494f 0a20 2020 2020 2020 2020 2020  ryIO.           
-00002ac0: 203a 7061 7261 6d20 6375 7374 6f6d 5f66   :param custom_f
-00002ad0: 696c 656e 616d 653a 2063 7573 746f 6d20  ilename: custom 
-00002ae0: 6669 6c65 206e 616d 6520 666f 7220 7570  file name for up
-00002af0: 6c6f 6164 0a20 2020 2020 2020 2020 2020  load.           
-00002b00: 203a 7479 7065 2063 7573 746f 6d5f 6669   :type custom_fi
-00002b10: 6c65 6e61 6d65 3a20 7374 720a 2020 2020  lename: str.    
-00002b20: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
-00002b30: 7263 6869 7665 5f70 6173 7377 6f72 643a  rchive_password:
-00002b40: 2070 6173 7377 6f72 642c 2069 6620 6669   password, if fi
-00002b50: 6c65 2069 7320 6120 7061 7373 776f 7264  le is a password
-00002b60: 2d70 726f 7465 6374 6564 2061 7263 6869  -protected archi
-00002b70: 7665 0a20 2020 2020 2020 2020 2020 203a  ve.            :
-00002b80: 7479 7065 2061 7263 6869 7665 5f70 6173  type archive_pas
-00002b90: 7377 6f72 643a 2073 7472 0a20 2020 2020  sword: str.     
-00002ba0: 2020 2020 2020 203a 7061 7261 6d20 726c         :param rl
-00002bb0: 5f63 6c6f 7564 5f73 616e 6462 6f78 5f70  _cloud_sandbox_p
-00002bc0: 6c61 7466 6f72 6d3a 2043 6c6f 7564 2053  latform: Cloud S
-00002bd0: 616e 6462 6f78 2070 6c61 7466 6f72 6d20  andbox platform 
-00002be0: 2877 696e 646f 7773 372c 2077 696e 646f  (windows7, windo
-00002bf0: 7773 3130 206f 7220 6d61 636f 735f 3131  ws10 or macos_11
-00002c00: 290a 2020 2020 2020 2020 2020 2020 3a74  ).            :t
-00002c10: 7970 6520 726c 5f63 6c6f 7564 5f73 616e  ype rl_cloud_san
-00002c20: 6462 6f78 5f70 6c61 7466 6f72 6d3a 2073  dbox_platform: s
-00002c30: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
-00002c40: 7061 7261 6d20 7461 6773 3a20 6120 7374  param tags: a st
-00002c50: 7269 6e67 206f 6620 636f 6d6d 6120 7365  ring of comma se
-00002c60: 7061 7261 7465 6420 7461 6773 0a20 2020  parated tags.   
-00002c70: 2020 2020 2020 2020 203a 7479 7065 2074           :type t
-00002c80: 6167 733a 2073 7472 0a20 2020 2020 2020  ags: str.       
-00002c90: 2020 2020 203a 7061 7261 6d20 636f 6d6d       :param comm
-00002ca0: 656e 743a 2063 6f6d 6d65 6e74 2073 7472  ent: comment str
-00002cb0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00002cc0: 3a74 7970 6520 636f 6d6d 656e 743a 2073  :type comment: s
-00002cd0: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
-00002ce0: 7061 7261 6d20 636c 6f75 645f 616e 616c  param cloud_anal
-00002cf0: 7973 6973 3a20 7573 6520 636c 6f75 6420  ysis: use cloud 
-00002d00: 616e 616c 7973 6973 0a20 2020 2020 2020  analysis.       
-00002d10: 2020 2020 203a 7479 7065 2063 6c6f 7564       :type cloud
-00002d20: 5f61 6e61 6c79 7369 733a 2062 6f6f 6c0a  _analysis: bool.
-00002d30: 2020 2020 2020 2020 2020 2020 3a72 6574              :ret
-00002d40: 7572 6e3a 203a 636c 6173 733a 6052 6573  urn: :class:`Res
-00002d50: 706f 6e73 6520 3c52 6573 706f 6e73 653e  ponse <Response>
-00002d60: 6020 6f62 6a65 6374 0a20 2020 2020 2020  ` object.       
-00002d70: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
-00002d80: 7565 7374 732e 5265 7370 6f6e 7365 0a20  uests.Response. 
-00002d90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00002da0: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
-00002db0: 7228 6669 6c65 5f73 6f75 7263 652c 2022  r(file_source, "
-00002dc0: 7265 6164 2229 3a0a 2020 2020 2020 2020  read"):.        
-00002dd0: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00002de0: 6e70 7574 4572 726f 7228 2266 696c 655f  nputError("file_
-00002df0: 736f 7572 6365 2070 6172 616d 6574 6572  source parameter
-00002e00: 206d 7573 7420 6265 2061 2066 696c 6520   must be a file 
-00002e10: 6f70 656e 2069 6e20 2772 6227 206d 6f64  open in 'rb' mod
-00002e20: 652e 2229 0a0a 2020 2020 2020 2020 6461  e.")..        da
-00002e30: 7461 203d 2073 656c 662e 5f5f 6372 6561  ta = self.__crea
-00002e40: 7465 5f70 6f73 745f 7061 796c 6f61 6428  te_post_payload(
-00002e50: 0a20 2020 2020 2020 2020 2020 2063 7573  .            cus
-00002e60: 746f 6d5f 6669 6c65 6e61 6d65 3d63 7573  tom_filename=cus
-00002e70: 746f 6d5f 6669 6c65 6e61 6d65 2c0a 2020  tom_filename,.  
-00002e80: 2020 2020 2020 2020 2020 6172 6368 6976            archiv
-00002e90: 655f 7061 7373 776f 7264 3d61 7263 6869  e_password=archi
-00002ea0: 7665 5f70 6173 7377 6f72 642c 0a20 2020  ve_password,.   
-00002eb0: 2020 2020 2020 2020 2072 6c5f 636c 6f75           rl_clou
-00002ec0: 645f 7361 6e64 626f 785f 706c 6174 666f  d_sandbox_platfo
-00002ed0: 726d 3d72 6c5f 636c 6f75 645f 7361 6e64  rm=rl_cloud_sand
-00002ee0: 626f 785f 706c 6174 666f 726d 2c0a 2020  box_platform,.  
-00002ef0: 2020 2020 2020 2020 2020 7461 6773 3d74            tags=t
-00002f00: 6167 732c 0a20 2020 2020 2020 2020 2020  ags,.           
-00002f10: 2063 6f6d 6d65 6e74 3d63 6f6d 6d65 6e74   comment=comment
-00002f20: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
-00002f30: 6f75 645f 616e 616c 7973 6973 3d63 6c6f  oud_analysis=clo
-00002f40: 7564 5f61 6e61 6c79 7369 730a 2020 2020  ud_analysis.    
-00002f50: 2020 2020 290a 0a20 2020 2020 2020 2075      )..        u
-00002f60: 726c 203d 2073 656c 662e 5f75 726c 2e66  rl = self._url.f
-00002f70: 6f72 6d61 7428 656e 6470 6f69 6e74 3d73  ormat(endpoint=s
-00002f80: 656c 662e 5f5f 5550 4c4f 4144 5f45 4e44  elf.__UPLOAD_END
-00002f90: 504f 494e 5429 0a0a 2020 2020 2020 2020  POINT)..        
-00002fa0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-00002fb0: 5f5f 706f 7374 5f72 6571 7565 7374 280a  __post_request(.
-00002fc0: 2020 2020 2020 2020 2020 2020 7572 6c3d              url=
-00002fd0: 7572 6c2c 0a20 2020 2020 2020 2020 2020  url,.           
-00002fe0: 2066 696c 6573 3d7b 2266 696c 6522 3a20   files={"file": 
-00002ff0: 6669 6c65 5f73 6f75 7263 657d 2c0a 2020  file_source},.  
-00003000: 2020 2020 2020 2020 2020 6461 7461 3d64            data=d
-00003010: 6174 610a 2020 2020 2020 2020 290a 0a20  ata.        ).. 
-00003020: 2020 2020 2020 2073 656c 662e 5f5f 7261         self.__ra
-00003030: 6973 655f 6f6e 5f65 7272 6f72 2872 6573  ise_on_error(res
-00003040: 706f 6e73 6529 0a0a 2020 2020 2020 2020  ponse)..        
-00003050: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-00003060: 0a20 2020 2064 6566 2075 706c 6f61 645f  .    def upload_
-00003070: 7361 6d70 6c65 5f66 726f 6d5f 7572 6c28  sample_from_url(
-00003080: 7365 6c66 2c20 6669 6c65 5f75 726c 2c20  self, file_url, 
-00003090: 6372 6177 6c65 723d 4e6f 6e65 2c20 6172  crawler=None, ar
-000030a0: 6368 6976 655f 7061 7373 776f 7264 3d4e  chive_password=N
-000030b0: 6f6e 652c 2072 6c5f 636c 6f75 645f 7361  one, rl_cloud_sa
-000030c0: 6e64 626f 785f 706c 6174 666f 726d 3d4e  ndbox_platform=N
-000030d0: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-000030e0: 2241 6363 6570 7473 2061 2066 696c 6520  "Accepts a file 
-000030f0: 7572 6c20 616e 6420 7265 7475 726e 7320  url and returns 
-00003100: 6120 7265 7370 6f6e 7365 2e0a 2020 2020  a response..    
-00003110: 2020 2020 4164 6469 7469 6f6e 616c 2070      Additional p
-00003120: 6172 616d 6574 6572 7320 6361 6e20 6265  arameters can be
-00003130: 2070 726f 7669 6465 642e 0a20 2020 2020   provided..     
-00003140: 2020 2020 2020 203a 7061 7261 6d20 6669         :param fi
-00003150: 6c65 5f75 726c 3a20 5552 4c20 6672 6f6d  le_url: URL from
-00003160: 2077 6869 6368 2074 6865 2061 7070 6c69   which the appli
-00003170: 616e 6365 2073 686f 756c 6420 646f 776e  ance should down
-00003180: 6c6f 6164 2074 6865 2064 6174 610a 2020  load the data.  
-00003190: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
-000031a0: 6669 6c65 5f75 726c 3a20 7374 720a 2020  file_url: str.  
-000031b0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-000031c0: 2063 7261 776c 6572 3a20 6372 6177 6c65   crawler: crawle
-000031d0: 7220 6d65 7468 6f64 2028 6c6f 6361 6c20  r method (local 
-000031e0: 6f72 2063 6c6f 7564 290a 2020 2020 2020  or cloud).      
-000031f0: 2020 2020 2020 3a74 7970 6520 6372 6177        :type craw
-00003200: 6c65 723a 2073 7472 0a20 2020 2020 2020  ler: str.       
-00003210: 2020 2020 203a 7061 7261 6d20 6172 6368       :param arch
-00003220: 6976 655f 7061 7373 776f 7264 3a20 7061  ive_password: pa
-00003230: 7373 776f 7264 2c20 6966 2066 696c 6520  ssword, if file 
-00003240: 6973 2061 2070 6173 7377 6f72 642d 7072  is a password-pr
-00003250: 6f74 6563 7465 6420 6172 6368 6976 650a  otected archive.
-00003260: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
-00003270: 6520 6172 6368 6976 655f 7061 7373 776f  e archive_passwo
-00003280: 7264 3a20 7374 720a 2020 2020 2020 2020  rd: str.        
-00003290: 2020 2020 3a70 6172 616d 2072 6c5f 636c      :param rl_cl
-000032a0: 6f75 645f 7361 6e64 626f 785f 706c 6174  oud_sandbox_plat
-000032b0: 666f 726d 3a20 436c 6f75 6420 5361 6e64  form: Cloud Sand
-000032c0: 626f 7820 706c 6174 666f 726d 2028 7769  box platform (wi
-000032d0: 6e64 6f77 7337 2c20 7769 6e64 6f77 7331  ndows7, windows1
-000032e0: 3020 6f72 206d 6163 6f73 5f31 3129 0a20  0 or macos_11). 
-000032f0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00003300: 2072 6c5f 636c 6f75 645f 7361 6e64 626f   rl_cloud_sandbo
-00003310: 785f 706c 6174 666f 726d 3a20 7374 720a  x_platform: str.
-00003320: 2020 2020 2020 2020 2020 2020 3a72 6574              :ret
-00003330: 7572 6e3a 203a 636c 6173 733a 6052 6573  urn: :class:`Res
-00003340: 706f 6e73 6520 3c52 6573 706f 6e73 653e  ponse <Response>
-00003350: 6020 6f62 6a65 6374 0a20 2020 2020 2020  ` object.       
-00003360: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
-00003370: 7565 7374 732e 5265 7370 6f6e 7365 0a20  uests.Response. 
-00003380: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00003390: 2020 2020 6461 7461 203d 2073 656c 662e      data = self.
-000033a0: 5f5f 6372 6561 7465 5f70 6f73 745f 7061  __create_post_pa
-000033b0: 796c 6f61 6428 0a20 2020 2020 2020 2020  yload(.         
-000033c0: 2020 2063 7261 776c 6572 3d63 7261 776c     crawler=crawl
-000033d0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-000033e0: 6172 6368 6976 655f 7061 7373 776f 7264  archive_password
-000033f0: 3d61 7263 6869 7665 5f70 6173 7377 6f72  =archive_passwor
-00003400: 642c 0a20 2020 2020 2020 2020 2020 2072  d,.            r
-00003410: 6c5f 636c 6f75 645f 7361 6e64 626f 785f  l_cloud_sandbox_
-00003420: 706c 6174 666f 726d 3d72 6c5f 636c 6f75  platform=rl_clou
-00003430: 645f 7361 6e64 626f 785f 706c 6174 666f  d_sandbox_platfo
-00003440: 726d 2c0a 2020 2020 2020 2020 2020 2020  rm,.            
-00003450: 6669 6c65 5f75 726c 3d66 696c 655f 7572  file_url=file_ur
-00003460: 6c0a 2020 2020 2020 2020 290a 0a20 2020  l.        )..   
-00003470: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
-00003480: 5f75 726c 2e66 6f72 6d61 7428 656e 6470  _url.format(endp
-00003490: 6f69 6e74 3d73 656c 662e 5f5f 5550 4c4f  oint=self.__UPLO
-000034a0: 4144 5f45 4e44 504f 494e 5429 0a0a 2020  AD_ENDPOINT)..  
-000034b0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-000034c0: 2073 656c 662e 5f5f 706f 7374 5f72 6571   self.__post_req
-000034d0: 7565 7374 280a 2020 2020 2020 2020 2020  uest(.          
-000034e0: 2020 7572 6c3d 7572 6c2c 0a20 2020 2020    url=url,.     
-000034f0: 2020 2020 2020 2064 6174 613d 6461 7461         data=data
-00003500: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00003510: 2020 2020 2073 656c 662e 5f5f 7261 6973       self.__rais
-00003520: 655f 6f6e 5f65 7272 6f72 2872 6573 706f  e_on_error(respo
-00003530: 6e73 6529 0a0a 2020 2020 2020 2020 7265  nse)..        re
-00003540: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
-00003550: 2020 2064 6566 2063 6865 636b 5f73 7562     def check_sub
-00003560: 6d69 7474 6564 5f75 726c 5f73 7461 7475  mitted_url_statu
-00003570: 7328 7365 6c66 2c20 7461 736b 5f69 6429  s(self, task_id)
-00003580: 3a0a 2020 2020 2020 2020 2222 2241 6363  :.        """Acc
-00003590: 6570 7473 2061 2074 6173 6b20 4944 2072  epts a task ID r
-000035a0: 6574 7572 6e65 6420 6279 2074 6865 2075  eturned by the u
-000035b0: 706c 6f61 6420 7361 6d70 6c65 2066 726f  pload sample fro
-000035c0: 6d20 7572 6c0a 2020 2020 2020 2020 2020  m url.          
-000035d0: 2020 3a70 6172 616d 2074 6173 6b5f 6964    :param task_id
-000035e0: 3a20 4944 206f 6620 7468 6520 7375 626d  : ID of the subm
-000035f0: 6974 7465 6420 7361 6d70 6c65 0a20 2020  itted sample.   
-00003600: 2020 2020 2020 2020 203a 7479 7065 2074           :type t
-00003610: 6173 6b5f 6964 3a20 7374 720a 2020 2020  ask_id: str.    
-00003620: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00003630: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
-00003640: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
-00003650: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
-00003660: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003670: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-00003680: 7461 6e63 6528 7461 736b 5f69 642c 2073  tance(task_id, s
-00003690: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-000036a0: 2072 6169 7365 2057 726f 6e67 496e 7075   raise WrongInpu
-000036b0: 7445 7272 6f72 2822 7461 736b 5f69 6420  tError("task_id 
-000036c0: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
-000036d0: 6520 6120 7374 7269 6e67 2e22 290a 0a20  e a string.").. 
-000036e0: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
-000036f0: 3d20 7365 6c66 2e5f 5f43 4845 434b 5f55  = self.__CHECK_U
-00003700: 524c 5f53 5441 5455 535f 454e 4450 4f49  RL_STATUS_ENDPOI
-00003710: 4e54 2e66 6f72 6d61 7428 7461 736b 5f69  NT.format(task_i
-00003720: 643d 7461 736b 5f69 6429 0a0a 2020 2020  d=task_id)..    
-00003730: 2020 2020 7572 6c20 3d20 7365 6c66 2e5f      url = self._
-00003740: 7572 6c2e 666f 726d 6174 2865 6e64 706f  url.format(endpo
-00003750: 696e 743d 656e 6470 6f69 6e74 290a 0a20  int=endpoint).. 
-00003760: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00003770: 3d20 7365 6c66 2e5f 5f67 6574 5f72 6571  = self.__get_req
-00003780: 7565 7374 2875 726c 3d75 726c 290a 0a20  uest(url=url).. 
-00003790: 2020 2020 2020 2073 656c 662e 5f5f 7261         self.__ra
-000037a0: 6973 655f 6f6e 5f65 7272 6f72 2872 6573  ise_on_error(res
-000037b0: 706f 6e73 6529 0a0a 2020 2020 2020 2020  ponse)..        
-000037c0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-000037d0: 0a20 2020 2064 6566 2067 6574 5f73 7562  .    def get_sub
-000037e0: 6d69 7474 6564 5f75 726c 5f72 6570 6f72  mitted_url_repor
-000037f0: 7428 7365 6c66 2c20 7461 736b 5f69 642c  t(self, task_id,
-00003800: 2072 6574 7279 293a 0a20 2020 2020 2020   retry):.       
-00003810: 2022 2222 4163 6365 7074 7320 6120 7461   """Accepts a ta
-00003820: 736b 2049 4420 7265 7475 726e 6564 2062  sk ID returned b
-00003830: 7920 7468 6520 7570 6c6f 6164 2073 616d  y the upload sam
-00003840: 706c 6520 6672 6f6d 2075 726c 2061 6e64  ple from url and
-00003850: 2072 6574 7572 6e73 2061 2072 6570 6f72   returns a repor
-00003860: 7420 7265 7370 6f6e 7365 2e0a 2020 2020  t response..    
-00003870: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
-00003880: 636f 6d62 696e 6573 2075 706c 6f61 6469  combines uploadi
-00003890: 6e67 2061 2073 616d 706c 6520 6672 6f6d  ng a sample from
-000038a0: 2075 726c 2061 6e64 206f 6274 6169 6e69   url and obtaini
-000038b0: 6e67 2074 6865 2061 6e61 6c79 7369 7320  ng the analysis 
-000038c0: 7265 706f 7274 2e0a 2020 2020 2020 2020  report..        
-000038d0: 4164 6469 7469 6f6e 616c 2066 6965 6c64  Additional field
-000038e0: 7320 6361 6e20 6265 2070 726f 7669 6465  s can be provide
-000038f0: 642e 0a20 2020 2020 2020 2054 6865 2072  d..        The r
-00003900: 6573 756c 7420 6665 7463 6869 6e67 2061  esult fetching a
-00003910: 6374 696f 6e20 6f66 2074 6869 7320 6d65  ction of this me
-00003920: 7468 6f64 2075 7469 6c69 7a65 7320 7468  thod utilizes th
-00003930: 6520 7365 7420 6e75 6d62 6572 206f 6620  e set number of 
-00003940: 7265 7472 6965 7320 616e 6420 7761 6974  retries and wait
-00003950: 2074 696d 6520 696e 2073 6563 6f6e 6473   time in seconds
-00003960: 2074 6f20 7469 6d65 0a20 2020 2020 2020   to time.       
-00003970: 206f 7574 2069 6620 7468 6520 616e 616c   out if the anal
-00003980: 7973 6973 2072 6573 756c 7473 2061 7265  ysis results are
-00003990: 206e 6f74 2072 6561 6479 2e0a 2020 2020   not ready..    
-000039a0: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-000039b0: 6173 6b5f 6964 3a20 4944 206f 6620 7468  ask_id: ID of th
-000039c0: 6520 7375 626d 6974 7465 6420 7361 6d70  e submitted samp
-000039d0: 6c65 0a20 2020 2020 2020 2020 2020 203a  le.            :
-000039e0: 7479 7065 2074 6173 6b5f 6964 3a20 7374  type task_id: st
-000039f0: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
-00003a00: 6172 616d 2072 6574 7279 3a20 6966 2073  aram retry: if s
-00003a10: 6574 2074 6f20 4661 6c73 6520 7468 6572  et to False ther
-00003a20: 6520 7769 6c6c 206f 6e6c 7920 6265 206f  e will only be o
-00003a30: 6e65 2074 7279 2061 7420 6f62 7461 696e  ne try at obtain
-00003a40: 696e 6720 7468 6520 616e 616c 7973 6973  ing the analysis
-00003a50: 2072 6570 6f72 740a 2020 2020 2020 2020   report.        
-00003a60: 2020 2020 3a74 7970 6520 7265 7472 793a      :type retry:
-00003a70: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
-00003a80: 2020 3a72 6574 7572 6e3a 2072 6573 706f    :return: respo
-00003a90: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
-00003aa0: 3a72 7479 7065 3a20 7265 7175 6573 7473  :rtype: requests
-00003ab0: 2e52 6573 706f 6e73 650a 2020 2020 2020  .Response.      
-00003ac0: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
-00003ad0: 6620 7265 7472 7920 6e6f 7420 696e 2028  f retry not in (
-00003ae0: 5472 7565 2c20 4661 6c73 6529 3a0a 2020  True, False):.  
-00003af0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00003b00: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
-00003b10: 2272 6574 7279 2070 6172 616d 6574 6572  "retry parameter
-00003b20: 206d 7573 7420 6265 2062 6f6f 6c65 616e   must be boolean
-00003b30: 2e22 290a 0a20 2020 2020 2020 2072 6574  .")..        ret
-00003b40: 7269 6573 203d 2073 656c 662e 5f72 6574  ries = self._ret
-00003b50: 7269 6573 2069 6620 7265 7472 7920 656c  ries if retry el
-00003b60: 7365 2030 0a0a 2020 2020 2020 2020 666f  se 0..        fo
-00003b70: 7220 6974 6572 6174 696f 6e20 696e 2072  r iteration in r
-00003b80: 616e 6765 2872 6574 7269 6573 202b 2031  ange(retries + 1
-00003b90: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00003ba0: 6620 6974 6572 6174 696f 6e3a 0a20 2020  f iteration:.   
-00003bb0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00003bc0: 652e 736c 6565 7028 7365 6c66 2e5f 7761  e.sleep(self._wa
-00003bd0: 6974 5f74 696d 655f 7365 636f 6e64 7329  it_time_seconds)
-00003be0: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00003bf0: 7370 6f6e 7365 203d 2073 656c 662e 6368  sponse = self.ch
-00003c00: 6563 6b5f 7375 626d 6974 7465 645f 7572  eck_submitted_ur
-00003c10: 6c5f 7374 6174 7573 2874 6173 6b5f 6964  l_status(task_id
-00003c20: 3d74 6173 6b5f 6964 290a 2020 2020 2020  =task_id).      
-00003c30: 2020 2020 2020 7374 6174 7573 203d 2072        status = r
-00003c40: 6573 706f 6e73 652e 6a73 6f6e 2829 2e67  esponse.json().g
-00003c50: 6574 2822 7072 6f63 6573 7369 6e67 5f73  et("processing_s
-00003c60: 7461 7475 7322 290a 0a20 2020 2020 2020  tatus")..       
-00003c70: 2020 2020 2069 6620 7374 6174 7573 203d       if status =
-00003c80: 3d20 2265 7272 6f72 223a 0a20 2020 2020  = "error":.     
-00003c90: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00003ca0: 2045 7863 6570 7469 6f6e 2872 6573 706f   Exception(respo
-00003cb0: 6e73 652e 6a73 6f6e 2829 2e67 6574 2822  nse.json().get("
-00003cc0: 6d65 7373 6167 6522 2929 0a0a 2020 2020  message"))..    
-00003cd0: 2020 2020 2020 2020 6966 2073 7461 7475          if statu
-00003ce0: 7320 3d3d 2022 636f 6d70 6c65 7465 223a  s == "complete":
-00003cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d00: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00003d10: 0a0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
-00003d20: 5265 7175 6573 7454 696d 656f 7574 4572  RequestTimeoutEr
-00003d30: 726f 7228 2252 6570 6f72 7420 6665 7463  ror("Report fetc
-00003d40: 6869 6e67 2061 7474 656d 7074 7320 6669  hing attempts fi
-00003d50: 6e69 7368 6564 202d 2054 6865 2061 6e61  nished - The ana
-00003d60: 6c79 7369 7320 7265 706f 7274 2069 7320  lysis report is 
-00003d70: 7374 696c 6c20 6e6f 7420 7265 6164 7920  still not ready 
-00003d80: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 2020 2020 226f 7220 7468 6520 7361 6d70      "or the samp
-00003db0: 6c65 2064 6f65 7320 6e6f 7420 6578 6973  le does not exis
-00003dc0: 7420 6f6e 2074 6865 2061 7070 6c69 616e  t on the applian
-00003dd0: 6365 2e22 290a 0a20 2020 2064 6566 2075  ce.")..    def u
-00003de0: 706c 6f61 645f 7361 6d70 6c65 5f66 726f  pload_sample_fro
-00003df0: 6d5f 7572 6c5f 616e 645f 6765 745f 7265  m_url_and_get_re
-00003e00: 706f 7274 2873 656c 662c 2066 696c 655f  port(self, file_
-00003e10: 7572 6c2c 2072 6574 7279 3d54 7275 652c  url, retry=True,
-00003e20: 2063 7261 776c 6572 3d22 6c6f 6361 6c22   crawler="local"
-00003e30: 2c20 6172 6368 6976 655f 7061 7373 776f  , archive_passwo
-00003e40: 7264 3d4e 6f6e 652c 0a20 2020 2020 2020  rd=None,.       
-00003e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e70: 2020 2020 2020 2072 6c5f 636c 6f75 645f         rl_cloud_
-00003e80: 7361 6e64 626f 785f 706c 6174 666f 726d  sandbox_platform
-00003e90: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00003ea0: 2222 2241 6363 6570 7473 2061 2066 696c  """Accepts a fil
-00003eb0: 6520 7572 6c20 666f 7220 6669 6c65 2075  e url for file u
-00003ec0: 706c 6f61 6420 616e 6420 7265 7475 726e  pload and return
-00003ed0: 7320 6120 7265 706f 7274 2072 6573 706f  s a report respo
-00003ee0: 6e73 652e 0a20 2020 2020 2020 2054 6869  nse..        Thi
-00003ef0: 7320 6d65 7468 6f64 2063 6f6d 6269 6e65  s method combine
-00003f00: 7320 7570 6c6f 6164 696e 6720 6120 7361  s uploading a sa
-00003f10: 6d70 6c65 2066 726f 6d20 7572 6c20 616e  mple from url an
-00003f20: 6420 6f62 7461 696e 696e 6720 7468 6520  d obtaining the 
-00003f30: 7375 6d6d 6172 7920 616e 616c 7973 6973  summary analysis
-00003f40: 2072 6570 6f72 742e 0a20 2020 2020 2020   report..       
-00003f50: 2041 6464 6974 696f 6e61 6c20 6669 656c   Additional fiel
-00003f60: 6473 2063 616e 2062 6520 7072 6f76 6964  ds can be provid
-00003f70: 6564 2e0a 2020 2020 2020 2020 5468 6520  ed..        The 
-00003f80: 7265 7375 6c74 2066 6574 6368 696e 6720  result fetching 
-00003f90: 6163 7469 6f6e 206f 6620 7468 6973 206d  action of this m
-00003fa0: 6574 686f 6420 7574 696c 697a 6573 2074  ethod utilizes t
-00003fb0: 6865 2073 6574 206e 756d 6265 7220 6f66  he set number of
-00003fc0: 2072 6574 7269 6573 2061 6e64 2077 6169   retries and wai
-00003fd0: 7420 7469 6d65 2069 6e20 7365 636f 6e64  t time in second
-00003fe0: 7320 746f 2074 696d 650a 2020 2020 2020  s to time.      
-00003ff0: 2020 6f75 7420 6966 2074 6865 2061 6e61    out if the ana
-00004000: 6c79 7369 7320 7265 7375 6c74 7320 6172  lysis results ar
-00004010: 6520 6e6f 7420 7265 6164 792e 0a20 2020  e not ready..   
-00004020: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00004030: 6669 6c65 5f75 726c 3a20 5552 4c20 6672  file_url: URL fr
-00004040: 6f6d 2077 6869 6368 2074 6865 2061 7070  om which the app
-00004050: 6c69 616e 6365 2073 686f 756c 6420 646f  liance should do
-00004060: 776e 6c6f 6164 2074 6865 2064 6174 610a  wnload the data.
-00004070: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
-00004080: 6520 6669 6c65 5f75 726c 3a20 7374 720a  e file_url: str.
-00004090: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-000040a0: 616d 2072 6574 7279 3a20 6966 2073 6574  am retry: if set
-000040b0: 2074 6f20 4661 6c73 6520 7468 6572 6520   to False there 
-000040c0: 7769 6c6c 206f 6e6c 7920 6265 206f 6e65  will only be one
-000040d0: 2074 7279 2061 7420 6f62 7461 696e 696e   try at obtainin
-000040e0: 6720 7468 6520 616e 616c 7973 6973 2072  g the analysis r
-000040f0: 6570 6f72 740a 2020 2020 2020 2020 2020  eport.          
-00004100: 2020 3a74 7970 6520 7265 7472 793a 2062    :type retry: b
-00004110: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-00004120: 3a70 6172 616d 2063 7261 776c 6572 3a20  :param crawler: 
-00004130: 6372 6177 6c65 7220 6d65 7468 6f64 2028  crawler method (
-00004140: 6c6f 6361 6c20 6f72 2063 6c6f 7564 290a  local or cloud).
-00004150: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
-00004160: 6520 6372 6177 6c65 723a 2073 7472 696e  e crawler: strin
-00004170: 670a 2020 2020 2020 2020 2020 2020 3a70  g.            :p
-00004180: 6172 616d 2061 7263 6869 7665 5f70 6173  aram archive_pas
-00004190: 7377 6f72 643a 2070 6173 7377 6f72 642c  sword: password,
-000041a0: 2069 6620 6669 6c65 2069 7320 6120 7061   if file is a pa
-000041b0: 7373 776f 7264 2d70 726f 7465 6374 6564  ssword-protected
-000041c0: 2061 7263 6869 7665 0a20 2020 2020 2020   archive.       
-000041d0: 2020 2020 203a 7479 7065 2061 7263 6869       :type archi
-000041e0: 7665 5f70 6173 7377 6f72 643a 2073 7472  ve_password: str
-000041f0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-00004200: 7261 6d20 726c 5f63 6c6f 7564 5f73 616e  ram rl_cloud_san
-00004210: 6462 6f78 5f70 6c61 7466 6f72 6d3a 2043  dbox_platform: C
-00004220: 6c6f 7564 2053 616e 6462 6f78 2070 6c61  loud Sandbox pla
-00004230: 7466 6f72 6d20 2877 696e 646f 7773 372c  tform (windows7,
-00004240: 2077 696e 646f 7773 3130 206f 7220 6d61   windows10 or ma
-00004250: 636f 735f 3131 290a 2020 2020 2020 2020  cos_11).        
-00004260: 2020 2020 3a74 7970 6520 726c 5f63 6c6f      :type rl_clo
-00004270: 7564 5f73 616e 6462 6f78 5f70 6c61 7466  ud_sandbox_platf
-00004280: 6f72 6d3a 2073 7472 0a20 2020 2020 2020  orm: str.       
-00004290: 2020 2020 203a 7265 7475 726e 3a20 3a63       :return: :c
-000042a0: 6c61 7373 3a60 5265 7370 6f6e 7365 203c  lass:`Response <
-000042b0: 5265 7370 6f6e 7365 3e60 206f 626a 6563  Response>` objec
-000042c0: 740a 2020 2020 2020 2020 2020 2020 3a72  t.            :r
-000042d0: 7479 7065 3a20 7265 7175 6573 7473 2e52  type: requests.R
-000042e0: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-000042f0: 2222 220a 0a20 2020 2020 2020 2075 706c  """..        upl
-00004300: 6f61 645f 7265 7370 6f6e 7365 203d 2073  oad_response = s
-00004310: 656c 662e 7570 6c6f 6164 5f73 616d 706c  elf.upload_sampl
-00004320: 655f 6672 6f6d 5f75 726c 2866 696c 655f  e_from_url(file_
-00004330: 7572 6c3d 6669 6c65 5f75 726c 2c20 6372  url=file_url, cr
-00004340: 6177 6c65 723d 6372 6177 6c65 722c 0a20  awler=crawler,. 
-00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004380: 2020 2020 2061 7263 6869 7665 5f70 6173       archive_pas
-00004390: 7377 6f72 643d 6172 6368 6976 655f 7061  sword=archive_pa
-000043a0: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
+000012a0: 6f72 6967 696e 222c 2022 636c 6173 7369  origin", "classi
+000012b0: 6669 6361 7469 6f6e 5f72 6561 736f 6e22  fication_reason"
+000012c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000012d0: 2020 2020 2022 636c 6173 7369 6669 6361       "classifica
+000012e0: 7469 6f6e 5f73 6f75 7263 6522 2c20 2263  tion_source", "c
+000012f0: 6c61 7373 6966 6963 6174 696f 6e22 2c20  lassification", 
+00001300: 2272 6973 6b73 636f 7265 222c 2022 636c  "riskscore", "cl
+00001310: 6173 7369 6669 6361 7469 6f6e 5f72 6573  assification_res
+00001320: 756c 7422 2c20 2274 6963 6f72 6522 2c20  ult", "ticore", 
+00001330: 2274 6167 7322 2c0a 2020 2020 2020 2020  "tags",.        
+00001340: 2020 2020 2020 2020 2020 2022 7375 6d6d             "summ
+00001350: 6172 7922 2c20 2274 6963 6c6f 7564 222c  ary", "ticloud",
+00001360: 2022 616c 6961 7365 7322 2c20 226e 6574   "aliases", "net
+00001370: 776f 726b 7468 7265 6174 696e 7465 6c6c  workthreatintell
+00001380: 6967 656e 6365 222c 2022 646f 6d61 696e  igence", "domain
+00001390: 7468 7265 6174 696e 7465 6c6c 6967 656e  threatintelligen
+000013a0: 6365 220a 2020 2020 2020 2020 2020 2020  ce".            
+000013b0: 2020 2020 2020 2029 0a0a 2020 2020 5f5f         )..    __
+000013c0: 5449 5441 4e49 554d 5f43 4f52 455f 4649  TITANIUM_CORE_FI
+000013d0: 454c 4453 203d 2022 7368 6131 2c20 7368  ELDS = "sha1, sh
+000013e0: 6132 3536 2c20 7368 6135 3132 2c20 6d64  a256, sha512, md
+000013f0: 352c 2069 6d70 6861 7368 2c20 696e 666f  5, imphash, info
+00001400: 2c20 6170 706c 6963 6174 696f 6e2c 2070  , application, p
+00001410: 726f 7465 6374 696f 6e2c 2073 6563 7572  rotection, secur
+00001420: 6974 792c 2062 6568 6176 696f 7572 2c22  ity, behaviour,"
+00001430: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 2220 6365 7274 6966 6963 6174 652c 2064  " certificate, d
+00001460: 6f63 756d 656e 742c 206d 6f62 696c 652c  ocument, mobile,
+00001470: 206d 6564 6961 2c20 7765 622c 2065 6d61   media, web, ema
+00001480: 696c 2c20 7374 7269 6e67 732c 2069 6e74  il, strings, int
+00001490: 6572 6573 7469 6e67 5f73 7472 696e 6773  eresting_strings
+000014a0: 2c22 205c 0a20 2020 2020 2020 2020 2020  ," \.           
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2220 636c 6173 7369 6669 6361 7469    " classificati
+000014d0: 6f6e 2c20 696e 6469 6361 746f 7273 2c20  on, indicators, 
+000014e0: 7461 6773 2c20 6174 7461 636b 2c20 7374  tags, attack, st
+000014f0: 6f72 7922 0a0a 2020 2020 6465 6620 5f5f  ory"..    def __
+00001500: 696e 6974 5f5f 2873 656c 662c 2068 6f73  init__(self, hos
+00001510: 742c 2075 7365 726e 616d 653d 4e6f 6e65  t, username=None
+00001520: 2c20 7061 7373 776f 7264 3d4e 6f6e 652c  , password=None,
+00001530: 2074 6f6b 656e 3d4e 6f6e 652c 2066 6965   token=None, fie
+00001540: 6c64 733d 5f5f 4649 454c 4453 2c20 6669  lds=__FIELDS, fi
+00001550: 656c 6473 5f76 323d 5f5f 4649 454c 4453  elds_v2=__FIELDS
+00001560: 5f56 322c 0a20 2020 2020 2020 2020 2020  _V2,.           
+00001570: 2020 2020 2020 7469 636f 7265 5f66 6965        ticore_fie
+00001580: 6c64 733d 5f5f 5449 5441 4e49 554d 5f43  lds=__TITANIUM_C
+00001590: 4f52 455f 4649 454c 4453 2c20 7761 6974  ORE_FIELDS, wait
+000015a0: 5f74 696d 655f 7365 636f 6e64 733d 322c  _time_seconds=2,
+000015b0: 2072 6574 7269 6573 3d31 302c 2076 6572   retries=10, ver
+000015c0: 6966 793d 5472 7565 2c20 7072 6f78 6965  ify=True, proxie
+000015d0: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+000015e0: 2020 2020 2020 2020 2075 7365 725f 6167           user_ag
+000015f0: 656e 743d 4445 4641 554c 545f 5553 4552  ent=DEFAULT_USER
+00001600: 5f41 4745 4e54 293a 0a0a 2020 2020 2020  _AGENT):..      
+00001610: 2020 7365 6c66 2e5f 686f 7374 203d 2073    self._host = s
+00001620: 656c 662e 5f5f 7661 6c69 6461 7465 5f68  elf.__validate_h
+00001630: 6f73 7428 686f 7374 290a 2020 2020 2020  ost(host).      
+00001640: 2020 7365 6c66 2e5f 7572 6c20 3d20 227b    self._url = "{
+00001650: 686f 7374 7d7b 7b65 6e64 706f 696e 747d  host}{{endpoint}
+00001660: 7d22 2e66 6f72 6d61 7428 686f 7374 3d73  }".format(host=s
+00001670: 656c 662e 5f68 6f73 7429 0a20 2020 2020  elf._host).     
+00001680: 2020 2073 656c 662e 5f76 6572 6966 7920     self._verify 
+00001690: 3d20 7665 7269 6679 0a20 2020 2020 2020  = verify.       
+000016a0: 2073 656c 662e 5f75 7365 725f 6167 656e   self._user_agen
+000016b0: 7420 3d20 7573 6572 5f61 6765 6e74 0a0a  t = user_agent..
+000016c0: 2020 2020 2020 2020 6966 2070 726f 7869          if proxi
+000016d0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+000016e0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+000016f0: 6528 7072 6f78 6965 732c 2064 6963 7429  e(proxies, dict)
+00001700: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001710: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+00001720: 7574 4572 726f 7228 2270 726f 7869 6573  utError("proxies
+00001730: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
+00001740: 6265 2061 2064 6963 7469 6f6e 6172 792e  be a dictionary.
+00001750: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+00001760: 6620 6c65 6e28 7072 6f78 6965 7329 203d  f len(proxies) =
+00001770: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00001780: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
+00001790: 496e 7075 7445 7272 6f72 2822 7072 6f78  InputError("prox
+000017a0: 6965 7320 7061 7261 6d65 7465 7220 6361  ies parameter ca
+000017b0: 6e20 6e6f 7420 6265 2061 6e20 656d 7074  n not be an empt
+000017c0: 7920 6469 6374 696f 6e61 7279 2e22 290a  y dictionary.").
+000017d0: 2020 2020 2020 2020 7365 6c66 2e5f 7072          self._pr
+000017e0: 6f78 6965 7320 3d20 7072 6f78 6965 730a  oxies = proxies.
+000017f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00001800: 746f 6b65 6e3a 0a20 2020 2020 2020 2020  token:.         
+00001810: 2020 2069 6620 6e6f 7420 7573 6572 6e61     if not userna
+00001820: 6d65 206f 7220 6e6f 7420 7061 7373 776f  me or not passwo
+00001830: 7264 3a0a 2020 2020 2020 2020 2020 2020  rd:.            
+00001840: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
+00001850: 6e70 7574 4572 726f 7228 2249 6620 746f  nputError("If to
+00001860: 6b65 6e20 6973 206e 6f74 2070 726f 7669  ken is not provi
+00001870: 6465 6420 7573 6572 6e61 6d65 2061 6e64  ded username and
+00001880: 2070 6173 7377 6f72 6420 6172 6520 7265   password are re
+00001890: 7175 6972 6564 2e22 290a 2020 2020 2020  quired.").      
+000018a0: 2020 2020 2020 746f 6b65 6e20 3d20 7365        token = se
+000018b0: 6c66 2e5f 5f67 6574 5f74 6f6b 656e 2875  lf.__get_token(u
+000018c0: 7365 726e 616d 652c 2070 6173 7377 6f72  sername, passwor
+000018d0: 6429 0a0a 2020 2020 2020 2020 7365 6c66  d)..        self
+000018e0: 2e5f 6865 6164 6572 7320 3d20 7b0a 2020  ._headers = {.  
+000018f0: 2020 2020 2020 2020 2020 2255 7365 722d            "User-
+00001900: 4167 656e 7422 3a20 7365 6c66 2e5f 7573  Agent": self._us
+00001910: 6572 5f61 6765 6e74 2c0a 2020 2020 2020  er_agent,.      
+00001920: 2020 2020 2020 2241 7574 686f 7269 7a61        "Authoriza
+00001930: 7469 6f6e 223a 2022 546f 6b65 6e20 7b74  tion": "Token {t
+00001940: 6f6b 656e 7d22 2e66 6f72 6d61 7428 746f  oken}".format(to
+00001950: 6b65 6e3d 746f 6b65 6e29 0a20 2020 2020  ken=token).     
+00001960: 2020 207d 0a20 2020 2020 2020 2073 656c     }.        sel
+00001970: 662e 5f66 6965 6c64 7320 3d20 6669 656c  f._fields = fiel
+00001980: 6473 0a20 2020 2020 2020 2073 656c 662e  ds.        self.
+00001990: 5f66 6965 6c64 735f 7632 203d 2066 6965  _fields_v2 = fie
+000019a0: 6c64 735f 7632 0a20 2020 2020 2020 2073  lds_v2.        s
+000019b0: 656c 662e 5f74 6963 6f72 655f 6669 656c  elf._ticore_fiel
+000019c0: 6473 203d 2074 6963 6f72 655f 6669 656c  ds = ticore_fiel
+000019d0: 6473 0a0a 2020 2020 2020 2020 6966 206e  ds..        if n
+000019e0: 6f74 2069 7369 6e73 7461 6e63 6528 7761  ot isinstance(wa
+000019f0: 6974 5f74 696d 655f 7365 636f 6e64 732c  it_time_seconds,
+00001a00: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
+00001a10: 2020 2072 6169 7365 2057 726f 6e67 496e     raise WrongIn
+00001a20: 7075 7445 7272 6f72 2822 7761 6974 5f74  putError("wait_t
+00001a30: 696d 655f 7365 636f 6e64 7320 6d75 7374  ime_seconds must
+00001a40: 2062 6520 616e 2069 6e74 6567 6572 2e22   be an integer."
+00001a50: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+00001a60: 7761 6974 5f74 696d 655f 7365 636f 6e64  wait_time_second
+00001a70: 7320 3d20 7761 6974 5f74 696d 655f 7365  s = wait_time_se
+00001a80: 636f 6e64 730a 0a20 2020 2020 2020 2069  conds..        i
+00001a90: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00001aa0: 2872 6574 7269 6573 2c20 696e 7429 3a0a  (retries, int):.
+00001ab0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00001ac0: 6520 5772 6f6e 6749 6e70 7574 4572 726f  e WrongInputErro
+00001ad0: 7228 2272 6574 7269 6573 206d 7573 7420  r("retries must 
+00001ae0: 6265 2061 6e20 696e 7465 6765 722e 2229  be an integer.")
+00001af0: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+00001b00: 6574 7269 6573 203d 2072 6574 7269 6573  etries = retries
+00001b10: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00001b20: 686f 640a 2020 2020 6465 6620 5f5f 7661  hod.    def __va
+00001b30: 6c69 6461 7465 5f68 6f73 7428 686f 7374  lidate_host(host
+00001b40: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+00001b50: 7475 726e 7320 6120 666f 726d 6174 7465  turns a formatte
+00001b60: 6420 686f 7374 2055 524c 2069 6e63 6c75  d host URL inclu
+00001b70: 6469 6e67 2074 6865 2070 726f 746f 636f  ding the protoco
+00001b80: 6c20 7072 6566 6978 2e0a 2020 2020 2020  l prefix..      
+00001b90: 2020 2020 2020 3a70 6172 616d 2068 6f73        :param hos
+00001ba0: 743a 2055 524c 2073 7472 696e 670a 2020  t: URL string.  
+00001bb0: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00001bc0: 686f 7374 3a20 7374 720a 2020 2020 2020  host: str.      
+00001bd0: 2020 2020 2020 3a72 6574 7572 6e73 3a20        :returns: 
+00001be0: 666f 726d 6174 7465 6420 5552 4c20 7374  formatted URL st
+00001bf0: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+00001c00: 203a 7274 7970 653a 2073 7472 0a20 2020   :rtype: str.   
+00001c10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00001c20: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+00001c30: 6365 2868 6f73 742c 2073 7472 293a 0a20  ce(host, str):. 
+00001c40: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00001c50: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
+00001c60: 2822 686f 7374 2070 6172 616d 6574 6572  ("host parameter
+00001c70: 206d 7573 7420 6265 2073 7472 696e 672e   must be string.
+00001c80: 2229 0a0a 2020 2020 2020 2020 6966 206e  ")..        if n
+00001c90: 6f74 2068 6f73 742e 7374 6172 7473 7769  ot host.startswi
+00001ca0: 7468 2828 2268 7474 703a 2f2f 222c 2022  th(("http://", "
+00001cb0: 6874 7470 733a 2f2f 2229 293a 0a20 2020  https://")):.   
+00001cc0: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+00001cd0: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+00001ce0: 686f 7374 2070 6172 616d 6574 6572 206d  host parameter m
+00001cf0: 7573 7420 636f 6e74 6169 6e20 6120 7072  ust contain a pr
+00001d00: 6f74 6f63 6f6c 2064 6566 696e 6974 696f  otocol definitio
+00001d10: 6e20 6174 2074 6865 2062 6567 696e 6e69  n at the beginni
+00001d20: 6e67 2e22 290a 0a20 2020 2020 2020 2068  ng.")..        h
+00001d30: 6f73 7420 3d20 686f 7374 2e72 7374 7269  ost = host.rstri
+00001d40: 7028 222f 2229 0a0a 2020 2020 2020 2020  p("/")..        
+00001d50: 7265 7475 726e 2068 6f73 740a 0a20 2020  return host..   
+00001d60: 2064 6566 2063 6f6e 6669 6775 7261 7469   def configurati
+00001d70: 6f6e 5f64 756d 7028 7365 6c66 293a 0a20  on_dump(self):. 
+00001d80: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+00001d90: 7320 7468 6520 636f 6e66 6967 7572 6174  s the configurat
+00001da0: 696f 6e20 6f66 2074 6865 2069 6e73 7461  ion of the insta
+00001db0: 6e74 6961 7465 6420 4131 3030 3020 6f62  ntiated A1000 ob
+00001dc0: 6a65 6374 2e0a 2020 2020 2020 2020 2020  ject..          
+00001dd0: 2020 3a72 6574 7572 6e3a 2063 6f6e 6669    :return: confi
+00001de0: 6775 7261 7469 6f6e 2073 7472 696e 670a  guration string.
+00001df0: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
+00001e00: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
+00001e10: 2222 220a 2020 2020 2020 2020 636f 6e66  """.        conf
+00001e20: 6967 7572 6174 696f 6e20 3d20 2222 220a  iguration = """.
+00001e30: 2020 2020 2020 2020 2020 2020 486f 7374              Host
+00001e40: 3a20 7b68 6f73 747d 0a20 2020 2020 2020  : {host}.       
+00001e50: 2020 2020 2052 6570 6f72 7420 7375 6d6d       Report summ
+00001e60: 6172 7920 6669 656c 6473 3a20 7b66 6965  ary fields: {fie
+00001e70: 6c64 737d 0a20 2020 2020 2020 2020 2020  lds}.           
+00001e80: 2057 6169 7420 7469 6d65 2069 6e20 7365   Wait time in se
+00001e90: 636f 6e64 733a 207b 7761 6974 5f74 696d  conds: {wait_tim
+00001ea0: 655f 7365 636f 6e64 737d 0a20 2020 2020  e_seconds}.     
+00001eb0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+00001ec0: 2072 6574 7269 6573 3a20 7b72 6574 7269   retries: {retri
+00001ed0: 6573 7d0a 2020 2020 2020 2020 2020 2020  es}.            
+00001ee0: 5573 6572 2061 6765 6e74 3a20 7b75 7365  User agent: {use
+00001ef0: 725f 6167 656e 747d 0a20 2020 2020 2020  r_agent}.       
+00001f00: 2020 2020 2053 534c 2076 6572 6966 793a       SSL verify:
+00001f10: 207b 7665 7269 6679 7d0a 2020 2020 2020   {verify}.      
+00001f20: 2020 2222 222e 666f 726d 6174 280a 2020    """.format(.  
+00001f30: 2020 2020 2020 2020 2020 686f 7374 3d73            host=s
+00001f40: 656c 662e 5f68 6f73 742c 0a20 2020 2020  elf._host,.     
+00001f50: 2020 2020 2020 2066 6965 6c64 733d 7365         fields=se
+00001f60: 6c66 2e5f 6669 656c 6473 5f76 322c 0a20  lf._fields_v2,. 
+00001f70: 2020 2020 2020 2020 2020 2077 6169 745f             wait_
+00001f80: 7469 6d65 5f73 6563 6f6e 6473 3d73 656c  time_seconds=sel
+00001f90: 662e 5f77 6169 745f 7469 6d65 5f73 6563  f._wait_time_sec
+00001fa0: 6f6e 6473 2c0a 2020 2020 2020 2020 2020  onds,.          
+00001fb0: 2020 7265 7472 6965 733d 7365 6c66 2e5f    retries=self._
+00001fc0: 7265 7472 6965 732c 0a20 2020 2020 2020  retries,.       
+00001fd0: 2020 2020 2075 7365 725f 6167 656e 743d       user_agent=
+00001fe0: 7365 6c66 2e5f 7573 6572 5f61 6765 6e74  self._user_agent
+00001ff0: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+00002000: 7269 6679 3d73 656c 662e 5f76 6572 6966  rify=self._verif
+00002010: 790a 2020 2020 2020 2020 290a 0a20 2020  y.        )..   
+00002020: 2020 2020 2072 6574 7572 6e20 636f 6e66       return conf
+00002030: 6967 7572 6174 696f 6e0a 0a20 2020 2064  iguration..    d
+00002040: 6566 2074 6573 745f 636f 6e6e 6563 7469  ef test_connecti
+00002050: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
+00002060: 2020 2222 2243 7265 6174 6573 2061 2072    """Creates a r
+00002070: 6571 7565 7374 2074 6f77 6172 6473 2074  equest towards t
+00002080: 6865 2041 3130 3030 2043 6865 636b 2053  he A1000 Check S
+00002090: 7461 7475 7320 4150 4920 746f 2074 6573  tatus API to tes
+000020a0: 7420 7468 6520 636f 6e6e 6563 7469 6f6e  t the connection
+000020b0: 0a20 2020 2020 2020 2077 6974 6820 4131  .        with A1
+000020c0: 3030 302e 0a20 2020 2020 2020 2022 2222  000..        """
+000020d0: 0a20 2020 2020 2020 205f 203d 2073 656c  .        _ = sel
+000020e0: 662e 5f5f 616e 616c 7973 6973 5f69 735f  f.__analysis_is_
+000020f0: 6669 6e69 7368 6564 280a 2020 2020 2020  finished(.      
+00002100: 2020 2020 2020 7361 6d70 6c65 5f68 6173        sample_has
+00002110: 6865 733d 5b22 3030 3030 3030 3030 3030  hes=["0000000000
+00002120: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
+00002130: 3030 3030 3030 3030 3030 3030 3030 225d  00000000000000"]
+00002140: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00002150: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00002160: 6465 6620 7570 6c6f 6164 5f73 616d 706c  def upload_sampl
+00002170: 655f 6672 6f6d 5f70 6174 6828 7365 6c66  e_from_path(self
+00002180: 2c20 6669 6c65 5f70 6174 682c 2063 7573  , file_path, cus
+00002190: 746f 6d5f 6669 6c65 6e61 6d65 3d4e 6f6e  tom_filename=Non
+000021a0: 652c 2061 7263 6869 7665 5f70 6173 7377  e, archive_passw
+000021b0: 6f72 643d 4e6f 6e65 2c0a 2020 2020 2020  ord=None,.      
+000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021d0: 2020 2020 2020 2020 2020 726c 5f63 6c6f            rl_clo
+000021e0: 7564 5f73 616e 6462 6f78 5f70 6c61 7466  ud_sandbox_platf
+000021f0: 6f72 6d3d 4e6f 6e65 2c20 7461 6773 3d4e  orm=None, tags=N
+00002200: 6f6e 652c 2063 6f6d 6d65 6e74 3d4e 6f6e  one, comment=Non
+00002210: 652c 2063 6c6f 7564 5f61 6e61 6c79 7369  e, cloud_analysi
+00002220: 733d 5472 7565 293a 0a20 2020 2020 2020  s=True):.       
+00002230: 2022 2222 4163 6365 7074 7320 6120 6669   """Accepts a fi
+00002240: 6c65 2070 6174 6820 7374 7269 6e67 2066  le path string f
+00002250: 6f72 2066 696c 6520 7570 6c6f 6164 2061  or file upload a
+00002260: 6e64 2072 6574 7572 6e73 2061 2072 6573  nd returns a res
+00002270: 706f 6e73 652e 0a20 2020 2020 2020 2041  ponse..        A
+00002280: 6464 6974 696f 6e61 6c20 7061 7261 6d65  dditional parame
+00002290: 7465 7273 2063 616e 2062 6520 7072 6f76  ters can be prov
+000022a0: 6964 6564 2e0a 2020 2020 2020 2020 2020  ided..          
+000022b0: 2020 3a70 6172 616d 2066 696c 655f 7061    :param file_pa
+000022c0: 7468 3a20 7061 7468 2074 6f20 6669 6c65  th: path to file
+000022d0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
+000022e0: 7065 2066 696c 655f 7061 7468 3a20 7374  pe file_path: st
+000022f0: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
+00002300: 6172 616d 2063 7573 746f 6d5f 6669 6c65  aram custom_file
+00002310: 6e61 6d65 3a20 6375 7374 6f6d 2066 696c  name: custom fil
+00002320: 6520 6e61 6d65 2066 6f72 2075 706c 6f61  e name for uploa
+00002330: 640a 2020 2020 2020 2020 2020 2020 3a74  d.            :t
+00002340: 7970 6520 6375 7374 6f6d 5f66 696c 656e  ype custom_filen
+00002350: 616d 653a 2073 7472 0a20 2020 2020 2020  ame: str.       
+00002360: 2020 2020 203a 7061 7261 6d20 6172 6368       :param arch
+00002370: 6976 655f 7061 7373 776f 7264 3a20 7061  ive_password: pa
+00002380: 7373 776f 7264 2c20 6966 2066 696c 6520  ssword, if file 
+00002390: 6973 2061 2070 6173 7377 6f72 642d 7072  is a password-pr
+000023a0: 6f74 6563 7465 6420 6172 6368 6976 650a  otected archive.
+000023b0: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+000023c0: 6520 6172 6368 6976 655f 7061 7373 776f  e archive_passwo
+000023d0: 7264 3a20 7374 720a 2020 2020 2020 2020  rd: str.        
+000023e0: 2020 2020 3a70 6172 616d 2072 6c5f 636c      :param rl_cl
+000023f0: 6f75 645f 7361 6e64 626f 785f 706c 6174  oud_sandbox_plat
+00002400: 666f 726d 3a20 436c 6f75 6420 5361 6e64  form: Cloud Sand
+00002410: 626f 7820 706c 6174 666f 726d 2028 7769  box platform (wi
+00002420: 6e64 6f77 7337 2c20 7769 6e64 6f77 7331  ndows7, windows1
+00002430: 3020 6f72 206d 6163 6f73 5f31 3129 0a20  0 or macos_11). 
+00002440: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00002450: 2072 6c5f 636c 6f75 645f 7361 6e64 626f   rl_cloud_sandbo
+00002460: 785f 706c 6174 666f 726d 3a20 7374 720a  x_platform: str.
+00002470: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00002480: 616d 2074 6167 733a 2061 2073 7472 696e  am tags: a strin
+00002490: 6720 6f66 2063 6f6d 6d61 2073 6570 6172  g of comma separ
+000024a0: 6174 6564 2074 6167 730a 2020 2020 2020  ated tags.      
+000024b0: 2020 2020 2020 3a74 7970 6520 7461 6773        :type tags
+000024c0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+000024d0: 2020 3a70 6172 616d 2063 6f6d 6d65 6e74    :param comment
+000024e0: 3a20 636f 6d6d 656e 7420 7374 7269 6e67  : comment string
+000024f0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
+00002500: 7065 2063 6f6d 6d65 6e74 3a20 7374 720a  pe comment: str.
+00002510: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00002520: 616d 2063 6c6f 7564 5f61 6e61 6c79 7369  am cloud_analysi
+00002530: 733a 2075 7365 2063 6c6f 7564 2061 6e61  s: use cloud ana
+00002540: 6c79 7369 730a 2020 2020 2020 2020 2020  lysis.          
+00002550: 2020 3a74 7970 6520 636c 6f75 645f 616e    :type cloud_an
+00002560: 616c 7973 6973 3a20 626f 6f6c 0a20 2020  alysis: bool.   
+00002570: 2020 2020 2020 2020 203a 7265 7475 726e           :return
+00002580: 3a20 3a63 6c61 7373 3a60 5265 7370 6f6e  : :class:`Respon
+00002590: 7365 203c 5265 7370 6f6e 7365 3e60 206f  se <Response>` o
+000025a0: 626a 6563 740a 2020 2020 2020 2020 2020  bject.          
+000025b0: 2020 3a72 7479 7065 3a20 7265 7175 6573    :rtype: reques
+000025c0: 7473 2e52 6573 706f 6e73 650a 2020 2020  ts.Response.    
+000025d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000025e0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+000025f0: 6528 6669 6c65 5f70 6174 682c 2073 7472  e(file_path, str
+00002600: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00002610: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
+00002620: 7272 6f72 2822 6669 6c65 5f70 6174 6820  rror("file_path 
+00002630: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
+00002640: 2e22 290a 0a20 2020 2020 2020 2064 6174  .")..        dat
+00002650: 6120 3d20 7365 6c66 2e5f 5f63 7265 6174  a = self.__creat
+00002660: 655f 706f 7374 5f70 6179 6c6f 6164 280a  e_post_payload(.
+00002670: 2020 2020 2020 2020 2020 2020 6375 7374              cust
+00002680: 6f6d 5f66 696c 656e 616d 653d 6375 7374  om_filename=cust
+00002690: 6f6d 5f66 696c 656e 616d 652c 0a20 2020  om_filename,.   
+000026a0: 2020 2020 2020 2020 2061 7263 6869 7665           archive
+000026b0: 5f70 6173 7377 6f72 643d 6172 6368 6976  _password=archiv
+000026c0: 655f 7061 7373 776f 7264 2c0a 2020 2020  e_password,.    
+000026d0: 2020 2020 2020 2020 726c 5f63 6c6f 7564          rl_cloud
+000026e0: 5f73 616e 6462 6f78 5f70 6c61 7466 6f72  _sandbox_platfor
+000026f0: 6d3d 726c 5f63 6c6f 7564 5f73 616e 6462  m=rl_cloud_sandb
+00002700: 6f78 5f70 6c61 7466 6f72 6d2c 0a20 2020  ox_platform,.   
+00002710: 2020 2020 2020 2020 2074 6167 733d 7461           tags=ta
+00002720: 6773 2c0a 2020 2020 2020 2020 2020 2020  gs,.            
+00002730: 636f 6d6d 656e 743d 636f 6d6d 656e 742c  comment=comment,
+00002740: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
+00002750: 7564 5f61 6e61 6c79 7369 733d 636c 6f75  ud_analysis=clou
+00002760: 645f 616e 616c 7973 6973 0a20 2020 2020  d_analysis.     
+00002770: 2020 2029 0a0a 2020 2020 2020 2020 7572     )..        ur
+00002780: 6c20 3d20 7365 6c66 2e5f 7572 6c2e 666f  l = self._url.fo
+00002790: 726d 6174 2865 6e64 706f 696e 743d 7365  rmat(endpoint=se
+000027a0: 6c66 2e5f 5f55 504c 4f41 445f 454e 4450  lf.__UPLOAD_ENDP
+000027b0: 4f49 4e54 290a 0a20 2020 2020 2020 2074  OINT)..        t
+000027c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+000027d0: 6669 6c65 5f68 616e 646c 6520 3d20 6f70  file_handle = op
+000027e0: 656e 2866 696c 655f 7061 7468 2c20 2272  en(file_path, "r
+000027f0: 6222 290a 2020 2020 2020 2020 6578 6365  b").        exce
+00002800: 7074 2049 4f45 7272 6f72 2061 7320 6572  pt IOError as er
+00002810: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+00002820: 2072 6169 7365 2057 726f 6e67 496e 7075   raise WrongInpu
+00002830: 7445 7272 6f72 2822 4572 726f 7220 7768  tError("Error wh
+00002840: 696c 6520 6f70 656e 696e 6720 6669 6c65  ile opening file
+00002850: 2069 6e20 2772 6227 206d 6f64 6520 2d20   in 'rb' mode - 
+00002860: 7b65 7272 6f72 7d22 2e66 6f72 6d61 7428  {error}".format(
+00002870: 6572 726f 723d 7374 7228 6572 726f 7229  error=str(error)
+00002880: 2929 0a0a 2020 2020 2020 2020 7265 7370  ))..        resp
+00002890: 6f6e 7365 203d 2073 656c 662e 5f5f 706f  onse = self.__po
+000028a0: 7374 5f72 6571 7565 7374 280a 2020 2020  st_request(.    
+000028b0: 2020 2020 2020 2020 7572 6c3d 7572 6c2c          url=url,
+000028c0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+000028d0: 6573 3d7b 2266 696c 6522 3a20 6669 6c65  es={"file": file
+000028e0: 5f68 616e 646c 657d 2c0a 2020 2020 2020  _handle},.      
+000028f0: 2020 2020 2020 6461 7461 3d64 6174 610a        data=data.
+00002900: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00002910: 2020 2073 656c 662e 5f5f 7261 6973 655f     self.__raise_
+00002920: 6f6e 5f65 7272 6f72 2872 6573 706f 6e73  on_error(respons
+00002930: 6529 0a0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00002940: 726e 2072 6573 706f 6e73 650a 0a20 2020  rn response..   
+00002950: 2064 6566 2075 706c 6f61 645f 7361 6d70   def upload_samp
+00002960: 6c65 5f66 726f 6d5f 6669 6c65 2873 656c  le_from_file(sel
+00002970: 662c 2066 696c 655f 736f 7572 6365 2c20  f, file_source, 
+00002980: 6375 7374 6f6d 5f66 696c 656e 616d 653d  custom_filename=
+00002990: 4e6f 6e65 2c20 6172 6368 6976 655f 7061  None, archive_pa
+000029a0: 7373 776f 7264 3d4e 6f6e 652c 0a20 2020  ssword=None,.   
+000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029c0: 2020 2020 2020 2020 2020 2020 2072 6c5f               rl_
+000029d0: 636c 6f75 645f 7361 6e64 626f 785f 706c  cloud_sandbox_pl
+000029e0: 6174 666f 726d 3d4e 6f6e 652c 2074 6167  atform=None, tag
+000029f0: 733d 4e6f 6e65 2c20 636f 6d6d 656e 743d  s=None, comment=
+00002a00: 4e6f 6e65 2c20 636c 6f75 645f 616e 616c  None, cloud_anal
+00002a10: 7973 6973 3d54 7275 6529 3a0a 2020 2020  ysis=True):.    
+00002a20: 2020 2020 2222 2241 6363 6570 7473 2061      """Accepts a
+00002a30: 6e20 6f70 656e 2066 696c 6520 696e 2027  n open file in '
+00002a40: 7262 2720 6d6f 6465 2066 6f72 2066 696c  rb' mode for fil
+00002a50: 6520 7570 6c6f 6164 2061 6e64 2072 6574  e upload and ret
+00002a60: 7572 6e73 2061 2072 6573 706f 6e73 652e  urns a response.
+00002a70: 0a20 2020 2020 2020 2041 6464 6974 696f  .        Additio
+00002a80: 6e61 6c20 7061 7261 6d65 7465 7273 2063  nal parameters c
+00002a90: 616e 2062 6520 7072 6f76 6964 6564 2e0a  an be provided..
+00002aa0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00002ab0: 616d 2066 696c 655f 736f 7572 6365 3a20  am file_source: 
+00002ac0: 6f70 656e 2066 696c 650a 2020 2020 2020  open file.      
+00002ad0: 2020 2020 2020 3a74 7970 6520 6669 6c65        :type file
+00002ae0: 5f73 6f75 7263 653a 2066 696c 6520 6f72  _source: file or
+00002af0: 2042 696e 6172 7949 4f0a 2020 2020 2020   BinaryIO.      
+00002b00: 2020 2020 2020 3a70 6172 616d 2063 7573        :param cus
+00002b10: 746f 6d5f 6669 6c65 6e61 6d65 3a20 6375  tom_filename: cu
+00002b20: 7374 6f6d 2066 696c 6520 6e61 6d65 2066  stom file name f
+00002b30: 6f72 2075 706c 6f61 640a 2020 2020 2020  or upload.      
+00002b40: 2020 2020 2020 3a74 7970 6520 6375 7374        :type cust
+00002b50: 6f6d 5f66 696c 656e 616d 653a 2073 7472  om_filename: str
+00002b60: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+00002b70: 7261 6d20 6172 6368 6976 655f 7061 7373  ram archive_pass
+00002b80: 776f 7264 3a20 7061 7373 776f 7264 2c20  word: password, 
+00002b90: 6966 2066 696c 6520 6973 2061 2070 6173  if file is a pas
+00002ba0: 7377 6f72 642d 7072 6f74 6563 7465 6420  sword-protected 
+00002bb0: 6172 6368 6976 650a 2020 2020 2020 2020  archive.        
+00002bc0: 2020 2020 3a74 7970 6520 6172 6368 6976      :type archiv
+00002bd0: 655f 7061 7373 776f 7264 3a20 7374 720a  e_password: str.
+00002be0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00002bf0: 616d 2072 6c5f 636c 6f75 645f 7361 6e64  am rl_cloud_sand
+00002c00: 626f 785f 706c 6174 666f 726d 3a20 436c  box_platform: Cl
+00002c10: 6f75 6420 5361 6e64 626f 7820 706c 6174  oud Sandbox plat
+00002c20: 666f 726d 2028 7769 6e64 6f77 7337 2c20  form (windows7, 
+00002c30: 7769 6e64 6f77 7331 3020 6f72 206d 6163  windows10 or mac
+00002c40: 6f73 5f31 3129 0a20 2020 2020 2020 2020  os_11).         
+00002c50: 2020 203a 7479 7065 2072 6c5f 636c 6f75     :type rl_clou
+00002c60: 645f 7361 6e64 626f 785f 706c 6174 666f  d_sandbox_platfo
+00002c70: 726d 3a20 7374 720a 2020 2020 2020 2020  rm: str.        
+00002c80: 2020 2020 3a70 6172 616d 2074 6167 733a      :param tags:
+00002c90: 2061 2073 7472 696e 6720 6f66 2063 6f6d   a string of com
+00002ca0: 6d61 2073 6570 6172 6174 6564 2074 6167  ma separated tag
+00002cb0: 730a 2020 2020 2020 2020 2020 2020 3a74  s.            :t
+00002cc0: 7970 6520 7461 6773 3a20 7374 720a 2020  ype tags: str.  
+00002cd0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00002ce0: 2063 6f6d 6d65 6e74 3a20 636f 6d6d 656e   comment: commen
+00002cf0: 7420 7374 7269 6e67 0a20 2020 2020 2020  t string.       
+00002d00: 2020 2020 203a 7479 7065 2063 6f6d 6d65       :type comme
+00002d10: 6e74 3a20 7374 720a 2020 2020 2020 2020  nt: str.        
+00002d20: 2020 2020 3a70 6172 616d 2063 6c6f 7564      :param cloud
+00002d30: 5f61 6e61 6c79 7369 733a 2075 7365 2063  _analysis: use c
+00002d40: 6c6f 7564 2061 6e61 6c79 7369 730a 2020  loud analysis.  
+00002d50: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00002d60: 636c 6f75 645f 616e 616c 7973 6973 3a20  cloud_analysis: 
+00002d70: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
+00002d80: 203a 7265 7475 726e 3a20 3a63 6c61 7373   :return: :class
+00002d90: 3a60 5265 7370 6f6e 7365 203c 5265 7370  :`Response <Resp
+00002da0: 6f6e 7365 3e60 206f 626a 6563 740a 2020  onse>` object.  
+00002db0: 2020 2020 2020 2020 2020 3a72 7479 7065            :rtype
+00002dc0: 3a20 7265 7175 6573 7473 2e52 6573 706f  : requests.Respo
+00002dd0: 6e73 650a 2020 2020 2020 2020 2222 220a  nse.        """.
+00002de0: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
+00002df0: 6173 6174 7472 2866 696c 655f 736f 7572  asattr(file_sour
+00002e00: 6365 2c20 2272 6561 6422 293a 0a20 2020  ce, "read"):.   
+00002e10: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+00002e20: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+00002e30: 6669 6c65 5f73 6f75 7263 6520 7061 7261  file_source para
+00002e40: 6d65 7465 7220 6d75 7374 2062 6520 6120  meter must be a 
+00002e50: 6669 6c65 206f 7065 6e20 696e 2027 7262  file open in 'rb
+00002e60: 2720 6d6f 6465 2e22 290a 0a20 2020 2020  ' mode.")..     
+00002e70: 2020 2064 6174 6120 3d20 7365 6c66 2e5f     data = self._
+00002e80: 5f63 7265 6174 655f 706f 7374 5f70 6179  _create_post_pay
+00002e90: 6c6f 6164 280a 2020 2020 2020 2020 2020  load(.          
+00002ea0: 2020 6375 7374 6f6d 5f66 696c 656e 616d    custom_filenam
+00002eb0: 653d 6375 7374 6f6d 5f66 696c 656e 616d  e=custom_filenam
+00002ec0: 652c 0a20 2020 2020 2020 2020 2020 2061  e,.            a
+00002ed0: 7263 6869 7665 5f70 6173 7377 6f72 643d  rchive_password=
+00002ee0: 6172 6368 6976 655f 7061 7373 776f 7264  archive_password
+00002ef0: 2c0a 2020 2020 2020 2020 2020 2020 726c  ,.            rl
+00002f00: 5f63 6c6f 7564 5f73 616e 6462 6f78 5f70  _cloud_sandbox_p
+00002f10: 6c61 7466 6f72 6d3d 726c 5f63 6c6f 7564  latform=rl_cloud
+00002f20: 5f73 616e 6462 6f78 5f70 6c61 7466 6f72  _sandbox_platfor
+00002f30: 6d2c 0a20 2020 2020 2020 2020 2020 2074  m,.            t
+00002f40: 6167 733d 7461 6773 2c0a 2020 2020 2020  ags=tags,.      
+00002f50: 2020 2020 2020 636f 6d6d 656e 743d 636f        comment=co
+00002f60: 6d6d 656e 742c 0a20 2020 2020 2020 2020  mment,.         
+00002f70: 2020 2063 6c6f 7564 5f61 6e61 6c79 7369     cloud_analysi
+00002f80: 733d 636c 6f75 645f 616e 616c 7973 6973  s=cloud_analysis
+00002f90: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00002fa0: 2020 2020 7572 6c20 3d20 7365 6c66 2e5f      url = self._
+00002fb0: 7572 6c2e 666f 726d 6174 2865 6e64 706f  url.format(endpo
+00002fc0: 696e 743d 7365 6c66 2e5f 5f55 504c 4f41  int=self.__UPLOA
+00002fd0: 445f 454e 4450 4f49 4e54 290a 0a20 2020  D_ENDPOINT)..   
+00002fe0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+00002ff0: 7365 6c66 2e5f 5f70 6f73 745f 7265 7175  self.__post_requ
+00003000: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
+00003010: 2075 726c 3d75 726c 2c0a 2020 2020 2020   url=url,.      
+00003020: 2020 2020 2020 6669 6c65 733d 7b22 6669        files={"fi
+00003030: 6c65 223a 2066 696c 655f 736f 7572 6365  le": file_source
+00003040: 7d2c 0a20 2020 2020 2020 2020 2020 2064  },.            d
+00003050: 6174 613d 6461 7461 0a20 2020 2020 2020  ata=data.       
+00003060: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
+00003070: 2e5f 5f72 6169 7365 5f6f 6e5f 6572 726f  .__raise_on_erro
+00003080: 7228 7265 7370 6f6e 7365 290a 0a20 2020  r(response)..   
+00003090: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+000030a0: 6f6e 7365 0a0a 2020 2020 6465 6620 7570  onse..    def up
+000030b0: 6c6f 6164 5f73 616d 706c 655f 6672 6f6d  load_sample_from
+000030c0: 5f75 726c 2873 656c 662c 2066 696c 655f  _url(self, file_
+000030d0: 7572 6c2c 2063 7261 776c 6572 3d4e 6f6e  url, crawler=Non
+000030e0: 652c 2061 7263 6869 7665 5f70 6173 7377  e, archive_passw
+000030f0: 6f72 643d 4e6f 6e65 2c20 726c 5f63 6c6f  ord=None, rl_clo
+00003100: 7564 5f73 616e 6462 6f78 5f70 6c61 7466  ud_sandbox_platf
+00003110: 6f72 6d3d 4e6f 6e65 293a 0a20 2020 2020  orm=None):.     
+00003120: 2020 2022 2222 4163 6365 7074 7320 6120     """Accepts a 
+00003130: 6669 6c65 2075 726c 2061 6e64 2072 6574  file url and ret
+00003140: 7572 6e73 2061 2072 6573 706f 6e73 652e  urns a response.
+00003150: 0a20 2020 2020 2020 2041 6464 6974 696f  .        Additio
+00003160: 6e61 6c20 7061 7261 6d65 7465 7273 2063  nal parameters c
+00003170: 616e 2062 6520 7072 6f76 6964 6564 2e0a  an be provided..
+00003180: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00003190: 616d 2066 696c 655f 7572 6c3a 2055 524c  am file_url: URL
+000031a0: 2066 726f 6d20 7768 6963 6820 7468 6520   from which the 
+000031b0: 6170 706c 6961 6e63 6520 7368 6f75 6c64  appliance should
+000031c0: 2064 6f77 6e6c 6f61 6420 7468 6520 6461   download the da
+000031d0: 7461 0a20 2020 2020 2020 2020 2020 203a  ta.            :
+000031e0: 7479 7065 2066 696c 655f 7572 6c3a 2073  type file_url: s
+000031f0: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
+00003200: 7061 7261 6d20 6372 6177 6c65 723a 2063  param crawler: c
+00003210: 7261 776c 6572 206d 6574 686f 6420 286c  rawler method (l
+00003220: 6f63 616c 206f 7220 636c 6f75 6429 0a20  ocal or cloud). 
+00003230: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00003240: 2063 7261 776c 6572 3a20 7374 720a 2020   crawler: str.  
+00003250: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00003260: 2061 7263 6869 7665 5f70 6173 7377 6f72   archive_passwor
+00003270: 643a 2070 6173 7377 6f72 642c 2069 6620  d: password, if 
+00003280: 6669 6c65 2069 7320 6120 7061 7373 776f  file is a passwo
+00003290: 7264 2d70 726f 7465 6374 6564 2061 7263  rd-protected arc
+000032a0: 6869 7665 0a20 2020 2020 2020 2020 2020  hive.           
+000032b0: 203a 7479 7065 2061 7263 6869 7665 5f70   :type archive_p
+000032c0: 6173 7377 6f72 643a 2073 7472 0a20 2020  assword: str.   
+000032d0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+000032e0: 726c 5f63 6c6f 7564 5f73 616e 6462 6f78  rl_cloud_sandbox
+000032f0: 5f70 6c61 7466 6f72 6d3a 2043 6c6f 7564  _platform: Cloud
+00003300: 2053 616e 6462 6f78 2070 6c61 7466 6f72   Sandbox platfor
+00003310: 6d20 2877 696e 646f 7773 372c 2077 696e  m (windows7, win
+00003320: 646f 7773 3130 206f 7220 6d61 636f 735f  dows10 or macos_
+00003330: 3131 290a 2020 2020 2020 2020 2020 2020  11).            
+00003340: 3a74 7970 6520 726c 5f63 6c6f 7564 5f73  :type rl_cloud_s
+00003350: 616e 6462 6f78 5f70 6c61 7466 6f72 6d3a  andbox_platform:
+00003360: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+00003370: 203a 7265 7475 726e 3a20 3a63 6c61 7373   :return: :class
+00003380: 3a60 5265 7370 6f6e 7365 203c 5265 7370  :`Response <Resp
+00003390: 6f6e 7365 3e60 206f 626a 6563 740a 2020  onse>` object.  
+000033a0: 2020 2020 2020 2020 2020 3a72 7479 7065            :rtype
+000033b0: 3a20 7265 7175 6573 7473 2e52 6573 706f  : requests.Respo
+000033c0: 6e73 650a 2020 2020 2020 2020 2222 220a  nse.        """.
+000033d0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+000033e0: 7365 6c66 2e5f 5f63 7265 6174 655f 706f  self.__create_po
+000033f0: 7374 5f70 6179 6c6f 6164 280a 2020 2020  st_payload(.    
+00003400: 2020 2020 2020 2020 6372 6177 6c65 723d          crawler=
+00003410: 6372 6177 6c65 722c 0a20 2020 2020 2020  crawler,.       
+00003420: 2020 2020 2061 7263 6869 7665 5f70 6173       archive_pas
+00003430: 7377 6f72 643d 6172 6368 6976 655f 7061  sword=archive_pa
+00003440: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
+00003450: 2020 2020 726c 5f63 6c6f 7564 5f73 616e      rl_cloud_san
+00003460: 6462 6f78 5f70 6c61 7466 6f72 6d3d 726c  dbox_platform=rl
+00003470: 5f63 6c6f 7564 5f73 616e 6462 6f78 5f70  _cloud_sandbox_p
+00003480: 6c61 7466 6f72 6d2c 0a20 2020 2020 2020  latform,.       
+00003490: 2020 2020 2066 696c 655f 7572 6c3d 6669       file_url=fi
+000034a0: 6c65 5f75 726c 0a20 2020 2020 2020 2029  le_url.        )
+000034b0: 0a0a 2020 2020 2020 2020 7572 6c20 3d20  ..        url = 
+000034c0: 7365 6c66 2e5f 7572 6c2e 666f 726d 6174  self._url.format
+000034d0: 2865 6e64 706f 696e 743d 7365 6c66 2e5f  (endpoint=self._
+000034e0: 5f55 504c 4f41 445f 454e 4450 4f49 4e54  _UPLOAD_ENDPOINT
+000034f0: 290a 0a20 2020 2020 2020 2072 6573 706f  )..        respo
+00003500: 6e73 6520 3d20 7365 6c66 2e5f 5f70 6f73  nse = self.__pos
+00003510: 745f 7265 7175 6573 7428 0a20 2020 2020  t_request(.     
+00003520: 2020 2020 2020 2075 726c 3d75 726c 2c0a         url=url,.
+00003530: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00003540: 3d64 6174 612c 0a20 2020 2020 2020 2029  =data,.        )
+00003550: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00003560: 5f72 6169 7365 5f6f 6e5f 6572 726f 7228  _raise_on_error(
+00003570: 7265 7370 6f6e 7365 290a 0a20 2020 2020  response)..     
+00003580: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
+00003590: 7365 0a0a 2020 2020 6465 6620 6368 6563  se..    def chec
+000035a0: 6b5f 7375 626d 6974 7465 645f 7572 6c5f  k_submitted_url_
+000035b0: 7374 6174 7573 2873 656c 662c 2074 6173  status(self, tas
+000035c0: 6b5f 6964 293a 0a20 2020 2020 2020 2022  k_id):.        "
+000035d0: 2222 4163 6365 7074 7320 6120 7461 736b  ""Accepts a task
+000035e0: 2049 4420 7265 7475 726e 6564 2062 7920   ID returned by 
+000035f0: 7468 6520 7570 6c6f 6164 2073 616d 706c  the upload sampl
+00003600: 6520 6672 6f6d 2075 726c 0a20 2020 2020  e from url.     
+00003610: 2020 2020 2020 203a 7061 7261 6d20 7461         :param ta
+00003620: 736b 5f69 643a 2049 4420 6f66 2074 6865  sk_id: ID of the
+00003630: 2073 7562 6d69 7474 6564 2073 616d 706c   submitted sampl
+00003640: 650a 2020 2020 2020 2020 2020 2020 3a74  e.            :t
+00003650: 7970 6520 7461 736b 5f69 643a 2073 7472  ype task_id: str
+00003660: 0a20 2020 2020 2020 2020 2020 203a 7265  .            :re
+00003670: 7475 726e 3a20 7265 7370 6f6e 7365 0a20  turn: response. 
+00003680: 2020 2020 2020 2020 2020 203a 7274 7970             :rtyp
+00003690: 653a 2072 6571 7565 7374 732e 5265 7370  e: requests.Resp
+000036a0: 6f6e 7365 0a20 2020 2020 2020 2022 2222  onse.        """
+000036b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000036c0: 6973 696e 7374 616e 6365 2874 6173 6b5f  isinstance(task_
+000036d0: 6964 2c20 7374 7229 3a0a 2020 2020 2020  id, str):.      
+000036e0: 2020 2020 2020 7261 6973 6520 5772 6f6e        raise Wron
+000036f0: 6749 6e70 7574 4572 726f 7228 2274 6173  gInputError("tas
+00003700: 6b5f 6964 2070 6172 616d 6574 6572 206d  k_id parameter m
+00003710: 7573 7420 6265 2061 2073 7472 696e 672e  ust be a string.
+00003720: 2229 0a0a 2020 2020 2020 2020 656e 6470  ")..        endp
+00003730: 6f69 6e74 203d 2073 656c 662e 5f5f 4348  oint = self.__CH
+00003740: 4543 4b5f 5552 4c5f 5354 4154 5553 5f45  ECK_URL_STATUS_E
+00003750: 4e44 504f 494e 542e 666f 726d 6174 2874  NDPOINT.format(t
+00003760: 6173 6b5f 6964 3d74 6173 6b5f 6964 290a  ask_id=task_id).
+00003770: 0a20 2020 2020 2020 2075 726c 203d 2073  .        url = s
+00003780: 656c 662e 5f75 726c 2e66 6f72 6d61 7428  elf._url.format(
+00003790: 656e 6470 6f69 6e74 3d65 6e64 706f 696e  endpoint=endpoin
+000037a0: 7429 0a0a 2020 2020 2020 2020 7265 7370  t)..        resp
+000037b0: 6f6e 7365 203d 2073 656c 662e 5f5f 6765  onse = self.__ge
+000037c0: 745f 7265 7175 6573 7428 7572 6c3d 7572  t_request(url=ur
+000037d0: 6c29 0a0a 2020 2020 2020 2020 7365 6c66  l)..        self
+000037e0: 2e5f 5f72 6169 7365 5f6f 6e5f 6572 726f  .__raise_on_erro
+000037f0: 7228 7265 7370 6f6e 7365 290a 0a20 2020  r(response)..   
+00003800: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+00003810: 6f6e 7365 0a0a 2020 2020 6465 6620 6765  onse..    def ge
+00003820: 745f 7375 626d 6974 7465 645f 7572 6c5f  t_submitted_url_
+00003830: 7265 706f 7274 2873 656c 662c 2074 6173  report(self, tas
+00003840: 6b5f 6964 2c20 7265 7472 7929 3a0a 2020  k_id, retry):.  
+00003850: 2020 2020 2020 2222 2241 6363 6570 7473        """Accepts
+00003860: 2061 2074 6173 6b20 4944 2072 6574 7572   a task ID retur
+00003870: 6e65 6420 6279 2074 6865 2075 706c 6f61  ned by the uploa
+00003880: 6420 7361 6d70 6c65 2066 726f 6d20 7572  d sample from ur
+00003890: 6c20 616e 6420 7265 7475 726e 7320 6120  l and returns a 
+000038a0: 7265 706f 7274 2072 6573 706f 6e73 652e  report response.
+000038b0: 0a20 2020 2020 2020 2054 6869 7320 6d65  .        This me
+000038c0: 7468 6f64 2063 6f6d 6269 6e65 7320 7570  thod combines up
+000038d0: 6c6f 6164 696e 6720 6120 7361 6d70 6c65  loading a sample
+000038e0: 2066 726f 6d20 7572 6c20 616e 6420 6f62   from url and ob
+000038f0: 7461 696e 696e 6720 7468 6520 616e 616c  taining the anal
+00003900: 7973 6973 2072 6570 6f72 742e 0a20 2020  ysis report..   
+00003910: 2020 2020 2041 6464 6974 696f 6e61 6c20       Additional 
+00003920: 6669 656c 6473 2063 616e 2062 6520 7072  fields can be pr
+00003930: 6f76 6964 6564 2e0a 2020 2020 2020 2020  ovided..        
+00003940: 5468 6520 7265 7375 6c74 2066 6574 6368  The result fetch
+00003950: 696e 6720 6163 7469 6f6e 206f 6620 7468  ing action of th
+00003960: 6973 206d 6574 686f 6420 7574 696c 697a  is method utiliz
+00003970: 6573 2074 6865 2073 6574 206e 756d 6265  es the set numbe
+00003980: 7220 6f66 2072 6574 7269 6573 2061 6e64  r of retries and
+00003990: 2077 6169 7420 7469 6d65 2069 6e20 7365   wait time in se
+000039a0: 636f 6e64 7320 746f 2074 696d 650a 2020  conds to time.  
+000039b0: 2020 2020 2020 6f75 7420 6966 2074 6865        out if the
+000039c0: 2061 6e61 6c79 7369 7320 7265 7375 6c74   analysis result
+000039d0: 7320 6172 6520 6e6f 7420 7265 6164 792e  s are not ready.
+000039e0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+000039f0: 7261 6d20 7461 736b 5f69 643a 2049 4420  ram task_id: ID 
+00003a00: 6f66 2074 6865 2073 7562 6d69 7474 6564  of the submitted
+00003a10: 2073 616d 706c 650a 2020 2020 2020 2020   sample.        
+00003a20: 2020 2020 3a74 7970 6520 7461 736b 5f69      :type task_i
+00003a30: 643a 2073 7472 0a20 2020 2020 2020 2020  d: str.         
+00003a40: 2020 203a 7061 7261 6d20 7265 7472 793a     :param retry:
+00003a50: 2069 6620 7365 7420 746f 2046 616c 7365   if set to False
+00003a60: 2074 6865 7265 2077 696c 6c20 6f6e 6c79   there will only
+00003a70: 2062 6520 6f6e 6520 7472 7920 6174 206f   be one try at o
+00003a80: 6274 6169 6e69 6e67 2074 6865 2061 6e61  btaining the ana
+00003a90: 6c79 7369 7320 7265 706f 7274 0a20 2020  lysis report.   
+00003aa0: 2020 2020 2020 2020 203a 7479 7065 2072           :type r
+00003ab0: 6574 7279 3a20 626f 6f6c 0a20 2020 2020  etry: bool.     
+00003ac0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00003ad0: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+00003ae0: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
+00003af0: 7565 7374 732e 5265 7370 6f6e 7365 0a20  uests.Response. 
+00003b00: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00003b10: 2020 2020 6966 2072 6574 7279 206e 6f74      if retry not
+00003b20: 2069 6e20 2854 7275 652c 2046 616c 7365   in (True, False
+00003b30: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00003b40: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
+00003b50: 7272 6f72 2822 7265 7472 7920 7061 7261  rror("retry para
+00003b60: 6d65 7465 7220 6d75 7374 2062 6520 626f  meter must be bo
+00003b70: 6f6c 6561 6e2e 2229 0a0a 2020 2020 2020  olean.")..      
+00003b80: 2020 7265 7472 6965 7320 3d20 7365 6c66    retries = self
+00003b90: 2e5f 7265 7472 6965 7320 6966 2072 6574  ._retries if ret
+00003ba0: 7279 2065 6c73 6520 300a 0a20 2020 2020  ry else 0..     
+00003bb0: 2020 2066 6f72 2069 7465 7261 7469 6f6e     for iteration
+00003bc0: 2069 6e20 7261 6e67 6528 7265 7472 6965   in range(retrie
+00003bd0: 7320 2b20 3129 3a0a 2020 2020 2020 2020  s + 1):.        
+00003be0: 2020 2020 6966 2069 7465 7261 7469 6f6e      if iteration
+00003bf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003c00: 2020 7469 6d65 2e73 6c65 6570 2873 656c    time.sleep(sel
+00003c10: 662e 5f77 6169 745f 7469 6d65 5f73 6563  f._wait_time_sec
+00003c20: 6f6e 6473 290a 0a20 2020 2020 2020 2020  onds)..         
+00003c30: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00003c40: 6c66 2e63 6865 636b 5f73 7562 6d69 7474  lf.check_submitt
+00003c50: 6564 5f75 726c 5f73 7461 7475 7328 7461  ed_url_status(ta
+00003c60: 736b 5f69 643d 7461 736b 5f69 6429 0a20  sk_id=task_id). 
+00003c70: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+00003c80: 7320 3d20 7265 7370 6f6e 7365 2e6a 736f  s = response.jso
+00003c90: 6e28 292e 6765 7428 2270 726f 6365 7373  n().get("process
+00003ca0: 696e 675f 7374 6174 7573 2229 0a0a 2020  ing_status")..  
+00003cb0: 2020 2020 2020 2020 2020 6966 2073 7461            if sta
+00003cc0: 7475 7320 3d3d 2022 6572 726f 7222 3a0a  tus == "error":.
+00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ce0: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+00003cf0: 7265 7370 6f6e 7365 2e6a 736f 6e28 292e  response.json().
+00003d00: 6765 7428 226d 6573 7361 6765 2229 290a  get("message")).
+00003d10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003d20: 7374 6174 7573 203d 3d20 2263 6f6d 706c  status == "compl
+00003d30: 6574 6522 3a0a 2020 2020 2020 2020 2020  ete":.          
+00003d40: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00003d50: 706f 6e73 650a 0a20 2020 2020 2020 2072  ponse..        r
+00003d60: 6169 7365 2052 6571 7565 7374 5469 6d65  aise RequestTime
+00003d70: 6f75 7445 7272 6f72 2822 5265 706f 7274  outError("Report
+00003d80: 2066 6574 6368 696e 6720 6174 7465 6d70   fetching attemp
+00003d90: 7473 2066 696e 6973 6865 6420 2d20 5468  ts finished - Th
+00003da0: 6520 616e 616c 7973 6973 2072 6570 6f72  e analysis repor
+00003db0: 7420 6973 2073 7469 6c6c 206e 6f74 2072  t is still not r
+00003dc0: 6561 6479 2022 0a20 2020 2020 2020 2020  eady ".         
+00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003de0: 2020 2020 2020 2020 2022 6f72 2074 6865           "or the
+00003df0: 2073 616d 706c 6520 646f 6573 206e 6f74   sample does not
+00003e00: 2065 7869 7374 206f 6e20 7468 6520 6170   exist on the ap
+00003e10: 706c 6961 6e63 652e 2229 0a0a 2020 2020  pliance.")..    
+00003e20: 6465 6620 7570 6c6f 6164 5f73 616d 706c  def upload_sampl
+00003e30: 655f 6672 6f6d 5f75 726c 5f61 6e64 5f67  e_from_url_and_g
+00003e40: 6574 5f72 6570 6f72 7428 7365 6c66 2c20  et_report(self, 
+00003e50: 6669 6c65 5f75 726c 2c20 7265 7472 793d  file_url, retry=
+00003e60: 5472 7565 2c20 6372 6177 6c65 723d 226c  True, crawler="l
+00003e70: 6f63 616c 222c 2061 7263 6869 7665 5f70  ocal", archive_p
+00003e80: 6173 7377 6f72 643d 4e6f 6e65 2c0a 2020  assword=None,.  
+00003e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003eb0: 2020 2020 2020 2020 2020 2020 726c 5f63              rl_c
+00003ec0: 6c6f 7564 5f73 616e 6462 6f78 5f70 6c61  loud_sandbox_pla
+00003ed0: 7466 6f72 6d3d 4e6f 6e65 293a 0a20 2020  tform=None):.   
+00003ee0: 2020 2020 2022 2222 4163 6365 7074 7320       """Accepts 
+00003ef0: 6120 6669 6c65 2075 726c 2066 6f72 2066  a file url for f
+00003f00: 696c 6520 7570 6c6f 6164 2061 6e64 2072  ile upload and r
+00003f10: 6574 7572 6e73 2061 2072 6570 6f72 7420  eturns a report 
+00003f20: 7265 7370 6f6e 7365 2e0a 2020 2020 2020  response..      
+00003f30: 2020 5468 6973 206d 6574 686f 6420 636f    This method co
+00003f40: 6d62 696e 6573 2075 706c 6f61 6469 6e67  mbines uploading
+00003f50: 2061 2073 616d 706c 6520 6672 6f6d 2075   a sample from u
+00003f60: 726c 2061 6e64 206f 6274 6169 6e69 6e67  rl and obtaining
+00003f70: 2074 6865 2073 756d 6d61 7279 2061 6e61   the summary ana
+00003f80: 6c79 7369 7320 7265 706f 7274 2e0a 2020  lysis report..  
+00003f90: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
+00003fa0: 2066 6965 6c64 7320 6361 6e20 6265 2070   fields can be p
+00003fb0: 726f 7669 6465 642e 0a20 2020 2020 2020  rovided..       
+00003fc0: 2054 6865 2072 6573 756c 7420 6665 7463   The result fetc
+00003fd0: 6869 6e67 2061 6374 696f 6e20 6f66 2074  hing action of t
+00003fe0: 6869 7320 6d65 7468 6f64 2075 7469 6c69  his method utili
+00003ff0: 7a65 7320 7468 6520 7365 7420 6e75 6d62  zes the set numb
+00004000: 6572 206f 6620 7265 7472 6965 7320 616e  er of retries an
+00004010: 6420 7761 6974 2074 696d 6520 696e 2073  d wait time in s
+00004020: 6563 6f6e 6473 2074 6f20 7469 6d65 0a20  econds to time. 
+00004030: 2020 2020 2020 206f 7574 2069 6620 7468         out if th
+00004040: 6520 616e 616c 7973 6973 2072 6573 756c  e analysis resul
+00004050: 7473 2061 7265 206e 6f74 2072 6561 6479  ts are not ready
+00004060: 2e0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
+00004070: 6172 616d 2066 696c 655f 7572 6c3a 2055  aram file_url: U
+00004080: 524c 2066 726f 6d20 7768 6963 6820 7468  RL from which th
+00004090: 6520 6170 706c 6961 6e63 6520 7368 6f75  e appliance shou
+000040a0: 6c64 2064 6f77 6e6c 6f61 6420 7468 6520  ld download the 
+000040b0: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
+000040c0: 203a 7479 7065 2066 696c 655f 7572 6c3a   :type file_url:
+000040d0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+000040e0: 203a 7061 7261 6d20 7265 7472 793a 2069   :param retry: i
+000040f0: 6620 7365 7420 746f 2046 616c 7365 2074  f set to False t
+00004100: 6865 7265 2077 696c 6c20 6f6e 6c79 2062  here will only b
+00004110: 6520 6f6e 6520 7472 7920 6174 206f 6274  e one try at obt
+00004120: 6169 6e69 6e67 2074 6865 2061 6e61 6c79  aining the analy
+00004130: 7369 7320 7265 706f 7274 0a20 2020 2020  sis report.     
+00004140: 2020 2020 2020 203a 7479 7065 2072 6574         :type ret
+00004150: 7279 3a20 626f 6f6c 0a20 2020 2020 2020  ry: bool.       
+00004160: 2020 2020 203a 7061 7261 6d20 6372 6177       :param craw
+00004170: 6c65 723a 2063 7261 776c 6572 206d 6574  ler: crawler met
+00004180: 686f 6420 286c 6f63 616c 206f 7220 636c  hod (local or cl
+00004190: 6f75 6429 0a20 2020 2020 2020 2020 2020  oud).           
+000041a0: 203a 7479 7065 2063 7261 776c 6572 3a20   :type crawler: 
+000041b0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+000041c0: 2020 203a 7061 7261 6d20 6172 6368 6976     :param archiv
+000041d0: 655f 7061 7373 776f 7264 3a20 7061 7373  e_password: pass
+000041e0: 776f 7264 2c20 6966 2066 696c 6520 6973  word, if file is
+000041f0: 2061 2070 6173 7377 6f72 642d 7072 6f74   a password-prot
+00004200: 6563 7465 6420 6172 6368 6976 650a 2020  ected archive.  
+00004210: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00004220: 6172 6368 6976 655f 7061 7373 776f 7264  archive_password
+00004230: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+00004240: 2020 3a70 6172 616d 2072 6c5f 636c 6f75    :param rl_clou
+00004250: 645f 7361 6e64 626f 785f 706c 6174 666f  d_sandbox_platfo
+00004260: 726d 3a20 436c 6f75 6420 5361 6e64 626f  rm: Cloud Sandbo
+00004270: 7820 706c 6174 666f 726d 2028 7769 6e64  x platform (wind
+00004280: 6f77 7337 2c20 7769 6e64 6f77 7331 3020  ows7, windows10 
+00004290: 6f72 206d 6163 6f73 5f31 3129 0a20 2020  or macos_11).   
+000042a0: 2020 2020 2020 2020 203a 7479 7065 2072           :type r
+000042b0: 6c5f 636c 6f75 645f 7361 6e64 626f 785f  l_cloud_sandbox_
+000042c0: 706c 6174 666f 726d 3a20 7374 720a 2020  platform: str.  
+000042d0: 2020 2020 2020 2020 2020 3a72 6574 7572            :retur
+000042e0: 6e3a 203a 636c 6173 733a 6052 6573 706f  n: :class:`Respo
+000042f0: 6e73 6520 3c52 6573 706f 6e73 653e 6020  nse <Response>` 
+00004300: 6f62 6a65 6374 0a20 2020 2020 2020 2020  object.         
+00004310: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
+00004320: 7374 732e 5265 7370 6f6e 7365 0a20 2020  sts.Response.   
+00004330: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00004340: 2020 7570 6c6f 6164 5f72 6573 706f 6e73    upload_respons
+00004350: 6520 3d20 7365 6c66 2e75 706c 6f61 645f  e = self.upload_
+00004360: 7361 6d70 6c65 5f66 726f 6d5f 7572 6c28  sample_from_url(
+00004370: 6669 6c65 5f75 726c 3d66 696c 655f 7572  file_url=file_ur
+00004380: 6c2c 2063 7261 776c 6572 3d63 7261 776c  l, crawler=crawl
+00004390: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043d0: 2020 2020 2020 2020 2020 2020 2020 726c                rl
-000043e0: 5f63 6c6f 7564 5f73 616e 6462 6f78 5f70  _cloud_sandbox_p
-000043f0: 6c61 7466 6f72 6d3d 726c 5f63 6c6f 7564  latform=rl_cloud
-00004400: 5f73 616e 6462 6f78 5f70 6c61 7466 6f72  _sandbox_platfor
-00004410: 6d29 0a0a 2020 2020 2020 2020 7265 7370  m)..        resp
-00004420: 6f6e 7365 5f64 6574 6169 6c20 3d20 7570  onse_detail = up
-00004430: 6c6f 6164 5f72 6573 706f 6e73 652e 6a73  load_response.js
-00004440: 6f6e 2829 2e67 6574 2822 6465 7461 696c  on().get("detail
-00004450: 2229 0a20 2020 2020 2020 2074 6173 6b5f  ").        task_
-00004460: 6964 203d 2072 6573 706f 6e73 655f 6465  id = response_de
-00004470: 7461 696c 2e67 6574 2822 6964 2229 0a20  tail.get("id"). 
-00004480: 2020 2020 2020 2074 6173 6b5f 6964 203d         task_id =
-00004490: 2073 7472 2874 6173 6b5f 6964 290a 0a20   str(task_id).. 
-000044a0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-000044b0: 3d20 7365 6c66 2e67 6574 5f73 7562 6d69  = self.get_submi
-000044c0: 7474 6564 5f75 726c 5f72 6570 6f72 7428  tted_url_report(
-000044d0: 7461 736b 5f69 643d 7461 736b 5f69 642c  task_id=task_id,
-000044e0: 2072 6574 7279 3d72 6574 7279 290a 0a20   retry=retry).. 
-000044f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00004500: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
-00004510: 6765 745f 7265 7375 6c74 7328 7365 6c66  get_results(self
-00004520: 2c20 7361 6d70 6c65 5f68 6173 6865 732c  , sample_hashes,
-00004530: 2072 6574 7279 3d54 7275 652c 2066 6965   retry=True, fie
-00004540: 6c64 733d 4e6f 6e65 293a 0a20 2020 2020  lds=None):.     
-00004550: 2020 2022 2222 5448 4953 204d 4554 484f     """THIS METHO
-00004560: 4420 4953 2044 4550 5245 4341 5445 442e  D IS DEPRECATED.
-00004570: 0a20 2020 2020 2020 2055 7365 2067 6574  .        Use get
-00004580: 5f73 756d 6d61 7279 5f72 6570 6f72 745f  _summary_report_
-00004590: 7632 2066 6f72 2061 2073 756d 6d61 7279  v2 for a summary
-000045a0: 2061 6e61 6c79 7369 7320 7265 706f 7274   analysis report
-000045b0: 206f 720a 2020 2020 2020 2020 6765 745f   or.        get_
-000045c0: 6465 7461 696c 6564 5f72 6570 6f72 745f  detailed_report_
-000045d0: 7632 2066 6f72 2061 2064 6574 6169 6c65  v2 for a detaile
-000045e0: 6420 616e 616c 7973 6973 2072 6570 6f72  d analysis repor
-000045f0: 742e 0a0a 2020 2020 2020 2020 4163 6365  t...        Acce
-00004600: 7074 7320 6120 6c69 7374 206f 6620 6861  pts a list of ha
-00004610: 7368 6573 2061 6e64 2072 6574 7572 6e73  shes and returns
-00004620: 204a 534f 4e20 636f 6e74 6169 6e69 6e67   JSON containing
-00004630: 2061 2073 756d 6d61 7279 2072 6570 6f72   a summary repor
-00004640: 7420 666f 7220 6561 6368 206f 6620 7468  t for each of th
-00004650: 656d 2e0a 2020 2020 2020 2020 5468 6973  em..        This
-00004660: 206d 6574 686f 6420 7574 696c 697a 6573   method utilizes
-00004670: 2074 6865 2073 6574 206e 756d 6265 7220   the set number 
-00004680: 6f66 2072 6574 7269 6573 2061 6e64 2077  of retries and w
-00004690: 6169 7420 7469 6d65 2069 6e20 7365 636f  ait time in seco
-000046a0: 6e64 7320 746f 2074 696d 650a 2020 2020  nds to time.    
-000046b0: 2020 2020 6f75 7420 6966 2074 6865 2061      out if the a
-000046c0: 6e61 6c79 7369 7320 7265 7375 6c74 7320  nalysis results 
-000046d0: 6172 6520 6e6f 7420 7265 6164 792e 0a20  are not ready.. 
-000046e0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-000046f0: 6d20 7361 6d70 6c65 5f68 6173 6865 733a  m sample_hashes:
-00004700: 2068 6173 6820 7374 7269 6e67 206f 7220   hash string or 
-00004710: 6c69 7374 206f 6620 6861 7368 2073 7472  list of hash str
-00004720: 696e 6773 0a20 2020 2020 2020 2020 2020  ings.           
-00004730: 203a 7479 7065 2073 616d 706c 655f 6861   :type sample_ha
-00004740: 7368 6573 3a20 7374 7220 6f72 206c 6973  shes: str or lis
-00004750: 745b 7374 725d 0a20 2020 2020 2020 2020  t[str].         
-00004760: 2020 203a 7061 7261 6d20 7265 7472 793a     :param retry:
-00004770: 2069 6620 7365 7420 746f 2046 616c 7365   if set to False
-00004780: 2074 6865 7265 2077 696c 6c20 6f6e 6c79   there will only
-00004790: 2062 6520 6f6e 6520 7472 7920 6174 206f   be one try at o
-000047a0: 6274 6169 6e69 6e67 2074 6865 2061 6e61  btaining the ana
-000047b0: 6c79 7369 7320 7265 706f 7274 0a20 2020  lysis report.   
-000047c0: 2020 2020 2020 2020 203a 7479 7065 2072           :type r
-000047d0: 6574 7279 3a20 626f 6f6c 0a20 2020 2020  etry: bool.     
-000047e0: 2020 2020 2020 203a 7061 7261 6d20 6669         :param fi
-000047f0: 656c 6473 3a20 6c69 7374 206f 6620 4131  elds: list of A1
-00004800: 3030 3020 7265 706f 7274 2027 6669 656c  000 report 'fiel
-00004810: 6473 2720 746f 2071 7565 7279 0a20 2020  ds' to query.   
-00004820: 2020 2020 2020 2020 203a 7479 7065 2066           :type f
-00004830: 6965 6c64 733a 206c 6973 745b 7374 725d  ields: list[str]
-00004840: 0a20 2020 2020 2020 2020 2020 203a 7265  .            :re
-00004850: 7475 726e 3a20 3a63 6c61 7373 3a60 5265  turn: :class:`Re
-00004860: 7370 6f6e 7365 203c 5265 7370 6f6e 7365  sponse <Response
-00004870: 3e60 206f 626a 6563 740a 2020 2020 2020  >` object.      
-00004880: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
-00004890: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
-000048a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000048b0: 2020 2020 7761 726e 2822 5468 6973 206d      warn("This m
-000048c0: 6574 686f 6420 6973 2064 6570 7265 6361  ethod is depreca
-000048d0: 7465 642e 2055 7365 2067 6574 5f73 756d  ted. Use get_sum
-000048e0: 6d61 7279 5f72 6570 6f72 745f 7632 2066  mary_report_v2 f
-000048f0: 6f72 2061 2073 756d 6d61 7279 2061 6e61  or a summary ana
-00004900: 6c79 7369 7320 7265 706f 7274 206f 7220  lysis report or 
-00004910: 220a 2020 2020 2020 2020 2020 2020 2022  ".             "
-00004920: 6765 745f 6465 7461 696c 6564 5f72 6570  get_detailed_rep
-00004930: 6f72 745f 7632 2066 6f72 2061 2064 6574  ort_v2 for a det
-00004940: 6169 6c65 6420 616e 616c 7973 6973 2072  ailed analysis r
-00004950: 6570 6f72 7422 2c20 4465 7072 6563 6174  eport", Deprecat
-00004960: 696f 6e57 6172 6e69 6e67 290a 0a20 2020  ionWarning)..   
-00004970: 2020 2020 2069 6620 6669 656c 6473 2061       if fields a
-00004980: 6e64 206e 6f74 2069 7369 6e73 7461 6e63  nd not isinstanc
-00004990: 6528 6669 656c 6473 2c20 6c69 7374 293a  e(fields, list):
-000049a0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000049b0: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-000049c0: 6f72 2822 6669 656c 6473 2070 6172 616d  or("fields param
-000049d0: 6574 6572 206d 7573 7420 6265 2061 206c  eter must be a l
-000049e0: 6973 7420 6f66 2073 7472 696e 6773 2e22  ist of strings."
-000049f0: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-00004a00: 7420 6669 656c 6473 3a0a 2020 2020 2020  t fields:.      
-00004a10: 2020 2020 2020 6669 656c 6473 203d 2073        fields = s
-00004a20: 656c 662e 5f66 6965 6c64 730a 0a20 2020  elf._fields..   
-00004a30: 2020 2020 2069 6620 7265 7472 7920 6e6f       if retry no
-00004a40: 7420 696e 2028 5472 7565 2c20 4661 6c73  t in (True, Fals
-00004a50: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00004a60: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
-00004a70: 4572 726f 7228 2272 6574 7279 2070 6172  Error("retry par
-00004a80: 616d 6574 6572 206d 7573 7420 6265 2062  ameter must be b
-00004a90: 6f6f 6c65 616e 2e22 290a 0a20 2020 2020  oolean.")..     
-00004aa0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00004ab0: 2873 616d 706c 655f 6861 7368 6573 2c20  (sample_hashes, 
-00004ac0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00004ad0: 2020 7361 6d70 6c65 5f68 6173 6865 7320    sample_hashes 
-00004ae0: 3d20 5b73 616d 706c 655f 6861 7368 6573  = [sample_hashes
-00004af0: 5d0a 0a20 2020 2020 2020 2076 616c 6964  ]..        valid
-00004b00: 6174 655f 6861 7368 6573 280a 2020 2020  ate_hashes(.    
-00004b10: 2020 2020 2020 2020 6861 7368 5f69 6e70          hash_inp
-00004b20: 7574 3d73 616d 706c 655f 6861 7368 6573  ut=sample_hashes
-00004b30: 2c0a 2020 2020 2020 2020 2020 2020 616c  ,.            al
-00004b40: 6c6f 7765 645f 6861 7368 5f74 7970 6573  lowed_hash_types
-00004b50: 3d28 4d44 352c 2053 4841 312c 2053 4841  =(MD5, SHA1, SHA
-00004b60: 3235 362c 2053 4841 3531 3229 0a20 2020  256, SHA512).   
-00004b70: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00004b80: 7265 7472 6965 7320 3d20 7365 6c66 2e5f  retries = self._
-00004b90: 7265 7472 6965 7320 6966 2072 6574 7279  retries if retry
-00004ba0: 2065 6c73 6520 300a 0a20 2020 2020 2020   else 0..       
-00004bb0: 2061 6e61 6c79 7369 735f 6973 5f66 696e   analysis_is_fin
-00004bc0: 6973 6865 6420 3d20 4661 6c73 650a 0a20  ished = False.. 
-00004bd0: 2020 2020 2020 2066 6f72 2069 7465 7261         for itera
-00004be0: 7469 6f6e 2069 6e20 7261 6e67 6528 7265  tion in range(re
-00004bf0: 7472 6965 7320 2b20 3129 3a0a 2020 2020  tries + 1):.    
-00004c00: 2020 2020 2020 2020 6966 2069 7465 7261          if itera
-00004c10: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-00004c20: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-00004c30: 2873 656c 662e 5f77 6169 745f 7469 6d65  (self._wait_time
-00004c40: 5f73 6563 6f6e 6473 290a 0a20 2020 2020  _seconds)..     
-00004c50: 2020 2020 2020 2061 6e61 6c79 7369 735f         analysis_
-00004c60: 6973 5f66 696e 6973 6865 6420 3d20 7365  is_finished = se
-00004c70: 6c66 2e5f 5f61 6e61 6c79 7369 735f 6973  lf.__analysis_is
-00004c80: 5f66 696e 6973 6865 6428 7361 6d70 6c65  _finished(sample
-00004c90: 5f68 6173 6865 7329 0a20 2020 2020 2020  _hashes).       
-00004ca0: 2020 2020 2069 6620 616e 616c 7973 6973       if analysis
-00004cb0: 5f69 735f 6669 6e69 7368 6564 3a0a 2020  _is_finished:.  
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00004cd0: 6561 6b0a 0a20 2020 2020 2020 2069 6620  eak..        if 
-00004ce0: 6e6f 7420 616e 616c 7973 6973 5f69 735f  not analysis_is_
-00004cf0: 6669 6e69 7368 6564 3a0a 2020 2020 2020  finished:.      
-00004d00: 2020 2020 2020 7261 6973 6520 5265 7175        raise Requ
-00004d10: 6573 7454 696d 656f 7574 4572 726f 7228  estTimeoutError(
-00004d20: 2252 6570 6f72 7420 6665 7463 6869 6e67  "Report fetching
-00004d30: 2061 7474 656d 7074 7320 6669 6e69 7368   attempts finish
-00004d40: 6564 202d 2054 6865 2061 6e61 6c79 7369  ed - The analysi
-00004d50: 7320 7265 706f 7274 2069 7320 7374 696c  s report is stil
-00004d60: 6c20 6e6f 7420 7265 6164 7920 220a 2020  l not ready ".  
-00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d90: 2020 2020 226f 7220 7468 6520 7361 6d70      "or the samp
-00004da0: 6c65 2064 6f65 7320 6e6f 7420 6578 6973  le does not exis
-00004db0: 7420 6f6e 2074 6865 2061 7070 6c69 616e  t on the applian
-00004dc0: 6365 2e22 290a 0a20 2020 2020 2020 2075  ce.")..        u
-00004dd0: 726c 203d 2073 656c 662e 5f75 726c 2e66  rl = self._url.f
-00004de0: 6f72 6d61 7428 656e 6470 6f69 6e74 3d73  ormat(endpoint=s
-00004df0: 656c 662e 5f5f 5245 5355 4c54 535f 454e  elf.__RESULTS_EN
-00004e00: 4450 4f49 4e54 290a 0a20 2020 2020 2020  DPOINT)..       
-00004e10: 2064 6174 6120 3d20 7b0a 2020 2020 2020   data = {.      
-00004e20: 2020 2020 2020 2268 6173 685f 7661 6c75        "hash_valu
-00004e30: 6573 223a 2073 616d 706c 655f 6861 7368  es": sample_hash
-00004e40: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00004e50: 2266 6965 6c64 7322 3a20 6669 656c 6473  "fields": fields
-00004e60: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00004e70: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-00004e80: 656c 662e 5f5f 706f 7374 5f72 6571 7565  elf.__post_reque
-00004e90: 7374 2875 726c 3d75 726c 2c20 6461 7461  st(url=url, data
-00004ea0: 3d64 6174 6129 0a0a 2020 2020 2020 2020  =data)..        
-00004eb0: 7365 6c66 2e5f 5f72 6169 7365 5f6f 6e5f  self.__raise_on_
-00004ec0: 6572 726f 7228 7265 7370 6f6e 7365 290a  error(response).
-00004ed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004ee0: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
-00004ef0: 6620 6765 745f 7375 6d6d 6172 795f 7265  f get_summary_re
-00004f00: 706f 7274 5f76 3228 7365 6c66 2c20 7361  port_v2(self, sa
-00004f10: 6d70 6c65 5f68 6173 6865 732c 2072 6574  mple_hashes, ret
-00004f20: 7279 3d54 7275 652c 2066 6965 6c64 733d  ry=True, fields=
-00004f30: 4e6f 6e65 2c20 696e 636c 7564 655f 6e65  None, include_ne
-00004f40: 7477 6f72 6b74 6872 6561 7469 6e74 656c  tworkthreatintel
-00004f50: 6c69 6765 6e63 653d 5472 7565 2c0a 2020  ligence=True,.  
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 2020 2020 2020 2020 736b 6970              skip
-00004f80: 5f72 6561 6e61 6c79 7369 733d 4661 6c73  _reanalysis=Fals
-00004f90: 6529 3a0a 2020 2020 2020 2020 2222 2241  e):.        """A
-00004fa0: 6363 6570 7473 2061 2073 696e 676c 6520  ccepts a single 
-00004fb0: 6861 7368 206f 7220 6120 6c69 7374 206f  hash or a list o
-00004fc0: 6620 6861 7368 6573 2061 6e64 2072 6574  f hashes and ret
-00004fd0: 7572 6e73 204a 534f 4e20 636f 6e74 6169  urns JSON contai
-00004fe0: 6e69 6e67 2061 2073 756d 6d61 7279 2072  ning a summary r
-00004ff0: 6570 6f72 7420 666f 7220 6561 6368 206f  eport for each o
-00005000: 6620 7468 656d 2e0a 2020 2020 2020 2020  f them..        
-00005010: 5468 6973 206d 6574 686f 6420 7574 696c  This method util
-00005020: 697a 6573 2074 6865 2073 6574 206e 756d  izes the set num
-00005030: 6265 7220 6f66 2072 6574 7269 6573 2061  ber of retries a
-00005040: 6e64 2077 6169 7420 7469 6d65 2069 6e20  nd wait time in 
-00005050: 7365 636f 6e64 7320 746f 2074 696d 650a  seconds to time.
-00005060: 2020 2020 2020 2020 6f75 7420 6966 2074          out if t
-00005070: 6865 2061 6e61 6c79 7369 7320 7265 7375  he analysis resu
-00005080: 6c74 7320 6172 6520 6e6f 7420 7265 6164  lts are not read
-00005090: 792e 0a20 2020 2020 2020 2020 2020 203a  y..            :
-000050a0: 7061 7261 6d20 7361 6d70 6c65 5f68 6173  param sample_has
-000050b0: 6865 733a 2068 6173 6820 7374 7269 6e67  hes: hash string
-000050c0: 206f 7220 6c69 7374 206f 6620 6861 7368   or list of hash
-000050d0: 2073 7472 696e 6773 0a20 2020 2020 2020   strings.       
-000050e0: 2020 2020 203a 7479 7065 2073 616d 706c       :type sampl
-000050f0: 655f 6861 7368 6573 3a20 7374 7220 6f72  e_hashes: str or
-00005100: 206c 6973 745b 7374 725d 0a20 2020 2020   list[str].     
-00005110: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
-00005120: 7472 793a 2069 6620 7365 7420 746f 2046  try: if set to F
-00005130: 616c 7365 2074 6865 7265 2077 696c 6c20  alse there will 
-00005140: 6f6e 6c79 2062 6520 6f6e 6520 7472 7920  only be one try 
-00005150: 6174 206f 6274 6169 6e69 6e67 2074 6865  at obtaining the
-00005160: 2061 6e61 6c79 7369 7320 7265 706f 7274   analysis report
-00005170: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00005180: 7065 2072 6574 7279 3a20 626f 6f6c 0a20  pe retry: bool. 
-00005190: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-000051a0: 6d20 6669 656c 6473 3a20 6c69 7374 206f  m fields: list o
-000051b0: 6620 4131 3030 3020 7265 706f 7274 2027  f A1000 report '
-000051c0: 6669 656c 6473 2720 746f 2071 7565 7279  fields' to query
-000051d0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-000051e0: 7065 2066 6965 6c64 733a 206c 6973 745b  pe fields: list[
-000051f0: 7374 725d 0a20 2020 2020 2020 2020 2020  str].           
-00005200: 203a 7061 7261 6d20 696e 636c 7564 655f   :param include_
-00005210: 6e65 7477 6f72 6b74 6872 6561 7469 6e74  networkthreatint
-00005220: 656c 6c69 6765 6e63 653a 2069 6e63 6c75  elligence: inclu
-00005230: 6465 206e 6574 776f 726b 2074 6872 6561  de network threa
-00005240: 7420 696e 7465 6c6c 6967 656e 6365 2069  t intelligence i
-00005250: 6e20 7468 6520 7375 6d6d 6172 7920 7265  n the summary re
-00005260: 706f 7274 0a20 2020 2020 2020 2020 2020  port.           
-00005270: 203a 7479 7065 2069 6e63 6c75 6465 5f6e   :type include_n
-00005280: 6574 776f 726b 7468 7265 6174 696e 7465  etworkthreatinte
-00005290: 6c6c 6967 656e 6365 3a20 626f 6f6c 0a20  lligence: bool. 
-000052a0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-000052b0: 6d20 736b 6970 5f72 6561 6e61 6c79 7369  m skip_reanalysi
-000052c0: 733a 2073 6b69 7020 7361 6d70 6c65 2072  s: skip sample r
-000052d0: 6561 6e61 6c79 7369 7320 7768 656e 2066  eanalysis when f
-000052e0: 6574 6368 696e 6720 7468 6520 7375 6d6d  etching the summ
-000052f0: 6172 7920 7265 706f 7274 0a20 2020 2020  ary report.     
-00005300: 2020 2020 2020 203a 7479 7065 2073 6b69         :type ski
-00005310: 705f 7265 616e 616c 7973 6973 3a20 626f  p_reanalysis: bo
-00005320: 6f6c 0a20 2020 2020 2020 2020 2020 203a  ol.            :
-00005330: 7265 7475 726e 3a20 3a63 6c61 7373 3a60  return: :class:`
-00005340: 5265 7370 6f6e 7365 203c 5265 7370 6f6e  Response <Respon
-00005350: 7365 3e60 206f 626a 6563 740a 2020 2020  se>` object.    
-00005360: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00005370: 7265 7175 6573 7473 2e52 6573 706f 6e73  requests.Respons
-00005380: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
-00005390: 2020 2020 2020 6966 2066 6965 6c64 7320        if fields 
-000053a0: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
-000053b0: 6365 2866 6965 6c64 732c 206c 6973 7429  ce(fields, list)
-000053c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000053d0: 6973 6520 5772 6f6e 6749 6e70 7574 4572  ise WrongInputEr
-000053e0: 726f 7228 2266 6965 6c64 7320 7061 7261  ror("fields para
-000053f0: 6d65 7465 7220 6d75 7374 2062 6520 6120  meter must be a 
-00005400: 6c69 7374 206f 6620 7374 7269 6e67 732e  list of strings.
-00005410: 2229 0a0a 2020 2020 2020 2020 6966 206e  ")..        if n
-00005420: 6f74 2066 6965 6c64 733a 0a20 2020 2020  ot fields:.     
-00005430: 2020 2020 2020 2066 6965 6c64 7320 3d20         fields = 
-00005440: 7365 6c66 2e5f 6669 656c 6473 5f76 320a  self._fields_v2.
-00005450: 0a20 2020 2020 2020 2069 6620 7265 7472  .        if retr
-00005460: 7920 6e6f 7420 696e 2028 5472 7565 2c20  y not in (True, 
-00005470: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
-00005480: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00005490: 6e70 7574 4572 726f 7228 2272 6574 7279  nputError("retry
-000054a0: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
-000054b0: 6265 2062 6f6f 6c65 616e 2e22 290a 0a20  be boolean.").. 
-000054c0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-000054d0: 616e 6365 2873 616d 706c 655f 6861 7368  ance(sample_hash
-000054e0: 6573 2c20 7374 7229 3a0a 2020 2020 2020  es, str):.      
-000054f0: 2020 2020 2020 7361 6d70 6c65 5f68 6173        sample_has
-00005500: 6865 7320 3d20 5b73 616d 706c 655f 6861  hes = [sample_ha
-00005510: 7368 6573 5d0a 0a20 2020 2020 2020 2076  shes]..        v
-00005520: 616c 6964 6174 655f 6861 7368 6573 280a  alidate_hashes(.
-00005530: 2020 2020 2020 2020 2020 2020 6861 7368              hash
-00005540: 5f69 6e70 7574 3d73 616d 706c 655f 6861  _input=sample_ha
-00005550: 7368 6573 2c0a 2020 2020 2020 2020 2020  shes,.          
-00005560: 2020 616c 6c6f 7765 645f 6861 7368 5f74    allowed_hash_t
-00005570: 7970 6573 3d28 4d44 352c 2053 4841 312c  ypes=(MD5, SHA1,
-00005580: 2053 4841 3235 362c 2053 4841 3531 3229   SHA256, SHA512)
-00005590: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000055a0: 2020 2020 7265 7472 6965 7320 3d20 7365      retries = se
-000055b0: 6c66 2e5f 7265 7472 6965 7320 6966 2072  lf._retries if r
-000055c0: 6574 7279 2065 6c73 6520 300a 0a20 2020  etry else 0..   
-000055d0: 2020 2020 2061 6e61 6c79 7369 735f 6973       analysis_is
-000055e0: 5f66 696e 6973 6865 6420 3d20 4661 6c73  _finished = Fals
-000055f0: 650a 0a20 2020 2020 2020 2066 6f72 2069  e..        for i
-00005600: 7465 7261 7469 6f6e 2069 6e20 7261 6e67  teration in rang
-00005610: 6528 7265 7472 6965 7320 2b20 3129 3a0a  e(retries + 1):.
-00005620: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00005630: 7465 7261 7469 6f6e 3a0a 2020 2020 2020  teration:.      
-00005640: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
-00005650: 6c65 6570 2873 656c 662e 5f77 6169 745f  leep(self._wait_
-00005660: 7469 6d65 5f73 6563 6f6e 6473 290a 0a20  time_seconds).. 
-00005670: 2020 2020 2020 2020 2020 2061 6e61 6c79             analy
-00005680: 7369 735f 6973 5f66 696e 6973 6865 6420  sis_is_finished 
-00005690: 3d20 7365 6c66 2e5f 5f61 6e61 6c79 7369  = self.__analysi
-000056a0: 735f 6973 5f66 696e 6973 6865 6428 7361  s_is_finished(sa
-000056b0: 6d70 6c65 5f68 6173 6865 7329 0a20 2020  mple_hashes).   
-000056c0: 2020 2020 2020 2020 2069 6620 616e 616c           if anal
-000056d0: 7973 6973 5f69 735f 6669 6e69 7368 6564  ysis_is_finished
-000056e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000056f0: 2020 6272 6561 6b0a 0a20 2020 2020 2020    break..       
-00005700: 2069 6620 6e6f 7420 616e 616c 7973 6973   if not analysis
-00005710: 5f69 735f 6669 6e69 7368 6564 3a0a 2020  _is_finished:.  
-00005720: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00005730: 5265 7175 6573 7454 696d 656f 7574 4572  RequestTimeoutEr
-00005740: 726f 7228 2252 6570 6f72 7420 6665 7463  ror("Report fetc
-00005750: 6869 6e67 2061 7474 656d 7074 7320 6669  hing attempts fi
-00005760: 6e69 7368 6564 202d 2054 6865 2061 6e61  nished - The ana
-00005770: 6c79 7369 7320 7265 706f 7274 2069 7320  lysis report is 
-00005780: 7374 696c 6c20 6e6f 7420 7265 6164 7920  still not ready 
-00005790: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057b0: 2020 2020 2020 2020 226f 7220 7468 6520          "or the 
-000057c0: 7361 6d70 6c65 2064 6f65 7320 6e6f 7420  sample does not 
-000057d0: 6578 6973 7420 6f6e 2074 6865 2061 7070  exist on the app
-000057e0: 6c69 616e 6365 2e22 290a 0a20 2020 2020  liance.")..     
-000057f0: 2020 2075 726c 203d 2073 656c 662e 5f75     url = self._u
-00005800: 726c 2e66 6f72 6d61 7428 656e 6470 6f69  rl.format(endpoi
-00005810: 6e74 3d73 656c 662e 5f5f 5355 4d4d 4152  nt=self.__SUMMAR
-00005820: 595f 5245 504f 5254 5f45 4e44 504f 494e  Y_REPORT_ENDPOIN
-00005830: 545f 5632 290a 0a20 2020 2020 2020 2069  T_V2)..        i
-00005840: 6620 696e 636c 7564 655f 6e65 7477 6f72  f include_networ
-00005850: 6b74 6872 6561 7469 6e74 656c 6c69 6765  kthreatintellige
-00005860: 6e63 6520 6e6f 7420 696e 2028 5472 7565  nce not in (True
-00005870: 2c20 4661 6c73 6529 3a0a 2020 2020 2020  , False):.      
-00005880: 2020 2020 2020 7261 6973 6520 5772 6f6e        raise Wron
-00005890: 6749 6e70 7574 4572 726f 7228 2269 6e63  gInputError("inc
-000058a0: 6c75 6465 5f6e 6574 776f 726b 7468 7265  lude_networkthre
-000058b0: 6174 696e 7465 6c6c 6967 656e 6365 2070  atintelligence p
-000058c0: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
-000058d0: 2062 6f6f 6c65 616e 2e22 290a 0a20 2020   boolean.")..   
-000058e0: 2020 2020 2069 6620 696e 636c 7564 655f       if include_
-000058f0: 6e65 7477 6f72 6b74 6872 6561 7469 6e74  networkthreatint
-00005900: 656c 6c69 6765 6e63 6520 616e 6420 5c0a  elligence and \.
-00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005920: 2822 6e65 7477 6f72 6b74 6872 6561 7469  ("networkthreati
-00005930: 6e74 656c 6c69 6765 6e63 6522 206e 6f74  ntelligence" not
-00005940: 2069 6e20 6669 656c 6473 206f 7220 2264   in fields or "d
-00005950: 6f6d 6169 6e74 6872 6561 7469 6e74 656c  omainthreatintel
-00005960: 6c69 6765 6e63 6522 206e 6f74 2069 6e20  ligence" not in 
-00005970: 6669 656c 6473 293a 0a20 2020 2020 2020  fields):.       
-00005980: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
-00005990: 496e 7075 7445 7272 6f72 2822 4966 2069  InputError("If i
-000059a0: 6e63 6c75 6465 5f6e 6574 776f 726b 7468  nclude_networkth
-000059b0: 7265 6174 696e 7465 6c6c 6967 656e 6365  reatintelligence
-000059c0: 2069 7320 7365 7420 746f 2054 7275 652c   is set to True,
-000059d0: 2074 6865 2066 6965 6c64 7320 6c69 7374   the fields list
-000059e0: 206d 7573 7420 696e 636c 7564 6520 220a   must include ".
-000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2020 2262 6f74 6820 276e 6574 776f 726b    "both 'network
-00005a20: 7468 7265 6174 696e 7465 6c6c 6967 656e  threatintelligen
-00005a30: 6365 2720 616e 6420 2764 6f6d 6169 6e74  ce' and 'domaint
-00005a40: 6872 6561 7469 6e74 656c 6c69 6765 6e63  hreatintelligenc
-00005a50: 6527 2e22 290a 0a20 2020 2020 2020 2069  e'.")..        i
-00005a60: 6620 736b 6970 5f72 6561 6e61 6c79 7369  f skip_reanalysi
-00005a70: 7320 6e6f 7420 696e 2028 5472 7565 2c20  s not in (True, 
-00005a80: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
-00005a90: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00005aa0: 6e70 7574 4572 726f 7228 2273 6b69 705f  nputError("skip_
-00005ab0: 7265 616e 616c 7973 6973 2070 6172 616d  reanalysis param
-00005ac0: 6574 6572 206d 7573 7420 6265 2062 6f6f  eter must be boo
-00005ad0: 6c65 616e 2e22 290a 0a20 2020 2020 2020  lean.")..       
-00005ae0: 2064 6174 6120 3d20 7b0a 2020 2020 2020   data = {.      
-00005af0: 2020 2020 2020 2268 6173 685f 7661 6c75        "hash_valu
-00005b00: 6573 223a 2073 616d 706c 655f 6861 7368  es": sample_hash
-00005b10: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00005b20: 2266 6965 6c64 7322 3a20 6669 656c 6473  "fields": fields
-00005b30: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
-00005b40: 6e63 6c75 6465 5f6e 6574 776f 726b 7468  nclude_networkth
-00005b50: 7265 6174 696e 7465 6c6c 6967 656e 6365  reatintelligence
-00005b60: 223a 2073 7472 2869 6e63 6c75 6465 5f6e  ": str(include_n
-00005b70: 6574 776f 726b 7468 7265 6174 696e 7465  etworkthreatinte
-00005b80: 6c6c 6967 656e 6365 292e 6c6f 7765 7228  lligence).lower(
-00005b90: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-00005ba0: 736b 6970 5f72 6561 6e61 6c79 7369 7322  skip_reanalysis"
-00005bb0: 3a20 7374 7228 736b 6970 5f72 6561 6e61  : str(skip_reana
-00005bc0: 6c79 7369 7329 2e6c 6f77 6572 2829 0a20  lysis).lower(). 
-00005bd0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00005be0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00005bf0: 662e 5f5f 706f 7374 5f72 6571 7565 7374  f.__post_request
-00005c00: 2875 726c 3d75 726c 2c20 6461 7461 3d64  (url=url, data=d
-00005c10: 6174 6129 0a0a 2020 2020 2020 2020 7365  ata)..        se
-00005c20: 6c66 2e5f 5f72 6169 7365 5f6f 6e5f 6572  lf.__raise_on_er
-00005c30: 726f 7228 7265 7370 6f6e 7365 290a 0a20  ror(response).. 
-00005c40: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00005c50: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
-00005c60: 7570 6c6f 6164 5f73 616d 706c 655f 616e  upload_sample_an
-00005c70: 645f 6765 745f 7265 7375 6c74 7328 7365  d_get_results(se
-00005c80: 6c66 2c20 6669 6c65 5f70 6174 683d 4e6f  lf, file_path=No
-00005c90: 6e65 2c20 6669 6c65 5f73 6f75 7263 653d  ne, file_source=
-00005ca0: 4e6f 6e65 2c20 7265 7472 793d 5472 7565  None, retry=True
-00005cb0: 2c20 6375 7374 6f6d 5f66 696c 656e 616d  , custom_filenam
-00005cc0: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00005cf0: 6773 3d4e 6f6e 652c 2063 6f6d 6d65 6e74  gs=None, comment
-00005d00: 3d4e 6f6e 652c 2063 6c6f 7564 5f61 6e61  =None, cloud_ana
-00005d10: 6c79 7369 733d 5472 7565 293a 0a20 2020  lysis=True):.   
-00005d20: 2020 2020 2022 2222 5448 4953 204d 4554       """THIS MET
-00005d30: 484f 4420 4953 2044 4550 5245 4341 5445  HOD IS DEPRECATE
-00005d40: 442e 2055 7365 2075 706c 6f61 645f 7361  D. Use upload_sa
-00005d50: 6d70 6c65 5f61 6e64 5f67 6574 5f73 756d  mple_and_get_sum
-00005d60: 6d61 7279 5f72 6570 6f72 745f 7632 2069  mary_report_v2 i
-00005d70: 6e73 7465 6164 2e0a 0a20 2020 2020 2020  nstead...       
-00005d80: 2041 6363 6570 7473 2065 6974 6865 7220   Accepts either 
-00005d90: 6120 6669 6c65 2070 6174 6820 7374 7269  a file path stri
-00005da0: 6e67 206f 7220 616e 206f 7065 6e20 6669  ng or an open fi
-00005db0: 6c65 2069 6e20 2772 6227 206d 6f64 6520  le in 'rb' mode 
-00005dc0: 666f 7220 6669 6c65 2075 706c 6f61 6420  for file upload 
-00005dd0: 616e 6420 7265 7475 726e 730a 2020 2020  and returns.    
-00005de0: 2020 2020 616e 2061 6e61 6c79 7369 7320      an analysis 
-00005df0: 7265 706f 7274 2072 6573 706f 6e73 652e  report response.
-00005e00: 2054 6869 7320 6d65 7468 6f64 2063 6f6d   This method com
-00005e10: 6269 6e65 7320 7570 6c6f 6164 696e 6720  bines uploading 
-00005e20: 6120 7361 6d70 6c65 2061 6e64 206f 6274  a sample and obt
-00005e30: 6169 6e69 6e67 2074 6865 2061 6e61 6c79  aining the analy
-00005e40: 7369 7320 7265 7375 6c74 732e 0a20 2020  sis results..   
-00005e50: 2020 2020 2041 6464 6974 696f 6e61 6c20       Additional 
-00005e60: 6669 656c 6473 2063 616e 2062 6520 7072  fields can be pr
-00005e70: 6f76 6964 6564 2e0a 2020 2020 2020 2020  ovided..        
-00005e80: 5468 6520 7265 7375 6c74 206f 6274 6169  The result obtai
-00005e90: 6e69 6e67 2061 6374 696f 6e20 6f66 2074  ning action of t
-00005ea0: 6869 7320 6d65 7468 6f64 2075 7469 6c69  his method utili
-00005eb0: 7a65 7320 7468 6520 7365 7420 6e75 6d62  zes the set numb
-00005ec0: 6572 206f 6620 7265 7472 6965 7320 616e  er of retries an
-00005ed0: 6420 7761 6974 2074 696d 6520 696e 2073  d wait time in s
-00005ee0: 6563 6f6e 6473 2074 6f20 7469 6d65 0a20  econds to time. 
-00005ef0: 2020 2020 2020 206f 7574 2069 6620 7468         out if th
-00005f00: 6520 616e 616c 7973 6973 2072 6573 756c  e analysis resul
-00005f10: 7473 2061 7265 206e 6f74 2072 6561 6479  ts are not ready
-00005f20: 2e0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
-00005f30: 6172 616d 2066 696c 655f 7061 7468 3a20  aram file_path: 
-00005f40: 6669 6c65 2070 6174 680a 2020 2020 2020  file path.      
-00005f50: 2020 2020 2020 3a74 7970 6520 6669 6c65        :type file
-00005f60: 5f70 6174 683a 2073 7472 0a20 2020 2020  _path: str.     
-00005f70: 2020 2020 2020 203a 7061 7261 6d20 6669         :param fi
-00005f80: 6c65 5f73 6f75 7263 653a 206f 7065 6e20  le_source: open 
-00005f90: 6669 6c65 0a20 2020 2020 2020 2020 2020  file.           
-00005fa0: 203a 7479 7065 2066 696c 655f 736f 7572   :type file_sour
-00005fb0: 6365 3a20 6669 6c65 206f 7220 4269 6e61  ce: file or Bina
-00005fc0: 7279 494f 0a20 2020 2020 2020 2020 2020  ryIO.           
-00005fd0: 203a 7061 7261 6d20 7265 7472 793a 2069   :param retry: i
-00005fe0: 6620 7365 7420 746f 2046 616c 7365 2074  f set to False t
-00005ff0: 6865 7265 2077 696c 6c20 6f6e 6c79 2062  here will only b
-00006000: 6520 6f6e 6520 7472 7920 6174 206f 6274  e one try at obt
-00006010: 6169 6e69 6e67 2074 6865 2061 6e61 6c79  aining the analy
-00006020: 7369 7320 7265 706f 7274 0a20 2020 2020  sis report.     
-00006030: 2020 2020 2020 203a 7479 7065 2072 6574         :type ret
-00006040: 7279 3a20 626f 6f6c 0a20 2020 2020 2020  ry: bool.       
-00006050: 2020 2020 203a 7061 7261 6d20 6375 7374       :param cust
-00006060: 6f6d 5f66 696c 656e 616d 653a 2063 7573  om_filename: cus
-00006070: 746f 6d20 6669 6c65 206e 616d 6520 666f  tom file name fo
-00006080: 7220 7570 6c6f 6164 0a20 2020 2020 2020  r upload.       
-00006090: 2020 2020 203a 7479 7065 2063 7573 746f       :type custo
-000060a0: 6d5f 6669 6c65 6e61 6d65 3a20 7374 720a  m_filename: str.
-000060b0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-000060c0: 616d 2074 6167 733a 2061 2073 7472 696e  am tags: a strin
-000060d0: 6720 6f66 2063 6f6d 6d61 2073 6570 6172  g of comma separ
-000060e0: 6174 6564 2074 6167 730a 2020 2020 2020  ated tags.      
-000060f0: 2020 2020 2020 3a74 7970 6520 7461 6773        :type tags
-00006100: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-00006110: 2020 3a70 6172 616d 2063 6f6d 6d65 6e74    :param comment
-00006120: 3a20 636f 6d6d 656e 7420 7374 7269 6e67  : comment string
-00006130: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00006140: 7065 2063 6f6d 6d65 6e74 3a20 7374 720a  pe comment: str.
-00006150: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00006160: 616d 2063 6c6f 7564 5f61 6e61 6c79 7369  am cloud_analysi
-00006170: 733a 2075 7365 2063 6c6f 7564 2061 6e61  s: use cloud ana
-00006180: 6c79 7369 730a 2020 2020 2020 2020 2020  lysis.          
-00006190: 2020 3a74 7970 6520 636c 6f75 645f 616e    :type cloud_an
-000061a0: 616c 7973 6973 3a20 626f 6f6c 0a20 2020  alysis: bool.   
-000061b0: 2020 2020 2020 2020 203a 7265 7475 726e           :return
-000061c0: 3a20 7265 7370 6f6e 7365 0a20 2020 2020  : response.     
-000061d0: 2020 2020 2020 203a 7274 7970 653a 2072         :rtype: r
-000061e0: 6571 7565 7374 732e 5265 7370 6f6e 7365  equests.Response
-000061f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006200: 2020 2020 2077 6172 6e28 2254 6869 7320       warn("This 
-00006210: 6d65 7468 6f64 2069 7320 6465 7072 6563  method is deprec
-00006220: 6174 6564 2e20 5573 6520 7570 6c6f 6164  ated. Use upload
-00006230: 5f73 616d 706c 655f 616e 645f 6765 745f  _sample_and_get_
-00006240: 7375 6d6d 6172 795f 7265 706f 7274 5f76  summary_report_v
-00006250: 3220 696e 7374 6561 642e 222c 2044 6570  2 instead.", Dep
-00006260: 7265 6361 7469 6f6e 5761 726e 696e 6729  recationWarning)
-00006270: 0a0a 2020 2020 2020 2020 6966 2028 6669  ..        if (fi
-00006280: 6c65 5f70 6174 6820 616e 6420 6669 6c65  le_path and file
-00006290: 5f73 6f75 7263 6529 206f 7220 286e 6f74  _source) or (not
-000062a0: 2066 696c 655f 7061 7468 2061 6e64 206e   file_path and n
-000062b0: 6f74 2066 696c 655f 736f 7572 6365 293a  ot file_source):
-000062c0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000062d0: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-000062e0: 6f72 2822 4569 7468 6572 2066 696c 655f  or("Either file_
-000062f0: 7061 7468 206f 7220 6669 6c65 5f73 6f75  path or file_sou
-00006300: 7263 6520 7061 7261 6d65 7465 7220 6d75  rce parameter mu
-00006310: 7374 2062 6520 7072 6f76 6964 6564 2e20  st be provided. 
-00006320: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00006330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006340: 2020 2020 2255 7369 6e67 2062 6f74 6820      "Using both 
-00006350: 6f72 206e 6f6e 6520 6f66 2074 6865 2070  or none of the p
-00006360: 6172 616d 6574 6572 7320 696e 2073 6f74  arameters in sot
-00006370: 2061 6c6c 6f77 6564 2e22 290a 0a20 2020   allowed.")..   
-00006380: 2020 2020 2069 6620 6669 6c65 5f70 6174       if file_pat
-00006390: 683a 0a20 2020 2020 2020 2020 2020 2075  h:.            u
-000063a0: 706c 6f61 645f 7265 7370 6f6e 7365 203d  pload_response =
-000063b0: 2073 656c 662e 7570 6c6f 6164 5f73 616d   self.upload_sam
-000063c0: 706c 655f 6672 6f6d 5f70 6174 6828 6669  ple_from_path(fi
-000063d0: 6c65 5f70 6174 682c 2063 7573 746f 6d5f  le_path, custom_
-000063e0: 6669 6c65 6e61 6d65 2c20 7461 6773 2c20  filename, tags, 
-000063f0: 636f 6d6d 656e 742c 2063 6c6f 7564 5f61  comment, cloud_a
-00006400: 6e61 6c79 7369 7329 0a20 2020 2020 2020  nalysis).       
-00006410: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00006420: 2020 2075 706c 6f61 645f 7265 7370 6f6e     upload_respon
-00006430: 7365 203d 2073 656c 662e 7570 6c6f 6164  se = self.upload
-00006440: 5f73 616d 706c 655f 6672 6f6d 5f66 696c  _sample_from_fil
-00006450: 6528 6669 6c65 5f73 6f75 7263 652c 2063  e(file_source, c
-00006460: 7573 746f 6d5f 6669 6c65 6e61 6d65 2c20  ustom_filename, 
-00006470: 7461 6773 2c20 636f 6d6d 656e 742c 2063  tags, comment, c
-00006480: 6c6f 7564 5f61 6e61 6c79 7369 7329 0a0a  loud_analysis)..
-00006490: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-000064a0: 5f64 6574 6169 6c20 3d20 7570 6c6f 6164  _detail = upload
-000064b0: 5f72 6573 706f 6e73 652e 6a73 6f6e 2829  _response.json()
-000064c0: 2e67 6574 2822 6465 7461 696c 2229 0a20  .get("detail"). 
-000064d0: 2020 2020 2020 2073 6861 3120 3d20 7265         sha1 = re
-000064e0: 7370 6f6e 7365 5f64 6574 6169 6c2e 6765  sponse_detail.ge
-000064f0: 7428 2273 6861 3122 290a 2020 2020 2020  t("sha1").      
-00006500: 2020 7368 6131 203d 2073 7472 2873 6861    sha1 = str(sha
-00006510: 3129 0a0a 2020 2020 2020 2020 7265 7370  1)..        resp
-00006520: 6f6e 7365 203d 2073 656c 662e 6765 745f  onse = self.get_
-00006530: 7265 7375 6c74 7328 0a20 2020 2020 2020  results(.       
-00006540: 2020 2020 2073 616d 706c 655f 6861 7368       sample_hash
-00006550: 6573 3d5b 7368 6131 5d2c 0a20 2020 2020  es=[sha1],.     
-00006560: 2020 2020 2020 2072 6574 7279 3d72 6574         retry=ret
-00006570: 7279 0a20 2020 2020 2020 2029 0a0a 2020  ry.        )..  
-00006580: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00006590: 706f 6e73 650a 0a20 2020 2064 6566 2075  ponse..    def u
-000065a0: 706c 6f61 645f 7361 6d70 6c65 5f61 6e64  pload_sample_and
-000065b0: 5f67 6574 5f73 756d 6d61 7279 5f72 6570  _get_summary_rep
-000065c0: 6f72 745f 7632 2873 656c 662c 2066 696c  ort_v2(self, fil
-000065d0: 655f 7061 7468 3d4e 6f6e 652c 2066 696c  e_path=None, fil
-000065e0: 655f 736f 7572 6365 3d4e 6f6e 652c 2072  e_source=None, r
-000065f0: 6574 7279 3d54 7275 652c 2066 6965 6c64  etry=True, field
-00006600: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006630: 2020 2020 2020 2020 696e 636c 7564 655f          include_
-00006640: 6e65 7477 6f72 6b74 6872 6561 7469 6e74  networkthreatint
-00006650: 656c 6c69 6765 6e63 653d 5472 7565 2c20  elligence=True, 
-00006660: 736b 6970 5f72 6561 6e61 6c79 7369 733d  skip_reanalysis=
-00006670: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066a0: 2020 2020 2020 2063 7573 746f 6d5f 6669         custom_fi
-000066b0: 6c65 6e61 6d65 3d4e 6f6e 652c 2074 6167  lename=None, tag
-000066c0: 733d 4e6f 6e65 2c20 636f 6d6d 656e 743d  s=None, comment=
-000066d0: 4e6f 6e65 2c20 636c 6f75 645f 616e 616c  None, cloud_anal
-000066e0: 7973 6973 3d54 7275 652c 0a20 2020 2020  ysis=True,.     
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006710: 2020 2020 2020 2020 2020 2061 7263 6869             archi
-00006720: 7665 5f70 6173 7377 6f72 643d 4e6f 6e65  ve_password=None
-00006730: 2c20 726c 5f63 6c6f 7564 5f73 616e 6462  , rl_cloud_sandb
-00006740: 6f78 5f70 6c61 7466 6f72 6d3d 4e6f 6e65  ox_platform=None
-00006750: 293a 0a20 2020 2020 2020 2022 2222 4163  ):.        """Ac
-00006760: 6365 7074 7320 6569 7468 6572 2061 2066  cepts either a f
-00006770: 696c 6520 7061 7468 2073 7472 696e 6720  ile path string 
-00006780: 6f72 2061 6e20 6f70 656e 2066 696c 6520  or an open file 
-00006790: 696e 2027 7262 2720 6d6f 6465 2066 6f72  in 'rb' mode for
-000067a0: 2066 696c 6520 7570 6c6f 6164 2061 6e64   file upload and
-000067b0: 2072 6574 7572 6e73 2061 2073 756d 6d61   returns a summa
-000067c0: 7279 2061 6e61 6c79 7369 730a 2020 2020  ry analysis.    
-000067d0: 2020 2020 7265 706f 7274 2072 6573 706f      report respo
-000067e0: 6e73 652e 2054 6869 7320 6d65 7468 6f64  nse. This method
-000067f0: 2063 6f6d 6269 6e65 7320 7570 6c6f 6164   combines upload
-00006800: 696e 6720 6120 7361 6d70 6c65 2061 6e64  ing a sample and
-00006810: 206f 6274 6169 6e69 6e67 2074 6865 2073   obtaining the s
-00006820: 756d 6d61 7279 2061 6e61 6c79 7369 7320  ummary analysis 
-00006830: 7265 706f 7274 2e0a 2020 2020 2020 2020  report..        
-00006840: 4164 6469 7469 6f6e 616c 2066 6965 6c64  Additional field
-00006850: 7320 6361 6e20 6265 2070 726f 7669 6465  s can be provide
-00006860: 642e 0a20 2020 2020 2020 2054 6865 2072  d..        The r
-00006870: 6573 756c 7420 6665 7463 6869 6e67 2061  esult fetching a
-00006880: 6374 696f 6e20 6f66 2074 6869 7320 6d65  ction of this me
-00006890: 7468 6f64 2075 7469 6c69 7a65 7320 7468  thod utilizes th
-000068a0: 6520 7365 7420 6e75 6d62 6572 206f 6620  e set number of 
-000068b0: 7265 7472 6965 7320 616e 6420 7761 6974  retries and wait
-000068c0: 2074 696d 6520 696e 2073 6563 6f6e 6473   time in seconds
-000068d0: 2074 6f20 7469 6d65 0a20 2020 2020 2020   to time.       
-000068e0: 206f 7574 2069 6620 7468 6520 616e 616c   out if the anal
-000068f0: 7973 6973 2072 6573 756c 7473 2061 7265  ysis results are
-00006900: 206e 6f74 2072 6561 6479 2e0a 2020 2020   not ready..    
-00006910: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00006920: 696c 655f 7061 7468 3a20 6669 6c65 2070  ile_path: file p
-00006930: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
-00006940: 3a74 7970 6520 6669 6c65 5f70 6174 683a  :type file_path:
-00006950: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
-00006960: 203a 7061 7261 6d20 6669 6c65 5f73 6f75   :param file_sou
-00006970: 7263 653a 206f 7065 6e20 6669 6c65 0a20  rce: open file. 
-00006980: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00006990: 2066 696c 655f 736f 7572 6365 3a20 6669   file_source: fi
-000069a0: 6c65 206f 7220 4269 6e61 7279 494f 0a20  le or BinaryIO. 
-000069b0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-000069c0: 6d20 7265 7472 793a 2069 6620 7365 7420  m retry: if set 
-000069d0: 746f 2046 616c 7365 2074 6865 7265 2077  to False there w
-000069e0: 696c 6c20 6f6e 6c79 2062 6520 6f6e 6520  ill only be one 
-000069f0: 7472 7920 6174 206f 6274 6169 6e69 6e67  try at obtaining
-00006a00: 2074 6865 2061 6e61 6c79 7369 7320 7265   the analysis re
-00006a10: 706f 7274 0a20 2020 2020 2020 2020 2020  port.           
-00006a20: 203a 7479 7065 2072 6574 7279 3a20 626f   :type retry: bo
-00006a30: 6f6c 0a20 2020 2020 2020 2020 2020 203a  ol.            :
-00006a40: 7061 7261 6d20 6669 656c 6473 3a20 6c69  param fields: li
-00006a50: 7374 206f 6620 4131 3030 3020 7265 706f  st of A1000 repo
-00006a60: 7274 2027 6669 656c 6473 2720 746f 2071  rt 'fields' to q
-00006a70: 7565 7279 0a20 2020 2020 2020 2020 2020  uery.           
-00006a80: 203a 7479 7065 2066 6965 6c64 733a 206c   :type fields: l
-00006a90: 6973 745b 7374 725d 0a20 2020 2020 2020  ist[str].       
-00006aa0: 2020 2020 203a 7061 7261 6d20 696e 636c       :param incl
-00006ab0: 7564 655f 6e65 7477 6f72 6b74 6872 6561  ude_networkthrea
-00006ac0: 7469 6e74 656c 6c69 6765 6e63 653a 2069  tintelligence: i
-00006ad0: 6e63 6c75 6465 206e 6574 776f 726b 2074  nclude network t
-00006ae0: 6872 6561 7420 696e 7465 6c6c 6967 656e  hreat intelligen
-00006af0: 6365 2069 6e20 7468 6520 7375 6d6d 6172  ce in the summar
-00006b00: 7920 7265 706f 7274 0a20 2020 2020 2020  y report.       
-00006b10: 2020 2020 203a 7479 7065 2069 6e63 6c75       :type inclu
-00006b20: 6465 5f6e 6574 776f 726b 7468 7265 6174  de_networkthreat
-00006b30: 696e 7465 6c6c 6967 656e 6365 3a20 626f  intelligence: bo
-00006b40: 6f6c 0a20 2020 2020 2020 2020 2020 203a  ol.            :
-00006b50: 7061 7261 6d20 736b 6970 5f72 6561 6e61  param skip_reana
-00006b60: 6c79 7369 733a 2073 6b69 7020 7361 6d70  lysis: skip samp
-00006b70: 6c65 2072 6561 6e61 6c79 7369 7320 7768  le reanalysis wh
-00006b80: 656e 2066 6574 6368 696e 6720 7468 6520  en fetching the 
-00006b90: 7375 6d6d 6172 7920 7265 706f 7274 0a20  summary report. 
-00006ba0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00006bb0: 2073 6b69 705f 7265 616e 616c 7973 6973   skip_reanalysis
-00006bc0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-00006bd0: 2020 203a 7061 7261 6d20 6375 7374 6f6d     :param custom
-00006be0: 5f66 696c 656e 616d 653a 2063 7573 746f  _filename: custo
-00006bf0: 6d20 6669 6c65 206e 616d 6520 666f 7220  m file name for 
-00006c00: 7570 6c6f 6164 0a20 2020 2020 2020 2020  upload.         
-00006c10: 2020 203a 7479 7065 2063 7573 746f 6d5f     :type custom_
-00006c20: 6669 6c65 6e61 6d65 3a20 7374 720a 2020  filename: str.  
-00006c30: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00006c40: 2074 6167 733a 2061 2073 7472 696e 6720   tags: a string 
-00006c50: 6f66 2063 6f6d 6d61 2073 6570 6172 6174  of comma separat
-00006c60: 6564 2074 6167 730a 2020 2020 2020 2020  ed tags.        
-00006c70: 2020 2020 3a74 7970 6520 7461 6773 3a20      :type tags: 
-00006c80: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-00006c90: 3a70 6172 616d 2063 6f6d 6d65 6e74 3a20  :param comment: 
-00006ca0: 636f 6d6d 656e 7420 7374 7269 6e67 0a20  comment string. 
-00006cb0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00006cc0: 2063 6f6d 6d65 6e74 3a20 7374 720a 2020   comment: str.  
-00006cd0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00006ce0: 2063 6c6f 7564 5f61 6e61 6c79 7369 733a   cloud_analysis:
-00006cf0: 2075 7365 2063 6c6f 7564 2061 6e61 6c79   use cloud analy
-00006d00: 7369 730a 2020 2020 2020 2020 2020 2020  sis.            
-00006d10: 3a74 7970 6520 636c 6f75 645f 616e 616c  :type cloud_anal
-00006d20: 7973 6973 3a20 626f 6f6c 0a20 2020 2020  ysis: bool.     
-00006d30: 2020 2020 2020 203a 7061 7261 6d20 6172         :param ar
-00006d40: 6368 6976 655f 7061 7373 776f 7264 3a20  chive_password: 
-00006d50: 7061 7373 776f 7264 2c20 6966 2066 696c  password, if fil
-00006d60: 6520 6973 2061 2070 6173 7377 6f72 642d  e is a password-
-00006d70: 7072 6f74 6563 7465 6420 6172 6368 6976  protected archiv
-00006d80: 650a 2020 2020 2020 2020 2020 2020 3a74  e.            :t
-00006d90: 7970 6520 6172 6368 6976 655f 7061 7373  ype archive_pass
-00006da0: 776f 7264 3a20 7374 720a 2020 2020 2020  word: str.      
-00006db0: 2020 2020 2020 3a70 6172 616d 2072 6c5f        :param rl_
-00006dc0: 636c 6f75 645f 7361 6e64 626f 785f 706c  cloud_sandbox_pl
-00006dd0: 6174 666f 726d 3a20 436c 6f75 6420 5361  atform: Cloud Sa
-00006de0: 6e64 626f 7820 706c 6174 666f 726d 2028  ndbox platform (
-00006df0: 7769 6e64 6f77 7337 2c20 7769 6e64 6f77  windows7, window
-00006e00: 7331 3020 6f72 206d 6163 6f73 5f31 3129  s10 or macos_11)
-00006e10: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00006e20: 7065 2072 6c5f 636c 6f75 645f 7361 6e64  pe rl_cloud_sand
-00006e30: 626f 785f 706c 6174 666f 726d 3a20 7374  box_platform: st
-00006e40: 720a 2020 2020 2020 2020 2020 2020 3a72  r.            :r
-00006e50: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
-00006e60: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
-00006e70: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
-00006e80: 706f 6e73 650a 2020 2020 2020 2020 2222  ponse.        ""
-00006e90: 220a 2020 2020 2020 2020 6966 2028 6669  ".        if (fi
-00006ea0: 6c65 5f70 6174 6820 616e 6420 6669 6c65  le_path and file
-00006eb0: 5f73 6f75 7263 6529 206f 7220 286e 6f74  _source) or (not
-00006ec0: 2066 696c 655f 7061 7468 2061 6e64 206e   file_path and n
-00006ed0: 6f74 2066 696c 655f 736f 7572 6365 293a  ot file_source):
-00006ee0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00006ef0: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-00006f00: 6f72 2822 4569 7468 6572 2066 696c 655f  or("Either file_
-00006f10: 7061 7468 206f 7220 6669 6c65 5f73 6f75  path or file_sou
-00006f20: 7263 6520 7061 7261 6d65 7465 7220 6d75  rce parameter mu
-00006f30: 7374 2062 6520 7072 6f76 6964 6564 2e20  st be provided. 
-00006f40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f60: 2020 2020 2255 7369 6e67 2062 6f74 6820      "Using both 
-00006f70: 6f72 206e 6f6e 6520 6f66 2074 6865 2070  or none of the p
-00006f80: 6172 616d 6574 6572 7320 696e 2073 6f74  arameters in sot
-00006f90: 2061 6c6c 6f77 6564 2e22 290a 0a20 2020   allowed.")..   
-00006fa0: 2020 2020 2069 6620 6669 6c65 5f70 6174       if file_pat
-00006fb0: 683a 0a20 2020 2020 2020 2020 2020 2075  h:.            u
-00006fc0: 706c 6f61 645f 7265 7370 6f6e 7365 203d  pload_response =
-00006fd0: 2073 656c 662e 7570 6c6f 6164 5f73 616d   self.upload_sam
-00006fe0: 706c 655f 6672 6f6d 5f70 6174 6828 6669  ple_from_path(fi
-00006ff0: 6c65 5f70 6174 682c 2063 7573 746f 6d5f  le_path, custom_
-00007000: 6669 6c65 6e61 6d65 2c20 6172 6368 6976  filename, archiv
-00007010: 655f 7061 7373 776f 7264 2c0a 2020 2020  e_password,.    
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007050: 2020 2020 2020 2072 6c5f 636c 6f75 645f         rl_cloud_
-00007060: 7361 6e64 626f 785f 706c 6174 666f 726d  sandbox_platform
-00007070: 2c20 7461 6773 2c20 636f 6d6d 656e 742c  , tags, comment,
-00007080: 2063 6c6f 7564 5f61 6e61 6c79 7369 7329   cloud_analysis)
-00007090: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000070a0: 2020 2020 2020 2020 2020 2075 706c 6f61             uploa
-000070b0: 645f 7265 7370 6f6e 7365 203d 2073 656c  d_response = sel
-000070c0: 662e 7570 6c6f 6164 5f73 616d 706c 655f  f.upload_sample_
-000070d0: 6672 6f6d 5f66 696c 6528 6669 6c65 5f73  from_file(file_s
-000070e0: 6f75 7263 652c 2063 7573 746f 6d5f 6669  ource, custom_fi
-000070f0: 6c65 6e61 6d65 2c20 7461 6773 2c20 6172  lename, tags, ar
-00007100: 6368 6976 655f 7061 7373 776f 7264 2c0a  chive_password,.
-00007110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007140: 2020 2020 2020 2020 2020 2072 6c5f 636c             rl_cl
-00007150: 6f75 645f 7361 6e64 626f 785f 706c 6174  oud_sandbox_plat
-00007160: 666f 726d 2c20 636f 6d6d 656e 742c 2063  form, comment, c
-00007170: 6c6f 7564 5f61 6e61 6c79 7369 7329 0a0a  loud_analysis)..
-00007180: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00007190: 5f64 6574 6169 6c20 3d20 7570 6c6f 6164  _detail = upload
-000071a0: 5f72 6573 706f 6e73 652e 6a73 6f6e 2829  _response.json()
-000071b0: 2e67 6574 2822 6465 7461 696c 2229 0a20  .get("detail"). 
-000071c0: 2020 2020 2020 2073 6861 3120 3d20 7265         sha1 = re
-000071d0: 7370 6f6e 7365 5f64 6574 6169 6c2e 6765  sponse_detail.ge
-000071e0: 7428 2273 6861 3122 290a 2020 2020 2020  t("sha1").      
-000071f0: 2020 7368 6131 203d 2073 7472 2873 6861    sha1 = str(sha
-00007200: 3129 0a0a 2020 2020 2020 2020 7265 7370  1)..        resp
-00007210: 6f6e 7365 203d 2073 656c 662e 6765 745f  onse = self.get_
-00007220: 7375 6d6d 6172 795f 7265 706f 7274 5f76  summary_report_v
-00007230: 3228 0a20 2020 2020 2020 2020 2020 2073  2(.            s
-00007240: 616d 706c 655f 6861 7368 6573 3d5b 7368  ample_hashes=[sh
-00007250: 6131 5d2c 0a20 2020 2020 2020 2020 2020  a1],.           
-00007260: 2072 6574 7279 3d72 6574 7279 2c0a 2020   retry=retry,.  
-00007270: 2020 2020 2020 2020 2020 6669 656c 6473            fields
-00007280: 3d66 6965 6c64 732c 0a20 2020 2020 2020  =fields,.       
-00007290: 2020 2020 2069 6e63 6c75 6465 5f6e 6574       include_net
-000072a0: 776f 726b 7468 7265 6174 696e 7465 6c6c  workthreatintell
-000072b0: 6967 656e 6365 3d69 6e63 6c75 6465 5f6e  igence=include_n
-000072c0: 6574 776f 726b 7468 7265 6174 696e 7465  etworkthreatinte
-000072d0: 6c6c 6967 656e 6365 2c0a 2020 2020 2020  lligence,.      
-000072e0: 2020 2020 2020 736b 6970 5f72 6561 6e61        skip_reana
-000072f0: 6c79 7369 733d 736b 6970 5f72 6561 6e61  lysis=skip_reana
-00007300: 6c79 7369 730a 2020 2020 2020 2020 290a  lysis.        ).
-00007310: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00007320: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
-00007330: 6620 6765 745f 6465 7461 696c 6564 5f72  f get_detailed_r
-00007340: 6570 6f72 745f 7632 2873 656c 662c 2073  eport_v2(self, s
-00007350: 616d 706c 655f 6861 7368 6573 2c20 7265  ample_hashes, re
-00007360: 7472 793d 4661 6c73 652c 2066 6965 6c64  try=False, field
-00007370: 733d 4e6f 6e65 2c20 736b 6970 5f72 6561  s=None, skip_rea
-00007380: 6e61 6c79 7369 733d 4661 6c73 6529 3a0a  nalysis=False):.
-00007390: 2020 2020 2020 2020 2222 2241 6363 6570          """Accep
-000073a0: 7473 2061 2073 696e 676c 6520 6861 7368  ts a single hash
-000073b0: 206f 7220 6120 6c69 7374 206f 6620 6861   or a list of ha
-000073c0: 7368 6573 2061 6e64 2072 6574 7572 6e73  shes and returns
-000073d0: 2061 2064 6574 6169 6c65 6420 616e 616c   a detailed anal
-000073e0: 7973 6973 2072 6570 6f72 7420 666f 7220  ysis report for 
-000073f0: 7468 6520 7365 6c65 6374 6564 2073 616d  the selected sam
-00007400: 706c 6573 2e0a 2020 2020 2020 2020 5468  ples..        Th
-00007410: 6973 206d 6574 686f 6420 7574 696c 697a  is method utiliz
-00007420: 6573 2074 6865 2073 6574 206e 756d 6265  es the set numbe
-00007430: 7220 6f66 2072 6574 7269 6573 2061 6e64  r of retries and
-00007440: 2077 6169 7420 7469 6d65 2069 6e20 7365   wait time in se
-00007450: 636f 6e64 7320 616e 6420 7469 6d65 7320  conds and times 
-00007460: 6f75 7420 6966 2074 6865 0a20 2020 2020  out if the.     
-00007470: 2020 2061 6e61 6c79 7369 7320 7265 7375     analysis resu
-00007480: 6c74 7320 6172 6520 6e6f 7420 7265 6164  lts are not read
-00007490: 792e 0a20 2020 2020 2020 2020 2020 203a  y..            :
-000074a0: 7061 7261 6d20 7361 6d70 6c65 5f68 6173  param sample_has
-000074b0: 6865 733a 2068 6173 6820 7374 7269 6e67  hes: hash string
-000074c0: 206f 7220 6c69 7374 206f 6620 6861 7368   or list of hash
-000074d0: 2073 7472 696e 6773 0a20 2020 2020 2020   strings.       
-000074e0: 2020 2020 203a 7479 7065 2073 616d 706c       :type sampl
-000074f0: 655f 6861 7368 6573 3a20 7374 7220 6f72  e_hashes: str or
-00007500: 206c 6973 745b 7374 725d 0a20 2020 2020   list[str].     
-00007510: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
-00007520: 7472 793a 2069 6620 7365 7420 746f 2046  try: if set to F
-00007530: 616c 7365 2074 6865 7265 2077 696c 6c20  alse there will 
-00007540: 6f6e 6c79 2062 6520 6f6e 6520 7472 7920  only be one try 
-00007550: 6174 206f 6274 6169 6e69 6e67 2074 6865  at obtaining the
-00007560: 2061 6e61 6c79 7369 7320 7265 706f 7274   analysis report
-00007570: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00007580: 7065 2072 6574 7279 3a20 626f 6f6c 0a20  pe retry: bool. 
-00007590: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-000075a0: 6d20 6669 656c 6473 3a20 6c69 7374 206f  m fields: list o
-000075b0: 6620 4131 3030 3020 7265 706f 7274 2027  f A1000 report '
-000075c0: 6669 656c 6473 2720 746f 2071 7565 7279  fields' to query
-000075d0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-000075e0: 7065 2066 6965 6c64 733a 206c 6973 745b  pe fields: list[
-000075f0: 7374 725d 0a20 2020 2020 2020 2020 2020  str].           
-00007600: 203a 7061 7261 6d20 736b 6970 5f72 6561   :param skip_rea
-00007610: 6e61 6c79 7369 733a 2073 6b69 7020 7361  nalysis: skip sa
-00007620: 6d70 6c65 2072 6561 6e61 6c79 7369 7320  mple reanalysis 
-00007630: 7768 656e 2066 6574 6368 696e 6720 7468  when fetching th
-00007640: 6520 7375 6d6d 6172 7920 7265 706f 7274  e summary report
-00007650: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00007660: 7065 2073 6b69 705f 7265 616e 616c 7973  pe skip_reanalys
-00007670: 6973 3a20 626f 6f6c 0a20 2020 2020 2020  is: bool.       
-00007680: 2020 2020 203a 7265 7475 726e 3a20 3a63       :return: :c
-00007690: 6c61 7373 3a60 5265 7370 6f6e 7365 203c  lass:`Response <
-000076a0: 5265 7370 6f6e 7365 3e60 206f 626a 6563  Response>` objec
-000076b0: 740a 2020 2020 2020 2020 2020 2020 3a72  t.            :r
-000076c0: 7479 7065 3a20 7265 7175 6573 7473 2e52  type: requests.R
-000076d0: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-000076e0: 2222 220a 2020 2020 2020 2020 6966 2066  """.        if f
-000076f0: 6965 6c64 7320 616e 6420 6e6f 7420 6973  ields and not is
-00007700: 696e 7374 616e 6365 2866 6965 6c64 732c  instance(fields,
-00007710: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
-00007720: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00007730: 6e70 7574 4572 726f 7228 2266 6965 6c64  nputError("field
-00007740: 7320 7061 7261 6d65 7465 7220 6d75 7374  s parameter must
-00007750: 2062 6520 6120 6c69 7374 206f 6620 7374   be a list of st
-00007760: 7269 6e67 732e 2229 0a0a 2020 2020 2020  rings.")..      
-00007770: 2020 6966 2072 6574 7279 206e 6f74 2069    if retry not i
-00007780: 6e20 2854 7275 652c 2046 616c 7365 293a  n (True, False):
-00007790: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000077a0: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-000077b0: 6f72 2822 7265 7472 7920 7061 7261 6d65  or("retry parame
-000077c0: 7465 7220 6d75 7374 2062 6520 626f 6f6c  ter must be bool
-000077d0: 6561 6e2e 2229 0a0a 2020 2020 2020 2020  ean.")..        
-000077e0: 6966 2073 6b69 705f 7265 616e 616c 7973  if skip_reanalys
-000077f0: 6973 206e 6f74 2069 6e20 2854 7275 652c  is not in (True,
-00007800: 2046 616c 7365 293a 0a20 2020 2020 2020   False):.       
-00007810: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
-00007820: 496e 7075 7445 7272 6f72 2822 736b 6970  InputError("skip
-00007830: 5f72 6561 6e61 6c79 7369 7320 7061 7261  _reanalysis para
-00007840: 6d65 7465 7220 6d75 7374 2062 6520 626f  meter must be bo
-00007850: 6f6c 6561 6e2e 2229 0a0a 2020 2020 2020  olean.")..      
-00007860: 2020 6966 206e 6f74 2066 6965 6c64 733a    if not fields:
-00007870: 0a20 2020 2020 2020 2020 2020 2066 6965  .            fie
-00007880: 6c64 7320 3d20 7365 6c66 2e5f 6669 656c  lds = self._fiel
-00007890: 6473 5f76 320a 0a20 2020 2020 2020 2069  ds_v2..        i
-000078a0: 6620 6973 696e 7374 616e 6365 2873 616d  f isinstance(sam
-000078b0: 706c 655f 6861 7368 6573 2c20 7374 7229  ple_hashes, str)
-000078c0: 3a0a 2020 2020 2020 2020 2020 2020 7361  :.            sa
-000078d0: 6d70 6c65 5f68 6173 6865 7320 3d20 5b73  mple_hashes = [s
-000078e0: 616d 706c 655f 6861 7368 6573 5d0a 0a20  ample_hashes].. 
-000078f0: 2020 2020 2020 2076 616c 6964 6174 655f         validate_
-00007900: 6861 7368 6573 280a 2020 2020 2020 2020  hashes(.        
-00007910: 2020 2020 6861 7368 5f69 6e70 7574 3d73      hash_input=s
-00007920: 616d 706c 655f 6861 7368 6573 2c0a 2020  ample_hashes,.  
-00007930: 2020 2020 2020 2020 2020 616c 6c6f 7765            allowe
-00007940: 645f 6861 7368 5f74 7970 6573 3d28 4d44  d_hash_types=(MD
-00007950: 352c 2053 4841 312c 2053 4841 3235 362c  5, SHA1, SHA256,
-00007960: 2053 4841 3531 3229 0a20 2020 2020 2020   SHA512).       
-00007970: 2029 0a0a 2020 2020 2020 2020 7265 7472   )..        retr
-00007980: 6965 7320 3d20 7365 6c66 2e5f 7265 7472  ies = self._retr
-00007990: 6965 7320 6966 2072 6574 7279 2065 6c73  ies if retry els
-000079a0: 6520 300a 0a20 2020 2020 2020 2061 6e61  e 0..        ana
-000079b0: 6c79 7369 735f 6973 5f66 696e 6973 6865  lysis_is_finishe
-000079c0: 6420 3d20 4661 6c73 650a 0a20 2020 2020  d = False..     
-000079d0: 2020 2066 6f72 2069 7465 7261 7469 6f6e     for iteration
-000079e0: 2069 6e20 7261 6e67 6528 7265 7472 6965   in range(retrie
-000079f0: 7320 2b20 3129 3a0a 2020 2020 2020 2020  s + 1):.        
-00007a00: 2020 2020 6966 2069 7465 7261 7469 6f6e      if iteration
-00007a10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007a20: 2020 7469 6d65 2e73 6c65 6570 2873 656c    time.sleep(sel
-00007a30: 662e 5f77 6169 745f 7469 6d65 5f73 6563  f._wait_time_sec
-00007a40: 6f6e 6473 290a 0a20 2020 2020 2020 2020  onds)..         
-00007a50: 2020 2061 6e61 6c79 7369 735f 6973 5f66     analysis_is_f
-00007a60: 696e 6973 6865 6420 3d20 7365 6c66 2e5f  inished = self._
-00007a70: 5f61 6e61 6c79 7369 735f 6973 5f66 696e  _analysis_is_fin
-00007a80: 6973 6865 6428 7361 6d70 6c65 5f68 6173  ished(sample_has
-00007a90: 6865 7329 0a20 2020 2020 2020 2020 2020  hes).           
-00007aa0: 2069 6620 616e 616c 7973 6973 5f69 735f   if analysis_is_
-00007ab0: 6669 6e69 7368 6564 3a0a 2020 2020 2020  finished:.      
-00007ac0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-00007ad0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00007ae0: 616e 616c 7973 6973 5f69 735f 6669 6e69  analysis_is_fini
-00007af0: 7368 6564 3a0a 2020 2020 2020 2020 2020  shed:.          
-00007b00: 2020 7261 6973 6520 5265 7175 6573 7454    raise RequestT
-00007b10: 696d 656f 7574 4572 726f 7228 2252 6570  imeoutError("Rep
-00007b20: 6f72 7420 6665 7463 6869 6e67 2061 7474  ort fetching att
-00007b30: 656d 7074 7320 6669 6e69 7368 6564 202d  empts finished -
-00007b40: 2054 6865 2061 6e61 6c79 7369 7320 7265   The analysis re
-00007b50: 706f 7274 2069 7320 7374 696c 6c20 6e6f  port is still no
-00007b60: 7420 7265 6164 7920 220a 2020 2020 2020  t ready ".      
-00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b90: 226f 7220 7468 6520 7361 6d70 6c65 2064  "or the sample d
-00007ba0: 6f65 7320 6e6f 7420 6578 6973 7420 6f6e  oes not exist on
-00007bb0: 2074 6865 2061 7070 6c69 616e 6365 2e22   the appliance."
-00007bc0: 290a 0a20 2020 2020 2020 2075 726c 203d  )..        url =
-00007bd0: 2073 656c 662e 5f75 726c 2e66 6f72 6d61   self._url.forma
-00007be0: 7428 656e 6470 6f69 6e74 3d73 656c 662e  t(endpoint=self.
-00007bf0: 5f5f 4445 5441 494c 4544 5f52 4550 4f52  __DETAILED_REPOR
-00007c00: 545f 454e 4450 4f49 4e54 5f56 3229 0a0a  T_ENDPOINT_V2)..
-00007c10: 2020 2020 2020 2020 6461 7461 203d 207b          data = {
-00007c20: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
-00007c30: 7368 5f76 616c 7565 7322 3a20 7361 6d70  sh_values": samp
-00007c40: 6c65 5f68 6173 6865 732c 0a20 2020 2020  le_hashes,.     
-00007c50: 2020 2020 2020 2022 6669 656c 6473 223a         "fields":
-00007c60: 2066 6965 6c64 732c 0a20 2020 2020 2020   fields,.       
-00007c70: 2020 2020 2022 736b 6970 5f72 6561 6e61       "skip_reana
-00007c80: 6c79 7369 7322 3a20 7374 7228 736b 6970  lysis": str(skip
-00007c90: 5f72 6561 6e61 6c79 7369 7329 2e6c 6f77  _reanalysis).low
-00007ca0: 6572 2829 0a20 2020 2020 2020 207d 0a0a  er().        }..
-00007cb0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00007cc0: 203d 2073 656c 662e 5f5f 706f 7374 5f72   = self.__post_r
-00007cd0: 6571 7565 7374 2875 726c 3d75 726c 2c20  equest(url=url, 
-00007ce0: 6461 7461 3d64 6174 6129 0a0a 2020 2020  data=data)..    
-00007cf0: 2020 2020 7365 6c66 2e5f 5f72 6169 7365      self.__raise
-00007d00: 5f6f 6e5f 6572 726f 7228 7265 7370 6f6e  _on_error(respon
-00007d10: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
-00007d20: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
-00007d30: 2020 6465 6620 6765 745f 636c 6173 7369    def get_classi
-00007d40: 6669 6361 7469 6f6e 2873 656c 662c 2073  fication(self, s
-00007d50: 616d 706c 655f 6861 7368 2c20 6c6f 6361  ample_hash, loca
-00007d60: 6c5f 6f6e 6c79 3d54 7275 6529 3a0a 2020  l_only=True):.  
-00007d70: 2020 2020 2020 2222 2254 4849 5320 4d45        """THIS ME
-00007d80: 5448 4f44 2049 5320 4445 5052 4543 4154  THOD IS DEPRECAT
-00007d90: 4544 2e0a 2020 2020 2020 2020 5573 6520  ED..        Use 
-00007da0: 6765 745f 636c 6173 7369 6669 6361 7469  get_classificati
-00007db0: 6f6e 5f76 3320 696e 7374 6561 642e 0a0a  on_v3 instead...
-00007dc0: 2020 2020 2020 2020 4765 7420 636c 6173          Get clas
-00007dd0: 7369 6669 6361 7469 6f6e 2066 6f72 206f  sification for o
-00007de0: 6e65 2073 616d 706c 6520 6861 7368 2e0a  ne sample hash..
-00007df0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00007e00: 616d 2073 616d 706c 655f 6861 7368 3a20  am sample_hash: 
-00007e10: 6861 7368 2073 7472 696e 670a 2020 2020  hash string.    
-00007e20: 2020 2020 2020 2020 3a74 7970 6520 7361          :type sa
-00007e30: 6d70 6c65 5f68 6173 683a 2073 7472 0a20  mple_hash: str. 
-00007e40: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00007e50: 6d20 6c6f 6361 6c5f 6f6e 6c79 3a20 7265  m local_only: re
-00007e60: 7475 726e 206f 6e6c 7920 6c6f 6361 6c20  turn only local 
-00007e70: 7361 6d70 6c65 730a 2020 2020 2020 2020  samples.        
-00007e80: 2020 2020 3a74 7970 6520 6c6f 6361 6c5f      :type local_
-00007e90: 6f6e 6c79 3a20 626f 6f6c 0a20 2020 2020  only: bool.     
-00007ea0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00007eb0: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
-00007ec0: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
-00007ed0: 7565 7374 732e 5265 7370 6f6e 7365 0a20  uests.Response. 
-00007ee0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007ef0: 2020 2077 6172 6e28 2254 6869 7320 6d65     warn("This me
-00007f00: 7468 6f64 2069 7320 6465 7072 6563 6174  thod is deprecat
-00007f10: 6564 2e20 5573 6520 6765 745f 636c 6173  ed. Use get_clas
-00007f20: 7369 6669 6361 7469 6f6e 5f76 3320 696e  sification_v3 in
-00007f30: 7374 6561 642e 222c 2044 6570 7265 6361  stead.", Depreca
-00007f40: 7469 6f6e 5761 726e 696e 6729 0a0a 2020  tionWarning)..  
-00007f50: 2020 2020 2020 7661 6c69 6461 7465 5f68        validate_h
-00007f60: 6173 6865 7328 0a20 2020 2020 2020 2020  ashes(.         
-00007f70: 2020 2068 6173 685f 696e 7075 743d 5b73     hash_input=[s
-00007f80: 616d 706c 655f 6861 7368 5d2c 0a20 2020  ample_hash],.   
-00007f90: 2020 2020 2020 2020 2061 6c6c 6f77 6564           allowed
-00007fa0: 5f68 6173 685f 7479 7065 733d 284d 4435  _hash_types=(MD5
-00007fb0: 2c20 5348 4131 2c20 5348 4132 3536 2c20  , SHA1, SHA256, 
-00007fc0: 5348 4135 3132 290a 2020 2020 2020 2020  SHA512).        
-00007fd0: 290a 0a20 2020 2020 2020 2069 6620 6c6f  )..        if lo
-00007fe0: 6361 6c5f 6f6e 6c79 206e 6f74 2069 6e20  cal_only not in 
-00007ff0: 2854 7275 652c 2046 616c 7365 293a 0a20  (True, False):. 
-00008000: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00008010: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
-00008020: 2822 6c6f 6361 6c5f 6f6e 6c79 2070 6172  ("local_only par
-00008030: 616d 6574 6572 206d 7573 7420 6265 2062  ameter must be b
-00008040: 6f6f 6c65 616e 2e22 290a 0a20 2020 2020  oolean.")..     
-00008050: 2020 2065 6e64 706f 696e 7420 3d20 7365     endpoint = se
-00008060: 6c66 2e5f 5f43 4c41 5353 4946 595f 454e  lf.__CLASSIFY_EN
-00008070: 4450 4f49 4e54 5f56 322e 666f 726d 6174  DPOINT_V2.format
-00008080: 280a 2020 2020 2020 2020 2020 2020 6861  (.            ha
-00008090: 7368 5f76 616c 7565 3d73 616d 706c 655f  sh_value=sample_
-000080a0: 6861 7368 2c0a 2020 2020 2020 2020 2020  hash,.          
-000080b0: 2020 6c6f 6361 6c6f 6e6c 793d 696e 7428    localonly=int(
-000080c0: 6c6f 6361 6c5f 6f6e 6c79 290a 2020 2020  local_only).    
-000080d0: 2020 2020 290a 0a20 2020 2020 2020 2075      )..        u
-000080e0: 726c 203d 2073 656c 662e 5f75 726c 2e66  rl = self._url.f
-000080f0: 6f72 6d61 7428 656e 6470 6f69 6e74 3d65  ormat(endpoint=e
-00008100: 6e64 706f 696e 7429 0a0a 2020 2020 2020  ndpoint)..      
-00008110: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00008120: 662e 5f5f 6765 745f 7265 7175 6573 7428  f.__get_request(
-00008130: 7572 6c3d 7572 6c29 0a0a 2020 2020 2020  url=url)..      
-00008140: 2020 7365 6c66 2e5f 5f72 6169 7365 5f6f    self.__raise_o
-00008150: 6e5f 6572 726f 7228 7265 7370 6f6e 7365  n_error(response
-00008160: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00008170: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
-00008180: 6465 6620 6765 745f 636c 6173 7369 6669  def get_classifi
-00008190: 6361 7469 6f6e 5f76 3328 7365 6c66 2c20  cation_v3(self, 
-000081a0: 7361 6d70 6c65 5f68 6173 682c 206c 6f63  sample_hash, loc
-000081b0: 616c 5f6f 6e6c 793d 4661 6c73 652c 2061  al_only=False, a
-000081c0: 765f 7363 616e 6e65 7273 3d46 616c 7365  v_scanners=False
-000081d0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-000081e0: 7420 636c 6173 7369 6669 6361 7469 6f6e  t classification
-000081f0: 2066 6f72 206f 6e65 2073 616d 706c 652e   for one sample.
-00008200: 0a20 2020 2020 2020 2054 6865 2064 6566  .        The def
-00008210: 6175 6c74 2076 616c 7565 206f 6620 6c6f  ault value of lo
-00008220: 6361 6c5f 6f6e 6c79 2069 7320 4661 6c73  cal_only is Fals
-00008230: 652c 2077 6869 6368 2c20 6966 206e 6f74  e, which, if not
-00008240: 2063 6861 6e67 6564 2c20 7769 6c6c 2073   changed, will s
-00008250: 656e 6420 6120 7265 7175 6573 7420 746f  end a request to
-00008260: 2054 6974 616e 6975 6d43 6c6f 7564 2074   TitaniumCloud t
-00008270: 6f0a 2020 2020 2020 2020 6765 7420 7468  o.        get th
-00008280: 6520 7361 6d70 6c65 2e20 5468 6520 6176  e sample. The av
-00008290: 5f73 6361 6e6e 6572 7320 7061 7261 6d65  _scanners parame
-000082a0: 7465 7220 6465 6369 6465 7320 6966 2074  ter decides if t
-000082b0: 6865 2041 5620 7363 616e 6e65 7220 7265  he AV scanner re
-000082c0: 7375 6c74 7320 7769 6c6c 2062 6520 696e  sults will be in
-000082d0: 636c 7564 6564 2069 6e20 7468 650a 2020  cluded in the.  
-000082e0: 2020 2020 2020 636c 6173 7369 6669 6361        classifica
-000082f0: 7469 6f6e 2072 6570 6f72 742e 0a20 2020  tion report..   
-00008300: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00008310: 7361 6d70 6c65 5f68 6173 683a 2068 6173  sample_hash: has
-00008320: 6820 7374 7269 6e67 0a20 2020 2020 2020  h string.       
-00008330: 2020 2020 203a 7479 7065 2073 616d 706c       :type sampl
-00008340: 655f 6861 7368 3a20 7374 720a 2020 2020  e_hash: str.    
-00008350: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
-00008360: 6f63 616c 5f6f 6e6c 793a 2072 6574 7572  ocal_only: retur
-00008370: 6e20 6f6e 6c79 206c 6f63 616c 2073 616d  n only local sam
-00008380: 706c 6573 2077 6974 686f 7574 2071 7565  ples without que
-00008390: 7279 696e 6720 5469 7461 6e69 756d 436c  rying TitaniumCl
-000083a0: 6f75 640a 2020 2020 2020 2020 2020 2020  oud.            
-000083b0: 3a74 7970 6520 6c6f 6361 6c5f 6f6e 6c79  :type local_only
-000083c0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-000083d0: 2020 203a 7061 7261 6d20 6176 5f73 6361     :param av_sca
-000083e0: 6e6e 6572 733a 2072 6574 7572 6e20 4156  nners: return AV
-000083f0: 2073 6361 6e6e 6572 2072 6573 756c 7473   scanner results
-00008400: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00008410: 7065 2061 765f 7363 616e 6e65 7273 3a20  pe av_scanners: 
-00008420: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
-00008430: 203a 7265 7475 726e 3a20 7265 7370 6f6e   :return: respon
-00008440: 7365 0a20 2020 2020 2020 2020 2020 203a  se.            :
-00008450: 7274 7970 653a 2072 6571 7565 7374 732e  rtype: requests.
-00008460: 5265 7370 6f6e 7365 0a20 2020 2020 2020  Response.       
-00008470: 2022 2222 0a20 2020 2020 2020 2076 616c   """.        val
-00008480: 6964 6174 655f 6861 7368 6573 280a 2020  idate_hashes(.  
-00008490: 2020 2020 2020 2020 2020 6861 7368 5f69            hash_i
-000084a0: 6e70 7574 3d5b 7361 6d70 6c65 5f68 6173  nput=[sample_has
-000084b0: 685d 2c0a 2020 2020 2020 2020 2020 2020  h],.            
-000084c0: 616c 6c6f 7765 645f 6861 7368 5f74 7970  allowed_hash_typ
-000084d0: 6573 3d28 4d44 352c 2053 4841 312c 2053  es=(MD5, SHA1, S
-000084e0: 4841 3235 362c 2053 4841 3531 3229 0a20  HA256, SHA512). 
-000084f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00008500: 2020 6966 206c 6f63 616c 5f6f 6e6c 7920    if local_only 
-00008510: 6e6f 7420 696e 2028 5472 7565 2c20 4661  not in (True, Fa
-00008520: 6c73 6529 3a0a 2020 2020 2020 2020 2020  lse):.          
-00008530: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
-00008540: 7574 4572 726f 7228 226c 6f63 616c 5f6f  utError("local_o
-00008550: 6e6c 7920 7061 7261 6d65 7465 7220 6d75  nly parameter mu
-00008560: 7374 2062 6520 626f 6f6c 6561 6e2e 2229  st be boolean.")
-00008570: 0a0a 2020 2020 2020 2020 6966 2061 765f  ..        if av_
-00008580: 7363 616e 6e65 7273 206e 6f74 2069 6e20  scanners not in 
-00008590: 2854 7275 652c 2046 616c 7365 293a 0a20  (True, False):. 
-000085a0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000085b0: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
-000085c0: 2822 6176 5f73 6361 6e6e 6572 7320 7061  ("av_scanners pa
-000085d0: 7261 6d65 7465 7220 6d75 7374 2062 6520  rameter must be 
-000085e0: 626f 6f6c 6561 6e2e 2229 0a0a 2020 2020  boolean.")..    
-000085f0: 2020 2020 6966 206c 6f63 616c 5f6f 6e6c      if local_onl
-00008600: 7920 616e 6420 6176 5f73 6361 6e6e 6572  y and av_scanner
-00008610: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-00008620: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
-00008630: 7272 6f72 2822 6c6f 6361 6c5f 6f6e 6c79  rror("local_only
-00008640: 206d 7573 7420 6265 2046 616c 7365 2069   must be False i
-00008650: 6620 6176 5f73 6361 6e6e 6572 7320 6172  f av_scanners ar
-00008660: 6520 7573 6564 2e22 290a 0a20 2020 2020  e used.")..     
-00008670: 2020 2070 6172 616d 7320 3d20 226c 6f63     params = "loc
-00008680: 616c 6f6e 6c79 3d7b 6c6f 6361 6c5f 6f6e  alonly={local_on
-00008690: 6c79 7d26 6176 5f73 6361 6e6e 6572 733d  ly}&av_scanners=
-000086a0: 7b61 765f 7363 616e 6e65 7273 7d22 2e66  {av_scanners}".f
-000086b0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-000086c0: 2020 206c 6f63 616c 5f6f 6e6c 793d 7374     local_only=st
-000086d0: 7228 696e 7428 6c6f 6361 6c5f 6f6e 6c79  r(int(local_only
-000086e0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-000086f0: 6176 5f73 6361 6e6e 6572 733d 7374 7228  av_scanners=str(
-00008700: 696e 7428 6176 5f73 6361 6e6e 6572 7329  int(av_scanners)
-00008710: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-00008720: 2020 2020 2065 6e64 706f 696e 7420 3d20       endpoint = 
-00008730: 227b 656e 6470 6f69 6e74 7d3f 7b70 6172  "{endpoint}?{par
-00008740: 616d 737d 222e 666f 726d 6174 280a 2020  ams}".format(.  
-00008750: 2020 2020 2020 2020 2020 656e 6470 6f69            endpoi
-00008760: 6e74 3d73 656c 662e 5f5f 434c 4153 5349  nt=self.__CLASSI
-00008770: 4659 5f45 4e44 504f 494e 545f 5633 2e66  FY_ENDPOINT_V3.f
-00008780: 6f72 6d61 7428 6861 7368 5f76 616c 7565  ormat(hash_value
-00008790: 3d73 616d 706c 655f 6861 7368 292c 0a20  =sample_hash),. 
-000087a0: 2020 2020 2020 2020 2020 2070 6172 616d             param
-000087b0: 733d 7061 7261 6d73 0a20 2020 2020 2020  s=params.       
-000087c0: 2029 0a0a 2020 2020 2020 2020 7572 6c20   )..        url 
-000087d0: 3d20 7365 6c66 2e5f 7572 6c2e 666f 726d  = self._url.form
-000087e0: 6174 2865 6e64 706f 696e 743d 656e 6470  at(endpoint=endp
-000087f0: 6f69 6e74 290a 0a20 2020 2020 2020 2072  oint)..        r
-00008800: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-00008810: 5f67 6574 5f72 6571 7565 7374 2875 726c  _get_request(url
-00008820: 3d75 726c 290a 0a20 2020 2020 2020 2073  =url)..        s
-00008830: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
-00008840: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
-00008850: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00008860: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
-00008870: 2072 6561 6e61 6c79 7a65 5f73 616d 706c   reanalyze_sampl
-00008880: 6573 2873 656c 662c 2068 6173 685f 696e  es(self, hash_in
-00008890: 7075 742c 2074 6974 616e 6975 6d5f 636c  put, titanium_cl
-000088a0: 6f75 643d 5472 7565 2c20 7469 7461 6e69  oud=True, titani
-000088b0: 756d 5f63 6f72 653d 5472 7565 293a 0a20  um_core=True):. 
-000088c0: 2020 2020 2020 2022 2222 5448 4953 204d         """THIS M
-000088d0: 4554 484f 4420 4953 2044 4550 5245 4341  ETHOD IS DEPRECA
-000088e0: 5445 442e 0a20 2020 2020 2020 2055 7365  TED..        Use
-000088f0: 2072 6561 6e61 6c79 7a65 5f73 616d 706c   reanalyze_sampl
-00008900: 6573 5f76 3220 696e 7374 6561 642e 0a0a  es_v2 instead...
-00008910: 2020 2020 2020 2020 4163 6365 7074 7320          Accepts 
-00008920: 6120 7369 6e67 6c65 2068 6173 6820 6f72  a single hash or
-00008930: 2061 206c 6973 7420 6f66 2068 6173 6865   a list of hashe
-00008940: 7320 6f66 2074 6865 2073 616d 6520 7479  s of the same ty
-00008950: 7065 2061 6e64 2072 6561 6e61 6c79 7a65  pe and reanalyze
-00008960: 7320 7468 650a 2020 2020 2020 2020 636f  s the.        co
-00008970: 7272 6573 706f 6e64 696e 6720 7361 6d70  rresponding samp
-00008980: 6c65 732e 0a20 2020 2020 2020 2020 2020  les..           
-00008990: 203a 7061 7261 6d20 6861 7368 5f69 6e70   :param hash_inp
-000089a0: 7574 3a20 7369 6e67 6c65 2068 6173 6820  ut: single hash 
-000089b0: 6f72 2061 206c 6973 7420 6f66 2068 6173  or a list of has
-000089c0: 6865 730a 2020 2020 2020 2020 2020 2020  hes.            
-000089d0: 3a74 7970 6520 6861 7368 5f69 6e70 7574  :type hash_input
-000089e0: 3a20 7374 7220 6f72 206c 6973 745b 7374  : str or list[st
-000089f0: 725d 0a20 2020 2020 2020 2020 2020 203a  r].            :
-00008a00: 7061 7261 6d20 7469 7461 6e69 756d 5f63  param titanium_c
-00008a10: 6c6f 7564 3a20 7573 6520 5469 7461 6e69  loud: use Titani
-00008a20: 756d 436c 6f75 640a 2020 2020 2020 2020  umCloud.        
-00008a30: 2020 2020 3a74 7970 6520 7469 7461 6e69      :type titani
-00008a40: 756d 5f63 6c6f 7564 3a20 626f 6f6c 0a20  um_cloud: bool. 
-00008a50: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00008a60: 6d20 7469 7461 6e69 756d 5f63 6f72 653a  m titanium_core:
-00008a70: 2075 7365 2054 6974 616e 6975 6d43 6f72   use TitaniumCor
-00008a80: 650a 2020 2020 2020 2020 2020 2020 3a74  e.            :t
-00008a90: 7970 6520 7469 7461 6e69 756d 5f63 6f72  ype titanium_cor
-00008aa0: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-00008ab0: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
-00008ac0: 706f 6e73 650a 2020 2020 2020 2020 2020  ponse.          
-00008ad0: 2020 3a72 7479 7065 3a20 7265 7175 6573    :rtype: reques
-00008ae0: 7473 2e52 6573 706f 6e73 650a 2020 2020  ts.Response.    
-00008af0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008b00: 7761 726e 2822 5468 6973 206d 6574 686f  warn("This metho
-00008b10: 6420 6973 2064 6570 7265 6361 7465 642e  d is deprecated.
-00008b20: 2055 7365 2072 6561 6e61 6c79 7a65 5f73   Use reanalyze_s
-00008b30: 616d 706c 6573 5f76 3220 696e 7374 6561  amples_v2 instea
-00008b40: 642e 222c 2044 6570 7265 6361 7469 6f6e  d.", Deprecation
-00008b50: 5761 726e 696e 6729 0a0a 2020 2020 2020  Warning)..      
-00008b60: 2020 6966 2074 6974 616e 6975 6d5f 636c    if titanium_cl
-00008b70: 6f75 6420 6e6f 7420 696e 2028 5472 7565  oud not in (True
-00008b80: 2c20 4661 6c73 6529 3a0a 2020 2020 2020  , False):.      
-00008b90: 2020 2020 2020 7261 6973 6520 5772 6f6e        raise Wron
-00008ba0: 6749 6e70 7574 4572 726f 7228 2274 6974  gInputError("tit
-00008bb0: 616e 6975 6d5f 636c 6f75 6420 7061 7261  anium_cloud para
-00008bc0: 6d65 7465 7220 6d75 7374 2062 6520 626f  meter must be bo
-00008bd0: 6f6c 6561 6e2e 2229 0a0a 2020 2020 2020  olean.")..      
-00008be0: 2020 6966 2074 6974 616e 6975 6d5f 636f    if titanium_co
-00008bf0: 7265 206e 6f74 2069 6e20 2854 7275 652c  re not in (True,
-00008c00: 2046 616c 7365 293a 0a20 2020 2020 2020   False):.       
-00008c10: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
-00008c20: 496e 7075 7445 7272 6f72 2822 7469 7461  InputError("tita
-00008c30: 6e69 756d 5f63 6f72 6520 7061 7261 6d65  nium_core parame
-00008c40: 7465 7220 6d75 7374 2062 6520 626f 6f6c  ter must be bool
-00008c50: 6561 6e2e 2229 0a0a 2020 2020 2020 2020  ean.")..        
-00008c60: 7061 7261 6d65 7465 725f 6469 6374 203d  parameter_dict =
-00008c70: 207b 2763 6f72 6527 3a20 7469 7461 6e69   {'core': titani
-00008c80: 756d 5f63 6f72 652c 2027 636c 6f75 6427  um_core, 'cloud'
-00008c90: 3a20 7469 7461 6e69 756d 5f63 6c6f 7564  : titanium_cloud
-00008ca0: 7d0a 0a20 2020 2020 2020 2061 6e61 6c79  }..        analy
-00008cb0: 7369 735f 6c69 7374 203d 205b 6b65 7920  sis_list = [key 
-00008cc0: 666f 7220 6b65 792c 2076 616c 7565 2069  for key, value i
-00008cd0: 6e20 7061 7261 6d65 7465 725f 6469 6374  n parameter_dict
-00008ce0: 2e69 7465 6d73 2829 2069 6620 7661 6c75  .items() if valu
-00008cf0: 655d 0a0a 2020 2020 2020 2020 6966 206c  e]..        if l
-00008d00: 656e 2861 6e61 6c79 7369 735f 6c69 7374  en(analysis_list
-00008d10: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-00008d20: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00008d30: 6e70 7574 4572 726f 7228 2241 7420 6c65  nputError("At le
-00008d40: 6173 7420 6f6e 6520 6f66 2074 6865 2066  ast one of the f
-00008d50: 6f6c 6c6f 7769 6e67 2070 6172 616d 6574  ollowing paramet
-00008d60: 6572 7320 6e65 6564 7320 746f 2062 6520  ers needs to be 
-00008d70: 656e 6162 6c65 643a 2022 0a20 2020 2020  enabled: ".     
-00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d90: 2020 2020 2020 2020 2020 2020 2022 7469               "ti
-00008da0: 7461 6e69 756d 5f63 6c6f 7564 2c20 7469  tanium_cloud, ti
-00008db0: 7461 6e69 756d 5f63 6f72 652e 2229 0a0a  tanium_core.")..
-00008dc0: 2020 2020 2020 2020 616e 616c 7973 6973          analysis
-00008dd0: 5f74 7970 6520 3d20 222c 222e 6a6f 696e  _type = ",".join
-00008de0: 2861 6e61 6c79 7369 735f 6c69 7374 290a  (analysis_list).
-00008df0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00008e00: 7374 616e 6365 2868 6173 685f 696e 7075  stance(hash_inpu
-00008e10: 742c 2073 7472 293a 0a20 2020 2020 2020  t, str):.       
-00008e20: 2020 2020 2076 616c 6964 6174 655f 6861       validate_ha
-00008e30: 7368 6573 280a 2020 2020 2020 2020 2020  shes(.          
-00008e40: 2020 2020 2020 6861 7368 5f69 6e70 7574        hash_input
-00008e50: 3d5b 6861 7368 5f69 6e70 7574 5d2c 0a20  =[hash_input],. 
-00008e60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00008e70: 6c6c 6f77 6564 5f68 6173 685f 7479 7065  llowed_hash_type
-00008e80: 733d 284d 4435 2c20 5348 4131 2c20 5348  s=(MD5, SHA1, SH
-00008e90: 4132 3536 2c20 5348 4135 3132 290a 2020  A256, SHA512).  
-00008ea0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00008eb0: 2020 2020 2020 2020 2065 6e64 706f 696e           endpoin
-00008ec0: 7420 3d20 7365 6c66 2e5f 5f52 4541 4e41  t = self.__REANA
-00008ed0: 4c59 5a45 5f45 4e44 504f 494e 542e 666f  LYZE_ENDPOINT.fo
-00008ee0: 726d 6174 2868 6173 685f 7661 6c75 653d  rmat(hash_value=
-00008ef0: 6861 7368 5f69 6e70 7574 290a 0a20 2020  hash_input)..   
-00008f00: 2020 2020 2020 2020 2075 726c 203d 2073           url = s
-00008f10: 656c 662e 5f75 726c 2e66 6f72 6d61 7428  elf._url.format(
-00008f20: 656e 6470 6f69 6e74 3d65 6e64 706f 696e  endpoint=endpoin
-00008f30: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
-00008f40: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-00008f50: 5f5f 706f 7374 5f72 6571 7565 7374 2875  __post_request(u
-00008f60: 726c 3d75 726c 2c20 6461 7461 3d7b 2261  rl=url, data={"a
-00008f70: 6e61 6c79 7369 7322 3a20 616e 616c 7973  nalysis": analys
-00008f80: 6973 5f74 7970 657d 290a 0a20 2020 2020  is_type})..     
-00008f90: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00008fa0: 6365 2868 6173 685f 696e 7075 742c 206c  ce(hash_input, l
-00008fb0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
-00008fc0: 2020 7661 6c69 6461 7465 5f68 6173 6865    validate_hashe
-00008fd0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00008fe0: 2020 2068 6173 685f 696e 7075 743d 6861     hash_input=ha
-00008ff0: 7368 5f69 6e70 7574 2c0a 2020 2020 2020  sh_input,.      
-00009000: 2020 2020 2020 2020 2020 616c 6c6f 7765            allowe
-00009010: 645f 6861 7368 5f74 7970 6573 3d28 4d44  d_hash_types=(MD
-00009020: 352c 2053 4841 312c 2053 4841 3235 362c  5, SHA1, SHA256,
-00009030: 2053 4841 3531 3229 0a20 2020 2020 2020   SHA512).       
-00009040: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00009050: 2020 2020 7572 6c20 3d20 7365 6c66 2e5f      url = self._
-00009060: 7572 6c2e 666f 726d 6174 2865 6e64 706f  url.format(endpo
-00009070: 696e 743d 7365 6c66 2e5f 5f52 4541 4e41  int=self.__REANA
-00009080: 4c59 5a45 5f42 554c 4b5f 454e 4450 4f49  LYZE_BULK_ENDPOI
-00009090: 4e54 290a 0a20 2020 2020 2020 2020 2020  NT)..           
-000090a0: 2064 6174 6120 3d20 7b22 6861 7368 5f76   data = {"hash_v
-000090b0: 616c 7565 223a 2068 6173 685f 696e 7075  alue": hash_inpu
-000090c0: 742c 2022 616e 616c 7973 6973 223a 2061  t, "analysis": a
-000090d0: 6e61 6c79 7369 735f 7479 7065 7d0a 0a20  nalysis_type}.. 
-000090e0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-000090f0: 6e73 6520 3d20 7365 6c66 2e5f 5f70 6f73  nse = self.__pos
-00009100: 745f 7265 7175 6573 7428 7572 6c3d 7572  t_request(url=ur
-00009110: 6c2c 2064 6174 613d 6461 7461 290a 0a20  l, data=data).. 
-00009120: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00009130: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
-00009140: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
-00009150: 6861 7368 5f69 6e70 7574 2070 6172 616d  hash_input param
-00009160: 6574 6572 2063 616e 206f 6e6c 7920 6265  eter can only be
-00009170: 2061 2073 696e 676c 6520 6861 7368 2073   a single hash s
-00009180: 7472 696e 6720 6f72 2022 0a20 2020 2020  tring or ".     
-00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091a0: 2020 2020 2020 2020 2020 2020 2022 6120               "a 
-000091b0: 6c69 7374 206f 6620 6861 7368 2073 7472  list of hash str
-000091c0: 696e 6773 206f 6620 7468 6520 7361 6d65  ings of the same
-000091d0: 2074 7970 652e 2229 0a0a 2020 2020 2020   type.")..      
-000091e0: 2020 7365 6c66 2e5f 5f72 6169 7365 5f6f    self.__raise_o
-000091f0: 6e5f 6572 726f 7228 7265 7370 6f6e 7365  n_error(response
-00009200: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00009210: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
-00009220: 6465 6620 7265 616e 616c 797a 655f 7361  def reanalyze_sa
-00009230: 6d70 6c65 735f 7632 2873 656c 662c 2068  mples_v2(self, h
-00009240: 6173 685f 696e 7075 742c 2074 6974 616e  ash_input, titan
-00009250: 6975 6d5f 636c 6f75 643d 4661 6c73 652c  ium_cloud=False,
-00009260: 2074 6974 616e 6975 6d5f 636f 7265 3d46   titanium_core=F
-00009270: 616c 7365 2c20 726c 5f63 6c6f 7564 5f73  alse, rl_cloud_s
-00009280: 616e 6462 6f78 3d46 616c 7365 2c0a 2020  andbox=False,.  
-00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092a0: 2020 2020 2020 2020 2020 2063 7563 6b6f             cucko
-000092b0: 6f5f 7361 6e64 626f 783d 4661 6c73 652c  o_sandbox=False,
-000092c0: 2066 6972 6565 7965 3d46 616c 7365 2c20   fireeye=False, 
-000092d0: 6a6f 655f 7361 6e64 626f 783d 4661 6c73  joe_sandbox=Fals
-000092e0: 652c 2063 6170 653d 4661 6c73 652c 0a20  e, cape=False,. 
-000092f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009300: 2020 2020 2020 2020 2020 2020 726c 5f63              rl_c
-00009310: 6c6f 7564 5f73 616e 6462 6f78 5f70 6c61  loud_sandbox_pla
-00009320: 7466 6f72 6d3d 4e6f 6e65 293a 0a20 2020  tform=None):.   
-00009330: 2020 2020 2022 2222 4163 6365 7074 7320       """Accepts 
-00009340: 6120 7369 6e67 6c65 2068 6173 6820 6f72  a single hash or
-00009350: 2061 206c 6973 7420 6f66 2068 6173 6865   a list of hashe
-00009360: 7320 6f66 2076 6172 696f 7573 2074 7970  s of various typ
-00009370: 6573 2061 6e64 2072 6561 6e61 6c79 7a65  es and reanalyze
-00009380: 7320 7468 6520 636f 7272 6573 706f 6e64  s the correspond
-00009390: 696e 6720 7361 6d70 6c65 2873 292e 0a20  ing sample(s).. 
-000093a0: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
-000093b0: 6f64 2063 616e 2062 6520 7573 6564 2066  od can be used f
-000093c0: 6f72 2072 6561 6e61 6c79 7a69 6e67 2061  or reanalyzing a
-000093d0: 2073 696e 676c 6520 7361 6d70 6c65 206f   single sample o
-000093e0: 7220 6120 6261 7463 6820 6f66 2073 616d  r a batch of sam
-000093f0: 706c 6573 2c20 6465 7065 6e64 696e 6720  ples, depending 
-00009400: 6f6e 2074 6865 2064 6174 6120 7479 7065  on the data type
-00009410: 0a20 2020 2020 2020 2070 6173 7365 642e  .        passed.
-00009420: 0a20 2020 2020 2020 2041 5420 6c65 6173  .        AT leas
-00009430: 7420 6f6e 6520 616e 616c 7973 6973 2074  t one analysis t
-00009440: 7970 6520 6d75 7374 2062 6520 7573 6564  ype must be used
-00009450: 2028 7365 7420 746f 2054 7275 6529 2e0a   (set to True)..
-00009460: 2020 2020 2020 2020 4966 2072 6c5f 636c          If rl_cl
-00009470: 6f75 645f 7361 6e64 626f 7820 6973 2075  oud_sandbox is u
-00009480: 7365 6420 6173 2061 6e20 616e 616c 7973  sed as an analys
-00009490: 6973 2074 7970 652c 2072 6c5f 636c 6f75  is type, rl_clou
-000094a0: 645f 7361 6e64 626f 785f 706c 6174 666f  d_sandbox_platfo
-000094b0: 726d 206d 7573 7420 6265 2064 6566 696e  rm must be defin
-000094c0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-000094d0: 3a70 6172 616d 2068 6173 685f 696e 7075  :param hash_inpu
-000094e0: 743a 2073 696e 676c 6520 6861 7368 206f  t: single hash o
-000094f0: 7220 6120 6c69 7374 206f 6620 6861 7368  r a list of hash
-00009500: 6573 0a20 2020 2020 2020 2020 2020 203a  es.            :
-00009510: 7479 7065 2068 6173 685f 696e 7075 743a  type hash_input:
-00009520: 2073 7472 206f 7220 6c69 7374 5b73 7472   str or list[str
-00009530: 5d0a 2020 2020 2020 2020 2020 2020 3a70  ].            :p
-00009540: 6172 616d 2074 6974 616e 6975 6d5f 636c  aram titanium_cl
-00009550: 6f75 643a 2075 7365 2054 6974 616e 6975  oud: use Titaniu
-00009560: 6d43 6c6f 7564 0a20 2020 2020 2020 2020  mCloud.         
-00009570: 2020 203a 7479 7065 2074 6974 616e 6975     :type titaniu
-00009580: 6d5f 636c 6f75 643a 2062 6f6f 6c0a 2020  m_cloud: bool.  
-00009590: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-000095a0: 2074 6974 616e 6975 6d5f 636f 7265 3a20   titanium_core: 
-000095b0: 7573 6520 5469 7461 6e69 756d 436f 7265  use TitaniumCore
-000095c0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-000095d0: 7065 2074 6974 616e 6975 6d5f 636f 7265  pe titanium_core
-000095e0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-000095f0: 2020 203a 7061 7261 6d20 726c 5f63 6c6f     :param rl_clo
-00009600: 7564 5f73 616e 6462 6f78 3a20 7573 6520  ud_sandbox: use 
-00009610: 524c 2063 6c6f 7564 2073 616e 6462 6f78  RL cloud sandbox
-00009620: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00009630: 7065 2072 6c5f 636c 6f75 645f 7361 6e64  pe rl_cloud_sand
-00009640: 626f 783a 2062 6f6f 6c0a 2020 2020 2020  box: bool.      
-00009650: 2020 2020 2020 3a70 6172 616d 2063 7563        :param cuc
-00009660: 6b6f 6f5f 7361 6e64 626f 783a 2075 7365  koo_sandbox: use
-00009670: 2043 7563 6b6f 6f20 7361 6e64 626f 780a   Cuckoo sandbox.
-00009680: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
-00009690: 6520 6375 636b 6f6f 5f73 616e 6462 6f78  e cuckoo_sandbox
-000096a0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-000096b0: 2020 203a 7061 7261 6d20 6669 7265 6579     :param fireey
-000096c0: 653a 2075 7365 2046 6972 6545 7965 0a20  e: use FireEye. 
-000096d0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-000096e0: 2066 6972 6565 7965 3a20 626f 6f6c 0a20   fireeye: bool. 
-000096f0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00009700: 6d20 6a6f 655f 7361 6e64 626f 783a 2075  m joe_sandbox: u
-00009710: 7365 204a 6f65 2073 616e 6462 6f78 0a20  se Joe sandbox. 
-00009720: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00009730: 206a 6f65 5f73 616e 6462 6f78 3a20 626f   joe_sandbox: bo
-00009740: 6f6c 0a20 2020 2020 2020 2020 2020 203a  ol.            :
-00009750: 7061 7261 6d20 6361 7065 3a20 7573 6520  param cape: use 
-00009760: 4361 7065 0a20 2020 2020 2020 2020 2020  Cape.           
-00009770: 203a 7479 7065 2063 6170 653a 2062 6f6f   :type cape: boo
-00009780: 6c0a 2020 2020 2020 2020 2020 2020 3a70  l.            :p
-00009790: 6172 616d 2072 6c5f 636c 6f75 645f 7361  aram rl_cloud_sa
-000097a0: 6e64 626f 785f 706c 6174 666f 726d 3a20  ndbox_platform: 
-000097b0: 6465 7369 7265 6420 706c 6174 666f 726d  desired platform
-000097c0: 206f 6e20 7768 6963 6820 7468 6520 7361   on which the sa
-000097d0: 6d70 6c65 2077 696c 6c20 6265 2064 6574  mple will be det
-000097e0: 6f6e 6174 6564 3b0a 2020 2020 2020 2020  onated;.        
-000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009810: 2020 2020 7365 6520 5265 7665 7273 696e      see Reversin
-00009820: 674c 6162 732e 5344 4b2e 6865 6c70 6572  gLabs.SDK.helper
-00009830: 2e41 5641 494c 4142 4c45 2050 4c41 5446  .AVAILABLE PLATF
-00009840: 4f52 4d53 2066 6f72 206f 7074 696f 6e73  ORMS for options
-00009850: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00009860: 7065 2072 6c5f 636c 6f75 645f 7361 6e64  pe rl_cloud_sand
-00009870: 626f 785f 706c 6174 666f 726d 3a20 7374  box_platform: st
-00009880: 720a 2020 2020 2020 2020 2020 2020 3a72  r.            :r
-00009890: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
-000098a0: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
-000098b0: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
-000098c0: 706f 6e73 650a 2020 2020 2020 2020 2222  ponse.        ""
-000098d0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-000098e0: 2069 7369 6e73 7461 6e63 6528 6861 7368   isinstance(hash
-000098f0: 5f69 6e70 7574 2c20 6c69 7374 293a 0a20  _input, list):. 
-00009900: 2020 2020 2020 2020 2020 2068 6173 685f             hash_
-00009910: 696e 7075 7420 3d20 5b68 6173 685f 696e  input = [hash_in
-00009920: 7075 745d 0a0a 2020 2020 2020 2020 7661  put]..        va
-00009930: 6c69 6461 7465 5f68 6173 6865 7328 0a20  lidate_hashes(. 
-00009940: 2020 2020 2020 2020 2020 2068 6173 685f             hash_
-00009950: 696e 7075 743d 6861 7368 5f69 6e70 7574  input=hash_input
-00009960: 2c0a 2020 2020 2020 2020 2020 2020 616c  ,.            al
-00009970: 6c6f 7765 645f 6861 7368 5f74 7970 6573  lowed_hash_types
-00009980: 3d28 4d44 352c 2053 4841 312c 2053 4841  =(MD5, SHA1, SHA
-00009990: 3235 362c 2053 4841 3531 3229 0a20 2020  256, SHA512).   
-000099a0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-000099b0: 616e 616c 7973 6973 5f74 7970 655f 6469  analysis_type_di
-000099c0: 6374 203d 207b 2263 6c6f 7564 223a 2074  ct = {"cloud": t
-000099d0: 6974 616e 6975 6d5f 636c 6f75 642c 2022  itanium_cloud, "
-000099e0: 636f 7265 223a 2074 6974 616e 6975 6d5f  core": titanium_
-000099f0: 636f 7265 2c20 2272 6c5f 636c 6f75 645f  core, "rl_cloud_
-00009a00: 7361 6e64 626f 7822 3a20 726c 5f63 6c6f  sandbox": rl_clo
-00009a10: 7564 5f73 616e 6462 6f78 2c0a 2020 2020  ud_sandbox,.    
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a30: 2020 2020 2020 2020 2020 2263 7563 6b6f            "cucko
-00009a40: 6f22 3a20 6375 636b 6f6f 5f73 616e 6462  o": cuckoo_sandb
-00009a50: 6f78 2c20 2266 6972 6565 7965 223a 2066  ox, "fireeye": f
-00009a60: 6972 6565 7965 2c20 226a 6f65 223a 206a  ireeye, "joe": j
-00009a70: 6f65 5f73 616e 6462 6f78 2c20 2263 6170  oe_sandbox, "cap
-00009a80: 6522 3a20 6361 7065 7d0a 0a20 2020 2020  e": cape}..     
-00009a90: 2020 2069 6620 6e6f 7420 616c 6c28 6973     if not all(is
-00009aa0: 696e 7374 616e 6365 2861 6e61 6c79 7369  instance(analysi
-00009ab0: 735f 7479 7065 2c20 626f 6f6c 2920 666f  s_type, bool) fo
-00009ac0: 7220 616e 616c 7973 6973 5f74 7970 6520  r analysis_type 
-00009ad0: 696e 2061 6e61 6c79 7369 735f 7479 7065  in analysis_type
-00009ae0: 5f64 6963 742e 7661 6c75 6573 2829 293a  _dict.values()):
-00009af0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00009b00: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-00009b10: 6f72 2822 416c 6c20 616e 616c 7973 6973  or("All analysis
-00009b20: 2074 7970 6520 7061 7261 6d65 7465 7273   type parameters
-00009b30: 206d 7573 7420 6265 2062 6f6f 6c65 616e   must be boolean
-00009b40: 2e22 290a 0a20 2020 2020 2020 2069 6620  .")..        if 
-00009b50: 726c 5f63 6c6f 7564 5f73 616e 6462 6f78  rl_cloud_sandbox
-00009b60: 2061 6e64 2072 6c5f 636c 6f75 645f 7361   and rl_cloud_sa
-00009b70: 6e64 626f 785f 706c 6174 666f 726d 206e  ndbox_platform n
-00009b80: 6f74 2069 6e20 4156 4149 4c41 424c 455f  ot in AVAILABLE_
-00009b90: 504c 4154 464f 524d 533a 0a20 2020 2020  PLATFORMS:.     
-00009ba0: 2020 2020 2020 2072 6169 7365 2057 726f         raise Wro
-00009bb0: 6e67 496e 7075 7445 7272 6f72 2822 6966  ngInputError("if
-00009bc0: 2072 6c5f 636c 6f75 645f 7361 6e64 626f   rl_cloud_sandbo
-00009bd0: 7820 6973 2075 7365 642c 2072 6c5f 636c  x is used, rl_cl
-00009be0: 6f75 645f 7361 6e64 626f 785f 706c 6174  oud_sandbox_plat
-00009bf0: 666f 726d 2070 6172 616d 6574 6572 206d  form parameter m
-00009c00: 7573 7420 6265 206f 6e65 2022 0a20 2020  ust be one ".   
-00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00009c30: 6f66 2074 6865 2066 6f6c 6c6f 7769 6e67  of the following
-00009c40: 2076 616c 7565 733a 207b 706c 6174 666f   values: {platfo
-00009c50: 726d 737d 222e 666f 726d 6174 2870 6c61  rms}".format(pla
-00009c60: 7466 6f72 6d73 3d41 5641 494c 4142 4c45  tforms=AVAILABLE
-00009c70: 5f50 4c41 5446 4f52 4d53 2929 0a0a 2020  _PLATFORMS))..  
-00009c80: 2020 2020 2020 616e 616c 7973 6973 5f6c        analysis_l
-00009c90: 6973 7420 3d20 5b6b 6579 2066 6f72 206b  ist = [key for k
-00009ca0: 6579 2c20 7661 6c75 6520 696e 2061 6e61  ey, value in ana
-00009cb0: 6c79 7369 735f 7479 7065 5f64 6963 742e  lysis_type_dict.
-00009cc0: 6974 656d 7328 2920 6966 2076 616c 7565  items() if value
-00009cd0: 5d0a 0a20 2020 2020 2020 2069 6620 6e6f  ]..        if no
-00009ce0: 7420 616e 616c 7973 6973 5f6c 6973 743a  t analysis_list:
-00009cf0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00009d00: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-00009d10: 6f72 2822 4174 206c 6561 7374 206f 6e65  or("At least one
-00009d20: 2061 6e61 6c79 7369 7320 7479 7065 2070   analysis type p
-00009d30: 6172 616d 6574 6572 206e 6565 6473 2074  arameter needs t
-00009d40: 6f20 6265 2064 6566 696e 6564 2e22 290a  o be defined.").
-00009d50: 0a20 2020 2020 2020 2061 6e61 6c79 7369  .        analysi
-00009d60: 735f 7479 7065 7320 3d20 222c 222e 6a6f  s_types = ",".jo
-00009d70: 696e 2861 6e61 6c79 7369 735f 6c69 7374  in(analysis_list
-00009d80: 290a 0a20 2020 2020 2020 2075 726c 203d  )..        url =
-00009d90: 2073 656c 662e 5f75 726c 2e66 6f72 6d61   self._url.forma
-00009da0: 7428 656e 6470 6f69 6e74 3d73 656c 662e  t(endpoint=self.
-00009db0: 5f5f 5245 414e 414c 595a 455f 4255 4c4b  __REANALYZE_BULK
-00009dc0: 5f45 4e44 504f 494e 545f 5632 290a 0a20  _ENDPOINT_V2).. 
-00009dd0: 2020 2020 2020 2064 6174 6120 3d20 7b0a         data = {.
-00009de0: 2020 2020 2020 2020 2020 2020 2268 6173              "has
-00009df0: 685f 7661 6c75 6522 3a20 6861 7368 5f69  h_value": hash_i
-00009e00: 6e70 7574 2c0a 2020 2020 2020 2020 2020  nput,.          
-00009e10: 2020 2261 6e61 6c79 7369 7322 3a20 616e    "analysis": an
-00009e20: 616c 7973 6973 5f74 7970 6573 2c0a 2020  alysis_types,.  
-00009e30: 2020 2020 2020 2020 2020 2272 6c5f 636c            "rl_cl
-00009e40: 6f75 645f 7361 6e64 626f 785f 706c 6174  oud_sandbox_plat
-00009e50: 666f 726d 223a 2072 6c5f 636c 6f75 645f  form": rl_cloud_
-00009e60: 7361 6e64 626f 785f 706c 6174 666f 726d  sandbox_platform
-00009e70: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00009e80: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-00009e90: 656c 662e 5f5f 706f 7374 5f72 6571 7565  elf.__post_reque
-00009ea0: 7374 2875 726c 3d75 726c 2c20 6461 7461  st(url=url, data
-00009eb0: 3d64 6174 6129 0a0a 2020 2020 2020 2020  =data)..        
-00009ec0: 7365 6c66 2e5f 5f72 6169 7365 5f6f 6e5f  self.__raise_on_
-00009ed0: 6572 726f 7228 7265 7370 6f6e 7365 290a  error(response).
-00009ee0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009ef0: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
-00009f00: 6620 6765 745f 6578 7472 6163 7465 645f  f get_extracted_
-00009f10: 6669 6c65 7328 7365 6c66 2c20 7361 6d70  files(self, samp
-00009f20: 6c65 5f68 6173 682c 2070 6167 655f 7369  le_hash, page_si
-00009f30: 7a65 3d4e 6f6e 652c 2070 6167 653d 4e6f  ze=None, page=No
-00009f40: 6e65 293a 0a20 2020 2020 2020 2022 2222  ne):.        """
-00009f50: 5448 4953 204d 4554 484f 4420 4953 2044  THIS METHOD IS D
-00009f60: 4550 5245 4341 5445 442e 2055 7365 206c  EPRECATED. Use l
-00009f70: 6973 745f 6578 7472 6163 7465 645f 6669  ist_extracted_fi
-00009f80: 6c65 735f 7632 2069 6e73 7465 6164 2e0a  les_v2 instead..
-00009f90: 0a20 2020 2020 2020 2047 6574 2061 206c  .        Get a l
-00009fa0: 6973 7420 6f66 2061 6c6c 2066 696c 6573  ist of all files
-00009fb0: 2054 6974 616e 6975 6d43 6f72 6520 656e   TitaniumCore en
-00009fc0: 6769 6e65 2065 7874 7261 6374 6564 2066  gine extracted f
-00009fd0: 726f 6d20 7468 6520 7265 7175 6573 7465  rom the requeste
-00009fe0: 6420 7361 6d70 6c65 2064 7572 696e 6720  d sample during 
-00009ff0: 7374 6174 6963 2061 6e61 6c79 7369 732e  static analysis.
-0000a000: 0a20 2020 2020 2020 2049 6620 7573 6564  .        If used
-0000a010: 2c20 7061 6765 5f73 697a 6520 616e 6420  , page_size and 
-0000a020: 7061 6765 206e 6565 6420 746f 2062 6520  page need to be 
-0000a030: 636f 6d62 696e 6564 2077 6869 6c65 206b  combined while k
-0000a040: 6565 7069 6e67 2074 7261 636b 206f 6620  eeping track of 
-0000a050: 7265 6d61 696e 696e 6720 7061 6765 7320  remaining pages 
-0000a060: 6f66 2072 6573 756c 7473 2e0a 2020 2020  of results..    
-0000a070: 2020 2020 652e 672e 202d 2069 6620 7265      e.g. - if re
-0000a080: 7375 6c74 2063 6f75 6e74 2069 7320 3520  sult count is 5 
-0000a090: 616e 6420 7061 6765 5f73 697a 6520 6973  and page_size is
-0000a0a0: 2032 2c20 7468 6572 6520 6973 206f 6e6c   2, there is onl
-0000a0b0: 7920 3320 7061 6765 7320 776f 7274 6820  y 3 pages worth 
-0000a0c0: 6f66 2072 6573 756c 7473 2e0a 2020 2020  of results..    
-0000a0d0: 2020 2020 5468 6520 7061 6765 2070 6172      The page par
-0000a0e0: 616d 6574 6572 2063 616e 206e 6f74 2062  ameter can not b
-0000a0f0: 6520 7573 6564 2077 6974 686f 7574 2070  e used without p
-0000a100: 6167 655f 7369 7a65 2e20 7061 6765 2061  age_size. page a
-0000a110: 6e64 2070 6167 655f 7369 7a65 206e 6565  nd page_size nee
-0000a120: 6420 746f 2062 6520 7573 6564 2074 6f67  d to be used tog
-0000a130: 6574 6865 722e 0a20 2020 2020 2020 2049  ether..        I
-0000a140: 6620 7061 6765 5f73 697a 6520 616e 6420  f page_size and 
-0000a150: 7061 6765 2061 7265 206e 6f74 2075 7365  page are not use
-0000a160: 642c 2061 6c6c 2072 6573 756c 7473 2061  d, all results a
-0000a170: 7265 2072 6574 7572 6e65 6420 696e 206f  re returned in o
-0000a180: 6e65 2072 6573 706f 6e73 652e 0a20 2020  ne response..   
-0000a190: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-0000a1a0: 7361 6d70 6c65 5f68 6173 683a 2068 6173  sample_hash: has
-0000a1b0: 6820 7374 7269 6e67 0a20 2020 2020 2020  h string.       
-0000a1c0: 2020 2020 203a 7479 7065 2073 616d 706c       :type sampl
-0000a1d0: 655f 6861 7368 3a20 7374 720a 2020 2020  e_hash: str.    
-0000a1e0: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-0000a1f0: 6167 655f 7369 7a65 3a20 6966 2064 6566  age_size: if def
-0000a200: 696e 6564 2c20 7265 7375 6c74 7320 6172  ined, results ar
-0000a210: 6520 7265 7475 726e 6564 2069 6e20 7061  e returned in pa
-0000a220: 6765 7320 6f66 2074 6869 7320 7369 7a65  ges of this size
-0000a230: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-0000a240: 7065 2070 6167 655f 7369 7a65 3a20 696e  pe page_size: in
-0000a250: 740a 2020 2020 2020 2020 2020 2020 3a70  t.            :p
-0000a260: 6172 616d 2070 6167 653a 2064 6566 696e  aram page: defin
-0000a270: 6573 2077 6869 6368 2070 6167 6520 6f66  es which page of
-0000a280: 2072 6573 756c 7473 2073 686f 756c 6420   results should 
-0000a290: 6265 2066 6574 6368 6564 0a20 2020 2020  be fetched.     
-0000a2a0: 2020 2020 2020 203a 7479 7065 2070 6167         :type pag
-0000a2b0: 653a 2069 6e74 0a20 2020 2020 2020 2020  e: int.         
-0000a2c0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
-0000a2d0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
-0000a2e0: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
-0000a2f0: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
-0000a300: 2020 2022 2222 0a20 2020 2020 2020 2077     """.        w
-0000a310: 6172 6e28 2254 6869 7320 6d65 7468 6f64  arn("This method
-0000a320: 2069 7320 6465 7072 6563 6174 6564 2e20   is deprecated. 
-0000a330: 5573 6520 6c69 7374 5f65 7874 7261 6374  Use list_extract
-0000a340: 6564 5f66 696c 6573 5f76 3220 696e 7374  ed_files_v2 inst
-0000a350: 6561 642e 222c 2044 6570 7265 6361 7469  ead.", Deprecati
-0000a360: 6f6e 5761 726e 696e 6729 0a0a 2020 2020  onWarning)..    
-0000a370: 2020 2020 7661 6c69 6461 7465 5f68 6173      validate_has
-0000a380: 6865 7328 0a20 2020 2020 2020 2020 2020  hes(.           
-0000a390: 2068 6173 685f 696e 7075 743d 5b73 616d   hash_input=[sam
-0000a3a0: 706c 655f 6861 7368 5d2c 0a20 2020 2020  ple_hash],.     
-0000a3b0: 2020 2020 2020 2061 6c6c 6f77 6564 5f68         allowed_h
-0000a3c0: 6173 685f 7479 7065 733d 284d 4435 2c20  ash_types=(MD5, 
-0000a3d0: 5348 4131 2c20 5348 4132 3536 2c20 5348  SHA1, SHA256, SH
-0000a3e0: 4135 3132 290a 2020 2020 2020 2020 290a  A512).        ).
-0000a3f0: 0a20 2020 2020 2020 2065 6e64 706f 696e  .        endpoin
-0000a400: 7420 3d20 7365 6c66 2e5f 5f4c 4953 545f  t = self.__LIST_
-0000a410: 4558 5452 4143 5445 445f 4649 4c45 535f  EXTRACTED_FILES_
-0000a420: 454e 4450 4f49 4e54 2e66 6f72 6d61 7428  ENDPOINT.format(
-0000a430: 0a20 2020 2020 2020 2020 2020 2068 6173  .            has
-0000a440: 685f 7661 6c75 653d 7361 6d70 6c65 5f68  h_value=sample_h
-0000a450: 6173 680a 2020 2020 2020 2020 290a 0a20  ash.        ).. 
-0000a460: 2020 2020 2020 2075 726c 203d 2073 656c         url = sel
-0000a470: 662e 5f75 726c 2e66 6f72 6d61 7428 656e  f._url.format(en
-0000a480: 6470 6f69 6e74 3d65 6e64 706f 696e 7429  dpoint=endpoint)
-0000a490: 0a0a 2020 2020 2020 2020 6966 2028 7061  ..        if (pa
-0000a4a0: 6765 5f73 697a 6520 616e 6420 6e6f 7420  ge_size and not 
-0000a4b0: 7061 6765 2920 6f72 2028 6e6f 7420 7061  page) or (not pa
-0000a4c0: 6765 5f73 697a 6520 616e 6420 7061 6765  ge_size and page
-0000a4d0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000a4e0: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
-0000a4f0: 7272 6f72 2822 5061 7261 6d65 7465 7273  rror("Parameters
-0000a500: 2070 6167 655f 7369 7a65 2061 6e64 2070   page_size and p
-0000a510: 6167 6520 6d75 7374 2062 6520 7573 6564  age must be used
-0000a520: 2074 6f67 6574 6865 722e 2229 0a0a 2020   together.")..  
-0000a530: 2020 2020 2020 6966 2070 6167 653a 0a20        if page:. 
-0000a540: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000a550: 7420 6973 696e 7374 616e 6365 2870 6167  t isinstance(pag
-0000a560: 655f 7369 7a65 2c20 696e 7429 206f 7220  e_size, int) or 
-0000a570: 6e6f 7420 6973 696e 7374 616e 6365 2870  not isinstance(p
-0000a580: 6167 652c 2069 6e74 293a 0a20 2020 2020  age, int):.     
-0000a590: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000a5a0: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
-0000a5b0: 2822 7061 6765 5f73 697a 6520 616e 6420  ("page_size and 
-0000a5c0: 7061 6765 2070 6172 616d 6574 6572 7320  page parameters 
-0000a5d0: 6e65 6564 2074 6f20 6265 2069 6e74 6567  need to be integ
-0000a5e0: 6572 2e22 290a 0a20 2020 2020 2020 2020  er.")..         
-0000a5f0: 2020 2075 726c 203d 2022 7b75 726c 7d3f     url = "{url}?
-0000a600: 7061 6765 5f73 697a 653d 7b70 6167 655f  page_size={page_
-0000a610: 7369 7a65 7d26 7061 6765 3d7b 7061 6765  size}&page={page
-0000a620: 7d22 2e66 6f72 6d61 7428 0a20 2020 2020  }".format(.     
-0000a630: 2020 2020 2020 2020 2020 2075 726c 3d75             url=u
-0000a640: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
-0000a650: 2020 2020 7061 6765 5f73 697a 653d 7061      page_size=pa
-0000a660: 6765 5f73 697a 652c 0a20 2020 2020 2020  ge_size,.       
-0000a670: 2020 2020 2020 2020 2070 6167 653d 7061           page=pa
-0000a680: 6765 0a20 2020 2020 2020 2020 2020 2029  ge.            )
-0000a690: 0a0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-0000a6a0: 7365 203d 2073 656c 662e 5f5f 6765 745f  se = self.__get_
-0000a6b0: 7265 7175 6573 7428 7572 6c3d 7572 6c29  request(url=url)
-0000a6c0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-0000a6d0: 5f72 6169 7365 5f6f 6e5f 6572 726f 7228  _raise_on_error(
-0000a6e0: 7265 7370 6f6e 7365 290a 0a20 2020 2020  response)..     
-0000a6f0: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-0000a700: 7365 0a0a 2020 2020 6465 6620 6c69 7374  se..    def list
-0000a710: 5f65 7874 7261 6374 6564 5f66 696c 6573  _extracted_files
-0000a720: 5f76 3228 7365 6c66 2c20 7361 6d70 6c65  _v2(self, sample
-0000a730: 5f68 6173 682c 2070 6167 655f 7369 7a65  _hash, page_size
-0000a740: 3d4e 6f6e 652c 2070 6167 653d 4e6f 6e65  =None, page=None
-0000a750: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-0000a760: 7420 6120 6c69 7374 206f 6620 616c 6c20  t a list of all 
-0000a770: 6669 6c65 7320 5469 7461 6e69 756d 436f  files TitaniumCo
-0000a780: 7265 2065 6e67 696e 6520 6578 7472 6163  re engine extrac
-0000a790: 7465 6420 6672 6f6d 2074 6865 2072 6571  ted from the req
-0000a7a0: 7565 7374 6564 2073 616d 706c 6520 6475  uested sample du
-0000a7b0: 7269 6e67 2073 7461 7469 6320 616e 616c  ring static anal
-0000a7c0: 7973 6973 2e0a 2020 2020 2020 2020 4966  ysis..        If
-0000a7d0: 2074 6865 2070 6167 6520 7061 7261 6d65   the page parame
-0000a7e0: 7465 7220 6973 2075 7365 642c 2069 7420  ter is used, it 
-0000a7f0: 6e65 6564 7320 746f 2062 6520 636f 6d62  needs to be comb
-0000a800: 696e 6564 2077 6974 6820 7468 6520 7061  ined with the pa
-0000a810: 6765 5f73 697a 6520 7061 7261 6d65 7465  ge_size paramete
-0000a820: 7220 7768 696c 6520 6b65 6570 696e 6720  r while keeping 
-0000a830: 7472 6163 6b20 6f66 0a20 2020 2020 2020  track of.       
-0000a840: 2072 656d 6169 6e69 6e67 2070 6167 6573   remaining pages
-0000a850: 206f 6620 7265 7375 6c74 732e 0a20 2020   of results..   
-0000a860: 2020 2020 2065 2e67 2e20 2d20 6966 2072       e.g. - if r
-0000a870: 6573 756c 7420 636f 756e 7420 6973 2035  esult count is 5
-0000a880: 2061 6e64 2070 6167 655f 7369 7a65 2069   and page_size i
-0000a890: 7320 322c 2074 6865 7265 2069 7320 6f6e  s 2, there is on
-0000a8a0: 6c79 2033 2070 6167 6573 2077 6f72 7468  ly 3 pages worth
-0000a8b0: 206f 6620 7265 7375 6c74 732e 0a20 2020   of results..   
-0000a8c0: 2020 2020 2054 6865 2070 6167 655f 7369       The page_si
-0000a8d0: 7a65 2070 6172 616d 6574 6572 2063 616e  ze parameter can
-0000a8e0: 2062 6520 7573 6564 2077 6974 686f 7574   be used without
-0000a8f0: 2074 6865 2070 6167 6520 7061 7261 6d65   the page parame
-0000a900: 7465 722e 0a20 2020 2020 2020 2049 6620  ter..        If 
-0000a910: 7061 6765 5f73 697a 6520 616e 6420 7061  page_size and pa
-0000a920: 6765 2061 7265 206e 6f74 2075 7365 642c  ge are not used,
-0000a930: 2061 6c6c 2072 6573 756c 7473 2061 7265   all results are
-0000a940: 2072 6574 7572 6e65 6420 696e 206f 6e65   returned in one
-0000a950: 2072 6573 706f 6e73 652e 0a20 2020 2020   response..     
-0000a960: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
-0000a970: 6d70 6c65 5f68 6173 683a 2068 6173 6820  mple_hash: hash 
-0000a980: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-0000a990: 2020 203a 7479 7065 2073 616d 706c 655f     :type sample_
-0000a9a0: 6861 7368 3a20 7374 720a 2020 2020 2020  hash: str.      
-0000a9b0: 2020 2020 2020 3a70 6172 616d 2070 6167        :param pag
-0000a9c0: 655f 7369 7a65 3a20 6465 6669 6e65 7320  e_size: defines 
-0000a9d0: 7468 6520 6e75 6d62 6572 206f 6620 7265  the number of re
-0000a9e0: 7375 6c74 7320 6f6e 2074 6865 2072 6574  sults on the ret
-0000a9f0: 7572 6e65 6420 7061 6765 0a20 2020 2020  urned page.     
-0000aa00: 2020 2020 2020 203a 7479 7065 2070 6167         :type pag
-0000aa10: 655f 7369 7a65 3a20 696e 740a 2020 2020  e_size: int.    
-0000aa20: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-0000aa30: 6167 653a 2064 6566 696e 6573 2077 6869  age: defines whi
-0000aa40: 6368 2070 6167 6520 6f66 2072 6573 756c  ch page of resul
-0000aa50: 7473 2073 686f 756c 6420 6265 2066 6574  ts should be fet
-0000aa60: 6368 6564 0a20 2020 2020 2020 2020 2020  ched.           
-0000aa70: 203a 7479 7065 2070 6167 653a 2069 6e74   :type page: int
-0000aa80: 0a20 2020 2020 2020 2020 2020 203a 7265  .            :re
-0000aa90: 7475 726e 3a20 7265 7370 6f6e 7365 0a20  turn: response. 
-0000aaa0: 2020 2020 2020 2020 2020 203a 7274 7970             :rtyp
-0000aab0: 653a 2072 6571 7565 7374 732e 5265 7370  e: requests.Resp
-0000aac0: 6f6e 7365 0a20 2020 2020 2020 2022 2222  onse.        """
-0000aad0: 0a20 2020 2020 2020 2076 616c 6964 6174  .        validat
-0000aae0: 655f 6861 7368 6573 280a 2020 2020 2020  e_hashes(.      
-0000aaf0: 2020 2020 2020 6861 7368 5f69 6e70 7574        hash_input
-0000ab00: 3d5b 7361 6d70 6c65 5f68 6173 685d 2c0a  =[sample_hash],.
-0000ab10: 2020 2020 2020 2020 2020 2020 616c 6c6f              allo
-0000ab20: 7765 645f 6861 7368 5f74 7970 6573 3d28  wed_hash_types=(
-0000ab30: 4d44 352c 2053 4841 312c 2053 4841 3235  MD5, SHA1, SHA25
-0000ab40: 362c 2053 4841 3531 3229 0a20 2020 2020  6, SHA512).     
-0000ab50: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-0000ab60: 2070 6167 6520 616e 6420 6e6f 7420 7061   page and not pa
-0000ab70: 6765 5f73 697a 653a 0a20 2020 2020 2020  ge_size:.       
-0000ab80: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
-0000ab90: 496e 7075 7445 7272 6f72 2822 4966 2074  InputError("If t
-0000aba0: 6865 2070 6167 6520 7061 7261 6d65 7465  he page paramete
-0000abb0: 7220 6973 2075 7365 642c 2070 6167 655f  r is used, page_
-0000abc0: 7369 7a65 206d 7573 7420 6265 2064 6566  size must be def
-0000abd0: 696e 6564 2e22 290a 0a20 2020 2020 2020  ined.")..       
-0000abe0: 2065 6e64 706f 696e 7420 3d20 7365 6c66   endpoint = self
-0000abf0: 2e5f 5f4c 4953 545f 4558 5452 4143 5445  .__LIST_EXTRACTE
-0000ac00: 445f 4649 4c45 535f 454e 4450 4f49 4e54  D_FILES_ENDPOINT
-0000ac10: 5f56 322e 666f 726d 6174 280a 2020 2020  _V2.format(.    
-0000ac20: 2020 2020 2020 2020 6861 7368 5f76 616c          hash_val
-0000ac30: 7565 3d73 616d 706c 655f 6861 7368 0a20  ue=sample_hash. 
-0000ac40: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000ac50: 2020 7572 6c20 3d20 7365 6c66 2e5f 7572    url = self._ur
-0000ac60: 6c2e 666f 726d 6174 2865 6e64 706f 696e  l.format(endpoin
-0000ac70: 743d 656e 6470 6f69 6e74 290a 0a20 2020  t=endpoint)..   
-0000ac80: 2020 2020 2070 6172 616d 735f 6469 6374       params_dict
-0000ac90: 203d 207b 2270 6167 6522 3a20 7061 6765   = {"page": page
-0000aca0: 2c20 2270 6167 655f 7369 7a65 223a 2070  , "page_size": p
-0000acb0: 6167 655f 7369 7a65 7d0a 0a20 2020 2020  age_size}..     
-0000acc0: 2020 2070 6172 616d 735f 6c69 7374 203d     params_list =
-0000acd0: 205b 5d0a 0a20 2020 2020 2020 2066 6f72   []..        for
-0000ace0: 206b 6579 2c20 7661 6c75 6520 696e 2070   key, value in p
-0000acf0: 6172 616d 735f 6469 6374 2e69 7465 6d73  arams_dict.items
-0000ad00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000ad10: 6966 2076 616c 7565 3a0a 2020 2020 2020  if value:.      
-0000ad20: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000ad30: 2069 7369 6e73 7461 6e63 6528 7661 6c75   isinstance(valu
-0000ad40: 652c 2069 6e74 293a 0a20 2020 2020 2020  e, int):.       
-0000ad50: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000ad60: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-0000ad70: 6f72 2822 7b70 6172 616d 7d20 7061 7261  or("{param} para
-0000ad80: 6d65 7465 7220 6d75 7374 2062 6520 696e  meter must be in
-0000ad90: 7465 6765 722e 222e 666f 726d 6174 2870  teger.".format(p
-0000ada0: 6172 616d 3d6b 6579 2929 0a0a 2020 2020  aram=key))..    
-0000adb0: 2020 2020 2020 2020 2020 2020 7061 7261              para
-0000adc0: 6d73 5f6c 6973 742e 6170 7065 6e64 2822  ms_list.append("
-0000add0: 7b6b 6579 7d3d 7b76 616c 7565 7d22 2e66  {key}={value}".f
-0000ade0: 6f72 6d61 7428 6b65 793d 6b65 792c 2076  ormat(key=key, v
-0000adf0: 616c 7565 3d76 616c 7565 2929 0a0a 2020  alue=value))..  
-0000ae00: 2020 2020 2020 6966 2070 6172 616d 735f        if params_
-0000ae10: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
-0000ae20: 2020 7061 7261 6d73 203d 2022 3f7b 7061    params = "?{pa
-0000ae30: 7261 6d73 7d22 2e66 6f72 6d61 7428 7061  rams}".format(pa
-0000ae40: 7261 6d73 3d22 2622 2e6a 6f69 6e28 7061  rams="&".join(pa
-0000ae50: 7261 6d73 5f6c 6973 7429 290a 0a20 2020  rams_list))..   
-0000ae60: 2020 2020 2020 2020 2075 726c 203d 2022           url = "
-0000ae70: 7b75 726c 7d7b 7061 7261 6d73 7d22 2e66  {url}{params}".f
-0000ae80: 6f72 6d61 7428 7572 6c3d 7572 6c2c 2070  ormat(url=url, p
-0000ae90: 6172 616d 733d 7061 7261 6d73 290a 0a20  arams=params).. 
-0000aea0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0000aeb0: 3d20 7365 6c66 2e5f 5f67 6574 5f72 6571  = self.__get_req
-0000aec0: 7565 7374 2875 726c 3d75 726c 290a 0a20  uest(url=url).. 
-0000aed0: 2020 2020 2020 2073 656c 662e 5f5f 7261         self.__ra
-0000aee0: 6973 655f 6f6e 5f65 7272 6f72 2872 6573  ise_on_error(res
-0000aef0: 706f 6e73 6529 0a0a 2020 2020 2020 2020  ponse)..        
-0000af00: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0000af10: 0a20 2020 2064 6566 206c 6973 745f 6578  .    def list_ex
-0000af20: 7472 6163 7465 645f 6669 6c65 735f 7632  tracted_files_v2
-0000af30: 5f61 6767 7265 6761 7465 6428 7365 6c66  _aggregated(self
-0000af40: 2c20 7361 6d70 6c65 5f68 6173 682c 206d  , sample_hash, m
-0000af50: 6178 5f72 6573 756c 7473 3d35 3030 3029  ax_results=5000)
-0000af60: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-0000af70: 2061 206c 6973 7420 6f66 2061 6c6c 2066   a list of all f
-0000af80: 696c 6573 2054 6974 616e 6975 6d43 6f72  iles TitaniumCor
-0000af90: 6520 656e 6769 6e65 2065 7874 7261 6374  e engine extract
-0000afa0: 6564 2066 726f 6d20 7468 6520 7265 7175  ed from the requ
-0000afb0: 6573 7465 6420 7361 6d70 6c65 2064 7572  ested sample dur
-0000afc0: 696e 6720 7374 6174 6963 2061 6e61 6c79  ing static analy
-0000afd0: 7369 732e 0a20 2020 2020 2020 2050 6167  sis..        Pag
-0000afe0: 696e 6720 6973 2064 6f6e 6520 6175 746f  ing is done auto
-0000aff0: 6d61 7469 6361 6c6c 7920 616e 6420 7265  matically and re
-0000b000: 7375 6c74 7320 6672 6f6d 2069 6e64 6976  sults from indiv
-0000b010: 6964 7561 6c20 7265 7370 6f6e 7365 7320  idual responses 
-0000b020: 6167 6772 6567 6174 6564 2069 6e74 6f20  aggregated into 
-0000b030: 6f6e 6520 6c69 7374 2061 6e64 2072 6574  one list and ret
-0000b040: 7572 6e65 642e 0a20 2020 2020 2020 2054  urned..        T
-0000b050: 6865 206d 6178 5f72 6573 756c 7473 2070  he max_results p
-0000b060: 6172 616d 6574 6572 2064 6566 696e 6573  arameter defines
-0000b070: 2074 6865 206d 6178 696d 756d 206e 756d   the maximum num
-0000b080: 6265 7220 6f66 2072 6573 756c 7473 2074  ber of results t
-0000b090: 6f20 6265 2072 6574 7572 6e65 6420 746f  o be returned to
-0000b0a0: 2074 6865 206c 6973 742e 0a20 2020 2020   the list..     
-0000b0b0: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
-0000b0c0: 6d70 6c65 5f68 6173 683a 2068 6173 6820  mple_hash: hash 
-0000b0d0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-0000b0e0: 2020 203a 7479 7065 2073 616d 706c 655f     :type sample_
-0000b0f0: 6861 7368 3a20 7374 720a 2020 2020 2020  hash: str.      
-0000b100: 2020 2020 2020 3a70 6172 616d 206d 6178        :param max
-0000b110: 5f72 6573 756c 7473 3a20 6d61 7869 6d75  _results: maximu
-0000b120: 6d20 6e75 6d62 6572 206f 6620 7265 7375  m number of resu
-0000b130: 6c74 7320 746f 2062 6520 7265 7475 726e  lts to be return
-0000b140: 6564 0a20 2020 2020 2020 2020 2020 203a  ed.            :
-0000b150: 7479 7065 206d 6178 5f72 6573 756c 7473  type max_results
-0000b160: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
-0000b170: 2020 3a72 6574 7572 6e3a 206c 6973 7420    :return: list 
-0000b180: 6f66 2072 6573 756c 7473 0a20 2020 2020  of results.     
-0000b190: 2020 2020 2020 203a 7274 7970 653a 206c         :rtype: l
-0000b1a0: 6973 740a 2020 2020 2020 2020 2222 220a  ist.        """.
-0000b1b0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-0000b1c0: 2020 2020 2072 6573 756c 745f 6c69 7374       result_list
-0000b1d0: 203d 205b 5d0a 2020 2020 2020 2020 6e65   = [].        ne
-0000b1e0: 7874 5f70 6167 6520 3d20 310a 0a20 2020  xt_page = 1..   
-0000b1f0: 2020 2020 2077 6869 6c65 206e 6578 745f       while next_
-0000b200: 7061 6765 3a0a 2020 2020 2020 2020 2020  page:.          
-0000b210: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-0000b220: 662e 6c69 7374 5f65 7874 7261 6374 6564  f.list_extracted
-0000b230: 5f66 696c 6573 5f76 3228 0a20 2020 2020  _files_v2(.     
-0000b240: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
-0000b250: 655f 6861 7368 3d73 616d 706c 655f 6861  e_hash=sample_ha
-0000b260: 7368 2c0a 2020 2020 2020 2020 2020 2020  sh,.            
-0000b270: 2020 2020 7061 6765 3d6e 6578 745f 7061      page=next_pa
-0000b280: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
-0000b290: 2020 2020 7061 6765 5f73 697a 653d 3130      page_size=10
-0000b2a0: 300a 2020 2020 2020 2020 2020 2020 290a  0.            ).
-0000b2b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000b2c0: 706f 6e73 655f 6a73 6f6e 203d 2072 6573  ponse_json = res
-0000b2d0: 706f 6e73 652e 6a73 6f6e 2829 0a0a 2020  ponse.json()..  
-0000b2e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000b2f0: 7320 3d20 7265 7370 6f6e 7365 5f6a 736f  s = response_jso
-0000b300: 6e2e 6765 7428 2272 6573 756c 7473 222c  n.get("results",
-0000b310: 205b 5d29 0a20 2020 2020 2020 2020 2020   []).           
-0000b320: 2072 6573 756c 745f 6c69 7374 2e65 7874   result_list.ext
-0000b330: 656e 6428 7265 7375 6c74 7329 0a0a 2020  end(results)..  
-0000b340: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-0000b350: 2872 6573 756c 745f 6c69 7374 2920 3e20  (result_list) > 
-0000b360: 6d61 785f 7265 7375 6c74 733a 0a20 2020  max_results:.   
-0000b370: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000b380: 756c 7473 203d 2072 6573 756c 745f 6c69  ults = result_li
-0000b390: 7374 5b3a 6d61 785f 7265 7375 6c74 735d  st[:max_results]
-0000b3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b3b0: 2072 6574 7572 6e20 7265 7375 6c74 730a   return results.
-0000b3c0: 0a20 2020 2020 2020 2020 2020 206e 6578  .            nex
-0000b3d0: 745f 7061 6765 5f75 726c 203d 2072 6573  t_page_url = res
-0000b3e0: 706f 6e73 655f 6a73 6f6e 2e67 6574 2822  ponse_json.get("
-0000b3f0: 6e65 7874 222c 204e 6f6e 6529 0a20 2020  next", None).   
-0000b400: 2020 2020 2020 2020 206e 6578 745f 7061           next_pa
-0000b410: 6765 203d 2069 6e74 286e 6578 745f 7061  ge = int(next_pa
-0000b420: 6765 5f75 726c 2e73 706c 6974 2822 3f22  ge_url.split("?"
-0000b430: 295b 315d 2e73 706c 6974 2822 2622 295b  )[1].split("&")[
-0000b440: 305d 2e73 706c 6974 2822 3d22 295b 315d  0].split("=")[1]
-0000b450: 2920 6966 206e 6578 745f 7061 6765 5f75  ) if next_page_u
-0000b460: 726c 2065 6c73 6520 4e6f 6e65 0a0a 2020  rl else None..  
-0000b470: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0000b480: 756c 745f 6c69 7374 0a0a 2020 2020 6465  ult_list..    de
-0000b490: 6620 646f 776e 6c6f 6164 5f65 7874 7261  f download_extra
-0000b4a0: 6374 6564 5f66 696c 6573 2873 656c 662c  cted_files(self,
-0000b4b0: 2073 616d 706c 655f 6861 7368 293a 0a20   sample_hash):. 
-0000b4c0: 2020 2020 2020 2022 2222 4163 6365 7074         """Accept
-0000b4d0: 7320 6120 7369 6e67 6c65 2068 6173 6820  s a single hash 
-0000b4e0: 7374 7269 6e67 2061 6e64 2072 6574 7572  string and retur
-0000b4f0: 6e73 2061 2064 6f77 6e6c 6f61 6461 626c  ns a downloadabl
-0000b500: 6520 6172 6368 6976 6520 6669 6c65 0a20  e archive file. 
-0000b510: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
-0000b520: 6720 6669 6c65 7320 6578 7472 6163 7465  g files extracte
-0000b530: 6420 6672 6f6d 2074 6865 2064 6573 6972  d from the desir
-0000b540: 6564 2073 616d 706c 652e 0a20 2020 2020  ed sample..     
-0000b550: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
-0000b560: 6d70 6c65 5f68 6173 683a 2068 6173 6820  mple_hash: hash 
-0000b570: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-0000b580: 2020 203a 7479 7065 2073 616d 706c 655f     :type sample_
-0000b590: 6861 7368 3a20 7374 720a 2020 2020 2020  hash: str.      
-0000b5a0: 2020 2020 2020 3a72 6574 7572 6e3a 2072        :return: r
-0000b5b0: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-0000b5c0: 2020 2020 3a72 7479 7065 3a20 7265 7175      :rtype: requ
-0000b5d0: 6573 7473 2e52 6573 706f 6e73 650a 2020  ests.Response.  
-0000b5e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000b5f0: 2020 7661 6c69 6461 7465 5f68 6173 6865    validate_hashe
-0000b600: 7328 0a20 2020 2020 2020 2020 2020 2068  s(.            h
-0000b610: 6173 685f 696e 7075 743d 5b73 616d 706c  ash_input=[sampl
-0000b620: 655f 6861 7368 5d2c 0a20 2020 2020 2020  e_hash],.       
-0000b630: 2020 2020 2061 6c6c 6f77 6564 5f68 6173       allowed_has
-0000b640: 685f 7479 7065 733d 284d 4435 2c20 5348  h_types=(MD5, SH
-0000b650: 4131 2c20 5348 4132 3536 2c20 5348 4135  A1, SHA256, SHA5
-0000b660: 3132 290a 2020 2020 2020 2020 290a 0a20  12).        ).. 
-0000b670: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
-0000b680: 3d20 7365 6c66 2e5f 5f44 4f57 4e4c 4f41  = self.__DOWNLOA
-0000b690: 445f 4558 5452 4143 5445 445f 4649 4c45  D_EXTRACTED_FILE
-0000b6a0: 535f 454e 4450 4f49 4e54 2e66 6f72 6d61  S_ENDPOINT.forma
-0000b6b0: 7428 6861 7368 5f76 616c 7565 3d73 616d  t(hash_value=sam
-0000b6c0: 706c 655f 6861 7368 290a 0a20 2020 2020  ple_hash)..     
-0000b6d0: 2020 2075 726c 203d 2073 656c 662e 5f75     url = self._u
-0000b6e0: 726c 2e66 6f72 6d61 7428 656e 6470 6f69  rl.format(endpoi
-0000b6f0: 6e74 3d65 6e64 706f 696e 7429 0a0a 2020  nt=endpoint)..  
-0000b700: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0000b710: 2073 656c 662e 5f5f 6765 745f 7265 7175   self.__get_requ
-0000b720: 6573 7428 7572 6c3d 7572 6c29 0a0a 2020  est(url=url)..  
-0000b730: 2020 2020 2020 7365 6c66 2e5f 5f72 6169        self.__rai
-0000b740: 7365 5f6f 6e5f 6572 726f 7228 7265 7370  se_on_error(resp
-0000b750: 6f6e 7365 290a 0a20 2020 2020 2020 2072  onse)..        r
-0000b760: 6574 7572 6e20 7265 7370 6f6e 7365 0a0a  eturn response..
-0000b770: 2020 2020 6465 6620 646f 776e 6c6f 6164      def download
-0000b780: 5f73 616d 706c 6528 7365 6c66 2c20 7361  _sample(self, sa
-0000b790: 6d70 6c65 5f68 6173 6829 3a0a 2020 2020  mple_hash):.    
-0000b7a0: 2020 2020 2222 2241 6363 6570 7473 2061      """Accepts a
-0000b7b0: 2073 696e 676c 6520 6861 7368 2073 7472   single hash str
-0000b7c0: 696e 6720 616e 6420 7265 7475 726e 7320  ing and returns 
-0000b7d0: 6120 646f 776e 6c6f 6164 6162 6c65 2073  a downloadable s
-0000b7e0: 616d 706c 652e 0a20 2020 2020 2020 2020  ample..         
-0000b7f0: 2020 203a 7061 7261 6d20 7361 6d70 6c65     :param sample
-0000b800: 5f68 6173 683a 2068 6173 6820 7374 7269  _hash: hash stri
-0000b810: 6e67 0a20 2020 2020 2020 2020 2020 203a  ng.            :
-0000b820: 7479 7065 2073 616d 706c 655f 6861 7368  type sample_hash
-0000b830: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-0000b840: 2020 3a72 6574 7572 6e3a 2072 6573 706f    :return: respo
-0000b850: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
-0000b860: 3a72 7479 7065 3a20 7265 7175 6573 7473  :rtype: requests
-0000b870: 2e52 6573 706f 6e73 650a 2020 2020 2020  .Response.      
-0000b880: 2020 2222 220a 2020 2020 2020 2020 7661    """.        va
-0000b890: 6c69 6461 7465 5f68 6173 6865 7328 0a20  lidate_hashes(. 
-0000b8a0: 2020 2020 2020 2020 2020 2068 6173 685f             hash_
-0000b8b0: 696e 7075 743d 5b73 616d 706c 655f 6861  input=[sample_ha
-0000b8c0: 7368 5d2c 0a20 2020 2020 2020 2020 2020  sh],.           
-0000b8d0: 2061 6c6c 6f77 6564 5f68 6173 685f 7479   allowed_hash_ty
-0000b8e0: 7065 733d 284d 4435 2c20 5348 4131 2c20  pes=(MD5, SHA1, 
-0000b8f0: 5348 4132 3536 2c20 5348 4135 3132 290a  SHA256, SHA512).
-0000b900: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000b910: 2020 2065 6e64 706f 696e 7420 3d20 7365     endpoint = se
-0000b920: 6c66 2e5f 5f44 4f57 4e4c 4f41 445f 5341  lf.__DOWNLOAD_SA
-0000b930: 4d50 4c45 5f45 4e44 504f 494e 542e 666f  MPLE_ENDPOINT.fo
-0000b940: 726d 6174 2868 6173 685f 7661 6c75 653d  rmat(hash_value=
-0000b950: 7361 6d70 6c65 5f68 6173 6829 0a0a 2020  sample_hash)..  
-0000b960: 2020 2020 2020 7572 6c20 3d20 7365 6c66        url = self
-0000b970: 2e5f 7572 6c2e 666f 726d 6174 2865 6e64  ._url.format(end
-0000b980: 706f 696e 743d 656e 6470 6f69 6e74 290a  point=endpoint).
-0000b990: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-0000b9a0: 6520 3d20 7365 6c66 2e5f 5f67 6574 5f72  e = self.__get_r
-0000b9b0: 6571 7565 7374 2875 726c 3d75 726c 290a  equest(url=url).
-0000b9c0: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
-0000b9d0: 7261 6973 655f 6f6e 5f65 7272 6f72 2872  raise_on_error(r
-0000b9e0: 6573 706f 6e73 6529 0a0a 2020 2020 2020  esponse)..      
-0000b9f0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-0000ba00: 650a 0a20 2020 2064 6566 2064 656c 6574  e..    def delet
-0000ba10: 655f 7361 6d70 6c65 7328 7365 6c66 2c20  e_samples(self, 
-0000ba20: 6861 7368 5f69 6e70 7574 293a 0a20 2020  hash_input):.   
-0000ba30: 2020 2020 2022 2222 4163 6365 7074 7320       """Accepts 
-0000ba40: 6120 7369 6e67 6c65 2068 6173 6820 7374  a single hash st
-0000ba50: 7269 6e67 206f 7220 6120 6c69 7374 206f  ring or a list o
-0000ba60: 6620 6861 7368 6573 2061 6e64 2064 656c  f hashes and del
-0000ba70: 6574 6573 2074 6865 2063 6f72 7265 7370  etes the corresp
-0000ba80: 6f6e 6469 6e67 2073 616d 706c 6573 2e0a  onding samples..
-0000ba90: 2020 2020 2020 2020 5468 6973 206d 6574          This met
-0000baa0: 686f 6420 636f 6d62 696e 6573 2074 6865  hod combines the
-0000bab0: 2075 7365 206f 6620 7477 6f20 656e 6470   use of two endp
-0000bac0: 6f69 6e74 7320 666f 7220 7468 6520 666f  oints for the fo
-0000bad0: 6c6c 6f77 696e 6720 7477 6f20 6163 7469  llowing two acti
-0000bae0: 6f6e 732e 0a20 2020 2020 2020 202d 2044  ons..        - D
-0000baf0: 656c 6574 6520 6120 7369 6e67 6c65 2073  elete a single s
-0000bb00: 616d 706c 653a 2027 4465 6c65 7465 2073  ample: 'Delete s
-0000bb10: 616d 706c 6527 2065 6e64 706f 696e 740a  ample' endpoint.
-0000bb20: 2020 2020 2020 2020 2d20 4465 6c65 7465          - Delete
-0000bb30: 2061 2062 6174 6368 206f 6620 7361 6d70   a batch of samp
-0000bb40: 6c65 733a 2027 4465 6c65 7465 206d 756c  les: 'Delete mul
-0000bb50: 7469 706c 6520 7361 6d70 6c65 7320 7632  tiple samples v2
-0000bb60: 2720 656e 6470 6f69 6e74 0a20 2020 2020  ' endpoint.     
-0000bb70: 2020 2020 2020 203a 7061 7261 6d20 6861         :param ha
-0000bb80: 7368 5f69 6e70 7574 3a20 7369 6e67 6c65  sh_input: single
-0000bb90: 2068 6173 6820 7374 7269 6e67 206f 7220   hash string or 
-0000bba0: 6120 6c69 7374 206f 6620 6861 7368 6573  a list of hashes
-0000bbb0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-0000bbc0: 7065 2068 6173 685f 696e 7075 743a 2073  pe hash_input: s
-0000bbd0: 7472 206f 7220 6c69 7374 5b73 7472 5d0a  tr or list[str].
-0000bbe0: 2020 2020 2020 2020 2020 2020 3a72 6574              :ret
-0000bbf0: 7572 6e3a 2072 6573 706f 6e73 650a 2020  urn: response.  
-0000bc00: 2020 2020 2020 2020 2020 3a72 7479 7065            :rtype
-0000bc10: 3a20 7265 7175 6573 7473 2e52 6573 706f  : requests.Respo
-0000bc20: 6e73 650a 2020 2020 2020 2020 2222 220a  nse.        """.
-0000bc30: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000bc40: 7461 6e63 6528 6861 7368 5f69 6e70 7574  tance(hash_input
-0000bc50: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-0000bc60: 2020 2020 7661 6c69 6461 7465 5f68 6173      validate_has
-0000bc70: 6865 7328 0a20 2020 2020 2020 2020 2020  hes(.           
-0000bc80: 2020 2020 2068 6173 685f 696e 7075 743d       hash_input=
-0000bc90: 5b68 6173 685f 696e 7075 745d 2c0a 2020  [hash_input],.  
-0000bca0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-0000bcb0: 6c6f 7765 645f 6861 7368 5f74 7970 6573  lowed_hash_types
-0000bcc0: 3d28 4d44 352c 2053 4841 312c 2053 4841  =(MD5, SHA1, SHA
-0000bcd0: 3235 362c 2053 4841 3531 3229 0a20 2020  256, SHA512).   
-0000bce0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000bcf0: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
-0000bd00: 203d 2073 656c 662e 5f5f 4445 4c45 5445   = self.__DELETE
-0000bd10: 5f53 414d 504c 455f 454e 4450 4f49 4e54  _SAMPLE_ENDPOINT
-0000bd20: 2e66 6f72 6d61 7428 6861 7368 5f76 616c  .format(hash_val
-0000bd30: 7565 3d68 6173 685f 696e 7075 7429 0a0a  ue=hash_input)..
-0000bd40: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
-0000bd50: 3d20 7365 6c66 2e5f 7572 6c2e 666f 726d  = self._url.form
-0000bd60: 6174 2865 6e64 706f 696e 743d 656e 6470  at(endpoint=endp
-0000bd70: 6f69 6e74 290a 0a20 2020 2020 2020 2020  oint)..         
-0000bd80: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-0000bd90: 6c66 2e5f 5f64 656c 6574 655f 7265 7175  lf.__delete_requ
-0000bda0: 6573 7428 7572 6c3d 7572 6c29 0a0a 2020  est(url=url)..  
-0000bdb0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-0000bdc0: 7461 6e63 6528 6861 7368 5f69 6e70 7574  tance(hash_input
-0000bdd0: 2c20 6c69 7374 293a 0a20 2020 2020 2020  , list):.       
-0000bde0: 2020 2020 2076 616c 6964 6174 655f 6861       validate_ha
-0000bdf0: 7368 6573 280a 2020 2020 2020 2020 2020  shes(.          
-0000be00: 2020 2020 2020 6861 7368 5f69 6e70 7574        hash_input
-0000be10: 3d68 6173 685f 696e 7075 742c 0a20 2020  =hash_input,.   
-0000be20: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-0000be30: 6f77 6564 5f68 6173 685f 7479 7065 733d  owed_hash_types=
-0000be40: 284d 4435 2c20 5348 4131 2c20 5348 4132  (MD5, SHA1, SHA2
-0000be50: 3536 2c20 5348 4135 3132 290a 2020 2020  56, SHA512).    
-0000be60: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000be70: 2020 2020 2020 2075 726c 203d 2073 656c         url = sel
-0000be80: 662e 5f75 726c 2e66 6f72 6d61 7428 656e  f._url.format(en
-0000be90: 6470 6f69 6e74 3d73 656c 662e 5f5f 4445  dpoint=self.__DE
-0000bea0: 4c45 5445 5f53 414d 504c 4553 5f42 554c  LETE_SAMPLES_BUL
-0000beb0: 4b5f 454e 4450 4f49 4e54 5f56 3229 0a0a  K_ENDPOINT_V2)..
-0000bec0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000bed0: 203d 207b 2268 6173 685f 7661 6c75 6573   = {"hash_values
-0000bee0: 223a 2068 6173 685f 696e 7075 747d 0a0a  ": hash_input}..
-0000bef0: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-0000bf00: 6f6e 7365 203d 2073 656c 662e 5f5f 706f  onse = self.__po
-0000bf10: 7374 5f72 6571 7565 7374 2875 726c 3d75  st_request(url=u
-0000bf20: 726c 2c20 6461 7461 3d64 6174 6129 0a0a  rl, data=data)..
-0000bf30: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000bf40: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000bf50: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
-0000bf60: 2268 6173 685f 696e 7075 7420 7061 7261  "hash_input para
-0000bf70: 6d65 7465 7220 6d75 7374 2062 6520 6120  meter must be a 
-0000bf80: 7369 6e67 6c65 2068 6173 6820 7374 7269  single hash stri
-0000bf90: 6e67 206f 7220 220a 2020 2020 2020 2020  ng or ".        
-0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfb0: 2020 2020 2020 2020 2020 2261 206c 6973            "a lis
-0000bfc0: 7420 6f66 2068 6173 6820 7374 7269 6e67  t of hash string
-0000bfd0: 7320 6f66 2074 6865 2073 616d 6520 7479  s of the same ty
-0000bfe0: 7065 2e22 290a 0a20 2020 2020 2020 2073  pe.")..        s
-0000bff0: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
-0000c000: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
-0000c010: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000c020: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
-0000c030: 2063 6865 636b 5f73 616d 706c 655f 7265   check_sample_re
-0000c040: 6d6f 7661 6c5f 7374 6174 7573 5f76 3228  moval_status_v2(
-0000c050: 7365 6c66 2c20 7461 736b 5f69 6429 3a0a  self, task_id):.
-0000c060: 2020 2020 2020 2020 2222 2241 6363 6570          """Accep
-0000c070: 7473 2074 6865 2074 6173 6b20 4944 2072  ts the task ID r
-0000c080: 6574 7572 6e65 6420 6279 2074 6865 2062  eturned by the b
-0000c090: 756c 6b20 7361 6d70 6c65 2072 656d 6f76  ulk sample remov
-0000c0a0: 616c 2065 6e64 706f 696e 7420 616e 6420  al endpoint and 
-0000c0b0: 7265 7475 726e 7320 6120 7265 7370 6f6e  returns a respon
-0000c0c0: 7365 2074 6861 740a 2020 2020 2020 2020  se that.        
-0000c0d0: 696e 6469 6361 7465 7320 6966 2074 6865  indicates if the
-0000c0e0: 2072 656d 6f76 616c 2072 6571 7565 7374   removal request
-0000c0f0: 2077 6173 2066 696e 6973 6865 6420 7375   was finished su
-0000c100: 6363 6573 7366 756c 6c79 2061 6e64 2069  ccessfully and i
-0000c110: 6620 616c 6c20 7361 6d70 6c65 7320 6861  f all samples ha
-0000c120: 7665 2062 6565 6e20 6465 6c65 7465 642e  ve been deleted.
-0000c130: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-0000c140: 7261 6d20 7461 736b 5f69 643a 2049 4420  ram task_id: ID 
-0000c150: 6f66 2074 6865 2062 756c 6b20 7361 6d70  of the bulk samp
-0000c160: 6c65 2072 656d 6f76 616c 2074 6173 6b0a  le removal task.
-0000c170: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
-0000c180: 6520 7461 736b 5f69 643a 2073 7472 0a20  e task_id: str. 
-0000c190: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
-0000c1a0: 726e 3a20 7265 7370 6f6e 7365 0a20 2020  rn: response.   
-0000c1b0: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
-0000c1c0: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
-0000c1d0: 7365 0a20 2020 2020 2020 2022 2222 0a20  se.        """. 
-0000c1e0: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-0000c1f0: 696e 7374 616e 6365 2874 6173 6b5f 6964  instance(task_id
-0000c200: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-0000c210: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-0000c220: 6e70 7574 4572 726f 7228 2274 6173 6b5f  nputError("task_
-0000c230: 6964 2070 6172 616d 6574 6572 206d 7573  id parameter mus
-0000c240: 7420 6265 2073 7472 696e 672e 2229 0a0a  t be string.")..
-0000c250: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
-0000c260: 203d 2073 656c 662e 5f5f 4348 4543 4b5f   = self.__CHECK_
-0000c270: 5341 4d50 4c45 5f52 454d 4f56 414c 5f53  SAMPLE_REMOVAL_S
-0000c280: 5441 5455 535f 454e 4450 4f49 4e54 5f56  TATUS_ENDPOINT_V
-0000c290: 322e 666f 726d 6174 2874 6173 6b5f 6964  2.format(task_id
-0000c2a0: 3d74 6173 6b5f 6964 290a 0a20 2020 2020  =task_id)..     
-0000c2b0: 2020 2075 726c 203d 2073 656c 662e 5f75     url = self._u
-0000c2c0: 726c 2e66 6f72 6d61 7428 656e 6470 6f69  rl.format(endpoi
-0000c2d0: 6e74 3d65 6e64 706f 696e 7429 0a0a 2020  nt=endpoint)..  
-0000c2e0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0000c2f0: 2073 656c 662e 5f5f 6765 745f 7265 7175   self.__get_requ
-0000c300: 6573 7428 7572 6c3d 7572 6c29 0a0a 2020  est(url=url)..  
-0000c310: 2020 2020 2020 7365 6c66 2e5f 5f72 6169        self.__rai
-0000c320: 7365 5f6f 6e5f 6572 726f 7228 7265 7370  se_on_error(resp
-0000c330: 6f6e 7365 290a 0a20 2020 2020 2020 2072  onse)..        r
-0000c340: 6574 7572 6e20 7265 7370 6f6e 7365 0a0a  eturn response..
-0000c350: 2020 2020 6465 6620 5f5f 7574 696c 697a      def __utiliz
-0000c360: 655f 7064 665f 656e 6470 6f69 6e74 2873  e_pdf_endpoint(s
-0000c370: 656c 662c 2073 616d 706c 655f 6861 7368  elf, sample_hash
-0000c380: 2c20 656e 6470 6f69 6e74 293a 0a20 2020  , endpoint):.   
-0000c390: 2020 2020 2022 2222 4163 6365 7074 7320       """Accepts 
-0000c3a0: 6120 7369 6e67 6c65 2068 6173 6820 7374  a single hash st
-0000c3b0: 7269 6e67 2061 6e64 2075 7469 6c69 7a65  ring and utilize
-0000c3c0: 7320 7064 6620 7265 706f 7274 2065 6e64  s pdf report end
-0000c3d0: 706f 696e 7420 666f 7220 696e 6974 6961  point for initia
-0000c3e0: 7469 6f6e 2c20 7374 6174 7573 2063 6865  tion, status che
-0000c3f0: 636b 696e 6720 616e 6420 646f 776e 6c6f  cking and downlo
-0000c400: 6164 696e 670a 2020 2020 2020 2020 6f66  ading.        of
-0000c410: 2061 2050 4446 2061 6e61 6c79 7369 7320   a PDF analysis 
-0000c420: 7265 706f 7274 2066 6f72 2074 6865 2072  report for the r
-0000c430: 6571 7565 7374 6564 2073 616d 706c 652e  equested sample.
-0000c440: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-0000c450: 7261 6d20 7361 6d70 6c65 5f68 6173 683a  ram sample_hash:
-0000c460: 2068 6173 6820 7374 7269 6e67 0a20 2020   hash string.   
-0000c470: 2020 2020 2020 2020 203a 7479 7065 2073           :type s
-0000c480: 616d 706c 655f 6861 7368 3a20 7374 720a  ample_hash: str.
-0000c490: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-0000c4a0: 616d 2065 6e64 706f 696e 743a 2065 6e64  am endpoint: end
-0000c4b0: 706f 696e 7420 7374 7269 6e67 0a20 2020  point string.   
-0000c4c0: 2020 2020 2020 2020 203a 7479 7065 2065           :type e
-0000c4d0: 6e64 706f 696e 743a 2073 7472 0a20 2020  ndpoint: str.   
-0000c4e0: 2020 2020 2020 2020 203a 7265 7475 726e           :return
-0000c4f0: 3a20 7265 7370 6f6e 7365 0a20 2020 2020  : response.     
-0000c500: 2020 2020 2020 203a 7274 7970 653a 2072         :rtype: r
-0000c510: 6571 7565 7374 732e 5265 7370 6f6e 7365  equests.Response
-0000c520: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c530: 2020 2020 2076 616c 6964 6174 655f 6861       validate_ha
-0000c540: 7368 6573 280a 2020 2020 2020 2020 2020  shes(.          
-0000c550: 2020 6861 7368 5f69 6e70 7574 3d5b 7361    hash_input=[sa
-0000c560: 6d70 6c65 5f68 6173 685d 2c0a 2020 2020  mple_hash],.    
-0000c570: 2020 2020 2020 2020 616c 6c6f 7765 645f          allowed_
-0000c580: 6861 7368 5f74 7970 6573 3d28 4d44 352c  hash_types=(MD5,
-0000c590: 2053 4841 312c 2053 4841 3235 3629 0a20   SHA1, SHA256). 
-0000c5a0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000c5b0: 2020 656e 6470 6f69 6e74 203d 2065 6e64    endpoint = end
-0000c5c0: 706f 696e 742e 666f 726d 6174 280a 2020  point.format(.  
-0000c5d0: 2020 2020 2020 2020 2020 6861 7368 5f76            hash_v
-0000c5e0: 616c 7565 3d73 616d 706c 655f 6861 7368  alue=sample_hash
-0000c5f0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000c600: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
-0000c610: 5f75 726c 2e66 6f72 6d61 7428 656e 6470  _url.format(endp
-0000c620: 6f69 6e74 3d65 6e64 706f 696e 7429 0a0a  oint=endpoint)..
-0000c630: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-0000c640: 203d 2073 656c 662e 5f5f 6765 745f 7265   = self.__get_re
-0000c650: 7175 6573 7428 7572 6c3d 7572 6c29 0a0a  quest(url=url)..
-0000c660: 2020 2020 2020 2020 7365 6c66 2e5f 5f72          self.__r
-0000c670: 6169 7365 5f6f 6e5f 6572 726f 7228 7265  aise_on_error(re
-0000c680: 7370 6f6e 7365 290a 0a20 2020 2020 2020  sponse)..       
-0000c690: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-0000c6a0: 0a0a 2020 2020 6465 6620 6372 6561 7465  ..    def create
-0000c6b0: 5f70 6466 5f72 6570 6f72 7428 7365 6c66  _pdf_report(self
-0000c6c0: 2c20 7361 6d70 6c65 5f68 6173 6829 3a0a  , sample_hash):.
-0000c6d0: 2020 2020 2020 2020 2222 2241 6363 6570          """Accep
-0000c6e0: 7473 2061 2073 696e 676c 6520 6861 7368  ts a single hash
-0000c6f0: 2073 7472 696e 6720 616e 6420 696e 6974   string and init
-0000c700: 6961 7465 7320 7468 6520 6372 6561 7469  iates the creati
-0000c710: 6f6e 206f 6620 6120 5044 4620 616e 616c  on of a PDF anal
-0000c720: 7973 6973 2072 6570 6f72 7420 666f 7220  ysis report for 
-0000c730: 7468 6520 7265 7175 6573 7465 6420 7361  the requested sa
-0000c740: 6d70 6c65 2e0a 2020 2020 2020 2020 5468  mple..        Th
-0000c750: 6520 7265 7370 6f6e 7365 2069 6e63 6c75  e response inclu
-0000c760: 6465 7320 6c69 6e6b 7320 746f 2074 6865  des links to the
-0000c770: 2070 6466 2063 7265 6174 696f 6e20 7374   pdf creation st
-0000c780: 6174 7573 2065 6e64 706f 696e 7420 616e  atus endpoint an
-0000c790: 6420 7064 6620 646f 776e 6c6f 6164 2065  d pdf download e
-0000c7a0: 646e 706f 696e 7420 666f 7220 7468 6520  dnpoint for the 
-0000c7b0: 7265 7175 6573 7465 640a 2020 2020 2020  requested.      
-0000c7c0: 2020 7361 6d70 6c65 2e0a 2020 2020 2020    sample..      
-0000c7d0: 2020 2020 2020 3a70 6172 616d 2073 616d        :param sam
-0000c7e0: 706c 655f 6861 7368 3a20 6861 7368 2073  ple_hash: hash s
-0000c7f0: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-0000c800: 2020 3a74 7970 6520 7361 6d70 6c65 5f68    :type sample_h
-0000c810: 6173 683a 2073 7472 0a20 2020 2020 2020  ash: str.       
-0000c820: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
-0000c830: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
-0000c840: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
-0000c850: 7374 732e 5265 7370 6f6e 7365 0a20 2020  sts.Response.   
-0000c860: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c870: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
-0000c880: 2e5f 5f75 7469 6c69 7a65 5f70 6466 5f65  .__utilize_pdf_e
-0000c890: 6e64 706f 696e 7428 7361 6d70 6c65 5f68  ndpoint(sample_h
-0000c8a0: 6173 682c 2073 656c 662e 5f5f 5044 465f  ash, self.__PDF_
-0000c8b0: 5245 504f 5254 5f43 5245 4154 455f 454e  REPORT_CREATE_EN
-0000c8c0: 4450 4f49 4e54 290a 2020 2020 2020 2020  DPOINT).        
-0000c8d0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0000c8e0: 0a20 2020 2064 6566 2063 6865 636b 5f70  .    def check_p
-0000c8f0: 6466 5f72 6570 6f72 745f 6372 6561 7469  df_report_creati
-0000c900: 6f6e 2873 656c 662c 2073 616d 706c 655f  on(self, sample_
-0000c910: 6861 7368 293a 0a20 2020 2020 2020 2022  hash):.        "
-0000c920: 2222 4163 6365 7074 7320 6120 7369 6e67  ""Accepts a sing
-0000c930: 6c65 2068 6173 6820 7374 7269 6e67 2074  le hash string t
-0000c940: 6861 7420 7368 6f75 6c64 2063 6f72 7265  hat should corre
-0000c950: 7370 6f6e 6420 746f 2074 6865 2068 6173  spond to the has
-0000c960: 6820 7573 6564 2069 6e20 7468 6520 7265  h used in the re
-0000c970: 7175 6573 7420 7769 7468 0a20 2020 2020  quest with.     
-0000c980: 2020 2063 7265 6174 655f 7064 665f 7265     create_pdf_re
-0000c990: 706f 7274 206d 6574 686f 642e 2054 6865  port method. The
-0000c9a0: 2072 6573 706f 6e73 6520 696e 636c 7564   response includ
-0000c9b0: 6573 2061 6e20 696e 666f 726d 6174 6976  es an informativ
-0000c9c0: 6520 6d65 7373 6167 6520 6162 6f75 7420  e message about 
-0000c9d0: 7468 6520 7374 6174 7573 206f 6620 7468  the status of th
-0000c9e0: 6520 5044 460a 2020 2020 2020 2020 7265  e PDF.        re
-0000c9f0: 706f 7274 2070 7265 7669 6f75 736c 7920  port previously 
-0000ca00: 7265 7175 6573 7465 642e 0a20 2020 2020  requested..     
-0000ca10: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
-0000ca20: 6d70 6c65 5f68 6173 683a 2068 6173 6820  mple_hash: hash 
-0000ca30: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-0000ca40: 2020 203a 7479 7065 2073 616d 706c 655f     :type sample_
-0000ca50: 6861 7368 3a20 7374 720a 2020 2020 2020  hash: str.      
-0000ca60: 2020 2020 2020 3a72 6574 7572 6e3a 2072        :return: r
-0000ca70: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-0000ca80: 2020 2020 3a72 7479 7065 3a20 7265 7175      :rtype: requ
-0000ca90: 6573 7473 2e52 6573 706f 6e73 650a 2020  ests.Response.  
-0000caa0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000cab0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-0000cac0: 662e 5f5f 7574 696c 697a 655f 7064 665f  f.__utilize_pdf_
-0000cad0: 656e 6470 6f69 6e74 2873 616d 706c 655f  endpoint(sample_
-0000cae0: 6861 7368 2c20 7365 6c66 2e5f 5f50 4446  hash, self.__PDF
-0000caf0: 5f52 4550 4f52 545f 5354 4154 5553 5f45  _REPORT_STATUS_E
-0000cb00: 4e44 504f 494e 5429 0a20 2020 2020 2020  NDPOINT).       
-0000cb10: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-0000cb20: 0a0a 2020 2020 6465 6620 646f 776e 6c6f  ..    def downlo
-0000cb30: 6164 5f70 6466 5f72 6570 6f72 7428 7365  ad_pdf_report(se
-0000cb40: 6c66 2c20 7361 6d70 6c65 5f68 6173 6829  lf, sample_hash)
-0000cb50: 3a0a 2020 2020 2020 2020 2222 2241 6363  :.        """Acc
-0000cb60: 6570 7473 2061 2073 696e 676c 6520 6861  epts a single ha
-0000cb70: 7368 2073 7472 696e 6720 7468 6174 2073  sh string that s
-0000cb80: 686f 756c 6420 636f 7272 6573 706f 6e64  hould correspond
-0000cb90: 2074 6f20 7468 6520 6861 7368 2075 7365   to the hash use
-0000cba0: 6420 696e 2074 6865 2072 6571 7565 7374  d in the request
-0000cbb0: 2077 6974 680a 2020 2020 2020 2020 6372   with.        cr
-0000cbc0: 6561 7465 5f70 6466 5f72 6570 6f72 7420  eate_pdf_report 
-0000cbd0: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
-0000cbe0: 2020 2020 3a70 6172 616d 2073 616d 706c      :param sampl
-0000cbf0: 655f 6861 7368 3a20 6861 7368 2073 7472  e_hash: hash str
-0000cc00: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-0000cc10: 3a74 7970 6520 7361 6d70 6c65 5f68 6173  :type sample_has
-0000cc20: 683a 2073 7472 0a20 2020 2020 2020 2020  h: str.         
-0000cc30: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
-0000cc40: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
-0000cc50: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
-0000cc60: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
-0000cc70: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000cc80: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-0000cc90: 5f75 7469 6c69 7a65 5f70 6466 5f65 6e64  _utilize_pdf_end
-0000cca0: 706f 696e 7428 7361 6d70 6c65 5f68 6173  point(sample_has
-0000ccb0: 682c 2073 656c 662e 5f5f 5044 465f 5245  h, self.__PDF_RE
-0000ccc0: 504f 5254 5f44 4f57 4e4c 4f41 445f 454e  PORT_DOWNLOAD_EN
-0000ccd0: 4450 4f49 4e54 290a 2020 2020 2020 2020  DPOINT).        
-0000cce0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0000ccf0: 0a20 2020 2064 6566 2067 6574 5f74 6974  .    def get_tit
-0000cd00: 616e 6975 6d5f 636f 7265 5f72 6570 6f72  anium_core_repor
-0000cd10: 745f 7632 2873 656c 662c 2073 616d 706c  t_v2(self, sampl
-0000cd20: 655f 6861 7368 2c20 6669 656c 6473 3d4e  e_hash, fields=N
-0000cd30: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-0000cd40: 2241 6363 6570 7473 2061 2073 696e 676c  "Accepts a singl
-0000cd50: 6520 6861 7368 2073 7472 696e 6720 616e  e hash string an
-0000cd60: 6420 6765 7473 2074 6865 2066 756c 6c20  d gets the full 
-0000cd70: 5469 7461 6e69 756d 436f 7265 2073 7461  TitaniumCore sta
-0000cd80: 7469 6320 616e 616c 7973 6973 2072 6570  tic analysis rep
-0000cd90: 6f72 7420 666f 7220 7468 6520 7265 7175  ort for the requ
-0000cda0: 6573 7465 6420 7361 6d70 6c65 2e0a 2020  ested sample..  
-0000cdb0: 2020 2020 2020 5468 6520 7265 7175 6573        The reques
-0000cdc0: 7465 6420 7361 6d70 6c65 206d 7573 7420  ted sample must 
-0000cdd0: 6265 2070 7265 7365 6e74 206f 6e20 7468  be present on th
-0000cde0: 6520 6170 706c 6961 6e63 652e 2049 6620  e appliance. If 
-0000cdf0: 7468 6520 6f70 7469 6f6e 616c 2066 6965  the optional fie
-0000ce00: 6c64 7320 7061 7261 6d65 7465 7220 6973  lds parameter is
-0000ce10: 206e 6f74 2070 726f 7669 6465 6420 696e   not provided in
-0000ce20: 2074 6865 0a20 2020 2020 2020 2072 6571   the.        req
-0000ce30: 7565 7374 2c20 616c 6c20 6176 6169 6c61  uest, all availa
-0000ce40: 626c 6520 7061 7274 7320 6f66 2074 6865  ble parts of the
-0000ce50: 2073 7461 7469 6320 616e 616c 7973 6973   static analysis
-0000ce60: 2072 6570 6f72 7420 6172 6520 7265 7475   report are retu
-0000ce70: 726e 6564 2069 6e20 7468 6520 7265 7370  rned in the resp
-0000ce80: 6f6e 7365 2e0a 2020 2020 2020 2020 2020  onse..          
-0000ce90: 2020 3a70 6172 616d 2073 616d 706c 655f    :param sample_
-0000cea0: 6861 7368 3a20 6861 7368 2073 7472 696e  hash: hash strin
-0000ceb0: 670a 2020 2020 2020 2020 2020 2020 3a74  g.            :t
-0000cec0: 7970 6520 7361 6d70 6c65 5f68 6173 683a  ype sample_hash:
-0000ced0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
-0000cee0: 203a 7061 7261 6d20 6669 656c 6473 3a20   :param fields: 
-0000cef0: 6120 7374 7269 6e67 206f 6620 636f 6d6d  a string of comm
-0000cf00: 6120 7365 7061 7261 7465 6420 5469 7461  a separated Tita
-0000cf10: 6e69 756d 436f 7265 2027 6669 656c 6473  niumCore 'fields
-0000cf20: 2720 746f 2071 7565 7279 0a20 2020 2020  ' to query.     
-0000cf30: 2020 2020 2020 203a 7479 7065 2066 6965         :type fie
-0000cf40: 6c64 733a 2073 7472 0a20 2020 2020 2020  lds: str.       
-0000cf50: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
-0000cf60: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
-0000cf70: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
-0000cf80: 7374 732e 5265 7370 6f6e 7365 0a20 2020  sts.Response.   
-0000cf90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000cfa0: 2076 616c 6964 6174 655f 6861 7368 6573   validate_hashes
-0000cfb0: 280a 2020 2020 2020 2020 2020 2020 6861  (.            ha
-0000cfc0: 7368 5f69 6e70 7574 3d5b 7361 6d70 6c65  sh_input=[sample
-0000cfd0: 5f68 6173 685d 2c0a 2020 2020 2020 2020  _hash],.        
-0000cfe0: 2020 2020 616c 6c6f 7765 645f 6861 7368      allowed_hash
-0000cff0: 5f74 7970 6573 3d28 4d44 352c 2053 4841  _types=(MD5, SHA
-0000d000: 312c 2053 4841 3235 362c 2053 4841 3531  1, SHA256, SHA51
-0000d010: 3229 0a20 2020 2020 2020 2029 0a0a 2020  2).        )..  
-0000d020: 2020 2020 2020 6966 2066 6965 6c64 7320        if fields 
-0000d030: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
-0000d040: 6365 2866 6965 6c64 732c 2073 7472 293a  ce(fields, str):
-0000d050: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000d060: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-0000d070: 6f72 2822 6669 656c 6473 2070 6172 616d  or("fields param
-0000d080: 6574 6572 206d 7573 7420 6265 2061 2073  eter must be a s
-0000d090: 7472 696e 672e 2229 0a0a 2020 2020 2020  tring.")..      
-0000d0a0: 2020 6966 2066 6965 6c64 7320 6973 204e    if fields is N
-0000d0b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000d0c0: 2066 6965 6c64 7320 3d20 7365 6c66 2e5f   fields = self._
-0000d0d0: 7469 636f 7265 5f66 6965 6c64 730a 0a20  ticore_fields.. 
-0000d0e0: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
-0000d0f0: 3d20 7365 6c66 2e5f 5f54 4954 414e 4955  = self.__TITANIU
-0000d100: 4d5f 434f 5245 5f52 4550 4f52 545f 454e  M_CORE_REPORT_EN
-0000d110: 4450 4f49 4e54 5f56 322e 666f 726d 6174  DPOINT_V2.format
-0000d120: 280a 2020 2020 2020 2020 2020 2020 6861  (.            ha
-0000d130: 7368 5f76 616c 7565 3d73 616d 706c 655f  sh_value=sample_
-0000d140: 6861 7368 2c0a 2020 2020 2020 2020 2020  hash,.          
-0000d150: 2020 6669 656c 6473 3d66 6965 6c64 730a    fields=fields.
-0000d160: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000d170: 2020 2075 726c 203d 2073 656c 662e 5f75     url = self._u
-0000d180: 726c 2e66 6f72 6d61 7428 656e 6470 6f69  rl.format(endpoi
-0000d190: 6e74 3d65 6e64 706f 696e 7429 0a0a 2020  nt=endpoint)..  
-0000d1a0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0000d1b0: 2073 656c 662e 5f5f 6765 745f 7265 7175   self.__get_requ
-0000d1c0: 6573 7428 7572 6c3d 7572 6c29 0a0a 2020  est(url=url)..  
-0000d1d0: 2020 2020 2020 7365 6c66 2e5f 5f72 6169        self.__rai
-0000d1e0: 7365 5f6f 6e5f 6572 726f 7228 7265 7370  se_on_error(resp
-0000d1f0: 6f6e 7365 290a 0a20 2020 2020 2020 2072  onse)..        r
-0000d200: 6574 7572 6e20 7265 7370 6f6e 7365 0a0a  eturn response..
-0000d210: 2020 2020 6465 6620 5f5f 7574 696c 697a      def __utiliz
-0000d220: 655f 6479 6e61 6d69 635f 616e 616c 7973  e_dynamic_analys
-0000d230: 6973 5f65 6e64 706f 696e 7428 7365 6c66  is_endpoint(self
-0000d240: 2c20 7361 6d70 6c65 5f68 6173 682c 2072  , sample_hash, r
-0000d250: 6570 6f72 745f 666f 726d 6174 2c20 656e  eport_format, en
-0000d260: 6470 6f69 6e74 293a 0a20 2020 2020 2020  dpoint):.       
-0000d270: 2022 2222 4163 6365 7074 7320 656e 6470   """Accepts endp
-0000d280: 6f69 6e74 2c20 6120 7369 6e67 6c65 2068  oint, a single h
-0000d290: 6173 6820 7374 7269 6e67 2061 6e64 2061  ash string and a
-0000d2a0: 2072 6570 6f72 7420 666f 726d 6174 2061   report format a
-0000d2b0: 6e64 2075 7469 6c69 7a65 7320 6479 6e61  nd utilizes dyna
-0000d2c0: 6d69 6320 616e 616c 7973 6973 2065 6e64  mic analysis end
-0000d2d0: 706f 696e 7420 666f 720a 2020 2020 2020  point for.      
-0000d2e0: 2020 696e 6974 6961 7469 6f6e 2c20 7374    initiation, st
-0000d2f0: 6174 7573 2063 6865 636b 696e 6720 616e  atus checking an
-0000d300: 6420 646f 776e 6c6f 6164 696e 6720 6f66  d downloading of
-0000d310: 2050 4446 206f 7220 4854 4d4c 2072 6570   PDF or HTML rep
-0000d320: 6f72 7473 0a20 2020 2020 2020 2066 6f72  orts.        for
-0000d330: 2073 616d 706c 6573 2074 6861 7420 6861   samples that ha
-0000d340: 7665 2067 6f6e 6520 7468 726f 7567 6820  ve gone through 
-0000d350: 6479 6e61 6d69 6320 616e 616c 7973 6973  dynamic analysis
-0000d360: 2069 6e20 7468 6520 5265 7665 7273 696e   in the Reversin
-0000d370: 674c 6162 7320 436c 6f75 6420 5361 6e64  gLabs Cloud Sand
-0000d380: 626f 782e 0a20 2020 2020 2020 2020 2020  box..           
-0000d390: 203a 7061 7261 6d20 7361 6d70 6c65 5f68   :param sample_h
-0000d3a0: 6173 683a 2068 6173 6820 7374 7269 6e67  ash: hash string
-0000d3b0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-0000d3c0: 7065 2073 616d 706c 655f 6861 7368 3a20  pe sample_hash: 
-0000d3d0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-0000d3e0: 3a70 6172 616d 2072 6570 6f72 745f 666f  :param report_fo
-0000d3f0: 726d 6174 3a20 7265 706f 7274 2066 6f72  rmat: report for
-0000d400: 6d61 7420 2827 6874 6d6c 2720 6f72 2027  mat ('html' or '
-0000d410: 7064 6627 290a 2020 2020 2020 2020 2020  pdf').          
-0000d420: 2020 3a72 7479 7065 2072 6570 6f72 745f    :rtype report_
-0000d430: 666f 726d 6174 3a20 7374 720a 2020 2020  format: str.    
-0000d440: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
-0000d450: 6e64 706f 696e 743a 2065 6e64 706f 696e  ndpoint: endpoin
-0000d460: 7420 7374 7269 6e67 0a20 2020 2020 2020  t string.       
-0000d470: 2020 2020 203a 7479 7065 2065 6e64 706f       :type endpo
-0000d480: 696e 743a 2073 7472 0a20 2020 2020 2020  int: str.       
-0000d490: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
-0000d4a0: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
-0000d4b0: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
-0000d4c0: 7374 732e 5265 7370 6f6e 7365 0a20 2020  sts.Response.   
-0000d4d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000d4e0: 2076 616c 6964 6174 655f 6861 7368 6573   validate_hashes
-0000d4f0: 280a 2020 2020 2020 2020 2020 2020 6861  (.            ha
-0000d500: 7368 5f69 6e70 7574 3d5b 7361 6d70 6c65  sh_input=[sample
-0000d510: 5f68 6173 685d 2c0a 2020 2020 2020 2020  _hash],.        
-0000d520: 2020 2020 616c 6c6f 7765 645f 6861 7368      allowed_hash
-0000d530: 5f74 7970 6573 3d28 5348 4131 2c29 0a20  _types=(SHA1,). 
-0000d540: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000d550: 2020 6966 2072 6570 6f72 745f 666f 726d    if report_form
-0000d560: 6174 206e 6f74 2069 6e20 2822 6874 6d6c  at not in ("html
-0000d570: 222c 2022 7064 6622 293a 0a20 2020 2020  ", "pdf"):.     
-0000d580: 2020 2020 2020 2072 6169 7365 2057 726f         raise Wro
-0000d590: 6e67 496e 7075 7445 7272 6f72 2822 7265  ngInputError("re
-0000d5a0: 706f 7274 5f66 6f72 6d61 7420 7061 7261  port_format para
-0000d5b0: 6d65 7465 7220 6d75 7374 2062 6520 6569  meter must be ei
-0000d5c0: 7468 6572 2027 6874 6d6c 2720 6f72 2027  ther 'html' or '
-0000d5d0: 7064 6627 2e22 290a 0a20 2020 2020 2020  pdf'.")..       
-0000d5e0: 2065 6e64 706f 696e 7420 3d20 656e 6470   endpoint = endp
-0000d5f0: 6f69 6e74 2e66 6f72 6d61 7428 0a20 2020  oint.format(.   
-0000d600: 2020 2020 2020 2020 2068 6173 685f 7661           hash_va
-0000d610: 6c75 653d 7361 6d70 6c65 5f68 6173 682c  lue=sample_hash,
-0000d620: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000d630: 6d61 743d 7265 706f 7274 5f66 6f72 6d61  mat=report_forma
-0000d640: 742c 0a20 2020 2020 2020 2029 0a0a 2020  t,.        )..  
-0000d650: 2020 2020 2020 7572 6c20 3d20 7365 6c66        url = self
-0000d660: 2e5f 7572 6c2e 666f 726d 6174 2865 6e64  ._url.format(end
-0000d670: 706f 696e 743d 656e 6470 6f69 6e74 290a  point=endpoint).
-0000d680: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-0000d690: 6520 3d20 7365 6c66 2e5f 5f67 6574 5f72  e = self.__get_r
-0000d6a0: 6571 7565 7374 2875 726c 3d75 726c 290a  equest(url=url).
-0000d6b0: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
-0000d6c0: 7261 6973 655f 6f6e 5f65 7272 6f72 2872  raise_on_error(r
-0000d6d0: 6573 706f 6e73 6529 0a0a 2020 2020 2020  esponse)..      
-0000d6e0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-0000d6f0: 650a 0a20 2020 2064 6566 2063 7265 6174  e..    def creat
-0000d700: 655f 6479 6e61 6d69 635f 616e 616c 7973  e_dynamic_analys
-0000d710: 6973 5f72 6570 6f72 7428 7365 6c66 2c20  is_report(self, 
-0000d720: 7361 6d70 6c65 5f68 6173 682c 2072 6570  sample_hash, rep
-0000d730: 6f72 745f 666f 726d 6174 293a 0a20 2020  ort_format):.   
-0000d740: 2020 2020 2022 2222 4163 6365 7074 7320       """Accepts 
-0000d750: 6120 7369 6e67 6c65 2068 6173 6820 7374  a single hash st
-0000d760: 7269 6e67 2061 6e64 2061 2072 6570 6f72  ring and a repor
-0000d770: 7420 666f 726d 6174 2061 6e64 2069 6e69  t format and ini
-0000d780: 7469 6174 6573 2074 6865 2063 7265 6174  tiates the creat
-0000d790: 696f 6e20 6f66 2050 4446 206f 7220 4854  ion of PDF or HT
-0000d7a0: 4d4c 2072 6570 6f72 7473 2066 6f72 0a20  ML reports for. 
-0000d7b0: 2020 2020 2020 2073 616d 706c 6573 2074         samples t
-0000d7c0: 6861 7420 6861 7665 2067 6f6e 6520 7468  hat have gone th
-0000d7d0: 726f 7567 6820 6479 6e61 6d69 6320 616e  rough dynamic an
-0000d7e0: 616c 7973 6973 2069 6e20 7468 6520 5265  alysis in the Re
-0000d7f0: 7665 7273 696e 674c 6162 7320 436c 6f75  versingLabs Clou
-0000d800: 6420 5361 6e64 626f 782e 0a20 2020 2020  d Sandbox..     
-0000d810: 2020 2054 6865 2072 6573 706f 6e73 6520     The response 
-0000d820: 696e 636c 7564 6573 206c 696e 6b73 2074  includes links t
-0000d830: 6f20 7468 6520 7265 706f 7274 2063 7265  o the report cre
-0000d840: 6174 696f 6e20 7374 6174 7573 2065 6e64  ation status end
-0000d850: 706f 696e 7420 616e 6420 7265 706f 7274  point and report
-0000d860: 2064 6f77 6e6c 6f61 6420 656e 6470 6f69   download endpoi
-0000d870: 6e74 2066 6f72 2074 6865 0a20 2020 2020  nt for the.     
-0000d880: 2020 2072 6571 7565 7374 6564 2073 616d     requested sam
-0000d890: 706c 652e 0a20 2020 2020 2020 2020 2020  ple..           
-0000d8a0: 203a 7061 7261 6d20 7361 6d70 6c65 5f68   :param sample_h
-0000d8b0: 6173 683a 2068 6173 6820 7374 7269 6e67  ash: hash string
-0000d8c0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-0000d8d0: 7065 2073 616d 706c 655f 6861 7368 3a20  pe sample_hash: 
-0000d8e0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-0000d8f0: 3a70 6172 616d 2072 6570 6f72 745f 666f  :param report_fo
-0000d900: 726d 6174 3a20 7265 706f 7274 2066 6f72  rmat: report for
-0000d910: 6d61 7420 2827 6874 6d6c 2720 6f72 2027  mat ('html' or '
-0000d920: 7064 6627 290a 2020 2020 2020 2020 2020  pdf').          
-0000d930: 2020 3a72 7479 7065 2072 6570 6f72 745f    :rtype report_
-0000d940: 666f 726d 6174 3a20 7374 720a 2020 2020  format: str.    
-0000d950: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-0000d960: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
-0000d970: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
-0000d980: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
-0000d990: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d9a0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-0000d9b0: 656c 662e 5f5f 7574 696c 697a 655f 6479  elf.__utilize_dy
-0000d9c0: 6e61 6d69 635f 616e 616c 7973 6973 5f65  namic_analysis_e
-0000d9d0: 6e64 706f 696e 7428 7361 6d70 6c65 5f68  ndpoint(sample_h
-0000d9e0: 6173 682c 0a20 2020 2020 2020 2020 2020  ash,.           
-0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da20: 2072 6570 6f72 745f 666f 726d 6174 2c0a   report_format,.
+000043c0: 2020 2020 2020 2020 2020 6172 6368 6976            archiv
+000043d0: 655f 7061 7373 776f 7264 3d61 7263 6869  e_password=archi
+000043e0: 7665 5f70 6173 7377 6f72 642c 0a20 2020  ve_password,.   
+000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004420: 2020 2072 6c5f 636c 6f75 645f 7361 6e64     rl_cloud_sand
+00004430: 626f 785f 706c 6174 666f 726d 3d72 6c5f  box_platform=rl_
+00004440: 636c 6f75 645f 7361 6e64 626f 785f 706c  cloud_sandbox_pl
+00004450: 6174 666f 726d 290a 0a20 2020 2020 2020  atform)..       
+00004460: 2072 6573 706f 6e73 655f 6465 7461 696c   response_detail
+00004470: 203d 2075 706c 6f61 645f 7265 7370 6f6e   = upload_respon
+00004480: 7365 2e6a 736f 6e28 292e 6765 7428 2264  se.json().get("d
+00004490: 6574 6169 6c22 290a 2020 2020 2020 2020  etail").        
+000044a0: 7461 736b 5f69 6420 3d20 7265 7370 6f6e  task_id = respon
+000044b0: 7365 5f64 6574 6169 6c2e 6765 7428 2269  se_detail.get("i
+000044c0: 6422 290a 2020 2020 2020 2020 7461 736b  d").        task
+000044d0: 5f69 6420 3d20 7374 7228 7461 736b 5f69  _id = str(task_i
+000044e0: 6429 0a0a 2020 2020 2020 2020 7265 7370  d)..        resp
+000044f0: 6f6e 7365 203d 2073 656c 662e 6765 745f  onse = self.get_
+00004500: 7375 626d 6974 7465 645f 7572 6c5f 7265  submitted_url_re
+00004510: 706f 7274 2874 6173 6b5f 6964 3d74 6173  port(task_id=tas
+00004520: 6b5f 6964 2c20 7265 7472 793d 7265 7472  k_id, retry=retr
+00004530: 7929 0a0a 2020 2020 2020 2020 7265 7475  y)..        retu
+00004540: 726e 2072 6573 706f 6e73 650a 0a20 2020  rn response..   
+00004550: 2064 6566 2067 6574 5f72 6573 756c 7473   def get_results
+00004560: 2873 656c 662c 2073 616d 706c 655f 6861  (self, sample_ha
+00004570: 7368 6573 2c20 7265 7472 793d 5472 7565  shes, retry=True
+00004580: 2c20 6669 656c 6473 3d4e 6f6e 6529 3a0a  , fields=None):.
+00004590: 2020 2020 2020 2020 2222 2254 4849 5320          """THIS 
+000045a0: 4d45 5448 4f44 2049 5320 4445 5052 4543  METHOD IS DEPREC
+000045b0: 4154 4544 2e0a 2020 2020 2020 2020 5573  ATED..        Us
+000045c0: 6520 6765 745f 7375 6d6d 6172 795f 7265  e get_summary_re
+000045d0: 706f 7274 5f76 3220 666f 7220 6120 7375  port_v2 for a su
+000045e0: 6d6d 6172 7920 616e 616c 7973 6973 2072  mmary analysis r
+000045f0: 6570 6f72 7420 6f72 0a20 2020 2020 2020  eport or.       
+00004600: 2067 6574 5f64 6574 6169 6c65 645f 7265   get_detailed_re
+00004610: 706f 7274 5f76 3220 666f 7220 6120 6465  port_v2 for a de
+00004620: 7461 696c 6564 2061 6e61 6c79 7369 7320  tailed analysis 
+00004630: 7265 706f 7274 2e0a 0a20 2020 2020 2020  report...       
+00004640: 2041 6363 6570 7473 2061 206c 6973 7420   Accepts a list 
+00004650: 6f66 2068 6173 6865 7320 616e 6420 7265  of hashes and re
+00004660: 7475 726e 7320 4a53 4f4e 2063 6f6e 7461  turns JSON conta
+00004670: 696e 696e 6720 6120 7375 6d6d 6172 7920  ining a summary 
+00004680: 7265 706f 7274 2066 6f72 2065 6163 6820  report for each 
+00004690: 6f66 2074 6865 6d2e 0a20 2020 2020 2020  of them..       
+000046a0: 2054 6869 7320 6d65 7468 6f64 2075 7469   This method uti
+000046b0: 6c69 7a65 7320 7468 6520 7365 7420 6e75  lizes the set nu
+000046c0: 6d62 6572 206f 6620 7265 7472 6965 7320  mber of retries 
+000046d0: 616e 6420 7761 6974 2074 696d 6520 696e  and wait time in
+000046e0: 2073 6563 6f6e 6473 2074 6f20 7469 6d65   seconds to time
+000046f0: 0a20 2020 2020 2020 206f 7574 2069 6620  .        out if 
+00004700: 7468 6520 616e 616c 7973 6973 2072 6573  the analysis res
+00004710: 756c 7473 2061 7265 206e 6f74 2072 6561  ults are not rea
+00004720: 6479 2e0a 2020 2020 2020 2020 2020 2020  dy..            
+00004730: 3a70 6172 616d 2073 616d 706c 655f 6861  :param sample_ha
+00004740: 7368 6573 3a20 6861 7368 2073 7472 696e  shes: hash strin
+00004750: 6720 6f72 206c 6973 7420 6f66 2068 6173  g or list of has
+00004760: 6820 7374 7269 6e67 730a 2020 2020 2020  h strings.      
+00004770: 2020 2020 2020 3a74 7970 6520 7361 6d70        :type samp
+00004780: 6c65 5f68 6173 6865 733a 2073 7472 206f  le_hashes: str o
+00004790: 7220 6c69 7374 5b73 7472 5d0a 2020 2020  r list[str].    
+000047a0: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
+000047b0: 6574 7279 3a20 6966 2073 6574 2074 6f20  etry: if set to 
+000047c0: 4661 6c73 6520 7468 6572 6520 7769 6c6c  False there will
+000047d0: 206f 6e6c 7920 6265 206f 6e65 2074 7279   only be one try
+000047e0: 2061 7420 6f62 7461 696e 696e 6720 7468   at obtaining th
+000047f0: 6520 616e 616c 7973 6973 2072 6570 6f72  e analysis repor
+00004800: 740a 2020 2020 2020 2020 2020 2020 3a74  t.            :t
+00004810: 7970 6520 7265 7472 793a 2062 6f6f 6c0a  ype retry: bool.
+00004820: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00004830: 616d 2066 6965 6c64 733a 206c 6973 7420  am fields: list 
+00004840: 6f66 2041 3130 3030 2072 6570 6f72 7420  of A1000 report 
+00004850: 2766 6965 6c64 7327 2074 6f20 7175 6572  'fields' to quer
+00004860: 790a 2020 2020 2020 2020 2020 2020 3a74  y.            :t
+00004870: 7970 6520 6669 656c 6473 3a20 6c69 7374  ype fields: list
+00004880: 5b73 7472 5d0a 2020 2020 2020 2020 2020  [str].          
+00004890: 2020 3a72 6574 7572 6e3a 203a 636c 6173    :return: :clas
+000048a0: 733a 6052 6573 706f 6e73 6520 3c52 6573  s:`Response <Res
+000048b0: 706f 6e73 653e 6020 6f62 6a65 6374 0a20  ponse>` object. 
+000048c0: 2020 2020 2020 2020 2020 203a 7274 7970             :rtyp
+000048d0: 653a 2072 6571 7565 7374 732e 5265 7370  e: requests.Resp
+000048e0: 6f6e 7365 0a20 2020 2020 2020 2022 2222  onse.        """
+000048f0: 0a20 2020 2020 2020 2077 6172 6e28 2254  .        warn("T
+00004900: 6869 7320 6d65 7468 6f64 2069 7320 6465  his method is de
+00004910: 7072 6563 6174 6564 2e20 5573 6520 6765  precated. Use ge
+00004920: 745f 7375 6d6d 6172 795f 7265 706f 7274  t_summary_report
+00004930: 5f76 3220 666f 7220 6120 7375 6d6d 6172  _v2 for a summar
+00004940: 7920 616e 616c 7973 6973 2072 6570 6f72  y analysis repor
+00004950: 7420 6f72 2022 0a20 2020 2020 2020 2020  t or ".         
+00004960: 2020 2020 2267 6574 5f64 6574 6169 6c65      "get_detaile
+00004970: 645f 7265 706f 7274 5f76 3220 666f 7220  d_report_v2 for 
+00004980: 6120 6465 7461 696c 6564 2061 6e61 6c79  a detailed analy
+00004990: 7369 7320 7265 706f 7274 222c 2044 6570  sis report", Dep
+000049a0: 7265 6361 7469 6f6e 5761 726e 696e 6729  recationWarning)
+000049b0: 0a0a 2020 2020 2020 2020 6966 2066 6965  ..        if fie
+000049c0: 6c64 7320 616e 6420 6e6f 7420 6973 696e  lds and not isin
+000049d0: 7374 616e 6365 2866 6965 6c64 732c 206c  stance(fields, l
+000049e0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
+000049f0: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+00004a00: 7574 4572 726f 7228 2266 6965 6c64 7320  utError("fields 
+00004a10: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
+00004a20: 6520 6120 6c69 7374 206f 6620 7374 7269  e a list of stri
+00004a30: 6e67 732e 2229 0a0a 2020 2020 2020 2020  ngs.")..        
+00004a40: 6966 206e 6f74 2066 6965 6c64 733a 0a20  if not fields:. 
+00004a50: 2020 2020 2020 2020 2020 2066 6965 6c64             field
+00004a60: 7320 3d20 7365 6c66 2e5f 6669 656c 6473  s = self._fields
+00004a70: 0a0a 2020 2020 2020 2020 6966 2072 6574  ..        if ret
+00004a80: 7279 206e 6f74 2069 6e20 2854 7275 652c  ry not in (True,
+00004a90: 2046 616c 7365 293a 0a20 2020 2020 2020   False):.       
+00004aa0: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
+00004ab0: 496e 7075 7445 7272 6f72 2822 7265 7472  InputError("retr
+00004ac0: 7920 7061 7261 6d65 7465 7220 6d75 7374  y parameter must
+00004ad0: 2062 6520 626f 6f6c 6561 6e2e 2229 0a0a   be boolean.")..
+00004ae0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00004af0: 7461 6e63 6528 7361 6d70 6c65 5f68 6173  tance(sample_has
+00004b00: 6865 732c 2073 7472 293a 0a20 2020 2020  hes, str):.     
+00004b10: 2020 2020 2020 2073 616d 706c 655f 6861         sample_ha
+00004b20: 7368 6573 203d 205b 7361 6d70 6c65 5f68  shes = [sample_h
+00004b30: 6173 6865 735d 0a0a 2020 2020 2020 2020  ashes]..        
+00004b40: 7661 6c69 6461 7465 5f68 6173 6865 7328  validate_hashes(
+00004b50: 0a20 2020 2020 2020 2020 2020 2068 6173  .            has
+00004b60: 685f 696e 7075 743d 7361 6d70 6c65 5f68  h_input=sample_h
+00004b70: 6173 6865 732c 0a20 2020 2020 2020 2020  ashes,.         
+00004b80: 2020 2061 6c6c 6f77 6564 5f68 6173 685f     allowed_hash_
+00004b90: 7479 7065 733d 284d 4435 2c20 5348 4131  types=(MD5, SHA1
+00004ba0: 2c20 5348 4132 3536 2c20 5348 4135 3132  , SHA256, SHA512
+00004bb0: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+00004bc0: 2020 2020 2072 6574 7269 6573 203d 2073       retries = s
+00004bd0: 656c 662e 5f72 6574 7269 6573 2069 6620  elf._retries if 
+00004be0: 7265 7472 7920 656c 7365 2030 0a0a 2020  retry else 0..  
+00004bf0: 2020 2020 2020 616e 616c 7973 6973 5f69        analysis_i
+00004c00: 735f 6669 6e69 7368 6564 203d 2046 616c  s_finished = Fal
+00004c10: 7365 0a0a 2020 2020 2020 2020 666f 7220  se..        for 
+00004c20: 6974 6572 6174 696f 6e20 696e 2072 616e  iteration in ran
+00004c30: 6765 2872 6574 7269 6573 202b 2031 293a  ge(retries + 1):
+00004c40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004c50: 6974 6572 6174 696f 6e3a 0a20 2020 2020  iteration:.     
+00004c60: 2020 2020 2020 2020 2020 2074 696d 652e             time.
+00004c70: 736c 6565 7028 7365 6c66 2e5f 7761 6974  sleep(self._wait
+00004c80: 5f74 696d 655f 7365 636f 6e64 7329 0a0a  _time_seconds)..
+00004c90: 2020 2020 2020 2020 2020 2020 616e 616c              anal
+00004ca0: 7973 6973 5f69 735f 6669 6e69 7368 6564  ysis_is_finished
+00004cb0: 203d 2073 656c 662e 5f5f 616e 616c 7973   = self.__analys
+00004cc0: 6973 5f69 735f 6669 6e69 7368 6564 2873  is_is_finished(s
+00004cd0: 616d 706c 655f 6861 7368 6573 290a 2020  ample_hashes).  
+00004ce0: 2020 2020 2020 2020 2020 6966 2061 6e61            if ana
+00004cf0: 6c79 7369 735f 6973 5f66 696e 6973 6865  lysis_is_finishe
+00004d00: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+00004d10: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
+00004d20: 2020 6966 206e 6f74 2061 6e61 6c79 7369    if not analysi
+00004d30: 735f 6973 5f66 696e 6973 6865 643a 0a20  s_is_finished:. 
+00004d40: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00004d50: 2052 6571 7565 7374 5469 6d65 6f75 7445   RequestTimeoutE
+00004d60: 7272 6f72 2822 5265 706f 7274 2066 6574  rror("Report fet
+00004d70: 6368 696e 6720 6174 7465 6d70 7473 2066  ching attempts f
+00004d80: 696e 6973 6865 6420 2d20 5468 6520 616e  inished - The an
+00004d90: 616c 7973 6973 2072 6570 6f72 7420 6973  alysis report is
+00004da0: 2073 7469 6c6c 206e 6f74 2072 6561 6479   still not ready
+00004db0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dd0: 2020 2020 2020 2020 2022 6f72 2074 6865           "or the
+00004de0: 2073 616d 706c 6520 646f 6573 206e 6f74   sample does not
+00004df0: 2065 7869 7374 206f 6e20 7468 6520 6170   exist on the ap
+00004e00: 706c 6961 6e63 652e 2229 0a0a 2020 2020  pliance.")..    
+00004e10: 2020 2020 7572 6c20 3d20 7365 6c66 2e5f      url = self._
+00004e20: 7572 6c2e 666f 726d 6174 2865 6e64 706f  url.format(endpo
+00004e30: 696e 743d 7365 6c66 2e5f 5f52 4553 554c  int=self.__RESUL
+00004e40: 5453 5f45 4e44 504f 494e 5429 0a0a 2020  TS_ENDPOINT)..  
+00004e50: 2020 2020 2020 6461 7461 203d 207b 0a20        data = {. 
+00004e60: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
+00004e70: 5f76 616c 7565 7322 3a20 7361 6d70 6c65  _values": sample
+00004e80: 5f68 6173 6865 732c 0a20 2020 2020 2020  _hashes,.       
+00004e90: 2020 2020 2022 6669 656c 6473 223a 2066       "fields": f
+00004ea0: 6965 6c64 730a 2020 2020 2020 2020 7d0a  ields.        }.
+00004eb0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00004ec0: 6520 3d20 7365 6c66 2e5f 5f70 6f73 745f  e = self.__post_
+00004ed0: 7265 7175 6573 7428 7572 6c3d 7572 6c2c  request(url=url,
+00004ee0: 2064 6174 613d 6461 7461 290a 0a20 2020   data=data)..   
+00004ef0: 2020 2020 2073 656c 662e 5f5f 7261 6973       self.__rais
+00004f00: 655f 6f6e 5f65 7272 6f72 2872 6573 706f  e_on_error(respo
+00004f10: 6e73 6529 0a0a 2020 2020 2020 2020 7265  nse)..        re
+00004f20: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+00004f30: 2020 2064 6566 2067 6574 5f73 756d 6d61     def get_summa
+00004f40: 7279 5f72 6570 6f72 745f 7632 2873 656c  ry_report_v2(sel
+00004f50: 662c 2073 616d 706c 655f 6861 7368 6573  f, sample_hashes
+00004f60: 2c20 7265 7472 793d 5472 7565 2c20 6669  , retry=True, fi
+00004f70: 656c 6473 3d4e 6f6e 652c 2069 6e63 6c75  elds=None, inclu
+00004f80: 6465 5f6e 6574 776f 726b 7468 7265 6174  de_networkthreat
+00004f90: 696e 7465 6c6c 6967 656e 6365 3d54 7275  intelligence=Tru
+00004fa0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fc0: 2073 6b69 705f 7265 616e 616c 7973 6973   skip_reanalysis
+00004fd0: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
+00004fe0: 2022 2222 4163 6365 7074 7320 6120 7369   """Accepts a si
+00004ff0: 6e67 6c65 2068 6173 6820 6f72 2061 206c  ngle hash or a l
+00005000: 6973 7420 6f66 2068 6173 6865 7320 616e  ist of hashes an
+00005010: 6420 7265 7475 726e 7320 4a53 4f4e 2063  d returns JSON c
+00005020: 6f6e 7461 696e 696e 6720 6120 7375 6d6d  ontaining a summ
+00005030: 6172 7920 7265 706f 7274 2066 6f72 2065  ary report for e
+00005040: 6163 6820 6f66 2074 6865 6d2e 0a20 2020  ach of them..   
+00005050: 2020 2020 2054 6869 7320 6d65 7468 6f64       This method
+00005060: 2075 7469 6c69 7a65 7320 7468 6520 7365   utilizes the se
+00005070: 7420 6e75 6d62 6572 206f 6620 7265 7472  t number of retr
+00005080: 6965 7320 616e 6420 7761 6974 2074 696d  ies and wait tim
+00005090: 6520 696e 2073 6563 6f6e 6473 2074 6f20  e in seconds to 
+000050a0: 7469 6d65 0a20 2020 2020 2020 206f 7574  time.        out
+000050b0: 2069 6620 7468 6520 616e 616c 7973 6973   if the analysis
+000050c0: 2072 6573 756c 7473 2061 7265 206e 6f74   results are not
+000050d0: 2072 6561 6479 2e0a 2020 2020 2020 2020   ready..        
+000050e0: 2020 2020 3a70 6172 616d 2073 616d 706c      :param sampl
+000050f0: 655f 6861 7368 6573 3a20 6861 7368 2073  e_hashes: hash s
+00005100: 7472 696e 6720 6f72 206c 6973 7420 6f66  tring or list of
+00005110: 2068 6173 6820 7374 7269 6e67 730a 2020   hash strings.  
+00005120: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00005130: 7361 6d70 6c65 5f68 6173 6865 733a 2073  sample_hashes: s
+00005140: 7472 206f 7220 6c69 7374 5b73 7472 5d0a  tr or list[str].
+00005150: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00005160: 616d 2072 6574 7279 3a20 6966 2073 6574  am retry: if set
+00005170: 2074 6f20 4661 6c73 6520 7468 6572 6520   to False there 
+00005180: 7769 6c6c 206f 6e6c 7920 6265 206f 6e65  will only be one
+00005190: 2074 7279 2061 7420 6f62 7461 696e 696e   try at obtainin
+000051a0: 6720 7468 6520 616e 616c 7973 6973 2072  g the analysis r
+000051b0: 6570 6f72 740a 2020 2020 2020 2020 2020  eport.          
+000051c0: 2020 3a74 7970 6520 7265 7472 793a 2062    :type retry: b
+000051d0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+000051e0: 3a70 6172 616d 2066 6965 6c64 733a 206c  :param fields: l
+000051f0: 6973 7420 6f66 2041 3130 3030 2072 6570  ist of A1000 rep
+00005200: 6f72 7420 2766 6965 6c64 7327 2074 6f20  ort 'fields' to 
+00005210: 7175 6572 790a 2020 2020 2020 2020 2020  query.          
+00005220: 2020 3a74 7970 6520 6669 656c 6473 3a20    :type fields: 
+00005230: 6c69 7374 5b73 7472 5d0a 2020 2020 2020  list[str].      
+00005240: 2020 2020 2020 3a70 6172 616d 2069 6e63        :param inc
+00005250: 6c75 6465 5f6e 6574 776f 726b 7468 7265  lude_networkthre
+00005260: 6174 696e 7465 6c6c 6967 656e 6365 3a20  atintelligence: 
+00005270: 696e 636c 7564 6520 6e65 7477 6f72 6b20  include network 
+00005280: 7468 7265 6174 2069 6e74 656c 6c69 6765  threat intellige
+00005290: 6e63 6520 696e 2074 6865 2073 756d 6d61  nce in the summa
+000052a0: 7279 2072 6570 6f72 740a 2020 2020 2020  ry report.      
+000052b0: 2020 2020 2020 3a74 7970 6520 696e 636c        :type incl
+000052c0: 7564 655f 6e65 7477 6f72 6b74 6872 6561  ude_networkthrea
+000052d0: 7469 6e74 656c 6c69 6765 6e63 653a 2062  tintelligence: b
+000052e0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+000052f0: 3a70 6172 616d 2073 6b69 705f 7265 616e  :param skip_rean
+00005300: 616c 7973 6973 3a20 736b 6970 2073 616d  alysis: skip sam
+00005310: 706c 6520 7265 616e 616c 7973 6973 2077  ple reanalysis w
+00005320: 6865 6e20 6665 7463 6869 6e67 2074 6865  hen fetching the
+00005330: 2073 756d 6d61 7279 2072 6570 6f72 740a   summary report.
+00005340: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+00005350: 6520 736b 6970 5f72 6561 6e61 6c79 7369  e skip_reanalysi
+00005360: 733a 2062 6f6f 6c0a 2020 2020 2020 2020  s: bool.        
+00005370: 2020 2020 3a72 6574 7572 6e3a 203a 636c      :return: :cl
+00005380: 6173 733a 6052 6573 706f 6e73 6520 3c52  ass:`Response <R
+00005390: 6573 706f 6e73 653e 6020 6f62 6a65 6374  esponse>` object
+000053a0: 0a20 2020 2020 2020 2020 2020 203a 7274  .            :rt
+000053b0: 7970 653a 2072 6571 7565 7374 732e 5265  ype: requests.Re
+000053c0: 7370 6f6e 7365 0a20 2020 2020 2020 2022  sponse.        "
+000053d0: 2222 0a20 2020 2020 2020 2069 6620 6669  "".        if fi
+000053e0: 656c 6473 2061 6e64 206e 6f74 2069 7369  elds and not isi
+000053f0: 6e73 7461 6e63 6528 6669 656c 6473 2c20  nstance(fields, 
+00005400: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
+00005410: 2020 2072 6169 7365 2057 726f 6e67 496e     raise WrongIn
+00005420: 7075 7445 7272 6f72 2822 6669 656c 6473  putError("fields
+00005430: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
+00005440: 6265 2061 206c 6973 7420 6f66 2073 7472  be a list of str
+00005450: 696e 6773 2e22 290a 0a20 2020 2020 2020  ings.")..       
+00005460: 2069 6620 6e6f 7420 6669 656c 6473 3a0a   if not fields:.
+00005470: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
+00005480: 6473 203d 2073 656c 662e 5f66 6965 6c64  ds = self._field
+00005490: 735f 7632 0a0a 2020 2020 2020 2020 6966  s_v2..        if
+000054a0: 2072 6574 7279 206e 6f74 2069 6e20 2854   retry not in (T
+000054b0: 7275 652c 2046 616c 7365 293a 0a20 2020  rue, False):.   
+000054c0: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+000054d0: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+000054e0: 7265 7472 7920 7061 7261 6d65 7465 7220  retry parameter 
+000054f0: 6d75 7374 2062 6520 626f 6f6c 6561 6e2e  must be boolean.
+00005500: 2229 0a0a 2020 2020 2020 2020 6966 2069  ")..        if i
+00005510: 7369 6e73 7461 6e63 6528 7361 6d70 6c65  sinstance(sample
+00005520: 5f68 6173 6865 732c 2073 7472 293a 0a20  _hashes, str):. 
+00005530: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
+00005540: 655f 6861 7368 6573 203d 205b 7361 6d70  e_hashes = [samp
+00005550: 6c65 5f68 6173 6865 735d 0a0a 2020 2020  le_hashes]..    
+00005560: 2020 2020 7661 6c69 6461 7465 5f68 6173      validate_has
+00005570: 6865 7328 0a20 2020 2020 2020 2020 2020  hes(.           
+00005580: 2068 6173 685f 696e 7075 743d 7361 6d70   hash_input=samp
+00005590: 6c65 5f68 6173 6865 732c 0a20 2020 2020  le_hashes,.     
+000055a0: 2020 2020 2020 2061 6c6c 6f77 6564 5f68         allowed_h
+000055b0: 6173 685f 7479 7065 733d 284d 4435 2c20  ash_types=(MD5, 
+000055c0: 5348 4131 2c20 5348 4132 3536 2c20 5348  SHA1, SHA256, SH
+000055d0: 4135 3132 290a 2020 2020 2020 2020 290a  A512).        ).
+000055e0: 0a20 2020 2020 2020 2072 6574 7269 6573  .        retries
+000055f0: 203d 2073 656c 662e 5f72 6574 7269 6573   = self._retries
+00005600: 2069 6620 7265 7472 7920 656c 7365 2030   if retry else 0
+00005610: 0a0a 2020 2020 2020 2020 616e 616c 7973  ..        analys
+00005620: 6973 5f69 735f 6669 6e69 7368 6564 203d  is_is_finished =
+00005630: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
+00005640: 666f 7220 6974 6572 6174 696f 6e20 696e  for iteration in
+00005650: 2072 616e 6765 2872 6574 7269 6573 202b   range(retries +
+00005660: 2031 293a 0a20 2020 2020 2020 2020 2020   1):.           
+00005670: 2069 6620 6974 6572 6174 696f 6e3a 0a20   if iteration:. 
+00005680: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00005690: 696d 652e 736c 6565 7028 7365 6c66 2e5f  ime.sleep(self._
+000056a0: 7761 6974 5f74 696d 655f 7365 636f 6e64  wait_time_second
+000056b0: 7329 0a0a 2020 2020 2020 2020 2020 2020  s)..            
+000056c0: 616e 616c 7973 6973 5f69 735f 6669 6e69  analysis_is_fini
+000056d0: 7368 6564 203d 2073 656c 662e 5f5f 616e  shed = self.__an
+000056e0: 616c 7973 6973 5f69 735f 6669 6e69 7368  alysis_is_finish
+000056f0: 6564 2873 616d 706c 655f 6861 7368 6573  ed(sample_hashes
+00005700: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00005710: 2061 6e61 6c79 7369 735f 6973 5f66 696e   analysis_is_fin
+00005720: 6973 6865 643a 0a20 2020 2020 2020 2020  ished:.         
+00005730: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+00005740: 2020 2020 2020 6966 206e 6f74 2061 6e61        if not ana
+00005750: 6c79 7369 735f 6973 5f66 696e 6973 6865  lysis_is_finishe
+00005760: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
+00005770: 6169 7365 2052 6571 7565 7374 5469 6d65  aise RequestTime
+00005780: 6f75 7445 7272 6f72 2822 5265 706f 7274  outError("Report
+00005790: 2066 6574 6368 696e 6720 6174 7465 6d70   fetching attemp
+000057a0: 7473 2066 696e 6973 6865 6420 2d20 5468  ts finished - Th
+000057b0: 6520 616e 616c 7973 6973 2072 6570 6f72  e analysis repor
+000057c0: 7420 6973 2073 7469 6c6c 206e 6f74 2072  t is still not r
+000057d0: 6561 6479 2022 0a20 2020 2020 2020 2020  eady ".         
+000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057f0: 2020 2020 2020 2020 2020 2020 2022 6f72               "or
+00005800: 2074 6865 2073 616d 706c 6520 646f 6573   the sample does
+00005810: 206e 6f74 2065 7869 7374 206f 6e20 7468   not exist on th
+00005820: 6520 6170 706c 6961 6e63 652e 2229 0a0a  e appliance.")..
+00005830: 2020 2020 2020 2020 7572 6c20 3d20 7365          url = se
+00005840: 6c66 2e5f 7572 6c2e 666f 726d 6174 2865  lf._url.format(e
+00005850: 6e64 706f 696e 743d 7365 6c66 2e5f 5f53  ndpoint=self.__S
+00005860: 554d 4d41 5259 5f52 4550 4f52 545f 454e  UMMARY_REPORT_EN
+00005870: 4450 4f49 4e54 5f56 3229 0a0a 2020 2020  DPOINT_V2)..    
+00005880: 2020 2020 6966 2069 6e63 6c75 6465 5f6e      if include_n
+00005890: 6574 776f 726b 7468 7265 6174 696e 7465  etworkthreatinte
+000058a0: 6c6c 6967 656e 6365 206e 6f74 2069 6e20  lligence not in 
+000058b0: 2854 7275 652c 2046 616c 7365 293a 0a20  (True, False):. 
+000058c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000058d0: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
+000058e0: 2822 696e 636c 7564 655f 6e65 7477 6f72  ("include_networ
+000058f0: 6b74 6872 6561 7469 6e74 656c 6c69 6765  kthreatintellige
+00005900: 6e63 6520 7061 7261 6d65 7465 7220 6d75  nce parameter mu
+00005910: 7374 2062 6520 626f 6f6c 6561 6e2e 2229  st be boolean.")
+00005920: 0a0a 2020 2020 2020 2020 6966 2069 6e63  ..        if inc
+00005930: 6c75 6465 5f6e 6574 776f 726b 7468 7265  lude_networkthre
+00005940: 6174 696e 7465 6c6c 6967 656e 6365 2061  atintelligence a
+00005950: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
+00005960: 2020 2020 2028 226e 6574 776f 726b 7468       ("networkth
+00005970: 7265 6174 696e 7465 6c6c 6967 656e 6365  reatintelligence
+00005980: 2220 6e6f 7420 696e 2066 6965 6c64 7320  " not in fields 
+00005990: 6f72 2022 646f 6d61 696e 7468 7265 6174  or "domainthreat
+000059a0: 696e 7465 6c6c 6967 656e 6365 2220 6e6f  intelligence" no
+000059b0: 7420 696e 2066 6965 6c64 7329 3a0a 2020  t in fields):.  
+000059c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000059d0: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
+000059e0: 2249 6620 696e 636c 7564 655f 6e65 7477  "If include_netw
+000059f0: 6f72 6b74 6872 6561 7469 6e74 656c 6c69  orkthreatintelli
+00005a00: 6765 6e63 6520 6973 2073 6574 2074 6f20  gence is set to 
+00005a10: 5472 7565 2c20 7468 6520 6669 656c 6473  True, the fields
+00005a20: 206c 6973 7420 6d75 7374 2069 6e63 6c75   list must inclu
+00005a30: 6465 2022 0a20 2020 2020 2020 2020 2020  de ".           
+00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a50: 2020 2020 2020 2022 626f 7468 2027 6e65         "both 'ne
+00005a60: 7477 6f72 6b74 6872 6561 7469 6e74 656c  tworkthreatintel
+00005a70: 6c69 6765 6e63 6527 2061 6e64 2027 646f  ligence' and 'do
+00005a80: 6d61 696e 7468 7265 6174 696e 7465 6c6c  mainthreatintell
+00005a90: 6967 656e 6365 272e 2229 0a0a 2020 2020  igence'.")..    
+00005aa0: 2020 2020 6966 2073 6b69 705f 7265 616e      if skip_rean
+00005ab0: 616c 7973 6973 206e 6f74 2069 6e20 2854  alysis not in (T
+00005ac0: 7275 652c 2046 616c 7365 293a 0a20 2020  rue, False):.   
+00005ad0: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+00005ae0: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+00005af0: 736b 6970 5f72 6561 6e61 6c79 7369 7320  skip_reanalysis 
+00005b00: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
+00005b10: 6520 626f 6f6c 6561 6e2e 2229 0a0a 2020  e boolean.")..  
+00005b20: 2020 2020 2020 6461 7461 203d 207b 0a20        data = {. 
+00005b30: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
+00005b40: 5f76 616c 7565 7322 3a20 7361 6d70 6c65  _values": sample
+00005b50: 5f68 6173 6865 732c 0a20 2020 2020 2020  _hashes,.       
+00005b60: 2020 2020 2022 6669 656c 6473 223a 2066       "fields": f
+00005b70: 6965 6c64 732c 0a20 2020 2020 2020 2020  ields,.         
+00005b80: 2020 2022 696e 636c 7564 655f 6e65 7477     "include_netw
+00005b90: 6f72 6b74 6872 6561 7469 6e74 656c 6c69  orkthreatintelli
+00005ba0: 6765 6e63 6522 3a20 7374 7228 696e 636c  gence": str(incl
+00005bb0: 7564 655f 6e65 7477 6f72 6b74 6872 6561  ude_networkthrea
+00005bc0: 7469 6e74 656c 6c69 6765 6e63 6529 2e6c  tintelligence).l
+00005bd0: 6f77 6572 2829 2c0a 2020 2020 2020 2020  ower(),.        
+00005be0: 2020 2020 2273 6b69 705f 7265 616e 616c      "skip_reanal
+00005bf0: 7973 6973 223a 2073 7472 2873 6b69 705f  ysis": str(skip_
+00005c00: 7265 616e 616c 7973 6973 292e 6c6f 7765  reanalysis).lowe
+00005c10: 7228 290a 2020 2020 2020 2020 7d0a 0a20  r().        }.. 
+00005c20: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+00005c30: 3d20 7365 6c66 2e5f 5f70 6f73 745f 7265  = self.__post_re
+00005c40: 7175 6573 7428 7572 6c3d 7572 6c2c 2064  quest(url=url, d
+00005c50: 6174 613d 6461 7461 290a 0a20 2020 2020  ata=data)..     
+00005c60: 2020 2073 656c 662e 5f5f 7261 6973 655f     self.__raise_
+00005c70: 6f6e 5f65 7272 6f72 2872 6573 706f 6e73  on_error(respons
+00005c80: 6529 0a0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00005c90: 726e 2072 6573 706f 6e73 650a 0a20 2020  rn response..   
+00005ca0: 2064 6566 2075 706c 6f61 645f 7361 6d70   def upload_samp
+00005cb0: 6c65 5f61 6e64 5f67 6574 5f72 6573 756c  le_and_get_resul
+00005cc0: 7473 2873 656c 662c 2066 696c 655f 7061  ts(self, file_pa
+00005cd0: 7468 3d4e 6f6e 652c 2066 696c 655f 736f  th=None, file_so
+00005ce0: 7572 6365 3d4e 6f6e 652c 2072 6574 7279  urce=None, retry
+00005cf0: 3d54 7275 652c 2063 7573 746f 6d5f 6669  =True, custom_fi
+00005d00: 6c65 6e61 6d65 3d4e 6f6e 652c 0a20 2020  lename=None,.   
+00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d30: 2020 2074 6167 733d 4e6f 6e65 2c20 636f     tags=None, co
+00005d40: 6d6d 656e 743d 4e6f 6e65 2c20 636c 6f75  mment=None, clou
+00005d50: 645f 616e 616c 7973 6973 3d54 7275 6529  d_analysis=True)
+00005d60: 3a0a 2020 2020 2020 2020 2222 2254 4849  :.        """THI
+00005d70: 5320 4d45 5448 4f44 2049 5320 4445 5052  S METHOD IS DEPR
+00005d80: 4543 4154 4544 2e20 5573 6520 7570 6c6f  ECATED. Use uplo
+00005d90: 6164 5f73 616d 706c 655f 616e 645f 6765  ad_sample_and_ge
+00005da0: 745f 7375 6d6d 6172 795f 7265 706f 7274  t_summary_report
+00005db0: 5f76 3220 696e 7374 6561 642e 0a0a 2020  _v2 instead...  
+00005dc0: 2020 2020 2020 4163 6365 7074 7320 6569        Accepts ei
+00005dd0: 7468 6572 2061 2066 696c 6520 7061 7468  ther a file path
+00005de0: 2073 7472 696e 6720 6f72 2061 6e20 6f70   string or an op
+00005df0: 656e 2066 696c 6520 696e 2027 7262 2720  en file in 'rb' 
+00005e00: 6d6f 6465 2066 6f72 2066 696c 6520 7570  mode for file up
+00005e10: 6c6f 6164 2061 6e64 2072 6574 7572 6e73  load and returns
+00005e20: 0a20 2020 2020 2020 2061 6e20 616e 616c  .        an anal
+00005e30: 7973 6973 2072 6570 6f72 7420 7265 7370  ysis report resp
+00005e40: 6f6e 7365 2e20 5468 6973 206d 6574 686f  onse. This metho
+00005e50: 6420 636f 6d62 696e 6573 2075 706c 6f61  d combines uploa
+00005e60: 6469 6e67 2061 2073 616d 706c 6520 616e  ding a sample an
+00005e70: 6420 6f62 7461 696e 696e 6720 7468 6520  d obtaining the 
+00005e80: 616e 616c 7973 6973 2072 6573 756c 7473  analysis results
+00005e90: 2e0a 2020 2020 2020 2020 4164 6469 7469  ..        Additi
+00005ea0: 6f6e 616c 2066 6965 6c64 7320 6361 6e20  onal fields can 
+00005eb0: 6265 2070 726f 7669 6465 642e 0a20 2020  be provided..   
+00005ec0: 2020 2020 2054 6865 2072 6573 756c 7420       The result 
+00005ed0: 6f62 7461 696e 696e 6720 6163 7469 6f6e  obtaining action
+00005ee0: 206f 6620 7468 6973 206d 6574 686f 6420   of this method 
+00005ef0: 7574 696c 697a 6573 2074 6865 2073 6574  utilizes the set
+00005f00: 206e 756d 6265 7220 6f66 2072 6574 7269   number of retri
+00005f10: 6573 2061 6e64 2077 6169 7420 7469 6d65  es and wait time
+00005f20: 2069 6e20 7365 636f 6e64 7320 746f 2074   in seconds to t
+00005f30: 696d 650a 2020 2020 2020 2020 6f75 7420  ime.        out 
+00005f40: 6966 2074 6865 2061 6e61 6c79 7369 7320  if the analysis 
+00005f50: 7265 7375 6c74 7320 6172 6520 6e6f 7420  results are not 
+00005f60: 7265 6164 792e 0a20 2020 2020 2020 2020  ready..         
+00005f70: 2020 203a 7061 7261 6d20 6669 6c65 5f70     :param file_p
+00005f80: 6174 683a 2066 696c 6520 7061 7468 0a20  ath: file path. 
+00005f90: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00005fa0: 2066 696c 655f 7061 7468 3a20 7374 720a   file_path: str.
+00005fb0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00005fc0: 616d 2066 696c 655f 736f 7572 6365 3a20  am file_source: 
+00005fd0: 6f70 656e 2066 696c 650a 2020 2020 2020  open file.      
+00005fe0: 2020 2020 2020 3a74 7970 6520 6669 6c65        :type file
+00005ff0: 5f73 6f75 7263 653a 2066 696c 6520 6f72  _source: file or
+00006000: 2042 696e 6172 7949 4f0a 2020 2020 2020   BinaryIO.      
+00006010: 2020 2020 2020 3a70 6172 616d 2072 6574        :param ret
+00006020: 7279 3a20 6966 2073 6574 2074 6f20 4661  ry: if set to Fa
+00006030: 6c73 6520 7468 6572 6520 7769 6c6c 206f  lse there will o
+00006040: 6e6c 7920 6265 206f 6e65 2074 7279 2061  nly be one try a
+00006050: 7420 6f62 7461 696e 696e 6720 7468 6520  t obtaining the 
+00006060: 616e 616c 7973 6973 2072 6570 6f72 740a  analysis report.
+00006070: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+00006080: 6520 7265 7472 793a 2062 6f6f 6c0a 2020  e retry: bool.  
+00006090: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+000060a0: 2063 7573 746f 6d5f 6669 6c65 6e61 6d65   custom_filename
+000060b0: 3a20 6375 7374 6f6d 2066 696c 6520 6e61  : custom file na
+000060c0: 6d65 2066 6f72 2075 706c 6f61 640a 2020  me for upload.  
+000060d0: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+000060e0: 6375 7374 6f6d 5f66 696c 656e 616d 653a  custom_filename:
+000060f0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+00006100: 203a 7061 7261 6d20 7461 6773 3a20 6120   :param tags: a 
+00006110: 7374 7269 6e67 206f 6620 636f 6d6d 6120  string of comma 
+00006120: 7365 7061 7261 7465 6420 7461 6773 0a20  separated tags. 
+00006130: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00006140: 2074 6167 733a 2073 7472 0a20 2020 2020   tags: str.     
+00006150: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+00006160: 6d6d 656e 743a 2063 6f6d 6d65 6e74 2073  mment: comment s
+00006170: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+00006180: 2020 3a74 7970 6520 636f 6d6d 656e 743a    :type comment:
+00006190: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+000061a0: 203a 7061 7261 6d20 636c 6f75 645f 616e   :param cloud_an
+000061b0: 616c 7973 6973 3a20 7573 6520 636c 6f75  alysis: use clou
+000061c0: 6420 616e 616c 7973 6973 0a20 2020 2020  d analysis.     
+000061d0: 2020 2020 2020 203a 7479 7065 2063 6c6f         :type clo
+000061e0: 7564 5f61 6e61 6c79 7369 733a 2062 6f6f  ud_analysis: boo
+000061f0: 6c0a 2020 2020 2020 2020 2020 2020 3a72  l.            :r
+00006200: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
+00006210: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
+00006220: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
+00006230: 706f 6e73 650a 2020 2020 2020 2020 2222  ponse.        ""
+00006240: 220a 2020 2020 2020 2020 7761 726e 2822  ".        warn("
+00006250: 5468 6973 206d 6574 686f 6420 6973 2064  This method is d
+00006260: 6570 7265 6361 7465 642e 2055 7365 2075  eprecated. Use u
+00006270: 706c 6f61 645f 7361 6d70 6c65 5f61 6e64  pload_sample_and
+00006280: 5f67 6574 5f73 756d 6d61 7279 5f72 6570  _get_summary_rep
+00006290: 6f72 745f 7632 2069 6e73 7465 6164 2e22  ort_v2 instead."
+000062a0: 2c20 4465 7072 6563 6174 696f 6e57 6172  , DeprecationWar
+000062b0: 6e69 6e67 290a 0a20 2020 2020 2020 2069  ning)..        i
+000062c0: 6620 2866 696c 655f 7061 7468 2061 6e64  f (file_path and
+000062d0: 2066 696c 655f 736f 7572 6365 2920 6f72   file_source) or
+000062e0: 2028 6e6f 7420 6669 6c65 5f70 6174 6820   (not file_path 
+000062f0: 616e 6420 6e6f 7420 6669 6c65 5f73 6f75  and not file_sou
+00006300: 7263 6529 3a0a 2020 2020 2020 2020 2020  rce):.          
+00006310: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+00006320: 7574 4572 726f 7228 2245 6974 6865 7220  utError("Either 
+00006330: 6669 6c65 5f70 6174 6820 6f72 2066 696c  file_path or fil
+00006340: 655f 736f 7572 6365 2070 6172 616d 6574  e_source paramet
+00006350: 6572 206d 7573 7420 6265 2070 726f 7669  er must be provi
+00006360: 6465 642e 2022 0a20 2020 2020 2020 2020  ded. ".         
+00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006380: 2020 2020 2020 2020 2022 5573 696e 6720           "Using 
+00006390: 626f 7468 206f 7220 6e6f 6e65 206f 6620  both or none of 
+000063a0: 7468 6520 7061 7261 6d65 7465 7273 2069  the parameters i
+000063b0: 6e20 736f 7420 616c 6c6f 7765 642e 2229  n sot allowed.")
+000063c0: 0a0a 2020 2020 2020 2020 6966 2066 696c  ..        if fil
+000063d0: 655f 7061 7468 3a0a 2020 2020 2020 2020  e_path:.        
+000063e0: 2020 2020 7570 6c6f 6164 5f72 6573 706f      upload_respo
+000063f0: 6e73 6520 3d20 7365 6c66 2e75 706c 6f61  nse = self.uploa
+00006400: 645f 7361 6d70 6c65 5f66 726f 6d5f 7061  d_sample_from_pa
+00006410: 7468 2866 696c 655f 7061 7468 2c20 6375  th(file_path, cu
+00006420: 7374 6f6d 5f66 696c 656e 616d 652c 2074  stom_filename, t
+00006430: 6167 732c 2063 6f6d 6d65 6e74 2c20 636c  ags, comment, cl
+00006440: 6f75 645f 616e 616c 7973 6973 290a 2020  oud_analysis).  
+00006450: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00006460: 2020 2020 2020 2020 7570 6c6f 6164 5f72          upload_r
+00006470: 6573 706f 6e73 6520 3d20 7365 6c66 2e75  esponse = self.u
+00006480: 706c 6f61 645f 7361 6d70 6c65 5f66 726f  pload_sample_fro
+00006490: 6d5f 6669 6c65 2866 696c 655f 736f 7572  m_file(file_sour
+000064a0: 6365 2c20 6375 7374 6f6d 5f66 696c 656e  ce, custom_filen
+000064b0: 616d 652c 2074 6167 732c 2063 6f6d 6d65  ame, tags, comme
+000064c0: 6e74 2c20 636c 6f75 645f 616e 616c 7973  nt, cloud_analys
+000064d0: 6973 290a 0a20 2020 2020 2020 2072 6573  is)..        res
+000064e0: 706f 6e73 655f 6465 7461 696c 203d 2075  ponse_detail = u
+000064f0: 706c 6f61 645f 7265 7370 6f6e 7365 2e6a  pload_response.j
+00006500: 736f 6e28 292e 6765 7428 2264 6574 6169  son().get("detai
+00006510: 6c22 290a 2020 2020 2020 2020 7368 6131  l").        sha1
+00006520: 203d 2072 6573 706f 6e73 655f 6465 7461   = response_deta
+00006530: 696c 2e67 6574 2822 7368 6131 2229 0a20  il.get("sha1"). 
+00006540: 2020 2020 2020 2073 6861 3120 3d20 7374         sha1 = st
+00006550: 7228 7368 6131 290a 0a20 2020 2020 2020  r(sha1)..       
+00006560: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
+00006570: 2e67 6574 5f72 6573 756c 7473 280a 2020  .get_results(.  
+00006580: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
+00006590: 5f68 6173 6865 733d 5b73 6861 315d 2c0a  _hashes=[sha1],.
+000065a0: 2020 2020 2020 2020 2020 2020 7265 7472              retr
+000065b0: 793d 7265 7472 790a 2020 2020 2020 2020  y=retry.        
+000065c0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000065d0: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
+000065e0: 6465 6620 7570 6c6f 6164 5f73 616d 706c  def upload_sampl
+000065f0: 655f 616e 645f 6765 745f 7375 6d6d 6172  e_and_get_summar
+00006600: 795f 7265 706f 7274 5f76 3228 7365 6c66  y_report_v2(self
+00006610: 2c20 6669 6c65 5f70 6174 683d 4e6f 6e65  , file_path=None
+00006620: 2c20 6669 6c65 5f73 6f75 7263 653d 4e6f  , file_source=No
+00006630: 6e65 2c20 7265 7472 793d 5472 7565 2c20  ne, retry=True, 
+00006640: 6669 656c 6473 3d4e 6f6e 652c 0a20 2020  fields=None,.   
+00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006670: 2020 2020 2020 2020 2020 2020 2069 6e63               inc
+00006680: 6c75 6465 5f6e 6574 776f 726b 7468 7265  lude_networkthre
+00006690: 6174 696e 7465 6c6c 6967 656e 6365 3d54  atintelligence=T
+000066a0: 7275 652c 2073 6b69 705f 7265 616e 616c  rue, skip_reanal
+000066b0: 7973 6973 3d46 616c 7365 2c0a 2020 2020  ysis=False,.    
+000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066e0: 2020 2020 2020 2020 2020 2020 6375 7374              cust
+000066f0: 6f6d 5f66 696c 656e 616d 653d 4e6f 6e65  om_filename=None
+00006700: 2c20 7461 6773 3d4e 6f6e 652c 2063 6f6d  , tags=None, com
+00006710: 6d65 6e74 3d4e 6f6e 652c 2063 6c6f 7564  ment=None, cloud
+00006720: 5f61 6e61 6c79 7369 733d 5472 7565 2c0a  _analysis=True,.
+00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006760: 6172 6368 6976 655f 7061 7373 776f 7264  archive_password
+00006770: 3d4e 6f6e 652c 2072 6c5f 636c 6f75 645f  =None, rl_cloud_
+00006780: 7361 6e64 626f 785f 706c 6174 666f 726d  sandbox_platform
+00006790: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+000067a0: 2222 2241 6363 6570 7473 2065 6974 6865  """Accepts eithe
+000067b0: 7220 6120 6669 6c65 2070 6174 6820 7374  r a file path st
+000067c0: 7269 6e67 206f 7220 616e 206f 7065 6e20  ring or an open 
+000067d0: 6669 6c65 2069 6e20 2772 6227 206d 6f64  file in 'rb' mod
+000067e0: 6520 666f 7220 6669 6c65 2075 706c 6f61  e for file uploa
+000067f0: 6420 616e 6420 7265 7475 726e 7320 6120  d and returns a 
+00006800: 7375 6d6d 6172 7920 616e 616c 7973 6973  summary analysis
+00006810: 0a20 2020 2020 2020 2072 6570 6f72 7420  .        report 
+00006820: 7265 7370 6f6e 7365 2e20 5468 6973 206d  response. This m
+00006830: 6574 686f 6420 636f 6d62 696e 6573 2075  ethod combines u
+00006840: 706c 6f61 6469 6e67 2061 2073 616d 706c  ploading a sampl
+00006850: 6520 616e 6420 6f62 7461 696e 696e 6720  e and obtaining 
+00006860: 7468 6520 7375 6d6d 6172 7920 616e 616c  the summary anal
+00006870: 7973 6973 2072 6570 6f72 742e 0a20 2020  ysis report..   
+00006880: 2020 2020 2041 6464 6974 696f 6e61 6c20       Additional 
+00006890: 6669 656c 6473 2063 616e 2062 6520 7072  fields can be pr
+000068a0: 6f76 6964 6564 2e0a 2020 2020 2020 2020  ovided..        
+000068b0: 5468 6520 7265 7375 6c74 2066 6574 6368  The result fetch
+000068c0: 696e 6720 6163 7469 6f6e 206f 6620 7468  ing action of th
+000068d0: 6973 206d 6574 686f 6420 7574 696c 697a  is method utiliz
+000068e0: 6573 2074 6865 2073 6574 206e 756d 6265  es the set numbe
+000068f0: 7220 6f66 2072 6574 7269 6573 2061 6e64  r of retries and
+00006900: 2077 6169 7420 7469 6d65 2069 6e20 7365   wait time in se
+00006910: 636f 6e64 7320 746f 2074 696d 650a 2020  conds to time.  
+00006920: 2020 2020 2020 6f75 7420 6966 2074 6865        out if the
+00006930: 2061 6e61 6c79 7369 7320 7265 7375 6c74   analysis result
+00006940: 7320 6172 6520 6e6f 7420 7265 6164 792e  s are not ready.
+00006950: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+00006960: 7261 6d20 6669 6c65 5f70 6174 683a 2066  ram file_path: f
+00006970: 696c 6520 7061 7468 0a20 2020 2020 2020  ile path.       
+00006980: 2020 2020 203a 7479 7065 2066 696c 655f       :type file_
+00006990: 7061 7468 3a20 7374 720a 2020 2020 2020  path: str.      
+000069a0: 2020 2020 2020 3a70 6172 616d 2066 696c        :param fil
+000069b0: 655f 736f 7572 6365 3a20 6f70 656e 2066  e_source: open f
+000069c0: 696c 650a 2020 2020 2020 2020 2020 2020  ile.            
+000069d0: 3a74 7970 6520 6669 6c65 5f73 6f75 7263  :type file_sourc
+000069e0: 653a 2066 696c 6520 6f72 2042 696e 6172  e: file or Binar
+000069f0: 7949 4f0a 2020 2020 2020 2020 2020 2020  yIO.            
+00006a00: 3a70 6172 616d 2072 6574 7279 3a20 6966  :param retry: if
+00006a10: 2073 6574 2074 6f20 4661 6c73 6520 7468   set to False th
+00006a20: 6572 6520 7769 6c6c 206f 6e6c 7920 6265  ere will only be
+00006a30: 206f 6e65 2074 7279 2061 7420 6f62 7461   one try at obta
+00006a40: 696e 696e 6720 7468 6520 616e 616c 7973  ining the analys
+00006a50: 6973 2072 6570 6f72 740a 2020 2020 2020  is report.      
+00006a60: 2020 2020 2020 3a74 7970 6520 7265 7472        :type retr
+00006a70: 793a 2062 6f6f 6c0a 2020 2020 2020 2020  y: bool.        
+00006a80: 2020 2020 3a70 6172 616d 2066 6965 6c64      :param field
+00006a90: 733a 206c 6973 7420 6f66 2041 3130 3030  s: list of A1000
+00006aa0: 2072 6570 6f72 7420 2766 6965 6c64 7327   report 'fields'
+00006ab0: 2074 6f20 7175 6572 790a 2020 2020 2020   to query.      
+00006ac0: 2020 2020 2020 3a74 7970 6520 6669 656c        :type fiel
+00006ad0: 6473 3a20 6c69 7374 5b73 7472 5d0a 2020  ds: list[str].  
+00006ae0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00006af0: 2069 6e63 6c75 6465 5f6e 6574 776f 726b   include_network
+00006b00: 7468 7265 6174 696e 7465 6c6c 6967 656e  threatintelligen
+00006b10: 6365 3a20 696e 636c 7564 6520 6e65 7477  ce: include netw
+00006b20: 6f72 6b20 7468 7265 6174 2069 6e74 656c  ork threat intel
+00006b30: 6c69 6765 6e63 6520 696e 2074 6865 2073  ligence in the s
+00006b40: 756d 6d61 7279 2072 6570 6f72 740a 2020  ummary report.  
+00006b50: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00006b60: 696e 636c 7564 655f 6e65 7477 6f72 6b74  include_networkt
+00006b70: 6872 6561 7469 6e74 656c 6c69 6765 6e63  hreatintelligenc
+00006b80: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00006b90: 2020 2020 3a70 6172 616d 2073 6b69 705f      :param skip_
+00006ba0: 7265 616e 616c 7973 6973 3a20 736b 6970  reanalysis: skip
+00006bb0: 2073 616d 706c 6520 7265 616e 616c 7973   sample reanalys
+00006bc0: 6973 2077 6865 6e20 6665 7463 6869 6e67  is when fetching
+00006bd0: 2074 6865 2073 756d 6d61 7279 2072 6570   the summary rep
+00006be0: 6f72 740a 2020 2020 2020 2020 2020 2020  ort.            
+00006bf0: 3a74 7970 6520 736b 6970 5f72 6561 6e61  :type skip_reana
+00006c00: 6c79 7369 733a 2062 6f6f 6c0a 2020 2020  lysis: bool.    
+00006c10: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+00006c20: 7573 746f 6d5f 6669 6c65 6e61 6d65 3a20  ustom_filename: 
+00006c30: 6375 7374 6f6d 2066 696c 6520 6e61 6d65  custom file name
+00006c40: 2066 6f72 2075 706c 6f61 640a 2020 2020   for upload.    
+00006c50: 2020 2020 2020 2020 3a74 7970 6520 6375          :type cu
+00006c60: 7374 6f6d 5f66 696c 656e 616d 653a 2073  stom_filename: s
+00006c70: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
+00006c80: 7061 7261 6d20 7461 6773 3a20 6120 7374  param tags: a st
+00006c90: 7269 6e67 206f 6620 636f 6d6d 6120 7365  ring of comma se
+00006ca0: 7061 7261 7465 6420 7461 6773 0a20 2020  parated tags.   
+00006cb0: 2020 2020 2020 2020 203a 7479 7065 2074           :type t
+00006cc0: 6167 733a 2073 7472 0a20 2020 2020 2020  ags: str.       
+00006cd0: 2020 2020 203a 7061 7261 6d20 636f 6d6d       :param comm
+00006ce0: 656e 743a 2063 6f6d 6d65 6e74 2073 7472  ent: comment str
+00006cf0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00006d00: 3a74 7970 6520 636f 6d6d 656e 743a 2073  :type comment: s
+00006d10: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
+00006d20: 7061 7261 6d20 636c 6f75 645f 616e 616c  param cloud_anal
+00006d30: 7973 6973 3a20 7573 6520 636c 6f75 6420  ysis: use cloud 
+00006d40: 616e 616c 7973 6973 0a20 2020 2020 2020  analysis.       
+00006d50: 2020 2020 203a 7479 7065 2063 6c6f 7564       :type cloud
+00006d60: 5f61 6e61 6c79 7369 733a 2062 6f6f 6c0a  _analysis: bool.
+00006d70: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00006d80: 616d 2061 7263 6869 7665 5f70 6173 7377  am archive_passw
+00006d90: 6f72 643a 2070 6173 7377 6f72 642c 2069  ord: password, i
+00006da0: 6620 6669 6c65 2069 7320 6120 7061 7373  f file is a pass
+00006db0: 776f 7264 2d70 726f 7465 6374 6564 2061  word-protected a
+00006dc0: 7263 6869 7665 0a20 2020 2020 2020 2020  rchive.         
+00006dd0: 2020 203a 7479 7065 2061 7263 6869 7665     :type archive
+00006de0: 5f70 6173 7377 6f72 643a 2073 7472 0a20  _password: str. 
+00006df0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00006e00: 6d20 726c 5f63 6c6f 7564 5f73 616e 6462  m rl_cloud_sandb
+00006e10: 6f78 5f70 6c61 7466 6f72 6d3a 2043 6c6f  ox_platform: Clo
+00006e20: 7564 2053 616e 6462 6f78 2070 6c61 7466  ud Sandbox platf
+00006e30: 6f72 6d20 2877 696e 646f 7773 372c 2077  orm (windows7, w
+00006e40: 696e 646f 7773 3130 206f 7220 6d61 636f  indows10 or maco
+00006e50: 735f 3131 290a 2020 2020 2020 2020 2020  s_11).          
+00006e60: 2020 3a74 7970 6520 726c 5f63 6c6f 7564    :type rl_cloud
+00006e70: 5f73 616e 6462 6f78 5f70 6c61 7466 6f72  _sandbox_platfor
+00006e80: 6d3a 2073 7472 0a20 2020 2020 2020 2020  m: str.         
+00006e90: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
+00006ea0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
+00006eb0: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
+00006ec0: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
+00006ed0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00006ee0: 6620 2866 696c 655f 7061 7468 2061 6e64  f (file_path and
+00006ef0: 2066 696c 655f 736f 7572 6365 2920 6f72   file_source) or
+00006f00: 2028 6e6f 7420 6669 6c65 5f70 6174 6820   (not file_path 
+00006f10: 616e 6420 6e6f 7420 6669 6c65 5f73 6f75  and not file_sou
+00006f20: 7263 6529 3a0a 2020 2020 2020 2020 2020  rce):.          
+00006f30: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+00006f40: 7574 4572 726f 7228 2245 6974 6865 7220  utError("Either 
+00006f50: 6669 6c65 5f70 6174 6820 6f72 2066 696c  file_path or fil
+00006f60: 655f 736f 7572 6365 2070 6172 616d 6574  e_source paramet
+00006f70: 6572 206d 7573 7420 6265 2070 726f 7669  er must be provi
+00006f80: 6465 642e 2022 0a20 2020 2020 2020 2020  ded. ".         
+00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fa0: 2020 2020 2020 2020 2022 5573 696e 6720           "Using 
+00006fb0: 626f 7468 206f 7220 6e6f 6e65 206f 6620  both or none of 
+00006fc0: 7468 6520 7061 7261 6d65 7465 7273 2069  the parameters i
+00006fd0: 6e20 736f 7420 616c 6c6f 7765 642e 2229  n sot allowed.")
+00006fe0: 0a0a 2020 2020 2020 2020 6966 2066 696c  ..        if fil
+00006ff0: 655f 7061 7468 3a0a 2020 2020 2020 2020  e_path:.        
+00007000: 2020 2020 7570 6c6f 6164 5f72 6573 706f      upload_respo
+00007010: 6e73 6520 3d20 7365 6c66 2e75 706c 6f61  nse = self.uploa
+00007020: 645f 7361 6d70 6c65 5f66 726f 6d5f 7061  d_sample_from_pa
+00007030: 7468 2866 696c 655f 7061 7468 2c20 6375  th(file_path, cu
+00007040: 7374 6f6d 5f66 696c 656e 616d 652c 2061  stom_filename, a
+00007050: 7263 6869 7665 5f70 6173 7377 6f72 642c  rchive_password,
+00007060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007090: 2020 2020 2020 2020 2020 2020 726c 5f63              rl_c
+000070a0: 6c6f 7564 5f73 616e 6462 6f78 5f70 6c61  loud_sandbox_pla
+000070b0: 7466 6f72 6d2c 2074 6167 732c 2063 6f6d  tform, tags, com
+000070c0: 6d65 6e74 2c20 636c 6f75 645f 616e 616c  ment, cloud_anal
+000070d0: 7973 6973 290a 2020 2020 2020 2020 656c  ysis).        el
+000070e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000070f0: 7570 6c6f 6164 5f72 6573 706f 6e73 6520  upload_response 
+00007100: 3d20 7365 6c66 2e75 706c 6f61 645f 7361  = self.upload_sa
+00007110: 6d70 6c65 5f66 726f 6d5f 6669 6c65 2866  mple_from_file(f
+00007120: 696c 655f 736f 7572 6365 2c20 6375 7374  ile_source, cust
+00007130: 6f6d 5f66 696c 656e 616d 652c 2074 6167  om_filename, tag
+00007140: 732c 2061 7263 6869 7665 5f70 6173 7377  s, archive_passw
+00007150: 6f72 642c 0a20 2020 2020 2020 2020 2020  ord,.           
+00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007190: 726c 5f63 6c6f 7564 5f73 616e 6462 6f78  rl_cloud_sandbox
+000071a0: 5f70 6c61 7466 6f72 6d2c 2063 6f6d 6d65  _platform, comme
+000071b0: 6e74 2c20 636c 6f75 645f 616e 616c 7973  nt, cloud_analys
+000071c0: 6973 290a 0a20 2020 2020 2020 2072 6573  is)..        res
+000071d0: 706f 6e73 655f 6465 7461 696c 203d 2075  ponse_detail = u
+000071e0: 706c 6f61 645f 7265 7370 6f6e 7365 2e6a  pload_response.j
+000071f0: 736f 6e28 292e 6765 7428 2264 6574 6169  son().get("detai
+00007200: 6c22 290a 2020 2020 2020 2020 7368 6131  l").        sha1
+00007210: 203d 2072 6573 706f 6e73 655f 6465 7461   = response_deta
+00007220: 696c 2e67 6574 2822 7368 6131 2229 0a20  il.get("sha1"). 
+00007230: 2020 2020 2020 2073 6861 3120 3d20 7374         sha1 = st
+00007240: 7228 7368 6131 290a 0a20 2020 2020 2020  r(sha1)..       
+00007250: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
+00007260: 2e67 6574 5f73 756d 6d61 7279 5f72 6570  .get_summary_rep
+00007270: 6f72 745f 7632 280a 2020 2020 2020 2020  ort_v2(.        
+00007280: 2020 2020 7361 6d70 6c65 5f68 6173 6865      sample_hashe
+00007290: 733d 5b73 6861 315d 2c0a 2020 2020 2020  s=[sha1],.      
+000072a0: 2020 2020 2020 7265 7472 793d 7265 7472        retry=retr
+000072b0: 792c 0a20 2020 2020 2020 2020 2020 2066  y,.            f
+000072c0: 6965 6c64 733d 6669 656c 6473 2c0a 2020  ields=fields,.  
+000072d0: 2020 2020 2020 2020 2020 696e 636c 7564            includ
+000072e0: 655f 6e65 7477 6f72 6b74 6872 6561 7469  e_networkthreati
+000072f0: 6e74 656c 6c69 6765 6e63 653d 696e 636c  ntelligence=incl
+00007300: 7564 655f 6e65 7477 6f72 6b74 6872 6561  ude_networkthrea
+00007310: 7469 6e74 656c 6c69 6765 6e63 652c 0a20  tintelligence,. 
+00007320: 2020 2020 2020 2020 2020 2073 6b69 705f             skip_
+00007330: 7265 616e 616c 7973 6973 3d73 6b69 705f  reanalysis=skip_
+00007340: 7265 616e 616c 7973 6973 0a20 2020 2020  reanalysis.     
+00007350: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
+00007360: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+00007370: 2020 2064 6566 2067 6574 5f64 6574 6169     def get_detai
+00007380: 6c65 645f 7265 706f 7274 5f76 3228 7365  led_report_v2(se
+00007390: 6c66 2c20 7361 6d70 6c65 5f68 6173 6865  lf, sample_hashe
+000073a0: 732c 2072 6574 7279 3d46 616c 7365 2c20  s, retry=False, 
+000073b0: 6669 656c 6473 3d4e 6f6e 652c 2073 6b69  fields=None, ski
+000073c0: 705f 7265 616e 616c 7973 6973 3d46 616c  p_reanalysis=Fal
+000073d0: 7365 293a 0a20 2020 2020 2020 2022 2222  se):.        """
+000073e0: 4163 6365 7074 7320 6120 7369 6e67 6c65  Accepts a single
+000073f0: 2068 6173 6820 6f72 2061 206c 6973 7420   hash or a list 
+00007400: 6f66 2068 6173 6865 7320 616e 6420 7265  of hashes and re
+00007410: 7475 726e 7320 6120 6465 7461 696c 6564  turns a detailed
+00007420: 2061 6e61 6c79 7369 7320 7265 706f 7274   analysis report
+00007430: 2066 6f72 2074 6865 2073 656c 6563 7465   for the selecte
+00007440: 6420 7361 6d70 6c65 732e 0a20 2020 2020  d samples..     
+00007450: 2020 2054 6869 7320 6d65 7468 6f64 2075     This method u
+00007460: 7469 6c69 7a65 7320 7468 6520 7365 7420  tilizes the set 
+00007470: 6e75 6d62 6572 206f 6620 7265 7472 6965  number of retrie
+00007480: 7320 616e 6420 7761 6974 2074 696d 6520  s and wait time 
+00007490: 696e 2073 6563 6f6e 6473 2061 6e64 2074  in seconds and t
+000074a0: 696d 6573 206f 7574 2069 6620 7468 650a  imes out if the.
+000074b0: 2020 2020 2020 2020 616e 616c 7973 6973          analysis
+000074c0: 2072 6573 756c 7473 2061 7265 206e 6f74   results are not
+000074d0: 2072 6561 6479 2e0a 2020 2020 2020 2020   ready..        
+000074e0: 2020 2020 3a70 6172 616d 2073 616d 706c      :param sampl
+000074f0: 655f 6861 7368 6573 3a20 6861 7368 2073  e_hashes: hash s
+00007500: 7472 696e 6720 6f72 206c 6973 7420 6f66  tring or list of
+00007510: 2068 6173 6820 7374 7269 6e67 730a 2020   hash strings.  
+00007520: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00007530: 7361 6d70 6c65 5f68 6173 6865 733a 2073  sample_hashes: s
+00007540: 7472 206f 7220 6c69 7374 5b73 7472 5d0a  tr or list[str].
+00007550: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00007560: 616d 2072 6574 7279 3a20 6966 2073 6574  am retry: if set
+00007570: 2074 6f20 4661 6c73 6520 7468 6572 6520   to False there 
+00007580: 7769 6c6c 206f 6e6c 7920 6265 206f 6e65  will only be one
+00007590: 2074 7279 2061 7420 6f62 7461 696e 696e   try at obtainin
+000075a0: 6720 7468 6520 616e 616c 7973 6973 2072  g the analysis r
+000075b0: 6570 6f72 740a 2020 2020 2020 2020 2020  eport.          
+000075c0: 2020 3a74 7970 6520 7265 7472 793a 2062    :type retry: b
+000075d0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+000075e0: 3a70 6172 616d 2066 6965 6c64 733a 206c  :param fields: l
+000075f0: 6973 7420 6f66 2041 3130 3030 2072 6570  ist of A1000 rep
+00007600: 6f72 7420 2766 6965 6c64 7327 2074 6f20  ort 'fields' to 
+00007610: 7175 6572 790a 2020 2020 2020 2020 2020  query.          
+00007620: 2020 3a74 7970 6520 6669 656c 6473 3a20    :type fields: 
+00007630: 6c69 7374 5b73 7472 5d0a 2020 2020 2020  list[str].      
+00007640: 2020 2020 2020 3a70 6172 616d 2073 6b69        :param ski
+00007650: 705f 7265 616e 616c 7973 6973 3a20 736b  p_reanalysis: sk
+00007660: 6970 2073 616d 706c 6520 7265 616e 616c  ip sample reanal
+00007670: 7973 6973 2077 6865 6e20 6665 7463 6869  ysis when fetchi
+00007680: 6e67 2074 6865 2073 756d 6d61 7279 2072  ng the summary r
+00007690: 6570 6f72 740a 2020 2020 2020 2020 2020  eport.          
+000076a0: 2020 3a74 7970 6520 736b 6970 5f72 6561    :type skip_rea
+000076b0: 6e61 6c79 7369 733a 2062 6f6f 6c0a 2020  nalysis: bool.  
+000076c0: 2020 2020 2020 2020 2020 3a72 6574 7572            :retur
+000076d0: 6e3a 203a 636c 6173 733a 6052 6573 706f  n: :class:`Respo
+000076e0: 6e73 6520 3c52 6573 706f 6e73 653e 6020  nse <Response>` 
+000076f0: 6f62 6a65 6374 0a20 2020 2020 2020 2020  object.         
+00007700: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
+00007710: 7374 732e 5265 7370 6f6e 7365 0a20 2020  sts.Response.   
+00007720: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007730: 2069 6620 6669 656c 6473 2061 6e64 206e   if fields and n
+00007740: 6f74 2069 7369 6e73 7461 6e63 6528 6669  ot isinstance(fi
+00007750: 656c 6473 2c20 6c69 7374 293a 0a20 2020  elds, list):.   
+00007760: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+00007770: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+00007780: 6669 656c 6473 2070 6172 616d 6574 6572  fields parameter
+00007790: 206d 7573 7420 6265 2061 206c 6973 7420   must be a list 
+000077a0: 6f66 2073 7472 696e 6773 2e22 290a 0a20  of strings.").. 
+000077b0: 2020 2020 2020 2069 6620 7265 7472 7920         if retry 
+000077c0: 6e6f 7420 696e 2028 5472 7565 2c20 4661  not in (True, Fa
+000077d0: 6c73 6529 3a0a 2020 2020 2020 2020 2020  lse):.          
+000077e0: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+000077f0: 7574 4572 726f 7228 2272 6574 7279 2070  utError("retry p
+00007800: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+00007810: 2062 6f6f 6c65 616e 2e22 290a 0a20 2020   boolean.")..   
+00007820: 2020 2020 2069 6620 736b 6970 5f72 6561       if skip_rea
+00007830: 6e61 6c79 7369 7320 6e6f 7420 696e 2028  nalysis not in (
+00007840: 5472 7565 2c20 4661 6c73 6529 3a0a 2020  True, False):.  
+00007850: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00007860: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
+00007870: 2273 6b69 705f 7265 616e 616c 7973 6973  "skip_reanalysis
+00007880: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
+00007890: 6265 2062 6f6f 6c65 616e 2e22 290a 0a20  be boolean.").. 
+000078a0: 2020 2020 2020 2069 6620 6e6f 7420 6669         if not fi
+000078b0: 656c 6473 3a0a 2020 2020 2020 2020 2020  elds:.          
+000078c0: 2020 6669 656c 6473 203d 2073 656c 662e    fields = self.
+000078d0: 5f66 6965 6c64 735f 7632 0a0a 2020 2020  _fields_v2..    
+000078e0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000078f0: 6528 7361 6d70 6c65 5f68 6173 6865 732c  e(sample_hashes,
+00007900: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+00007910: 2020 2073 616d 706c 655f 6861 7368 6573     sample_hashes
+00007920: 203d 205b 7361 6d70 6c65 5f68 6173 6865   = [sample_hashe
+00007930: 735d 0a0a 2020 2020 2020 2020 7661 6c69  s]..        vali
+00007940: 6461 7465 5f68 6173 6865 7328 0a20 2020  date_hashes(.   
+00007950: 2020 2020 2020 2020 2068 6173 685f 696e           hash_in
+00007960: 7075 743d 7361 6d70 6c65 5f68 6173 6865  put=sample_hashe
+00007970: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
+00007980: 6c6c 6f77 6564 5f68 6173 685f 7479 7065  llowed_hash_type
+00007990: 733d 284d 4435 2c20 5348 4131 2c20 5348  s=(MD5, SHA1, SH
+000079a0: 4132 3536 2c20 5348 4135 3132 290a 2020  A256, SHA512).  
+000079b0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000079c0: 2072 6574 7269 6573 203d 2073 656c 662e   retries = self.
+000079d0: 5f72 6574 7269 6573 2069 6620 7265 7472  _retries if retr
+000079e0: 7920 656c 7365 2030 0a0a 2020 2020 2020  y else 0..      
+000079f0: 2020 616e 616c 7973 6973 5f69 735f 6669    analysis_is_fi
+00007a00: 6e69 7368 6564 203d 2046 616c 7365 0a0a  nished = False..
+00007a10: 2020 2020 2020 2020 666f 7220 6974 6572          for iter
+00007a20: 6174 696f 6e20 696e 2072 616e 6765 2872  ation in range(r
+00007a30: 6574 7269 6573 202b 2031 293a 0a20 2020  etries + 1):.   
+00007a40: 2020 2020 2020 2020 2069 6620 6974 6572           if iter
+00007a50: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
+00007a60: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
+00007a70: 7028 7365 6c66 2e5f 7761 6974 5f74 696d  p(self._wait_tim
+00007a80: 655f 7365 636f 6e64 7329 0a0a 2020 2020  e_seconds)..    
+00007a90: 2020 2020 2020 2020 616e 616c 7973 6973          analysis
+00007aa0: 5f69 735f 6669 6e69 7368 6564 203d 2073  _is_finished = s
+00007ab0: 656c 662e 5f5f 616e 616c 7973 6973 5f69  elf.__analysis_i
+00007ac0: 735f 6669 6e69 7368 6564 2873 616d 706c  s_finished(sampl
+00007ad0: 655f 6861 7368 6573 290a 2020 2020 2020  e_hashes).      
+00007ae0: 2020 2020 2020 6966 2061 6e61 6c79 7369        if analysi
+00007af0: 735f 6973 5f66 696e 6973 6865 643a 0a20  s_is_finished:. 
+00007b00: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00007b10: 7265 616b 0a0a 2020 2020 2020 2020 6966  reak..        if
+00007b20: 206e 6f74 2061 6e61 6c79 7369 735f 6973   not analysis_is
+00007b30: 5f66 696e 6973 6865 643a 0a20 2020 2020  _finished:.     
+00007b40: 2020 2020 2020 2072 6169 7365 2052 6571         raise Req
+00007b50: 7565 7374 5469 6d65 6f75 7445 7272 6f72  uestTimeoutError
+00007b60: 2822 5265 706f 7274 2066 6574 6368 696e  ("Report fetchin
+00007b70: 6720 6174 7465 6d70 7473 2066 696e 6973  g attempts finis
+00007b80: 6865 6420 2d20 5468 6520 616e 616c 7973  hed - The analys
+00007b90: 6973 2072 6570 6f72 7420 6973 2073 7469  is report is sti
+00007ba0: 6c6c 206e 6f74 2072 6561 6479 2022 0a20  ll not ready ". 
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bd0: 2020 2020 2022 6f72 2074 6865 2073 616d       "or the sam
+00007be0: 706c 6520 646f 6573 206e 6f74 2065 7869  ple does not exi
+00007bf0: 7374 206f 6e20 7468 6520 6170 706c 6961  st on the applia
+00007c00: 6e63 652e 2229 0a0a 2020 2020 2020 2020  nce.")..        
+00007c10: 7572 6c20 3d20 7365 6c66 2e5f 7572 6c2e  url = self._url.
+00007c20: 666f 726d 6174 2865 6e64 706f 696e 743d  format(endpoint=
+00007c30: 7365 6c66 2e5f 5f44 4554 4149 4c45 445f  self.__DETAILED_
+00007c40: 5245 504f 5254 5f45 4e44 504f 494e 545f  REPORT_ENDPOINT_
+00007c50: 5632 290a 0a20 2020 2020 2020 2064 6174  V2)..        dat
+00007c60: 6120 3d20 7b0a 2020 2020 2020 2020 2020  a = {.          
+00007c70: 2020 2268 6173 685f 7661 6c75 6573 223a    "hash_values":
+00007c80: 2073 616d 706c 655f 6861 7368 6573 2c0a   sample_hashes,.
+00007c90: 2020 2020 2020 2020 2020 2020 2266 6965              "fie
+00007ca0: 6c64 7322 3a20 6669 656c 6473 2c0a 2020  lds": fields,.  
+00007cb0: 2020 2020 2020 2020 2020 2273 6b69 705f            "skip_
+00007cc0: 7265 616e 616c 7973 6973 223a 2073 7472  reanalysis": str
+00007cd0: 2873 6b69 705f 7265 616e 616c 7973 6973  (skip_reanalysis
+00007ce0: 292e 6c6f 7765 7228 290a 2020 2020 2020  ).lower().      
+00007cf0: 2020 7d0a 0a20 2020 2020 2020 2072 6573    }..        res
+00007d00: 706f 6e73 6520 3d20 7365 6c66 2e5f 5f70  ponse = self.__p
+00007d10: 6f73 745f 7265 7175 6573 7428 7572 6c3d  ost_request(url=
+00007d20: 7572 6c2c 2064 6174 613d 6461 7461 290a  url, data=data).
+00007d30: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00007d40: 7261 6973 655f 6f6e 5f65 7272 6f72 2872  raise_on_error(r
+00007d50: 6573 706f 6e73 6529 0a0a 2020 2020 2020  esponse)..      
+00007d60: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+00007d70: 650a 0a20 2020 2064 6566 2067 6574 5f63  e..    def get_c
+00007d80: 6c61 7373 6966 6963 6174 696f 6e28 7365  lassification(se
+00007d90: 6c66 2c20 7361 6d70 6c65 5f68 6173 682c  lf, sample_hash,
+00007da0: 206c 6f63 616c 5f6f 6e6c 793d 5472 7565   local_only=True
+00007db0: 293a 0a20 2020 2020 2020 2022 2222 5448  ):.        """TH
+00007dc0: 4953 204d 4554 484f 4420 4953 2044 4550  IS METHOD IS DEP
+00007dd0: 5245 4341 5445 442e 0a20 2020 2020 2020  RECATED..       
+00007de0: 2055 7365 2067 6574 5f63 6c61 7373 6966   Use get_classif
+00007df0: 6963 6174 696f 6e5f 7633 2069 6e73 7465  ication_v3 inste
+00007e00: 6164 2e0a 0a20 2020 2020 2020 2047 6574  ad...        Get
+00007e10: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
+00007e20: 666f 7220 6f6e 6520 7361 6d70 6c65 2068  for one sample h
+00007e30: 6173 682e 0a20 2020 2020 2020 2020 2020  ash..           
+00007e40: 203a 7061 7261 6d20 7361 6d70 6c65 5f68   :param sample_h
+00007e50: 6173 683a 2068 6173 6820 7374 7269 6e67  ash: hash string
+00007e60: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
+00007e70: 7065 2073 616d 706c 655f 6861 7368 3a20  pe sample_hash: 
+00007e80: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00007e90: 3a70 6172 616d 206c 6f63 616c 5f6f 6e6c  :param local_onl
+00007ea0: 793a 2072 6574 7572 6e20 6f6e 6c79 206c  y: return only l
+00007eb0: 6f63 616c 2073 616d 706c 6573 0a20 2020  ocal samples.   
+00007ec0: 2020 2020 2020 2020 203a 7479 7065 206c           :type l
+00007ed0: 6f63 616c 5f6f 6e6c 793a 2062 6f6f 6c0a  ocal_only: bool.
+00007ee0: 2020 2020 2020 2020 2020 2020 3a72 6574              :ret
+00007ef0: 7572 6e3a 2072 6573 706f 6e73 650a 2020  urn: response.  
+00007f00: 2020 2020 2020 2020 2020 3a72 7479 7065            :rtype
+00007f10: 3a20 7265 7175 6573 7473 2e52 6573 706f  : requests.Respo
+00007f20: 6e73 650a 2020 2020 2020 2020 2222 220a  nse.        """.
+00007f30: 2020 2020 2020 2020 7761 726e 2822 5468          warn("Th
+00007f40: 6973 206d 6574 686f 6420 6973 2064 6570  is method is dep
+00007f50: 7265 6361 7465 642e 2055 7365 2067 6574  recated. Use get
+00007f60: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
+00007f70: 7633 2069 6e73 7465 6164 2e22 2c20 4465  v3 instead.", De
+00007f80: 7072 6563 6174 696f 6e57 6172 6e69 6e67  precationWarning
+00007f90: 290a 0a20 2020 2020 2020 2076 616c 6964  )..        valid
+00007fa0: 6174 655f 6861 7368 6573 280a 2020 2020  ate_hashes(.    
+00007fb0: 2020 2020 2020 2020 6861 7368 5f69 6e70          hash_inp
+00007fc0: 7574 3d5b 7361 6d70 6c65 5f68 6173 685d  ut=[sample_hash]
+00007fd0: 2c0a 2020 2020 2020 2020 2020 2020 616c  ,.            al
+00007fe0: 6c6f 7765 645f 6861 7368 5f74 7970 6573  lowed_hash_types
+00007ff0: 3d28 4d44 352c 2053 4841 312c 2053 4841  =(MD5, SHA1, SHA
+00008000: 3235 362c 2053 4841 3531 3229 0a20 2020  256, SHA512).   
+00008010: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00008020: 6966 206c 6f63 616c 5f6f 6e6c 7920 6e6f  if local_only no
+00008030: 7420 696e 2028 5472 7565 2c20 4661 6c73  t in (True, Fals
+00008040: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00008050: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
+00008060: 4572 726f 7228 226c 6f63 616c 5f6f 6e6c  Error("local_onl
+00008070: 7920 7061 7261 6d65 7465 7220 6d75 7374  y parameter must
+00008080: 2062 6520 626f 6f6c 6561 6e2e 2229 0a0a   be boolean.")..
+00008090: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
+000080a0: 203d 2073 656c 662e 5f5f 434c 4153 5349   = self.__CLASSI
+000080b0: 4659 5f45 4e44 504f 494e 545f 5632 2e66  FY_ENDPOINT_V2.f
+000080c0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+000080d0: 2020 2068 6173 685f 7661 6c75 653d 7361     hash_value=sa
+000080e0: 6d70 6c65 5f68 6173 682c 0a20 2020 2020  mple_hash,.     
+000080f0: 2020 2020 2020 206c 6f63 616c 6f6e 6c79         localonly
+00008100: 3d69 6e74 286c 6f63 616c 5f6f 6e6c 7929  =int(local_only)
+00008110: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00008120: 2020 2020 7572 6c20 3d20 7365 6c66 2e5f      url = self._
+00008130: 7572 6c2e 666f 726d 6174 2865 6e64 706f  url.format(endpo
+00008140: 696e 743d 656e 6470 6f69 6e74 290a 0a20  int=endpoint).. 
+00008150: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+00008160: 3d20 7365 6c66 2e5f 5f67 6574 5f72 6571  = self.__get_req
+00008170: 7565 7374 2875 726c 3d75 726c 290a 0a20  uest(url=url).. 
+00008180: 2020 2020 2020 2073 656c 662e 5f5f 7261         self.__ra
+00008190: 6973 655f 6f6e 5f65 7272 6f72 2872 6573  ise_on_error(res
+000081a0: 706f 6e73 6529 0a0a 2020 2020 2020 2020  ponse)..        
+000081b0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
+000081c0: 0a20 2020 2064 6566 2067 6574 5f63 6c61  .    def get_cla
+000081d0: 7373 6966 6963 6174 696f 6e5f 7633 2873  ssification_v3(s
+000081e0: 656c 662c 2073 616d 706c 655f 6861 7368  elf, sample_hash
+000081f0: 2c20 6c6f 6361 6c5f 6f6e 6c79 3d46 616c  , local_only=Fal
+00008200: 7365 2c20 6176 5f73 6361 6e6e 6572 733d  se, av_scanners=
+00008210: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
+00008220: 2222 2247 6574 2063 6c61 7373 6966 6963  """Get classific
+00008230: 6174 696f 6e20 666f 7220 6f6e 6520 7361  ation for one sa
+00008240: 6d70 6c65 2e0a 2020 2020 2020 2020 5468  mple..        Th
+00008250: 6520 6465 6661 756c 7420 7661 6c75 6520  e default value 
+00008260: 6f66 206c 6f63 616c 5f6f 6e6c 7920 6973  of local_only is
+00008270: 2046 616c 7365 2c20 7768 6963 682c 2069   False, which, i
+00008280: 6620 6e6f 7420 6368 616e 6765 642c 2077  f not changed, w
+00008290: 696c 6c20 7365 6e64 2061 2072 6571 7565  ill send a reque
+000082a0: 7374 2074 6f20 5469 7461 6e69 756d 436c  st to TitaniumCl
+000082b0: 6f75 6420 746f 0a20 2020 2020 2020 2067  oud to.        g
+000082c0: 6574 2074 6865 2073 616d 706c 652e 2054  et the sample. T
+000082d0: 6865 2061 765f 7363 616e 6e65 7273 2070  he av_scanners p
+000082e0: 6172 616d 6574 6572 2064 6563 6964 6573  arameter decides
+000082f0: 2069 6620 7468 6520 4156 2073 6361 6e6e   if the AV scann
+00008300: 6572 2072 6573 756c 7473 2077 696c 6c20  er results will 
+00008310: 6265 2069 6e63 6c75 6465 6420 696e 2074  be included in t
+00008320: 6865 0a20 2020 2020 2020 2063 6c61 7373  he.        class
+00008330: 6966 6963 6174 696f 6e20 7265 706f 7274  ification report
+00008340: 2e0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
+00008350: 6172 616d 2073 616d 706c 655f 6861 7368  aram sample_hash
+00008360: 3a20 6861 7368 2073 7472 696e 670a 2020  : hash string.  
+00008370: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00008380: 7361 6d70 6c65 5f68 6173 683a 2073 7472  sample_hash: str
+00008390: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+000083a0: 7261 6d20 6c6f 6361 6c5f 6f6e 6c79 3a20  ram local_only: 
+000083b0: 7265 7475 726e 206f 6e6c 7920 6c6f 6361  return only loca
+000083c0: 6c20 7361 6d70 6c65 7320 7769 7468 6f75  l samples withou
+000083d0: 7420 7175 6572 7969 6e67 2054 6974 616e  t querying Titan
+000083e0: 6975 6d43 6c6f 7564 0a20 2020 2020 2020  iumCloud.       
+000083f0: 2020 2020 203a 7479 7065 206c 6f63 616c       :type local
+00008400: 5f6f 6e6c 793a 2062 6f6f 6c0a 2020 2020  _only: bool.    
+00008410: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
+00008420: 765f 7363 616e 6e65 7273 3a20 7265 7475  v_scanners: retu
+00008430: 726e 2041 5620 7363 616e 6e65 7220 7265  rn AV scanner re
+00008440: 7375 6c74 730a 2020 2020 2020 2020 2020  sults.          
+00008450: 2020 3a74 7970 6520 6176 5f73 6361 6e6e    :type av_scann
+00008460: 6572 733a 2062 6f6f 6c0a 2020 2020 2020  ers: bool.      
+00008470: 2020 2020 2020 3a72 6574 7572 6e3a 2072        :return: r
+00008480: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
+00008490: 2020 2020 3a72 7479 7065 3a20 7265 7175      :rtype: requ
+000084a0: 6573 7473 2e52 6573 706f 6e73 650a 2020  ests.Response.  
+000084b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000084c0: 2020 7661 6c69 6461 7465 5f68 6173 6865    validate_hashe
+000084d0: 7328 0a20 2020 2020 2020 2020 2020 2068  s(.            h
+000084e0: 6173 685f 696e 7075 743d 5b73 616d 706c  ash_input=[sampl
+000084f0: 655f 6861 7368 5d2c 0a20 2020 2020 2020  e_hash],.       
+00008500: 2020 2020 2061 6c6c 6f77 6564 5f68 6173       allowed_has
+00008510: 685f 7479 7065 733d 284d 4435 2c20 5348  h_types=(MD5, SH
+00008520: 4131 2c20 5348 4132 3536 2c20 5348 4135  A1, SHA256, SHA5
+00008530: 3132 290a 2020 2020 2020 2020 290a 0a20  12).        ).. 
+00008540: 2020 2020 2020 2069 6620 6c6f 6361 6c5f         if local_
+00008550: 6f6e 6c79 206e 6f74 2069 6e20 2854 7275  only not in (Tru
+00008560: 652c 2046 616c 7365 293a 0a20 2020 2020  e, False):.     
+00008570: 2020 2020 2020 2072 6169 7365 2057 726f         raise Wro
+00008580: 6e67 496e 7075 7445 7272 6f72 2822 6c6f  ngInputError("lo
+00008590: 6361 6c5f 6f6e 6c79 2070 6172 616d 6574  cal_only paramet
+000085a0: 6572 206d 7573 7420 6265 2062 6f6f 6c65  er must be boole
+000085b0: 616e 2e22 290a 0a20 2020 2020 2020 2069  an.")..        i
+000085c0: 6620 6176 5f73 6361 6e6e 6572 7320 6e6f  f av_scanners no
+000085d0: 7420 696e 2028 5472 7565 2c20 4661 6c73  t in (True, Fals
+000085e0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+000085f0: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
+00008600: 4572 726f 7228 2261 765f 7363 616e 6e65  Error("av_scanne
+00008610: 7273 2070 6172 616d 6574 6572 206d 7573  rs parameter mus
+00008620: 7420 6265 2062 6f6f 6c65 616e 2e22 290a  t be boolean.").
+00008630: 0a20 2020 2020 2020 2069 6620 6c6f 6361  .        if loca
+00008640: 6c5f 6f6e 6c79 2061 6e64 2061 765f 7363  l_only and av_sc
+00008650: 616e 6e65 7273 3a0a 2020 2020 2020 2020  anners:.        
+00008660: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
+00008670: 6e70 7574 4572 726f 7228 226c 6f63 616c  nputError("local
+00008680: 5f6f 6e6c 7920 6d75 7374 2062 6520 4661  _only must be Fa
+00008690: 6c73 6520 6966 2061 765f 7363 616e 6e65  lse if av_scanne
+000086a0: 7273 2061 7265 2075 7365 642e 2229 0a0a  rs are used.")..
+000086b0: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+000086c0: 2022 6c6f 6361 6c6f 6e6c 793d 7b6c 6f63   "localonly={loc
+000086d0: 616c 5f6f 6e6c 797d 2661 765f 7363 616e  al_only}&av_scan
+000086e0: 6e65 7273 3d7b 6176 5f73 6361 6e6e 6572  ners={av_scanner
+000086f0: 737d 222e 666f 726d 6174 280a 2020 2020  s}".format(.    
+00008700: 2020 2020 2020 2020 6c6f 6361 6c5f 6f6e          local_on
+00008710: 6c79 3d73 7472 2869 6e74 286c 6f63 616c  ly=str(int(local
+00008720: 5f6f 6e6c 7929 292c 0a20 2020 2020 2020  _only)),.       
+00008730: 2020 2020 2061 765f 7363 616e 6e65 7273       av_scanners
+00008740: 3d73 7472 2869 6e74 2861 765f 7363 616e  =str(int(av_scan
+00008750: 6e65 7273 2929 0a20 2020 2020 2020 2029  ners)).        )
+00008760: 0a0a 2020 2020 2020 2020 656e 6470 6f69  ..        endpoi
+00008770: 6e74 203d 2022 7b65 6e64 706f 696e 747d  nt = "{endpoint}
+00008780: 3f7b 7061 7261 6d73 7d22 2e66 6f72 6d61  ?{params}".forma
+00008790: 7428 0a20 2020 2020 2020 2020 2020 2065  t(.            e
+000087a0: 6e64 706f 696e 743d 7365 6c66 2e5f 5f43  ndpoint=self.__C
+000087b0: 4c41 5353 4946 595f 454e 4450 4f49 4e54  LASSIFY_ENDPOINT
+000087c0: 5f56 332e 666f 726d 6174 2868 6173 685f  _V3.format(hash_
+000087d0: 7661 6c75 653d 7361 6d70 6c65 5f68 6173  value=sample_has
+000087e0: 6829 2c0a 2020 2020 2020 2020 2020 2020  h),.            
+000087f0: 7061 7261 6d73 3d70 6172 616d 730a 2020  params=params.  
+00008800: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00008810: 2075 726c 203d 2073 656c 662e 5f75 726c   url = self._url
+00008820: 2e66 6f72 6d61 7428 656e 6470 6f69 6e74  .format(endpoint
+00008830: 3d65 6e64 706f 696e 7429 0a0a 2020 2020  =endpoint)..    
+00008840: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+00008850: 656c 662e 5f5f 6765 745f 7265 7175 6573  elf.__get_reques
+00008860: 7428 7572 6c3d 7572 6c29 0a0a 2020 2020  t(url=url)..    
+00008870: 2020 2020 7365 6c66 2e5f 5f72 6169 7365      self.__raise
+00008880: 5f6f 6e5f 6572 726f 7228 7265 7370 6f6e  _on_error(respon
+00008890: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
+000088a0: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+000088b0: 2020 6465 6620 7265 616e 616c 797a 655f    def reanalyze_
+000088c0: 7361 6d70 6c65 7328 7365 6c66 2c20 6861  samples(self, ha
+000088d0: 7368 5f69 6e70 7574 2c20 7469 7461 6e69  sh_input, titani
+000088e0: 756d 5f63 6c6f 7564 3d54 7275 652c 2074  um_cloud=True, t
+000088f0: 6974 616e 6975 6d5f 636f 7265 3d54 7275  itanium_core=Tru
+00008900: 6529 3a0a 2020 2020 2020 2020 2222 2254  e):.        """T
+00008910: 4849 5320 4d45 5448 4f44 2049 5320 4445  HIS METHOD IS DE
+00008920: 5052 4543 4154 4544 2e0a 2020 2020 2020  PRECATED..      
+00008930: 2020 5573 6520 7265 616e 616c 797a 655f    Use reanalyze_
+00008940: 7361 6d70 6c65 735f 7632 2069 6e73 7465  samples_v2 inste
+00008950: 6164 2e0a 0a20 2020 2020 2020 2041 6363  ad...        Acc
+00008960: 6570 7473 2061 2073 696e 676c 6520 6861  epts a single ha
+00008970: 7368 206f 7220 6120 6c69 7374 206f 6620  sh or a list of 
+00008980: 6861 7368 6573 206f 6620 7468 6520 7361  hashes of the sa
+00008990: 6d65 2074 7970 6520 616e 6420 7265 616e  me type and rean
+000089a0: 616c 797a 6573 2074 6865 0a20 2020 2020  alyzes the.     
+000089b0: 2020 2063 6f72 7265 7370 6f6e 6469 6e67     corresponding
+000089c0: 2073 616d 706c 6573 2e0a 2020 2020 2020   samples..      
+000089d0: 2020 2020 2020 3a70 6172 616d 2068 6173        :param has
+000089e0: 685f 696e 7075 743a 2073 696e 676c 6520  h_input: single 
+000089f0: 6861 7368 206f 7220 6120 6c69 7374 206f  hash or a list o
+00008a00: 6620 6861 7368 6573 0a20 2020 2020 2020  f hashes.       
+00008a10: 2020 2020 203a 7479 7065 2068 6173 685f       :type hash_
+00008a20: 696e 7075 743a 2073 7472 206f 7220 6c69  input: str or li
+00008a30: 7374 5b73 7472 5d0a 2020 2020 2020 2020  st[str].        
+00008a40: 2020 2020 3a70 6172 616d 2074 6974 616e      :param titan
+00008a50: 6975 6d5f 636c 6f75 643a 2075 7365 2054  ium_cloud: use T
+00008a60: 6974 616e 6975 6d43 6c6f 7564 0a20 2020  itaniumCloud.   
+00008a70: 2020 2020 2020 2020 203a 7479 7065 2074           :type t
+00008a80: 6974 616e 6975 6d5f 636c 6f75 643a 2062  itanium_cloud: b
+00008a90: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+00008aa0: 3a70 6172 616d 2074 6974 616e 6975 6d5f  :param titanium_
+00008ab0: 636f 7265 3a20 7573 6520 5469 7461 6e69  core: use Titani
+00008ac0: 756d 436f 7265 0a20 2020 2020 2020 2020  umCore.         
+00008ad0: 2020 203a 7479 7065 2074 6974 616e 6975     :type titaniu
+00008ae0: 6d5f 636f 7265 3a20 626f 6f6c 0a20 2020  m_core: bool.   
+00008af0: 2020 2020 2020 2020 203a 7265 7475 726e           :return
+00008b00: 3a20 7265 7370 6f6e 7365 0a20 2020 2020  : response.     
+00008b10: 2020 2020 2020 203a 7274 7970 653a 2072         :rtype: r
+00008b20: 6571 7565 7374 732e 5265 7370 6f6e 7365  equests.Response
+00008b30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00008b40: 2020 2020 2077 6172 6e28 2254 6869 7320       warn("This 
+00008b50: 6d65 7468 6f64 2069 7320 6465 7072 6563  method is deprec
+00008b60: 6174 6564 2e20 5573 6520 7265 616e 616c  ated. Use reanal
+00008b70: 797a 655f 7361 6d70 6c65 735f 7632 2069  yze_samples_v2 i
+00008b80: 6e73 7465 6164 2e22 2c20 4465 7072 6563  nstead.", Deprec
+00008b90: 6174 696f 6e57 6172 6e69 6e67 290a 0a20  ationWarning).. 
+00008ba0: 2020 2020 2020 2069 6620 7469 7461 6e69         if titani
+00008bb0: 756d 5f63 6c6f 7564 206e 6f74 2069 6e20  um_cloud not in 
+00008bc0: 2854 7275 652c 2046 616c 7365 293a 0a20  (True, False):. 
+00008bd0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00008be0: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
+00008bf0: 2822 7469 7461 6e69 756d 5f63 6c6f 7564  ("titanium_cloud
+00008c00: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
+00008c10: 6265 2062 6f6f 6c65 616e 2e22 290a 0a20  be boolean.").. 
+00008c20: 2020 2020 2020 2069 6620 7469 7461 6e69         if titani
+00008c30: 756d 5f63 6f72 6520 6e6f 7420 696e 2028  um_core not in (
+00008c40: 5472 7565 2c20 4661 6c73 6529 3a0a 2020  True, False):.  
+00008c50: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00008c60: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
+00008c70: 2274 6974 616e 6975 6d5f 636f 7265 2070  "titanium_core p
+00008c80: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+00008c90: 2062 6f6f 6c65 616e 2e22 290a 0a20 2020   boolean.")..   
+00008ca0: 2020 2020 2070 6172 616d 6574 6572 5f64       parameter_d
+00008cb0: 6963 7420 3d20 7b27 636f 7265 273a 2074  ict = {'core': t
+00008cc0: 6974 616e 6975 6d5f 636f 7265 2c20 2763  itanium_core, 'c
+00008cd0: 6c6f 7564 273a 2074 6974 616e 6975 6d5f  loud': titanium_
+00008ce0: 636c 6f75 647d 0a0a 2020 2020 2020 2020  cloud}..        
+00008cf0: 616e 616c 7973 6973 5f6c 6973 7420 3d20  analysis_list = 
+00008d00: 5b6b 6579 2066 6f72 206b 6579 2c20 7661  [key for key, va
+00008d10: 6c75 6520 696e 2070 6172 616d 6574 6572  lue in parameter
+00008d20: 5f64 6963 742e 6974 656d 7328 2920 6966  _dict.items() if
+00008d30: 2076 616c 7565 5d0a 0a20 2020 2020 2020   value]..       
+00008d40: 2069 6620 6c65 6e28 616e 616c 7973 6973   if len(analysis
+00008d50: 5f6c 6973 7429 203d 3d20 303a 0a20 2020  _list) == 0:.   
+00008d60: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+00008d70: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+00008d80: 4174 206c 6561 7374 206f 6e65 206f 6620  At least one of 
+00008d90: 7468 6520 666f 6c6c 6f77 696e 6720 7061  the following pa
+00008da0: 7261 6d65 7465 7273 206e 6565 6473 2074  rameters needs t
+00008db0: 6f20 6265 2065 6e61 626c 6564 3a20 220a  o be enabled: ".
+00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008de0: 2020 2274 6974 616e 6975 6d5f 636c 6f75    "titanium_clou
+00008df0: 642c 2074 6974 616e 6975 6d5f 636f 7265  d, titanium_core
+00008e00: 2e22 290a 0a20 2020 2020 2020 2061 6e61  .")..        ana
+00008e10: 6c79 7369 735f 7479 7065 203d 2022 2c22  lysis_type = ","
+00008e20: 2e6a 6f69 6e28 616e 616c 7973 6973 5f6c  .join(analysis_l
+00008e30: 6973 7429 0a0a 2020 2020 2020 2020 6966  ist)..        if
+00008e40: 2069 7369 6e73 7461 6e63 6528 6861 7368   isinstance(hash
+00008e50: 5f69 6e70 7574 2c20 7374 7229 3a0a 2020  _input, str):.  
+00008e60: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
+00008e70: 7465 5f68 6173 6865 7328 0a20 2020 2020  te_hashes(.     
+00008e80: 2020 2020 2020 2020 2020 2068 6173 685f             hash_
+00008e90: 696e 7075 743d 5b68 6173 685f 696e 7075  input=[hash_inpu
+00008ea0: 745d 2c0a 2020 2020 2020 2020 2020 2020  t],.            
+00008eb0: 2020 2020 616c 6c6f 7765 645f 6861 7368      allowed_hash
+00008ec0: 5f74 7970 6573 3d28 4d44 352c 2053 4841  _types=(MD5, SHA
+00008ed0: 312c 2053 4841 3235 362c 2053 4841 3531  1, SHA256, SHA51
+00008ee0: 3229 0a20 2020 2020 2020 2020 2020 2029  2).            )
+00008ef0: 0a0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+00008f00: 6470 6f69 6e74 203d 2073 656c 662e 5f5f  dpoint = self.__
+00008f10: 5245 414e 414c 595a 455f 454e 4450 4f49  REANALYZE_ENDPOI
+00008f20: 4e54 2e66 6f72 6d61 7428 6861 7368 5f76  NT.format(hash_v
+00008f30: 616c 7565 3d68 6173 685f 696e 7075 7429  alue=hash_input)
+00008f40: 0a0a 2020 2020 2020 2020 2020 2020 7572  ..            ur
+00008f50: 6c20 3d20 7365 6c66 2e5f 7572 6c2e 666f  l = self._url.fo
+00008f60: 726d 6174 2865 6e64 706f 696e 743d 656e  rmat(endpoint=en
+00008f70: 6470 6f69 6e74 290a 0a20 2020 2020 2020  dpoint)..       
+00008f80: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+00008f90: 7365 6c66 2e5f 5f70 6f73 745f 7265 7175  self.__post_requ
+00008fa0: 6573 7428 7572 6c3d 7572 6c2c 2064 6174  est(url=url, dat
+00008fb0: 613d 7b22 616e 616c 7973 6973 223a 2061  a={"analysis": a
+00008fc0: 6e61 6c79 7369 735f 7479 7065 7d29 0a0a  nalysis_type})..
+00008fd0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00008fe0: 6e73 7461 6e63 6528 6861 7368 5f69 6e70  nstance(hash_inp
+00008ff0: 7574 2c20 6c69 7374 293a 0a20 2020 2020  ut, list):.     
+00009000: 2020 2020 2020 2076 616c 6964 6174 655f         validate_
+00009010: 6861 7368 6573 280a 2020 2020 2020 2020  hashes(.        
+00009020: 2020 2020 2020 2020 6861 7368 5f69 6e70          hash_inp
+00009030: 7574 3d68 6173 685f 696e 7075 742c 0a20  ut=hash_input,. 
+00009040: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00009050: 6c6c 6f77 6564 5f68 6173 685f 7479 7065  llowed_hash_type
+00009060: 733d 284d 4435 2c20 5348 4131 2c20 5348  s=(MD5, SHA1, SH
+00009070: 4132 3536 2c20 5348 4135 3132 290a 2020  A256, SHA512).  
+00009080: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00009090: 2020 2020 2020 2020 2075 726c 203d 2073           url = s
+000090a0: 656c 662e 5f75 726c 2e66 6f72 6d61 7428  elf._url.format(
+000090b0: 656e 6470 6f69 6e74 3d73 656c 662e 5f5f  endpoint=self.__
+000090c0: 5245 414e 414c 595a 455f 4255 4c4b 5f45  REANALYZE_BULK_E
+000090d0: 4e44 504f 494e 5429 0a0a 2020 2020 2020  NDPOINT)..      
+000090e0: 2020 2020 2020 6461 7461 203d 207b 2268        data = {"h
+000090f0: 6173 685f 7661 6c75 6522 3a20 6861 7368  ash_value": hash
+00009100: 5f69 6e70 7574 2c20 2261 6e61 6c79 7369  _input, "analysi
+00009110: 7322 3a20 616e 616c 7973 6973 5f74 7970  s": analysis_typ
+00009120: 657d 0a0a 2020 2020 2020 2020 2020 2020  e}..            
+00009130: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00009140: 5f5f 706f 7374 5f72 6571 7565 7374 2875  __post_request(u
+00009150: 726c 3d75 726c 2c20 6461 7461 3d64 6174  rl=url, data=dat
+00009160: 6129 0a0a 2020 2020 2020 2020 656c 7365  a)..        else
+00009170: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00009180: 6973 6520 5772 6f6e 6749 6e70 7574 4572  ise WrongInputEr
+00009190: 726f 7228 2268 6173 685f 696e 7075 7420  ror("hash_input 
+000091a0: 7061 7261 6d65 7465 7220 6361 6e20 6f6e  parameter can on
+000091b0: 6c79 2062 6520 6120 7369 6e67 6c65 2068  ly be a single h
+000091c0: 6173 6820 7374 7269 6e67 206f 7220 220a  ash string or ".
+000091d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091f0: 2020 2261 206c 6973 7420 6f66 2068 6173    "a list of has
+00009200: 6820 7374 7269 6e67 7320 6f66 2074 6865  h strings of the
+00009210: 2073 616d 6520 7479 7065 2e22 290a 0a20   same type.").. 
+00009220: 2020 2020 2020 2073 656c 662e 5f5f 7261         self.__ra
+00009230: 6973 655f 6f6e 5f65 7272 6f72 2872 6573  ise_on_error(res
+00009240: 706f 6e73 6529 0a0a 2020 2020 2020 2020  ponse)..        
+00009250: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
+00009260: 0a20 2020 2064 6566 2072 6561 6e61 6c79  .    def reanaly
+00009270: 7a65 5f73 616d 706c 6573 5f76 3228 7365  ze_samples_v2(se
+00009280: 6c66 2c20 6861 7368 5f69 6e70 7574 2c20  lf, hash_input, 
+00009290: 7469 7461 6e69 756d 5f63 6c6f 7564 3d46  titanium_cloud=F
+000092a0: 616c 7365 2c20 7469 7461 6e69 756d 5f63  alse, titanium_c
+000092b0: 6f72 653d 4661 6c73 652c 2072 6c5f 636c  ore=False, rl_cl
+000092c0: 6f75 645f 7361 6e64 626f 783d 4661 6c73  oud_sandbox=Fals
+000092d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092f0: 6375 636b 6f6f 5f73 616e 6462 6f78 3d46  cuckoo_sandbox=F
+00009300: 616c 7365 2c20 6669 7265 6579 653d 4661  alse, fireeye=Fa
+00009310: 6c73 652c 206a 6f65 5f73 616e 6462 6f78  lse, joe_sandbox
+00009320: 3d46 616c 7365 2c20 6361 7065 3d46 616c  =False, cape=Fal
+00009330: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009350: 2072 6c5f 636c 6f75 645f 7361 6e64 626f   rl_cloud_sandbo
+00009360: 785f 706c 6174 666f 726d 3d4e 6f6e 6529  x_platform=None)
+00009370: 3a0a 2020 2020 2020 2020 2222 2241 6363  :.        """Acc
+00009380: 6570 7473 2061 2073 696e 676c 6520 6861  epts a single ha
+00009390: 7368 206f 7220 6120 6c69 7374 206f 6620  sh or a list of 
+000093a0: 6861 7368 6573 206f 6620 7661 7269 6f75  hashes of variou
+000093b0: 7320 7479 7065 7320 616e 6420 7265 616e  s types and rean
+000093c0: 616c 797a 6573 2074 6865 2063 6f72 7265  alyzes the corre
+000093d0: 7370 6f6e 6469 6e67 2073 616d 706c 6528  sponding sample(
+000093e0: 7329 2e0a 2020 2020 2020 2020 5468 6973  s)..        This
+000093f0: 206d 6574 686f 6420 6361 6e20 6265 2075   method can be u
+00009400: 7365 6420 666f 7220 7265 616e 616c 797a  sed for reanalyz
+00009410: 696e 6720 6120 7369 6e67 6c65 2073 616d  ing a single sam
+00009420: 706c 6520 6f72 2061 2062 6174 6368 206f  ple or a batch o
+00009430: 6620 7361 6d70 6c65 732c 2064 6570 656e  f samples, depen
+00009440: 6469 6e67 206f 6e20 7468 6520 6461 7461  ding on the data
+00009450: 2074 7970 650a 2020 2020 2020 2020 7061   type.        pa
+00009460: 7373 6564 2e0a 2020 2020 2020 2020 4154  ssed..        AT
+00009470: 206c 6561 7374 206f 6e65 2061 6e61 6c79   least one analy
+00009480: 7369 7320 7479 7065 206d 7573 7420 6265  sis type must be
+00009490: 2075 7365 6420 2873 6574 2074 6f20 5472   used (set to Tr
+000094a0: 7565 292e 0a20 2020 2020 2020 2049 6620  ue)..        If 
+000094b0: 726c 5f63 6c6f 7564 5f73 616e 6462 6f78  rl_cloud_sandbox
+000094c0: 2069 7320 7573 6564 2061 7320 616e 2061   is used as an a
+000094d0: 6e61 6c79 7369 7320 7479 7065 2c20 726c  nalysis type, rl
+000094e0: 5f63 6c6f 7564 5f73 616e 6462 6f78 5f70  _cloud_sandbox_p
+000094f0: 6c61 7466 6f72 6d20 6d75 7374 2062 6520  latform must be 
+00009500: 6465 6669 6e65 642e 0a20 2020 2020 2020  defined..       
+00009510: 2020 2020 203a 7061 7261 6d20 6861 7368       :param hash
+00009520: 5f69 6e70 7574 3a20 7369 6e67 6c65 2068  _input: single h
+00009530: 6173 6820 6f72 2061 206c 6973 7420 6f66  ash or a list of
+00009540: 2068 6173 6865 730a 2020 2020 2020 2020   hashes.        
+00009550: 2020 2020 3a74 7970 6520 6861 7368 5f69      :type hash_i
+00009560: 6e70 7574 3a20 7374 7220 6f72 206c 6973  nput: str or lis
+00009570: 745b 7374 725d 0a20 2020 2020 2020 2020  t[str].         
+00009580: 2020 203a 7061 7261 6d20 7469 7461 6e69     :param titani
+00009590: 756d 5f63 6c6f 7564 3a20 7573 6520 5469  um_cloud: use Ti
+000095a0: 7461 6e69 756d 436c 6f75 640a 2020 2020  taniumCloud.    
+000095b0: 2020 2020 2020 2020 3a74 7970 6520 7469          :type ti
+000095c0: 7461 6e69 756d 5f63 6c6f 7564 3a20 626f  tanium_cloud: bo
+000095d0: 6f6c 0a20 2020 2020 2020 2020 2020 203a  ol.            :
+000095e0: 7061 7261 6d20 7469 7461 6e69 756d 5f63  param titanium_c
+000095f0: 6f72 653a 2075 7365 2054 6974 616e 6975  ore: use Titaniu
+00009600: 6d43 6f72 650a 2020 2020 2020 2020 2020  mCore.          
+00009610: 2020 3a74 7970 6520 7469 7461 6e69 756d    :type titanium
+00009620: 5f63 6f72 653a 2062 6f6f 6c0a 2020 2020  _core: bool.    
+00009630: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
+00009640: 6c5f 636c 6f75 645f 7361 6e64 626f 783a  l_cloud_sandbox:
+00009650: 2075 7365 2052 4c20 636c 6f75 6420 7361   use RL cloud sa
+00009660: 6e64 626f 780a 2020 2020 2020 2020 2020  ndbox.          
+00009670: 2020 3a74 7970 6520 726c 5f63 6c6f 7564    :type rl_cloud
+00009680: 5f73 616e 6462 6f78 3a20 626f 6f6c 0a20  _sandbox: bool. 
+00009690: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+000096a0: 6d20 6375 636b 6f6f 5f73 616e 6462 6f78  m cuckoo_sandbox
+000096b0: 3a20 7573 6520 4375 636b 6f6f 2073 616e  : use Cuckoo san
+000096c0: 6462 6f78 0a20 2020 2020 2020 2020 2020  dbox.           
+000096d0: 203a 7479 7065 2063 7563 6b6f 6f5f 7361   :type cuckoo_sa
+000096e0: 6e64 626f 783a 2062 6f6f 6c0a 2020 2020  ndbox: bool.    
+000096f0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
+00009700: 6972 6565 7965 3a20 7573 6520 4669 7265  ireeye: use Fire
+00009710: 4579 650a 2020 2020 2020 2020 2020 2020  Eye.            
+00009720: 3a74 7970 6520 6669 7265 6579 653a 2062  :type fireeye: b
+00009730: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+00009740: 3a70 6172 616d 206a 6f65 5f73 616e 6462  :param joe_sandb
+00009750: 6f78 3a20 7573 6520 4a6f 6520 7361 6e64  ox: use Joe sand
+00009760: 626f 780a 2020 2020 2020 2020 2020 2020  box.            
+00009770: 3a74 7970 6520 6a6f 655f 7361 6e64 626f  :type joe_sandbo
+00009780: 783a 2062 6f6f 6c0a 2020 2020 2020 2020  x: bool.        
+00009790: 2020 2020 3a70 6172 616d 2063 6170 653a      :param cape:
+000097a0: 2075 7365 2043 6170 650a 2020 2020 2020   use Cape.      
+000097b0: 2020 2020 2020 3a74 7970 6520 6361 7065        :type cape
+000097c0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+000097d0: 2020 203a 7061 7261 6d20 726c 5f63 6c6f     :param rl_clo
+000097e0: 7564 5f73 616e 6462 6f78 5f70 6c61 7466  ud_sandbox_platf
+000097f0: 6f72 6d3a 2064 6573 6972 6564 2070 6c61  orm: desired pla
+00009800: 7466 6f72 6d20 6f6e 2077 6869 6368 2074  tform on which t
+00009810: 6865 2073 616d 706c 6520 7769 6c6c 2062  he sample will b
+00009820: 6520 6465 746f 6e61 7465 643b 0a20 2020  e detonated;.   
+00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009850: 2020 2020 2020 2020 2073 6565 2052 6576           see Rev
+00009860: 6572 7369 6e67 4c61 6273 2e53 444b 2e68  ersingLabs.SDK.h
+00009870: 656c 7065 722e 4156 4149 4c41 424c 4520  elper.AVAILABLE 
+00009880: 504c 4154 464f 524d 5320 666f 7220 6f70  PLATFORMS for op
+00009890: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+000098a0: 2020 3a74 7970 6520 726c 5f63 6c6f 7564    :type rl_cloud
+000098b0: 5f73 616e 6462 6f78 5f70 6c61 7466 6f72  _sandbox_platfor
+000098c0: 6d3a 2073 7472 0a20 2020 2020 2020 2020  m: str.         
+000098d0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
+000098e0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
+000098f0: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
+00009900: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
+00009910: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00009920: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00009930: 2868 6173 685f 696e 7075 742c 206c 6973  (hash_input, lis
+00009940: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00009950: 6861 7368 5f69 6e70 7574 203d 205b 6861  hash_input = [ha
+00009960: 7368 5f69 6e70 7574 5d0a 0a20 2020 2020  sh_input]..     
+00009970: 2020 2076 616c 6964 6174 655f 6861 7368     validate_hash
+00009980: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+00009990: 6861 7368 5f69 6e70 7574 3d68 6173 685f  hash_input=hash_
+000099a0: 696e 7075 742c 0a20 2020 2020 2020 2020  input,.         
+000099b0: 2020 2061 6c6c 6f77 6564 5f68 6173 685f     allowed_hash_
+000099c0: 7479 7065 733d 284d 4435 2c20 5348 4131  types=(MD5, SHA1
+000099d0: 2c20 5348 4132 3536 2c20 5348 4135 3132  , SHA256, SHA512
+000099e0: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+000099f0: 2020 2020 2061 6e61 6c79 7369 735f 7479       analysis_ty
+00009a00: 7065 5f64 6963 7420 3d20 7b22 636c 6f75  pe_dict = {"clou
+00009a10: 6422 3a20 7469 7461 6e69 756d 5f63 6c6f  d": titanium_clo
+00009a20: 7564 2c20 2263 6f72 6522 3a20 7469 7461  ud, "core": tita
+00009a30: 6e69 756d 5f63 6f72 652c 2022 726c 5f63  nium_core, "rl_c
+00009a40: 6c6f 7564 5f73 616e 6462 6f78 223a 2072  loud_sandbox": r
+00009a50: 6c5f 636c 6f75 645f 7361 6e64 626f 782c  l_cloud_sandbox,
+00009a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00009a80: 6375 636b 6f6f 223a 2063 7563 6b6f 6f5f  cuckoo": cuckoo_
+00009a90: 7361 6e64 626f 782c 2022 6669 7265 6579  sandbox, "fireey
+00009aa0: 6522 3a20 6669 7265 6579 652c 2022 6a6f  e": fireeye, "jo
+00009ab0: 6522 3a20 6a6f 655f 7361 6e64 626f 782c  e": joe_sandbox,
+00009ac0: 2022 6361 7065 223a 2063 6170 657d 0a0a   "cape": cape}..
+00009ad0: 2020 2020 2020 2020 6966 206e 6f74 2061          if not a
+00009ae0: 6c6c 2869 7369 6e73 7461 6e63 6528 616e  ll(isinstance(an
+00009af0: 616c 7973 6973 5f74 7970 652c 2062 6f6f  alysis_type, boo
+00009b00: 6c29 2066 6f72 2061 6e61 6c79 7369 735f  l) for analysis_
+00009b10: 7479 7065 2069 6e20 616e 616c 7973 6973  type in analysis
+00009b20: 5f74 7970 655f 6469 6374 2e76 616c 7565  _type_dict.value
+00009b30: 7328 2929 3a0a 2020 2020 2020 2020 2020  s()):.          
+00009b40: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+00009b50: 7574 4572 726f 7228 2241 6c6c 2061 6e61  utError("All ana
+00009b60: 6c79 7369 7320 7479 7065 2070 6172 616d  lysis type param
+00009b70: 6574 6572 7320 6d75 7374 2062 6520 626f  eters must be bo
+00009b80: 6f6c 6561 6e2e 2229 0a0a 2020 2020 2020  olean.")..      
+00009b90: 2020 6966 2072 6c5f 636c 6f75 645f 7361    if rl_cloud_sa
+00009ba0: 6e64 626f 7820 616e 6420 726c 5f63 6c6f  ndbox and rl_clo
+00009bb0: 7564 5f73 616e 6462 6f78 5f70 6c61 7466  ud_sandbox_platf
+00009bc0: 6f72 6d20 6e6f 7420 696e 2041 5641 494c  orm not in AVAIL
+00009bd0: 4142 4c45 5f50 4c41 5446 4f52 4d53 3a0a  ABLE_PLATFORMS:.
+00009be0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00009bf0: 6520 5772 6f6e 6749 6e70 7574 4572 726f  e WrongInputErro
+00009c00: 7228 2269 6620 726c 5f63 6c6f 7564 5f73  r("if rl_cloud_s
+00009c10: 616e 6462 6f78 2069 7320 7573 6564 2c20  andbox is used, 
+00009c20: 726c 5f63 6c6f 7564 5f73 616e 6462 6f78  rl_cloud_sandbox
+00009c30: 5f70 6c61 7466 6f72 6d20 7061 7261 6d65  _platform parame
+00009c40: 7465 7220 6d75 7374 2062 6520 6f6e 6520  ter must be one 
+00009c50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c70: 2020 2020 226f 6620 7468 6520 666f 6c6c      "of the foll
+00009c80: 6f77 696e 6720 7661 6c75 6573 3a20 7b70  owing values: {p
+00009c90: 6c61 7466 6f72 6d73 7d22 2e66 6f72 6d61  latforms}".forma
+00009ca0: 7428 706c 6174 666f 726d 733d 4156 4149  t(platforms=AVAI
+00009cb0: 4c41 424c 455f 504c 4154 464f 524d 5329  LABLE_PLATFORMS)
+00009cc0: 290a 0a20 2020 2020 2020 2061 6e61 6c79  )..        analy
+00009cd0: 7369 735f 6c69 7374 203d 205b 6b65 7920  sis_list = [key 
+00009ce0: 666f 7220 6b65 792c 2076 616c 7565 2069  for key, value i
+00009cf0: 6e20 616e 616c 7973 6973 5f74 7970 655f  n analysis_type_
+00009d00: 6469 6374 2e69 7465 6d73 2829 2069 6620  dict.items() if 
+00009d10: 7661 6c75 655d 0a0a 2020 2020 2020 2020  value]..        
+00009d20: 6966 206e 6f74 2061 6e61 6c79 7369 735f  if not analysis_
+00009d30: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
+00009d40: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+00009d50: 7574 4572 726f 7228 2241 7420 6c65 6173  utError("At leas
+00009d60: 7420 6f6e 6520 616e 616c 7973 6973 2074  t one analysis t
+00009d70: 7970 6520 7061 7261 6d65 7465 7220 6e65  ype parameter ne
+00009d80: 6564 7320 746f 2062 6520 6465 6669 6e65  eds to be define
+00009d90: 642e 2229 0a0a 2020 2020 2020 2020 616e  d.")..        an
+00009da0: 616c 7973 6973 5f74 7970 6573 203d 2022  alysis_types = "
+00009db0: 2c22 2e6a 6f69 6e28 616e 616c 7973 6973  ,".join(analysis
+00009dc0: 5f6c 6973 7429 0a0a 2020 2020 2020 2020  _list)..        
+00009dd0: 7572 6c20 3d20 7365 6c66 2e5f 7572 6c2e  url = self._url.
+00009de0: 666f 726d 6174 2865 6e64 706f 696e 743d  format(endpoint=
+00009df0: 7365 6c66 2e5f 5f52 4541 4e41 4c59 5a45  self.__REANALYZE
+00009e00: 5f42 554c 4b5f 454e 4450 4f49 4e54 5f56  _BULK_ENDPOINT_V
+00009e10: 3229 0a0a 2020 2020 2020 2020 6461 7461  2)..        data
+00009e20: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00009e30: 2022 6861 7368 5f76 616c 7565 223a 2068   "hash_value": h
+00009e40: 6173 685f 696e 7075 742c 0a20 2020 2020  ash_input,.     
+00009e50: 2020 2020 2020 2022 616e 616c 7973 6973         "analysis
+00009e60: 223a 2061 6e61 6c79 7369 735f 7479 7065  ": analysis_type
+00009e70: 732c 0a20 2020 2020 2020 2020 2020 2022  s,.            "
+00009e80: 726c 5f63 6c6f 7564 5f73 616e 6462 6f78  rl_cloud_sandbox
+00009e90: 5f70 6c61 7466 6f72 6d22 3a20 726c 5f63  _platform": rl_c
+00009ea0: 6c6f 7564 5f73 616e 6462 6f78 5f70 6c61  loud_sandbox_pla
+00009eb0: 7466 6f72 6d0a 2020 2020 2020 2020 7d0a  tform.        }.
+00009ec0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00009ed0: 6520 3d20 7365 6c66 2e5f 5f70 6f73 745f  e = self.__post_
+00009ee0: 7265 7175 6573 7428 7572 6c3d 7572 6c2c  request(url=url,
+00009ef0: 2064 6174 613d 6461 7461 290a 0a20 2020   data=data)..   
+00009f00: 2020 2020 2073 656c 662e 5f5f 7261 6973       self.__rais
+00009f10: 655f 6f6e 5f65 7272 6f72 2872 6573 706f  e_on_error(respo
+00009f20: 6e73 6529 0a0a 2020 2020 2020 2020 7265  nse)..        re
+00009f30: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+00009f40: 2020 2064 6566 2067 6574 5f65 7874 7261     def get_extra
+00009f50: 6374 6564 5f66 696c 6573 2873 656c 662c  cted_files(self,
+00009f60: 2073 616d 706c 655f 6861 7368 2c20 7061   sample_hash, pa
+00009f70: 6765 5f73 697a 653d 4e6f 6e65 2c20 7061  ge_size=None, pa
+00009f80: 6765 3d4e 6f6e 6529 3a0a 2020 2020 2020  ge=None):.      
+00009f90: 2020 2222 2254 4849 5320 4d45 5448 4f44    """THIS METHOD
+00009fa0: 2049 5320 4445 5052 4543 4154 4544 2e20   IS DEPRECATED. 
+00009fb0: 5573 6520 6c69 7374 5f65 7874 7261 6374  Use list_extract
+00009fc0: 6564 5f66 696c 6573 5f76 3220 696e 7374  ed_files_v2 inst
+00009fd0: 6561 642e 0a0a 2020 2020 2020 2020 4765  ead...        Ge
+00009fe0: 7420 6120 6c69 7374 206f 6620 616c 6c20  t a list of all 
+00009ff0: 6669 6c65 7320 5469 7461 6e69 756d 436f  files TitaniumCo
+0000a000: 7265 2065 6e67 696e 6520 6578 7472 6163  re engine extrac
+0000a010: 7465 6420 6672 6f6d 2074 6865 2072 6571  ted from the req
+0000a020: 7565 7374 6564 2073 616d 706c 6520 6475  uested sample du
+0000a030: 7269 6e67 2073 7461 7469 6320 616e 616c  ring static anal
+0000a040: 7973 6973 2e0a 2020 2020 2020 2020 4966  ysis..        If
+0000a050: 2075 7365 642c 2070 6167 655f 7369 7a65   used, page_size
+0000a060: 2061 6e64 2070 6167 6520 6e65 6564 2074   and page need t
+0000a070: 6f20 6265 2063 6f6d 6269 6e65 6420 7768  o be combined wh
+0000a080: 696c 6520 6b65 6570 696e 6720 7472 6163  ile keeping trac
+0000a090: 6b20 6f66 2072 656d 6169 6e69 6e67 2070  k of remaining p
+0000a0a0: 6167 6573 206f 6620 7265 7375 6c74 732e  ages of results.
+0000a0b0: 0a20 2020 2020 2020 2065 2e67 2e20 2d20  .        e.g. - 
+0000a0c0: 6966 2072 6573 756c 7420 636f 756e 7420  if result count 
+0000a0d0: 6973 2035 2061 6e64 2070 6167 655f 7369  is 5 and page_si
+0000a0e0: 7a65 2069 7320 322c 2074 6865 7265 2069  ze is 2, there i
+0000a0f0: 7320 6f6e 6c79 2033 2070 6167 6573 2077  s only 3 pages w
+0000a100: 6f72 7468 206f 6620 7265 7375 6c74 732e  orth of results.
+0000a110: 0a20 2020 2020 2020 2054 6865 2070 6167  .        The pag
+0000a120: 6520 7061 7261 6d65 7465 7220 6361 6e20  e parameter can 
+0000a130: 6e6f 7420 6265 2075 7365 6420 7769 7468  not be used with
+0000a140: 6f75 7420 7061 6765 5f73 697a 652e 2070  out page_size. p
+0000a150: 6167 6520 616e 6420 7061 6765 5f73 697a  age and page_siz
+0000a160: 6520 6e65 6564 2074 6f20 6265 2075 7365  e need to be use
+0000a170: 6420 746f 6765 7468 6572 2e0a 2020 2020  d together..    
+0000a180: 2020 2020 4966 2070 6167 655f 7369 7a65      If page_size
+0000a190: 2061 6e64 2070 6167 6520 6172 6520 6e6f   and page are no
+0000a1a0: 7420 7573 6564 2c20 616c 6c20 7265 7375  t used, all resu
+0000a1b0: 6c74 7320 6172 6520 7265 7475 726e 6564  lts are returned
+0000a1c0: 2069 6e20 6f6e 6520 7265 7370 6f6e 7365   in one response
+0000a1d0: 2e0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
+0000a1e0: 6172 616d 2073 616d 706c 655f 6861 7368  aram sample_hash
+0000a1f0: 3a20 6861 7368 2073 7472 696e 670a 2020  : hash string.  
+0000a200: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+0000a210: 7361 6d70 6c65 5f68 6173 683a 2073 7472  sample_hash: str
+0000a220: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+0000a230: 7261 6d20 7061 6765 5f73 697a 653a 2069  ram page_size: i
+0000a240: 6620 6465 6669 6e65 642c 2072 6573 756c  f defined, resul
+0000a250: 7473 2061 7265 2072 6574 7572 6e65 6420  ts are returned 
+0000a260: 696e 2070 6167 6573 206f 6620 7468 6973  in pages of this
+0000a270: 2073 697a 650a 2020 2020 2020 2020 2020   size.          
+0000a280: 2020 3a74 7970 6520 7061 6765 5f73 697a    :type page_siz
+0000a290: 653a 2069 6e74 0a20 2020 2020 2020 2020  e: int.         
+0000a2a0: 2020 203a 7061 7261 6d20 7061 6765 3a20     :param page: 
+0000a2b0: 6465 6669 6e65 7320 7768 6963 6820 7061  defines which pa
+0000a2c0: 6765 206f 6620 7265 7375 6c74 7320 7368  ge of results sh
+0000a2d0: 6f75 6c64 2062 6520 6665 7463 6865 640a  ould be fetched.
+0000a2e0: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+0000a2f0: 6520 7061 6765 3a20 696e 740a 2020 2020  e page: int.    
+0000a300: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+0000a310: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+0000a320: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
+0000a330: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
+0000a340: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000a350: 2020 2020 7761 726e 2822 5468 6973 206d      warn("This m
+0000a360: 6574 686f 6420 6973 2064 6570 7265 6361  ethod is depreca
+0000a370: 7465 642e 2055 7365 206c 6973 745f 6578  ted. Use list_ex
+0000a380: 7472 6163 7465 645f 6669 6c65 735f 7632  tracted_files_v2
+0000a390: 2069 6e73 7465 6164 2e22 2c20 4465 7072   instead.", Depr
+0000a3a0: 6563 6174 696f 6e57 6172 6e69 6e67 290a  ecationWarning).
+0000a3b0: 0a20 2020 2020 2020 2076 616c 6964 6174  .        validat
+0000a3c0: 655f 6861 7368 6573 280a 2020 2020 2020  e_hashes(.      
+0000a3d0: 2020 2020 2020 6861 7368 5f69 6e70 7574        hash_input
+0000a3e0: 3d5b 7361 6d70 6c65 5f68 6173 685d 2c0a  =[sample_hash],.
+0000a3f0: 2020 2020 2020 2020 2020 2020 616c 6c6f              allo
+0000a400: 7765 645f 6861 7368 5f74 7970 6573 3d28  wed_hash_types=(
+0000a410: 4d44 352c 2053 4841 312c 2053 4841 3235  MD5, SHA1, SHA25
+0000a420: 362c 2053 4841 3531 3229 0a20 2020 2020  6, SHA512).     
+0000a430: 2020 2029 0a0a 2020 2020 2020 2020 656e     )..        en
+0000a440: 6470 6f69 6e74 203d 2073 656c 662e 5f5f  dpoint = self.__
+0000a450: 4c49 5354 5f45 5854 5241 4354 4544 5f46  LIST_EXTRACTED_F
+0000a460: 494c 4553 5f45 4e44 504f 494e 542e 666f  ILES_ENDPOINT.fo
+0000a470: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+0000a480: 2020 6861 7368 5f76 616c 7565 3d73 616d    hash_value=sam
+0000a490: 706c 655f 6861 7368 0a20 2020 2020 2020  ple_hash.       
+0000a4a0: 2029 0a0a 2020 2020 2020 2020 7572 6c20   )..        url 
+0000a4b0: 3d20 7365 6c66 2e5f 7572 6c2e 666f 726d  = self._url.form
+0000a4c0: 6174 2865 6e64 706f 696e 743d 656e 6470  at(endpoint=endp
+0000a4d0: 6f69 6e74 290a 0a20 2020 2020 2020 2069  oint)..        i
+0000a4e0: 6620 2870 6167 655f 7369 7a65 2061 6e64  f (page_size and
+0000a4f0: 206e 6f74 2070 6167 6529 206f 7220 286e   not page) or (n
+0000a500: 6f74 2070 6167 655f 7369 7a65 2061 6e64  ot page_size and
+0000a510: 2070 6167 6529 3a0a 2020 2020 2020 2020   page):.        
+0000a520: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
+0000a530: 6e70 7574 4572 726f 7228 2250 6172 616d  nputError("Param
+0000a540: 6574 6572 7320 7061 6765 5f73 697a 6520  eters page_size 
+0000a550: 616e 6420 7061 6765 206d 7573 7420 6265  and page must be
+0000a560: 2075 7365 6420 746f 6765 7468 6572 2e22   used together."
+0000a570: 290a 0a20 2020 2020 2020 2069 6620 7061  )..        if pa
+0000a580: 6765 3a0a 2020 2020 2020 2020 2020 2020  ge:.            
+0000a590: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+0000a5a0: 6528 7061 6765 5f73 697a 652c 2069 6e74  e(page_size, int
+0000a5b0: 2920 6f72 206e 6f74 2069 7369 6e73 7461  ) or not isinsta
+0000a5c0: 6e63 6528 7061 6765 2c20 696e 7429 3a0a  nce(page, int):.
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5e0: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
+0000a5f0: 4572 726f 7228 2270 6167 655f 7369 7a65  Error("page_size
+0000a600: 2061 6e64 2070 6167 6520 7061 7261 6d65   and page parame
+0000a610: 7465 7273 206e 6565 6420 746f 2062 6520  ters need to be 
+0000a620: 696e 7465 6765 722e 2229 0a0a 2020 2020  integer.")..    
+0000a630: 2020 2020 2020 2020 7572 6c20 3d20 227b          url = "{
+0000a640: 7572 6c7d 3f70 6167 655f 7369 7a65 3d7b  url}?page_size={
+0000a650: 7061 6765 5f73 697a 657d 2670 6167 653d  page_size}&page=
+0000a660: 7b70 6167 657d 222e 666f 726d 6174 280a  {page}".format(.
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a680: 7572 6c3d 7572 6c2c 0a20 2020 2020 2020  url=url,.       
+0000a690: 2020 2020 2020 2020 2070 6167 655f 7369           page_si
+0000a6a0: 7a65 3d70 6167 655f 7369 7a65 2c0a 2020  ze=page_size,.  
+0000a6b0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000a6c0: 6765 3d70 6167 650a 2020 2020 2020 2020  ge=page.        
+0000a6d0: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
+0000a6e0: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+0000a6f0: 5f67 6574 5f72 6571 7565 7374 2875 726c  _get_request(url
+0000a700: 3d75 726c 290a 0a20 2020 2020 2020 2073  =url)..        s
+0000a710: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
+0000a720: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
+0000a730: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000a740: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
+0000a750: 206c 6973 745f 6578 7472 6163 7465 645f   list_extracted_
+0000a760: 6669 6c65 735f 7632 2873 656c 662c 2073  files_v2(self, s
+0000a770: 616d 706c 655f 6861 7368 2c20 7061 6765  ample_hash, page
+0000a780: 5f73 697a 653d 4e6f 6e65 2c20 7061 6765  _size=None, page
+0000a790: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0000a7a0: 2222 2247 6574 2061 206c 6973 7420 6f66  """Get a list of
+0000a7b0: 2061 6c6c 2066 696c 6573 2054 6974 616e   all files Titan
+0000a7c0: 6975 6d43 6f72 6520 656e 6769 6e65 2065  iumCore engine e
+0000a7d0: 7874 7261 6374 6564 2066 726f 6d20 7468  xtracted from th
+0000a7e0: 6520 7265 7175 6573 7465 6420 7361 6d70  e requested samp
+0000a7f0: 6c65 2064 7572 696e 6720 7374 6174 6963  le during static
+0000a800: 2061 6e61 6c79 7369 732e 0a20 2020 2020   analysis..     
+0000a810: 2020 2049 6620 7468 6520 7061 6765 2070     If the page p
+0000a820: 6172 616d 6574 6572 2069 7320 7573 6564  arameter is used
+0000a830: 2c20 6974 206e 6565 6473 2074 6f20 6265  , it needs to be
+0000a840: 2063 6f6d 6269 6e65 6420 7769 7468 2074   combined with t
+0000a850: 6865 2070 6167 655f 7369 7a65 2070 6172  he page_size par
+0000a860: 616d 6574 6572 2077 6869 6c65 206b 6565  ameter while kee
+0000a870: 7069 6e67 2074 7261 636b 206f 660a 2020  ping track of.  
+0000a880: 2020 2020 2020 7265 6d61 696e 696e 6720        remaining 
+0000a890: 7061 6765 7320 6f66 2072 6573 756c 7473  pages of results
+0000a8a0: 2e0a 2020 2020 2020 2020 652e 672e 202d  ..        e.g. -
+0000a8b0: 2069 6620 7265 7375 6c74 2063 6f75 6e74   if result count
+0000a8c0: 2069 7320 3520 616e 6420 7061 6765 5f73   is 5 and page_s
+0000a8d0: 697a 6520 6973 2032 2c20 7468 6572 6520  ize is 2, there 
+0000a8e0: 6973 206f 6e6c 7920 3320 7061 6765 7320  is only 3 pages 
+0000a8f0: 776f 7274 6820 6f66 2072 6573 756c 7473  worth of results
+0000a900: 2e0a 2020 2020 2020 2020 5468 6520 7061  ..        The pa
+0000a910: 6765 5f73 697a 6520 7061 7261 6d65 7465  ge_size paramete
+0000a920: 7220 6361 6e20 6265 2075 7365 6420 7769  r can be used wi
+0000a930: 7468 6f75 7420 7468 6520 7061 6765 2070  thout the page p
+0000a940: 6172 616d 6574 6572 2e0a 2020 2020 2020  arameter..      
+0000a950: 2020 4966 2070 6167 655f 7369 7a65 2061    If page_size a
+0000a960: 6e64 2070 6167 6520 6172 6520 6e6f 7420  nd page are not 
+0000a970: 7573 6564 2c20 616c 6c20 7265 7375 6c74  used, all result
+0000a980: 7320 6172 6520 7265 7475 726e 6564 2069  s are returned i
+0000a990: 6e20 6f6e 6520 7265 7370 6f6e 7365 2e0a  n one response..
+0000a9a0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0000a9b0: 616d 2073 616d 706c 655f 6861 7368 3a20  am sample_hash: 
+0000a9c0: 6861 7368 2073 7472 696e 670a 2020 2020  hash string.    
+0000a9d0: 2020 2020 2020 2020 3a74 7970 6520 7361          :type sa
+0000a9e0: 6d70 6c65 5f68 6173 683a 2073 7472 0a20  mple_hash: str. 
+0000a9f0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+0000aa00: 6d20 7061 6765 5f73 697a 653a 2064 6566  m page_size: def
+0000aa10: 696e 6573 2074 6865 206e 756d 6265 7220  ines the number 
+0000aa20: 6f66 2072 6573 756c 7473 206f 6e20 7468  of results on th
+0000aa30: 6520 7265 7475 726e 6564 2070 6167 650a  e returned page.
+0000aa40: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+0000aa50: 6520 7061 6765 5f73 697a 653a 2069 6e74  e page_size: int
+0000aa60: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+0000aa70: 7261 6d20 7061 6765 3a20 6465 6669 6e65  ram page: define
+0000aa80: 7320 7768 6963 6820 7061 6765 206f 6620  s which page of 
+0000aa90: 7265 7375 6c74 7320 7368 6f75 6c64 2062  results should b
+0000aaa0: 6520 6665 7463 6865 640a 2020 2020 2020  e fetched.      
+0000aab0: 2020 2020 2020 3a74 7970 6520 7061 6765        :type page
+0000aac0: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
+0000aad0: 2020 3a72 6574 7572 6e3a 2072 6573 706f    :return: respo
+0000aae0: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
+0000aaf0: 3a72 7479 7065 3a20 7265 7175 6573 7473  :rtype: requests
+0000ab00: 2e52 6573 706f 6e73 650a 2020 2020 2020  .Response.      
+0000ab10: 2020 2222 220a 2020 2020 2020 2020 7661    """.        va
+0000ab20: 6c69 6461 7465 5f68 6173 6865 7328 0a20  lidate_hashes(. 
+0000ab30: 2020 2020 2020 2020 2020 2068 6173 685f             hash_
+0000ab40: 696e 7075 743d 5b73 616d 706c 655f 6861  input=[sample_ha
+0000ab50: 7368 5d2c 0a20 2020 2020 2020 2020 2020  sh],.           
+0000ab60: 2061 6c6c 6f77 6564 5f68 6173 685f 7479   allowed_hash_ty
+0000ab70: 7065 733d 284d 4435 2c20 5348 4131 2c20  pes=(MD5, SHA1, 
+0000ab80: 5348 4132 3536 2c20 5348 4135 3132 290a  SHA256, SHA512).
+0000ab90: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000aba0: 2020 2069 6620 7061 6765 2061 6e64 206e     if page and n
+0000abb0: 6f74 2070 6167 655f 7369 7a65 3a0a 2020  ot page_size:.  
+0000abc0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000abd0: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
+0000abe0: 2249 6620 7468 6520 7061 6765 2070 6172  "If the page par
+0000abf0: 616d 6574 6572 2069 7320 7573 6564 2c20  ameter is used, 
+0000ac00: 7061 6765 5f73 697a 6520 6d75 7374 2062  page_size must b
+0000ac10: 6520 6465 6669 6e65 642e 2229 0a0a 2020  e defined.")..  
+0000ac20: 2020 2020 2020 656e 6470 6f69 6e74 203d        endpoint =
+0000ac30: 2073 656c 662e 5f5f 4c49 5354 5f45 5854   self.__LIST_EXT
+0000ac40: 5241 4354 4544 5f46 494c 4553 5f45 4e44  RACTED_FILES_END
+0000ac50: 504f 494e 545f 5632 2e66 6f72 6d61 7428  POINT_V2.format(
+0000ac60: 0a20 2020 2020 2020 2020 2020 2068 6173  .            has
+0000ac70: 685f 7661 6c75 653d 7361 6d70 6c65 5f68  h_value=sample_h
+0000ac80: 6173 680a 2020 2020 2020 2020 290a 0a20  ash.        ).. 
+0000ac90: 2020 2020 2020 2075 726c 203d 2073 656c         url = sel
+0000aca0: 662e 5f75 726c 2e66 6f72 6d61 7428 656e  f._url.format(en
+0000acb0: 6470 6f69 6e74 3d65 6e64 706f 696e 7429  dpoint=endpoint)
+0000acc0: 0a0a 2020 2020 2020 2020 7061 7261 6d73  ..        params
+0000acd0: 5f64 6963 7420 3d20 7b22 7061 6765 223a  _dict = {"page":
+0000ace0: 2070 6167 652c 2022 7061 6765 5f73 697a   page, "page_siz
+0000acf0: 6522 3a20 7061 6765 5f73 697a 657d 0a0a  e": page_size}..
+0000ad00: 2020 2020 2020 2020 7061 7261 6d73 5f6c          params_l
+0000ad10: 6973 7420 3d20 5b5d 0a0a 2020 2020 2020  ist = []..      
+0000ad20: 2020 666f 7220 6b65 792c 2076 616c 7565    for key, value
+0000ad30: 2069 6e20 7061 7261 6d73 5f64 6963 742e   in params_dict.
+0000ad40: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+0000ad50: 2020 2020 2069 6620 7661 6c75 653a 0a20       if value:. 
+0000ad60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000ad70: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+0000ad80: 2876 616c 7565 2c20 696e 7429 3a0a 2020  (value, int):.  
+0000ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ada0: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+0000adb0: 7574 4572 726f 7228 227b 7061 7261 6d7d  utError("{param}
+0000adc0: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
+0000add0: 6265 2069 6e74 6567 6572 2e22 2e66 6f72  be integer.".for
+0000ade0: 6d61 7428 7061 7261 6d3d 6b65 7929 290a  mat(param=key)).
+0000adf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ae00: 2070 6172 616d 735f 6c69 7374 2e61 7070   params_list.app
+0000ae10: 656e 6428 227b 6b65 797d 3d7b 7661 6c75  end("{key}={valu
+0000ae20: 657d 222e 666f 726d 6174 286b 6579 3d6b  e}".format(key=k
+0000ae30: 6579 2c20 7661 6c75 653d 7661 6c75 6529  ey, value=value)
+0000ae40: 290a 0a20 2020 2020 2020 2069 6620 7061  )..        if pa
+0000ae50: 7261 6d73 5f6c 6973 743a 0a20 2020 2020  rams_list:.     
+0000ae60: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
+0000ae70: 223f 7b70 6172 616d 737d 222e 666f 726d  "?{params}".form
+0000ae80: 6174 2870 6172 616d 733d 2226 222e 6a6f  at(params="&".jo
+0000ae90: 696e 2870 6172 616d 735f 6c69 7374 2929  in(params_list))
+0000aea0: 0a0a 2020 2020 2020 2020 2020 2020 7572  ..            ur
+0000aeb0: 6c20 3d20 227b 7572 6c7d 7b70 6172 616d  l = "{url}{param
+0000aec0: 737d 222e 666f 726d 6174 2875 726c 3d75  s}".format(url=u
+0000aed0: 726c 2c20 7061 7261 6d73 3d70 6172 616d  rl, params=param
+0000aee0: 7329 0a0a 2020 2020 2020 2020 7265 7370  s)..        resp
+0000aef0: 6f6e 7365 203d 2073 656c 662e 5f5f 6765  onse = self.__ge
+0000af00: 745f 7265 7175 6573 7428 7572 6c3d 7572  t_request(url=ur
+0000af10: 6c29 0a0a 2020 2020 2020 2020 7365 6c66  l)..        self
+0000af20: 2e5f 5f72 6169 7365 5f6f 6e5f 6572 726f  .__raise_on_erro
+0000af30: 7228 7265 7370 6f6e 7365 290a 0a20 2020  r(response)..   
+0000af40: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+0000af50: 6f6e 7365 0a0a 2020 2020 6465 6620 6c69  onse..    def li
+0000af60: 7374 5f65 7874 7261 6374 6564 5f66 696c  st_extracted_fil
+0000af70: 6573 5f76 325f 6167 6772 6567 6174 6564  es_v2_aggregated
+0000af80: 2873 656c 662c 2073 616d 706c 655f 6861  (self, sample_ha
+0000af90: 7368 2c20 6d61 785f 7265 7375 6c74 733d  sh, max_results=
+0000afa0: 3530 3030 293a 0a20 2020 2020 2020 2022  5000):.        "
+0000afb0: 2222 4765 7420 6120 6c69 7374 206f 6620  ""Get a list of 
+0000afc0: 616c 6c20 6669 6c65 7320 5469 7461 6e69  all files Titani
+0000afd0: 756d 436f 7265 2065 6e67 696e 6520 6578  umCore engine ex
+0000afe0: 7472 6163 7465 6420 6672 6f6d 2074 6865  tracted from the
+0000aff0: 2072 6571 7565 7374 6564 2073 616d 706c   requested sampl
+0000b000: 6520 6475 7269 6e67 2073 7461 7469 6320  e during static 
+0000b010: 616e 616c 7973 6973 2e0a 2020 2020 2020  analysis..      
+0000b020: 2020 5061 6769 6e67 2069 7320 646f 6e65    Paging is done
+0000b030: 2061 7574 6f6d 6174 6963 616c 6c79 2061   automatically a
+0000b040: 6e64 2072 6573 756c 7473 2066 726f 6d20  nd results from 
+0000b050: 696e 6469 7669 6475 616c 2072 6573 706f  individual respo
+0000b060: 6e73 6573 2061 6767 7265 6761 7465 6420  nses aggregated 
+0000b070: 696e 746f 206f 6e65 206c 6973 7420 616e  into one list an
+0000b080: 6420 7265 7475 726e 6564 2e0a 2020 2020  d returned..    
+0000b090: 2020 2020 5468 6520 6d61 785f 7265 7375      The max_resu
+0000b0a0: 6c74 7320 7061 7261 6d65 7465 7220 6465  lts parameter de
+0000b0b0: 6669 6e65 7320 7468 6520 6d61 7869 6d75  fines the maximu
+0000b0c0: 6d20 6e75 6d62 6572 206f 6620 7265 7375  m number of resu
+0000b0d0: 6c74 7320 746f 2062 6520 7265 7475 726e  lts to be return
+0000b0e0: 6564 2074 6f20 7468 6520 6c69 7374 2e0a  ed to the list..
+0000b0f0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0000b100: 616d 2073 616d 706c 655f 6861 7368 3a20  am sample_hash: 
+0000b110: 6861 7368 2073 7472 696e 670a 2020 2020  hash string.    
+0000b120: 2020 2020 2020 2020 3a74 7970 6520 7361          :type sa
+0000b130: 6d70 6c65 5f68 6173 683a 2073 7472 0a20  mple_hash: str. 
+0000b140: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+0000b150: 6d20 6d61 785f 7265 7375 6c74 733a 206d  m max_results: m
+0000b160: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+0000b170: 2072 6573 756c 7473 2074 6f20 6265 2072   results to be r
+0000b180: 6574 7572 6e65 640a 2020 2020 2020 2020  eturned.        
+0000b190: 2020 2020 3a74 7970 6520 6d61 785f 7265      :type max_re
+0000b1a0: 7375 6c74 733a 2069 6e74 0a20 2020 2020  sults: int.     
+0000b1b0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+0000b1c0: 6c69 7374 206f 6620 7265 7375 6c74 730a  list of results.
+0000b1d0: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
+0000b1e0: 7065 3a20 6c69 7374 0a20 2020 2020 2020  pe: list.       
+0000b1f0: 2022 2222 0a20 2020 2020 2020 2070 6173   """.        pas
+0000b200: 730a 2020 2020 2020 2020 7265 7375 6c74  s.        result
+0000b210: 5f6c 6973 7420 3d20 5b5d 0a20 2020 2020  _list = [].     
+0000b220: 2020 206e 6578 745f 7061 6765 203d 2031     next_page = 1
+0000b230: 0a0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
+0000b240: 6e65 7874 5f70 6167 653a 0a20 2020 2020  next_page:.     
+0000b250: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0000b260: 3d20 7365 6c66 2e6c 6973 745f 6578 7472  = self.list_extr
+0000b270: 6163 7465 645f 6669 6c65 735f 7632 280a  acted_files_v2(.
+0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b290: 7361 6d70 6c65 5f68 6173 683d 7361 6d70  sample_hash=samp
+0000b2a0: 6c65 5f68 6173 682c 0a20 2020 2020 2020  le_hash,.       
+0000b2b0: 2020 2020 2020 2020 2070 6167 653d 6e65           page=ne
+0000b2c0: 7874 5f70 6167 652c 0a20 2020 2020 2020  xt_page,.       
+0000b2d0: 2020 2020 2020 2020 2070 6167 655f 7369           page_si
+0000b2e0: 7a65 3d31 3030 0a20 2020 2020 2020 2020  ze=100.         
+0000b2f0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+0000b300: 2020 7265 7370 6f6e 7365 5f6a 736f 6e20    response_json 
+0000b310: 3d20 7265 7370 6f6e 7365 2e6a 736f 6e28  = response.json(
+0000b320: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
+0000b330: 6573 756c 7473 203d 2072 6573 706f 6e73  esults = respons
+0000b340: 655f 6a73 6f6e 2e67 6574 2822 7265 7375  e_json.get("resu
+0000b350: 6c74 7322 2c20 5b5d 290a 2020 2020 2020  lts", []).      
+0000b360: 2020 2020 2020 7265 7375 6c74 5f6c 6973        result_lis
+0000b370: 742e 6578 7465 6e64 2872 6573 756c 7473  t.extend(results
+0000b380: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000b390: 6620 6c65 6e28 7265 7375 6c74 5f6c 6973  f len(result_lis
+0000b3a0: 7429 203e 206d 6178 5f72 6573 756c 7473  t) > max_results
+0000b3b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b3c0: 2020 7265 7375 6c74 7320 3d20 7265 7375    results = resu
+0000b3d0: 6c74 5f6c 6973 745b 3a6d 6178 5f72 6573  lt_list[:max_res
+0000b3e0: 756c 7473 5d0a 2020 2020 2020 2020 2020  ults].          
+0000b3f0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0000b400: 756c 7473 0a0a 2020 2020 2020 2020 2020  ults..          
+0000b410: 2020 6e65 7874 5f70 6167 655f 7572 6c20    next_page_url 
+0000b420: 3d20 7265 7370 6f6e 7365 5f6a 736f 6e2e  = response_json.
+0000b430: 6765 7428 226e 6578 7422 2c20 4e6f 6e65  get("next", None
+0000b440: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
+0000b450: 7874 5f70 6167 6520 3d20 696e 7428 6e65  xt_page = int(ne
+0000b460: 7874 5f70 6167 655f 7572 6c2e 7370 6c69  xt_page_url.spli
+0000b470: 7428 223f 2229 5b31 5d2e 7370 6c69 7428  t("?")[1].split(
+0000b480: 2226 2229 5b30 5d2e 7370 6c69 7428 223d  "&")[0].split("=
+0000b490: 2229 5b31 5d29 2069 6620 6e65 7874 5f70  ")[1]) if next_p
+0000b4a0: 6167 655f 7572 6c20 656c 7365 204e 6f6e  age_url else Non
+0000b4b0: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+0000b4c0: 6e20 7265 7375 6c74 5f6c 6973 740a 0a20  n result_list.. 
+0000b4d0: 2020 2064 6566 2064 6f77 6e6c 6f61 645f     def download_
+0000b4e0: 6578 7472 6163 7465 645f 6669 6c65 7328  extracted_files(
+0000b4f0: 7365 6c66 2c20 7361 6d70 6c65 5f68 6173  self, sample_has
+0000b500: 6829 3a0a 2020 2020 2020 2020 2222 2241  h):.        """A
+0000b510: 6363 6570 7473 2061 2073 696e 676c 6520  ccepts a single 
+0000b520: 6861 7368 2073 7472 696e 6720 616e 6420  hash string and 
+0000b530: 7265 7475 726e 7320 6120 646f 776e 6c6f  returns a downlo
+0000b540: 6164 6162 6c65 2061 7263 6869 7665 2066  adable archive f
+0000b550: 696c 650a 2020 2020 2020 2020 636f 6e74  ile.        cont
+0000b560: 6169 6e69 6e67 2066 696c 6573 2065 7874  aining files ext
+0000b570: 7261 6374 6564 2066 726f 6d20 7468 6520  racted from the 
+0000b580: 6465 7369 7265 6420 7361 6d70 6c65 2e0a  desired sample..
+0000b590: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0000b5a0: 616d 2073 616d 706c 655f 6861 7368 3a20  am sample_hash: 
+0000b5b0: 6861 7368 2073 7472 696e 670a 2020 2020  hash string.    
+0000b5c0: 2020 2020 2020 2020 3a74 7970 6520 7361          :type sa
+0000b5d0: 6d70 6c65 5f68 6173 683a 2073 7472 0a20  mple_hash: str. 
+0000b5e0: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
+0000b5f0: 726e 3a20 7265 7370 6f6e 7365 0a20 2020  rn: response.   
+0000b600: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
+0000b610: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
+0000b620: 7365 0a20 2020 2020 2020 2022 2222 0a20  se.        """. 
+0000b630: 2020 2020 2020 2076 616c 6964 6174 655f         validate_
+0000b640: 6861 7368 6573 280a 2020 2020 2020 2020  hashes(.        
+0000b650: 2020 2020 6861 7368 5f69 6e70 7574 3d5b      hash_input=[
+0000b660: 7361 6d70 6c65 5f68 6173 685d 2c0a 2020  sample_hash],.  
+0000b670: 2020 2020 2020 2020 2020 616c 6c6f 7765            allowe
+0000b680: 645f 6861 7368 5f74 7970 6573 3d28 4d44  d_hash_types=(MD
+0000b690: 352c 2053 4841 312c 2053 4841 3235 362c  5, SHA1, SHA256,
+0000b6a0: 2053 4841 3531 3229 0a20 2020 2020 2020   SHA512).       
+0000b6b0: 2029 0a0a 2020 2020 2020 2020 656e 6470   )..        endp
+0000b6c0: 6f69 6e74 203d 2073 656c 662e 5f5f 444f  oint = self.__DO
+0000b6d0: 574e 4c4f 4144 5f45 5854 5241 4354 4544  WNLOAD_EXTRACTED
+0000b6e0: 5f46 494c 4553 5f45 4e44 504f 494e 542e  _FILES_ENDPOINT.
+0000b6f0: 666f 726d 6174 2868 6173 685f 7661 6c75  format(hash_valu
+0000b700: 653d 7361 6d70 6c65 5f68 6173 6829 0a0a  e=sample_hash)..
+0000b710: 2020 2020 2020 2020 7572 6c20 3d20 7365          url = se
+0000b720: 6c66 2e5f 7572 6c2e 666f 726d 6174 2865  lf._url.format(e
+0000b730: 6e64 706f 696e 743d 656e 6470 6f69 6e74  ndpoint=endpoint
+0000b740: 290a 0a20 2020 2020 2020 2072 6573 706f  )..        respo
+0000b750: 6e73 6520 3d20 7365 6c66 2e5f 5f67 6574  nse = self.__get
+0000b760: 5f72 6571 7565 7374 2875 726c 3d75 726c  _request(url=url
+0000b770: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000b780: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
+0000b790: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+0000b7a0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+0000b7b0: 6e73 650a 0a20 2020 2064 6566 2064 6f77  nse..    def dow
+0000b7c0: 6e6c 6f61 645f 7361 6d70 6c65 2873 656c  nload_sample(sel
+0000b7d0: 662c 2073 616d 706c 655f 6861 7368 293a  f, sample_hash):
+0000b7e0: 0a20 2020 2020 2020 2022 2222 4163 6365  .        """Acce
+0000b7f0: 7074 7320 6120 7369 6e67 6c65 2068 6173  pts a single has
+0000b800: 6820 7374 7269 6e67 2061 6e64 2072 6574  h string and ret
+0000b810: 7572 6e73 2061 2064 6f77 6e6c 6f61 6461  urns a downloada
+0000b820: 626c 6520 7361 6d70 6c65 2e0a 2020 2020  ble sample..    
+0000b830: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+0000b840: 616d 706c 655f 6861 7368 3a20 6861 7368  ample_hash: hash
+0000b850: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+0000b860: 2020 2020 3a74 7970 6520 7361 6d70 6c65      :type sample
+0000b870: 5f68 6173 683a 2073 7472 0a20 2020 2020  _hash: str.     
+0000b880: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+0000b890: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+0000b8a0: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
+0000b8b0: 7565 7374 732e 5265 7370 6f6e 7365 0a20  uests.Response. 
+0000b8c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000b8d0: 2020 2076 616c 6964 6174 655f 6861 7368     validate_hash
+0000b8e0: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+0000b8f0: 6861 7368 5f69 6e70 7574 3d5b 7361 6d70  hash_input=[samp
+0000b900: 6c65 5f68 6173 685d 2c0a 2020 2020 2020  le_hash],.      
+0000b910: 2020 2020 2020 616c 6c6f 7765 645f 6861        allowed_ha
+0000b920: 7368 5f74 7970 6573 3d28 4d44 352c 2053  sh_types=(MD5, S
+0000b930: 4841 312c 2053 4841 3235 362c 2053 4841  HA1, SHA256, SHA
+0000b940: 3531 3229 0a20 2020 2020 2020 2029 0a0a  512).        )..
+0000b950: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
+0000b960: 203d 2073 656c 662e 5f5f 444f 574e 4c4f   = self.__DOWNLO
+0000b970: 4144 5f53 414d 504c 455f 454e 4450 4f49  AD_SAMPLE_ENDPOI
+0000b980: 4e54 2e66 6f72 6d61 7428 6861 7368 5f76  NT.format(hash_v
+0000b990: 616c 7565 3d73 616d 706c 655f 6861 7368  alue=sample_hash
+0000b9a0: 290a 0a20 2020 2020 2020 2075 726c 203d  )..        url =
+0000b9b0: 2073 656c 662e 5f75 726c 2e66 6f72 6d61   self._url.forma
+0000b9c0: 7428 656e 6470 6f69 6e74 3d65 6e64 706f  t(endpoint=endpo
+0000b9d0: 696e 7429 0a0a 2020 2020 2020 2020 7265  int)..        re
+0000b9e0: 7370 6f6e 7365 203d 2073 656c 662e 5f5f  sponse = self.__
+0000b9f0: 6765 745f 7265 7175 6573 7428 7572 6c3d  get_request(url=
+0000ba00: 7572 6c29 0a0a 2020 2020 2020 2020 7365  url)..        se
+0000ba10: 6c66 2e5f 5f72 6169 7365 5f6f 6e5f 6572  lf.__raise_on_er
+0000ba20: 726f 7228 7265 7370 6f6e 7365 290a 0a20  ror(response).. 
+0000ba30: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000ba40: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
+0000ba50: 6465 6c65 7465 5f73 616d 706c 6573 2873  delete_samples(s
+0000ba60: 656c 662c 2068 6173 685f 696e 7075 7429  elf, hash_input)
+0000ba70: 3a0a 2020 2020 2020 2020 2222 2241 6363  :.        """Acc
+0000ba80: 6570 7473 2061 2073 696e 676c 6520 6861  epts a single ha
+0000ba90: 7368 2073 7472 696e 6720 6f72 2061 206c  sh string or a l
+0000baa0: 6973 7420 6f66 2068 6173 6865 7320 616e  ist of hashes an
+0000bab0: 6420 6465 6c65 7465 7320 7468 6520 636f  d deletes the co
+0000bac0: 7272 6573 706f 6e64 696e 6720 7361 6d70  rresponding samp
+0000bad0: 6c65 732e 0a20 2020 2020 2020 2054 6869  les..        Thi
+0000bae0: 7320 6d65 7468 6f64 2063 6f6d 6269 6e65  s method combine
+0000baf0: 7320 7468 6520 7573 6520 6f66 2074 776f  s the use of two
+0000bb00: 2065 6e64 706f 696e 7473 2066 6f72 2074   endpoints for t
+0000bb10: 6865 2066 6f6c 6c6f 7769 6e67 2074 776f  he following two
+0000bb20: 2061 6374 696f 6e73 2e0a 2020 2020 2020   actions..      
+0000bb30: 2020 2d20 4465 6c65 7465 2061 2073 696e    - Delete a sin
+0000bb40: 676c 6520 7361 6d70 6c65 3a20 2744 656c  gle sample: 'Del
+0000bb50: 6574 6520 7361 6d70 6c65 2720 656e 6470  ete sample' endp
+0000bb60: 6f69 6e74 0a20 2020 2020 2020 202d 2044  oint.        - D
+0000bb70: 656c 6574 6520 6120 6261 7463 6820 6f66  elete a batch of
+0000bb80: 2073 616d 706c 6573 3a20 2744 656c 6574   samples: 'Delet
+0000bb90: 6520 6d75 6c74 6970 6c65 2073 616d 706c  e multiple sampl
+0000bba0: 6573 2076 3227 2065 6e64 706f 696e 740a  es v2' endpoint.
+0000bbb0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0000bbc0: 616d 2068 6173 685f 696e 7075 743a 2073  am hash_input: s
+0000bbd0: 696e 676c 6520 6861 7368 2073 7472 696e  ingle hash strin
+0000bbe0: 6720 6f72 2061 206c 6973 7420 6f66 2068  g or a list of h
+0000bbf0: 6173 6865 730a 2020 2020 2020 2020 2020  ashes.          
+0000bc00: 2020 3a74 7970 6520 6861 7368 5f69 6e70    :type hash_inp
+0000bc10: 7574 3a20 7374 7220 6f72 206c 6973 745b  ut: str or list[
+0000bc20: 7374 725d 0a20 2020 2020 2020 2020 2020  str].           
+0000bc30: 203a 7265 7475 726e 3a20 7265 7370 6f6e   :return: respon
+0000bc40: 7365 0a20 2020 2020 2020 2020 2020 203a  se.            :
+0000bc50: 7274 7970 653a 2072 6571 7565 7374 732e  rtype: requests.
+0000bc60: 5265 7370 6f6e 7365 0a20 2020 2020 2020  Response.       
+0000bc70: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+0000bc80: 6973 696e 7374 616e 6365 2868 6173 685f  isinstance(hash_
+0000bc90: 696e 7075 742c 2073 7472 293a 0a20 2020  input, str):.   
+0000bca0: 2020 2020 2020 2020 2076 616c 6964 6174           validat
+0000bcb0: 655f 6861 7368 6573 280a 2020 2020 2020  e_hashes(.      
+0000bcc0: 2020 2020 2020 2020 2020 6861 7368 5f69            hash_i
+0000bcd0: 6e70 7574 3d5b 6861 7368 5f69 6e70 7574  nput=[hash_input
+0000bce0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000bcf0: 2020 2061 6c6c 6f77 6564 5f68 6173 685f     allowed_hash_
+0000bd00: 7479 7065 733d 284d 4435 2c20 5348 4131  types=(MD5, SHA1
+0000bd10: 2c20 5348 4132 3536 2c20 5348 4135 3132  , SHA256, SHA512
+0000bd20: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+0000bd30: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
+0000bd40: 706f 696e 7420 3d20 7365 6c66 2e5f 5f44  point = self.__D
+0000bd50: 454c 4554 455f 5341 4d50 4c45 5f45 4e44  ELETE_SAMPLE_END
+0000bd60: 504f 494e 542e 666f 726d 6174 2868 6173  POINT.format(has
+0000bd70: 685f 7661 6c75 653d 6861 7368 5f69 6e70  h_value=hash_inp
+0000bd80: 7574 290a 0a20 2020 2020 2020 2020 2020  ut)..           
+0000bd90: 2075 726c 203d 2073 656c 662e 5f75 726c   url = self._url
+0000bda0: 2e66 6f72 6d61 7428 656e 6470 6f69 6e74  .format(endpoint
+0000bdb0: 3d65 6e64 706f 696e 7429 0a0a 2020 2020  =endpoint)..    
+0000bdc0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+0000bdd0: 203d 2073 656c 662e 5f5f 6465 6c65 7465   = self.__delete
+0000bde0: 5f72 6571 7565 7374 2875 726c 3d75 726c  _request(url=url
+0000bdf0: 290a 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
+0000be00: 6973 696e 7374 616e 6365 2868 6173 685f  isinstance(hash_
+0000be10: 696e 7075 742c 206c 6973 7429 3a0a 2020  input, list):.  
+0000be20: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
+0000be30: 7465 5f68 6173 6865 7328 0a20 2020 2020  te_hashes(.     
+0000be40: 2020 2020 2020 2020 2020 2068 6173 685f             hash_
+0000be50: 696e 7075 743d 6861 7368 5f69 6e70 7574  input=hash_input
+0000be60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000be70: 2020 616c 6c6f 7765 645f 6861 7368 5f74    allowed_hash_t
+0000be80: 7970 6573 3d28 4d44 352c 2053 4841 312c  ypes=(MD5, SHA1,
+0000be90: 2053 4841 3235 362c 2053 4841 3531 3229   SHA256, SHA512)
+0000bea0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+0000beb0: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
+0000bec0: 3d20 7365 6c66 2e5f 7572 6c2e 666f 726d  = self._url.form
+0000bed0: 6174 2865 6e64 706f 696e 743d 7365 6c66  at(endpoint=self
+0000bee0: 2e5f 5f44 454c 4554 455f 5341 4d50 4c45  .__DELETE_SAMPLE
+0000bef0: 535f 4255 4c4b 5f45 4e44 504f 494e 545f  S_BULK_ENDPOINT_
+0000bf00: 5632 290a 0a20 2020 2020 2020 2020 2020  V2)..           
+0000bf10: 2064 6174 6120 3d20 7b22 6861 7368 5f76   data = {"hash_v
+0000bf20: 616c 7565 7322 3a20 6861 7368 5f69 6e70  alues": hash_inp
+0000bf30: 7574 7d0a 0a20 2020 2020 2020 2020 2020  ut}..           
+0000bf40: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
+0000bf50: 2e5f 5f70 6f73 745f 7265 7175 6573 7428  .__post_request(
+0000bf60: 7572 6c3d 7572 6c2c 2064 6174 613d 6461  url=url, data=da
+0000bf70: 7461 290a 0a20 2020 2020 2020 2065 6c73  ta)..        els
+0000bf80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000bf90: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
+0000bfa0: 7272 6f72 2822 6861 7368 5f69 6e70 7574  rror("hash_input
+0000bfb0: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
+0000bfc0: 6265 2061 2073 696e 676c 6520 6861 7368  be a single hash
+0000bfd0: 2073 7472 696e 6720 6f72 2022 0a20 2020   string or ".   
+0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bff0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000c000: 6120 6c69 7374 206f 6620 6861 7368 2073  a list of hash s
+0000c010: 7472 696e 6773 206f 6620 7468 6520 7361  trings of the sa
+0000c020: 6d65 2074 7970 652e 2229 0a0a 2020 2020  me type.")..    
+0000c030: 2020 2020 7365 6c66 2e5f 5f72 6169 7365      self.__raise
+0000c040: 5f6f 6e5f 6572 726f 7228 7265 7370 6f6e  _on_error(respon
+0000c050: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
+0000c060: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+0000c070: 2020 6465 6620 6368 6563 6b5f 7361 6d70    def check_samp
+0000c080: 6c65 5f72 656d 6f76 616c 5f73 7461 7475  le_removal_statu
+0000c090: 735f 7632 2873 656c 662c 2074 6173 6b5f  s_v2(self, task_
+0000c0a0: 6964 293a 0a20 2020 2020 2020 2022 2222  id):.        """
+0000c0b0: 4163 6365 7074 7320 7468 6520 7461 736b  Accepts the task
+0000c0c0: 2049 4420 7265 7475 726e 6564 2062 7920   ID returned by 
+0000c0d0: 7468 6520 6275 6c6b 2073 616d 706c 6520  the bulk sample 
+0000c0e0: 7265 6d6f 7661 6c20 656e 6470 6f69 6e74  removal endpoint
+0000c0f0: 2061 6e64 2072 6574 7572 6e73 2061 2072   and returns a r
+0000c100: 6573 706f 6e73 6520 7468 6174 0a20 2020  esponse that.   
+0000c110: 2020 2020 2069 6e64 6963 6174 6573 2069       indicates i
+0000c120: 6620 7468 6520 7265 6d6f 7661 6c20 7265  f the removal re
+0000c130: 7175 6573 7420 7761 7320 6669 6e69 7368  quest was finish
+0000c140: 6564 2073 7563 6365 7373 6675 6c6c 7920  ed successfully 
+0000c150: 616e 6420 6966 2061 6c6c 2073 616d 706c  and if all sampl
+0000c160: 6573 2068 6176 6520 6265 656e 2064 656c  es have been del
+0000c170: 6574 6564 2e0a 2020 2020 2020 2020 2020  eted..          
+0000c180: 2020 3a70 6172 616d 2074 6173 6b5f 6964    :param task_id
+0000c190: 3a20 4944 206f 6620 7468 6520 6275 6c6b  : ID of the bulk
+0000c1a0: 2073 616d 706c 6520 7265 6d6f 7661 6c20   sample removal 
+0000c1b0: 7461 736b 0a20 2020 2020 2020 2020 2020  task.           
+0000c1c0: 203a 7479 7065 2074 6173 6b5f 6964 3a20   :type task_id: 
+0000c1d0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+0000c1e0: 3a72 6574 7572 6e3a 2072 6573 706f 6e73  :return: respons
+0000c1f0: 650a 2020 2020 2020 2020 2020 2020 3a72  e.            :r
+0000c200: 7479 7065 3a20 7265 7175 6573 7473 2e52  type: requests.R
+0000c210: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
+0000c220: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+0000c230: 6f74 2069 7369 6e73 7461 6e63 6528 7461  ot isinstance(ta
+0000c240: 736b 5f69 642c 2073 7472 293a 0a20 2020  sk_id, str):.   
+0000c250: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+0000c260: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+0000c270: 7461 736b 5f69 6420 7061 7261 6d65 7465  task_id paramete
+0000c280: 7220 6d75 7374 2062 6520 7374 7269 6e67  r must be string
+0000c290: 2e22 290a 0a20 2020 2020 2020 2065 6e64  .")..        end
+0000c2a0: 706f 696e 7420 3d20 7365 6c66 2e5f 5f43  point = self.__C
+0000c2b0: 4845 434b 5f53 414d 504c 455f 5245 4d4f  HECK_SAMPLE_REMO
+0000c2c0: 5641 4c5f 5354 4154 5553 5f45 4e44 504f  VAL_STATUS_ENDPO
+0000c2d0: 494e 545f 5632 2e66 6f72 6d61 7428 7461  INT_V2.format(ta
+0000c2e0: 736b 5f69 643d 7461 736b 5f69 6429 0a0a  sk_id=task_id)..
+0000c2f0: 2020 2020 2020 2020 7572 6c20 3d20 7365          url = se
+0000c300: 6c66 2e5f 7572 6c2e 666f 726d 6174 2865  lf._url.format(e
+0000c310: 6e64 706f 696e 743d 656e 6470 6f69 6e74  ndpoint=endpoint
+0000c320: 290a 0a20 2020 2020 2020 2072 6573 706f  )..        respo
+0000c330: 6e73 6520 3d20 7365 6c66 2e5f 5f67 6574  nse = self.__get
+0000c340: 5f72 6571 7565 7374 2875 726c 3d75 726c  _request(url=url
+0000c350: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000c360: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
+0000c370: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+0000c380: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+0000c390: 6e73 650a 0a20 2020 2064 6566 205f 5f75  nse..    def __u
+0000c3a0: 7469 6c69 7a65 5f70 6466 5f65 6e64 706f  tilize_pdf_endpo
+0000c3b0: 696e 7428 7365 6c66 2c20 7361 6d70 6c65  int(self, sample
+0000c3c0: 5f68 6173 682c 2065 6e64 706f 696e 7429  _hash, endpoint)
+0000c3d0: 3a0a 2020 2020 2020 2020 2222 2241 6363  :.        """Acc
+0000c3e0: 6570 7473 2061 2073 696e 676c 6520 6861  epts a single ha
+0000c3f0: 7368 2073 7472 696e 6720 616e 6420 7574  sh string and ut
+0000c400: 696c 697a 6573 2070 6466 2072 6570 6f72  ilizes pdf repor
+0000c410: 7420 656e 6470 6f69 6e74 2066 6f72 2069  t endpoint for i
+0000c420: 6e69 7469 6174 696f 6e2c 2073 7461 7475  nitiation, statu
+0000c430: 7320 6368 6563 6b69 6e67 2061 6e64 2064  s checking and d
+0000c440: 6f77 6e6c 6f61 6469 6e67 0a20 2020 2020  ownloading.     
+0000c450: 2020 206f 6620 6120 5044 4620 616e 616c     of a PDF anal
+0000c460: 7973 6973 2072 6570 6f72 7420 666f 7220  ysis report for 
+0000c470: 7468 6520 7265 7175 6573 7465 6420 7361  the requested sa
+0000c480: 6d70 6c65 2e0a 2020 2020 2020 2020 2020  mple..          
+0000c490: 2020 3a70 6172 616d 2073 616d 706c 655f    :param sample_
+0000c4a0: 6861 7368 3a20 6861 7368 2073 7472 696e  hash: hash strin
+0000c4b0: 670a 2020 2020 2020 2020 2020 2020 3a74  g.            :t
+0000c4c0: 7970 6520 7361 6d70 6c65 5f68 6173 683a  ype sample_hash:
+0000c4d0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+0000c4e0: 203a 7061 7261 6d20 656e 6470 6f69 6e74   :param endpoint
+0000c4f0: 3a20 656e 6470 6f69 6e74 2073 7472 696e  : endpoint strin
+0000c500: 670a 2020 2020 2020 2020 2020 2020 3a74  g.            :t
+0000c510: 7970 6520 656e 6470 6f69 6e74 3a20 7374  ype endpoint: st
+0000c520: 720a 2020 2020 2020 2020 2020 2020 3a72  r.            :r
+0000c530: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
+0000c540: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
+0000c550: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
+0000c560: 706f 6e73 650a 2020 2020 2020 2020 2222  ponse.        ""
+0000c570: 220a 2020 2020 2020 2020 7661 6c69 6461  ".        valida
+0000c580: 7465 5f68 6173 6865 7328 0a20 2020 2020  te_hashes(.     
+0000c590: 2020 2020 2020 2068 6173 685f 696e 7075         hash_inpu
+0000c5a0: 743d 5b73 616d 706c 655f 6861 7368 5d2c  t=[sample_hash],
+0000c5b0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
+0000c5c0: 6f77 6564 5f68 6173 685f 7479 7065 733d  owed_hash_types=
+0000c5d0: 284d 4435 2c20 5348 4131 2c20 5348 4132  (MD5, SHA1, SHA2
+0000c5e0: 3536 290a 2020 2020 2020 2020 290a 0a20  56).        ).. 
+0000c5f0: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
+0000c600: 3d20 656e 6470 6f69 6e74 2e66 6f72 6d61  = endpoint.forma
+0000c610: 7428 0a20 2020 2020 2020 2020 2020 2068  t(.            h
+0000c620: 6173 685f 7661 6c75 653d 7361 6d70 6c65  ash_value=sample
+0000c630: 5f68 6173 682c 0a20 2020 2020 2020 2029  _hash,.        )
+0000c640: 0a0a 2020 2020 2020 2020 7572 6c20 3d20  ..        url = 
+0000c650: 7365 6c66 2e5f 7572 6c2e 666f 726d 6174  self._url.format
+0000c660: 2865 6e64 706f 696e 743d 656e 6470 6f69  (endpoint=endpoi
+0000c670: 6e74 290a 0a20 2020 2020 2020 2072 6573  nt)..        res
+0000c680: 706f 6e73 6520 3d20 7365 6c66 2e5f 5f67  ponse = self.__g
+0000c690: 6574 5f72 6571 7565 7374 2875 726c 3d75  et_request(url=u
+0000c6a0: 726c 290a 0a20 2020 2020 2020 2073 656c  rl)..        sel
+0000c6b0: 662e 5f5f 7261 6973 655f 6f6e 5f65 7272  f.__raise_on_err
+0000c6c0: 6f72 2872 6573 706f 6e73 6529 0a0a 2020  or(response)..  
+0000c6d0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0000c6e0: 706f 6e73 650a 0a20 2020 2064 6566 2063  ponse..    def c
+0000c6f0: 7265 6174 655f 7064 665f 7265 706f 7274  reate_pdf_report
+0000c700: 2873 656c 662c 2073 616d 706c 655f 6861  (self, sample_ha
+0000c710: 7368 293a 0a20 2020 2020 2020 2022 2222  sh):.        """
+0000c720: 4163 6365 7074 7320 6120 7369 6e67 6c65  Accepts a single
+0000c730: 2068 6173 6820 7374 7269 6e67 2061 6e64   hash string and
+0000c740: 2069 6e69 7469 6174 6573 2074 6865 2063   initiates the c
+0000c750: 7265 6174 696f 6e20 6f66 2061 2050 4446  reation of a PDF
+0000c760: 2061 6e61 6c79 7369 7320 7265 706f 7274   analysis report
+0000c770: 2066 6f72 2074 6865 2072 6571 7565 7374   for the request
+0000c780: 6564 2073 616d 706c 652e 0a20 2020 2020  ed sample..     
+0000c790: 2020 2054 6865 2072 6573 706f 6e73 6520     The response 
+0000c7a0: 696e 636c 7564 6573 206c 696e 6b73 2074  includes links t
+0000c7b0: 6f20 7468 6520 7064 6620 6372 6561 7469  o the pdf creati
+0000c7c0: 6f6e 2073 7461 7475 7320 656e 6470 6f69  on status endpoi
+0000c7d0: 6e74 2061 6e64 2070 6466 2064 6f77 6e6c  nt and pdf downl
+0000c7e0: 6f61 6420 6564 6e70 6f69 6e74 2066 6f72  oad ednpoint for
+0000c7f0: 2074 6865 2072 6571 7565 7374 6564 0a20   the requested. 
+0000c800: 2020 2020 2020 2073 616d 706c 652e 0a20         sample.. 
+0000c810: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+0000c820: 6d20 7361 6d70 6c65 5f68 6173 683a 2068  m sample_hash: h
+0000c830: 6173 6820 7374 7269 6e67 0a20 2020 2020  ash string.     
+0000c840: 2020 2020 2020 203a 7479 7065 2073 616d         :type sam
+0000c850: 706c 655f 6861 7368 3a20 7374 720a 2020  ple_hash: str.  
+0000c860: 2020 2020 2020 2020 2020 3a72 6574 7572            :retur
+0000c870: 6e3a 2072 6573 706f 6e73 650a 2020 2020  n: response.    
+0000c880: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+0000c890: 7265 7175 6573 7473 2e52 6573 706f 6e73  requests.Respons
+0000c8a0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+0000c8b0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+0000c8c0: 2073 656c 662e 5f5f 7574 696c 697a 655f   self.__utilize_
+0000c8d0: 7064 665f 656e 6470 6f69 6e74 2873 616d  pdf_endpoint(sam
+0000c8e0: 706c 655f 6861 7368 2c20 7365 6c66 2e5f  ple_hash, self._
+0000c8f0: 5f50 4446 5f52 4550 4f52 545f 4352 4541  _PDF_REPORT_CREA
+0000c900: 5445 5f45 4e44 504f 494e 5429 0a20 2020  TE_ENDPOINT).   
+0000c910: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+0000c920: 6f6e 7365 0a0a 2020 2020 6465 6620 6368  onse..    def ch
+0000c930: 6563 6b5f 7064 665f 7265 706f 7274 5f63  eck_pdf_report_c
+0000c940: 7265 6174 696f 6e28 7365 6c66 2c20 7361  reation(self, sa
+0000c950: 6d70 6c65 5f68 6173 6829 3a0a 2020 2020  mple_hash):.    
+0000c960: 2020 2020 2222 2241 6363 6570 7473 2061      """Accepts a
+0000c970: 2073 696e 676c 6520 6861 7368 2073 7472   single hash str
+0000c980: 696e 6720 7468 6174 2073 686f 756c 6420  ing that should 
+0000c990: 636f 7272 6573 706f 6e64 2074 6f20 7468  correspond to th
+0000c9a0: 6520 6861 7368 2075 7365 6420 696e 2074  e hash used in t
+0000c9b0: 6865 2072 6571 7565 7374 2077 6974 680a  he request with.
+0000c9c0: 2020 2020 2020 2020 6372 6561 7465 5f70          create_p
+0000c9d0: 6466 5f72 6570 6f72 7420 6d65 7468 6f64  df_report method
+0000c9e0: 2e20 5468 6520 7265 7370 6f6e 7365 2069  . The response i
+0000c9f0: 6e63 6c75 6465 7320 616e 2069 6e66 6f72  ncludes an infor
+0000ca00: 6d61 7469 7665 206d 6573 7361 6765 2061  mative message a
+0000ca10: 626f 7574 2074 6865 2073 7461 7475 7320  bout the status 
+0000ca20: 6f66 2074 6865 2050 4446 0a20 2020 2020  of the PDF.     
+0000ca30: 2020 2072 6570 6f72 7420 7072 6576 696f     report previo
+0000ca40: 7573 6c79 2072 6571 7565 7374 6564 2e0a  usly requested..
+0000ca50: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0000ca60: 616d 2073 616d 706c 655f 6861 7368 3a20  am sample_hash: 
+0000ca70: 6861 7368 2073 7472 696e 670a 2020 2020  hash string.    
+0000ca80: 2020 2020 2020 2020 3a74 7970 6520 7361          :type sa
+0000ca90: 6d70 6c65 5f68 6173 683a 2073 7472 0a20  mple_hash: str. 
+0000caa0: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
+0000cab0: 726e 3a20 7265 7370 6f6e 7365 0a20 2020  rn: response.   
+0000cac0: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
+0000cad0: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
+0000cae0: 7365 0a20 2020 2020 2020 2022 2222 0a20  se.        """. 
+0000caf0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0000cb00: 3d20 7365 6c66 2e5f 5f75 7469 6c69 7a65  = self.__utilize
+0000cb10: 5f70 6466 5f65 6e64 706f 696e 7428 7361  _pdf_endpoint(sa
+0000cb20: 6d70 6c65 5f68 6173 682c 2073 656c 662e  mple_hash, self.
+0000cb30: 5f5f 5044 465f 5245 504f 5254 5f53 5441  __PDF_REPORT_STA
+0000cb40: 5455 535f 454e 4450 4f49 4e54 290a 2020  TUS_ENDPOINT).  
+0000cb50: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0000cb60: 706f 6e73 650a 0a20 2020 2064 6566 2064  ponse..    def d
+0000cb70: 6f77 6e6c 6f61 645f 7064 665f 7265 706f  ownload_pdf_repo
+0000cb80: 7274 2873 656c 662c 2073 616d 706c 655f  rt(self, sample_
+0000cb90: 6861 7368 293a 0a20 2020 2020 2020 2022  hash):.        "
+0000cba0: 2222 4163 6365 7074 7320 6120 7369 6e67  ""Accepts a sing
+0000cbb0: 6c65 2068 6173 6820 7374 7269 6e67 2074  le hash string t
+0000cbc0: 6861 7420 7368 6f75 6c64 2063 6f72 7265  hat should corre
+0000cbd0: 7370 6f6e 6420 746f 2074 6865 2068 6173  spond to the has
+0000cbe0: 6820 7573 6564 2069 6e20 7468 6520 7265  h used in the re
+0000cbf0: 7175 6573 7420 7769 7468 0a20 2020 2020  quest with.     
+0000cc00: 2020 2063 7265 6174 655f 7064 665f 7265     create_pdf_re
+0000cc10: 706f 7274 206d 6574 686f 642e 0a20 2020  port method..   
+0000cc20: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+0000cc30: 7361 6d70 6c65 5f68 6173 683a 2068 6173  sample_hash: has
+0000cc40: 6820 7374 7269 6e67 0a20 2020 2020 2020  h string.       
+0000cc50: 2020 2020 203a 7479 7065 2073 616d 706c       :type sampl
+0000cc60: 655f 6861 7368 3a20 7374 720a 2020 2020  e_hash: str.    
+0000cc70: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+0000cc80: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+0000cc90: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
+0000cca0: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
+0000ccb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000ccc0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+0000ccd0: 656c 662e 5f5f 7574 696c 697a 655f 7064  elf.__utilize_pd
+0000cce0: 665f 656e 6470 6f69 6e74 2873 616d 706c  f_endpoint(sampl
+0000ccf0: 655f 6861 7368 2c20 7365 6c66 2e5f 5f50  e_hash, self.__P
+0000cd00: 4446 5f52 4550 4f52 545f 444f 574e 4c4f  DF_REPORT_DOWNLO
+0000cd10: 4144 5f45 4e44 504f 494e 5429 0a20 2020  AD_ENDPOINT).   
+0000cd20: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+0000cd30: 6f6e 7365 0a0a 2020 2020 6465 6620 6765  onse..    def ge
+0000cd40: 745f 7469 7461 6e69 756d 5f63 6f72 655f  t_titanium_core_
+0000cd50: 7265 706f 7274 5f76 3228 7365 6c66 2c20  report_v2(self, 
+0000cd60: 7361 6d70 6c65 5f68 6173 682c 2066 6965  sample_hash, fie
+0000cd70: 6c64 733d 4e6f 6e65 293a 0a20 2020 2020  lds=None):.     
+0000cd80: 2020 2022 2222 4163 6365 7074 7320 6120     """Accepts a 
+0000cd90: 7369 6e67 6c65 2068 6173 6820 7374 7269  single hash stri
+0000cda0: 6e67 2061 6e64 2067 6574 7320 7468 6520  ng and gets the 
+0000cdb0: 6675 6c6c 2054 6974 616e 6975 6d43 6f72  full TitaniumCor
+0000cdc0: 6520 7374 6174 6963 2061 6e61 6c79 7369  e static analysi
+0000cdd0: 7320 7265 706f 7274 2066 6f72 2074 6865  s report for the
+0000cde0: 2072 6571 7565 7374 6564 2073 616d 706c   requested sampl
+0000cdf0: 652e 0a20 2020 2020 2020 2054 6865 2072  e..        The r
+0000ce00: 6571 7565 7374 6564 2073 616d 706c 6520  equested sample 
+0000ce10: 6d75 7374 2062 6520 7072 6573 656e 7420  must be present 
+0000ce20: 6f6e 2074 6865 2061 7070 6c69 616e 6365  on the appliance
+0000ce30: 2e20 4966 2074 6865 206f 7074 696f 6e61  . If the optiona
+0000ce40: 6c20 6669 656c 6473 2070 6172 616d 6574  l fields paramet
+0000ce50: 6572 2069 7320 6e6f 7420 7072 6f76 6964  er is not provid
+0000ce60: 6564 2069 6e20 7468 650a 2020 2020 2020  ed in the.      
+0000ce70: 2020 7265 7175 6573 742c 2061 6c6c 2061    request, all a
+0000ce80: 7661 696c 6162 6c65 2070 6172 7473 206f  vailable parts o
+0000ce90: 6620 7468 6520 7374 6174 6963 2061 6e61  f the static ana
+0000cea0: 6c79 7369 7320 7265 706f 7274 2061 7265  lysis report are
+0000ceb0: 2072 6574 7572 6e65 6420 696e 2074 6865   returned in the
+0000cec0: 2072 6573 706f 6e73 652e 0a20 2020 2020   response..     
+0000ced0: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
+0000cee0: 6d70 6c65 5f68 6173 683a 2068 6173 6820  mple_hash: hash 
+0000cef0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+0000cf00: 2020 203a 7479 7065 2073 616d 706c 655f     :type sample_
+0000cf10: 6861 7368 3a20 7374 720a 2020 2020 2020  hash: str.      
+0000cf20: 2020 2020 2020 3a70 6172 616d 2066 6965        :param fie
+0000cf30: 6c64 733a 2061 2073 7472 696e 6720 6f66  lds: a string of
+0000cf40: 2063 6f6d 6d61 2073 6570 6172 6174 6564   comma separated
+0000cf50: 2054 6974 616e 6975 6d43 6f72 6520 2766   TitaniumCore 'f
+0000cf60: 6965 6c64 7327 2074 6f20 7175 6572 790a  ields' to query.
+0000cf70: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+0000cf80: 6520 6669 656c 6473 3a20 7374 720a 2020  e fields: str.  
+0000cf90: 2020 2020 2020 2020 2020 3a72 6574 7572            :retur
+0000cfa0: 6e3a 2072 6573 706f 6e73 650a 2020 2020  n: response.    
+0000cfb0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+0000cfc0: 7265 7175 6573 7473 2e52 6573 706f 6e73  requests.Respons
+0000cfd0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+0000cfe0: 2020 2020 2020 7661 6c69 6461 7465 5f68        validate_h
+0000cff0: 6173 6865 7328 0a20 2020 2020 2020 2020  ashes(.         
+0000d000: 2020 2068 6173 685f 696e 7075 743d 5b73     hash_input=[s
+0000d010: 616d 706c 655f 6861 7368 5d2c 0a20 2020  ample_hash],.   
+0000d020: 2020 2020 2020 2020 2061 6c6c 6f77 6564           allowed
+0000d030: 5f68 6173 685f 7479 7065 733d 284d 4435  _hash_types=(MD5
+0000d040: 2c20 5348 4131 2c20 5348 4132 3536 2c20  , SHA1, SHA256, 
+0000d050: 5348 4135 3132 290a 2020 2020 2020 2020  SHA512).        
+0000d060: 290a 0a20 2020 2020 2020 2069 6620 6669  )..        if fi
+0000d070: 656c 6473 2061 6e64 206e 6f74 2069 7369  elds and not isi
+0000d080: 6e73 7461 6e63 6528 6669 656c 6473 2c20  nstance(fields, 
+0000d090: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+0000d0a0: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+0000d0b0: 7574 4572 726f 7228 2266 6965 6c64 7320  utError("fields 
+0000d0c0: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
+0000d0d0: 6520 6120 7374 7269 6e67 2e22 290a 0a20  e a string.").. 
+0000d0e0: 2020 2020 2020 2069 6620 6669 656c 6473         if fields
+0000d0f0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000d100: 2020 2020 2020 6669 656c 6473 203d 2073        fields = s
+0000d110: 656c 662e 5f74 6963 6f72 655f 6669 656c  elf._ticore_fiel
+0000d120: 6473 0a0a 2020 2020 2020 2020 656e 6470  ds..        endp
+0000d130: 6f69 6e74 203d 2073 656c 662e 5f5f 5449  oint = self.__TI
+0000d140: 5441 4e49 554d 5f43 4f52 455f 5245 504f  TANIUM_CORE_REPO
+0000d150: 5254 5f45 4e44 504f 494e 545f 5632 2e66  RT_ENDPOINT_V2.f
+0000d160: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+0000d170: 2020 2068 6173 685f 7661 6c75 653d 7361     hash_value=sa
+0000d180: 6d70 6c65 5f68 6173 682c 0a20 2020 2020  mple_hash,.     
+0000d190: 2020 2020 2020 2066 6965 6c64 733d 6669         fields=fi
+0000d1a0: 656c 6473 0a20 2020 2020 2020 2029 0a0a  elds.        )..
+0000d1b0: 2020 2020 2020 2020 7572 6c20 3d20 7365          url = se
+0000d1c0: 6c66 2e5f 7572 6c2e 666f 726d 6174 2865  lf._url.format(e
+0000d1d0: 6e64 706f 696e 743d 656e 6470 6f69 6e74  ndpoint=endpoint
+0000d1e0: 290a 0a20 2020 2020 2020 2072 6573 706f  )..        respo
+0000d1f0: 6e73 6520 3d20 7365 6c66 2e5f 5f67 6574  nse = self.__get
+0000d200: 5f72 6571 7565 7374 2875 726c 3d75 726c  _request(url=url
+0000d210: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000d220: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
+0000d230: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+0000d240: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+0000d250: 6e73 650a 0a20 2020 2064 6566 205f 5f75  nse..    def __u
+0000d260: 7469 6c69 7a65 5f64 796e 616d 6963 5f61  tilize_dynamic_a
+0000d270: 6e61 6c79 7369 735f 656e 6470 6f69 6e74  nalysis_endpoint
+0000d280: 2873 656c 662c 2073 616d 706c 655f 6861  (self, sample_ha
+0000d290: 7368 2c20 7265 706f 7274 5f66 6f72 6d61  sh, report_forma
+0000d2a0: 742c 2065 6e64 706f 696e 7429 3a0a 2020  t, endpoint):.  
+0000d2b0: 2020 2020 2020 2222 2241 6363 6570 7473        """Accepts
+0000d2c0: 2065 6e64 706f 696e 742c 2061 2073 696e   endpoint, a sin
+0000d2d0: 676c 6520 6861 7368 2073 7472 696e 6720  gle hash string 
+0000d2e0: 616e 6420 6120 7265 706f 7274 2066 6f72  and a report for
+0000d2f0: 6d61 7420 616e 6420 7574 696c 697a 6573  mat and utilizes
+0000d300: 2064 796e 616d 6963 2061 6e61 6c79 7369   dynamic analysi
+0000d310: 7320 656e 6470 6f69 6e74 2066 6f72 0a20  s endpoint for. 
+0000d320: 2020 2020 2020 2069 6e69 7469 6174 696f         initiatio
+0000d330: 6e2c 2073 7461 7475 7320 6368 6563 6b69  n, status checki
+0000d340: 6e67 2061 6e64 2064 6f77 6e6c 6f61 6469  ng and downloadi
+0000d350: 6e67 206f 6620 5044 4620 6f72 2048 544d  ng of PDF or HTM
+0000d360: 4c20 7265 706f 7274 730a 2020 2020 2020  L reports.      
+0000d370: 2020 666f 7220 7361 6d70 6c65 7320 7468    for samples th
+0000d380: 6174 2068 6176 6520 676f 6e65 2074 6872  at have gone thr
+0000d390: 6f75 6768 2064 796e 616d 6963 2061 6e61  ough dynamic ana
+0000d3a0: 6c79 7369 7320 696e 2074 6865 2052 6576  lysis in the Rev
+0000d3b0: 6572 7369 6e67 4c61 6273 2043 6c6f 7564  ersingLabs Cloud
+0000d3c0: 2053 616e 6462 6f78 2e0a 2020 2020 2020   Sandbox..      
+0000d3d0: 2020 2020 2020 3a70 6172 616d 2073 616d        :param sam
+0000d3e0: 706c 655f 6861 7368 3a20 6861 7368 2073  ple_hash: hash s
+0000d3f0: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+0000d400: 2020 3a74 7970 6520 7361 6d70 6c65 5f68    :type sample_h
+0000d410: 6173 683a 2073 7472 0a20 2020 2020 2020  ash: str.       
+0000d420: 2020 2020 203a 7061 7261 6d20 7265 706f       :param repo
+0000d430: 7274 5f66 6f72 6d61 743a 2072 6570 6f72  rt_format: repor
+0000d440: 7420 666f 726d 6174 2028 2768 746d 6c27  t format ('html'
+0000d450: 206f 7220 2770 6466 2729 0a20 2020 2020   or 'pdf').     
+0000d460: 2020 2020 2020 203a 7274 7970 6520 7265         :rtype re
+0000d470: 706f 7274 5f66 6f72 6d61 743a 2073 7472  port_format: str
+0000d480: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+0000d490: 7261 6d20 656e 6470 6f69 6e74 3a20 656e  ram endpoint: en
+0000d4a0: 6470 6f69 6e74 2073 7472 696e 670a 2020  dpoint string.  
+0000d4b0: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+0000d4c0: 656e 6470 6f69 6e74 3a20 7374 720a 2020  endpoint: str.  
+0000d4d0: 2020 2020 2020 2020 2020 3a72 6574 7572            :retur
+0000d4e0: 6e3a 2072 6573 706f 6e73 650a 2020 2020  n: response.    
+0000d4f0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+0000d500: 7265 7175 6573 7473 2e52 6573 706f 6e73  requests.Respons
+0000d510: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+0000d520: 2020 2020 2020 7661 6c69 6461 7465 5f68        validate_h
+0000d530: 6173 6865 7328 0a20 2020 2020 2020 2020  ashes(.         
+0000d540: 2020 2068 6173 685f 696e 7075 743d 5b73     hash_input=[s
+0000d550: 616d 706c 655f 6861 7368 5d2c 0a20 2020  ample_hash],.   
+0000d560: 2020 2020 2020 2020 2061 6c6c 6f77 6564           allowed
+0000d570: 5f68 6173 685f 7479 7065 733d 2853 4841  _hash_types=(SHA
+0000d580: 312c 290a 2020 2020 2020 2020 290a 0a20  1,).        ).. 
+0000d590: 2020 2020 2020 2069 6620 7265 706f 7274         if report
+0000d5a0: 5f66 6f72 6d61 7420 6e6f 7420 696e 2028  _format not in (
+0000d5b0: 2268 746d 6c22 2c20 2270 6466 2229 3a0a  "html", "pdf"):.
+0000d5c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000d5d0: 6520 5772 6f6e 6749 6e70 7574 4572 726f  e WrongInputErro
+0000d5e0: 7228 2272 6570 6f72 745f 666f 726d 6174  r("report_format
+0000d5f0: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
+0000d600: 6265 2065 6974 6865 7220 2768 746d 6c27  be either 'html'
+0000d610: 206f 7220 2770 6466 272e 2229 0a0a 2020   or 'pdf'.")..  
+0000d620: 2020 2020 2020 656e 6470 6f69 6e74 203d        endpoint =
+0000d630: 2065 6e64 706f 696e 742e 666f 726d 6174   endpoint.format
+0000d640: 280a 2020 2020 2020 2020 2020 2020 6861  (.            ha
+0000d650: 7368 5f76 616c 7565 3d73 616d 706c 655f  sh_value=sample_
+0000d660: 6861 7368 2c0a 2020 2020 2020 2020 2020  hash,.          
+0000d670: 2020 666f 726d 6174 3d72 6570 6f72 745f    format=report_
+0000d680: 666f 726d 6174 2c0a 2020 2020 2020 2020  format,.        
+0000d690: 290a 0a20 2020 2020 2020 2075 726c 203d  )..        url =
+0000d6a0: 2073 656c 662e 5f75 726c 2e66 6f72 6d61   self._url.forma
+0000d6b0: 7428 656e 6470 6f69 6e74 3d65 6e64 706f  t(endpoint=endpo
+0000d6c0: 696e 7429 0a0a 2020 2020 2020 2020 7265  int)..        re
+0000d6d0: 7370 6f6e 7365 203d 2073 656c 662e 5f5f  sponse = self.__
+0000d6e0: 6765 745f 7265 7175 6573 7428 7572 6c3d  get_request(url=
+0000d6f0: 7572 6c29 0a0a 2020 2020 2020 2020 7365  url)..        se
+0000d700: 6c66 2e5f 5f72 6169 7365 5f6f 6e5f 6572  lf.__raise_on_er
+0000d710: 726f 7228 7265 7370 6f6e 7365 290a 0a20  ror(response).. 
+0000d720: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000d730: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
+0000d740: 6372 6561 7465 5f64 796e 616d 6963 5f61  create_dynamic_a
+0000d750: 6e61 6c79 7369 735f 7265 706f 7274 2873  nalysis_report(s
+0000d760: 656c 662c 2073 616d 706c 655f 6861 7368  elf, sample_hash
+0000d770: 2c20 7265 706f 7274 5f66 6f72 6d61 7429  , report_format)
+0000d780: 3a0a 2020 2020 2020 2020 2222 2241 6363  :.        """Acc
+0000d790: 6570 7473 2061 2073 696e 676c 6520 6861  epts a single ha
+0000d7a0: 7368 2073 7472 696e 6720 616e 6420 6120  sh string and a 
+0000d7b0: 7265 706f 7274 2066 6f72 6d61 7420 616e  report format an
+0000d7c0: 6420 696e 6974 6961 7465 7320 7468 6520  d initiates the 
+0000d7d0: 6372 6561 7469 6f6e 206f 6620 5044 4620  creation of PDF 
+0000d7e0: 6f72 2048 544d 4c20 7265 706f 7274 7320  or HTML reports 
+0000d7f0: 666f 720a 2020 2020 2020 2020 7361 6d70  for.        samp
+0000d800: 6c65 7320 7468 6174 2068 6176 6520 676f  les that have go
+0000d810: 6e65 2074 6872 6f75 6768 2064 796e 616d  ne through dynam
+0000d820: 6963 2061 6e61 6c79 7369 7320 696e 2074  ic analysis in t
+0000d830: 6865 2052 6576 6572 7369 6e67 4c61 6273  he ReversingLabs
+0000d840: 2043 6c6f 7564 2053 616e 6462 6f78 2e0a   Cloud Sandbox..
+0000d850: 2020 2020 2020 2020 5468 6520 7265 7370          The resp
+0000d860: 6f6e 7365 2069 6e63 6c75 6465 7320 6c69  onse includes li
+0000d870: 6e6b 7320 746f 2074 6865 2072 6570 6f72  nks to the repor
+0000d880: 7420 6372 6561 7469 6f6e 2073 7461 7475  t creation statu
+0000d890: 7320 656e 6470 6f69 6e74 2061 6e64 2072  s endpoint and r
+0000d8a0: 6570 6f72 7420 646f 776e 6c6f 6164 2065  eport download e
+0000d8b0: 6e64 706f 696e 7420 666f 7220 7468 650a  ndpoint for the.
+0000d8c0: 2020 2020 2020 2020 7265 7175 6573 7465          requeste
+0000d8d0: 6420 7361 6d70 6c65 2e0a 2020 2020 2020  d sample..      
+0000d8e0: 2020 2020 2020 3a70 6172 616d 2073 616d        :param sam
+0000d8f0: 706c 655f 6861 7368 3a20 6861 7368 2073  ple_hash: hash s
+0000d900: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+0000d910: 2020 3a74 7970 6520 7361 6d70 6c65 5f68    :type sample_h
+0000d920: 6173 683a 2073 7472 0a20 2020 2020 2020  ash: str.       
+0000d930: 2020 2020 203a 7061 7261 6d20 7265 706f       :param repo
+0000d940: 7274 5f66 6f72 6d61 743a 2072 6570 6f72  rt_format: repor
+0000d950: 7420 666f 726d 6174 2028 2768 746d 6c27  t format ('html'
+0000d960: 206f 7220 2770 6466 2729 0a20 2020 2020   or 'pdf').     
+0000d970: 2020 2020 2020 203a 7274 7970 6520 7265         :rtype re
+0000d980: 706f 7274 5f66 6f72 6d61 743a 2073 7472  port_format: str
+0000d990: 0a20 2020 2020 2020 2020 2020 203a 7265  .            :re
+0000d9a0: 7475 726e 3a20 7265 7370 6f6e 7365 0a20  turn: response. 
+0000d9b0: 2020 2020 2020 2020 2020 203a 7274 7970             :rtyp
+0000d9c0: 653a 2072 6571 7565 7374 732e 5265 7370  e: requests.Resp
+0000d9d0: 6f6e 7365 0a20 2020 2020 2020 2022 2222  onse.        """
+0000d9e0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+0000d9f0: 6520 3d20 7365 6c66 2e5f 5f75 7469 6c69  e = self.__utili
+0000da00: 7a65 5f64 796e 616d 6963 5f61 6e61 6c79  ze_dynamic_analy
+0000da10: 7369 735f 656e 6470 6f69 6e74 2873 616d  sis_endpoint(sam
+0000da20: 706c 655f 6861 7368 2c0a 2020 2020 2020  ple_hash,.      
 0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000da70: 2e5f 5f44 594e 414d 4943 5f41 4e41 4c59  .__DYNAMIC_ANALY
-0000da80: 5349 535f 5245 504f 5254 5f43 5245 4154  SIS_REPORT_CREAT
-0000da90: 455f 454e 4450 4f49 4e54 290a 2020 2020  E_ENDPOINT).    
-0000daa0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-0000dab0: 6e73 650a 0a20 2020 2064 6566 2063 6865  nse..    def che
-0000dac0: 636b 5f64 796e 616d 6963 5f61 6e61 6c79  ck_dynamic_analy
-0000dad0: 7369 735f 7265 706f 7274 5f73 7461 7475  sis_report_statu
-0000dae0: 7328 7365 6c66 2c20 7361 6d70 6c65 5f68  s(self, sample_h
-0000daf0: 6173 682c 2072 6570 6f72 745f 666f 726d  ash, report_form
-0000db00: 6174 293a 0a20 2020 2020 2020 2022 2222  at):.        """
-0000db10: 4163 6365 7074 7320 6120 7369 6e67 6c65  Accepts a single
-0000db20: 2068 6173 6820 7374 7269 6e67 2061 6e64   hash string and
-0000db30: 2072 6570 6f72 7420 666f 726d 6174 2070   report format p
-0000db40: 6172 616d 6574 6572 7320 7468 6174 2073  arameters that s
-0000db50: 686f 756c 6420 636f 7272 6573 706f 6e64  hould correspond
-0000db60: 2074 6f20 7468 6520 7061 7261 6d65 7465   to the paramete
-0000db70: 7273 2075 7365 6420 696e 0a20 2020 2020  rs used in.     
-0000db80: 2020 2074 6865 2072 6571 7565 7374 2077     the request w
-0000db90: 6974 6820 6372 6561 7465 5f64 796e 616d  ith create_dynam
-0000dba0: 6963 5f61 6e61 6c79 7369 735f 7265 706f  ic_analysis_repo
-0000dbb0: 7274 206d 6574 686f 642e 2054 6865 2072  rt method. The r
-0000dbc0: 6573 706f 6e73 6520 696e 636c 7564 6573  esponse includes
-0000dbd0: 2061 6e20 696e 666f 726d 6174 6976 650a   an informative.
-0000dbe0: 2020 2020 2020 2020 6d65 7373 6167 6520          message 
-0000dbf0: 6162 6f75 7420 7468 6520 7374 6174 7573  about the status
-0000dc00: 206f 6620 7468 6520 7265 706f 7274 2070   of the report p
-0000dc10: 7265 7669 6f75 736c 7920 7265 7175 6573  reviously reques
-0000dc20: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
-0000dc30: 203a 7061 7261 6d20 7361 6d70 6c65 5f68   :param sample_h
-0000dc40: 6173 683a 2068 6173 6820 7374 7269 6e67  ash: hash string
-0000dc50: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-0000dc60: 7065 2073 616d 706c 655f 6861 7368 3a20  pe sample_hash: 
-0000dc70: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-0000dc80: 3a70 6172 616d 2072 6570 6f72 745f 666f  :param report_fo
-0000dc90: 726d 6174 3a20 7265 706f 7274 2066 6f72  rmat: report for
-0000dca0: 6d61 7420 2827 6874 6d6c 2720 6f72 2027  mat ('html' or '
-0000dcb0: 7064 6627 290a 2020 2020 2020 2020 2020  pdf').          
-0000dcc0: 2020 3a72 7479 7065 2072 6570 6f72 745f    :rtype report_
-0000dcd0: 666f 726d 6174 3a20 7374 720a 2020 2020  format: str.    
-0000dce0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-0000dcf0: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
-0000dd00: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
-0000dd10: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
-0000dd20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000dd30: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-0000dd40: 656c 662e 5f5f 7574 696c 697a 655f 6479  elf.__utilize_dy
-0000dd50: 6e61 6d69 635f 616e 616c 7973 6973 5f65  namic_analysis_e
-0000dd60: 6e64 706f 696e 7428 7361 6d70 6c65 5f68  ndpoint(sample_h
-0000dd70: 6173 682c 0a20 2020 2020 2020 2020 2020  ash,.           
-0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddb0: 2072 6570 6f72 745f 666f 726d 6174 2c0a   report_format,.
+0000da60: 2020 2020 2020 7265 706f 7274 5f66 6f72        report_for
+0000da70: 6d61 742c 0a20 2020 2020 2020 2020 2020  mat,.           
+0000da80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dab0: 2073 656c 662e 5f5f 4459 4e41 4d49 435f   self.__DYNAMIC_
+0000dac0: 414e 414c 5953 4953 5f52 4550 4f52 545f  ANALYSIS_REPORT_
+0000dad0: 4352 4541 5445 5f45 4e44 504f 494e 5429  CREATE_ENDPOINT)
+0000dae0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000daf0: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
+0000db00: 6620 6368 6563 6b5f 6479 6e61 6d69 635f  f check_dynamic_
+0000db10: 616e 616c 7973 6973 5f72 6570 6f72 745f  analysis_report_
+0000db20: 7374 6174 7573 2873 656c 662c 2073 616d  status(self, sam
+0000db30: 706c 655f 6861 7368 2c20 7265 706f 7274  ple_hash, report
+0000db40: 5f66 6f72 6d61 7429 3a0a 2020 2020 2020  _format):.      
+0000db50: 2020 2222 2241 6363 6570 7473 2061 2073    """Accepts a s
+0000db60: 696e 676c 6520 6861 7368 2073 7472 696e  ingle hash strin
+0000db70: 6720 616e 6420 7265 706f 7274 2066 6f72  g and report for
+0000db80: 6d61 7420 7061 7261 6d65 7465 7273 2074  mat parameters t
+0000db90: 6861 7420 7368 6f75 6c64 2063 6f72 7265  hat should corre
+0000dba0: 7370 6f6e 6420 746f 2074 6865 2070 6172  spond to the par
+0000dbb0: 616d 6574 6572 7320 7573 6564 2069 6e0a  ameters used in.
+0000dbc0: 2020 2020 2020 2020 7468 6520 7265 7175          the requ
+0000dbd0: 6573 7420 7769 7468 2063 7265 6174 655f  est with create_
+0000dbe0: 6479 6e61 6d69 635f 616e 616c 7973 6973  dynamic_analysis
+0000dbf0: 5f72 6570 6f72 7420 6d65 7468 6f64 2e20  _report method. 
+0000dc00: 5468 6520 7265 7370 6f6e 7365 2069 6e63  The response inc
+0000dc10: 6c75 6465 7320 616e 2069 6e66 6f72 6d61  ludes an informa
+0000dc20: 7469 7665 0a20 2020 2020 2020 206d 6573  tive.        mes
+0000dc30: 7361 6765 2061 626f 7574 2074 6865 2073  sage about the s
+0000dc40: 7461 7475 7320 6f66 2074 6865 2072 6570  tatus of the rep
+0000dc50: 6f72 7420 7072 6576 696f 7573 6c79 2072  ort previously r
+0000dc60: 6571 7565 7374 6564 2e0a 2020 2020 2020  equested..      
+0000dc70: 2020 2020 2020 3a70 6172 616d 2073 616d        :param sam
+0000dc80: 706c 655f 6861 7368 3a20 6861 7368 2073  ple_hash: hash s
+0000dc90: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+0000dca0: 2020 3a74 7970 6520 7361 6d70 6c65 5f68    :type sample_h
+0000dcb0: 6173 683a 2073 7472 0a20 2020 2020 2020  ash: str.       
+0000dcc0: 2020 2020 203a 7061 7261 6d20 7265 706f       :param repo
+0000dcd0: 7274 5f66 6f72 6d61 743a 2072 6570 6f72  rt_format: repor
+0000dce0: 7420 666f 726d 6174 2028 2768 746d 6c27  t format ('html'
+0000dcf0: 206f 7220 2770 6466 2729 0a20 2020 2020   or 'pdf').     
+0000dd00: 2020 2020 2020 203a 7274 7970 6520 7265         :rtype re
+0000dd10: 706f 7274 5f66 6f72 6d61 743a 2073 7472  port_format: str
+0000dd20: 0a20 2020 2020 2020 2020 2020 203a 7265  .            :re
+0000dd30: 7475 726e 3a20 7265 7370 6f6e 7365 0a20  turn: response. 
+0000dd40: 2020 2020 2020 2020 2020 203a 7274 7970             :rtyp
+0000dd50: 653a 2072 6571 7565 7374 732e 5265 7370  e: requests.Resp
+0000dd60: 6f6e 7365 0a20 2020 2020 2020 2022 2222  onse.        """
+0000dd70: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+0000dd80: 6520 3d20 7365 6c66 2e5f 5f75 7469 6c69  e = self.__utili
+0000dd90: 7a65 5f64 796e 616d 6963 5f61 6e61 6c79  ze_dynamic_analy
+0000dda0: 7369 735f 656e 6470 6f69 6e74 2873 616d  sis_endpoint(sam
+0000ddb0: 706c 655f 6861 7368 2c0a 2020 2020 2020  ple_hash,.      
 0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000de00: 2e5f 5f44 594e 414d 4943 5f41 4e41 4c59  .__DYNAMIC_ANALY
-0000de10: 5349 535f 5245 504f 5254 5f53 5441 5455  SIS_REPORT_STATU
-0000de20: 535f 454e 4450 4f49 4e54 290a 2020 2020  S_ENDPOINT).    
-0000de30: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-0000de40: 6e73 650a 0a20 2020 2064 6566 2064 6f77  nse..    def dow
-0000de50: 6e6c 6f61 645f 6479 6e61 6d69 635f 616e  nload_dynamic_an
-0000de60: 616c 7973 6973 5f72 6570 6f72 7428 7365  alysis_report(se
-0000de70: 6c66 2c20 7361 6d70 6c65 5f68 6173 682c  lf, sample_hash,
-0000de80: 2072 6570 6f72 745f 666f 726d 6174 293a   report_format):
-0000de90: 0a20 2020 2020 2020 2022 2222 4163 6365  .        """Acce
-0000dea0: 7074 7320 6120 7369 6e67 6c65 2068 6173  pts a single has
-0000deb0: 6820 7374 7269 6e67 2061 6e64 2072 6570  h string and rep
-0000dec0: 6f72 7420 666f 726d 6174 2070 6172 616d  ort format param
-0000ded0: 6574 6572 7320 7468 6174 2073 686f 756c  eters that shoul
-0000dee0: 6420 636f 7272 6573 706f 6e64 2074 6f20  d correspond to 
-0000def0: 7468 6520 7061 7261 6d65 7465 7273 2075  the parameters u
-0000df00: 7365 6420 696e 0a20 2020 2020 2020 2074  sed in.        t
-0000df10: 6865 2072 6571 7565 7374 2077 6974 6820  he request with 
-0000df20: 6372 6561 7465 5f64 796e 616d 6963 5f61  create_dynamic_a
-0000df30: 6e61 6c79 7369 735f 7265 706f 7274 206d  nalysis_report m
-0000df40: 6574 686f 642e 0a20 2020 2020 2020 2020  ethod..         
-0000df50: 2020 203a 7061 7261 6d20 7361 6d70 6c65     :param sample
-0000df60: 5f68 6173 683a 2068 6173 6820 7374 7269  _hash: hash stri
-0000df70: 6e67 0a20 2020 2020 2020 2020 2020 203a  ng.            :
-0000df80: 7479 7065 2073 616d 706c 655f 6861 7368  type sample_hash
-0000df90: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-0000dfa0: 2020 3a70 6172 616d 2072 6570 6f72 745f    :param report_
-0000dfb0: 666f 726d 6174 3a20 7265 706f 7274 2066  format: report f
-0000dfc0: 6f72 6d61 7420 2827 6874 6d6c 2720 6f72  ormat ('html' or
-0000dfd0: 2027 7064 6627 290a 2020 2020 2020 2020   'pdf').        
-0000dfe0: 2020 2020 3a72 7479 7065 2072 6570 6f72      :rtype repor
-0000dff0: 745f 666f 726d 6174 3a20 7374 720a 2020  t_format: str.  
-0000e000: 2020 2020 2020 2020 2020 3a72 6574 7572            :retur
-0000e010: 6e3a 2072 6573 706f 6e73 650a 2020 2020  n: response.    
-0000e020: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-0000e030: 7265 7175 6573 7473 2e52 6573 706f 6e73  requests.Respons
-0000e040: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
-0000e050: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0000e060: 2073 656c 662e 5f5f 7574 696c 697a 655f   self.__utilize_
-0000e070: 6479 6e61 6d69 635f 616e 616c 7973 6973  dynamic_analysis
-0000e080: 5f65 6e64 706f 696e 7428 7361 6d70 6c65  _endpoint(sample
-0000e090: 5f68 6173 682c 0a20 2020 2020 2020 2020  _hash,.         
-0000e0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0d0: 2020 2072 6570 6f72 745f 666f 726d 6174     report_format
-0000e0e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ddf0: 2020 2020 2020 7265 706f 7274 5f66 6f72        report_for
+0000de00: 6d61 742c 0a20 2020 2020 2020 2020 2020  mat,.           
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de40: 2073 656c 662e 5f5f 4459 4e41 4d49 435f   self.__DYNAMIC_
+0000de50: 414e 414c 5953 4953 5f52 4550 4f52 545f  ANALYSIS_REPORT_
+0000de60: 5354 4154 5553 5f45 4e44 504f 494e 5429  STATUS_ENDPOINT)
+0000de70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000de80: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
+0000de90: 6620 646f 776e 6c6f 6164 5f64 796e 616d  f download_dynam
+0000dea0: 6963 5f61 6e61 6c79 7369 735f 7265 706f  ic_analysis_repo
+0000deb0: 7274 2873 656c 662c 2073 616d 706c 655f  rt(self, sample_
+0000dec0: 6861 7368 2c20 7265 706f 7274 5f66 6f72  hash, report_for
+0000ded0: 6d61 7429 3a0a 2020 2020 2020 2020 2222  mat):.        ""
+0000dee0: 2241 6363 6570 7473 2061 2073 696e 676c  "Accepts a singl
+0000def0: 6520 6861 7368 2073 7472 696e 6720 616e  e hash string an
+0000df00: 6420 7265 706f 7274 2066 6f72 6d61 7420  d report format 
+0000df10: 7061 7261 6d65 7465 7273 2074 6861 7420  parameters that 
+0000df20: 7368 6f75 6c64 2063 6f72 7265 7370 6f6e  should correspon
+0000df30: 6420 746f 2074 6865 2070 6172 616d 6574  d to the paramet
+0000df40: 6572 7320 7573 6564 2069 6e0a 2020 2020  ers used in.    
+0000df50: 2020 2020 7468 6520 7265 7175 6573 7420      the request 
+0000df60: 7769 7468 2063 7265 6174 655f 6479 6e61  with create_dyna
+0000df70: 6d69 635f 616e 616c 7973 6973 5f72 6570  mic_analysis_rep
+0000df80: 6f72 7420 6d65 7468 6f64 2e0a 2020 2020  ort method..    
+0000df90: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+0000dfa0: 616d 706c 655f 6861 7368 3a20 6861 7368  ample_hash: hash
+0000dfb0: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+0000dfc0: 2020 2020 3a74 7970 6520 7361 6d70 6c65      :type sample
+0000dfd0: 5f68 6173 683a 2073 7472 0a20 2020 2020  _hash: str.     
+0000dfe0: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
+0000dff0: 706f 7274 5f66 6f72 6d61 743a 2072 6570  port_format: rep
+0000e000: 6f72 7420 666f 726d 6174 2028 2768 746d  ort format ('htm
+0000e010: 6c27 206f 7220 2770 6466 2729 0a20 2020  l' or 'pdf').   
+0000e020: 2020 2020 2020 2020 203a 7274 7970 6520           :rtype 
+0000e030: 7265 706f 7274 5f66 6f72 6d61 743a 2073  report_format: s
+0000e040: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
+0000e050: 7265 7475 726e 3a20 7265 7370 6f6e 7365  return: response
+0000e060: 0a20 2020 2020 2020 2020 2020 203a 7274  .            :rt
+0000e070: 7970 653a 2072 6571 7565 7374 732e 5265  ype: requests.Re
+0000e080: 7370 6f6e 7365 0a20 2020 2020 2020 2022  sponse.        "
+0000e090: 2222 0a20 2020 2020 2020 2072 6573 706f  "".        respo
+0000e0a0: 6e73 6520 3d20 7365 6c66 2e5f 5f75 7469  nse = self.__uti
+0000e0b0: 6c69 7a65 5f64 796e 616d 6963 5f61 6e61  lize_dynamic_ana
+0000e0c0: 6c79 7369 735f 656e 6470 6f69 6e74 2873  lysis_endpoint(s
+0000e0d0: 616d 706c 655f 6861 7368 2c0a 2020 2020  ample_hash,.    
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e110: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e120: 6c66 2e5f 5f44 594e 414d 4943 5f41 4e41  lf.__DYNAMIC_ANA
-0000e130: 4c59 5349 535f 5245 504f 5254 5f44 4f57  LYSIS_REPORT_DOW
-0000e140: 4e4c 4f41 445f 454e 4450 4f49 4e54 290a  NLOAD_ENDPOINT).
-0000e150: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000e160: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
-0000e170: 2073 6574 5f63 6c61 7373 6966 6963 6174   set_classificat
-0000e180: 696f 6e28 7365 6c66 2c20 7361 6d70 6c65  ion(self, sample
-0000e190: 5f68 6173 682c 2063 6c61 7373 6966 6963  _hash, classific
-0000e1a0: 6174 696f 6e2c 2073 7973 7465 6d2c 2072  ation, system, r
-0000e1b0: 6973 6b5f 7363 6f72 653d 4e6f 6e65 2c20  isk_score=None, 
-0000e1c0: 7468 7265 6174 5f70 6c61 7466 6f72 6d3d  threat_platform=
-0000e1d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 2074 6872 6561 745f 7479 7065 3d4e 6f6e   threat_type=Non
-0000e200: 652c 2074 6872 6561 745f 6e61 6d65 3d4e  e, threat_name=N
-0000e210: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-0000e220: 2241 6363 6570 7473 2061 2073 696e 676c  "Accepts a singl
-0000e230: 6520 6861 7368 2073 7472 696e 672c 2061  e hash string, a
-0000e240: 6c6c 6f77 7320 7468 6520 7573 6572 2074  llows the user t
-0000e250: 6f20 7365 7420 7468 6520 636c 6173 7369  o set the classi
-0000e260: 6669 6361 7469 6f6e 206f 6620 6120 7361  fication of a sa
-0000e270: 6d70 6c65 2c20 6569 7468 6572 2069 6e20  mple, either in 
-0000e280: 5469 7461 6e69 756d 436c 6f75 640a 2020  TitaniumCloud.  
-0000e290: 2020 2020 2020 6f72 206c 6f63 616c 6c79        or locally
-0000e2a0: 206f 6e20 7468 6520 4131 3030 302e 2052   on the A1000. R
-0000e2b0: 6574 7572 6e73 2061 2072 6573 706f 6e73  eturns a respons
-0000e2c0: 6520 636f 6e74 6169 6e69 6e67 2061 206e  e containing a n
-0000e2d0: 6577 2063 6c61 7373 6966 6963 6174 696f  ew classificatio
-0000e2e0: 6e2e 0a20 2020 2020 2020 2020 2020 203a  n..            :
-0000e2f0: 7061 7261 6d20 7361 6d70 6c65 5f68 6173  param sample_has
-0000e300: 683a 2068 6173 6820 7374 7269 6e67 0a20  h: hash string. 
-0000e310: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-0000e320: 2073 616d 706c 655f 6861 7368 3a20 7374   sample_hash: st
-0000e330: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
-0000e340: 6172 616d 2073 7973 7465 6d3a 2027 6c6f  aram system: 'lo
-0000e350: 6361 6c27 206f 7220 2774 6963 6c6f 7564  cal' or 'ticloud
-0000e360: 270a 2020 2020 2020 2020 2020 2020 3a74  '.            :t
-0000e370: 7970 6520 7379 7374 656d 3a20 7374 720a  ype system: str.
-0000e380: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-0000e390: 616d 2063 6c61 7373 6966 6963 6174 696f  am classificatio
-0000e3a0: 6e3a 2027 676f 6f64 7761 7265 272c 2027  n: 'goodware', '
-0000e3b0: 7375 7370 6963 696f 7573 2720 6f72 2027  suspicious' or '
-0000e3c0: 6d61 6c69 6369 6f75 7327 0a20 2020 2020  malicious'.     
-0000e3d0: 2020 2020 2020 203a 7479 7065 2063 6c61         :type cla
-0000e3e0: 7373 6966 6963 6174 696f 6e3a 2073 7472  ssification: str
-0000e3f0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-0000e400: 7261 6d20 7269 736b 5f73 636f 7265 3a20  ram risk_score: 
-0000e410: 4966 2073 7065 6369 6669 6564 2c20 6974  If specified, it
-0000e420: 206d 7573 7420 6265 2077 6974 6869 6e20   must be within 
-0000e430: 7261 6e67 6520 666f 7220 7468 6520 7370  range for the sp
-0000e440: 6563 6966 6965 6420 636c 6173 7369 6669  ecified classifi
-0000e450: 6361 7469 6f6e 2e20 4966 206e 6f74 2073  cation. If not s
-0000e460: 7065 6369 6669 6564 2c0a 2020 2020 2020  pecified,.      
-0000e470: 2020 2020 2020 6120 6465 6661 756c 7420        a default 
-0000e480: 7661 6c75 6520 6973 2075 7365 643a 2047  value is used: G
-0000e490: 6f6f 6477 6172 653a 2030 2c20 5375 7370  oodware: 0, Susp
-0000e4a0: 6963 696f 7573 3a20 362c 204d 616c 6963  icious: 6, Malic
-0000e4b0: 696f 7573 3a20 3130 0a20 2020 2020 2020  ious: 10.       
-0000e4c0: 2020 2020 203a 7479 7065 2072 6973 6b5f       :type risk_
-0000e4d0: 7363 6f72 653a 2073 7472 0a20 2020 2020  score: str.     
-0000e4e0: 2020 2020 2020 203a 7061 7261 6d20 7468         :param th
-0000e4f0: 7265 6174 5f70 6c61 7466 6f72 6d3a 2069  reat_platform: i
-0000e500: 6620 7370 6563 6966 6965 642c 2069 7420  f specified, it 
-0000e510: 6d75 7374 2062 6520 6f6e 2074 6865 2073  must be on the s
-0000e520: 7570 706f 7274 6564 206c 6973 7420 2870  upported list (p
-0000e530: 6c61 7466 6f72 6d73 2061 6e64 2073 7562  latforms and sub
-0000e540: 706c 6174 666f 726d 7320 2d20 7365 650a  platforms - see.
-0000e550: 2020 2020 2020 2020 2020 2020 6f66 6669              offi
-0000e560: 6369 616c 2041 5049 2064 6f63 7329 2e20  cial API docs). 
-0000e570: 4966 206e 6f74 2073 7065 6369 6669 6564  If not specified
-0000e580: 2c20 7468 6520 6465 6661 756c 7420 7661  , the default va
-0000e590: 6c75 6520 6973 2027 5769 6e33 3227 2e0a  lue is 'Win32'..
-0000e5a0: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
-0000e5b0: 6520 7468 7265 6174 5f70 6c61 7466 6f72  e threat_platfor
-0000e5c0: 6d3a 2073 7472 0a20 2020 2020 2020 2020  m: str.         
-0000e5d0: 2020 203a 7061 7261 6d20 7468 7265 6174     :param threat
-0000e5e0: 5f74 7970 653a 2049 6620 7370 6563 6966  _type: If specif
-0000e5f0: 6965 642c 2069 7420 6d75 7374 2062 6520  ied, it must be 
-0000e600: 6f6e 2074 6865 2073 7570 706f 7274 6564  on the supported
-0000e610: 206c 6973 7420 286d 616c 7761 7265 2074   list (malware t
-0000e620: 7970 6573 202d 2073 6565 206f 6666 6963  ypes - see offic
-0000e630: 6961 6c20 4150 4920 646f 6373 292e 0a20  ial API docs).. 
-0000e640: 2020 2020 2020 2020 2020 2049 6620 6e6f             If no
-0000e650: 7420 7370 6563 6966 6965 642c 2074 6865  t specified, the
-0000e660: 2064 6566 6175 6c74 2076 616c 7565 2069   default value i
-0000e670: 7320 274d 616c 7761 7265 272e 0a20 2020  s 'Malware'..   
-0000e680: 2020 2020 2020 2020 203a 7479 7065 2074           :type t
-0000e690: 6872 6561 745f 7479 7065 3a20 7374 720a  hreat_type: str.
-0000e6a0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-0000e6b0: 616d 2074 6872 6561 745f 6e61 6d65 3a20  am threat_name: 
-0000e6c0: 4966 2073 7065 6369 6669 6564 2c20 6d75  If specified, mu
-0000e6d0: 7374 2062 6520 616e 2061 6c70 6861 6e75  st be an alphanu
-0000e6e0: 6d65 7269 6320 7374 7269 6e67 206e 6f74  meric string not
-0000e6f0: 206c 6f6e 6765 7220 7468 616e 2033 3220   longer than 32 
-0000e700: 6368 6172 6163 7465 7273 2e20 4966 206e  characters. If n
-0000e710: 6f74 0a20 2020 2020 2020 2020 2020 2073  ot.            s
-0000e720: 7065 6369 6669 6564 2c20 7468 6520 6465  pecified, the de
-0000e730: 6661 756c 7420 7661 6c75 6520 6973 2027  fault value is '
-0000e740: 4765 6e65 7269 6327 2e0a 2020 2020 2020  Generic'..      
-0000e750: 2020 2020 2020 3a74 7970 6520 7468 7265        :type thre
-0000e760: 6174 5f6e 616d 653a 2073 7472 0a20 2020  at_name: str.   
-0000e770: 2020 2020 2020 2020 203a 7265 7475 726e           :return
-0000e780: 3a20 7265 7370 6f6e 7365 0a20 2020 2020  : response.     
-0000e790: 2020 2020 2020 203a 7274 7970 653a 2072         :rtype: r
-0000e7a0: 6571 7565 7374 732e 5265 7370 6f6e 7365  equests.Response
-0000e7b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000e7c0: 2020 2020 2076 616c 6964 6174 655f 6861       validate_ha
-0000e7d0: 7368 6573 280a 2020 2020 2020 2020 2020  shes(.          
-0000e7e0: 2020 6861 7368 5f69 6e70 7574 3d5b 7361    hash_input=[sa
-0000e7f0: 6d70 6c65 5f68 6173 685d 2c0a 2020 2020  mple_hash],.    
-0000e800: 2020 2020 2020 2020 616c 6c6f 7765 645f          allowed_
-0000e810: 6861 7368 5f74 7970 6573 3d28 4d44 352c  hash_types=(MD5,
-0000e820: 2053 4841 312c 2053 4841 3235 362c 2053   SHA1, SHA256, S
-0000e830: 4841 3531 3229 0a20 2020 2020 2020 2029  HA512).        )
-0000e840: 0a0a 2020 2020 2020 2020 6966 2073 7973  ..        if sys
-0000e850: 7465 6d20 6e6f 7420 696e 2028 226c 6f63  tem not in ("loc
-0000e860: 616c 222c 2022 7469 636c 6f75 6422 293a  al", "ticloud"):
-0000e870: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000e880: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-0000e890: 6f72 2822 7379 7374 656d 2070 6172 616d  or("system param
-0000e8a0: 6574 6572 206d 7573 7420 6265 2065 6974  eter must be eit
-0000e8b0: 6865 7220 276c 6f63 616c 2720 6f72 2027  her 'local' or '
-0000e8c0: 7469 636c 6f75 6427 2e22 290a 0a20 2020  ticloud'.")..   
-0000e8d0: 2020 2020 2065 6e64 706f 696e 7420 3d20       endpoint = 
-0000e8e0: 7365 6c66 2e5f 5f53 4554 5f4f 525f 4445  self.__SET_OR_DE
-0000e8f0: 4c45 5445 5f43 4c41 5353 4946 4943 4154  LETE_CLASSIFICAT
-0000e900: 494f 4e5f 454e 4450 4f49 4e54 2e66 6f72  ION_ENDPOINT.for
-0000e910: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-0000e920: 2068 6173 685f 7661 6c75 653d 7361 6d70   hash_value=samp
-0000e930: 6c65 5f68 6173 682c 0a20 2020 2020 2020  le_hash,.       
-0000e940: 2020 2020 2073 7973 7465 6d3d 7379 7374       system=syst
-0000e950: 656d 0a20 2020 2020 2020 2029 0a0a 2020  em.        )..  
-0000e960: 2020 2020 2020 6461 7461 203d 2073 656c        data = sel
-0000e970: 662e 5f5f 6372 6561 7465 5f70 6f73 745f  f.__create_post_
-0000e980: 7061 796c 6f61 6428 0a20 2020 2020 2020  payload(.       
-0000e990: 2020 2020 2063 6c61 7373 6966 6963 6174       classificat
-0000e9a0: 696f 6e3d 636c 6173 7369 6669 6361 7469  ion=classificati
-0000e9b0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-0000e9c0: 7269 736b 5f73 636f 7265 3d72 6973 6b5f  risk_score=risk_
-0000e9d0: 7363 6f72 652c 0a20 2020 2020 2020 2020  score,.         
-0000e9e0: 2020 2074 6872 6561 745f 706c 6174 666f     threat_platfo
-0000e9f0: 726d 3d74 6872 6561 745f 706c 6174 666f  rm=threat_platfo
-0000ea00: 726d 2c0a 2020 2020 2020 2020 2020 2020  rm,.            
-0000ea10: 7468 7265 6174 5f74 7970 653d 7468 7265  threat_type=thre
-0000ea20: 6174 5f74 7970 652c 0a20 2020 2020 2020  at_type,.       
-0000ea30: 2020 2020 2074 6872 6561 745f 6e61 6d65       threat_name
-0000ea40: 3d74 6872 6561 745f 6e61 6d65 0a20 2020  =threat_name.   
-0000ea50: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000ea60: 7572 6c20 3d20 7365 6c66 2e5f 7572 6c2e  url = self._url.
-0000ea70: 666f 726d 6174 2865 6e64 706f 696e 743d  format(endpoint=
-0000ea80: 656e 6470 6f69 6e74 290a 0a20 2020 2020  endpoint)..     
-0000ea90: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-0000eaa0: 6c66 2e5f 5f70 6f73 745f 7265 7175 6573  lf.__post_reques
-0000eab0: 7428 7572 6c3d 7572 6c2c 2064 6174 613d  t(url=url, data=
-0000eac0: 6461 7461 290a 0a20 2020 2020 2020 2073  data)..        s
-0000ead0: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
-0000eae0: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
-0000eaf0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000eb00: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
-0000eb10: 2064 656c 6574 655f 636c 6173 7369 6669   delete_classifi
-0000eb20: 6361 7469 6f6e 2873 656c 662c 2073 616d  cation(self, sam
-0000eb30: 706c 655f 6861 7368 2c20 7379 7374 656d  ple_hash, system
-0000eb40: 3d22 6c6f 6361 6c22 293a 0a20 2020 2020  ="local"):.     
-0000eb50: 2020 2022 2222 4163 6365 7074 7320 6120     """Accepts a 
-0000eb60: 7369 6e67 6c65 2068 6173 6820 7374 7269  single hash stri
-0000eb70: 6e67 2c20 616c 6c6f 7773 2074 6865 2075  ng, allows the u
-0000eb80: 7365 7220 746f 2064 656c 6574 6520 7468  ser to delete th
-0000eb90: 6520 636c 6173 7369 6669 6361 7469 6f6e  e classification
-0000eba0: 206f 6620 6120 7361 6d70 6c65 2c20 6569   of a sample, ei
-0000ebb0: 7468 6572 2069 6e0a 2020 2020 2020 2020  ther in.        
-0000ebc0: 5469 7461 6e69 756d 436c 6f75 6420 6f72  TitaniumCloud or
-0000ebd0: 206c 6f63 616c 6c79 206f 6e20 7468 6520   locally on the 
-0000ebe0: 4131 3030 302e 0a20 2020 2020 2020 2020  A1000..         
-0000ebf0: 2020 203a 7061 7261 6d20 7361 6d70 6c65     :param sample
-0000ec00: 5f68 6173 683a 2068 6173 6820 7374 7269  _hash: hash stri
-0000ec10: 6e67 0a20 2020 2020 2020 2020 2020 203a  ng.            :
-0000ec20: 7479 7065 2073 616d 706c 655f 6861 7368  type sample_hash
-0000ec30: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-0000ec40: 2020 3a70 6172 616d 2073 7973 7465 6d3a    :param system:
-0000ec50: 2027 6c6f 6361 6c27 206f 7220 2774 6963   'local' or 'tic
-0000ec60: 6c6f 7564 270a 2020 2020 2020 2020 2020  loud'.          
-0000ec70: 2020 3a74 7970 6520 7379 7374 656d 3a20    :type system: 
-0000ec80: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-0000ec90: 3a72 6574 7572 6e3a 2072 6573 706f 6e73  :return: respons
-0000eca0: 650a 2020 2020 2020 2020 2020 2020 3a72  e.            :r
-0000ecb0: 7479 7065 3a20 7265 7175 6573 7473 2e52  type: requests.R
-0000ecc0: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-0000ecd0: 2222 220a 2020 2020 2020 2020 7661 6c69  """.        vali
-0000ece0: 6461 7465 5f68 6173 6865 7328 0a20 2020  date_hashes(.   
-0000ecf0: 2020 2020 2020 2020 2068 6173 685f 696e           hash_in
-0000ed00: 7075 743d 5b73 616d 706c 655f 6861 7368  put=[sample_hash
-0000ed10: 5d2c 0a20 2020 2020 2020 2020 2020 2061  ],.            a
-0000ed20: 6c6c 6f77 6564 5f68 6173 685f 7479 7065  llowed_hash_type
-0000ed30: 733d 284d 4435 2c20 5348 4131 2c20 5348  s=(MD5, SHA1, SH
-0000ed40: 4132 3536 2c20 5348 4135 3132 290a 2020  A256, SHA512).  
-0000ed50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000ed60: 2069 6620 7379 7374 656d 2061 6e64 2073   if system and s
-0000ed70: 7973 7465 6d20 6e6f 7420 696e 2028 226c  ystem not in ("l
-0000ed80: 6f63 616c 222c 2022 7469 636c 6f75 6422  ocal", "ticloud"
-0000ed90: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000eda0: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
-0000edb0: 7272 6f72 2822 7379 7374 656d 2070 6172  rror("system par
-0000edc0: 616d 6574 6572 206d 7573 7420 6265 2065  ameter must be e
-0000edd0: 6974 6865 7220 276c 6f63 616c 2720 6f72  ither 'local' or
-0000ede0: 2027 7469 636c 6f75 6427 2e22 290a 0a20   'ticloud'.").. 
-0000edf0: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
-0000ee00: 3d20 7365 6c66 2e5f 5f53 4554 5f4f 525f  = self.__SET_OR_
-0000ee10: 4445 4c45 5445 5f43 4c41 5353 4946 4943  DELETE_CLASSIFIC
-0000ee20: 4154 494f 4e5f 454e 4450 4f49 4e54 2e66  ATION_ENDPOINT.f
-0000ee30: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-0000ee40: 2020 2068 6173 685f 7661 6c75 653d 7361     hash_value=sa
-0000ee50: 6d70 6c65 5f68 6173 682c 0a20 2020 2020  mple_hash,.     
-0000ee60: 2020 2020 2020 2073 7973 7465 6d3d 7379         system=sy
-0000ee70: 7374 656d 0a20 2020 2020 2020 2029 0a0a  stem.        )..
-0000ee80: 2020 2020 2020 2020 7572 6c20 3d20 7365          url = se
-0000ee90: 6c66 2e5f 7572 6c2e 666f 726d 6174 2865  lf._url.format(e
-0000eea0: 6e64 706f 696e 743d 656e 6470 6f69 6e74  ndpoint=endpoint
-0000eeb0: 290a 0a20 2020 2020 2020 2072 6573 706f  )..        respo
-0000eec0: 6e73 6520 3d20 7365 6c66 2e5f 5f64 656c  nse = self.__del
-0000eed0: 6574 655f 7265 7175 6573 7428 7572 6c3d  ete_request(url=
-0000eee0: 7572 6c29 0a0a 2020 2020 2020 2020 7365  url)..        se
-0000eef0: 6c66 2e5f 5f72 6169 7365 5f6f 6e5f 6572  lf.__raise_on_er
-0000ef00: 726f 7228 7265 7370 6f6e 7365 290a 0a20  ror(response).. 
-0000ef10: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000ef20: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
-0000ef30: 6765 745f 7573 6572 5f74 6167 7328 7365  get_user_tags(se
-0000ef40: 6c66 2c20 7361 6d70 6c65 5f68 6173 6829  lf, sample_hash)
-0000ef50: 3a0a 2020 2020 2020 2020 2222 2241 6363  :.        """Acc
-0000ef60: 6570 7473 2061 2073 696e 676c 6520 6861  epts a single ha
-0000ef70: 7368 2073 7472 696e 6720 616e 6420 7265  sh string and re
-0000ef80: 7475 726e 7320 6c69 7374 7320 6f66 2065  turns lists of e
-0000ef90: 7869 7374 696e 6720 7573 6572 2074 6167  xisting user tag
-0000efa0: 7320 666f 7220 7468 6520 7265 7175 6573  s for the reques
-0000efb0: 7465 6420 7361 6d70 6c65 2e0a 2020 2020  ted sample..    
-0000efc0: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
-0000efd0: 6d70 6c65 5f68 6173 683a 2068 6173 6820  mple_hash: hash 
-0000efe0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-0000eff0: 2020 3a74 7970 6520 7361 6d70 6c65 5f68    :type sample_h
-0000f000: 6173 683a 2073 7472 0a20 2020 2020 2020  ash: str.       
-0000f010: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
-0000f020: 706f 6e73 650a 2020 2020 2020 2020 2020  ponse.          
-0000f030: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
-0000f040: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
-0000f050: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000f060: 2020 7661 6c69 6461 7465 5f68 6173 6865    validate_hashe
-0000f070: 7328 0a20 2020 2020 2020 2020 2020 2068  s(.            h
-0000f080: 6173 685f 696e 7075 743d 5b73 616d 706c  ash_input=[sampl
-0000f090: 655f 6861 7368 5d2c 0a20 2020 2020 2020  e_hash],.       
-0000f0a0: 2020 2020 2061 6c6c 6f77 6564 5f68 6173       allowed_has
-0000f0b0: 685f 7479 7065 733d 284d 4435 2c20 5348  h_types=(MD5, SH
-0000f0c0: 4131 2c20 5348 4132 3536 290a 2020 2020  A1, SHA256).    
-0000f0d0: 2020 2020 290a 0a20 2020 2020 2020 2065      )..        e
-0000f0e0: 6e64 706f 696e 7420 3d20 7365 6c66 2e5f  ndpoint = self._
-0000f0f0: 5f54 4147 535f 454e 4450 4f49 4e54 2e66  _TAGS_ENDPOINT.f
-0000f100: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-0000f110: 2020 2068 6173 685f 7661 6c75 653d 7361     hash_value=sa
-0000f120: 6d70 6c65 5f68 6173 680a 2020 2020 2020  mple_hash.      
-0000f130: 2020 290a 0a20 2020 2020 2020 2075 726c    )..        url
-0000f140: 203d 2073 656c 662e 5f75 726c 2e66 6f72   = self._url.for
-0000f150: 6d61 7428 656e 6470 6f69 6e74 3d65 6e64  mat(endpoint=end
-0000f160: 706f 696e 7429 0a0a 2020 2020 2020 2020  point)..        
-0000f170: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-0000f180: 5f5f 6765 745f 7265 7175 6573 7428 7572  __get_request(ur
-0000f190: 6c3d 7572 6c29 0a0a 2020 2020 2020 2020  l=url)..        
-0000f1a0: 7365 6c66 2e5f 5f72 6169 7365 5f6f 6e5f  self.__raise_on_
-0000f1b0: 6572 726f 7228 7265 7370 6f6e 7365 290a  error(response).
-0000f1c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000f1d0: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
-0000f1e0: 6620 706f 7374 5f75 7365 725f 7461 6773  f post_user_tags
-0000f1f0: 2873 656c 662c 2073 616d 706c 655f 6861  (self, sample_ha
-0000f200: 7368 2c20 7461 6773 293a 0a20 2020 2020  sh, tags):.     
-0000f210: 2020 2022 2222 4163 6365 7074 7320 6120     """Accepts a 
-0000f220: 7369 6e67 6c65 2068 6173 6820 7374 7269  single hash stri
-0000f230: 6e67 2061 6e64 2061 6464 7320 6f6e 6520  ng and adds one 
-0000f240: 6f72 206d 6f72 6520 7573 6572 2074 6167  or more user tag
-0000f250: 7320 746f 2074 6865 2072 6571 7565 7374  s to the request
-0000f260: 6564 2073 616d 706c 652e 0a20 2020 2020  ed sample..     
-0000f270: 2020 2020 2020 3a70 6172 616d 2073 616d        :param sam
-0000f280: 706c 655f 6861 7368 3a20 6861 7368 2073  ple_hash: hash s
-0000f290: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-0000f2a0: 203a 7479 7065 2073 616d 706c 655f 6861   :type sample_ha
-0000f2b0: 7368 3a20 7374 720a 2020 2020 2020 2020  sh: str.        
-0000f2c0: 2020 203a 7061 7261 6d20 7461 6773 3a20     :param tags: 
-0000f2d0: 6c69 7374 206f 6620 6861 7368 2073 7472  list of hash str
-0000f2e0: 696e 6773 0a20 2020 2020 2020 2020 2020  ings.           
-0000f2f0: 3a74 7970 6520 7461 6773 3a20 6c69 7374  :type tags: list
-0000f300: 5b73 7472 5d0a 2020 2020 2020 2020 2020  [str].          
-0000f310: 203a 7265 7475 726e 3a20 7265 7370 6f6e   :return: respon
-0000f320: 7365 0a20 2020 2020 2020 2020 2020 3a72  se.           :r
-0000f330: 7479 7065 3a20 7265 7175 6573 7473 2e52  type: requests.R
-0000f340: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-0000f350: 2222 220a 2020 2020 2020 2020 7661 6c69  """.        vali
-0000f360: 6461 7465 5f68 6173 6865 7328 0a20 2020  date_hashes(.   
-0000f370: 2020 2020 2020 2020 2068 6173 685f 696e           hash_in
-0000f380: 7075 743d 5b73 616d 706c 655f 6861 7368  put=[sample_hash
-0000f390: 5d2c 0a20 2020 2020 2020 2020 2020 2061  ],.            a
-0000f3a0: 6c6c 6f77 6564 5f68 6173 685f 7479 7065  llowed_hash_type
-0000f3b0: 733d 284d 4435 2c20 5348 4131 2c20 5348  s=(MD5, SHA1, SH
-0000f3c0: 4132 3536 290a 2020 2020 2020 2020 290a  A256).        ).
-0000f3d0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000f3e0: 6973 696e 7374 616e 6365 2874 6167 732c  isinstance(tags,
-0000f3f0: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
-0000f400: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-0000f410: 6e70 7574 4572 726f 7228 2274 6167 7320  nputError("tags 
-0000f420: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
-0000f430: 6520 6120 6c69 7374 206f 6620 7374 7269  e a list of stri
-0000f440: 6e67 732e 2229 0a0a 2020 2020 2020 2020  ngs.")..        
-0000f450: 656e 6470 6f69 6e74 203d 2073 656c 662e  endpoint = self.
-0000f460: 5f5f 5441 4753 5f45 4e44 504f 494e 542e  __TAGS_ENDPOINT.
-0000f470: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-0000f480: 2020 2020 6861 7368 5f76 616c 7565 3d73      hash_value=s
-0000f490: 616d 706c 655f 6861 7368 0a20 2020 2020  ample_hash.     
-0000f4a0: 2020 2029 0a0a 2020 2020 2020 2020 706f     )..        po
-0000f4b0: 7374 5f6a 736f 6e20 3d20 7b22 7461 6773  st_json = {"tags
-0000f4c0: 223a 2074 6167 737d 0a0a 2020 2020 2020  ": tags}..      
-0000f4d0: 2020 7572 6c20 3d20 7365 6c66 2e5f 7572    url = self._ur
-0000f4e0: 6c2e 666f 726d 6174 2865 6e64 706f 696e  l.format(endpoin
-0000f4f0: 743d 656e 6470 6f69 6e74 290a 0a20 2020  t=endpoint)..   
-0000f500: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-0000f510: 7365 6c66 2e5f 5f70 6f73 745f 7265 7175  self.__post_requ
-0000f520: 6573 7428 7572 6c3d 7572 6c2c 2070 6f73  est(url=url, pos
-0000f530: 745f 6a73 6f6e 3d70 6f73 745f 6a73 6f6e  t_json=post_json
-0000f540: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000f550: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
-0000f560: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
-0000f570: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-0000f580: 6e73 650a 0a20 2020 2064 6566 2064 656c  nse..    def del
-0000f590: 6574 655f 7573 6572 5f74 6167 7328 7365  ete_user_tags(se
-0000f5a0: 6c66 2c20 7361 6d70 6c65 5f68 6173 682c  lf, sample_hash,
-0000f5b0: 2074 6167 7329 3a0a 2020 2020 2020 2020   tags):.        
-0000f5c0: 2222 2241 6363 6570 7473 2061 2073 696e  """Accepts a sin
-0000f5d0: 676c 6520 6861 7368 2073 7472 696e 6720  gle hash string 
-0000f5e0: 616e 6420 7265 6d6f 7665 7320 6f6e 6520  and removes one 
-0000f5f0: 6f72 206d 6f72 6520 7573 6572 2074 6167  or more user tag
-0000f600: 7320 6672 6f6d 2074 6865 2072 6571 7565  s from the reque
-0000f610: 7374 6564 2073 616d 706c 652e 0a20 2020  sted sample..   
-0000f620: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0000f630: 616d 706c 655f 6861 7368 3a20 6861 7368  ample_hash: hash
-0000f640: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-0000f650: 2020 203a 7479 7065 2073 616d 706c 655f     :type sample_
-0000f660: 6861 7368 3a20 7374 720a 2020 2020 2020  hash: str.      
-0000f670: 2020 2020 203a 7061 7261 6d20 7461 6773       :param tags
-0000f680: 3a20 6c69 7374 206f 6620 6861 7368 2073  : list of hash s
-0000f690: 7472 696e 6773 0a20 2020 2020 2020 2020  trings.         
-0000f6a0: 2020 3a74 7970 6520 7461 6773 3a20 6c69    :type tags: li
-0000f6b0: 7374 5b73 7472 5d0a 2020 2020 2020 2020  st[str].        
-0000f6c0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
-0000f6d0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
-0000f6e0: 3a72 7479 7065 3a20 7265 7175 6573 7473  :rtype: requests
-0000f6f0: 2e52 6573 706f 6e73 650a 2020 2020 2020  .Response.      
-0000f700: 2020 2222 220a 2020 2020 2020 2020 7661    """.        va
-0000f710: 6c69 6461 7465 5f68 6173 6865 7328 0a20  lidate_hashes(. 
-0000f720: 2020 2020 2020 2020 2020 2068 6173 685f             hash_
-0000f730: 696e 7075 743d 5b73 616d 706c 655f 6861  input=[sample_ha
-0000f740: 7368 5d2c 0a20 2020 2020 2020 2020 2020  sh],.           
-0000f750: 2061 6c6c 6f77 6564 5f68 6173 685f 7479   allowed_hash_ty
-0000f760: 7065 733d 284d 4435 2c20 5348 4131 2c20  pes=(MD5, SHA1, 
-0000f770: 5348 4132 3536 290a 2020 2020 2020 2020  SHA256).        
-0000f780: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-0000f790: 7420 6973 696e 7374 616e 6365 2874 6167  t isinstance(tag
-0000f7a0: 732c 206c 6973 7429 3a0a 2020 2020 2020  s, list):.      
-0000f7b0: 2020 2020 2020 7261 6973 6520 5772 6f6e        raise Wron
-0000f7c0: 6749 6e70 7574 4572 726f 7228 2274 6167  gInputError("tag
-0000f7d0: 7320 7061 7261 6d65 7465 7220 6d75 7374  s parameter must
-0000f7e0: 2062 6520 6120 6c69 7374 206f 6620 7374   be a list of st
-0000f7f0: 7269 6e67 732e 2229 0a0a 2020 2020 2020  rings.")..      
-0000f800: 2020 656e 6470 6f69 6e74 203d 2073 656c    endpoint = sel
-0000f810: 662e 5f5f 5441 4753 5f45 4e44 504f 494e  f.__TAGS_ENDPOIN
-0000f820: 542e 666f 726d 6174 280a 2020 2020 2020  T.format(.      
-0000f830: 2020 2020 2020 6861 7368 5f76 616c 7565        hash_value
-0000f840: 3d73 616d 706c 655f 6861 7368 0a20 2020  =sample_hash.   
-0000f850: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000f860: 706f 7374 5f6a 736f 6e20 3d20 7b22 7461  post_json = {"ta
-0000f870: 6773 223a 2074 6167 737d 0a0a 2020 2020  gs": tags}..    
-0000f880: 2020 2020 7572 6c20 3d20 7365 6c66 2e5f      url = self._
-0000f890: 7572 6c2e 666f 726d 6174 2865 6e64 706f  url.format(endpo
-0000f8a0: 696e 743d 656e 6470 6f69 6e74 290a 0a20  int=endpoint).. 
-0000f8b0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0000f8c0: 3d20 7365 6c66 2e5f 5f64 656c 6574 655f  = self.__delete_
-0000f8d0: 7265 7175 6573 7428 7572 6c3d 7572 6c2c  request(url=url,
-0000f8e0: 2070 6f73 745f 6a73 6f6e 3d70 6f73 745f   post_json=post_
-0000f8f0: 6a73 6f6e 290a 0a20 2020 2020 2020 2073  json)..        s
-0000f900: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
-0000f910: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
-0000f920: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000f930: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
-0000f940: 2067 6574 5f79 6172 615f 7275 6c65 7365   get_yara_rulese
-0000f950: 7473 5f6f 6e5f 7468 655f 6170 706c 6961  ts_on_the_applia
-0000f960: 6e63 655f 7632 2873 656c 662c 206f 776e  nce_v2(self, own
-0000f970: 6572 5f74 7970 653d 4e6f 6e65 2c20 7374  er_type=None, st
-0000f980: 6174 7573 3d4e 6f6e 652c 2073 6f75 7263  atus=None, sourc
-0000f990: 653d 4e6f 6e65 2c20 7061 6765 3d4e 6f6e  e=None, page=Non
-0000f9a0: 652c 2070 6167 655f 7369 7a65 3d4e 6f6e  e, page_size=Non
-0000f9b0: 6529 3a0a 2020 2020 2020 2020 2222 2252  e):.        """R
-0000f9c0: 6574 7269 6576 6573 2061 206c 6973 7420  etrieves a list 
-0000f9d0: 6f66 2059 4152 4120 7275 6c65 7365 7473  of YARA rulesets
-0000f9e0: 2074 6861 7420 6172 6520 6f6e 2074 6865   that are on the
-0000f9f0: 2041 3130 3030 2061 7070 6c69 616e 6365   A1000 appliance
-0000fa00: 2e20 5468 6520 6c69 7374 2063 616e 2062  . The list can b
-0000fa10: 6520 6669 6c74 6572 6564 2062 7920 7365  e filtered by se
-0000fa20: 7665 7261 6c0a 2020 2020 2020 2020 6372  veral.        cr
-0000fa30: 6974 6572 6961 2028 7275 6c65 7365 7420  iteria (ruleset 
-0000fa40: 7374 6174 7573 2c20 736f 7572 6365 2c20  status, source, 
-0000fa50: 616e 6420 6f77 6e65 7229 2075 7369 6e67  and owner) using
-0000fa60: 206f 7074 696f 6e61 6c20 7061 7261 6d65   optional parame
-0000fa70: 7465 7273 2e0a 2020 2020 2020 2020 2020  ters..          
-0000fa80: 2020 3a70 6172 616d 206f 776e 6572 5f74    :param owner_t
-0000fa90: 7970 653a 2073 7570 706f 7274 6564 2076  ype: supported v
-0000faa0: 616c 7565 733a 206d 7920 2864 6566 6175  alues: my (defau
-0000fab0: 6c74 202d 2063 7572 7265 6e74 6c79 2061  lt - currently a
-0000fac0: 7574 6865 6e74 6963 6174 6564 2075 7365  uthenticated use
-0000fad0: 7229 2c20 7573 6572 2c20 7379 7374 656d  r), user, system
-0000fae0: 2c20 616c 6c0a 2020 2020 2020 2020 2020  , all.          
-0000faf0: 2020 3a74 7970 6520 6f77 6e65 725f 7479    :type owner_ty
-0000fb00: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-0000fb10: 2020 2020 3a70 6172 616d 2073 7461 7475      :param statu
-0000fb20: 733a 2073 7570 706f 7274 6564 2076 616c  s: supported val
-0000fb30: 7565 733a 2061 6c6c 2028 6465 6661 756c  ues: all (defaul
-0000fb40: 7429 2c20 6572 726f 722c 2061 6374 6976  t), error, activ
-0000fb50: 652c 2064 6973 6162 6c65 642c 2070 656e  e, disabled, pen
-0000fb60: 6469 6e67 2c20 696e 7661 6c69 642c 2063  ding, invalid, c
-0000fb70: 6170 7065 640a 2020 2020 2020 2020 2020  apped.          
-0000fb80: 2020 3a74 7970 6520 7374 6174 7573 3a20    :type status: 
-0000fb90: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-0000fba0: 3a70 6172 616d 2073 6f75 7263 653a 2073  :param source: s
-0000fbb0: 7570 706f 7274 6564 2076 616c 7565 733a  upported values:
-0000fbc0: 2061 6c6c 2028 6465 6661 756c 7429 2c20   all (default), 
-0000fbd0: 6c6f 6361 6c2c 2063 6c6f 7564 0a20 2020  local, cloud.   
-0000fbe0: 2020 2020 2020 2020 203a 7479 7065 2073           :type s
-0000fbf0: 6f75 7263 653a 2073 7472 0a20 2020 2020  ource: str.     
-0000fc00: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
-0000fc10: 6765 3a20 7768 656e 2074 6869 7320 7061  ge: when this pa
-0000fc20: 7261 6d65 7465 7220 6973 206f 6d69 7474  rameter is omitt
-0000fc30: 6564 2066 726f 6d20 7468 6520 7265 7175  ed from the requ
-0000fc40: 6573 742c 2061 6c6c 2061 7661 696c 6162  est, all availab
-0000fc50: 6c65 2072 6573 756c 7473 2061 7265 2072  le results are r
-0000fc60: 6574 7572 6e65 6420 6174 206f 6e63 650a  eturned at once.
-0000fc70: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
-0000fc80: 6520 7061 6765 3a20 7374 720a 2020 2020  e page: str.    
-0000fc90: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-0000fca0: 6167 655f 7369 7a65 3a20 7061 7261 6d65  age_size: parame
-0000fcb0: 7465 7220 7468 6174 2063 6f6e 7472 6f6c  ter that control
-0000fcc0: 7320 686f 7720 6d61 6e79 2072 6573 756c  s how many resul
-0000fcd0: 7473 2074 6f20 7265 7475 726e 2070 6572  ts to return per
-0000fce0: 2070 6167 6520 696e 2074 6865 2072 6573   page in the res
-0000fcf0: 706f 6e73 650a 2020 2020 2020 2020 2020  ponse.          
-0000fd00: 2020 3a74 7970 6520 7061 6765 5f73 697a    :type page_siz
-0000fd10: 653a 2073 7472 0a20 2020 2020 2020 2020  e: str.         
-0000fd20: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
-0000fd30: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
-0000fd40: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
-0000fd50: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
-0000fd60: 2020 2022 2222 0a20 2020 2020 2020 2070     """.        p
-0000fd70: 6172 616d 7320 3d20 7b22 7479 7065 223a  arams = {"type":
-0000fd80: 206f 776e 6572 5f74 7970 652c 2022 7374   owner_type, "st
-0000fd90: 6174 7573 223a 2073 7461 7475 732c 2022  atus": status, "
-0000fda0: 736f 7572 6365 223a 2073 6f75 7263 652c  source": source,
-0000fdb0: 2022 7061 6765 223a 2070 6167 652c 2022   "page": page, "
-0000fdc0: 7061 6765 5f73 697a 6522 3a20 7061 6765  page_size": page
-0000fdd0: 5f73 697a 657d 0a20 2020 2020 2020 2070  _size}.        p
-0000fde0: 6172 616d 735f 7374 7269 6e67 5f61 7272  arams_string_arr
-0000fdf0: 6179 203d 205b 5d0a 0a20 2020 2020 2020  ay = []..       
-0000fe00: 2069 6620 626f 6f6c 2870 6172 616d 735b   if bool(params[
-0000fe10: 2270 6167 6522 5d29 2021 3d20 626f 6f6c  "page"]) != bool
-0000fe20: 2870 6172 616d 735b 2270 6167 655f 7369  (params["page_si
-0000fe30: 7a65 225d 293a 0a20 2020 2020 2020 2020  ze"]):.         
-0000fe40: 2020 2072 6169 7365 2057 726f 6e67 496e     raise WrongIn
-0000fe50: 7075 7445 7272 6f72 2822 7061 6765 2061  putError("page a
-0000fe60: 6e64 2070 6167 655f 7369 7a65 2070 6172  nd page_size par
-0000fe70: 616d 6574 6573 206d 7573 7420 6265 2075  ametes must be u
-0000fe80: 7365 6420 746f 6765 7468 6572 2229 0a0a  sed together")..
-0000fe90: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
-0000fea0: 2076 616c 2069 6e20 7061 7261 6d73 2e69   val in params.i
-0000feb0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-0000fec0: 2020 2020 6966 2076 616c 3a0a 2020 2020      if val:.    
-0000fed0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000fee0: 6f74 2069 7369 6e73 7461 6e63 6528 7661  ot isinstance(va
-0000fef0: 6c2c 2073 7472 293a 0a20 2020 2020 2020  l, str):.       
-0000ff00: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000ff10: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-0000ff20: 6f72 2822 7b6b 6579 7d20 7061 7261 6d65  or("{key} parame
-0000ff30: 7465 7220 6d75 7374 2062 6520 6120 7374  ter must be a st
-0000ff40: 7269 6e67 222e 666f 726d 6174 286b 6579  ring".format(key
-0000ff50: 3d6b 6579 2929 0a20 2020 2020 2020 2020  =key)).         
-0000ff60: 2020 2020 2020 2070 6172 616d 735f 7374         params_st
-0000ff70: 7269 6e67 5f61 7272 6179 2e61 7070 656e  ring_array.appen
-0000ff80: 6428 227b 6b65 797d 3d7b 7661 6c7d 222e  d("{key}={val}".
-0000ff90: 666f 726d 6174 286b 6579 3d6b 6579 2c20  format(key=key, 
-0000ffa0: 7661 6c3d 7661 6c29 290a 0a20 2020 2020  val=val))..     
-0000ffb0: 2020 2069 6620 6c65 6e28 7061 7261 6d73     if len(params
-0000ffc0: 5f73 7472 696e 675f 6172 7261 7929 203e  _string_array) >
-0000ffd0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-0000ffe0: 7175 6572 795f 7374 7269 6e67 203d 2022  query_string = "
-0000fff0: 2622 2e6a 6f69 6e28 7061 7261 6d73 5f73  &".join(params_s
-00010000: 7472 696e 675f 6172 7261 7929 0a20 2020  tring_array).   
-00010010: 2020 2020 2020 2020 2065 6e64 706f 696e           endpoin
-00010020: 7420 3d20 227b 656e 6470 6f69 6e74 7d3f  t = "{endpoint}?
-00010030: 7b71 7565 7279 5f73 7472 696e 677d 222e  {query_string}".
-00010040: 666f 726d 6174 2865 6e64 706f 696e 743d  format(endpoint=
-00010050: 7365 6c66 2e5f 5f52 4554 5249 4556 455f  self.__RETRIEVE_
-00010060: 5941 5241 5f52 554c 4553 4554 535f 454e  YARA_RULESETS_EN
-00010070: 4450 4f49 4e54 5f56 322c 0a20 2020 2020  DPOINT_V2,.     
-00010080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100b0: 2020 2020 2071 7565 7279 5f73 7472 696e       query_strin
-000100c0: 673d 7175 6572 795f 7374 7269 6e67 290a  g=query_string).
-000100d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000100e0: 2020 2020 2020 2020 2020 656e 6470 6f69            endpoi
-000100f0: 6e74 203d 2073 656c 662e 5f5f 5245 5452  nt = self.__RETR
-00010100: 4945 5645 5f59 4152 415f 5255 4c45 5345  IEVE_YARA_RULESE
-00010110: 5453 5f45 4e44 504f 494e 545f 5632 0a0a  TS_ENDPOINT_V2..
-00010120: 2020 2020 2020 2020 7572 6c20 3d20 7365          url = se
-00010130: 6c66 2e5f 7572 6c2e 666f 726d 6174 2865  lf._url.format(e
-00010140: 6e64 706f 696e 743d 656e 6470 6f69 6e74  ndpoint=endpoint
-00010150: 290a 0a20 2020 2020 2020 2072 6573 706f  )..        respo
-00010160: 6e73 6520 3d20 7365 6c66 2e5f 5f67 6574  nse = self.__get
-00010170: 5f72 6571 7565 7374 2875 726c 3d75 726c  _request(url=url
-00010180: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00010190: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
-000101a0: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
-000101b0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-000101c0: 6e73 650a 0a20 2020 2064 6566 2067 6574  nse..    def get
-000101d0: 5f79 6172 615f 7275 6c65 7365 745f 636f  _yara_ruleset_co
-000101e0: 6e74 656e 7473 2873 656c 662c 2072 756c  ntents(self, rul
-000101f0: 6573 6574 5f6e 616d 6529 3a0a 2020 2020  eset_name):.    
-00010200: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010210: 5265 7472 6965 7665 7320 7468 6520 6675  Retrieves the fu
-00010220: 6c6c 2063 6f6e 7465 6e74 7320 6f66 2074  ll contents of t
-00010230: 6865 2072 6571 7565 7374 6564 2072 756c  he requested rul
-00010240: 6573 6574 2069 6e20 7261 7720 7465 7874  eset in raw text
-00010250: 2f70 6c61 696e 2066 6f72 6d61 742e 2041  /plain format. A
-00010260: 6c6c 2072 756c 6573 6574 7320 6361 6e20  ll rulesets can 
-00010270: 6265 2072 6574 7269 6576 6564 2c0a 2020  be retrieved,.  
-00010280: 2020 2020 2020 7265 6761 7264 6c65 7373        regardless
-00010290: 206f 6620 7468 6569 7220 6375 7272 656e   of their curren
-000102a0: 7420 7374 6174 7573 206f 6e20 7468 6520  t status on the 
-000102b0: 6170 706c 6961 6e63 6520 2865 6e61 626c  appliance (enabl
-000102c0: 6564 2c20 6469 7361 626c 6564 e280 a629  ed, disabled...)
-000102d0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-000102e0: 7261 6d20 7275 6c65 7365 745f 6e61 6d65  ram ruleset_name
-000102f0: 3a20 6e61 6d65 206f 6620 7468 6520 5941  : name of the YA
-00010300: 5241 2072 756c 6573 6574 2074 6f20 7265  RA ruleset to re
-00010310: 7472 6965 7665 2e20 5275 6c65 7365 7420  trieve. Ruleset 
-00010320: 6e61 6d65 7320 6172 6520 6361 7365 2d73  names are case-s
-00010330: 656e 7369 7469 7665 0a20 2020 2020 2020  ensitive.       
-00010340: 2020 2020 203a 7479 7065 2072 756c 6573       :type rules
-00010350: 6574 5f6e 616d 653a 2073 7472 0a20 2020  et_name: str.   
-00010360: 2020 2020 2020 2020 203a 7265 7475 726e           :return
-00010370: 3a20 7265 7370 6f6e 7365 0a20 2020 2020  : response.     
-00010380: 2020 2020 2020 203a 7274 7970 653a 2072         :rtype: r
-00010390: 6571 7565 7374 732e 5265 7370 6f6e 7365  equests.Response
-000103a0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000103b0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-000103c0: 6e73 7461 6e63 6528 7275 6c65 7365 745f  nstance(ruleset_
-000103d0: 6e61 6d65 2c20 7374 7229 3a0a 2020 2020  name, str):.    
-000103e0: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
-000103f0: 6f6e 6749 6e70 7574 4572 726f 7228 2272  ongInputError("r
-00010400: 756c 6573 6574 5f6e 616d 6520 7061 7261  uleset_name para
-00010410: 6d65 7465 7220 6d75 7374 2062 6520 6120  meter must be a 
-00010420: 7374 7269 6e67 2229 0a0a 2020 2020 2020  string")..      
-00010430: 2020 656e 6470 6f69 6e74 203d 2073 656c    endpoint = sel
-00010440: 662e 5f5f 5245 5452 4945 5645 5f59 4152  f.__RETRIEVE_YAR
-00010450: 415f 5255 4c45 5345 545f 434f 4e54 454e  A_RULESET_CONTEN
-00010460: 5453 5f45 4e44 504f 494e 542e 666f 726d  TS_ENDPOINT.form
-00010470: 6174 2872 756c 6573 6574 5f6e 616d 653d  at(ruleset_name=
-00010480: 7275 6c65 7365 745f 6e61 6d65 290a 0a20  ruleset_name).. 
-00010490: 2020 2020 2020 2075 726c 203d 2073 656c         url = sel
-000104a0: 662e 5f75 726c 2e66 6f72 6d61 7428 656e  f._url.format(en
-000104b0: 6470 6f69 6e74 3d65 6e64 706f 696e 7429  dpoint=endpoint)
-000104c0: 0a0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-000104d0: 7365 203d 2073 656c 662e 5f5f 6765 745f  se = self.__get_
-000104e0: 7265 7175 6573 7428 7572 6c3d 7572 6c29  request(url=url)
-000104f0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00010500: 5f72 6169 7365 5f6f 6e5f 6572 726f 7228  _raise_on_error(
-00010510: 7265 7370 6f6e 7365 290a 0a20 2020 2020  response)..     
-00010520: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-00010530: 7365 0a0a 2020 2020 6465 6620 6765 745f  se..    def get_
-00010540: 7961 7261 5f72 756c 6573 6574 5f6d 6174  yara_ruleset_mat
-00010550: 6368 6573 5f76 3228 7365 6c66 2c20 7275  ches_v2(self, ru
-00010560: 6c65 7365 745f 6e61 6d65 2c20 7061 6765  leset_name, page
-00010570: 3d4e 6f6e 652c 2070 6167 655f 7369 7a65  =None, page_size
-00010580: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00010590: 2222 2252 6574 7269 6576 6573 2074 6865  """Retrieves the
-000105a0: 206c 6973 7420 6f66 2059 4152 4120 6d61   list of YARA ma
-000105b0: 7463 6865 7320 2862 6f74 6820 6c6f 6361  tches (both loca
-000105c0: 6c20 616e 6420 636c 6f75 6429 2066 6f72  l and cloud) for
-000105d0: 2072 6571 7565 7374 6564 2072 756c 6573   requested rules
-000105e0: 6574 732e 2049 6620 6d75 6c74 6970 6c65  ets. If multiple
-000105f0: 2072 756c 6573 6574 7320 6172 650a 2020   rulesets are.  
-00010600: 2020 2020 2020 7072 6f76 6964 6564 2069        provided i
-00010610: 6e20 7468 6520 7265 7175 6573 742c 206f  n the request, o
-00010620: 6e6c 7920 7468 6520 7361 6d70 6c65 7320  nly the samples 
-00010630: 7468 6174 206d 6174 6368 2061 6c6c 2072  that match all r
-00010640: 6571 7565 7374 6564 2072 756c 6573 6574  equested ruleset
-00010650: 7320 6172 6520 6c69 7374 6564 2069 6e20  s are listed in 
-00010660: 7468 6520 7265 7370 6f6e 7365 2e0a 2020  the response..  
-00010670: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00010680: 2072 756c 6573 6574 5f6e 616d 653a 0a20   ruleset_name:. 
-00010690: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-000106a0: 2072 756c 6573 6574 5f6e 616d 653a 2073   ruleset_name: s
-000106b0: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
-000106c0: 7061 7261 6d20 7061 6765 3a20 7768 656e  param page: when
-000106d0: 2074 6869 7320 7061 7261 6d65 7465 7220   this parameter 
-000106e0: 6973 206f 6d69 7474 6564 2066 726f 6d20  is omitted from 
-000106f0: 7468 6520 7265 7175 6573 742c 2061 6c6c  the request, all
-00010700: 2061 7661 696c 6162 6c65 2072 6573 756c   available resul
-00010710: 7473 2061 7265 2072 6574 7572 6e65 6420  ts are returned 
-00010720: 6174 206f 6e63 650a 2020 2020 2020 2020  at once.        
-00010730: 2020 2020 3a74 7970 6520 7061 6765 3a20      :type page: 
-00010740: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-00010750: 3a70 6172 616d 2070 6167 655f 7369 7a65  :param page_size
-00010760: 3a20 7061 7261 6d65 7465 7220 7468 6174  : parameter that
-00010770: 2063 6f6e 7472 6f6c 7320 686f 7720 6d61   controls how ma
-00010780: 6e79 2072 6573 756c 7473 2074 6f20 7265  ny results to re
-00010790: 7475 726e 2070 6572 2070 6167 6520 696e  turn per page in
-000107a0: 2074 6865 2072 6573 706f 6e73 650a 2020   the response.  
-000107b0: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
-000107c0: 7061 6765 5f73 697a 653a 2073 7472 0a20  page_size: str. 
-000107d0: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
-000107e0: 726e 3a20 7265 7370 6f6e 7365 0a20 2020  rn: response.   
-000107f0: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
-00010800: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
-00010810: 7365 3a0a 2020 2020 2020 2020 2222 220a  se:.        """.
-00010820: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-00010830: 207b 226e 616d 6522 3a20 7275 6c65 7365   {"name": rulese
-00010840: 745f 6e61 6d65 2c20 2270 6167 6522 3a20  t_name, "page": 
-00010850: 7061 6765 2c20 2270 6167 655f 7369 7a65  page, "page_size
-00010860: 223a 2070 6167 655f 7369 7a65 7d0a 2020  ": page_size}.  
-00010870: 2020 2020 2020 7061 7261 6d73 5f73 7472        params_str
-00010880: 696e 675f 6172 7261 7920 3d20 5b5d 0a0a  ing_array = []..
-00010890: 2020 2020 2020 2020 6966 2062 6f6f 6c28          if bool(
-000108a0: 7061 7261 6d73 5b22 7061 6765 225d 2920  params["page"]) 
-000108b0: 213d 2062 6f6f 6c28 7061 7261 6d73 5b22  != bool(params["
-000108c0: 7061 6765 5f73 697a 6522 5d29 3a0a 2020  page_size"]):.  
-000108d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000108e0: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
-000108f0: 2270 6167 6520 616e 6420 7061 6765 5f73  "page and page_s
-00010900: 697a 6520 7061 7261 6d65 7465 7320 6d75  ize parametes mu
-00010910: 7374 2062 6520 7573 6564 2074 6f67 6574  st be used toget
-00010920: 6865 7222 290a 0a20 2020 2020 2020 2066  her")..        f
-00010930: 6f72 206b 6579 2c20 7661 6c20 696e 2070  or key, val in p
-00010940: 6172 616d 732e 6974 656d 7328 293a 0a20  arams.items():. 
-00010950: 2020 2020 2020 2020 2020 2069 6620 7661             if va
-00010960: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-00010970: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00010980: 616e 6365 2876 616c 2c20 7374 7229 3a0a  ance(val, str):.
-00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109a0: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-000109b0: 6e70 7574 4572 726f 7228 227b 6b65 797d  nputError("{key}
-000109c0: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
-000109d0: 6265 2061 2073 7472 696e 6722 2e66 6f72  be a string".for
-000109e0: 6d61 7428 6b65 793d 6b65 7929 290a 2020  mat(key=key)).  
-000109f0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00010a00: 7261 6d73 5f73 7472 696e 675f 6172 7261  rams_string_arra
-00010a10: 792e 6170 7065 6e64 2822 7b6b 6579 7d3d  y.append("{key}=
-00010a20: 7b76 616c 7d22 2e66 6f72 6d61 7428 6b65  {val}".format(ke
-00010a30: 793d 6b65 792c 2076 616c 3d76 616c 2929  y=key, val=val))
-00010a40: 0a0a 2020 2020 2020 2020 7175 6572 795f  ..        query_
-00010a50: 7374 7269 6e67 203d 2022 2622 2e6a 6f69  string = "&".joi
-00010a60: 6e28 7061 7261 6d73 5f73 7472 696e 675f  n(params_string_
-00010a70: 6172 7261 7929 0a20 2020 2020 2020 2065  array).        e
-00010a80: 6e64 706f 696e 7420 3d20 227b 656e 6470  ndpoint = "{endp
-00010a90: 6f69 6e74 7d3f 7b71 7565 7279 5f73 7472  oint}?{query_str
-00010aa0: 696e 677d 222e 666f 726d 6174 2865 6e64  ing}".format(end
-00010ab0: 706f 696e 743d 7365 6c66 2e5f 5f52 4554  point=self.__RET
-00010ac0: 5249 4556 455f 4d41 5443 4845 535f 464f  RIEVE_MATCHES_FO
-00010ad0: 525f 415f 5941 5241 5f52 554c 4553 4554  R_A_YARA_RULESET
-00010ae0: 5f45 4e44 504f 494e 545f 5632 2c0a 2020  _ENDPOINT_V2,.  
-00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b20: 2020 2020 7175 6572 795f 7374 7269 6e67      query_string
-00010b30: 3d71 7565 7279 5f73 7472 696e 6729 0a0a  =query_string)..
-00010b40: 2020 2020 2020 2020 7572 6c20 3d20 7365          url = se
-00010b50: 6c66 2e5f 7572 6c2e 666f 726d 6174 2865  lf._url.format(e
-00010b60: 6e64 706f 696e 743d 656e 6470 6f69 6e74  ndpoint=endpoint
-00010b70: 290a 0a20 2020 2020 2020 2072 6573 706f  )..        respo
-00010b80: 6e73 6520 3d20 7365 6c66 2e5f 5f67 6574  nse = self.__get
-00010b90: 5f72 6571 7565 7374 2875 726c 3d75 726c  _request(url=url
-00010ba0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00010bb0: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
-00010bc0: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
-00010bd0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00010be0: 6e73 650a 0a20 2020 2064 6566 2063 7265  nse..    def cre
-00010bf0: 6174 655f 6f72 5f75 7064 6174 655f 7961  ate_or_update_ya
-00010c00: 7261 5f72 756c 6573 6574 2873 656c 662c  ra_ruleset(self,
-00010c10: 206e 616d 652c 2063 6f6e 7465 6e74 2c20   name, content, 
-00010c20: 7075 626c 6973 683d 4e6f 6e65 2c20 7469  publish=None, ti
-00010c30: 636c 6f75 643d 4e6f 6e65 293a 0a20 2020  cloud=None):.   
-00010c40: 2020 2020 2022 2222 4372 6561 7465 7320       """Creates 
-00010c50: 6120 6e65 7720 5941 5241 2072 756c 6573  a new YARA rules
-00010c60: 6574 2069 6620 6974 2064 6f65 736e e280  et if it doesn..
-00010c70: 9974 2065 7869 7374 2e20 4966 2061 2072  .t exist. If a r
-00010c80: 756c 6573 6574 2077 6974 6820 7468 6520  uleset with the 
-00010c90: 7370 6563 6966 6965 6420 6e61 6d65 2061  specified name a
-00010ca0: 6c72 6561 6479 2065 7869 7374 732c 2061  lready exists, a
-00010cb0: 206e 6577 0a20 2020 2020 2020 2072 6576   new.        rev
-00010cc0: 6973 696f 6e20 2875 7064 6174 6529 206f  ision (update) o
-00010cd0: 6620 7468 6520 7275 6c65 7365 7420 6973  f the ruleset is
-00010ce0: 2063 7265 6174 6564 2e0a 2020 2020 2020   created..      
-00010cf0: 2020 2020 2020 3a70 6172 616d 206e 616d        :param nam
-00010d00: 653a 206e 616d 6520 6f66 2074 6865 2072  e: name of the r
-00010d10: 756c 6573 6574 2074 6f20 6372 6561 7465  uleset to create
-00010d20: 206f 7220 7570 6461 7465 0a20 2020 2020   or update.     
-00010d30: 2020 2020 2020 203a 7479 7065 206e 616d         :type nam
-00010d40: 653a 2073 7472 0a20 2020 2020 2020 2020  e: str.         
-00010d50: 2020 203a 7061 7261 6d20 636f 6e74 656e     :param conten
-00010d60: 743a 2063 6f6e 7465 6e74 206f 6620 7468  t: content of th
-00010d70: 6520 5941 5241 2072 756c 6573 6574 2074  e YARA ruleset t
-00010d80: 6f20 6372 6561 7465 206f 7220 7570 6461  o create or upda
-00010d90: 7465 0a20 2020 2020 2020 2020 2020 203a  te.            :
-00010da0: 7479 7065 2063 6f6e 7465 6e74 3a20 7374  type content: st
-00010db0: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
-00010dc0: 6172 616d 2070 7562 6c69 7368 3a20 6465  aram publish: de
-00010dd0: 7465 726d 696e 6573 2077 6865 7468 6572  termines whether
-00010de0: 2074 6865 2072 756c 6573 6574 2073 686f   the ruleset sho
-00010df0: 756c 6420 6265 2073 796e 6368 726f 6e69  uld be synchroni
-00010e00: 7a65 6420 746f 206f 7468 6572 2061 7070  zed to other app
-00010e10: 6c69 616e 6365 7320 696e 2074 6865 2073  liances in the s
-00010e20: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-00010e30: 4331 3030 3020 636c 7573 7465 720a 2020  C1000 cluster.  
-00010e40: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
-00010e50: 7075 626c 6973 683a 2062 6f6f 6c0a 2020  publish: bool.  
-00010e60: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00010e70: 2074 6963 6c6f 7564 3a20 6465 7465 726d   ticloud: determ
-00010e80: 696e 6573 2077 6865 7468 6572 2074 6865  ines whether the
-00010e90: 2072 756c 6573 6574 2073 686f 756c 6420   ruleset should 
-00010ea0: 6265 2073 796e 6368 726f 6e69 7a65 6420  be synchronized 
-00010eb0: 7769 7468 2054 6974 616e 6975 6d43 6c6f  with TitaniumClo
-00010ec0: 7564 206f 7220 6e6f 740a 2020 2020 2020  ud or not.      
-00010ed0: 2020 2020 2020 3a74 7970 6520 7469 636c        :type ticl
-00010ee0: 6f75 643a 2062 6f6f 6c0a 2020 2020 2020  oud: bool.      
-00010ef0: 2020 2020 2020 3a72 6574 7572 6e3a 2072        :return: r
-00010f00: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-00010f10: 2020 2020 3a72 7479 7065 3a20 7265 7175      :rtype: requ
-00010f20: 6573 7473 2e52 6573 706f 6e73 653a 0a20  ests.Response:. 
-00010f30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010f40: 2020 2064 6174 6120 3d20 7365 6c66 2e5f     data = self._
-00010f50: 5f63 7265 6174 655f 706f 7374 5f70 6179  _create_post_pay
-00010f60: 6c6f 6164 280a 2020 2020 2020 2020 2020  load(.          
-00010f70: 2020 6e61 6d65 3d6e 616d 652c 0a20 2020    name=name,.   
-00010f80: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
-00010f90: 3d63 6f6e 7465 6e74 2c0a 2020 2020 2020  =content,.      
-00010fa0: 2020 2020 2020 7075 626c 6973 683d 7075        publish=pu
-00010fb0: 626c 6973 682c 0a20 2020 2020 2020 2020  blish,.         
-00010fc0: 2020 2074 6963 6c6f 7564 3d74 6963 6c6f     ticloud=ticlo
-00010fd0: 7564 0a20 2020 2020 2020 2029 0a0a 2020  ud.        )..  
-00010fe0: 2020 2020 2020 656e 6470 6f69 6e74 203d        endpoint =
-00010ff0: 2073 656c 662e 5f5f 5941 5241 5f52 554c   self.__YARA_RUL
-00011000: 4553 4554 5f45 4e44 504f 494e 540a 0a20  ESET_ENDPOINT.. 
-00011010: 2020 2020 2020 2075 726c 203d 2073 656c         url = sel
-00011020: 662e 5f75 726c 2e66 6f72 6d61 7428 656e  f._url.format(en
-00011030: 6470 6f69 6e74 3d65 6e64 706f 696e 7429  dpoint=endpoint)
-00011040: 0a0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-00011050: 7365 203d 2073 656c 662e 5f5f 706f 7374  se = self.__post
-00011060: 5f72 6571 7565 7374 2875 726c 3d75 726c  _request(url=url
-00011070: 2c20 6461 7461 3d64 6174 6129 0a0a 2020  , data=data)..  
-00011080: 2020 2020 2020 7365 6c66 2e5f 5f72 6169        self.__rai
-00011090: 7365 5f6f 6e5f 6572 726f 7228 7265 7370  se_on_error(resp
-000110a0: 6f6e 7365 290a 0a20 2020 2020 2020 2072  onse)..        r
-000110b0: 6574 7572 6e20 7265 7370 6f6e 7365 0a0a  eturn response..
-000110c0: 2020 2020 6465 6620 6465 6c65 7465 5f79      def delete_y
-000110d0: 6172 615f 7275 6c65 7365 7428 7365 6c66  ara_ruleset(self
-000110e0: 2c20 6e61 6d65 2c20 7075 626c 6973 683d  , name, publish=
-000110f0: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-00011100: 2222 4465 6c65 7465 7320 7468 6520 7370  ""Deletes the sp
-00011110: 6563 6966 6965 6420 5941 5241 2072 756c  ecified YARA rul
-00011120: 6573 6574 2061 6e64 2069 7473 206d 6174  eset and its mat
-00011130: 6368 6573 2066 726f 6d20 7468 6520 6170  ches from the ap
-00011140: 706c 6961 6e63 652e 0a20 2020 2020 2020  pliance..       
-00011150: 2020 2020 203a 7061 7261 6d20 6e61 6d65       :param name
-00011160: 3a20 6e61 6d65 206f 6620 7468 6520 7275  : name of the ru
-00011170: 6c65 7365 7420 746f 2063 7265 6174 6520  leset to create 
-00011180: 6f72 2075 7064 6174 650a 2020 2020 2020  or update.      
-00011190: 2020 2020 2020 3a74 7970 6520 6e61 6d65        :type name
-000111a0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-000111b0: 2020 3a70 6172 616d 2070 7562 6c69 7368    :param publish
-000111c0: 3a20 6465 7465 726d 696e 6573 2077 6865  : determines whe
-000111d0: 7468 6572 2074 6865 2072 756c 6573 6574  ther the ruleset
-000111e0: 2073 686f 756c 6420 6265 2073 796e 6368   should be synch
-000111f0: 726f 6e69 7a65 6420 746f 206f 7468 6572  ronized to other
-00011200: 2061 7070 6c69 616e 6365 7320 696e 2074   appliances in t
-00011210: 6865 2073 616d 650a 2020 2020 2020 2020  he same.        
-00011220: 2020 2020 4331 3030 3020 636c 7573 7465      C1000 cluste
-00011230: 720a 2020 2020 2020 2020 2020 2020 3a74  r.            :t
-00011240: 7970 6520 7075 626c 6973 683a 2062 6f6f  ype publish: boo
-00011250: 6c0a 2020 2020 2020 2020 2020 2020 3a72  l.            :r
-00011260: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
-00011270: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
-00011280: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
-00011290: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
-000112a0: 2222 0a20 2020 2020 2020 2070 6f73 745f  "".        post_
-000112b0: 6a73 6f6e 203d 2073 656c 662e 5f5f 6372  json = self.__cr
-000112c0: 6561 7465 5f70 6f73 745f 7061 796c 6f61  eate_post_payloa
-000112d0: 6428 0a20 2020 2020 2020 2020 2020 206e  d(.            n
-000112e0: 616d 653d 6e61 6d65 2c0a 2020 2020 2020  ame=name,.      
-000112f0: 2020 2020 2020 7075 626c 6973 683d 7075        publish=pu
-00011300: 626c 6973 682c 0a0a 2020 2020 2020 2020  blish,..        
-00011310: 290a 2020 2020 2020 2020 656e 6470 6f69  ).        endpoi
-00011320: 6e74 203d 2073 656c 662e 5f5f 5941 5241  nt = self.__YARA
-00011330: 5f52 554c 4553 4554 5f45 4e44 504f 494e  _RULESET_ENDPOIN
-00011340: 540a 0a20 2020 2020 2020 2075 726c 203d  T..        url =
-00011350: 2073 656c 662e 5f75 726c 2e66 6f72 6d61   self._url.forma
-00011360: 7428 656e 6470 6f69 6e74 3d65 6e64 706f  t(endpoint=endpo
-00011370: 696e 7429 0a0a 2020 2020 2020 2020 7265  int)..        re
-00011380: 7370 6f6e 7365 203d 2073 656c 662e 5f5f  sponse = self.__
-00011390: 6465 6c65 7465 5f72 6571 7565 7374 2875  delete_request(u
-000113a0: 726c 3d75 726c 2c20 706f 7374 5f6a 736f  rl=url, post_jso
-000113b0: 6e3d 706f 7374 5f6a 736f 6e29 0a0a 2020  n=post_json)..  
-000113c0: 2020 2020 2020 7365 6c66 2e5f 5f72 6169        self.__rai
-000113d0: 7365 5f6f 6e5f 6572 726f 7228 7265 7370  se_on_error(resp
-000113e0: 6f6e 7365 290a 0a20 2020 2020 2020 2072  onse)..        r
-000113f0: 6574 7572 6e20 7265 7370 6f6e 7365 0a0a  eturn response..
-00011400: 2020 2020 6465 6620 656e 6162 6c65 5f6f      def enable_o
-00011410: 725f 6469 7361 626c 655f 7961 7261 5f72  r_disable_yara_r
-00011420: 756c 6573 6574 2873 656c 662c 2065 6e61  uleset(self, ena
-00011430: 626c 6564 2c20 6e61 6d65 2c20 7075 626c  bled, name, publ
-00011440: 6973 683d 4e6f 6e65 293a 0a20 2020 2020  ish=None):.     
-00011450: 2020 2022 2222 456e 6162 6c65 732f 6469     """Enables/di
-00011460: 7361 626c 6573 2072 756c 6573 6574 206f  sables ruleset o
-00011470: 6e20 7468 6520 6170 706c 6961 6e63 652e  n the appliance.
-00011480: 2041 646d 696e 6973 7472 6174 6f72 7320   Administrators 
-00011490: 6361 6e20 6d61 6e61 6765 2061 6e79 2072  can manage any r
-000114a0: 756c 6573 6574 2077 6869 6c65 2072 6567  uleset while reg
-000114b0: 756c 6172 2041 3130 3030 2075 7365 7273  ular A1000 users
-000114c0: 0a20 2020 2020 2020 2063 616e 206f 6e6c  .        can onl
-000114d0: 7920 6d65 6e61 6765 2074 6865 6972 206f  y menage their o
-000114e0: 776e 2072 756c 6573 6574 732e 0a20 2020  wn rulesets..   
-000114f0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00011500: 656e 6162 6c65 643a 2077 6865 7468 6572  enabled: whether
-00011510: 2074 6f20 656e 6162 6c65 2028 656e 6162   to enable (enab
-00011520: 6c65 643d 5472 7565 2920 6f72 2064 6973  led=True) or dis
-00011530: 6162 6c65 2028 656e 6162 6c65 643d 4661  able (enabled=Fa
-00011540: 6c73 6529 2074 6865 2073 7065 6369 6669  lse) the specifi
-00011550: 6564 2072 756c 6573 6574 0a20 2020 2020  ed ruleset.     
-00011560: 2020 2020 2020 203a 7479 7065 2065 6e61         :type ena
-00011570: 626c 6564 3a20 626f 6f6c 0a20 2020 2020  bled: bool.     
-00011580: 2020 2020 2020 203a 7061 7261 6d20 6e61         :param na
-00011590: 6d65 3a20 6e61 6d65 206f 6620 7468 6520  me: name of the 
-000115a0: 7275 6c65 7365 7420 746f 2065 6e61 626c  ruleset to enabl
-000115b0: 652f 6469 7361 626c 650a 2020 2020 2020  e/disable.      
-000115c0: 2020 2020 2020 3a74 7970 6520 6e61 6d65        :type name
-000115d0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-000115e0: 2020 3a70 6172 616d 2070 7562 6c69 7368    :param publish
-000115f0: 3a20 6465 7465 726d 696e 6573 2077 6865  : determines whe
-00011600: 7468 6572 2074 6865 2072 756c 6573 6574  ther the ruleset
-00011610: 2073 686f 756c 6420 6265 2073 796e 6368   should be synch
-00011620: 726f 6e69 7a65 6420 746f 206f 7468 6572  ronized to other
-00011630: 2061 7070 6c69 616e 6365 7320 696e 2074   appliances in t
-00011640: 6865 2073 616d 650a 2020 2020 2020 2020  he same.        
-00011650: 2020 2020 4331 3030 3020 636c 7573 7465      C1000 cluste
-00011660: 720a 2020 2020 2020 2020 2020 2020 3a74  r.            :t
-00011670: 7970 6520 7075 626c 6973 683a 2062 6f6f  ype publish: boo
-00011680: 6c0a 2020 2020 2020 2020 2020 2020 3a72  l.            :r
-00011690: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
-000116a0: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
-000116b0: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
-000116c0: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
-000116d0: 2222 0a20 2020 2020 2020 2064 6174 6120  "".        data 
-000116e0: 3d20 7365 6c66 2e5f 5f63 7265 6174 655f  = self.__create_
-000116f0: 706f 7374 5f70 6179 6c6f 6164 280a 2020  post_payload(.  
-00011700: 2020 2020 2020 2020 2020 6e61 6d65 3d6e            name=n
-00011710: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00011720: 2070 7562 6c69 7368 3d70 7562 6c69 7368   publish=publish
-00011730: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00011740: 2020 2020 2069 6620 656e 6162 6c65 6420       if enabled 
-00011750: 616e 6420 656e 6162 6c65 6420 6e6f 7420  and enabled not 
-00011760: 696e 2028 5472 7565 2c20 4661 6c73 6529  in (True, False)
-00011770: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00011780: 6973 6520 5772 6f6e 6749 6e70 7574 4572  ise WrongInputEr
-00011790: 726f 7228 2265 6e61 626c 6564 2070 6172  ror("enabled par
-000117a0: 616d 6574 6572 206d 7573 7420 6265 2062  ameter must be b
-000117b0: 6f6f 6c65 616e 2e22 290a 0a20 2020 2020  oolean.")..     
-000117c0: 2020 2065 6e64 706f 696e 7420 3d20 7365     endpoint = se
-000117d0: 6c66 2e5f 5f45 4e41 424c 455f 4f52 5f44  lf.__ENABLE_OR_D
-000117e0: 4953 4142 4c45 5f59 4152 415f 5255 4c45  ISABLE_YARA_RULE
-000117f0: 5345 545f 454e 4450 4f49 4e54 2e66 6f72  SET_ENDPOINT.for
-00011800: 6d61 7428 6f70 6572 6174 696f 6e3d 2265  mat(operation="e
-00011810: 6e61 626c 6522 2069 6620 656e 6162 6c65  nable" if enable
-00011820: 6420 656c 7365 2022 6469 7361 626c 6522  d else "disable"
-00011830: 290a 0a20 2020 2020 2020 2075 726c 203d  )..        url =
-00011840: 2073 656c 662e 5f75 726c 2e66 6f72 6d61   self._url.forma
-00011850: 7428 656e 6470 6f69 6e74 3d65 6e64 706f  t(endpoint=endpo
-00011860: 696e 7429 0a0a 2020 2020 2020 2020 7265  int)..        re
-00011870: 7370 6f6e 7365 203d 2073 656c 662e 5f5f  sponse = self.__
-00011880: 706f 7374 5f72 6571 7565 7374 2875 726c  post_request(url
-00011890: 3d75 726c 2c20 6461 7461 3d64 6174 6129  =url, data=data)
-000118a0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-000118b0: 5f72 6169 7365 5f6f 6e5f 6572 726f 7228  _raise_on_error(
-000118c0: 7265 7370 6f6e 7365 290a 0a20 2020 2020  response)..     
-000118d0: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-000118e0: 7365 0a0a 2020 2020 6465 6620 6765 745f  se..    def get_
-000118f0: 7961 7261 5f72 756c 6573 6574 5f73 796e  yara_ruleset_syn
-00011900: 6368 726f 6e69 7a61 7469 6f6e 5f74 696d  chronization_tim
-00011910: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00011920: 2022 2222 4765 7473 2069 6e66 6f72 6d61   """Gets informa
-00011930: 7469 6f6e 2061 626f 7574 2074 6865 2063  tion about the c
-00011940: 7572 7265 6e74 2073 796e 6368 726f 6e69  urrent synchroni
-00011950: 7a61 7469 6f6e 2073 7461 7475 7320 666f  zation status fo
-00011960: 7220 5469 7461 6e69 756d 436c 6f75 642d  r TitaniumCloud-
-00011970: 656e 6162 6c65 6420 7275 6c65 7365 7473  enabled rulesets
-00011980: 2e0a 2020 2020 2020 2020 2020 2020 3a72  ..            :r
-00011990: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
-000119a0: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
-000119b0: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
-000119c0: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
-000119d0: 2222 0a20 2020 2020 2020 2065 6e64 706f  "".        endpo
-000119e0: 696e 7420 3d20 7365 6c66 2e5f 5f47 4554  int = self.__GET
-000119f0: 5f4f 525f 5345 545f 5941 5241 5f52 554c  _OR_SET_YARA_RUL
-00011a00: 4553 4554 5f53 594e 4348 524f 4e49 5a41  ESET_SYNCHRONIZA
-00011a10: 5449 4f4e 5f54 494d 455f 454e 4450 4f49  TION_TIME_ENDPOI
-00011a20: 4e54 0a0a 2020 2020 2020 2020 7572 6c20  NT..        url 
-00011a30: 3d20 7365 6c66 2e5f 7572 6c2e 666f 726d  = self._url.form
-00011a40: 6174 2865 6e64 706f 696e 743d 656e 6470  at(endpoint=endp
-00011a50: 6f69 6e74 290a 0a20 2020 2020 2020 2072  oint)..        r
-00011a60: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-00011a70: 5f67 6574 5f72 6571 7565 7374 2875 726c  _get_request(url
-00011a80: 3d75 726c 290a 0a20 2020 2020 2020 2073  =url)..        s
-00011a90: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
-00011aa0: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
-00011ab0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00011ac0: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
-00011ad0: 2075 7064 6174 655f 7961 7261 5f72 756c   update_yara_rul
-00011ae0: 6573 6574 5f73 796e 6368 726f 6e69 7a61  eset_synchroniza
-00011af0: 7469 6f6e 5f74 696d 6528 7365 6c66 2c20  tion_time(self, 
-00011b00: 7379 6e63 5f74 696d 6529 3a0a 2020 2020  sync_time):.    
-00011b10: 2020 2020 2222 2255 7064 6174 6573 2074      """Updates t
-00011b20: 6865 2054 6974 616e 6975 6d43 6c6f 7564  he TitaniumCloud
-00011b30: 2073 796e 6368 726f 6e69 7a61 7469 6f6e   synchronization
-00011b40: 2074 696d 6520 666f 7220 5469 7461 6e69   time for Titani
-00011b50: 756d 436c 6f75 642d 656e 6162 6c65 6420  umCloud-enabled 
-00011b60: 5941 5241 2072 756c 6573 6574 732e 0a20  YARA rulesets.. 
-00011b70: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00011b80: 6d20 7379 6e63 5f74 696d 653a 2066 6f72  m sync_time: for
-00011b90: 6d61 7420 7368 6f75 6c64 2062 6520 5554  mat should be UT
-00011ba0: 4320 2859 5959 592d 4d4d 2d44 4420 6868  C (YYYY-MM-DD hh
-00011bb0: 3a6d 6d29 0a20 2020 2020 2020 2020 2020  :mm).           
-00011bc0: 203a 7479 7065 2073 796e 635f 7469 6d65   :type sync_time
-00011bd0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-00011be0: 2020 3a72 6574 7572 6e3a 2072 6573 706f    :return: respo
-00011bf0: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
-00011c00: 3a72 7479 7065 3a20 7265 7175 6573 7473  :rtype: requests
-00011c10: 2e52 6573 706f 6e73 653a 0a20 2020 2020  .Response:.     
-00011c20: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-00011c30: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00011c40: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-00011c50: 652e 7374 7270 7469 6d65 2873 796e 635f  e.strptime(sync_
-00011c60: 7469 6d65 2c20 2725 592d 256d 2d25 6420  time, '%Y-%m-%d 
-00011c70: 2548 3a25 4d27 290a 2020 2020 2020 2020  %H:%M').        
-00011c80: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-00011c90: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-00011ca0: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
-00011cb0: 7272 6f72 2822 496e 636f 7272 6563 7420  rror("Incorrect 
-00011cc0: 7379 6e63 5f74 696d 6520 666f 726d 6174  sync_time format
-00011cd0: 2c20 7368 6f75 6c64 2062 6520 5959 5959  , should be YYYY
-00011ce0: 2d4d 4d2d 4444 2068 683a 6d6d 2229 0a0a  -MM-DD hh:mm")..
-00011cf0: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
-00011d00: 203d 2073 656c 662e 5f5f 4745 545f 4f52   = self.__GET_OR
-00011d10: 5f53 4554 5f59 4152 415f 5255 4c45 5345  _SET_YARA_RULESE
-00011d20: 545f 5359 4e43 4852 4f4e 495a 4154 494f  T_SYNCHRONIZATIO
-00011d30: 4e5f 5449 4d45 5f45 4e44 504f 494e 540a  N_TIME_ENDPOINT.
-00011d40: 0a20 2020 2020 2020 2075 726c 203d 2073  .        url = s
-00011d50: 656c 662e 5f75 726c 2e66 6f72 6d61 7428  elf._url.format(
-00011d60: 656e 6470 6f69 6e74 3d65 6e64 706f 696e  endpoint=endpoin
-00011d70: 7429 0a0a 2020 2020 2020 2020 7265 7370  t)..        resp
-00011d80: 6f6e 7365 203d 2073 656c 662e 5f5f 706f  onse = self.__po
-00011d90: 7374 5f72 6571 7565 7374 2875 726c 3d75  st_request(url=u
-00011da0: 726c 2c20 6461 7461 3d7b 2274 696d 6522  rl, data={"time"
-00011db0: 3a20 7379 6e63 5f74 696d 657d 290a 0a20  : sync_time}).. 
-00011dc0: 2020 2020 2020 2073 656c 662e 5f5f 7261         self.__ra
-00011dd0: 6973 655f 6f6e 5f65 7272 6f72 2872 6573  ise_on_error(res
-00011de0: 706f 6e73 6529 0a0a 2020 2020 2020 2020  ponse)..        
-00011df0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-00011e00: 0a20 2020 2064 6566 2073 7461 7274 5f6f  .    def start_o
-00011e10: 725f 7374 6f70 5f79 6172 615f 6c6f 6361  r_stop_yara_loca
-00011e20: 6c5f 7265 7472 6f5f 7363 616e 2873 656c  l_retro_scan(sel
-00011e30: 662c 206f 7065 7261 7469 6f6e 293a 0a20  f, operation):. 
-00011e40: 2020 2020 2020 2022 2222 416c 6c6f 7773         """Allows
-00011e50: 2075 7365 7273 2074 6f20 696e 6974 6961   users to initia
-00011e60: 7465 2074 6865 204c 6f63 616c 2052 6574  te the Local Ret
-00011e70: 726f 2073 6361 6e20 6f6e 2074 6865 2041  ro scan on the A
-00011e80: 3130 3030 2061 7070 6c69 616e 6365 2c20  1000 appliance, 
-00011e90: 616e 6420 7374 6f70 2074 6865 204c 6f63  and stop the Loc
-00011ea0: 616c 2052 6574 726f 2073 6361 6e20 7468  al Retro scan th
-00011eb0: 6174 2069 730a 2020 2020 2020 2020 696e  at is.        in
-00011ec0: 2070 726f 6772 6573 7320 6f6e 2074 6865   progress on the
-00011ed0: 2061 7070 6c69 616e 6365 2e0a 2020 2020   appliance..    
-00011ee0: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
-00011ef0: 7065 7261 7469 6f6e 3a20 6163 6365 7074  peration: accept
-00011f00: 6564 2076 616c 7565 733a 2053 5441 5254  ed values: START
-00011f10: 2c20 5354 4f50 2028 6361 7365 2d73 656e  , STOP (case-sen
-00011f20: 7369 7469 7665 290a 2020 2020 2020 2020  sitive).        
-00011f30: 2020 2020 3a74 7970 6520 6f70 6572 6174      :type operat
-00011f40: 696f 6e3a 2073 7472 0a20 2020 2020 2020  ion: str.       
-00011f50: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
-00011f60: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
-00011f70: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
-00011f80: 7374 732e 5265 7370 6f6e 7365 3a0a 2020  sts.Response:.  
-00011f90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011fa0: 2020 6966 206f 7065 7261 7469 6f6e 206e    if operation n
-00011fb0: 6f74 2069 6e20 2822 5354 4152 5422 2c20  ot in ("START", 
-00011fc0: 2253 544f 5022 293a 0a20 2020 2020 2020  "STOP"):.       
-00011fd0: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
-00011fe0: 496e 7075 7445 7272 6f72 2822 6f70 6572  InputError("oper
-00011ff0: 6174 696f 6e20 7061 7261 6d65 7465 7220  ation parameter 
-00012000: 6d75 7374 2062 6520 6569 7468 6572 2027  must be either '
-00012010: 5354 4152 5427 206f 7220 2753 544f 5027  START' or 'STOP'
-00012020: 2229 0a0a 2020 2020 2020 2020 656e 6470  ")..        endp
-00012030: 6f69 6e74 203d 2073 656c 662e 5f5f 5941  oint = self.__YA
-00012040: 5241 5f4c 4f43 414c 5f52 4554 524f 5343  RA_LOCAL_RETROSC
-00012050: 414e 5f45 4e44 504f 494e 540a 0a20 2020  AN_ENDPOINT..   
-00012060: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
-00012070: 5f75 726c 2e66 6f72 6d61 7428 656e 6470  _url.format(endp
-00012080: 6f69 6e74 3d65 6e64 706f 696e 7429 0a0a  oint=endpoint)..
-00012090: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-000120a0: 203d 2073 656c 662e 5f5f 706f 7374 5f72   = self.__post_r
-000120b0: 6571 7565 7374 2875 726c 3d75 726c 2c20  equest(url=url, 
-000120c0: 6461 7461 3d7b 226f 7065 7261 7469 6f6e  data={"operation
-000120d0: 223a 206f 7065 7261 7469 6f6e 7d29 0a0a  ": operation})..
-000120e0: 2020 2020 2020 2020 7365 6c66 2e5f 5f72          self.__r
-000120f0: 6169 7365 5f6f 6e5f 6572 726f 7228 7265  aise_on_error(re
-00012100: 7370 6f6e 7365 290a 0a20 2020 2020 2020  sponse)..       
-00012110: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00012120: 0a0a 2020 2020 6465 6620 6765 745f 7961  ..    def get_ya
-00012130: 7261 5f6c 6f63 616c 5f72 6574 726f 5f73  ra_local_retro_s
-00012140: 6361 6e5f 7374 6174 7573 2873 656c 6629  can_status(self)
-00012150: 3a0a 2020 2020 2020 2020 2222 2241 6c6c  :.        """All
-00012160: 6f77 7320 7573 6572 7320 746f 2063 6865  ows users to che
-00012170: 636b 2074 6865 2073 7461 7475 7320 6f66  ck the status of
-00012180: 204c 6f63 616c 2052 6574 726f 206f 6e20   Local Retro on 
-00012190: 7468 6520 4131 3030 3020 6170 706c 6961  the A1000 applia
-000121a0: 6e63 652e 2054 6865 2072 6573 706f 6e73  nce. The respons
-000121b0: 6520 696e 6469 6361 7465 7320 7468 6520  e indicates the 
-000121c0: 6375 7272 656e 740a 2020 2020 2020 2020  current.        
-000121d0: 7374 6174 6520 6f66 204c 6f63 616c 2052  state of Local R
-000121e0: 6574 726f 2c20 7469 6d65 2061 6e64 2064  etro, time and d
-000121f0: 6174 6520 7768 656e 2074 6865 206c 6174  ate when the lat
-00012200: 6573 7420 4c6f 6361 6c20 5265 7472 6f20  est Local Retro 
-00012210: 7363 616e 2077 6173 2073 7461 7274 6564  scan was started
-00012220: 2061 6e64 2f6f 7220 7374 6f70 7065 642c   and/or stopped,
-00012230: 2061 6e64 2061 206c 6973 7420 6f66 0a20   and a list of. 
-00012240: 2020 2020 2020 2070 7265 7669 6f75 7320         previous 
-00012250: 4c6f 6361 6c20 5265 7472 6f20 7363 616e  Local Retro scan
-00012260: 7320 7769 7468 2074 6865 2073 616d 6520  s with the same 
-00012270: 6465 7461 696c 732e 0a20 2020 2020 2020  details..       
-00012280: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
-00012290: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
-000122a0: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
-000122b0: 7374 732e 5265 7370 6f6e 7365 3a0a 2020  sts.Response:.  
-000122c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000122d0: 2020 656e 6470 6f69 6e74 203d 2073 656c    endpoint = sel
-000122e0: 662e 5f5f 5941 5241 5f4c 4f43 414c 5f52  f.__YARA_LOCAL_R
-000122f0: 4554 524f 5343 414e 5f45 4e44 504f 494e  ETROSCAN_ENDPOIN
-00012300: 540a 0a20 2020 2020 2020 2075 726c 203d  T..        url =
-00012310: 2073 656c 662e 5f75 726c 2e66 6f72 6d61   self._url.forma
-00012320: 7428 656e 6470 6f69 6e74 3d65 6e64 706f  t(endpoint=endpo
-00012330: 696e 7429 0a0a 2020 2020 2020 2020 7265  int)..        re
-00012340: 7370 6f6e 7365 203d 2073 656c 662e 5f5f  sponse = self.__
-00012350: 6765 745f 7265 7175 6573 7428 7572 6c3d  get_request(url=
-00012360: 7572 6c29 0a0a 2020 2020 2020 2020 7365  url)..        se
-00012370: 6c66 2e5f 5f72 6169 7365 5f6f 6e5f 6572  lf.__raise_on_er
-00012380: 726f 7228 7265 7370 6f6e 7365 290a 0a20  ror(response).. 
-00012390: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000123a0: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
-000123b0: 7374 6172 745f 6f72 5f73 746f 705f 7961  start_or_stop_ya
-000123c0: 7261 5f63 6c6f 7564 5f72 6574 726f 5f73  ra_cloud_retro_s
-000123d0: 6361 6e28 7365 6c66 2c20 6f70 6572 6174  can(self, operat
-000123e0: 696f 6e2c 2072 756c 6573 6574 5f6e 616d  ion, ruleset_nam
-000123f0: 6529 3a0a 2020 2020 2020 2020 2222 2241  e):.        """A
-00012400: 6c6c 6f77 7320 7573 6572 7320 746f 2073  llows users to s
-00012410: 7461 7274 2061 6e64 2073 746f 7020 6120  tart and stop a 
-00012420: 436c 6f75 6420 5265 7472 6f20 7363 616e  Cloud Retro scan
-00012430: 2066 6f72 2061 2073 7065 6369 6669 6564   for a specified
-00012440: 2072 756c 6573 6574 206f 6e20 7468 6520   ruleset on the 
-00012450: 4131 3030 3020 6170 706c 6961 6e63 652c  A1000 appliance,
-00012460: 2061 7320 7765 6c6c 2061 730a 2020 2020   as well as.    
-00012470: 2020 2020 746f 2063 6c65 6172 2061 6c6c      to clear all
-00012480: 2043 6c6f 7564 2052 6574 726f 2072 6573   Cloud Retro res
-00012490: 756c 7473 2066 6f72 2074 6865 2072 756c  ults for the rul
-000124a0: 6573 6574 2e0a 2020 2020 2020 2020 2020  eset..          
-000124b0: 2020 3a70 6172 616d 206f 7065 7261 7469    :param operati
-000124c0: 6f6e 3a20 6163 6365 7074 6564 2076 616c  on: accepted val
-000124d0: 7565 733a 2053 5441 5254 2c20 5354 4f50  ues: START, STOP
-000124e0: 2c20 434c 4541 5220 2863 6173 652d 7365  , CLEAR (case-se
-000124f0: 6e73 6974 6976 6529 0a20 2020 2020 2020  nsitive).       
-00012500: 2020 2020 203a 7479 7065 206f 7065 7261       :type opera
-00012510: 7469 6f6e 3a20 7374 720a 2020 2020 2020  tion: str.      
-00012520: 2020 2020 2020 3a70 6172 616d 2072 756c        :param rul
-00012530: 6573 6574 5f6e 616d 653a 206e 616d 6520  eset_name: name 
-00012540: 6f66 2074 6865 2059 4152 4120 7275 6c65  of the YARA rule
-00012550: 7365 7420 7468 6174 2074 6865 2043 6c6f  set that the Clo
-00012560: 7564 2052 6574 726f 2073 6361 6e20 7368  ud Retro scan sh
-00012570: 6f75 6c64 2062 6520 7275 6e20 6f6e 0a20  ould be run on. 
-00012580: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00012590: 2072 756c 6573 6574 5f6e 616d 653a 2073   ruleset_name: s
-000125a0: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
-000125b0: 7265 7475 726e 3a20 7265 7370 6f6e 7365  return: response
-000125c0: 0a20 2020 2020 2020 2020 2020 203a 7274  .            :rt
-000125d0: 7970 653a 2072 6571 7565 7374 732e 5265  ype: requests.Re
-000125e0: 7370 6f6e 7365 0a20 2020 2020 2020 2022  sponse.        "
-000125f0: 2222 0a20 2020 2020 2020 2069 6620 6f70  "".        if op
-00012600: 6572 6174 696f 6e20 6e6f 7420 696e 2028  eration not in (
-00012610: 2253 5441 5254 222c 2022 5354 4f50 222c  "START", "STOP",
-00012620: 2022 434c 4541 5222 293a 0a20 2020 2020   "CLEAR"):.     
-00012630: 2020 2020 2020 2072 6169 7365 2057 726f         raise Wro
-00012640: 6e67 496e 7075 7445 7272 6f72 2822 6f70  ngInputError("op
-00012650: 6572 6174 696f 6e20 7061 7261 6d65 7465  eration paramete
-00012660: 7220 6d75 7374 2062 6520 6569 7468 6572  r must be either
-00012670: 2027 5354 4152 5427 2c20 2753 544f 5027   'START', 'STOP'
-00012680: 206f 7220 2743 4c45 4152 2722 290a 0a20   or 'CLEAR'").. 
-00012690: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-000126a0: 696e 7374 616e 6365 2872 756c 6573 6574  instance(ruleset
-000126b0: 5f6e 616d 652c 2073 7472 293a 0a20 2020  _name, str):.   
-000126c0: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
-000126d0: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
-000126e0: 7275 6c65 7365 745f 6e61 6d65 2070 6172  ruleset_name par
-000126f0: 616d 6574 6572 206d 7573 7420 6265 2061  ameter must be a
-00012700: 2073 7472 696e 6722 290a 0a20 2020 2020   string")..     
-00012710: 2020 2065 6e64 706f 696e 7420 3d20 7365     endpoint = se
-00012720: 6c66 2e5f 5f59 4152 415f 434c 4f55 445f  lf.__YARA_CLOUD_
-00012730: 5245 5452 4f53 4341 4e53 5f45 4e44 504f  RETROSCANS_ENDPO
-00012740: 494e 542e 666f 726d 6174 2872 756c 6573  INT.format(rules
-00012750: 6574 5f6e 616d 653d 7275 6c65 7365 745f  et_name=ruleset_
-00012760: 6e61 6d65 290a 0a20 2020 2020 2020 2075  name)..        u
-00012770: 726c 203d 2073 656c 662e 5f75 726c 2e66  rl = self._url.f
-00012780: 6f72 6d61 7428 656e 6470 6f69 6e74 3d65  ormat(endpoint=e
-00012790: 6e64 706f 696e 7429 0a0a 2020 2020 2020  ndpoint)..      
-000127a0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-000127b0: 662e 5f5f 706f 7374 5f72 6571 7565 7374  f.__post_request
-000127c0: 2875 726c 3d75 726c 2c20 6461 7461 3d7b  (url=url, data={
-000127d0: 226f 7065 7261 7469 6f6e 223a 206f 7065  "operation": ope
-000127e0: 7261 7469 6f6e 7d29 0a0a 2020 2020 2020  ration})..      
-000127f0: 2020 7365 6c66 2e5f 5f72 6169 7365 5f6f    self.__raise_o
-00012800: 6e5f 6572 726f 7228 7265 7370 6f6e 7365  n_error(response
-00012810: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00012820: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
-00012830: 6465 6620 6765 745f 7961 7261 5f63 6c6f  def get_yara_clo
-00012840: 7564 5f72 6574 726f 5f73 6361 6e5f 7374  ud_retro_scan_st
-00012850: 6174 7573 2873 656c 662c 2072 756c 6573  atus(self, rules
-00012860: 6574 5f6e 616d 6529 3a0a 2020 2020 2020  et_name):.      
-00012870: 2020 2222 2241 6c6c 6f77 7320 7573 6572    """Allows user
-00012880: 7320 746f 2063 6865 636b 2074 6865 2073  s to check the s
-00012890: 7461 7475 7320 6f66 2043 6c6f 7564 2052  tatus of Cloud R
-000128a0: 6574 726f 2066 6f72 2074 6865 2073 7065  etro for the spe
-000128b0: 6369 6669 6564 2059 4152 4120 7275 6c65  cified YARA rule
-000128c0: 7365 742e 2054 6865 2072 6573 706f 6e73  set. The respons
-000128d0: 6520 696e 6469 6361 7465 7320 7468 650a  e indicates the.
-000128e0: 2020 2020 2020 2020 6375 7272 656e 7420          current 
-000128f0: 7374 6174 6520 6f66 2043 6c6f 7564 2052  state of Cloud R
-00012900: 6574 726f 2c20 7469 6d65 2061 6e64 2064  etro, time and d
-00012910: 6174 6520 7768 656e 2074 6865 206c 6174  ate when the lat
-00012920: 6573 7420 436c 6f75 6420 5265 7472 6f20  est Cloud Retro 
-00012930: 7363 616e 2077 6173 2073 7461 7274 6564  scan was started
-00012940: 2061 6e64 2f6f 7220 7374 6f70 7065 642c   and/or stopped,
-00012950: 2061 6e64 2061 0a20 2020 2020 2020 206c   and a.        l
-00012960: 6973 7420 6f66 2070 7265 7669 6f75 7320  ist of previous 
-00012970: 436c 6f75 6420 5265 7472 6f20 7363 616e  Cloud Retro scan
-00012980: 7320 7769 7468 2074 6865 2073 616d 6520  s with the same 
-00012990: 6465 7461 696c 732e 0a20 2020 2020 2020  details..       
-000129a0: 2020 2020 203a 7061 7261 6d20 7275 6c65       :param rule
-000129b0: 7365 745f 6e61 6d65 3a20 6e61 6d65 206f  set_name: name o
-000129c0: 6620 7468 6520 5941 5241 2072 756c 6573  f the YARA rules
-000129d0: 6574 2066 6f72 2077 6869 6368 2074 6f20  et for which to 
-000129e0: 6368 6563 6b20 666f 7220 7468 6520 436c  check for the Cl
-000129f0: 6f75 6420 5265 7472 6f20 7363 616e 2073  oud Retro scan s
-00012a00: 7461 7475 730a 2020 2020 2020 2020 2020  tatus.          
-00012a10: 2020 3a74 7970 6520 7275 6c65 7365 745f    :type ruleset_
-00012a20: 6e61 6d65 3a20 7374 720a 2020 2020 2020  name: str.      
-00012a30: 2020 2020 2020 3a72 6574 7572 6e3a 2072        :return: r
-00012a40: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-00012a50: 2020 2020 3a72 7479 7065 3a20 7265 7175      :rtype: requ
-00012a60: 6573 7473 2e52 6573 706f 6e73 650a 2020  ests.Response.  
-00012a70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012a80: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00012a90: 6e63 6528 7275 6c65 7365 745f 6e61 6d65  nce(ruleset_name
-00012aa0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-00012ab0: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00012ac0: 6e70 7574 4572 726f 7228 2272 756c 6573  nputError("rules
-00012ad0: 6574 5f6e 616d 6520 7061 7261 6d65 7465  et_name paramete
-00012ae0: 7220 6d75 7374 2062 6520 6120 7374 7269  r must be a stri
-00012af0: 6e67 2229 0a0a 2020 2020 2020 2020 656e  ng")..        en
-00012b00: 6470 6f69 6e74 203d 2073 656c 662e 5f5f  dpoint = self.__
-00012b10: 5941 5241 5f43 4c4f 5544 5f52 4554 524f  YARA_CLOUD_RETRO
-00012b20: 5343 414e 535f 454e 4450 4f49 4e54 2e66  SCANS_ENDPOINT.f
-00012b30: 6f72 6d61 7428 7275 6c65 7365 745f 6e61  ormat(ruleset_na
-00012b40: 6d65 3d72 756c 6573 6574 5f6e 616d 6529  me=ruleset_name)
-00012b50: 0a0a 2020 2020 2020 2020 7572 6c20 3d20  ..        url = 
-00012b60: 7365 6c66 2e5f 7572 6c2e 666f 726d 6174  self._url.format
-00012b70: 2865 6e64 706f 696e 743d 656e 6470 6f69  (endpoint=endpoi
-00012b80: 6e74 290a 0a20 2020 2020 2020 2072 6573  nt)..        res
-00012b90: 706f 6e73 6520 3d20 7365 6c66 2e5f 5f67  ponse = self.__g
-00012ba0: 6574 5f72 6571 7565 7374 2875 726c 3d75  et_request(url=u
-00012bb0: 726c 290a 0a20 2020 2020 2020 2073 656c  rl)..        sel
-00012bc0: 662e 5f5f 7261 6973 655f 6f6e 5f65 7272  f.__raise_on_err
-00012bd0: 6f72 2872 6573 706f 6e73 6529 0a0a 2020  or(response)..  
-00012be0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00012bf0: 706f 6e73 650a 0a20 2020 2064 6566 2061  ponse..    def a
-00012c00: 6476 616e 6365 645f 7365 6172 6368 2873  dvanced_search(s
-00012c10: 656c 662c 2071 7565 7279 5f73 7472 696e  elf, query_strin
-00012c20: 672c 2070 6167 655f 6e75 6d62 6572 3d31  g, page_number=1
-00012c30: 2c20 7265 636f 7264 735f 7065 725f 7061  , records_per_pa
-00012c40: 6765 3d32 302c 2073 6f72 7469 6e67 5f63  ge=20, sorting_c
-00012c50: 7269 7465 7269 613d 4e6f 6e65 2c0a 2020  riteria=None,.  
-00012c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c70: 2020 2020 2020 736f 7274 696e 675f 6f72        sorting_or
-00012c80: 6465 723d 2264 6573 6322 293a 0a20 2020  der="desc"):.   
-00012c90: 2020 2020 2022 2222 5448 4953 204d 4554       """THIS MET
-00012ca0: 484f 4420 4953 2044 4550 5245 4341 5445  HOD IS DEPRECATE
-00012cb0: 442e 2055 7365 2061 6476 616e 6365 645f  D. Use advanced_
-00012cc0: 7365 6172 6368 5f76 3220 696e 7374 6561  search_v2 instea
-00012cd0: 642e 0a0a 2020 2020 2020 2020 5365 6e64  d...        Send
-00012ce0: 7320 6120 7175 6572 7920 7374 7269 6e67  s a query string
-00012cf0: 2074 6f20 7468 6520 4131 3030 3020 4164   to the A1000 Ad
-00012d00: 7661 6e63 6564 2053 6561 7263 6820 4150  vanced Search AP
-00012d10: 492e 0a20 2020 2020 2020 2054 6865 2071  I..        The q
-00012d20: 7565 7279 2073 7472 696e 6720 6d75 7374  uery string must
-00012d30: 2062 6520 636f 6d70 6f73 6564 206f 6620   be composed of 
-00012d40: 6b65 792d 7661 6c75 6520 7061 6972 7320  key-value pairs 
-00012d50: 7365 7061 7261 7465 6420 6279 2073 7061  separated by spa
-00012d60: 6365 2e0a 2020 2020 2020 2020 4120 6b65  ce..        A ke
-00012d70: 7920 6973 2073 6570 6172 6174 6564 2066  y is separated f
-00012d80: 726f 6d20 6974 7320 7661 6c75 6520 6279  rom its value by
-00012d90: 2061 2063 6f6c 6f6e 2073 796d 626f 6c20   a colon symbol 
-00012da0: 616e 6420 6e6f 2073 7061 6365 732e 0a20  and no spaces.. 
-00012db0: 2020 2020 2020 2049 6620 6120 7061 6765         If a page
-00012dc0: 206e 756d 6265 7220 6973 206e 6f74 2070   number is not p
-00012dd0: 726f 7669 6465 642c 2074 6865 2066 6972  rovided, the fir
-00012de0: 7374 2070 6167 6520 6f66 2072 6573 756c  st page of resul
-00012df0: 7473 2077 696c 6c20 6265 2072 6574 7572  ts will be retur
-00012e00: 6e65 642e 0a20 2020 2020 2020 2020 2020  ned..           
-00012e10: 2051 7565 7279 2073 7472 696e 6720 6578   Query string ex
-00012e20: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
-00012e30: 2020 2027 6176 2d63 6f75 6e74 3a35 2061     'av-count:5 a
-00012e40: 7661 696c 6162 6c65 3a54 5255 4527 0a0a  vailable:TRUE'..
-00012e50: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00012e60: 616d 2071 7565 7279 5f73 7472 696e 673a  am query_string:
-00012e70: 2071 7565 7279 2073 7472 696e 670a 2020   query string.  
-00012e80: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
-00012e90: 7175 6572 795f 7374 7269 6e67 3a20 7374  query_string: st
-00012ea0: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
-00012eb0: 6172 616d 2070 6167 655f 6e75 6d62 6572  aram page_number
-00012ec0: 3a20 7061 6765 206e 756d 6265 720a 2020  : page number.  
-00012ed0: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
-00012ee0: 7061 6765 5f6e 756d 6265 723a 2069 6e74  page_number: int
-00012ef0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-00012f00: 7261 6d20 7265 636f 7264 735f 7065 725f  ram records_per_
-00012f10: 7061 6765 3a20 6e75 6d62 6572 206f 6620  page: number of 
-00012f20: 7265 636f 7264 7320 7265 7475 726e 6564  records returned
-00012f30: 2070 6572 2070 6167 653b 206d 6178 696d   per page; maxim
-00012f40: 756d 2076 616c 7565 2069 7320 3130 300a  um value is 100.
-00012f50: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
-00012f60: 6520 7265 636f 7264 735f 7065 725f 7061  e records_per_pa
-00012f70: 6765 3a20 696e 740a 2020 2020 2020 2020  ge: int.        
-00012f80: 2020 2020 3a70 6172 616d 2073 6f72 7469      :param sorti
-00012f90: 6e67 5f63 7269 7465 7269 613a 2064 6566  ng_criteria: def
-00012fa0: 696e 6520 7468 6520 6372 6974 6572 6961  ine the criteria
-00012fb0: 2075 7365 6420 696e 2073 6f72 7469 6e67   used in sorting
-00012fc0: 3b20 706f 7373 6962 6c65 2076 616c 7565  ; possible value
-00012fd0: 7320 6172 6520 2773 6861 3127 2c20 2766  s are 'sha1', 'f
-00012fe0: 6972 7374 7365 656e 272c 0a20 2020 2020  irstseen',.     
-00012ff0: 2020 2020 2020 2027 7468 7265 6174 6e61         'threatna
-00013000: 6d65 272c 2027 7361 6d70 6c65 7479 7065  me', 'sampletype
-00013010: 272c 2027 6669 6c65 636f 756e 7427 2c20  ', 'filecount', 
-00013020: 2773 697a 6527 0a20 2020 2020 2020 2020  'size'.         
-00013030: 2020 203a 7479 7065 2073 6f72 7469 6e67     :type sorting
-00013040: 5f63 7269 7465 7269 613a 2073 7472 0a20  _criteria: str. 
-00013050: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00013060: 6d20 736f 7274 696e 675f 6f72 6465 723a  m sorting_order:
-00013070: 2073 6f72 7469 6e67 206f 7264 6572 3b20   sorting order; 
-00013080: 706f 7373 6962 6c65 2076 616c 7565 7320  possible values 
-00013090: 6172 6520 2764 6573 6327 2c20 2761 7363  are 'desc', 'asc
-000130a0: 270a 2020 2020 2020 2020 2020 2020 3a74  '.            :t
-000130b0: 7970 6520 736f 7274 696e 675f 6f72 6465  ype sorting_orde
-000130c0: 723a 2073 7472 0a20 2020 2020 2020 2020  r: str.         
-000130d0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
-000130e0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
-000130f0: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
-00013100: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
-00013110: 2020 2022 2222 0a20 2020 2020 2020 2077     """.        w
-00013120: 6172 6e28 2254 6869 7320 6d65 7468 6f64  arn("This method
-00013130: 2069 7320 6465 7072 6563 6174 6564 2e20   is deprecated. 
-00013140: 5573 6520 6164 7661 6e63 6564 5f73 6561  Use advanced_sea
-00013150: 7263 685f 7632 2069 6e73 7465 6164 2e22  rch_v2 instead."
-00013160: 2c20 4465 7072 6563 6174 696f 6e57 6172  , DeprecationWar
-00013170: 6e69 6e67 290a 0a20 2020 2020 2020 2069  ning)..        i
-00013180: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00013190: 2871 7565 7279 5f73 7472 696e 672c 2073  (query_string, s
-000131a0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-000131b0: 2072 6169 7365 2057 726f 6e67 496e 7075   raise WrongInpu
-000131c0: 7445 7272 6f72 2822 5468 6520 7365 6172  tError("The sear
-000131d0: 6368 2071 7565 7279 206d 7573 7420 6265  ch query must be
-000131e0: 2061 2073 7472 696e 672e 2229 0a0a 2020   a string.")..  
-000131f0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-00013200: 6e73 7461 6e63 6528 7265 636f 7264 735f  nstance(records_
-00013210: 7065 725f 7061 6765 2c20 696e 7429 206f  per_page, int) o
-00013220: 7220 6e6f 7420 3120 3c3d 2072 6563 6f72  r not 1 <= recor
-00013230: 6473 5f70 6572 5f70 6167 6520 3c3d 2031  ds_per_page <= 1
-00013240: 3030 3a0a 2020 2020 2020 2020 2020 2020  00:.            
-00013250: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
-00013260: 4572 726f 7228 2272 6563 6f72 6473 5f70  Error("records_p
-00013270: 6572 5f70 6167 6520 7061 7261 6d65 7465  er_page paramete
-00013280: 7220 6d75 7374 2062 6520 616e 2069 6e74  r must be an int
-00013290: 6567 6572 2077 6974 6820 6120 7661 6c75  eger with a valu
-000132a0: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
-000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132c0: 2020 2020 2020 2262 6574 7765 656e 2031        "between 1
-000132d0: 2061 6e64 2031 3030 2028 696e 636c 7564   and 100 (includ
-000132e0: 6564 292e 2229 0a0a 2020 2020 2020 2020  ed).")..        
-000132f0: 7572 6c20 3d20 7365 6c66 2e5f 7572 6c2e  url = self._url.
-00013300: 666f 726d 6174 2865 6e64 706f 696e 743d  format(endpoint=
-00013310: 7365 6c66 2e5f 5f41 4456 414e 4345 445f  self.__ADVANCED_
-00013320: 5345 4152 4348 5f45 4e44 504f 494e 5429  SEARCH_ENDPOINT)
-00013330: 0a0a 2020 2020 2020 2020 706f 7374 5f6a  ..        post_j
-00013340: 736f 6e20 3d20 7b22 7175 6572 7922 3a20  son = {"query": 
-00013350: 7175 6572 795f 7374 7269 6e67 2c20 2270  query_string, "p
-00013360: 6167 6522 3a20 7061 6765 5f6e 756d 6265  age": page_numbe
-00013370: 722c 2022 7265 636f 7264 735f 7065 725f  r, "records_per_
-00013380: 7061 6765 223a 2072 6563 6f72 6473 5f70  page": records_p
-00013390: 6572 5f70 6167 657d 0a0a 2020 2020 2020  er_page}..      
-000133a0: 2020 6966 2073 6f72 7469 6e67 5f63 7269    if sorting_cri
-000133b0: 7465 7269 613a 0a20 2020 2020 2020 2020  teria:.         
-000133c0: 2020 2069 6620 736f 7274 696e 675f 6372     if sorting_cr
-000133d0: 6974 6572 6961 206e 6f74 2069 6e20 4144  iteria not in AD
-000133e0: 5641 4e43 4544 5f53 4541 5243 485f 534f  VANCED_SEARCH_SO
-000133f0: 5254 494e 475f 4352 4954 4552 4941 206f  RTING_CRITERIA o
-00013400: 7220 736f 7274 696e 675f 6f72 6465 7220  r sorting_order 
-00013410: 6e6f 7420 696e 2028 2264 6573 6322 2c20  not in ("desc", 
-00013420: 2261 7363 2229 3a0a 2020 2020 2020 2020  "asc"):.        
-00013430: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
-00013440: 6f6e 6749 6e70 7574 4572 726f 7228 2253  ongInputError("S
-00013450: 6f72 7469 6e67 2063 7269 7465 7269 6120  orting criteria 
-00013460: 6d75 7374 2062 6520 6f6e 6520 6f66 2074  must be one of t
-00013470: 6865 2066 6f6c 6c6f 7769 6e67 206f 7074  he following opt
-00013480: 696f 6e73 3a20 7b63 7269 7465 7269 617d  ions: {criteria}
-00013490: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-000134a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134b0: 2020 2020 2020 2020 2020 2253 6f72 7469            "Sorti
-000134c0: 6e67 206f 7264 6572 206e 6565 6473 2074  ng order needs t
-000134d0: 6f20 6265 2027 6465 7363 2720 6f72 2027  o be 'desc' or '
-000134e0: 6173 6327 2e22 2e66 6f72 6d61 7428 0a20  asc'.".format(. 
-000134f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013510: 2020 2020 2020 2063 7269 7465 7269 613d         criteria=
-00013520: 4144 5641 4e43 4544 5f53 4541 5243 485f  ADVANCED_SEARCH_
-00013530: 534f 5254 494e 475f 4352 4954 4552 4941  SORTING_CRITERIA
-00013540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013560: 2020 2020 2020 2029 290a 2020 2020 2020         )).      
-00013570: 2020 2020 2020 736f 7274 696e 675f 6578        sorting_ex
-00013580: 7072 6573 7369 6f6e 203d 2022 7b63 7269  pression = "{cri
-00013590: 7465 7269 617d 207b 6f72 6465 727d 222e  teria} {order}".
-000135a0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-000135b0: 2020 2020 2020 2020 6372 6974 6572 6961          criteria
-000135c0: 3d73 6f72 7469 6e67 5f63 7269 7465 7269  =sorting_criteri
-000135d0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-000135e0: 2020 206f 7264 6572 3d73 6f72 7469 6e67     order=sorting
-000135f0: 5f6f 7264 6572 0a20 2020 2020 2020 2020  _order.         
-00013600: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00013610: 2020 706f 7374 5f6a 736f 6e5b 2273 6f72    post_json["sor
-00013620: 7422 5d20 3d20 736f 7274 696e 675f 6578  t"] = sorting_ex
-00013630: 7072 6573 7369 6f6e 0a0a 2020 2020 2020  pression..      
-00013640: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00013650: 662e 5f5f 706f 7374 5f72 6571 7565 7374  f.__post_request
-00013660: 2875 726c 3d75 726c 2c20 706f 7374 5f6a  (url=url, post_j
-00013670: 736f 6e3d 706f 7374 5f6a 736f 6e29 0a0a  son=post_json)..
-00013680: 2020 2020 2020 2020 7365 6c66 2e5f 5f72          self.__r
-00013690: 6169 7365 5f6f 6e5f 6572 726f 7228 7265  aise_on_error(re
-000136a0: 7370 6f6e 7365 290a 0a20 2020 2020 2020  sponse)..       
-000136b0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-000136c0: 0a0a 2020 2020 6465 6620 6164 7661 6e63  ..    def advanc
-000136d0: 6564 5f73 6561 7263 685f 6167 6772 6567  ed_search_aggreg
-000136e0: 6174 6564 2873 656c 662c 2071 7565 7279  ated(self, query
-000136f0: 5f73 7472 696e 672c 206d 6178 5f72 6573  _string, max_res
-00013700: 756c 7473 3d35 3030 302c 2073 6f72 7469  ults=5000, sorti
-00013710: 6e67 5f63 7269 7465 7269 613d 4e6f 6e65  ng_criteria=None
-00013720: 2c20 736f 7274 696e 675f 6f72 6465 723d  , sorting_order=
-00013730: 2264 6573 6322 293a 0a20 2020 2020 2020  "desc"):.       
-00013740: 2022 2222 5448 4953 204d 4554 484f 4420   """THIS METHOD 
-00013750: 4953 2044 4550 5245 4341 5445 442e 2055  IS DEPRECATED. U
-00013760: 7365 2061 6476 616e 6365 645f 7365 6172  se advanced_sear
-00013770: 6368 5f76 325f 6167 6772 6567 6174 6564  ch_v2_aggregated
-00013780: 2069 6e73 7465 6164 2e0a 0a20 2020 2020   instead...     
-00013790: 2020 2053 656e 6473 2074 6865 2071 7565     Sends the que
-000137a0: 7279 2073 7472 696e 6720 746f 2074 6865  ry string to the
-000137b0: 2041 3130 3030 2041 6476 616e 6365 6420   A1000 Advanced 
-000137c0: 5365 6172 6368 2041 5049 2e0a 2020 2020  Search API..    
-000137d0: 2020 2020 5468 6520 7175 6572 7920 7374      The query st
-000137e0: 7269 6e67 206d 7573 7420 6265 2063 6f6d  ring must be com
-000137f0: 706f 7365 6420 6f66 206b 6579 2d76 616c  posed of key-val
-00013800: 7565 2070 6169 7273 2073 6570 6172 6174  ue pairs separat
-00013810: 6564 2062 7920 7370 6163 652e 0a20 2020  ed by space..   
-00013820: 2020 2020 2041 206b 6579 2069 7320 7365       A key is se
-00013830: 7061 7261 7465 6420 6672 6f6d 2069 7473  parated from its
-00013840: 2076 616c 7565 2062 7920 6120 636f 6c6f   value by a colo
-00013850: 6e20 7379 6d62 6f6c 2061 6e64 206e 6f20  n symbol and no 
-00013860: 7370 6163 6573 2e0a 2020 2020 2020 2020  spaces..        
-00013870: 5061 6769 6e67 2069 7320 646f 6e65 2061  Paging is done a
-00013880: 7574 6f6d 6174 6963 616c 6c79 2061 6e64  utomatically and
-00013890: 2072 6573 756c 7473 2066 726f 6d20 696e   results from in
-000138a0: 6469 7669 6475 616c 0a20 2020 2020 2020  dividual.       
-000138b0: 2072 6573 706f 6e73 6573 2061 6767 7265   responses aggre
-000138c0: 6761 7465 6420 696e 746f 206f 6e65 206c  gated into one l
-000138d0: 6973 7420 616e 6420 7265 7475 726e 6564  ist and returned
-000138e0: 2e0a 2020 2020 2020 2020 5468 6520 276d  ..        The 'm
-000138f0: 6178 5f72 6573 756c 7473 2720 7061 7261  ax_results' para
-00013900: 6d65 7465 7220 6465 6669 6e65 7320 7468  meter defines th
-00013910: 6520 6d61 7869 6d75 6d20 6465 7369 7265  e maximum desire
-00013920: 6420 6e75 6d62 6572 206f 6620 7265 7375  d number of resu
-00013930: 6c74 7320 746f 2062 6520 7265 7475 726e  lts to be return
-00013940: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00013950: 5175 6572 7920 7374 7269 6e67 2065 7861  Query string exa
-00013960: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-00013970: 2020 2761 762d 636f 756e 743a 3520 6176    'av-count:5 av
-00013980: 6169 6c61 626c 653a 5452 5545 270a 0a20  ailable:TRUE'.. 
-00013990: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-000139a0: 6d20 7175 6572 795f 7374 7269 6e67 3a20  m query_string: 
-000139b0: 7365 6172 6368 2071 7565 7279 202d 2073  search query - s
-000139c0: 6565 2041 5049 2064 6f63 756d 656e 7461  ee API documenta
-000139d0: 7469 6f6e 2066 6f72 2064 6574 6169 6c73  tion for details
-000139e0: 206f 6e20 7772 6974 696e 6720 7365 6172   on writing sear
-000139f0: 6368 2071 7565 7269 6573 0a20 2020 2020  ch queries.     
-00013a00: 2020 2020 2020 203a 7479 7065 2071 7565         :type que
-00013a10: 7279 5f73 7472 696e 673a 2073 7472 0a20  ry_string: str. 
-00013a20: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00013a30: 6d20 6d61 785f 7265 7375 6c74 733a 206d  m max_results: m
-00013a40: 6178 696d 756d 2072 6573 756c 7473 2074  aximum results t
-00013a50: 6f20 6265 2072 6574 7572 6e65 6420 696e  o be returned in
-00013a60: 2061 206c 6973 743b 2064 6566 6175 6c74   a list; default
-00013a70: 2076 616c 7565 2069 7320 3530 3030 0a20   value is 5000. 
-00013a80: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00013a90: 206d 6178 5f72 6573 756c 7473 3a20 696e   max_results: in
-00013aa0: 740a 2020 2020 2020 2020 2020 2020 3a70  t.            :p
-00013ab0: 6172 616d 2073 6f72 7469 6e67 5f63 7269  aram sorting_cri
-00013ac0: 7465 7269 613a 2064 6566 696e 6520 7468  teria: define th
-00013ad0: 6520 6372 6974 6572 6961 2075 7365 6420  e criteria used 
-00013ae0: 696e 2073 6f72 7469 6e67 3b20 706f 7373  in sorting; poss
-00013af0: 6962 6c65 2076 616c 7565 7320 6172 6520  ible values are 
-00013b00: 2773 6861 3127 2c20 2766 6972 7374 7365  'sha1', 'firstse
-00013b10: 656e 272c 0a20 2020 2020 2020 2020 2020  en',.           
-00013b20: 2027 7468 7265 6174 6e61 6d65 272c 2027   'threatname', '
-00013b30: 7361 6d70 6c65 7479 7065 272c 2027 6669  sampletype', 'fi
-00013b40: 6c65 636f 756e 7427 2c20 2773 697a 6527  lecount', 'size'
-00013b50: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00013b60: 7065 2073 6f72 7469 6e67 5f63 7269 7465  pe sorting_crite
-00013b70: 7269 613a 2073 7472 0a20 2020 2020 2020  ria: str.       
-00013b80: 2020 2020 203a 7061 7261 6d20 736f 7274       :param sort
-00013b90: 696e 675f 6f72 6465 723a 2073 6f72 7469  ing_order: sorti
-00013ba0: 6e67 206f 7264 6572 3b20 706f 7373 6962  ng order; possib
-00013bb0: 6c65 2076 616c 7565 7320 6172 6520 2764  le values are 'd
-00013bc0: 6573 6327 2c20 2761 7363 270a 2020 2020  esc', 'asc'.    
-00013bd0: 2020 2020 2020 2020 3a74 7970 6520 736f          :type so
-00013be0: 7274 696e 675f 6f72 6465 723a 2073 7472  rting_order: str
-00013bf0: 0a20 2020 2020 2020 2020 2020 203a 7265  .            :re
-00013c00: 7475 726e 3a20 6c69 7374 206f 6620 7265  turn: list of re
-00013c10: 7375 6c74 730a 2020 2020 2020 2020 2020  sults.          
-00013c20: 2020 3a72 7479 7065 3a20 6c69 7374 0a20    :rtype: list. 
-00013c30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013c40: 2020 2077 6172 6e28 2254 6869 7320 6d65     warn("This me
-00013c50: 7468 6f64 2069 7320 6465 7072 6563 6174  thod is deprecat
-00013c60: 6564 2e20 5573 6520 6164 7661 6e63 6564  ed. Use advanced
-00013c70: 5f73 6561 7263 685f 7632 5f61 6767 7265  _search_v2_aggre
-00013c80: 6761 7465 6420 696e 7374 6561 642e 222c  gated instead.",
-00013c90: 2044 6570 7265 6361 7469 6f6e 5761 726e   DeprecationWarn
-00013ca0: 696e 6729 0a0a 2020 2020 2020 2020 6966  ing)..        if
-00013cb0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00013cc0: 6d61 785f 7265 7375 6c74 732c 2069 6e74  max_results, int
-00013cd0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00013ce0: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
-00013cf0: 7272 6f72 2822 6d61 785f 7265 7375 6c74  rror("max_result
-00013d00: 7320 7061 7261 6d65 7465 7220 6d75 7374  s parameter must
-00013d10: 2062 6520 696e 7465 6765 722e 2229 0a0a   be integer.")..
-00013d20: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
-00013d30: 3d20 5b5d 0a20 2020 2020 2020 206e 6578  = [].        nex
-00013d40: 745f 7061 6765 203d 2031 0a20 2020 2020  t_page = 1.     
-00013d50: 2020 206d 6f72 655f 7061 6765 7320 3d20     more_pages = 
-00013d60: 5472 7565 0a0a 2020 2020 2020 2020 7768  True..        wh
-00013d70: 696c 6520 6d6f 7265 5f70 6167 6573 3a0a  ile more_pages:.
-00013d80: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-00013d90: 6f6e 7365 203d 2073 656c 662e 6164 7661  onse = self.adva
-00013da0: 6e63 6564 5f73 6561 7263 6828 0a20 2020  nced_search(.   
-00013db0: 2020 2020 2020 2020 2020 2020 2071 7565               que
-00013dc0: 7279 5f73 7472 696e 673d 7175 6572 795f  ry_string=query_
-00013dd0: 7374 7269 6e67 2c0a 2020 2020 2020 2020  string,.        
-00013de0: 2020 2020 2020 2020 7061 6765 5f6e 756d          page_num
-00013df0: 6265 723d 6e65 7874 5f70 6167 652c 0a20  ber=next_page,. 
-00013e00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00013e10: 6563 6f72 6473 5f70 6572 5f70 6167 653d  ecords_per_page=
-00013e20: 3130 302c 0a20 2020 2020 2020 2020 2020  100,.           
-00013e30: 2020 2020 2073 6f72 7469 6e67 5f63 7269       sorting_cri
-00013e40: 7465 7269 613d 736f 7274 696e 675f 6372  teria=sorting_cr
-00013e50: 6974 6572 6961 2c0a 2020 2020 2020 2020  iteria,.        
-00013e60: 2020 2020 2020 2020 736f 7274 696e 675f          sorting_
-00013e70: 6f72 6465 723d 736f 7274 696e 675f 6f72  order=sorting_or
-00013e80: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
-00013e90: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00013ea0: 6573 706f 6e73 655f 6a73 6f6e 203d 2072  esponse_json = r
-00013eb0: 6573 706f 6e73 652e 6a73 6f6e 2829 0a0a  esponse.json()..
-00013ec0: 2020 2020 2020 2020 2020 2020 656e 7472              entr
-00013ed0: 6965 7320 3d20 7265 7370 6f6e 7365 5f6a  ies = response_j
-00013ee0: 736f 6e2e 6765 7428 2272 6c22 292e 6765  son.get("rl").ge
-00013ef0: 7428 2277 6562 5f73 6561 7263 685f 6170  t("web_search_ap
-00013f00: 6922 292e 6765 7428 2265 6e74 7269 6573  i").get("entries
-00013f10: 222c 205b 5d29 0a20 2020 2020 2020 2020  ", []).         
-00013f20: 2020 2072 6573 756c 7473 2e65 7874 656e     results.exten
-00013f30: 6428 656e 7472 6965 7329 0a0a 2020 2020  d(entries)..    
-00013f40: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-00013f50: 6573 756c 7473 2920 3e20 6d61 785f 7265  esults) > max_re
-00013f60: 7375 6c74 733a 0a20 2020 2020 2020 2020  sults:.         
-00013f70: 2020 2020 2020 2072 6573 756c 7473 203d         results =
-00013f80: 2072 6573 756c 7473 5b3a 6d61 785f 7265   results[:max_re
-00013f90: 7375 6c74 735d 0a20 2020 2020 2020 2020  sults].         
-00013fa0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00013fb0: 7375 6c74 730a 0a20 2020 2020 2020 2020  sults..         
-00013fc0: 2020 206e 6578 745f 7061 6765 203d 2072     next_page = r
-00013fd0: 6573 706f 6e73 655f 6a73 6f6e 2e67 6574  esponse_json.get
-00013fe0: 2822 726c 2229 2e67 6574 2822 7765 625f  ("rl").get("web_
-00013ff0: 7365 6172 6368 5f61 7069 2229 2e67 6574  search_api").get
-00014000: 2822 6e65 7874 5f70 6167 6522 2c20 4e6f  ("next_page", No
-00014010: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-00014020: 6d6f 7265 5f70 6167 6573 203d 2072 6573  more_pages = res
-00014030: 706f 6e73 655f 6a73 6f6e 2e67 6574 2822  ponse_json.get("
-00014040: 726c 2229 2e67 6574 2822 7765 625f 7365  rl").get("web_se
-00014050: 6172 6368 5f61 7069 2229 2e67 6574 2822  arch_api").get("
-00014060: 6d6f 7265 5f70 6167 6573 222c 2046 616c  more_pages", Fal
-00014070: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
-00014080: 7572 6e20 7265 7375 6c74 730a 0a20 2020  urn results..   
-00014090: 2064 6566 2061 6476 616e 6365 645f 7365   def advanced_se
-000140a0: 6172 6368 5f76 3228 7365 6c66 2c20 7175  arch_v2(self, qu
-000140b0: 6572 795f 7374 7269 6e67 2c20 7469 636c  ery_string, ticl
-000140c0: 6f75 643d 4661 6c73 652c 2070 6167 655f  oud=False, page_
-000140d0: 6e75 6d62 6572 3d31 2c20 7265 636f 7264  number=1, record
-000140e0: 735f 7065 725f 7061 6765 3d32 302c 2073  s_per_page=20, s
-000140f0: 6f72 7469 6e67 5f63 7269 7465 7269 613d  orting_criteria=
-00014100: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00014110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014120: 2073 6f72 7469 6e67 5f6f 7264 6572 3d22   sorting_order="
-00014130: 6465 7363 2229 3a0a 2020 2020 2020 2020  desc"):.        
-00014140: 2222 2253 656e 6473 2061 2071 7565 7279  """Sends a query
-00014150: 2073 7472 696e 6720 746f 2074 6865 2041   string to the A
-00014160: 3130 3030 2041 6476 616e 6365 6420 5365  1000 Advanced Se
-00014170: 6172 6368 2041 5049 2076 322e 0a20 2020  arch API v2..   
-00014180: 2020 2020 2054 6865 2071 7565 7279 2073       The query s
-00014190: 7472 696e 6720 6d75 7374 2062 6520 636f  tring must be co
-000141a0: 6d70 6f73 6564 206f 6620 6b65 792d 7661  mposed of key-va
-000141b0: 6c75 6520 7061 6972 7320 7365 7061 7261  lue pairs separa
-000141c0: 7465 6420 6279 2073 7061 6365 2e0a 2020  ted by space..  
-000141d0: 2020 2020 2020 4120 6b65 7920 6973 2073        A key is s
-000141e0: 6570 6172 6174 6564 2066 726f 6d20 6974  eparated from it
-000141f0: 7320 7661 6c75 6520 6279 2061 2063 6f6c  s value by a col
-00014200: 6f6e 2073 796d 626f 6c20 616e 6420 6e6f  on symbol and no
-00014210: 2073 7061 6365 732e 0a20 2020 2020 2020   spaces..       
-00014220: 2046 6f72 2064 6972 6563 7469 6f6e 7320   For directions 
-00014230: 6f6e 2068 6f77 2074 6f20 7772 6974 6520  on how to write 
-00014240: 6164 7661 6e63 6564 2073 6561 7263 6820  advanced search 
-00014250: 7175 6572 6965 732c 2063 6f6e 7375 6c74  queries, consult
-00014260: 2074 6865 2041 3130 3030 2064 6f63 756d   the A1000 docum
-00014270: 656e 7461 7469 6f6e 2e0a 2020 2020 2020  entation..      
-00014280: 2020 4966 2061 2070 6167 6520 6e75 6d62    If a page numb
-00014290: 6572 2069 7320 6e6f 7420 7072 6f76 6964  er is not provid
-000142a0: 6564 2c20 7468 6520 6669 7273 7420 7061  ed, the first pa
-000142b0: 6765 206f 6620 7265 7375 6c74 7320 7769  ge of results wi
-000142c0: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
-000142d0: 2020 2020 2020 2020 2020 2020 5175 6572              Quer
-000142e0: 7920 7374 7269 6e67 2065 7861 6d70 6c65  y string example
-000142f0: 3a0a 2020 2020 2020 2020 2020 2020 2761  :.            'a
-00014300: 762d 636f 756e 743a 3520 6176 6169 6c61  v-count:5 availa
-00014310: 626c 653a 5452 5545 270a 0a20 2020 2020  ble:TRUE'..     
-00014320: 2020 2020 2020 203a 7061 7261 6d20 7175         :param qu
-00014330: 6572 795f 7374 7269 6e67 3a20 7175 6572  ery_string: quer
-00014340: 7920 7374 7269 6e67 0a20 2020 2020 2020  y string.       
-00014350: 2020 2020 203a 7479 7065 2071 7565 7279       :type query
-00014360: 5f73 7472 696e 673a 2073 7472 0a20 2020  _string: str.   
-00014370: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00014380: 7469 636c 6f75 643a 2073 686f 7720 6f6e  ticloud: show on
-00014390: 6c79 2063 6c6f 7564 2072 6573 756c 7473  ly cloud results
-000143a0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-000143b0: 7065 2074 6963 6c6f 7564 3a20 626f 6f6c  pe ticloud: bool
-000143c0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-000143d0: 7261 6d20 7061 6765 5f6e 756d 6265 723a  ram page_number:
-000143e0: 2070 6167 6520 6e75 6d62 6572 0a20 2020   page number.   
-000143f0: 2020 2020 2020 2020 203a 7479 7065 2070           :type p
-00014400: 6167 655f 6e75 6d62 6572 3a20 696e 740a  age_number: int.
-00014410: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00014420: 616d 2072 6563 6f72 6473 5f70 6572 5f70  am records_per_p
-00014430: 6167 653a 206e 756d 6265 7220 6f66 2072  age: number of r
-00014440: 6563 6f72 6473 2072 6574 7572 6e65 6420  ecords returned 
-00014450: 7065 7220 7061 6765 3b20 6d61 7869 6d75  per page; maximu
-00014460: 6d20 7661 6c75 6520 6973 2031 3030 0a20  m value is 100. 
-00014470: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00014480: 2072 6563 6f72 6473 5f70 6572 5f70 6167   records_per_pag
-00014490: 653a 2069 6e74 0a20 2020 2020 2020 2020  e: int.         
-000144a0: 2020 203a 7061 7261 6d20 736f 7274 696e     :param sortin
-000144b0: 675f 6372 6974 6572 6961 3a20 6465 6669  g_criteria: defi
-000144c0: 6e65 2074 6865 2063 7269 7465 7269 6120  ne the criteria 
-000144d0: 7573 6564 2069 6e20 736f 7274 696e 673b  used in sorting;
-000144e0: 2070 6f73 7369 626c 6520 7661 6c75 6573   possible values
-000144f0: 2061 7265 2027 7368 6131 272c 2027 6669   are 'sha1', 'fi
-00014500: 7273 7473 6565 6e27 2c0a 2020 2020 2020  rstseen',.      
-00014510: 2020 2020 2020 2774 6872 6561 746e 616d        'threatnam
-00014520: 6527 2c20 2773 616d 706c 6574 7970 6527  e', 'sampletype'
-00014530: 2c20 2766 696c 6563 6f75 6e74 272c 2027  , 'filecount', '
-00014540: 7369 7a65 270a 2020 2020 2020 2020 2020  size'.          
-00014550: 2020 3a74 7970 6520 736f 7274 696e 675f    :type sorting_
-00014560: 6372 6974 6572 6961 3a20 7374 720a 2020  criteria: str.  
-00014570: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00014580: 2073 6f72 7469 6e67 5f6f 7264 6572 3a20   sorting_order: 
-00014590: 736f 7274 696e 6720 6f72 6465 723b 2070  sorting order; p
-000145a0: 6f73 7369 626c 6520 7661 6c75 6573 2061  ossible values a
-000145b0: 7265 2027 6465 7363 272c 2027 6173 6327  re 'desc', 'asc'
-000145c0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-000145d0: 7065 2073 6f72 7469 6e67 5f6f 7264 6572  pe sorting_order
-000145e0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-000145f0: 2020 3a72 6574 7572 6e3a 2072 6573 706f    :return: respo
-00014600: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
-00014610: 3a72 7479 7065 3a20 7265 7175 6573 7473  :rtype: requests
-00014620: 2e52 6573 706f 6e73 650a 2020 2020 2020  .Response.      
-00014630: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00014640: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00014650: 7175 6572 795f 7374 7269 6e67 2c20 7374  query_string, st
-00014660: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00014670: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
-00014680: 4572 726f 7228 2254 6865 2073 6561 7263  Error("The searc
-00014690: 6820 7175 6572 7920 6d75 7374 2062 6520  h query must be 
-000146a0: 6120 7374 7269 6e67 2e22 290a 0a20 2020  a string.")..   
-000146b0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-000146c0: 7374 616e 6365 2874 6963 6c6f 7564 2c20  stance(ticloud, 
-000146d0: 626f 6f6c 293a 0a20 2020 2020 2020 2020  bool):.         
-000146e0: 2020 2072 6169 7365 2057 726f 6e67 496e     raise WrongIn
-000146f0: 7075 7445 7272 6f72 2822 7469 636c 6f75  putError("ticlou
-00014700: 6420 7061 7261 6d65 7465 7220 6d75 7374  d parameter must
-00014710: 2062 6520 626f 6f6c 6561 6e2e 2229 0a0a   be boolean.")..
-00014720: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00014730: 7369 6e73 7461 6e63 6528 7265 636f 7264  sinstance(record
-00014740: 735f 7065 725f 7061 6765 2c20 696e 7429  s_per_page, int)
-00014750: 206f 7220 6e6f 7420 3120 3c3d 2072 6563   or not 1 <= rec
-00014760: 6f72 6473 5f70 6572 5f70 6167 6520 3c3d  ords_per_page <=
-00014770: 2031 3030 3a0a 2020 2020 2020 2020 2020   100:.          
-00014780: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
-00014790: 7574 4572 726f 7228 2272 6563 6f72 6473  utError("records
-000147a0: 5f70 6572 5f70 6167 6520 7061 7261 6d65  _per_page parame
-000147b0: 7465 7220 6d75 7374 2062 6520 616e 2069  ter must be an i
-000147c0: 6e74 6567 6572 2077 6974 6820 6120 7661  nteger with a va
-000147d0: 6c75 6520 220a 2020 2020 2020 2020 2020  lue ".          
-000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147f0: 2020 2020 2020 2020 2262 6574 7765 656e          "between
-00014800: 2031 2061 6e64 2031 3030 2028 696e 636c   1 and 100 (incl
-00014810: 7564 6564 292e 2229 0a0a 2020 2020 2020  uded).")..      
-00014820: 2020 7572 6c20 3d20 7365 6c66 2e5f 7572    url = self._ur
-00014830: 6c2e 666f 726d 6174 2865 6e64 706f 696e  l.format(endpoin
-00014840: 743d 7365 6c66 2e5f 5f41 4456 414e 4345  t=self.__ADVANCE
-00014850: 445f 5345 4152 4348 5f45 4e44 504f 494e  D_SEARCH_ENDPOIN
-00014860: 545f 5632 290a 0a20 2020 2020 2020 2070  T_V2)..        p
-00014870: 6f73 745f 6a73 6f6e 203d 207b 2271 7565  ost_json = {"que
-00014880: 7279 223a 2071 7565 7279 5f73 7472 696e  ry": query_strin
-00014890: 672c 2022 7469 636c 6f75 6422 3a20 7469  g, "ticloud": ti
-000148a0: 636c 6f75 642c 2022 7061 6765 223a 2070  cloud, "page": p
-000148b0: 6167 655f 6e75 6d62 6572 2c0a 2020 2020  age_number,.    
-000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148d0: 2022 7265 636f 7264 735f 7065 725f 7061   "records_per_pa
-000148e0: 6765 223a 2072 6563 6f72 6473 5f70 6572  ge": records_per
-000148f0: 5f70 6167 657d 0a0a 2020 2020 2020 2020  _page}..        
-00014900: 6966 2073 6f72 7469 6e67 5f63 7269 7465  if sorting_crite
-00014910: 7269 613a 0a20 2020 2020 2020 2020 2020  ria:.           
-00014920: 2069 6620 736f 7274 696e 675f 6372 6974   if sorting_crit
-00014930: 6572 6961 206e 6f74 2069 6e20 4144 5641  eria not in ADVA
-00014940: 4e43 4544 5f53 4541 5243 485f 534f 5254  NCED_SEARCH_SORT
-00014950: 494e 475f 4352 4954 4552 4941 206f 7220  ING_CRITERIA or 
-00014960: 736f 7274 696e 675f 6f72 6465 7220 6e6f  sorting_order no
-00014970: 7420 696e 2028 2264 6573 6322 2c20 2261  t in ("desc", "a
-00014980: 7363 2229 3a0a 2020 2020 2020 2020 2020  sc"):.          
-00014990: 2020 2020 2020 7261 6973 6520 5772 6f6e        raise Wron
-000149a0: 6749 6e70 7574 4572 726f 7228 2253 6f72  gInputError("Sor
-000149b0: 7469 6e67 2063 7269 7465 7269 6120 6d75  ting criteria mu
-000149c0: 7374 2062 6520 6f6e 6520 6f66 2074 6865  st be one of the
-000149d0: 2066 6f6c 6c6f 7769 6e67 206f 7074 696f   following optio
-000149e0: 6e73 3a20 7b63 7269 7465 7269 617d 2e20  ns: {criteria}. 
-000149f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00014a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a10: 2020 2020 2020 2020 2253 6f72 7469 6e67          "Sorting
-00014a20: 206f 7264 6572 206e 6565 6473 2074 6f20   order needs to 
-00014a30: 6265 2027 6465 7363 2720 6f72 2027 6173  be 'desc' or 'as
-00014a40: 6327 2e22 2e66 6f72 6d61 7428 0a20 2020  c'.".format(.   
-00014a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a70: 2020 2020 2063 7269 7465 7269 613d 4144       criteria=AD
-00014a80: 5641 4e43 4544 5f53 4541 5243 485f 534f  VANCED_SEARCH_SO
-00014a90: 5254 494e 475f 4352 4954 4552 4941 0a20  RTING_CRITERIA. 
+0000e110: 2020 2020 2020 2020 7265 706f 7274 5f66          report_f
+0000e120: 6f72 6d61 742c 0a20 2020 2020 2020 2020  ormat,.         
+0000e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e160: 2020 2073 656c 662e 5f5f 4459 4e41 4d49     self.__DYNAMI
+0000e170: 435f 414e 414c 5953 4953 5f52 4550 4f52  C_ANALYSIS_REPOR
+0000e180: 545f 444f 574e 4c4f 4144 5f45 4e44 504f  T_DOWNLOAD_ENDPO
+0000e190: 494e 5429 0a20 2020 2020 2020 2072 6574  INT).        ret
+0000e1a0: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+0000e1b0: 2020 6465 6620 7365 745f 636c 6173 7369    def set_classi
+0000e1c0: 6669 6361 7469 6f6e 2873 656c 662c 2073  fication(self, s
+0000e1d0: 616d 706c 655f 6861 7368 2c20 636c 6173  ample_hash, clas
+0000e1e0: 7369 6669 6361 7469 6f6e 2c20 7379 7374  sification, syst
+0000e1f0: 656d 2c20 7269 736b 5f73 636f 7265 3d4e  em, risk_score=N
+0000e200: 6f6e 652c 2074 6872 6561 745f 706c 6174  one, threat_plat
+0000e210: 666f 726d 3d4e 6f6e 652c 0a20 2020 2020  form=None,.     
+0000e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e230: 2020 2020 2020 7468 7265 6174 5f74 7970        threat_typ
+0000e240: 653d 4e6f 6e65 2c20 7468 7265 6174 5f6e  e=None, threat_n
+0000e250: 616d 653d 4e6f 6e65 293a 0a20 2020 2020  ame=None):.     
+0000e260: 2020 2022 2222 4163 6365 7074 7320 6120     """Accepts a 
+0000e270: 7369 6e67 6c65 2068 6173 6820 7374 7269  single hash stri
+0000e280: 6e67 2c20 616c 6c6f 7773 2074 6865 2075  ng, allows the u
+0000e290: 7365 7220 746f 2073 6574 2074 6865 2063  ser to set the c
+0000e2a0: 6c61 7373 6966 6963 6174 696f 6e20 6f66  lassification of
+0000e2b0: 2061 2073 616d 706c 652c 2065 6974 6865   a sample, eithe
+0000e2c0: 7220 696e 2054 6974 616e 6975 6d43 6c6f  r in TitaniumClo
+0000e2d0: 7564 0a20 2020 2020 2020 206f 7220 6c6f  ud.        or lo
+0000e2e0: 6361 6c6c 7920 6f6e 2074 6865 2041 3130  cally on the A10
+0000e2f0: 3030 2e20 5265 7475 726e 7320 6120 7265  00. Returns a re
+0000e300: 7370 6f6e 7365 2063 6f6e 7461 696e 696e  sponse containin
+0000e310: 6720 6120 6e65 7720 636c 6173 7369 6669  g a new classifi
+0000e320: 6361 7469 6f6e 2e0a 2020 2020 2020 2020  cation..        
+0000e330: 2020 2020 3a70 6172 616d 2073 616d 706c      :param sampl
+0000e340: 655f 6861 7368 3a20 6861 7368 2073 7472  e_hash: hash str
+0000e350: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+0000e360: 3a74 7970 6520 7361 6d70 6c65 5f68 6173  :type sample_has
+0000e370: 683a 2073 7472 0a20 2020 2020 2020 2020  h: str.         
+0000e380: 2020 203a 7061 7261 6d20 7379 7374 656d     :param system
+0000e390: 3a20 276c 6f63 616c 2720 6f72 2027 7469  : 'local' or 'ti
+0000e3a0: 636c 6f75 6427 0a20 2020 2020 2020 2020  cloud'.         
+0000e3b0: 2020 203a 7479 7065 2073 7973 7465 6d3a     :type system:
+0000e3c0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+0000e3d0: 203a 7061 7261 6d20 636c 6173 7369 6669   :param classifi
+0000e3e0: 6361 7469 6f6e 3a20 2767 6f6f 6477 6172  cation: 'goodwar
+0000e3f0: 6527 2c20 2773 7573 7069 6369 6f75 7327  e', 'suspicious'
+0000e400: 206f 7220 276d 616c 6963 696f 7573 270a   or 'malicious'.
+0000e410: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+0000e420: 6520 636c 6173 7369 6669 6361 7469 6f6e  e classification
+0000e430: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+0000e440: 2020 3a70 6172 616d 2072 6973 6b5f 7363    :param risk_sc
+0000e450: 6f72 653a 2049 6620 7370 6563 6966 6965  ore: If specifie
+0000e460: 642c 2069 7420 6d75 7374 2062 6520 7769  d, it must be wi
+0000e470: 7468 696e 2072 616e 6765 2066 6f72 2074  thin range for t
+0000e480: 6865 2073 7065 6369 6669 6564 2063 6c61  he specified cla
+0000e490: 7373 6966 6963 6174 696f 6e2e 2049 6620  ssification. If 
+0000e4a0: 6e6f 7420 7370 6563 6966 6965 642c 0a20  not specified,. 
+0000e4b0: 2020 2020 2020 2020 2020 2061 2064 6566             a def
+0000e4c0: 6175 6c74 2076 616c 7565 2069 7320 7573  ault value is us
+0000e4d0: 6564 3a20 476f 6f64 7761 7265 3a20 302c  ed: Goodware: 0,
+0000e4e0: 2053 7573 7069 6369 6f75 733a 2036 2c20   Suspicious: 6, 
+0000e4f0: 4d61 6c69 6369 6f75 733a 2031 300a 2020  Malicious: 10.  
+0000e500: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+0000e510: 7269 736b 5f73 636f 7265 3a20 7374 720a  risk_score: str.
+0000e520: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0000e530: 616d 2074 6872 6561 745f 706c 6174 666f  am threat_platfo
+0000e540: 726d 3a20 6966 2073 7065 6369 6669 6564  rm: if specified
+0000e550: 2c20 6974 206d 7573 7420 6265 206f 6e20  , it must be on 
+0000e560: 7468 6520 7375 7070 6f72 7465 6420 6c69  the supported li
+0000e570: 7374 2028 706c 6174 666f 726d 7320 616e  st (platforms an
+0000e580: 6420 7375 6270 6c61 7466 6f72 6d73 202d  d subplatforms -
+0000e590: 2073 6565 0a20 2020 2020 2020 2020 2020   see.           
+0000e5a0: 206f 6666 6963 6961 6c20 4150 4920 646f   official API do
+0000e5b0: 6373 292e 2049 6620 6e6f 7420 7370 6563  cs). If not spec
+0000e5c0: 6966 6965 642c 2074 6865 2064 6566 6175  ified, the defau
+0000e5d0: 6c74 2076 616c 7565 2069 7320 2757 696e  lt value is 'Win
+0000e5e0: 3332 272e 0a20 2020 2020 2020 2020 2020  32'..           
+0000e5f0: 203a 7479 7065 2074 6872 6561 745f 706c   :type threat_pl
+0000e600: 6174 666f 726d 3a20 7374 720a 2020 2020  atform: str.    
+0000e610: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
+0000e620: 6872 6561 745f 7479 7065 3a20 4966 2073  hreat_type: If s
+0000e630: 7065 6369 6669 6564 2c20 6974 206d 7573  pecified, it mus
+0000e640: 7420 6265 206f 6e20 7468 6520 7375 7070  t be on the supp
+0000e650: 6f72 7465 6420 6c69 7374 2028 6d61 6c77  orted list (malw
+0000e660: 6172 6520 7479 7065 7320 2d20 7365 6520  are types - see 
+0000e670: 6f66 6669 6369 616c 2041 5049 2064 6f63  official API doc
+0000e680: 7329 2e0a 2020 2020 2020 2020 2020 2020  s)..            
+0000e690: 4966 206e 6f74 2073 7065 6369 6669 6564  If not specified
+0000e6a0: 2c20 7468 6520 6465 6661 756c 7420 7661  , the default va
+0000e6b0: 6c75 6520 6973 2027 4d61 6c77 6172 6527  lue is 'Malware'
+0000e6c0: 2e0a 2020 2020 2020 2020 2020 2020 3a74  ..            :t
+0000e6d0: 7970 6520 7468 7265 6174 5f74 7970 653a  ype threat_type:
+0000e6e0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+0000e6f0: 203a 7061 7261 6d20 7468 7265 6174 5f6e   :param threat_n
+0000e700: 616d 653a 2049 6620 7370 6563 6966 6965  ame: If specifie
+0000e710: 642c 206d 7573 7420 6265 2061 6e20 616c  d, must be an al
+0000e720: 7068 616e 756d 6572 6963 2073 7472 696e  phanumeric strin
+0000e730: 6720 6e6f 7420 6c6f 6e67 6572 2074 6861  g not longer tha
+0000e740: 6e20 3332 2063 6861 7261 6374 6572 732e  n 32 characters.
+0000e750: 2049 6620 6e6f 740a 2020 2020 2020 2020   If not.        
+0000e760: 2020 2020 7370 6563 6966 6965 642c 2074      specified, t
+0000e770: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
+0000e780: 2069 7320 2747 656e 6572 6963 272e 0a20   is 'Generic'.. 
+0000e790: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+0000e7a0: 2074 6872 6561 745f 6e61 6d65 3a20 7374   threat_name: st
+0000e7b0: 720a 2020 2020 2020 2020 2020 2020 3a72  r.            :r
+0000e7c0: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
+0000e7d0: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
+0000e7e0: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
+0000e7f0: 706f 6e73 650a 2020 2020 2020 2020 2222  ponse.        ""
+0000e800: 220a 2020 2020 2020 2020 7661 6c69 6461  ".        valida
+0000e810: 7465 5f68 6173 6865 7328 0a20 2020 2020  te_hashes(.     
+0000e820: 2020 2020 2020 2068 6173 685f 696e 7075         hash_inpu
+0000e830: 743d 5b73 616d 706c 655f 6861 7368 5d2c  t=[sample_hash],
+0000e840: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
+0000e850: 6f77 6564 5f68 6173 685f 7479 7065 733d  owed_hash_types=
+0000e860: 284d 4435 2c20 5348 4131 2c20 5348 4132  (MD5, SHA1, SHA2
+0000e870: 3536 2c20 5348 4135 3132 290a 2020 2020  56, SHA512).    
+0000e880: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+0000e890: 6620 7379 7374 656d 206e 6f74 2069 6e20  f system not in 
+0000e8a0: 2822 6c6f 6361 6c22 2c20 2274 6963 6c6f  ("local", "ticlo
+0000e8b0: 7564 2229 3a0a 2020 2020 2020 2020 2020  ud"):.          
+0000e8c0: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+0000e8d0: 7574 4572 726f 7228 2273 7973 7465 6d20  utError("system 
+0000e8e0: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
+0000e8f0: 6520 6569 7468 6572 2027 6c6f 6361 6c27  e either 'local'
+0000e900: 206f 7220 2774 6963 6c6f 7564 272e 2229   or 'ticloud'.")
+0000e910: 0a0a 2020 2020 2020 2020 656e 6470 6f69  ..        endpoi
+0000e920: 6e74 203d 2073 656c 662e 5f5f 5345 545f  nt = self.__SET_
+0000e930: 4f52 5f44 454c 4554 455f 434c 4153 5349  OR_DELETE_CLASSI
+0000e940: 4649 4341 5449 4f4e 5f45 4e44 504f 494e  FICATION_ENDPOIN
+0000e950: 542e 666f 726d 6174 280a 2020 2020 2020  T.format(.      
+0000e960: 2020 2020 2020 6861 7368 5f76 616c 7565        hash_value
+0000e970: 3d73 616d 706c 655f 6861 7368 2c0a 2020  =sample_hash,.  
+0000e980: 2020 2020 2020 2020 2020 7379 7374 656d            system
+0000e990: 3d73 7973 7465 6d0a 2020 2020 2020 2020  =system.        
+0000e9a0: 290a 0a20 2020 2020 2020 2064 6174 6120  )..        data 
+0000e9b0: 3d20 7365 6c66 2e5f 5f63 7265 6174 655f  = self.__create_
+0000e9c0: 706f 7374 5f70 6179 6c6f 6164 280a 2020  post_payload(.  
+0000e9d0: 2020 2020 2020 2020 2020 636c 6173 7369            classi
+0000e9e0: 6669 6361 7469 6f6e 3d63 6c61 7373 6966  fication=classif
+0000e9f0: 6963 6174 696f 6e2c 0a20 2020 2020 2020  ication,.       
+0000ea00: 2020 2020 2072 6973 6b5f 7363 6f72 653d       risk_score=
+0000ea10: 7269 736b 5f73 636f 7265 2c0a 2020 2020  risk_score,.    
+0000ea20: 2020 2020 2020 2020 7468 7265 6174 5f70          threat_p
+0000ea30: 6c61 7466 6f72 6d3d 7468 7265 6174 5f70  latform=threat_p
+0000ea40: 6c61 7466 6f72 6d2c 0a20 2020 2020 2020  latform,.       
+0000ea50: 2020 2020 2074 6872 6561 745f 7479 7065       threat_type
+0000ea60: 3d74 6872 6561 745f 7479 7065 2c0a 2020  =threat_type,.  
+0000ea70: 2020 2020 2020 2020 2020 7468 7265 6174            threat
+0000ea80: 5f6e 616d 653d 7468 7265 6174 5f6e 616d  _name=threat_nam
+0000ea90: 650a 2020 2020 2020 2020 290a 0a20 2020  e.        )..   
+0000eaa0: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
+0000eab0: 5f75 726c 2e66 6f72 6d61 7428 656e 6470  _url.format(endp
+0000eac0: 6f69 6e74 3d65 6e64 706f 696e 7429 0a0a  oint=endpoint)..
+0000ead0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+0000eae0: 203d 2073 656c 662e 5f5f 706f 7374 5f72   = self.__post_r
+0000eaf0: 6571 7565 7374 2875 726c 3d75 726c 2c20  equest(url=url, 
+0000eb00: 6461 7461 3d64 6174 6129 0a0a 2020 2020  data=data)..    
+0000eb10: 2020 2020 7365 6c66 2e5f 5f72 6169 7365      self.__raise
+0000eb20: 5f6f 6e5f 6572 726f 7228 7265 7370 6f6e  _on_error(respon
+0000eb30: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
+0000eb40: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+0000eb50: 2020 6465 6620 6465 6c65 7465 5f63 6c61    def delete_cla
+0000eb60: 7373 6966 6963 6174 696f 6e28 7365 6c66  ssification(self
+0000eb70: 2c20 7361 6d70 6c65 5f68 6173 682c 2073  , sample_hash, s
+0000eb80: 7973 7465 6d3d 226c 6f63 616c 2229 3a0a  ystem="local"):.
+0000eb90: 2020 2020 2020 2020 2222 2241 6363 6570          """Accep
+0000eba0: 7473 2061 2073 696e 676c 6520 6861 7368  ts a single hash
+0000ebb0: 2073 7472 696e 672c 2061 6c6c 6f77 7320   string, allows 
+0000ebc0: 7468 6520 7573 6572 2074 6f20 6465 6c65  the user to dele
+0000ebd0: 7465 2074 6865 2063 6c61 7373 6966 6963  te the classific
+0000ebe0: 6174 696f 6e20 6f66 2061 2073 616d 706c  ation of a sampl
+0000ebf0: 652c 2065 6974 6865 7220 696e 0a20 2020  e, either in.   
+0000ec00: 2020 2020 2054 6974 616e 6975 6d43 6c6f       TitaniumClo
+0000ec10: 7564 206f 7220 6c6f 6361 6c6c 7920 6f6e  ud or locally on
+0000ec20: 2074 6865 2041 3130 3030 2e0a 2020 2020   the A1000..    
+0000ec30: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+0000ec40: 616d 706c 655f 6861 7368 3a20 6861 7368  ample_hash: hash
+0000ec50: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+0000ec60: 2020 2020 3a74 7970 6520 7361 6d70 6c65      :type sample
+0000ec70: 5f68 6173 683a 2073 7472 0a20 2020 2020  _hash: str.     
+0000ec80: 2020 2020 2020 203a 7061 7261 6d20 7379         :param sy
+0000ec90: 7374 656d 3a20 276c 6f63 616c 2720 6f72  stem: 'local' or
+0000eca0: 2027 7469 636c 6f75 6427 0a20 2020 2020   'ticloud'.     
+0000ecb0: 2020 2020 2020 203a 7479 7065 2073 7973         :type sys
+0000ecc0: 7465 6d3a 2073 7472 0a20 2020 2020 2020  tem: str.       
+0000ecd0: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
+0000ece0: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
+0000ecf0: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
+0000ed00: 7374 732e 5265 7370 6f6e 7365 0a20 2020  sts.Response.   
+0000ed10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ed20: 2076 616c 6964 6174 655f 6861 7368 6573   validate_hashes
+0000ed30: 280a 2020 2020 2020 2020 2020 2020 6861  (.            ha
+0000ed40: 7368 5f69 6e70 7574 3d5b 7361 6d70 6c65  sh_input=[sample
+0000ed50: 5f68 6173 685d 2c0a 2020 2020 2020 2020  _hash],.        
+0000ed60: 2020 2020 616c 6c6f 7765 645f 6861 7368      allowed_hash
+0000ed70: 5f74 7970 6573 3d28 4d44 352c 2053 4841  _types=(MD5, SHA
+0000ed80: 312c 2053 4841 3235 362c 2053 4841 3531  1, SHA256, SHA51
+0000ed90: 3229 0a20 2020 2020 2020 2029 0a0a 2020  2).        )..  
+0000eda0: 2020 2020 2020 6966 2073 7973 7465 6d20        if system 
+0000edb0: 616e 6420 7379 7374 656d 206e 6f74 2069  and system not i
+0000edc0: 6e20 2822 6c6f 6361 6c22 2c20 2274 6963  n ("local", "tic
+0000edd0: 6c6f 7564 2229 3a0a 2020 2020 2020 2020  loud"):.        
+0000ede0: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
+0000edf0: 6e70 7574 4572 726f 7228 2273 7973 7465  nputError("syste
+0000ee00: 6d20 7061 7261 6d65 7465 7220 6d75 7374  m parameter must
+0000ee10: 2062 6520 6569 7468 6572 2027 6c6f 6361   be either 'loca
+0000ee20: 6c27 206f 7220 2774 6963 6c6f 7564 272e  l' or 'ticloud'.
+0000ee30: 2229 0a0a 2020 2020 2020 2020 656e 6470  ")..        endp
+0000ee40: 6f69 6e74 203d 2073 656c 662e 5f5f 5345  oint = self.__SE
+0000ee50: 545f 4f52 5f44 454c 4554 455f 434c 4153  T_OR_DELETE_CLAS
+0000ee60: 5349 4649 4341 5449 4f4e 5f45 4e44 504f  SIFICATION_ENDPO
+0000ee70: 494e 542e 666f 726d 6174 280a 2020 2020  INT.format(.    
+0000ee80: 2020 2020 2020 2020 6861 7368 5f76 616c          hash_val
+0000ee90: 7565 3d73 616d 706c 655f 6861 7368 2c0a  ue=sample_hash,.
+0000eea0: 2020 2020 2020 2020 2020 2020 7379 7374              syst
+0000eeb0: 656d 3d73 7973 7465 6d0a 2020 2020 2020  em=system.      
+0000eec0: 2020 290a 0a20 2020 2020 2020 2075 726c    )..        url
+0000eed0: 203d 2073 656c 662e 5f75 726c 2e66 6f72   = self._url.for
+0000eee0: 6d61 7428 656e 6470 6f69 6e74 3d65 6e64  mat(endpoint=end
+0000eef0: 706f 696e 7429 0a0a 2020 2020 2020 2020  point)..        
+0000ef00: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+0000ef10: 5f5f 6465 6c65 7465 5f72 6571 7565 7374  __delete_request
+0000ef20: 2875 726c 3d75 726c 290a 0a20 2020 2020  (url=url)..     
+0000ef30: 2020 2073 656c 662e 5f5f 7261 6973 655f     self.__raise_
+0000ef40: 6f6e 5f65 7272 6f72 2872 6573 706f 6e73  on_error(respons
+0000ef50: 6529 0a0a 2020 2020 2020 2020 7265 7475  e)..        retu
+0000ef60: 726e 2072 6573 706f 6e73 650a 0a20 2020  rn response..   
+0000ef70: 2064 6566 2067 6574 5f75 7365 725f 7461   def get_user_ta
+0000ef80: 6773 2873 656c 662c 2073 616d 706c 655f  gs(self, sample_
+0000ef90: 6861 7368 293a 0a20 2020 2020 2020 2022  hash):.        "
+0000efa0: 2222 4163 6365 7074 7320 6120 7369 6e67  ""Accepts a sing
+0000efb0: 6c65 2068 6173 6820 7374 7269 6e67 2061  le hash string a
+0000efc0: 6e64 2072 6574 7572 6e73 206c 6973 7473  nd returns lists
+0000efd0: 206f 6620 6578 6973 7469 6e67 2075 7365   of existing use
+0000efe0: 7220 7461 6773 2066 6f72 2074 6865 2072  r tags for the r
+0000eff0: 6571 7565 7374 6564 2073 616d 706c 652e  equested sample.
+0000f000: 0a20 2020 2020 2020 2020 2020 3a70 6172  .           :par
+0000f010: 616d 2073 616d 706c 655f 6861 7368 3a20  am sample_hash: 
+0000f020: 6861 7368 2073 7472 696e 670a 2020 2020  hash string.    
+0000f030: 2020 2020 2020 203a 7479 7065 2073 616d         :type sam
+0000f040: 706c 655f 6861 7368 3a20 7374 720a 2020  ple_hash: str.  
+0000f050: 2020 2020 2020 2020 203a 7265 7475 726e           :return
+0000f060: 3a20 7265 7370 6f6e 7365 0a20 2020 2020  : response.     
+0000f070: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
+0000f080: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
+0000f090: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
+0000f0a0: 2020 2020 2020 2076 616c 6964 6174 655f         validate_
+0000f0b0: 6861 7368 6573 280a 2020 2020 2020 2020  hashes(.        
+0000f0c0: 2020 2020 6861 7368 5f69 6e70 7574 3d5b      hash_input=[
+0000f0d0: 7361 6d70 6c65 5f68 6173 685d 2c0a 2020  sample_hash],.  
+0000f0e0: 2020 2020 2020 2020 2020 616c 6c6f 7765            allowe
+0000f0f0: 645f 6861 7368 5f74 7970 6573 3d28 4d44  d_hash_types=(MD
+0000f100: 352c 2053 4841 312c 2053 4841 3235 3629  5, SHA1, SHA256)
+0000f110: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000f120: 2020 2020 656e 6470 6f69 6e74 203d 2073      endpoint = s
+0000f130: 656c 662e 5f5f 5441 4753 5f45 4e44 504f  elf.__TAGS_ENDPO
+0000f140: 494e 542e 666f 726d 6174 280a 2020 2020  INT.format(.    
+0000f150: 2020 2020 2020 2020 6861 7368 5f76 616c          hash_val
+0000f160: 7565 3d73 616d 706c 655f 6861 7368 0a20  ue=sample_hash. 
+0000f170: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000f180: 2020 7572 6c20 3d20 7365 6c66 2e5f 7572    url = self._ur
+0000f190: 6c2e 666f 726d 6174 2865 6e64 706f 696e  l.format(endpoin
+0000f1a0: 743d 656e 6470 6f69 6e74 290a 0a20 2020  t=endpoint)..   
+0000f1b0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0000f1c0: 7365 6c66 2e5f 5f67 6574 5f72 6571 7565  self.__get_reque
+0000f1d0: 7374 2875 726c 3d75 726c 290a 0a20 2020  st(url=url)..   
+0000f1e0: 2020 2020 2073 656c 662e 5f5f 7261 6973       self.__rais
+0000f1f0: 655f 6f6e 5f65 7272 6f72 2872 6573 706f  e_on_error(respo
+0000f200: 6e73 6529 0a0a 2020 2020 2020 2020 7265  nse)..        re
+0000f210: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+0000f220: 2020 2064 6566 2070 6f73 745f 7573 6572     def post_user
+0000f230: 5f74 6167 7328 7365 6c66 2c20 7361 6d70  _tags(self, samp
+0000f240: 6c65 5f68 6173 682c 2074 6167 7329 3a0a  le_hash, tags):.
+0000f250: 2020 2020 2020 2020 2222 2241 6363 6570          """Accep
+0000f260: 7473 2061 2073 696e 676c 6520 6861 7368  ts a single hash
+0000f270: 2073 7472 696e 6720 616e 6420 6164 6473   string and adds
+0000f280: 206f 6e65 206f 7220 6d6f 7265 2075 7365   one or more use
+0000f290: 7220 7461 6773 2074 6f20 7468 6520 7265  r tags to the re
+0000f2a0: 7175 6573 7465 6420 7361 6d70 6c65 2e0a  quested sample..
+0000f2b0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+0000f2c0: 6d20 7361 6d70 6c65 5f68 6173 683a 2068  m sample_hash: h
+0000f2d0: 6173 6820 7374 7269 6e67 0a20 2020 2020  ash string.     
+0000f2e0: 2020 2020 2020 3a74 7970 6520 7361 6d70        :type samp
+0000f2f0: 6c65 5f68 6173 683a 2073 7472 0a20 2020  le_hash: str.   
+0000f300: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
+0000f310: 6167 733a 206c 6973 7420 6f66 2068 6173  ags: list of has
+0000f320: 6820 7374 7269 6e67 730a 2020 2020 2020  h strings.      
+0000f330: 2020 2020 203a 7479 7065 2074 6167 733a       :type tags:
+0000f340: 206c 6973 745b 7374 725d 0a20 2020 2020   list[str].     
+0000f350: 2020 2020 2020 3a72 6574 7572 6e3a 2072        :return: r
+0000f360: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
+0000f370: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
+0000f380: 7374 732e 5265 7370 6f6e 7365 0a20 2020  sts.Response.   
+0000f390: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f3a0: 2076 616c 6964 6174 655f 6861 7368 6573   validate_hashes
+0000f3b0: 280a 2020 2020 2020 2020 2020 2020 6861  (.            ha
+0000f3c0: 7368 5f69 6e70 7574 3d5b 7361 6d70 6c65  sh_input=[sample
+0000f3d0: 5f68 6173 685d 2c0a 2020 2020 2020 2020  _hash],.        
+0000f3e0: 2020 2020 616c 6c6f 7765 645f 6861 7368      allowed_hash
+0000f3f0: 5f74 7970 6573 3d28 4d44 352c 2053 4841  _types=(MD5, SHA
+0000f400: 312c 2053 4841 3235 3629 0a20 2020 2020  1, SHA256).     
+0000f410: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+0000f420: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+0000f430: 7461 6773 2c20 6c69 7374 293a 0a20 2020  tags, list):.   
+0000f440: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+0000f450: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+0000f460: 7461 6773 2070 6172 616d 6574 6572 206d  tags parameter m
+0000f470: 7573 7420 6265 2061 206c 6973 7420 6f66  ust be a list of
+0000f480: 2073 7472 696e 6773 2e22 290a 0a20 2020   strings.")..   
+0000f490: 2020 2020 2065 6e64 706f 696e 7420 3d20       endpoint = 
+0000f4a0: 7365 6c66 2e5f 5f54 4147 535f 454e 4450  self.__TAGS_ENDP
+0000f4b0: 4f49 4e54 2e66 6f72 6d61 7428 0a20 2020  OINT.format(.   
+0000f4c0: 2020 2020 2020 2020 2068 6173 685f 7661           hash_va
+0000f4d0: 6c75 653d 7361 6d70 6c65 5f68 6173 680a  lue=sample_hash.
+0000f4e0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000f4f0: 2020 2070 6f73 745f 6a73 6f6e 203d 207b     post_json = {
+0000f500: 2274 6167 7322 3a20 7461 6773 7d0a 0a20  "tags": tags}.. 
+0000f510: 2020 2020 2020 2075 726c 203d 2073 656c         url = sel
+0000f520: 662e 5f75 726c 2e66 6f72 6d61 7428 656e  f._url.format(en
+0000f530: 6470 6f69 6e74 3d65 6e64 706f 696e 7429  dpoint=endpoint)
+0000f540: 0a0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
+0000f550: 7365 203d 2073 656c 662e 5f5f 706f 7374  se = self.__post
+0000f560: 5f72 6571 7565 7374 2875 726c 3d75 726c  _request(url=url
+0000f570: 2c20 706f 7374 5f6a 736f 6e3d 706f 7374  , post_json=post
+0000f580: 5f6a 736f 6e29 0a0a 2020 2020 2020 2020  _json)..        
+0000f590: 7365 6c66 2e5f 5f72 6169 7365 5f6f 6e5f  self.__raise_on_
+0000f5a0: 6572 726f 7228 7265 7370 6f6e 7365 290a  error(response).
+0000f5b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f5c0: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
+0000f5d0: 6620 6465 6c65 7465 5f75 7365 725f 7461  f delete_user_ta
+0000f5e0: 6773 2873 656c 662c 2073 616d 706c 655f  gs(self, sample_
+0000f5f0: 6861 7368 2c20 7461 6773 293a 0a20 2020  hash, tags):.   
+0000f600: 2020 2020 2022 2222 4163 6365 7074 7320       """Accepts 
+0000f610: 6120 7369 6e67 6c65 2068 6173 6820 7374  a single hash st
+0000f620: 7269 6e67 2061 6e64 2072 656d 6f76 6573  ring and removes
+0000f630: 206f 6e65 206f 7220 6d6f 7265 2075 7365   one or more use
+0000f640: 7220 7461 6773 2066 726f 6d20 7468 6520  r tags from the 
+0000f650: 7265 7175 6573 7465 6420 7361 6d70 6c65  requested sample
+0000f660: 2e0a 2020 2020 2020 2020 2020 203a 7061  ..           :pa
+0000f670: 7261 6d20 7361 6d70 6c65 5f68 6173 683a  ram sample_hash:
+0000f680: 2068 6173 6820 7374 7269 6e67 0a20 2020   hash string.   
+0000f690: 2020 2020 2020 2020 3a74 7970 6520 7361          :type sa
+0000f6a0: 6d70 6c65 5f68 6173 683a 2073 7472 0a20  mple_hash: str. 
+0000f6b0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+0000f6c0: 2074 6167 733a 206c 6973 7420 6f66 2068   tags: list of h
+0000f6d0: 6173 6820 7374 7269 6e67 730a 2020 2020  ash strings.    
+0000f6e0: 2020 2020 2020 203a 7479 7065 2074 6167         :type tag
+0000f6f0: 733a 206c 6973 745b 7374 725d 0a20 2020  s: list[str].   
+0000f700: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+0000f710: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+0000f720: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
+0000f730: 7565 7374 732e 5265 7370 6f6e 7365 0a20  uests.Response. 
+0000f740: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000f750: 2020 2076 616c 6964 6174 655f 6861 7368     validate_hash
+0000f760: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+0000f770: 6861 7368 5f69 6e70 7574 3d5b 7361 6d70  hash_input=[samp
+0000f780: 6c65 5f68 6173 685d 2c0a 2020 2020 2020  le_hash],.      
+0000f790: 2020 2020 2020 616c 6c6f 7765 645f 6861        allowed_ha
+0000f7a0: 7368 5f74 7970 6573 3d28 4d44 352c 2053  sh_types=(MD5, S
+0000f7b0: 4841 312c 2053 4841 3235 3629 0a20 2020  HA1, SHA256).   
+0000f7c0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000f7d0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+0000f7e0: 6528 7461 6773 2c20 6c69 7374 293a 0a20  e(tags, list):. 
+0000f7f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000f800: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
+0000f810: 2822 7461 6773 2070 6172 616d 6574 6572  ("tags parameter
+0000f820: 206d 7573 7420 6265 2061 206c 6973 7420   must be a list 
+0000f830: 6f66 2073 7472 696e 6773 2e22 290a 0a20  of strings.").. 
+0000f840: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
+0000f850: 3d20 7365 6c66 2e5f 5f54 4147 535f 454e  = self.__TAGS_EN
+0000f860: 4450 4f49 4e54 2e66 6f72 6d61 7428 0a20  DPOINT.format(. 
+0000f870: 2020 2020 2020 2020 2020 2068 6173 685f             hash_
+0000f880: 7661 6c75 653d 7361 6d70 6c65 5f68 6173  value=sample_has
+0000f890: 680a 2020 2020 2020 2020 290a 0a20 2020  h.        )..   
+0000f8a0: 2020 2020 2070 6f73 745f 6a73 6f6e 203d       post_json =
+0000f8b0: 207b 2274 6167 7322 3a20 7461 6773 7d0a   {"tags": tags}.
+0000f8c0: 0a20 2020 2020 2020 2075 726c 203d 2073  .        url = s
+0000f8d0: 656c 662e 5f75 726c 2e66 6f72 6d61 7428  elf._url.format(
+0000f8e0: 656e 6470 6f69 6e74 3d65 6e64 706f 696e  endpoint=endpoin
+0000f8f0: 7429 0a0a 2020 2020 2020 2020 7265 7370  t)..        resp
+0000f900: 6f6e 7365 203d 2073 656c 662e 5f5f 6465  onse = self.__de
+0000f910: 6c65 7465 5f72 6571 7565 7374 2875 726c  lete_request(url
+0000f920: 3d75 726c 2c20 706f 7374 5f6a 736f 6e3d  =url, post_json=
+0000f930: 706f 7374 5f6a 736f 6e29 0a0a 2020 2020  post_json)..    
+0000f940: 2020 2020 7365 6c66 2e5f 5f72 6169 7365      self.__raise
+0000f950: 5f6f 6e5f 6572 726f 7228 7265 7370 6f6e  _on_error(respon
+0000f960: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
+0000f970: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+0000f980: 2020 6465 6620 6765 745f 7961 7261 5f72    def get_yara_r
+0000f990: 756c 6573 6574 735f 6f6e 5f74 6865 5f61  ulesets_on_the_a
+0000f9a0: 7070 6c69 616e 6365 5f76 3228 7365 6c66  ppliance_v2(self
+0000f9b0: 2c20 6f77 6e65 725f 7479 7065 3d4e 6f6e  , owner_type=Non
+0000f9c0: 652c 2073 7461 7475 733d 4e6f 6e65 2c20  e, status=None, 
+0000f9d0: 736f 7572 6365 3d4e 6f6e 652c 2070 6167  source=None, pag
+0000f9e0: 653d 4e6f 6e65 2c20 7061 6765 5f73 697a  e=None, page_siz
+0000f9f0: 653d 4e6f 6e65 293a 0a20 2020 2020 2020  e=None):.       
+0000fa00: 2022 2222 5265 7472 6965 7665 7320 6120   """Retrieves a 
+0000fa10: 6c69 7374 206f 6620 5941 5241 2072 756c  list of YARA rul
+0000fa20: 6573 6574 7320 7468 6174 2061 7265 206f  esets that are o
+0000fa30: 6e20 7468 6520 4131 3030 3020 6170 706c  n the A1000 appl
+0000fa40: 6961 6e63 652e 2054 6865 206c 6973 7420  iance. The list 
+0000fa50: 6361 6e20 6265 2066 696c 7465 7265 6420  can be filtered 
+0000fa60: 6279 2073 6576 6572 616c 0a20 2020 2020  by several.     
+0000fa70: 2020 2063 7269 7465 7269 6120 2872 756c     criteria (rul
+0000fa80: 6573 6574 2073 7461 7475 732c 2073 6f75  eset status, sou
+0000fa90: 7263 652c 2061 6e64 206f 776e 6572 2920  rce, and owner) 
+0000faa0: 7573 696e 6720 6f70 7469 6f6e 616c 2070  using optional p
+0000fab0: 6172 616d 6574 6572 732e 0a20 2020 2020  arameters..     
+0000fac0: 2020 2020 2020 203a 7061 7261 6d20 6f77         :param ow
+0000fad0: 6e65 725f 7479 7065 3a20 7375 7070 6f72  ner_type: suppor
+0000fae0: 7465 6420 7661 6c75 6573 3a20 6d79 2028  ted values: my (
+0000faf0: 6465 6661 756c 7420 2d20 6375 7272 656e  default - curren
+0000fb00: 746c 7920 6175 7468 656e 7469 6361 7465  tly authenticate
+0000fb10: 6420 7573 6572 292c 2075 7365 722c 2073  d user), user, s
+0000fb20: 7973 7465 6d2c 2061 6c6c 0a20 2020 2020  ystem, all.     
+0000fb30: 2020 2020 2020 203a 7479 7065 206f 776e         :type own
+0000fb40: 6572 5f74 7970 653a 2073 7472 0a20 2020  er_type: str.   
+0000fb50: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+0000fb60: 7374 6174 7573 3a20 7375 7070 6f72 7465  status: supporte
+0000fb70: 6420 7661 6c75 6573 3a20 616c 6c20 2864  d values: all (d
+0000fb80: 6566 6175 6c74 292c 2065 7272 6f72 2c20  efault), error, 
+0000fb90: 6163 7469 7665 2c20 6469 7361 626c 6564  active, disabled
+0000fba0: 2c20 7065 6e64 696e 672c 2069 6e76 616c  , pending, inval
+0000fbb0: 6964 2c20 6361 7070 6564 0a20 2020 2020  id, capped.     
+0000fbc0: 2020 2020 2020 203a 7479 7065 2073 7461         :type sta
+0000fbd0: 7475 733a 2073 7472 0a20 2020 2020 2020  tus: str.       
+0000fbe0: 2020 2020 203a 7061 7261 6d20 736f 7572       :param sour
+0000fbf0: 6365 3a20 7375 7070 6f72 7465 6420 7661  ce: supported va
+0000fc00: 6c75 6573 3a20 616c 6c20 2864 6566 6175  lues: all (defau
+0000fc10: 6c74 292c 206c 6f63 616c 2c20 636c 6f75  lt), local, clou
+0000fc20: 640a 2020 2020 2020 2020 2020 2020 3a74  d.            :t
+0000fc30: 7970 6520 736f 7572 6365 3a20 7374 720a  ype source: str.
+0000fc40: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+0000fc50: 616d 2070 6167 653a 2077 6865 6e20 7468  am page: when th
+0000fc60: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
+0000fc70: 6f6d 6974 7465 6420 6672 6f6d 2074 6865  omitted from the
+0000fc80: 2072 6571 7565 7374 2c20 616c 6c20 6176   request, all av
+0000fc90: 6169 6c61 626c 6520 7265 7375 6c74 7320  ailable results 
+0000fca0: 6172 6520 7265 7475 726e 6564 2061 7420  are returned at 
+0000fcb0: 6f6e 6365 0a20 2020 2020 2020 2020 2020  once.           
+0000fcc0: 203a 7479 7065 2070 6167 653a 2073 7472   :type page: str
+0000fcd0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+0000fce0: 7261 6d20 7061 6765 5f73 697a 653a 2070  ram page_size: p
+0000fcf0: 6172 616d 6574 6572 2074 6861 7420 636f  arameter that co
+0000fd00: 6e74 726f 6c73 2068 6f77 206d 616e 7920  ntrols how many 
+0000fd10: 7265 7375 6c74 7320 746f 2072 6574 7572  results to retur
+0000fd20: 6e20 7065 7220 7061 6765 2069 6e20 7468  n per page in th
+0000fd30: 6520 7265 7370 6f6e 7365 0a20 2020 2020  e response.     
+0000fd40: 2020 2020 2020 203a 7479 7065 2070 6167         :type pag
+0000fd50: 655f 7369 7a65 3a20 7374 720a 2020 2020  e_size: str.    
+0000fd60: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+0000fd70: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+0000fd80: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
+0000fd90: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
+0000fda0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000fdb0: 2020 2020 7061 7261 6d73 203d 207b 2274      params = {"t
+0000fdc0: 7970 6522 3a20 6f77 6e65 725f 7479 7065  ype": owner_type
+0000fdd0: 2c20 2273 7461 7475 7322 3a20 7374 6174  , "status": stat
+0000fde0: 7573 2c20 2273 6f75 7263 6522 3a20 736f  us, "source": so
+0000fdf0: 7572 6365 2c20 2270 6167 6522 3a20 7061  urce, "page": pa
+0000fe00: 6765 2c20 2270 6167 655f 7369 7a65 223a  ge, "page_size":
+0000fe10: 2070 6167 655f 7369 7a65 7d0a 2020 2020   page_size}.    
+0000fe20: 2020 2020 7061 7261 6d73 5f73 7472 696e      params_strin
+0000fe30: 675f 6172 7261 7920 3d20 5b5d 0a0a 2020  g_array = []..  
+0000fe40: 2020 2020 2020 6966 2062 6f6f 6c28 7061        if bool(pa
+0000fe50: 7261 6d73 5b22 7061 6765 225d 2920 213d  rams["page"]) !=
+0000fe60: 2062 6f6f 6c28 7061 7261 6d73 5b22 7061   bool(params["pa
+0000fe70: 6765 5f73 697a 6522 5d29 3a0a 2020 2020  ge_size"]):.    
+0000fe80: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
+0000fe90: 6f6e 6749 6e70 7574 4572 726f 7228 2270  ongInputError("p
+0000fea0: 6167 6520 616e 6420 7061 6765 5f73 697a  age and page_siz
+0000feb0: 6520 7061 7261 6d65 7465 7320 6d75 7374  e parametes must
+0000fec0: 2062 6520 7573 6564 2074 6f67 6574 6865   be used togethe
+0000fed0: 7222 290a 0a20 2020 2020 2020 2066 6f72  r")..        for
+0000fee0: 206b 6579 2c20 7661 6c20 696e 2070 6172   key, val in par
+0000fef0: 616d 732e 6974 656d 7328 293a 0a20 2020  ams.items():.   
+0000ff00: 2020 2020 2020 2020 2069 6620 7661 6c3a           if val:
+0000ff10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ff20: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0000ff30: 6365 2876 616c 2c20 7374 7229 3a0a 2020  ce(val, str):.  
+0000ff40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff50: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+0000ff60: 7574 4572 726f 7228 227b 6b65 797d 2070  utError("{key} p
+0000ff70: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+0000ff80: 2061 2073 7472 696e 6722 2e66 6f72 6d61   a string".forma
+0000ff90: 7428 6b65 793d 6b65 7929 290a 2020 2020  t(key=key)).    
+0000ffa0: 2020 2020 2020 2020 2020 2020 7061 7261              para
+0000ffb0: 6d73 5f73 7472 696e 675f 6172 7261 792e  ms_string_array.
+0000ffc0: 6170 7065 6e64 2822 7b6b 6579 7d3d 7b76  append("{key}={v
+0000ffd0: 616c 7d22 2e66 6f72 6d61 7428 6b65 793d  al}".format(key=
+0000ffe0: 6b65 792c 2076 616c 3d76 616c 2929 0a0a  key, val=val))..
+0000fff0: 2020 2020 2020 2020 6966 206c 656e 2870          if len(p
+00010000: 6172 616d 735f 7374 7269 6e67 5f61 7272  arams_string_arr
+00010010: 6179 2920 3e20 303a 0a20 2020 2020 2020  ay) > 0:.       
+00010020: 2020 2020 2071 7565 7279 5f73 7472 696e       query_strin
+00010030: 6720 3d20 2226 222e 6a6f 696e 2870 6172  g = "&".join(par
+00010040: 616d 735f 7374 7269 6e67 5f61 7272 6179  ams_string_array
+00010050: 290a 2020 2020 2020 2020 2020 2020 656e  ).            en
+00010060: 6470 6f69 6e74 203d 2022 7b65 6e64 706f  dpoint = "{endpo
+00010070: 696e 747d 3f7b 7175 6572 795f 7374 7269  int}?{query_stri
+00010080: 6e67 7d22 2e66 6f72 6d61 7428 656e 6470  ng}".format(endp
+00010090: 6f69 6e74 3d73 656c 662e 5f5f 5245 5452  oint=self.__RETR
+000100a0: 4945 5645 5f59 4152 415f 5255 4c45 5345  IEVE_YARA_RULESE
+000100b0: 5453 5f45 4e44 504f 494e 545f 5632 2c0a  TS_ENDPOINT_V2,.
+000100c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100f0: 2020 2020 2020 2020 2020 7175 6572 795f            query_
+00010100: 7374 7269 6e67 3d71 7565 7279 5f73 7472  string=query_str
+00010110: 696e 6729 0a20 2020 2020 2020 2065 6c73  ing).        els
+00010120: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
+00010130: 6e64 706f 696e 7420 3d20 7365 6c66 2e5f  ndpoint = self._
+00010140: 5f52 4554 5249 4556 455f 5941 5241 5f52  _RETRIEVE_YARA_R
+00010150: 554c 4553 4554 535f 454e 4450 4f49 4e54  ULESETS_ENDPOINT
+00010160: 5f56 320a 0a20 2020 2020 2020 2075 726c  _V2..        url
+00010170: 203d 2073 656c 662e 5f75 726c 2e66 6f72   = self._url.for
+00010180: 6d61 7428 656e 6470 6f69 6e74 3d65 6e64  mat(endpoint=end
+00010190: 706f 696e 7429 0a0a 2020 2020 2020 2020  point)..        
+000101a0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+000101b0: 5f5f 6765 745f 7265 7175 6573 7428 7572  __get_request(ur
+000101c0: 6c3d 7572 6c29 0a0a 2020 2020 2020 2020  l=url)..        
+000101d0: 7365 6c66 2e5f 5f72 6169 7365 5f6f 6e5f  self.__raise_on_
+000101e0: 6572 726f 7228 7265 7370 6f6e 7365 290a  error(response).
+000101f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010200: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
+00010210: 6620 6765 745f 7961 7261 5f72 756c 6573  f get_yara_rules
+00010220: 6574 5f63 6f6e 7465 6e74 7328 7365 6c66  et_contents(self
+00010230: 2c20 7275 6c65 7365 745f 6e61 6d65 293a  , ruleset_name):
+00010240: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010250: 2020 2020 2052 6574 7269 6576 6573 2074       Retrieves t
+00010260: 6865 2066 756c 6c20 636f 6e74 656e 7473  he full contents
+00010270: 206f 6620 7468 6520 7265 7175 6573 7465   of the requeste
+00010280: 6420 7275 6c65 7365 7420 696e 2072 6177  d ruleset in raw
+00010290: 2074 6578 742f 706c 6169 6e20 666f 726d   text/plain form
+000102a0: 6174 2e20 416c 6c20 7275 6c65 7365 7473  at. All rulesets
+000102b0: 2063 616e 2062 6520 7265 7472 6965 7665   can be retrieve
+000102c0: 642c 0a20 2020 2020 2020 2072 6567 6172  d,.        regar
+000102d0: 646c 6573 7320 6f66 2074 6865 6972 2063  dless of their c
+000102e0: 7572 7265 6e74 2073 7461 7475 7320 6f6e  urrent status on
+000102f0: 2074 6865 2061 7070 6c69 616e 6365 2028   the appliance (
+00010300: 656e 6162 6c65 642c 2064 6973 6162 6c65  enabled, disable
+00010310: 64e2 80a6 290a 2020 2020 2020 2020 2020  d...).          
+00010320: 2020 3a70 6172 616d 2072 756c 6573 6574    :param ruleset
+00010330: 5f6e 616d 653a 206e 616d 6520 6f66 2074  _name: name of t
+00010340: 6865 2059 4152 4120 7275 6c65 7365 7420  he YARA ruleset 
+00010350: 746f 2072 6574 7269 6576 652e 2052 756c  to retrieve. Rul
+00010360: 6573 6574 206e 616d 6573 2061 7265 2063  eset names are c
+00010370: 6173 652d 7365 6e73 6974 6976 650a 2020  ase-sensitive.  
+00010380: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00010390: 7275 6c65 7365 745f 6e61 6d65 3a20 7374  ruleset_name: st
+000103a0: 720a 2020 2020 2020 2020 2020 2020 3a72  r.            :r
+000103b0: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
+000103c0: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
+000103d0: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
+000103e0: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
+000103f0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+00010400: 7420 6973 696e 7374 616e 6365 2872 756c  t isinstance(rul
+00010410: 6573 6574 5f6e 616d 652c 2073 7472 293a  eset_name, str):
+00010420: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00010430: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
+00010440: 6f72 2822 7275 6c65 7365 745f 6e61 6d65  or("ruleset_name
+00010450: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
+00010460: 6265 2061 2073 7472 696e 6722 290a 0a20  be a string").. 
+00010470: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
+00010480: 3d20 7365 6c66 2e5f 5f52 4554 5249 4556  = self.__RETRIEV
+00010490: 455f 5941 5241 5f52 554c 4553 4554 5f43  E_YARA_RULESET_C
+000104a0: 4f4e 5445 4e54 535f 454e 4450 4f49 4e54  ONTENTS_ENDPOINT
+000104b0: 2e66 6f72 6d61 7428 7275 6c65 7365 745f  .format(ruleset_
+000104c0: 6e61 6d65 3d72 756c 6573 6574 5f6e 616d  name=ruleset_nam
+000104d0: 6529 0a0a 2020 2020 2020 2020 7572 6c20  e)..        url 
+000104e0: 3d20 7365 6c66 2e5f 7572 6c2e 666f 726d  = self._url.form
+000104f0: 6174 2865 6e64 706f 696e 743d 656e 6470  at(endpoint=endp
+00010500: 6f69 6e74 290a 0a20 2020 2020 2020 2072  oint)..        r
+00010510: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+00010520: 5f67 6574 5f72 6571 7565 7374 2875 726c  _get_request(url
+00010530: 3d75 726c 290a 0a20 2020 2020 2020 2073  =url)..        s
+00010540: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
+00010550: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
+00010560: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00010570: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
+00010580: 2067 6574 5f79 6172 615f 7275 6c65 7365   get_yara_rulese
+00010590: 745f 6d61 7463 6865 735f 7632 2873 656c  t_matches_v2(sel
+000105a0: 662c 2072 756c 6573 6574 5f6e 616d 652c  f, ruleset_name,
+000105b0: 2070 6167 653d 4e6f 6e65 2c20 7061 6765   page=None, page
+000105c0: 5f73 697a 653d 4e6f 6e65 293a 0a20 2020  _size=None):.   
+000105d0: 2020 2020 2022 2222 5265 7472 6965 7665       """Retrieve
+000105e0: 7320 7468 6520 6c69 7374 206f 6620 5941  s the list of YA
+000105f0: 5241 206d 6174 6368 6573 2028 626f 7468  RA matches (both
+00010600: 206c 6f63 616c 2061 6e64 2063 6c6f 7564   local and cloud
+00010610: 2920 666f 7220 7265 7175 6573 7465 6420  ) for requested 
+00010620: 7275 6c65 7365 7473 2e20 4966 206d 756c  rulesets. If mul
+00010630: 7469 706c 6520 7275 6c65 7365 7473 2061  tiple rulesets a
+00010640: 7265 0a20 2020 2020 2020 2070 726f 7669  re.        provi
+00010650: 6465 6420 696e 2074 6865 2072 6571 7565  ded in the reque
+00010660: 7374 2c20 6f6e 6c79 2074 6865 2073 616d  st, only the sam
+00010670: 706c 6573 2074 6861 7420 6d61 7463 6820  ples that match 
+00010680: 616c 6c20 7265 7175 6573 7465 6420 7275  all requested ru
+00010690: 6c65 7365 7473 2061 7265 206c 6973 7465  lesets are liste
+000106a0: 6420 696e 2074 6865 2072 6573 706f 6e73  d in the respons
+000106b0: 652e 0a20 2020 2020 2020 2020 2020 203a  e..            :
+000106c0: 7061 7261 6d20 7275 6c65 7365 745f 6e61  param ruleset_na
+000106d0: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+000106e0: 3a74 7970 6520 7275 6c65 7365 745f 6e61  :type ruleset_na
+000106f0: 6d65 3a20 7374 720a 2020 2020 2020 2020  me: str.        
+00010700: 2020 2020 3a70 6172 616d 2070 6167 653a      :param page:
+00010710: 2077 6865 6e20 7468 6973 2070 6172 616d   when this param
+00010720: 6574 6572 2069 7320 6f6d 6974 7465 6420  eter is omitted 
+00010730: 6672 6f6d 2074 6865 2072 6571 7565 7374  from the request
+00010740: 2c20 616c 6c20 6176 6169 6c61 626c 6520  , all available 
+00010750: 7265 7375 6c74 7320 6172 6520 7265 7475  results are retu
+00010760: 726e 6564 2061 7420 6f6e 6365 0a20 2020  rned at once.   
+00010770: 2020 2020 2020 2020 203a 7479 7065 2070           :type p
+00010780: 6167 653a 2073 7472 0a20 2020 2020 2020  age: str.       
+00010790: 2020 2020 203a 7061 7261 6d20 7061 6765       :param page
+000107a0: 5f73 697a 653a 2070 6172 616d 6574 6572  _size: parameter
+000107b0: 2074 6861 7420 636f 6e74 726f 6c73 2068   that controls h
+000107c0: 6f77 206d 616e 7920 7265 7375 6c74 7320  ow many results 
+000107d0: 746f 2072 6574 7572 6e20 7065 7220 7061  to return per pa
+000107e0: 6765 2069 6e20 7468 6520 7265 7370 6f6e  ge in the respon
+000107f0: 7365 0a20 2020 2020 2020 2020 2020 203a  se.            :
+00010800: 7479 7065 2070 6167 655f 7369 7a65 3a20  type page_size: 
+00010810: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00010820: 3a72 6574 7572 6e3a 2072 6573 706f 6e73  :return: respons
+00010830: 650a 2020 2020 2020 2020 2020 2020 3a72  e.            :r
+00010840: 7479 7065 3a20 7265 7175 6573 7473 2e52  type: requests.R
+00010850: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+00010860: 2022 2222 0a20 2020 2020 2020 2070 6172   """.        par
+00010870: 616d 7320 3d20 7b22 6e61 6d65 223a 2072  ams = {"name": r
+00010880: 756c 6573 6574 5f6e 616d 652c 2022 7061  uleset_name, "pa
+00010890: 6765 223a 2070 6167 652c 2022 7061 6765  ge": page, "page
+000108a0: 5f73 697a 6522 3a20 7061 6765 5f73 697a  _size": page_siz
+000108b0: 657d 0a20 2020 2020 2020 2070 6172 616d  e}.        param
+000108c0: 735f 7374 7269 6e67 5f61 7272 6179 203d  s_string_array =
+000108d0: 205b 5d0a 0a20 2020 2020 2020 2069 6620   []..        if 
+000108e0: 626f 6f6c 2870 6172 616d 735b 2270 6167  bool(params["pag
+000108f0: 6522 5d29 2021 3d20 626f 6f6c 2870 6172  e"]) != bool(par
+00010900: 616d 735b 2270 6167 655f 7369 7a65 225d  ams["page_size"]
+00010910: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00010920: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
+00010930: 7272 6f72 2822 7061 6765 2061 6e64 2070  rror("page and p
+00010940: 6167 655f 7369 7a65 2070 6172 616d 6574  age_size paramet
+00010950: 6573 206d 7573 7420 6265 2075 7365 6420  es must be used 
+00010960: 746f 6765 7468 6572 2229 0a0a 2020 2020  together")..    
+00010970: 2020 2020 666f 7220 6b65 792c 2076 616c      for key, val
+00010980: 2069 6e20 7061 7261 6d73 2e69 7465 6d73   in params.items
+00010990: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000109a0: 6966 2076 616c 3a0a 2020 2020 2020 2020  if val:.        
+000109b0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+000109c0: 7369 6e73 7461 6e63 6528 7661 6c2c 2073  sinstance(val, s
+000109d0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+000109e0: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+000109f0: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+00010a00: 7b6b 6579 7d20 7061 7261 6d65 7465 7220  {key} parameter 
+00010a10: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
+00010a20: 222e 666f 726d 6174 286b 6579 3d6b 6579  ".format(key=key
+00010a30: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00010a40: 2020 2070 6172 616d 735f 7374 7269 6e67     params_string
+00010a50: 5f61 7272 6179 2e61 7070 656e 6428 227b  _array.append("{
+00010a60: 6b65 797d 3d7b 7661 6c7d 222e 666f 726d  key}={val}".form
+00010a70: 6174 286b 6579 3d6b 6579 2c20 7661 6c3d  at(key=key, val=
+00010a80: 7661 6c29 290a 0a20 2020 2020 2020 2071  val))..        q
+00010a90: 7565 7279 5f73 7472 696e 6720 3d20 2226  uery_string = "&
+00010aa0: 222e 6a6f 696e 2870 6172 616d 735f 7374  ".join(params_st
+00010ab0: 7269 6e67 5f61 7272 6179 290a 2020 2020  ring_array).    
+00010ac0: 2020 2020 656e 6470 6f69 6e74 203d 2022      endpoint = "
+00010ad0: 7b65 6e64 706f 696e 747d 3f7b 7175 6572  {endpoint}?{quer
+00010ae0: 795f 7374 7269 6e67 7d22 2e66 6f72 6d61  y_string}".forma
+00010af0: 7428 656e 6470 6f69 6e74 3d73 656c 662e  t(endpoint=self.
+00010b00: 5f5f 5245 5452 4945 5645 5f4d 4154 4348  __RETRIEVE_MATCH
+00010b10: 4553 5f46 4f52 5f41 5f59 4152 415f 5255  ES_FOR_A_YARA_RU
+00010b20: 4c45 5345 545f 454e 4450 4f49 4e54 5f56  LESET_ENDPOINT_V
+00010b30: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b60: 2020 2020 2020 2020 2071 7565 7279 5f73           query_s
+00010b70: 7472 696e 673d 7175 6572 795f 7374 7269  tring=query_stri
+00010b80: 6e67 290a 0a20 2020 2020 2020 2075 726c  ng)..        url
+00010b90: 203d 2073 656c 662e 5f75 726c 2e66 6f72   = self._url.for
+00010ba0: 6d61 7428 656e 6470 6f69 6e74 3d65 6e64  mat(endpoint=end
+00010bb0: 706f 696e 7429 0a0a 2020 2020 2020 2020  point)..        
+00010bc0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00010bd0: 5f5f 6765 745f 7265 7175 6573 7428 7572  __get_request(ur
+00010be0: 6c3d 7572 6c29 0a0a 2020 2020 2020 2020  l=url)..        
+00010bf0: 7365 6c66 2e5f 5f72 6169 7365 5f6f 6e5f  self.__raise_on_
+00010c00: 6572 726f 7228 7265 7370 6f6e 7365 290a  error(response).
+00010c10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010c20: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
+00010c30: 6620 6372 6561 7465 5f6f 725f 7570 6461  f create_or_upda
+00010c40: 7465 5f79 6172 615f 7275 6c65 7365 7428  te_yara_ruleset(
+00010c50: 7365 6c66 2c20 6e61 6d65 2c20 636f 6e74  self, name, cont
+00010c60: 656e 742c 2070 7562 6c69 7368 3d4e 6f6e  ent, publish=Non
+00010c70: 652c 2074 6963 6c6f 7564 3d4e 6f6e 6529  e, ticloud=None)
+00010c80: 3a0a 2020 2020 2020 2020 2222 2243 7265  :.        """Cre
+00010c90: 6174 6573 2061 206e 6577 2059 4152 4120  ates a new YARA 
+00010ca0: 7275 6c65 7365 7420 6966 2069 7420 646f  ruleset if it do
+00010cb0: 6573 6ee2 8099 7420 6578 6973 742e 2049  esn...t exist. I
+00010cc0: 6620 6120 7275 6c65 7365 7420 7769 7468  f a ruleset with
+00010cd0: 2074 6865 2073 7065 6369 6669 6564 206e   the specified n
+00010ce0: 616d 6520 616c 7265 6164 7920 6578 6973  ame already exis
+00010cf0: 7473 2c20 6120 6e65 770a 2020 2020 2020  ts, a new.      
+00010d00: 2020 7265 7669 7369 6f6e 2028 7570 6461    revision (upda
+00010d10: 7465 2920 6f66 2074 6865 2072 756c 6573  te) of the rules
+00010d20: 6574 2069 7320 6372 6561 7465 642e 0a20  et is created.. 
+00010d30: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00010d40: 6d20 6e61 6d65 3a20 6e61 6d65 206f 6620  m name: name of 
+00010d50: 7468 6520 7275 6c65 7365 7420 746f 2063  the ruleset to c
+00010d60: 7265 6174 6520 6f72 2075 7064 6174 650a  reate or update.
+00010d70: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+00010d80: 6520 6e61 6d65 3a20 7374 720a 2020 2020  e name: str.    
+00010d90: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+00010da0: 6f6e 7465 6e74 3a20 636f 6e74 656e 7420  ontent: content 
+00010db0: 6f66 2074 6865 2059 4152 4120 7275 6c65  of the YARA rule
+00010dc0: 7365 7420 746f 2063 7265 6174 6520 6f72  set to create or
+00010dd0: 2075 7064 6174 650a 2020 2020 2020 2020   update.        
+00010de0: 2020 2020 3a74 7970 6520 636f 6e74 656e      :type conten
+00010df0: 743a 2073 7472 0a20 2020 2020 2020 2020  t: str.         
+00010e00: 2020 203a 7061 7261 6d20 7075 626c 6973     :param publis
+00010e10: 683a 2064 6574 6572 6d69 6e65 7320 7768  h: determines wh
+00010e20: 6574 6865 7220 7468 6520 7275 6c65 7365  ether the rulese
+00010e30: 7420 7368 6f75 6c64 2062 6520 7379 6e63  t should be sync
+00010e40: 6872 6f6e 697a 6564 2074 6f20 6f74 6865  hronized to othe
+00010e50: 7220 6170 706c 6961 6e63 6573 2069 6e20  r appliances in 
+00010e60: 7468 6520 7361 6d65 0a20 2020 2020 2020  the same.       
+00010e70: 2020 2020 2043 3130 3030 2063 6c75 7374       C1000 clust
+00010e80: 6572 0a20 2020 2020 2020 2020 2020 203a  er.            :
+00010e90: 7479 7065 2070 7562 6c69 7368 3a20 626f  type publish: bo
+00010ea0: 6f6c 0a20 2020 2020 2020 2020 2020 203a  ol.            :
+00010eb0: 7061 7261 6d20 7469 636c 6f75 643a 2064  param ticloud: d
+00010ec0: 6574 6572 6d69 6e65 7320 7768 6574 6865  etermines whethe
+00010ed0: 7220 7468 6520 7275 6c65 7365 7420 7368  r the ruleset sh
+00010ee0: 6f75 6c64 2062 6520 7379 6e63 6872 6f6e  ould be synchron
+00010ef0: 697a 6564 2077 6974 6820 5469 7461 6e69  ized with Titani
+00010f00: 756d 436c 6f75 6420 6f72 206e 6f74 0a20  umCloud or not. 
+00010f10: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00010f20: 2074 6963 6c6f 7564 3a20 626f 6f6c 0a20   ticloud: bool. 
+00010f30: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
+00010f40: 726e 3a20 7265 7370 6f6e 7365 0a20 2020  rn: response.   
+00010f50: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
+00010f60: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
+00010f70: 7365 3a0a 2020 2020 2020 2020 2222 220a  se:.        """.
+00010f80: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
+00010f90: 656c 662e 5f5f 6372 6561 7465 5f70 6f73  elf.__create_pos
+00010fa0: 745f 7061 796c 6f61 6428 0a20 2020 2020  t_payload(.     
+00010fb0: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
+00010fc0: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+00010fd0: 6e74 656e 743d 636f 6e74 656e 742c 0a20  ntent=content,. 
+00010fe0: 2020 2020 2020 2020 2020 2070 7562 6c69             publi
+00010ff0: 7368 3d70 7562 6c69 7368 2c0a 2020 2020  sh=publish,.    
+00011000: 2020 2020 2020 2020 7469 636c 6f75 643d          ticloud=
+00011010: 7469 636c 6f75 640a 2020 2020 2020 2020  ticloud.        
+00011020: 290a 0a20 2020 2020 2020 2065 6e64 706f  )..        endpo
+00011030: 696e 7420 3d20 7365 6c66 2e5f 5f59 4152  int = self.__YAR
+00011040: 415f 5255 4c45 5345 545f 454e 4450 4f49  A_RULESET_ENDPOI
+00011050: 4e54 0a0a 2020 2020 2020 2020 7572 6c20  NT..        url 
+00011060: 3d20 7365 6c66 2e5f 7572 6c2e 666f 726d  = self._url.form
+00011070: 6174 2865 6e64 706f 696e 743d 656e 6470  at(endpoint=endp
+00011080: 6f69 6e74 290a 0a20 2020 2020 2020 2072  oint)..        r
+00011090: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+000110a0: 5f70 6f73 745f 7265 7175 6573 7428 7572  _post_request(ur
+000110b0: 6c3d 7572 6c2c 2064 6174 613d 6461 7461  l=url, data=data
+000110c0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000110d0: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
+000110e0: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+000110f0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00011100: 6e73 650a 0a20 2020 2064 6566 2064 656c  nse..    def del
+00011110: 6574 655f 7961 7261 5f72 756c 6573 6574  ete_yara_ruleset
+00011120: 2873 656c 662c 206e 616d 652c 2070 7562  (self, name, pub
+00011130: 6c69 7368 3d4e 6f6e 6529 3a0a 2020 2020  lish=None):.    
+00011140: 2020 2020 2222 2244 656c 6574 6573 2074      """Deletes t
+00011150: 6865 2073 7065 6369 6669 6564 2059 4152  he specified YAR
+00011160: 4120 7275 6c65 7365 7420 616e 6420 6974  A ruleset and it
+00011170: 7320 6d61 7463 6865 7320 6672 6f6d 2074  s matches from t
+00011180: 6865 2061 7070 6c69 616e 6365 2e0a 2020  he appliance..  
+00011190: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+000111a0: 206e 616d 653a 206e 616d 6520 6f66 2074   name: name of t
+000111b0: 6865 2072 756c 6573 6574 2074 6f20 6372  he ruleset to cr
+000111c0: 6561 7465 206f 7220 7570 6461 7465 0a20  eate or update. 
+000111d0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+000111e0: 206e 616d 653a 2073 7472 0a20 2020 2020   name: str.     
+000111f0: 2020 2020 2020 203a 7061 7261 6d20 7075         :param pu
+00011200: 626c 6973 683a 2064 6574 6572 6d69 6e65  blish: determine
+00011210: 7320 7768 6574 6865 7220 7468 6520 7275  s whether the ru
+00011220: 6c65 7365 7420 7368 6f75 6c64 2062 6520  leset should be 
+00011230: 7379 6e63 6872 6f6e 697a 6564 2074 6f20  synchronized to 
+00011240: 6f74 6865 7220 6170 706c 6961 6e63 6573  other appliances
+00011250: 2069 6e20 7468 6520 7361 6d65 0a20 2020   in the same.   
+00011260: 2020 2020 2020 2020 2043 3130 3030 2063           C1000 c
+00011270: 6c75 7374 6572 0a20 2020 2020 2020 2020  luster.         
+00011280: 2020 203a 7479 7065 2070 7562 6c69 7368     :type publish
+00011290: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+000112a0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
+000112b0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
+000112c0: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
+000112d0: 732e 5265 7370 6f6e 7365 3a0a 2020 2020  s.Response:.    
+000112e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000112f0: 706f 7374 5f6a 736f 6e20 3d20 7365 6c66  post_json = self
+00011300: 2e5f 5f63 7265 6174 655f 706f 7374 5f70  .__create_post_p
+00011310: 6179 6c6f 6164 280a 2020 2020 2020 2020  ayload(.        
+00011320: 2020 2020 6e61 6d65 3d6e 616d 652c 0a20      name=name,. 
+00011330: 2020 2020 2020 2020 2020 2070 7562 6c69             publi
+00011340: 7368 3d70 7562 6c69 7368 2c0a 0a20 2020  sh=publish,..   
+00011350: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+00011360: 6e64 706f 696e 7420 3d20 7365 6c66 2e5f  ndpoint = self._
+00011370: 5f59 4152 415f 5255 4c45 5345 545f 454e  _YARA_RULESET_EN
+00011380: 4450 4f49 4e54 0a0a 2020 2020 2020 2020  DPOINT..        
+00011390: 7572 6c20 3d20 7365 6c66 2e5f 7572 6c2e  url = self._url.
+000113a0: 666f 726d 6174 2865 6e64 706f 696e 743d  format(endpoint=
+000113b0: 656e 6470 6f69 6e74 290a 0a20 2020 2020  endpoint)..     
+000113c0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+000113d0: 6c66 2e5f 5f64 656c 6574 655f 7265 7175  lf.__delete_requ
+000113e0: 6573 7428 7572 6c3d 7572 6c2c 2070 6f73  est(url=url, pos
+000113f0: 745f 6a73 6f6e 3d70 6f73 745f 6a73 6f6e  t_json=post_json
+00011400: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00011410: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
+00011420: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+00011430: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00011440: 6e73 650a 0a20 2020 2064 6566 2065 6e61  nse..    def ena
+00011450: 626c 655f 6f72 5f64 6973 6162 6c65 5f79  ble_or_disable_y
+00011460: 6172 615f 7275 6c65 7365 7428 7365 6c66  ara_ruleset(self
+00011470: 2c20 656e 6162 6c65 642c 206e 616d 652c  , enabled, name,
+00011480: 2070 7562 6c69 7368 3d4e 6f6e 6529 3a0a   publish=None):.
+00011490: 2020 2020 2020 2020 2222 2245 6e61 626c          """Enabl
+000114a0: 6573 2f64 6973 6162 6c65 7320 7275 6c65  es/disables rule
+000114b0: 7365 7420 6f6e 2074 6865 2061 7070 6c69  set on the appli
+000114c0: 616e 6365 2e20 4164 6d69 6e69 7374 7261  ance. Administra
+000114d0: 746f 7273 2063 616e 206d 616e 6167 6520  tors can manage 
+000114e0: 616e 7920 7275 6c65 7365 7420 7768 696c  any ruleset whil
+000114f0: 6520 7265 6775 6c61 7220 4131 3030 3020  e regular A1000 
+00011500: 7573 6572 730a 2020 2020 2020 2020 6361  users.        ca
+00011510: 6e20 6f6e 6c79 206d 616e 6167 6520 7468  n only manage th
+00011520: 6569 7220 6f77 6e20 7275 6c65 7365 7473  eir own rulesets
+00011530: 2e0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
+00011540: 6172 616d 2065 6e61 626c 6564 3a20 7768  aram enabled: wh
+00011550: 6574 6865 7220 746f 2065 6e61 626c 6520  ether to enable 
+00011560: 2865 6e61 626c 6564 3d54 7275 6529 206f  (enabled=True) o
+00011570: 7220 6469 7361 626c 6520 2865 6e61 626c  r disable (enabl
+00011580: 6564 3d46 616c 7365 2920 7468 6520 7370  ed=False) the sp
+00011590: 6563 6966 6965 6420 7275 6c65 7365 740a  ecified ruleset.
+000115a0: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+000115b0: 6520 656e 6162 6c65 643a 2062 6f6f 6c0a  e enabled: bool.
+000115c0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+000115d0: 616d 206e 616d 653a 206e 616d 6520 6f66  am name: name of
+000115e0: 2074 6865 2072 756c 6573 6574 2074 6f20   the ruleset to 
+000115f0: 656e 6162 6c65 2f64 6973 6162 6c65 0a20  enable/disable. 
+00011600: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00011610: 206e 616d 653a 2073 7472 0a20 2020 2020   name: str.     
+00011620: 2020 2020 2020 203a 7061 7261 6d20 7075         :param pu
+00011630: 626c 6973 683a 2064 6574 6572 6d69 6e65  blish: determine
+00011640: 7320 7768 6574 6865 7220 7468 6520 7275  s whether the ru
+00011650: 6c65 7365 7420 7368 6f75 6c64 2062 6520  leset should be 
+00011660: 7379 6e63 6872 6f6e 697a 6564 2074 6f20  synchronized to 
+00011670: 6f74 6865 7220 6170 706c 6961 6e63 6573  other appliances
+00011680: 2069 6e20 7468 6520 7361 6d65 0a20 2020   in the same.   
+00011690: 2020 2020 2020 2020 2043 3130 3030 2063           C1000 c
+000116a0: 6c75 7374 6572 0a20 2020 2020 2020 2020  luster.         
+000116b0: 2020 203a 7479 7065 2070 7562 6c69 7368     :type publish
+000116c0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+000116d0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
+000116e0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
+000116f0: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
+00011700: 732e 5265 7370 6f6e 7365 3a0a 2020 2020  s.Response:.    
+00011710: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011720: 6461 7461 203d 2073 656c 662e 5f5f 6372  data = self.__cr
+00011730: 6561 7465 5f70 6f73 745f 7061 796c 6f61  eate_post_payloa
+00011740: 6428 0a20 2020 2020 2020 2020 2020 206e  d(.            n
+00011750: 616d 653d 6e61 6d65 2c0a 2020 2020 2020  ame=name,.      
+00011760: 2020 2020 2020 7075 626c 6973 683d 7075        publish=pu
+00011770: 626c 6973 682c 0a20 2020 2020 2020 2029  blish,.        )
+00011780: 0a0a 2020 2020 2020 2020 6966 2065 6e61  ..        if ena
+00011790: 626c 6564 2061 6e64 2065 6e61 626c 6564  bled and enabled
+000117a0: 206e 6f74 2069 6e20 2854 7275 652c 2046   not in (True, F
+000117b0: 616c 7365 293a 0a20 2020 2020 2020 2020  alse):.         
+000117c0: 2020 2072 6169 7365 2057 726f 6e67 496e     raise WrongIn
+000117d0: 7075 7445 7272 6f72 2822 656e 6162 6c65  putError("enable
+000117e0: 6420 7061 7261 6d65 7465 7220 6d75 7374  d parameter must
+000117f0: 2062 6520 626f 6f6c 6561 6e2e 2229 0a0a   be boolean.")..
+00011800: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
+00011810: 203d 2073 656c 662e 5f5f 454e 4142 4c45   = self.__ENABLE
+00011820: 5f4f 525f 4449 5341 424c 455f 5941 5241  _OR_DISABLE_YARA
+00011830: 5f52 554c 4553 4554 5f45 4e44 504f 494e  _RULESET_ENDPOIN
+00011840: 542e 666f 726d 6174 286f 7065 7261 7469  T.format(operati
+00011850: 6f6e 3d22 656e 6162 6c65 2220 6966 2065  on="enable" if e
+00011860: 6e61 626c 6564 2065 6c73 6520 2264 6973  nabled else "dis
+00011870: 6162 6c65 2229 0a0a 2020 2020 2020 2020  able")..        
+00011880: 7572 6c20 3d20 7365 6c66 2e5f 7572 6c2e  url = self._url.
+00011890: 666f 726d 6174 2865 6e64 706f 696e 743d  format(endpoint=
+000118a0: 656e 6470 6f69 6e74 290a 0a20 2020 2020  endpoint)..     
+000118b0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+000118c0: 6c66 2e5f 5f70 6f73 745f 7265 7175 6573  lf.__post_reques
+000118d0: 7428 7572 6c3d 7572 6c2c 2064 6174 613d  t(url=url, data=
+000118e0: 6461 7461 290a 0a20 2020 2020 2020 2073  data)..        s
+000118f0: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
+00011900: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
+00011910: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00011920: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
+00011930: 2067 6574 5f79 6172 615f 7275 6c65 7365   get_yara_rulese
+00011940: 745f 7379 6e63 6872 6f6e 697a 6174 696f  t_synchronizatio
+00011950: 6e5f 7469 6d65 2873 656c 6629 3a0a 2020  n_time(self):.  
+00011960: 2020 2020 2020 2222 2247 6574 7320 696e        """Gets in
+00011970: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+00011980: 7468 6520 6375 7272 656e 7420 7379 6e63  the current sync
+00011990: 6872 6f6e 697a 6174 696f 6e20 7374 6174  hronization stat
+000119a0: 7573 2066 6f72 2054 6974 616e 6975 6d43  us for TitaniumC
+000119b0: 6c6f 7564 2d65 6e61 626c 6564 2072 756c  loud-enabled rul
+000119c0: 6573 6574 732e 0a20 2020 2020 2020 2020  esets..         
+000119d0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
+000119e0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
+000119f0: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
+00011a00: 732e 5265 7370 6f6e 7365 3a0a 2020 2020  s.Response:.    
+00011a10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011a20: 656e 6470 6f69 6e74 203d 2073 656c 662e  endpoint = self.
+00011a30: 5f5f 4745 545f 4f52 5f53 4554 5f59 4152  __GET_OR_SET_YAR
+00011a40: 415f 5255 4c45 5345 545f 5359 4e43 4852  A_RULESET_SYNCHR
+00011a50: 4f4e 495a 4154 494f 4e5f 5449 4d45 5f45  ONIZATION_TIME_E
+00011a60: 4e44 504f 494e 540a 0a20 2020 2020 2020  NDPOINT..       
+00011a70: 2075 726c 203d 2073 656c 662e 5f75 726c   url = self._url
+00011a80: 2e66 6f72 6d61 7428 656e 6470 6f69 6e74  .format(endpoint
+00011a90: 3d65 6e64 706f 696e 7429 0a0a 2020 2020  =endpoint)..    
+00011aa0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+00011ab0: 656c 662e 5f5f 6765 745f 7265 7175 6573  elf.__get_reques
+00011ac0: 7428 7572 6c3d 7572 6c29 0a0a 2020 2020  t(url=url)..    
+00011ad0: 2020 2020 7365 6c66 2e5f 5f72 6169 7365      self.__raise
+00011ae0: 5f6f 6e5f 6572 726f 7228 7265 7370 6f6e  _on_error(respon
+00011af0: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
+00011b00: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+00011b10: 2020 6465 6620 7570 6461 7465 5f79 6172    def update_yar
+00011b20: 615f 7275 6c65 7365 745f 7379 6e63 6872  a_ruleset_synchr
+00011b30: 6f6e 697a 6174 696f 6e5f 7469 6d65 2873  onization_time(s
+00011b40: 656c 662c 2073 796e 635f 7469 6d65 293a  elf, sync_time):
+00011b50: 0a20 2020 2020 2020 2022 2222 5570 6461  .        """Upda
+00011b60: 7465 7320 7468 6520 5469 7461 6e69 756d  tes the Titanium
+00011b70: 436c 6f75 6420 7379 6e63 6872 6f6e 697a  Cloud synchroniz
+00011b80: 6174 696f 6e20 7469 6d65 2066 6f72 2054  ation time for T
+00011b90: 6974 616e 6975 6d43 6c6f 7564 2d65 6e61  itaniumCloud-ena
+00011ba0: 626c 6564 2059 4152 4120 7275 6c65 7365  bled YARA rulese
+00011bb0: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+00011bc0: 3a70 6172 616d 2073 796e 635f 7469 6d65  :param sync_time
+00011bd0: 3a20 666f 726d 6174 2073 686f 756c 6420  : format should 
+00011be0: 6265 2055 5443 2028 5959 5959 2d4d 4d2d  be UTC (YYYY-MM-
+00011bf0: 4444 2068 683a 6d6d 290a 2020 2020 2020  DD hh:mm).      
+00011c00: 2020 2020 2020 3a74 7970 6520 7379 6e63        :type sync
+00011c10: 5f74 696d 653a 2073 7472 0a20 2020 2020  _time: str.     
+00011c20: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00011c30: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+00011c40: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
+00011c50: 7565 7374 732e 5265 7370 6f6e 7365 3a0a  uests.Response:.
+00011c60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011c70: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00011c80: 2020 2020 2064 6174 6574 696d 652e 6461       datetime.da
+00011c90: 7465 7469 6d65 2e73 7472 7074 696d 6528  tetime.strptime(
+00011ca0: 7379 6e63 5f74 696d 652c 2027 2559 2d25  sync_time, '%Y-%
+00011cb0: 6d2d 2564 2025 483a 254d 2729 0a20 2020  m-%d %H:%M').   
+00011cc0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+00011cd0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00011ce0: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
+00011cf0: 6e70 7574 4572 726f 7228 2249 6e63 6f72  nputError("Incor
+00011d00: 7265 6374 2073 796e 635f 7469 6d65 2066  rect sync_time f
+00011d10: 6f72 6d61 742c 2073 686f 756c 6420 6265  ormat, should be
+00011d20: 2059 5959 592d 4d4d 2d44 4420 6868 3a6d   YYYY-MM-DD hh:m
+00011d30: 6d22 290a 0a20 2020 2020 2020 2065 6e64  m")..        end
+00011d40: 706f 696e 7420 3d20 7365 6c66 2e5f 5f47  point = self.__G
+00011d50: 4554 5f4f 525f 5345 545f 5941 5241 5f52  ET_OR_SET_YARA_R
+00011d60: 554c 4553 4554 5f53 594e 4348 524f 4e49  ULESET_SYNCHRONI
+00011d70: 5a41 5449 4f4e 5f54 494d 455f 454e 4450  ZATION_TIME_ENDP
+00011d80: 4f49 4e54 0a0a 2020 2020 2020 2020 7572  OINT..        ur
+00011d90: 6c20 3d20 7365 6c66 2e5f 7572 6c2e 666f  l = self._url.fo
+00011da0: 726d 6174 2865 6e64 706f 696e 743d 656e  rmat(endpoint=en
+00011db0: 6470 6f69 6e74 290a 0a20 2020 2020 2020  dpoint)..       
+00011dc0: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
+00011dd0: 2e5f 5f70 6f73 745f 7265 7175 6573 7428  .__post_request(
+00011de0: 7572 6c3d 7572 6c2c 2064 6174 613d 7b22  url=url, data={"
+00011df0: 7469 6d65 223a 2073 796e 635f 7469 6d65  time": sync_time
+00011e00: 7d29 0a0a 2020 2020 2020 2020 7365 6c66  })..        self
+00011e10: 2e5f 5f72 6169 7365 5f6f 6e5f 6572 726f  .__raise_on_erro
+00011e20: 7228 7265 7370 6f6e 7365 290a 0a20 2020  r(response)..   
+00011e30: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+00011e40: 6f6e 7365 0a0a 2020 2020 6465 6620 7374  onse..    def st
+00011e50: 6172 745f 6f72 5f73 746f 705f 7961 7261  art_or_stop_yara
+00011e60: 5f6c 6f63 616c 5f72 6574 726f 5f73 6361  _local_retro_sca
+00011e70: 6e28 7365 6c66 2c20 6f70 6572 6174 696f  n(self, operatio
+00011e80: 6e29 3a0a 2020 2020 2020 2020 2222 2241  n):.        """A
+00011e90: 6c6c 6f77 7320 7573 6572 7320 746f 2069  llows users to i
+00011ea0: 6e69 7469 6174 6520 7468 6520 4c6f 6361  nitiate the Loca
+00011eb0: 6c20 5265 7472 6f20 7363 616e 206f 6e20  l Retro scan on 
+00011ec0: 7468 6520 4131 3030 3020 6170 706c 6961  the A1000 applia
+00011ed0: 6e63 652c 2061 6e64 2073 746f 7020 7468  nce, and stop th
+00011ee0: 6520 4c6f 6361 6c20 5265 7472 6f20 7363  e Local Retro sc
+00011ef0: 616e 2074 6861 7420 6973 0a20 2020 2020  an that is.     
+00011f00: 2020 2069 6e20 7072 6f67 7265 7373 206f     in progress o
+00011f10: 6e20 7468 6520 6170 706c 6961 6e63 652e  n the appliance.
+00011f20: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+00011f30: 7261 6d20 6f70 6572 6174 696f 6e3a 2061  ram operation: a
+00011f40: 6363 6570 7465 6420 7661 6c75 6573 3a20  ccepted values: 
+00011f50: 5354 4152 542c 2053 544f 5020 2863 6173  START, STOP (cas
+00011f60: 652d 7365 6e73 6974 6976 6529 0a20 2020  e-sensitive).   
+00011f70: 2020 2020 2020 2020 203a 7479 7065 206f           :type o
+00011f80: 7065 7261 7469 6f6e 3a20 7374 720a 2020  peration: str.  
+00011f90: 2020 2020 2020 2020 2020 3a72 6574 7572            :retur
+00011fa0: 6e3a 2072 6573 706f 6e73 650a 2020 2020  n: response.    
+00011fb0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00011fc0: 7265 7175 6573 7473 2e52 6573 706f 6e73  requests.Respons
+00011fd0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00011fe0: 2020 2020 2020 2069 6620 6f70 6572 6174         if operat
+00011ff0: 696f 6e20 6e6f 7420 696e 2028 2253 5441  ion not in ("STA
+00012000: 5254 222c 2022 5354 4f50 2229 3a0a 2020  RT", "STOP"):.  
+00012010: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00012020: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
+00012030: 226f 7065 7261 7469 6f6e 2070 6172 616d  "operation param
+00012040: 6574 6572 206d 7573 7420 6265 2065 6974  eter must be eit
+00012050: 6865 7220 2753 5441 5254 2720 6f72 2027  her 'START' or '
+00012060: 5354 4f50 2722 290a 0a20 2020 2020 2020  STOP'")..       
+00012070: 2065 6e64 706f 696e 7420 3d20 7365 6c66   endpoint = self
+00012080: 2e5f 5f59 4152 415f 4c4f 4341 4c5f 5245  .__YARA_LOCAL_RE
+00012090: 5452 4f53 4341 4e5f 454e 4450 4f49 4e54  TROSCAN_ENDPOINT
+000120a0: 0a0a 2020 2020 2020 2020 7572 6c20 3d20  ..        url = 
+000120b0: 7365 6c66 2e5f 7572 6c2e 666f 726d 6174  self._url.format
+000120c0: 2865 6e64 706f 696e 743d 656e 6470 6f69  (endpoint=endpoi
+000120d0: 6e74 290a 0a20 2020 2020 2020 2072 6573  nt)..        res
+000120e0: 706f 6e73 6520 3d20 7365 6c66 2e5f 5f70  ponse = self.__p
+000120f0: 6f73 745f 7265 7175 6573 7428 7572 6c3d  ost_request(url=
+00012100: 7572 6c2c 2064 6174 613d 7b22 6f70 6572  url, data={"oper
+00012110: 6174 696f 6e22 3a20 6f70 6572 6174 696f  ation": operatio
+00012120: 6e7d 290a 0a20 2020 2020 2020 2073 656c  n})..        sel
+00012130: 662e 5f5f 7261 6973 655f 6f6e 5f65 7272  f.__raise_on_err
+00012140: 6f72 2872 6573 706f 6e73 6529 0a0a 2020  or(response)..  
+00012150: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00012160: 706f 6e73 650a 0a20 2020 2064 6566 2067  ponse..    def g
+00012170: 6574 5f79 6172 615f 6c6f 6361 6c5f 7265  et_yara_local_re
+00012180: 7472 6f5f 7363 616e 5f73 7461 7475 7328  tro_scan_status(
+00012190: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000121a0: 2222 416c 6c6f 7773 2075 7365 7273 2074  ""Allows users t
+000121b0: 6f20 6368 6563 6b20 7468 6520 7374 6174  o check the stat
+000121c0: 7573 206f 6620 4c6f 6361 6c20 5265 7472  us of Local Retr
+000121d0: 6f20 6f6e 2074 6865 2041 3130 3030 2061  o on the A1000 a
+000121e0: 7070 6c69 616e 6365 2e20 5468 6520 7265  ppliance. The re
+000121f0: 7370 6f6e 7365 2069 6e64 6963 6174 6573  sponse indicates
+00012200: 2074 6865 2063 7572 7265 6e74 0a20 2020   the current.   
+00012210: 2020 2020 2073 7461 7465 206f 6620 4c6f       state of Lo
+00012220: 6361 6c20 5265 7472 6f2c 2074 696d 6520  cal Retro, time 
+00012230: 616e 6420 6461 7465 2077 6865 6e20 7468  and date when th
+00012240: 6520 6c61 7465 7374 204c 6f63 616c 2052  e latest Local R
+00012250: 6574 726f 2073 6361 6e20 7761 7320 7374  etro scan was st
+00012260: 6172 7465 6420 616e 642f 6f72 2073 746f  arted and/or sto
+00012270: 7070 6564 2c20 616e 6420 6120 6c69 7374  pped, and a list
+00012280: 206f 660a 2020 2020 2020 2020 7072 6576   of.        prev
+00012290: 696f 7573 204c 6f63 616c 2052 6574 726f  ious Local Retro
+000122a0: 2073 6361 6e73 2077 6974 6820 7468 6520   scans with the 
+000122b0: 7361 6d65 2064 6574 6169 6c73 2e0a 2020  same details..  
+000122c0: 2020 2020 2020 2020 2020 3a72 6574 7572            :retur
+000122d0: 6e3a 2072 6573 706f 6e73 650a 2020 2020  n: response.    
+000122e0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000122f0: 7265 7175 6573 7473 2e52 6573 706f 6e73  requests.Respons
+00012300: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00012310: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
+00012320: 3d20 7365 6c66 2e5f 5f59 4152 415f 4c4f  = self.__YARA_LO
+00012330: 4341 4c5f 5245 5452 4f53 4341 4e5f 454e  CAL_RETROSCAN_EN
+00012340: 4450 4f49 4e54 0a0a 2020 2020 2020 2020  DPOINT..        
+00012350: 7572 6c20 3d20 7365 6c66 2e5f 7572 6c2e  url = self._url.
+00012360: 666f 726d 6174 2865 6e64 706f 696e 743d  format(endpoint=
+00012370: 656e 6470 6f69 6e74 290a 0a20 2020 2020  endpoint)..     
+00012380: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+00012390: 6c66 2e5f 5f67 6574 5f72 6571 7565 7374  lf.__get_request
+000123a0: 2875 726c 3d75 726c 290a 0a20 2020 2020  (url=url)..     
+000123b0: 2020 2073 656c 662e 5f5f 7261 6973 655f     self.__raise_
+000123c0: 6f6e 5f65 7272 6f72 2872 6573 706f 6e73  on_error(respons
+000123d0: 6529 0a0a 2020 2020 2020 2020 7265 7475  e)..        retu
+000123e0: 726e 2072 6573 706f 6e73 650a 0a20 2020  rn response..   
+000123f0: 2064 6566 2073 7461 7274 5f6f 725f 7374   def start_or_st
+00012400: 6f70 5f79 6172 615f 636c 6f75 645f 7265  op_yara_cloud_re
+00012410: 7472 6f5f 7363 616e 2873 656c 662c 206f  tro_scan(self, o
+00012420: 7065 7261 7469 6f6e 2c20 7275 6c65 7365  peration, rulese
+00012430: 745f 6e61 6d65 293a 0a20 2020 2020 2020  t_name):.       
+00012440: 2022 2222 416c 6c6f 7773 2075 7365 7273   """Allows users
+00012450: 2074 6f20 7374 6172 7420 616e 6420 7374   to start and st
+00012460: 6f70 2061 2043 6c6f 7564 2052 6574 726f  op a Cloud Retro
+00012470: 2073 6361 6e20 666f 7220 6120 7370 6563   scan for a spec
+00012480: 6966 6965 6420 7275 6c65 7365 7420 6f6e  ified ruleset on
+00012490: 2074 6865 2041 3130 3030 2061 7070 6c69   the A1000 appli
+000124a0: 616e 6365 2c20 6173 2077 656c 6c20 6173  ance, as well as
+000124b0: 0a20 2020 2020 2020 2074 6f20 636c 6561  .        to clea
+000124c0: 7220 616c 6c20 436c 6f75 6420 5265 7472  r all Cloud Retr
+000124d0: 6f20 7265 7375 6c74 7320 666f 7220 7468  o results for th
+000124e0: 6520 7275 6c65 7365 742e 0a20 2020 2020  e ruleset..     
+000124f0: 2020 2020 2020 203a 7061 7261 6d20 6f70         :param op
+00012500: 6572 6174 696f 6e3a 2061 6363 6570 7465  eration: accepte
+00012510: 6420 7661 6c75 6573 3a20 5354 4152 542c  d values: START,
+00012520: 2053 544f 502c 2043 4c45 4152 2028 6361   STOP, CLEAR (ca
+00012530: 7365 2d73 656e 7369 7469 7665 290a 2020  se-sensitive).  
+00012540: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00012550: 6f70 6572 6174 696f 6e3a 2073 7472 0a20  operation: str. 
+00012560: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00012570: 6d20 7275 6c65 7365 745f 6e61 6d65 3a20  m ruleset_name: 
+00012580: 6e61 6d65 206f 6620 7468 6520 5941 5241  name of the YARA
+00012590: 2072 756c 6573 6574 2074 6861 7420 7468   ruleset that th
+000125a0: 6520 436c 6f75 6420 5265 7472 6f20 7363  e Cloud Retro sc
+000125b0: 616e 2073 686f 756c 6420 6265 2072 756e  an should be run
+000125c0: 206f 6e0a 2020 2020 2020 2020 2020 2020   on.            
+000125d0: 3a74 7970 6520 7275 6c65 7365 745f 6e61  :type ruleset_na
+000125e0: 6d65 3a20 7374 720a 2020 2020 2020 2020  me: str.        
+000125f0: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
+00012600: 706f 6e73 650a 2020 2020 2020 2020 2020  ponse.          
+00012610: 2020 3a72 7479 7065 3a20 7265 7175 6573    :rtype: reques
+00012620: 7473 2e52 6573 706f 6e73 650a 2020 2020  ts.Response.    
+00012630: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012640: 6966 206f 7065 7261 7469 6f6e 206e 6f74  if operation not
+00012650: 2069 6e20 2822 5354 4152 5422 2c20 2253   in ("START", "S
+00012660: 544f 5022 2c20 2243 4c45 4152 2229 3a0a  TOP", "CLEAR"):.
+00012670: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00012680: 6520 5772 6f6e 6749 6e70 7574 4572 726f  e WrongInputErro
+00012690: 7228 226f 7065 7261 7469 6f6e 2070 6172  r("operation par
+000126a0: 616d 6574 6572 206d 7573 7420 6265 2065  ameter must be e
+000126b0: 6974 6865 7220 2753 5441 5254 272c 2027  ither 'START', '
+000126c0: 5354 4f50 2720 6f72 2027 434c 4541 5227  STOP' or 'CLEAR'
+000126d0: 2229 0a0a 2020 2020 2020 2020 6966 206e  ")..        if n
+000126e0: 6f74 2069 7369 6e73 7461 6e63 6528 7275  ot isinstance(ru
+000126f0: 6c65 7365 745f 6e61 6d65 2c20 7374 7229  leset_name, str)
+00012700: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00012710: 6973 6520 5772 6f6e 6749 6e70 7574 4572  ise WrongInputEr
+00012720: 726f 7228 2272 756c 6573 6574 5f6e 616d  ror("ruleset_nam
+00012730: 6520 7061 7261 6d65 7465 7220 6d75 7374  e parameter must
+00012740: 2062 6520 6120 7374 7269 6e67 2229 0a0a   be a string")..
+00012750: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
+00012760: 203d 2073 656c 662e 5f5f 5941 5241 5f43   = self.__YARA_C
+00012770: 4c4f 5544 5f52 4554 524f 5343 414e 535f  LOUD_RETROSCANS_
+00012780: 454e 4450 4f49 4e54 2e66 6f72 6d61 7428  ENDPOINT.format(
+00012790: 7275 6c65 7365 745f 6e61 6d65 3d72 756c  ruleset_name=rul
+000127a0: 6573 6574 5f6e 616d 6529 0a0a 2020 2020  eset_name)..    
+000127b0: 2020 2020 7572 6c20 3d20 7365 6c66 2e5f      url = self._
+000127c0: 7572 6c2e 666f 726d 6174 2865 6e64 706f  url.format(endpo
+000127d0: 696e 743d 656e 6470 6f69 6e74 290a 0a20  int=endpoint).. 
+000127e0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+000127f0: 3d20 7365 6c66 2e5f 5f70 6f73 745f 7265  = self.__post_re
+00012800: 7175 6573 7428 7572 6c3d 7572 6c2c 2064  quest(url=url, d
+00012810: 6174 613d 7b22 6f70 6572 6174 696f 6e22  ata={"operation"
+00012820: 3a20 6f70 6572 6174 696f 6e7d 290a 0a20  : operation}).. 
+00012830: 2020 2020 2020 2073 656c 662e 5f5f 7261         self.__ra
+00012840: 6973 655f 6f6e 5f65 7272 6f72 2872 6573  ise_on_error(res
+00012850: 706f 6e73 6529 0a0a 2020 2020 2020 2020  ponse)..        
+00012860: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
+00012870: 0a20 2020 2064 6566 2067 6574 5f79 6172  .    def get_yar
+00012880: 615f 636c 6f75 645f 7265 7472 6f5f 7363  a_cloud_retro_sc
+00012890: 616e 5f73 7461 7475 7328 7365 6c66 2c20  an_status(self, 
+000128a0: 7275 6c65 7365 745f 6e61 6d65 293a 0a20  ruleset_name):. 
+000128b0: 2020 2020 2020 2022 2222 416c 6c6f 7773         """Allows
+000128c0: 2075 7365 7273 2074 6f20 6368 6563 6b20   users to check 
+000128d0: 7468 6520 7374 6174 7573 206f 6620 436c  the status of Cl
+000128e0: 6f75 6420 5265 7472 6f20 666f 7220 7468  oud Retro for th
+000128f0: 6520 7370 6563 6966 6965 6420 5941 5241  e specified YARA
+00012900: 2072 756c 6573 6574 2e20 5468 6520 7265   ruleset. The re
+00012910: 7370 6f6e 7365 2069 6e64 6963 6174 6573  sponse indicates
+00012920: 2074 6865 0a20 2020 2020 2020 2063 7572   the.        cur
+00012930: 7265 6e74 2073 7461 7465 206f 6620 436c  rent state of Cl
+00012940: 6f75 6420 5265 7472 6f2c 2074 696d 6520  oud Retro, time 
+00012950: 616e 6420 6461 7465 2077 6865 6e20 7468  and date when th
+00012960: 6520 6c61 7465 7374 2043 6c6f 7564 2052  e latest Cloud R
+00012970: 6574 726f 2073 6361 6e20 7761 7320 7374  etro scan was st
+00012980: 6172 7465 6420 616e 642f 6f72 2073 746f  arted and/or sto
+00012990: 7070 6564 2c20 616e 6420 610a 2020 2020  pped, and a.    
+000129a0: 2020 2020 6c69 7374 206f 6620 7072 6576      list of prev
+000129b0: 696f 7573 2043 6c6f 7564 2052 6574 726f  ious Cloud Retro
+000129c0: 2073 6361 6e73 2077 6974 6820 7468 6520   scans with the 
+000129d0: 7361 6d65 2064 6574 6169 6c73 2e0a 2020  same details..  
+000129e0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+000129f0: 2072 756c 6573 6574 5f6e 616d 653a 206e   ruleset_name: n
+00012a00: 616d 6520 6f66 2074 6865 2059 4152 4120  ame of the YARA 
+00012a10: 7275 6c65 7365 7420 666f 7220 7768 6963  ruleset for whic
+00012a20: 6820 746f 2063 6865 636b 2066 6f72 2074  h to check for t
+00012a30: 6865 2043 6c6f 7564 2052 6574 726f 2073  he Cloud Retro s
+00012a40: 6361 6e20 7374 6174 7573 0a20 2020 2020  can status.     
+00012a50: 2020 2020 2020 203a 7479 7065 2072 756c         :type rul
+00012a60: 6573 6574 5f6e 616d 653a 2073 7472 0a20  eset_name: str. 
+00012a70: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
+00012a80: 726e 3a20 7265 7370 6f6e 7365 0a20 2020  rn: response.   
+00012a90: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
+00012aa0: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
+00012ab0: 7365 0a20 2020 2020 2020 2022 2222 0a20  se.        """. 
+00012ac0: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+00012ad0: 696e 7374 616e 6365 2872 756c 6573 6574  instance(ruleset
+00012ae0: 5f6e 616d 652c 2073 7472 293a 0a20 2020  _name, str):.   
+00012af0: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+00012b00: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+00012b10: 7275 6c65 7365 745f 6e61 6d65 2070 6172  ruleset_name par
+00012b20: 616d 6574 6572 206d 7573 7420 6265 2061  ameter must be a
+00012b30: 2073 7472 696e 6722 290a 0a20 2020 2020   string")..     
+00012b40: 2020 2065 6e64 706f 696e 7420 3d20 7365     endpoint = se
+00012b50: 6c66 2e5f 5f59 4152 415f 434c 4f55 445f  lf.__YARA_CLOUD_
+00012b60: 5245 5452 4f53 4341 4e53 5f45 4e44 504f  RETROSCANS_ENDPO
+00012b70: 494e 542e 666f 726d 6174 2872 756c 6573  INT.format(rules
+00012b80: 6574 5f6e 616d 653d 7275 6c65 7365 745f  et_name=ruleset_
+00012b90: 6e61 6d65 290a 0a20 2020 2020 2020 2075  name)..        u
+00012ba0: 726c 203d 2073 656c 662e 5f75 726c 2e66  rl = self._url.f
+00012bb0: 6f72 6d61 7428 656e 6470 6f69 6e74 3d65  ormat(endpoint=e
+00012bc0: 6e64 706f 696e 7429 0a0a 2020 2020 2020  ndpoint)..      
+00012bd0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
+00012be0: 662e 5f5f 6765 745f 7265 7175 6573 7428  f.__get_request(
+00012bf0: 7572 6c3d 7572 6c29 0a0a 2020 2020 2020  url=url)..      
+00012c00: 2020 7365 6c66 2e5f 5f72 6169 7365 5f6f    self.__raise_o
+00012c10: 6e5f 6572 726f 7228 7265 7370 6f6e 7365  n_error(response
+00012c20: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00012c30: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
+00012c40: 6465 6620 6164 7661 6e63 6564 5f73 6561  def advanced_sea
+00012c50: 7263 6828 7365 6c66 2c20 7175 6572 795f  rch(self, query_
+00012c60: 7374 7269 6e67 2c20 7061 6765 5f6e 756d  string, page_num
+00012c70: 6265 723d 312c 2072 6563 6f72 6473 5f70  ber=1, records_p
+00012c80: 6572 5f70 6167 653d 3230 2c20 736f 7274  er_page=20, sort
+00012c90: 696e 675f 6372 6974 6572 6961 3d4e 6f6e  ing_criteria=Non
+00012ca0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00012cb0: 2020 2020 2020 2020 2020 2073 6f72 7469             sorti
+00012cc0: 6e67 5f6f 7264 6572 3d22 6465 7363 2229  ng_order="desc")
+00012cd0: 3a0a 2020 2020 2020 2020 2222 2254 4849  :.        """THI
+00012ce0: 5320 4d45 5448 4f44 2049 5320 4445 5052  S METHOD IS DEPR
+00012cf0: 4543 4154 4544 2e20 5573 6520 6164 7661  ECATED. Use adva
+00012d00: 6e63 6564 5f73 6561 7263 685f 7632 2069  nced_search_v2 i
+00012d10: 6e73 7465 6164 2e0a 0a20 2020 2020 2020  nstead...       
+00012d20: 2053 656e 6473 2061 2071 7565 7279 2073   Sends a query s
+00012d30: 7472 696e 6720 746f 2074 6865 2041 3130  tring to the A10
+00012d40: 3030 2041 6476 616e 6365 6420 5365 6172  00 Advanced Sear
+00012d50: 6368 2041 5049 2e0a 2020 2020 2020 2020  ch API..        
+00012d60: 5468 6520 7175 6572 7920 7374 7269 6e67  The query string
+00012d70: 206d 7573 7420 6265 2063 6f6d 706f 7365   must be compose
+00012d80: 6420 6f66 206b 6579 2d76 616c 7565 2070  d of key-value p
+00012d90: 6169 7273 2073 6570 6172 6174 6564 2062  airs separated b
+00012da0: 7920 7370 6163 652e 0a20 2020 2020 2020  y space..       
+00012db0: 2041 206b 6579 2069 7320 7365 7061 7261   A key is separa
+00012dc0: 7465 6420 6672 6f6d 2069 7473 2076 616c  ted from its val
+00012dd0: 7565 2062 7920 6120 636f 6c6f 6e20 7379  ue by a colon sy
+00012de0: 6d62 6f6c 2061 6e64 206e 6f20 7370 6163  mbol and no spac
+00012df0: 6573 2e0a 2020 2020 2020 2020 4966 2061  es..        If a
+00012e00: 2070 6167 6520 6e75 6d62 6572 2069 7320   page number is 
+00012e10: 6e6f 7420 7072 6f76 6964 6564 2c20 7468  not provided, th
+00012e20: 6520 6669 7273 7420 7061 6765 206f 6620  e first page of 
+00012e30: 7265 7375 6c74 7320 7769 6c6c 2062 6520  results will be 
+00012e40: 7265 7475 726e 6564 2e0a 2020 2020 2020  returned..      
+00012e50: 2020 2020 2020 5175 6572 7920 7374 7269        Query stri
+00012e60: 6e67 2065 7861 6d70 6c65 3a0a 2020 2020  ng example:.    
+00012e70: 2020 2020 2020 2020 2761 762d 636f 756e          'av-coun
+00012e80: 743a 3520 6176 6169 6c61 626c 653a 5452  t:5 available:TR
+00012e90: 5545 270a 0a20 2020 2020 2020 2020 2020  UE'..           
+00012ea0: 203a 7061 7261 6d20 7175 6572 795f 7374   :param query_st
+00012eb0: 7269 6e67 3a20 7175 6572 7920 7374 7269  ring: query stri
+00012ec0: 6e67 0a20 2020 2020 2020 2020 2020 203a  ng.            :
+00012ed0: 7479 7065 2071 7565 7279 5f73 7472 696e  type query_strin
+00012ee0: 673a 2073 7472 0a20 2020 2020 2020 2020  g: str.         
+00012ef0: 2020 203a 7061 7261 6d20 7061 6765 5f6e     :param page_n
+00012f00: 756d 6265 723a 2070 6167 6520 6e75 6d62  umber: page numb
+00012f10: 6572 0a20 2020 2020 2020 2020 2020 203a  er.            :
+00012f20: 7479 7065 2070 6167 655f 6e75 6d62 6572  type page_number
+00012f30: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
+00012f40: 2020 3a70 6172 616d 2072 6563 6f72 6473    :param records
+00012f50: 5f70 6572 5f70 6167 653a 206e 756d 6265  _per_page: numbe
+00012f60: 7220 6f66 2072 6563 6f72 6473 2072 6574  r of records ret
+00012f70: 7572 6e65 6420 7065 7220 7061 6765 3b20  urned per page; 
+00012f80: 6d61 7869 6d75 6d20 7661 6c75 6520 6973  maximum value is
+00012f90: 2031 3030 0a20 2020 2020 2020 2020 2020   100.           
+00012fa0: 203a 7479 7065 2072 6563 6f72 6473 5f70   :type records_p
+00012fb0: 6572 5f70 6167 653a 2069 6e74 0a20 2020  er_page: int.   
+00012fc0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00012fd0: 736f 7274 696e 675f 6372 6974 6572 6961  sorting_criteria
+00012fe0: 3a20 6465 6669 6e65 2074 6865 2063 7269  : define the cri
+00012ff0: 7465 7269 6120 7573 6564 2069 6e20 736f  teria used in so
+00013000: 7274 696e 673b 2070 6f73 7369 626c 6520  rting; possible 
+00013010: 7661 6c75 6573 2061 7265 2027 7368 6131  values are 'sha1
+00013020: 272c 2027 6669 7273 7473 6565 6e27 2c0a  ', 'firstseen',.
+00013030: 2020 2020 2020 2020 2020 2020 2774 6872              'thr
+00013040: 6561 746e 616d 6527 2c20 2773 616d 706c  eatname', 'sampl
+00013050: 6574 7970 6527 2c20 2766 696c 6563 6f75  etype', 'filecou
+00013060: 6e74 272c 2027 7369 7a65 270a 2020 2020  nt', 'size'.    
+00013070: 2020 2020 2020 2020 3a74 7970 6520 736f          :type so
+00013080: 7274 696e 675f 6372 6974 6572 6961 3a20  rting_criteria: 
+00013090: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+000130a0: 3a70 6172 616d 2073 6f72 7469 6e67 5f6f  :param sorting_o
+000130b0: 7264 6572 3a20 736f 7274 696e 6720 6f72  rder: sorting or
+000130c0: 6465 723b 2070 6f73 7369 626c 6520 7661  der; possible va
+000130d0: 6c75 6573 2061 7265 2027 6465 7363 272c  lues are 'desc',
+000130e0: 2027 6173 6327 0a20 2020 2020 2020 2020   'asc'.         
+000130f0: 2020 203a 7479 7065 2073 6f72 7469 6e67     :type sorting
+00013100: 5f6f 7264 6572 3a20 7374 720a 2020 2020  _order: str.    
+00013110: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00013120: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+00013130: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
+00013140: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
+00013150: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013160: 2020 2020 7761 726e 2822 5468 6973 206d      warn("This m
+00013170: 6574 686f 6420 6973 2064 6570 7265 6361  ethod is depreca
+00013180: 7465 642e 2055 7365 2061 6476 616e 6365  ted. Use advance
+00013190: 645f 7365 6172 6368 5f76 3220 696e 7374  d_search_v2 inst
+000131a0: 6561 642e 222c 2044 6570 7265 6361 7469  ead.", Deprecati
+000131b0: 6f6e 5761 726e 696e 6729 0a0a 2020 2020  onWarning)..    
+000131c0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+000131d0: 7461 6e63 6528 7175 6572 795f 7374 7269  tance(query_stri
+000131e0: 6e67 2c20 7374 7229 3a0a 2020 2020 2020  ng, str):.      
+000131f0: 2020 2020 2020 7261 6973 6520 5772 6f6e        raise Wron
+00013200: 6749 6e70 7574 4572 726f 7228 2254 6865  gInputError("The
+00013210: 2073 6561 7263 6820 7175 6572 7920 6d75   search query mu
+00013220: 7374 2062 6520 6120 7374 7269 6e67 2e22  st be a string."
+00013230: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+00013240: 7420 6973 696e 7374 616e 6365 2872 6563  t isinstance(rec
+00013250: 6f72 6473 5f70 6572 5f70 6167 652c 2069  ords_per_page, i
+00013260: 6e74 2920 6f72 206e 6f74 2031 203c 3d20  nt) or not 1 <= 
+00013270: 7265 636f 7264 735f 7065 725f 7061 6765  records_per_page
+00013280: 203c 3d20 3130 303a 0a20 2020 2020 2020   <= 100:.       
+00013290: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
+000132a0: 496e 7075 7445 7272 6f72 2822 7265 636f  InputError("reco
+000132b0: 7264 735f 7065 725f 7061 6765 2070 6172  rds_per_page par
+000132c0: 616d 6574 6572 206d 7573 7420 6265 2061  ameter must be a
+000132d0: 6e20 696e 7465 6765 7220 7769 7468 2061  n integer with a
+000132e0: 2076 616c 7565 2022 0a20 2020 2020 2020   value ".       
+000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013300: 2020 2020 2020 2020 2020 2022 6265 7477             "betw
+00013310: 6565 6e20 3120 616e 6420 3130 3020 2869  een 1 and 100 (i
+00013320: 6e63 6c75 6465 6429 2e22 290a 0a20 2020  ncluded).")..   
+00013330: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
+00013340: 5f75 726c 2e66 6f72 6d61 7428 656e 6470  _url.format(endp
+00013350: 6f69 6e74 3d73 656c 662e 5f5f 4144 5641  oint=self.__ADVA
+00013360: 4e43 4544 5f53 4541 5243 485f 454e 4450  NCED_SEARCH_ENDP
+00013370: 4f49 4e54 290a 0a20 2020 2020 2020 2070  OINT)..        p
+00013380: 6f73 745f 6a73 6f6e 203d 207b 2271 7565  ost_json = {"que
+00013390: 7279 223a 2071 7565 7279 5f73 7472 696e  ry": query_strin
+000133a0: 672c 2022 7061 6765 223a 2070 6167 655f  g, "page": page_
+000133b0: 6e75 6d62 6572 2c20 2272 6563 6f72 6473  number, "records
+000133c0: 5f70 6572 5f70 6167 6522 3a20 7265 636f  _per_page": reco
+000133d0: 7264 735f 7065 725f 7061 6765 7d0a 0a20  rds_per_page}.. 
+000133e0: 2020 2020 2020 2069 6620 736f 7274 696e         if sortin
+000133f0: 675f 6372 6974 6572 6961 3a0a 2020 2020  g_criteria:.    
+00013400: 2020 2020 2020 2020 6966 2073 6f72 7469          if sorti
+00013410: 6e67 5f63 7269 7465 7269 6120 6e6f 7420  ng_criteria not 
+00013420: 696e 2041 4456 414e 4345 445f 5345 4152  in ADVANCED_SEAR
+00013430: 4348 5f53 4f52 5449 4e47 5f43 5249 5445  CH_SORTING_CRITE
+00013440: 5249 4120 6f72 2073 6f72 7469 6e67 5f6f  RIA or sorting_o
+00013450: 7264 6572 206e 6f74 2069 6e20 2822 6465  rder not in ("de
+00013460: 7363 222c 2022 6173 6322 293a 0a20 2020  sc", "asc"):.   
+00013470: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00013480: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
+00013490: 6f72 2822 536f 7274 696e 6720 6372 6974  or("Sorting crit
+000134a0: 6572 6961 206d 7573 7420 6265 206f 6e65  eria must be one
+000134b0: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
+000134c0: 6720 6f70 7469 6f6e 733a 207b 6372 6974  g options: {crit
+000134d0: 6572 6961 7d2e 2022 0a20 2020 2020 2020  eria}. ".       
+000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013500: 536f 7274 696e 6720 6f72 6465 7220 6e65  Sorting order ne
+00013510: 6564 7320 746f 2062 6520 2764 6573 6327  eds to be 'desc'
+00013520: 206f 7220 2761 7363 272e 222e 666f 726d   or 'asc'.".form
+00013530: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013550: 2020 2020 2020 2020 2020 2020 6372 6974              crit
+00013560: 6572 6961 3d41 4456 414e 4345 445f 5345  eria=ADVANCED_SE
+00013570: 4152 4348 5f53 4f52 5449 4e47 5f43 5249  ARCH_SORTING_CRI
+00013580: 5445 5249 410a 2020 2020 2020 2020 2020  TERIA.          
+00013590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135a0: 2020 2020 2020 2020 2020 2020 2929 0a20              )). 
+000135b0: 2020 2020 2020 2020 2020 2073 6f72 7469             sorti
+000135c0: 6e67 5f65 7870 7265 7373 696f 6e20 3d20  ng_expression = 
+000135d0: 227b 6372 6974 6572 6961 7d20 7b6f 7264  "{criteria} {ord
+000135e0: 6572 7d22 2e66 6f72 6d61 7428 0a20 2020  er}".format(.   
+000135f0: 2020 2020 2020 2020 2020 2020 2063 7269               cri
+00013600: 7465 7269 613d 736f 7274 696e 675f 6372  teria=sorting_cr
+00013610: 6974 6572 6961 2c0a 2020 2020 2020 2020  iteria,.        
+00013620: 2020 2020 2020 2020 6f72 6465 723d 736f          order=so
+00013630: 7274 696e 675f 6f72 6465 720a 2020 2020  rting_order.    
+00013640: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00013650: 2020 2020 2020 2070 6f73 745f 6a73 6f6e         post_json
+00013660: 5b22 736f 7274 225d 203d 2073 6f72 7469  ["sort"] = sorti
+00013670: 6e67 5f65 7870 7265 7373 696f 6e0a 0a20  ng_expression.. 
+00013680: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+00013690: 3d20 7365 6c66 2e5f 5f70 6f73 745f 7265  = self.__post_re
+000136a0: 7175 6573 7428 7572 6c3d 7572 6c2c 2070  quest(url=url, p
+000136b0: 6f73 745f 6a73 6f6e 3d70 6f73 745f 6a73  ost_json=post_js
+000136c0: 6f6e 290a 0a20 2020 2020 2020 2073 656c  on)..        sel
+000136d0: 662e 5f5f 7261 6973 655f 6f6e 5f65 7272  f.__raise_on_err
+000136e0: 6f72 2872 6573 706f 6e73 6529 0a0a 2020  or(response)..  
+000136f0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00013700: 706f 6e73 650a 0a20 2020 2064 6566 2061  ponse..    def a
+00013710: 6476 616e 6365 645f 7365 6172 6368 5f61  dvanced_search_a
+00013720: 6767 7265 6761 7465 6428 7365 6c66 2c20  ggregated(self, 
+00013730: 7175 6572 795f 7374 7269 6e67 2c20 6d61  query_string, ma
+00013740: 785f 7265 7375 6c74 733d 3530 3030 2c20  x_results=5000, 
+00013750: 736f 7274 696e 675f 6372 6974 6572 6961  sorting_criteria
+00013760: 3d4e 6f6e 652c 2073 6f72 7469 6e67 5f6f  =None, sorting_o
+00013770: 7264 6572 3d22 6465 7363 2229 3a0a 2020  rder="desc"):.  
+00013780: 2020 2020 2020 2222 2254 4849 5320 4d45        """THIS ME
+00013790: 5448 4f44 2049 5320 4445 5052 4543 4154  THOD IS DEPRECAT
+000137a0: 4544 2e20 5573 6520 6164 7661 6e63 6564  ED. Use advanced
+000137b0: 5f73 6561 7263 685f 7632 5f61 6767 7265  _search_v2_aggre
+000137c0: 6761 7465 6420 696e 7374 6561 642e 0a0a  gated instead...
+000137d0: 2020 2020 2020 2020 5365 6e64 7320 7468          Sends th
+000137e0: 6520 7175 6572 7920 7374 7269 6e67 2074  e query string t
+000137f0: 6f20 7468 6520 4131 3030 3020 4164 7661  o the A1000 Adva
+00013800: 6e63 6564 2053 6561 7263 6820 4150 492e  nced Search API.
+00013810: 0a20 2020 2020 2020 2054 6865 2071 7565  .        The que
+00013820: 7279 2073 7472 696e 6720 6d75 7374 2062  ry string must b
+00013830: 6520 636f 6d70 6f73 6564 206f 6620 6b65  e composed of ke
+00013840: 792d 7661 6c75 6520 7061 6972 7320 7365  y-value pairs se
+00013850: 7061 7261 7465 6420 6279 2073 7061 6365  parated by space
+00013860: 2e0a 2020 2020 2020 2020 4120 6b65 7920  ..        A key 
+00013870: 6973 2073 6570 6172 6174 6564 2066 726f  is separated fro
+00013880: 6d20 6974 7320 7661 6c75 6520 6279 2061  m its value by a
+00013890: 2063 6f6c 6f6e 2073 796d 626f 6c20 616e   colon symbol an
+000138a0: 6420 6e6f 2073 7061 6365 732e 0a20 2020  d no spaces..   
+000138b0: 2020 2020 2050 6167 696e 6720 6973 2064       Paging is d
+000138c0: 6f6e 6520 6175 746f 6d61 7469 6361 6c6c  one automaticall
+000138d0: 7920 616e 6420 7265 7375 6c74 7320 6672  y and results fr
+000138e0: 6f6d 2069 6e64 6976 6964 7561 6c0a 2020  om individual.  
+000138f0: 2020 2020 2020 7265 7370 6f6e 7365 7320        responses 
+00013900: 6167 6772 6567 6174 6564 2069 6e74 6f20  aggregated into 
+00013910: 6f6e 6520 6c69 7374 2061 6e64 2072 6574  one list and ret
+00013920: 7572 6e65 642e 0a20 2020 2020 2020 2054  urned..        T
+00013930: 6865 2027 6d61 785f 7265 7375 6c74 7327  he 'max_results'
+00013940: 2070 6172 616d 6574 6572 2064 6566 696e   parameter defin
+00013950: 6573 2074 6865 206d 6178 696d 756d 2064  es the maximum d
+00013960: 6573 6972 6564 206e 756d 6265 7220 6f66  esired number of
+00013970: 2072 6573 756c 7473 2074 6f20 6265 2072   results to be r
+00013980: 6574 7572 6e65 642e 0a20 2020 2020 2020  eturned..       
+00013990: 2020 2020 2051 7565 7279 2073 7472 696e       Query strin
+000139a0: 6720 6578 616d 706c 653a 0a20 2020 2020  g example:.     
+000139b0: 2020 2020 2020 2027 6176 2d63 6f75 6e74         'av-count
+000139c0: 3a35 2061 7661 696c 6162 6c65 3a54 5255  :5 available:TRU
+000139d0: 4527 0a0a 2020 2020 2020 2020 2020 2020  E'..            
+000139e0: 3a70 6172 616d 2071 7565 7279 5f73 7472  :param query_str
+000139f0: 696e 673a 2073 6561 7263 6820 7175 6572  ing: search quer
+00013a00: 7920 2d20 7365 6520 4150 4920 646f 6375  y - see API docu
+00013a10: 6d65 6e74 6174 696f 6e20 666f 7220 6465  mentation for de
+00013a20: 7461 696c 7320 6f6e 2077 7269 7469 6e67  tails on writing
+00013a30: 2073 6561 7263 6820 7175 6572 6965 730a   search queries.
+00013a40: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+00013a50: 6520 7175 6572 795f 7374 7269 6e67 3a20  e query_string: 
+00013a60: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00013a70: 3a70 6172 616d 206d 6178 5f72 6573 756c  :param max_resul
+00013a80: 7473 3a20 6d61 7869 6d75 6d20 7265 7375  ts: maximum resu
+00013a90: 6c74 7320 746f 2062 6520 7265 7475 726e  lts to be return
+00013aa0: 6564 2069 6e20 6120 6c69 7374 3b20 6465  ed in a list; de
+00013ab0: 6661 756c 7420 7661 6c75 6520 6973 2035  fault value is 5
+00013ac0: 3030 300a 2020 2020 2020 2020 2020 2020  000.            
+00013ad0: 3a74 7970 6520 6d61 785f 7265 7375 6c74  :type max_result
+00013ae0: 733a 2069 6e74 0a20 2020 2020 2020 2020  s: int.         
+00013af0: 2020 203a 7061 7261 6d20 736f 7274 696e     :param sortin
+00013b00: 675f 6372 6974 6572 6961 3a20 6465 6669  g_criteria: defi
+00013b10: 6e65 2074 6865 2063 7269 7465 7269 6120  ne the criteria 
+00013b20: 7573 6564 2069 6e20 736f 7274 696e 673b  used in sorting;
+00013b30: 2070 6f73 7369 626c 6520 7661 6c75 6573   possible values
+00013b40: 2061 7265 2027 7368 6131 272c 2027 6669   are 'sha1', 'fi
+00013b50: 7273 7473 6565 6e27 2c0a 2020 2020 2020  rstseen',.      
+00013b60: 2020 2020 2020 2774 6872 6561 746e 616d        'threatnam
+00013b70: 6527 2c20 2773 616d 706c 6574 7970 6527  e', 'sampletype'
+00013b80: 2c20 2766 696c 6563 6f75 6e74 272c 2027  , 'filecount', '
+00013b90: 7369 7a65 270a 2020 2020 2020 2020 2020  size'.          
+00013ba0: 2020 3a74 7970 6520 736f 7274 696e 675f    :type sorting_
+00013bb0: 6372 6974 6572 6961 3a20 7374 720a 2020  criteria: str.  
+00013bc0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+00013bd0: 2073 6f72 7469 6e67 5f6f 7264 6572 3a20   sorting_order: 
+00013be0: 736f 7274 696e 6720 6f72 6465 723b 2070  sorting order; p
+00013bf0: 6f73 7369 626c 6520 7661 6c75 6573 2061  ossible values a
+00013c00: 7265 2027 6465 7363 272c 2027 6173 6327  re 'desc', 'asc'
+00013c10: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
+00013c20: 7065 2073 6f72 7469 6e67 5f6f 7264 6572  pe sorting_order
+00013c30: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+00013c40: 2020 3a72 6574 7572 6e3a 206c 6973 7420    :return: list 
+00013c50: 6f66 2072 6573 756c 7473 0a20 2020 2020  of results.     
+00013c60: 2020 2020 2020 203a 7274 7970 653a 206c         :rtype: l
+00013c70: 6973 740a 2020 2020 2020 2020 2222 220a  ist.        """.
+00013c80: 2020 2020 2020 2020 7761 726e 2822 5468          warn("Th
+00013c90: 6973 206d 6574 686f 6420 6973 2064 6570  is method is dep
+00013ca0: 7265 6361 7465 642e 2055 7365 2061 6476  recated. Use adv
+00013cb0: 616e 6365 645f 7365 6172 6368 5f76 325f  anced_search_v2_
+00013cc0: 6167 6772 6567 6174 6564 2069 6e73 7465  aggregated inste
+00013cd0: 6164 2e22 2c20 4465 7072 6563 6174 696f  ad.", Deprecatio
+00013ce0: 6e57 6172 6e69 6e67 290a 0a20 2020 2020  nWarning)..     
+00013cf0: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00013d00: 616e 6365 286d 6178 5f72 6573 756c 7473  ance(max_results
+00013d10: 2c20 696e 7429 3a0a 2020 2020 2020 2020  , int):.        
+00013d20: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
+00013d30: 6e70 7574 4572 726f 7228 226d 6178 5f72  nputError("max_r
+00013d40: 6573 756c 7473 2070 6172 616d 6574 6572  esults parameter
+00013d50: 206d 7573 7420 6265 2069 6e74 6567 6572   must be integer
+00013d60: 2e22 290a 0a20 2020 2020 2020 2072 6573  .")..        res
+00013d70: 756c 7473 203d 205b 5d0a 2020 2020 2020  ults = [].      
+00013d80: 2020 6e65 7874 5f70 6167 6520 3d20 310a    next_page = 1.
+00013d90: 2020 2020 2020 2020 6d6f 7265 5f70 6167          more_pag
+00013da0: 6573 203d 2054 7275 650a 0a20 2020 2020  es = True..     
+00013db0: 2020 2077 6869 6c65 206d 6f72 655f 7061     while more_pa
+00013dc0: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
+00013dd0: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
+00013de0: 2e61 6476 616e 6365 645f 7365 6172 6368  .advanced_search
+00013df0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00013e00: 2020 7175 6572 795f 7374 7269 6e67 3d71    query_string=q
+00013e10: 7565 7279 5f73 7472 696e 672c 0a20 2020  uery_string,.   
+00013e20: 2020 2020 2020 2020 2020 2020 2070 6167               pag
+00013e30: 655f 6e75 6d62 6572 3d6e 6578 745f 7061  e_number=next_pa
+00013e40: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
+00013e50: 2020 2020 7265 636f 7264 735f 7065 725f      records_per_
+00013e60: 7061 6765 3d31 3030 2c0a 2020 2020 2020  page=100,.      
+00013e70: 2020 2020 2020 2020 2020 736f 7274 696e            sortin
+00013e80: 675f 6372 6974 6572 6961 3d73 6f72 7469  g_criteria=sorti
+00013e90: 6e67 5f63 7269 7465 7269 612c 0a20 2020  ng_criteria,.   
+00013ea0: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
+00013eb0: 7469 6e67 5f6f 7264 6572 3d73 6f72 7469  ting_order=sorti
+00013ec0: 6e67 5f6f 7264 6572 0a20 2020 2020 2020  ng_order.       
+00013ed0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00013ee0: 2020 2020 7265 7370 6f6e 7365 5f6a 736f      response_jso
+00013ef0: 6e20 3d20 7265 7370 6f6e 7365 2e6a 736f  n = response.jso
+00013f00: 6e28 290a 0a20 2020 2020 2020 2020 2020  n()..           
+00013f10: 2065 6e74 7269 6573 203d 2072 6573 706f   entries = respo
+00013f20: 6e73 655f 6a73 6f6e 2e67 6574 2822 726c  nse_json.get("rl
+00013f30: 2229 2e67 6574 2822 7765 625f 7365 6172  ").get("web_sear
+00013f40: 6368 5f61 7069 2229 2e67 6574 2822 656e  ch_api").get("en
+00013f50: 7472 6965 7322 2c20 5b5d 290a 2020 2020  tries", []).    
+00013f60: 2020 2020 2020 2020 7265 7375 6c74 732e          results.
+00013f70: 6578 7465 6e64 2865 6e74 7269 6573 290a  extend(entries).
+00013f80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013f90: 6c65 6e28 7265 7375 6c74 7329 203e 206d  len(results) > m
+00013fa0: 6178 5f72 6573 756c 7473 3a0a 2020 2020  ax_results:.    
+00013fb0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00013fc0: 6c74 7320 3d20 7265 7375 6c74 735b 3a6d  lts = results[:m
+00013fd0: 6178 5f72 6573 756c 7473 5d0a 2020 2020  ax_results].    
+00013fe0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013ff0: 726e 2072 6573 756c 7473 0a0a 2020 2020  rn results..    
+00014000: 2020 2020 2020 2020 6e65 7874 5f70 6167          next_pag
+00014010: 6520 3d20 7265 7370 6f6e 7365 5f6a 736f  e = response_jso
+00014020: 6e2e 6765 7428 2272 6c22 292e 6765 7428  n.get("rl").get(
+00014030: 2277 6562 5f73 6561 7263 685f 6170 6922  "web_search_api"
+00014040: 292e 6765 7428 226e 6578 745f 7061 6765  ).get("next_page
+00014050: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
+00014060: 2020 2020 206d 6f72 655f 7061 6765 7320       more_pages 
+00014070: 3d20 7265 7370 6f6e 7365 5f6a 736f 6e2e  = response_json.
+00014080: 6765 7428 2272 6c22 292e 6765 7428 2277  get("rl").get("w
+00014090: 6562 5f73 6561 7263 685f 6170 6922 292e  eb_search_api").
+000140a0: 6765 7428 226d 6f72 655f 7061 6765 7322  get("more_pages"
+000140b0: 2c20 4661 6c73 6529 0a0a 2020 2020 2020  , False)..      
+000140c0: 2020 7265 7475 726e 2072 6573 756c 7473    return results
+000140d0: 0a0a 2020 2020 6465 6620 6164 7661 6e63  ..    def advanc
+000140e0: 6564 5f73 6561 7263 685f 7632 2873 656c  ed_search_v2(sel
+000140f0: 662c 2071 7565 7279 5f73 7472 696e 672c  f, query_string,
+00014100: 2074 6963 6c6f 7564 3d46 616c 7365 2c20   ticloud=False, 
+00014110: 7061 6765 5f6e 756d 6265 723d 312c 2072  page_number=1, r
+00014120: 6563 6f72 6473 5f70 6572 5f70 6167 653d  ecords_per_page=
+00014130: 3230 2c20 736f 7274 696e 675f 6372 6974  20, sorting_crit
+00014140: 6572 6961 3d4e 6f6e 652c 0a20 2020 2020  eria=None,.     
+00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014160: 2020 2020 2020 736f 7274 696e 675f 6f72        sorting_or
+00014170: 6465 723d 2264 6573 6322 293a 0a20 2020  der="desc"):.   
+00014180: 2020 2020 2022 2222 5365 6e64 7320 6120       """Sends a 
+00014190: 7175 6572 7920 7374 7269 6e67 2074 6f20  query string to 
+000141a0: 7468 6520 4131 3030 3020 4164 7661 6e63  the A1000 Advanc
+000141b0: 6564 2053 6561 7263 6820 4150 4920 7632  ed Search API v2
+000141c0: 2e0a 2020 2020 2020 2020 5468 6520 7175  ..        The qu
+000141d0: 6572 7920 7374 7269 6e67 206d 7573 7420  ery string must 
+000141e0: 6265 2063 6f6d 706f 7365 6420 6f66 206b  be composed of k
+000141f0: 6579 2d76 616c 7565 2070 6169 7273 2073  ey-value pairs s
+00014200: 6570 6172 6174 6564 2062 7920 7370 6163  eparated by spac
+00014210: 652e 0a20 2020 2020 2020 2041 206b 6579  e..        A key
+00014220: 2069 7320 7365 7061 7261 7465 6420 6672   is separated fr
+00014230: 6f6d 2069 7473 2076 616c 7565 2062 7920  om its value by 
+00014240: 6120 636f 6c6f 6e20 7379 6d62 6f6c 2061  a colon symbol a
+00014250: 6e64 206e 6f20 7370 6163 6573 2e0a 2020  nd no spaces..  
+00014260: 2020 2020 2020 466f 7220 6469 7265 6374        For direct
+00014270: 696f 6e73 206f 6e20 686f 7720 746f 2077  ions on how to w
+00014280: 7269 7465 2061 6476 616e 6365 6420 7365  rite advanced se
+00014290: 6172 6368 2071 7565 7269 6573 2c20 636f  arch queries, co
+000142a0: 6e73 756c 7420 7468 6520 4131 3030 3020  nsult the A1000 
+000142b0: 646f 6375 6d65 6e74 6174 696f 6e2e 0a20  documentation.. 
+000142c0: 2020 2020 2020 2049 6620 6120 7061 6765         If a page
+000142d0: 206e 756d 6265 7220 6973 206e 6f74 2070   number is not p
+000142e0: 726f 7669 6465 642c 2074 6865 2066 6972  rovided, the fir
+000142f0: 7374 2070 6167 6520 6f66 2072 6573 756c  st page of resul
+00014300: 7473 2077 696c 6c20 6265 2072 6574 7572  ts will be retur
+00014310: 6e65 642e 0a20 2020 2020 2020 2020 2020  ned..           
+00014320: 2051 7565 7279 2073 7472 696e 6720 6578   Query string ex
+00014330: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
+00014340: 2020 2027 6176 2d63 6f75 6e74 3a35 2061     'av-count:5 a
+00014350: 7661 696c 6162 6c65 3a54 5255 4527 0a0a  vailable:TRUE'..
+00014360: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00014370: 616d 2071 7565 7279 5f73 7472 696e 673a  am query_string:
+00014380: 2071 7565 7279 2073 7472 696e 670a 2020   query string.  
+00014390: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+000143a0: 7175 6572 795f 7374 7269 6e67 3a20 7374  query_string: st
+000143b0: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
+000143c0: 6172 616d 2074 6963 6c6f 7564 3a20 7368  aram ticloud: sh
+000143d0: 6f77 206f 6e6c 7920 636c 6f75 6420 7265  ow only cloud re
+000143e0: 7375 6c74 730a 2020 2020 2020 2020 2020  sults.          
+000143f0: 2020 3a74 7970 6520 7469 636c 6f75 643a    :type ticloud:
+00014400: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
+00014410: 2020 3a70 6172 616d 2070 6167 655f 6e75    :param page_nu
+00014420: 6d62 6572 3a20 7061 6765 206e 756d 6265  mber: page numbe
+00014430: 720a 2020 2020 2020 2020 2020 2020 3a74  r.            :t
+00014440: 7970 6520 7061 6765 5f6e 756d 6265 723a  ype page_number:
+00014450: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+00014460: 203a 7061 7261 6d20 7265 636f 7264 735f   :param records_
+00014470: 7065 725f 7061 6765 3a20 6e75 6d62 6572  per_page: number
+00014480: 206f 6620 7265 636f 7264 7320 7265 7475   of records retu
+00014490: 726e 6564 2070 6572 2070 6167 653b 206d  rned per page; m
+000144a0: 6178 696d 756d 2076 616c 7565 2069 7320  aximum value is 
+000144b0: 3130 300a 2020 2020 2020 2020 2020 2020  100.            
+000144c0: 3a74 7970 6520 7265 636f 7264 735f 7065  :type records_pe
+000144d0: 725f 7061 6765 3a20 696e 740a 2020 2020  r_page: int.    
+000144e0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+000144f0: 6f72 7469 6e67 5f63 7269 7465 7269 613a  orting_criteria:
+00014500: 2064 6566 696e 6520 7468 6520 6372 6974   define the crit
+00014510: 6572 6961 2075 7365 6420 696e 2073 6f72  eria used in sor
+00014520: 7469 6e67 3b20 706f 7373 6962 6c65 2076  ting; possible v
+00014530: 616c 7565 7320 6172 6520 2773 6861 3127  alues are 'sha1'
+00014540: 2c20 2766 6972 7374 7365 656e 272c 0a20  , 'firstseen',. 
+00014550: 2020 2020 2020 2020 2020 2027 7468 7265             'thre
+00014560: 6174 6e61 6d65 272c 2027 7361 6d70 6c65  atname', 'sample
+00014570: 7479 7065 272c 2027 6669 6c65 636f 756e  type', 'filecoun
+00014580: 7427 2c20 2773 697a 6527 0a20 2020 2020  t', 'size'.     
+00014590: 2020 2020 2020 203a 7479 7065 2073 6f72         :type sor
+000145a0: 7469 6e67 5f63 7269 7465 7269 613a 2073  ting_criteria: s
+000145b0: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
+000145c0: 7061 7261 6d20 736f 7274 696e 675f 6f72  param sorting_or
+000145d0: 6465 723a 2073 6f72 7469 6e67 206f 7264  der: sorting ord
+000145e0: 6572 3b20 706f 7373 6962 6c65 2076 616c  er; possible val
+000145f0: 7565 7320 6172 6520 2764 6573 6327 2c20  ues are 'desc', 
+00014600: 2761 7363 270a 2020 2020 2020 2020 2020  'asc'.          
+00014610: 2020 3a74 7970 6520 736f 7274 696e 675f    :type sorting_
+00014620: 6f72 6465 723a 2073 7472 0a20 2020 2020  order: str.     
+00014630: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00014640: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+00014650: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
+00014660: 7565 7374 732e 5265 7370 6f6e 7365 0a20  uests.Response. 
+00014670: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014680: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00014690: 616e 6365 2871 7565 7279 5f73 7472 696e  ance(query_strin
+000146a0: 672c 2073 7472 293a 0a20 2020 2020 2020  g, str):.       
+000146b0: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
+000146c0: 496e 7075 7445 7272 6f72 2822 5468 6520  InputError("The 
+000146d0: 7365 6172 6368 2071 7565 7279 206d 7573  search query mus
+000146e0: 7420 6265 2061 2073 7472 696e 672e 2229  t be a string.")
+000146f0: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00014700: 2069 7369 6e73 7461 6e63 6528 7469 636c   isinstance(ticl
+00014710: 6f75 642c 2062 6f6f 6c29 3a0a 2020 2020  oud, bool):.    
+00014720: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
+00014730: 6f6e 6749 6e70 7574 4572 726f 7228 2274  ongInputError("t
+00014740: 6963 6c6f 7564 2070 6172 616d 6574 6572  icloud parameter
+00014750: 206d 7573 7420 6265 2062 6f6f 6c65 616e   must be boolean
+00014760: 2e22 290a 0a20 2020 2020 2020 2069 6620  .")..        if 
+00014770: 6e6f 7420 6973 696e 7374 616e 6365 2872  not isinstance(r
+00014780: 6563 6f72 6473 5f70 6572 5f70 6167 652c  ecords_per_page,
+00014790: 2069 6e74 2920 6f72 206e 6f74 2031 203c   int) or not 1 <
+000147a0: 3d20 7265 636f 7264 735f 7065 725f 7061  = records_per_pa
+000147b0: 6765 203c 3d20 3130 303a 0a20 2020 2020  ge <= 100:.     
+000147c0: 2020 2020 2020 2072 6169 7365 2057 726f         raise Wro
+000147d0: 6e67 496e 7075 7445 7272 6f72 2822 7265  ngInputError("re
+000147e0: 636f 7264 735f 7065 725f 7061 6765 2070  cords_per_page p
+000147f0: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+00014800: 2061 6e20 696e 7465 6765 7220 7769 7468   an integer with
+00014810: 2061 2076 616c 7565 2022 0a20 2020 2020   a value ".     
+00014820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014830: 2020 2020 2020 2020 2020 2020 2022 6265               "be
+00014840: 7477 6565 6e20 3120 616e 6420 3130 3020  tween 1 and 100 
+00014850: 2869 6e63 6c75 6465 6429 2e22 290a 0a20  (included).").. 
+00014860: 2020 2020 2020 2075 726c 203d 2073 656c         url = sel
+00014870: 662e 5f75 726c 2e66 6f72 6d61 7428 656e  f._url.format(en
+00014880: 6470 6f69 6e74 3d73 656c 662e 5f5f 4144  dpoint=self.__AD
+00014890: 5641 4e43 4544 5f53 4541 5243 485f 454e  VANCED_SEARCH_EN
+000148a0: 4450 4f49 4e54 5f56 3229 0a0a 2020 2020  DPOINT_V2)..    
+000148b0: 2020 2020 706f 7374 5f6a 736f 6e20 3d20      post_json = 
+000148c0: 7b22 7175 6572 7922 3a20 7175 6572 795f  {"query": query_
+000148d0: 7374 7269 6e67 2c20 2274 6963 6c6f 7564  string, "ticloud
+000148e0: 223a 2074 6963 6c6f 7564 2c20 2270 6167  ": ticloud, "pag
+000148f0: 6522 3a20 7061 6765 5f6e 756d 6265 722c  e": page_number,
+00014900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014910: 2020 2020 2020 2272 6563 6f72 6473 5f70        "records_p
+00014920: 6572 5f70 6167 6522 3a20 7265 636f 7264  er_page": record
+00014930: 735f 7065 725f 7061 6765 7d0a 0a20 2020  s_per_page}..   
+00014940: 2020 2020 2069 6620 736f 7274 696e 675f       if sorting_
+00014950: 6372 6974 6572 6961 3a0a 2020 2020 2020  criteria:.      
+00014960: 2020 2020 2020 6966 2073 6f72 7469 6e67        if sorting
+00014970: 5f63 7269 7465 7269 6120 6e6f 7420 696e  _criteria not in
+00014980: 2041 4456 414e 4345 445f 5345 4152 4348   ADVANCED_SEARCH
+00014990: 5f53 4f52 5449 4e47 5f43 5249 5445 5249  _SORTING_CRITERI
+000149a0: 4120 6f72 2073 6f72 7469 6e67 5f6f 7264  A or sorting_ord
+000149b0: 6572 206e 6f74 2069 6e20 2822 6465 7363  er not in ("desc
+000149c0: 222c 2022 6173 6322 293a 0a20 2020 2020  ", "asc"):.     
+000149d0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000149e0: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
+000149f0: 2822 536f 7274 696e 6720 6372 6974 6572  ("Sorting criter
+00014a00: 6961 206d 7573 7420 6265 206f 6e65 206f  ia must be one o
+00014a10: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
+00014a20: 6f70 7469 6f6e 733a 207b 6372 6974 6572  options: {criter
+00014a30: 6961 7d2e 2022 0a20 2020 2020 2020 2020  ia}. ".         
+00014a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a50: 2020 2020 2020 2020 2020 2020 2022 536f               "So
+00014a60: 7274 696e 6720 6f72 6465 7220 6e65 6564  rting order need
+00014a70: 7320 746f 2062 6520 2764 6573 6327 206f  s to be 'desc' o
+00014a80: 7220 2761 7363 272e 222e 666f 726d 6174  r 'asc'.".format
+00014a90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
 00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ac0: 2020 2020 2029 290a 2020 2020 2020 2020       )).        
-00014ad0: 2020 2020 736f 7274 696e 675f 6578 7072      sorting_expr
-00014ae0: 6573 7369 6f6e 203d 2022 7b63 7269 7465  ession = "{crite
-00014af0: 7269 617d 207b 6f72 6465 727d 222e 666f  ria} {order}".fo
-00014b00: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00014b10: 2020 2020 2020 6372 6974 6572 6961 3d73        criteria=s
-00014b20: 6f72 7469 6e67 5f63 7269 7465 7269 612c  orting_criteria,
-00014b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014b40: 206f 7264 6572 3d73 6f72 7469 6e67 5f6f   order=sorting_o
-00014b50: 7264 6572 0a20 2020 2020 2020 2020 2020  rder.           
-00014b60: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00014b70: 706f 7374 5f6a 736f 6e5b 2273 6f72 7422  post_json["sort"
-00014b80: 5d20 3d20 736f 7274 696e 675f 6578 7072  ] = sorting_expr
-00014b90: 6573 7369 6f6e 0a0a 2020 2020 2020 2020  ession..        
-00014ba0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-00014bb0: 5f5f 706f 7374 5f72 6571 7565 7374 2875  __post_request(u
-00014bc0: 726c 3d75 726c 2c20 706f 7374 5f6a 736f  rl=url, post_jso
-00014bd0: 6e3d 706f 7374 5f6a 736f 6e29 0a0a 2020  n=post_json)..  
-00014be0: 2020 2020 2020 7365 6c66 2e5f 5f72 6169        self.__rai
-00014bf0: 7365 5f6f 6e5f 6572 726f 7228 7265 7370  se_on_error(resp
-00014c00: 6f6e 7365 290a 0a20 2020 2020 2020 2072  onse)..        r
-00014c10: 6574 7572 6e20 7265 7370 6f6e 7365 0a0a  eturn response..
-00014c20: 2020 2020 6465 6620 6164 7661 6e63 6564      def advanced
-00014c30: 5f73 6561 7263 685f 7632 5f61 6767 7265  _search_v2_aggre
-00014c40: 6761 7465 6428 7365 6c66 2c20 2071 7565  gated(self,  que
-00014c50: 7279 5f73 7472 696e 672c 2074 6963 6c6f  ry_string, ticlo
-00014c60: 7564 3d46 616c 7365 2c20 6d61 785f 7265  ud=False, max_re
-00014c70: 7375 6c74 733d 3530 3030 2c20 736f 7274  sults=5000, sort
-00014c80: 696e 675f 6372 6974 6572 6961 3d4e 6f6e  ing_criteria=Non
-00014c90: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00014ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cb0: 2020 2020 2020 2020 2073 6f72 7469 6e67           sorting
-00014cc0: 5f6f 7264 6572 3d22 6465 7363 2229 3a0a  _order="desc"):.
-00014cd0: 2020 2020 2020 2020 2222 2253 656e 6473          """Sends
-00014ce0: 2061 2071 7565 7279 2073 7472 696e 6720   a query string 
-00014cf0: 746f 2074 6865 2041 3130 3030 2041 6476  to the A1000 Adv
-00014d00: 616e 6365 6420 5365 6172 6368 2041 5049  anced Search API
-00014d10: 2076 322e 0a20 2020 2020 2020 2054 6865   v2..        The
-00014d20: 2071 7565 7279 2073 7472 696e 6720 6d75   query string mu
-00014d30: 7374 2062 6520 636f 6d70 6f73 6564 206f  st be composed o
-00014d40: 6620 6b65 792d 7661 6c75 6520 7061 6972  f key-value pair
-00014d50: 7320 7365 7061 7261 7465 6420 6279 2073  s separated by s
-00014d60: 7061 6365 2e0a 2020 2020 2020 2020 4120  pace..        A 
-00014d70: 6b65 7920 6973 2073 6570 6172 6174 6564  key is separated
-00014d80: 2066 726f 6d20 6974 7320 7661 6c75 6520   from its value 
-00014d90: 6279 2061 2063 6f6c 6f6e 2073 796d 626f  by a colon symbo
-00014da0: 6c20 616e 6420 6e6f 2073 7061 6365 732e  l and no spaces.
-00014db0: 0a20 2020 2020 2020 2046 6f72 2064 6972  .        For dir
-00014dc0: 6563 7469 6f6e 7320 6f6e 2068 6f77 2074  ections on how t
-00014dd0: 6f20 7772 6974 6520 6164 7661 6e63 6564  o write advanced
-00014de0: 2073 6561 7263 6820 7175 6572 6965 732c   search queries,
-00014df0: 2063 6f6e 7375 6c74 2074 6865 2041 3130   consult the A10
-00014e00: 3030 2064 6f63 756d 656e 7461 7469 6f6e  00 documentation
-00014e10: 2e0a 2020 2020 2020 2020 5061 6769 6e67  ..        Paging
-00014e20: 2069 7320 646f 6e65 2061 7574 6f6d 6174   is done automat
-00014e30: 6963 616c 6c79 2061 6e64 2072 6573 756c  ically and resul
-00014e40: 7473 2066 726f 6d20 696e 6469 7669 6475  ts from individu
-00014e50: 616c 0a20 2020 2020 2020 2072 6573 706f  al.        respo
-00014e60: 6e73 6573 2061 6767 7265 6761 7465 6420  nses aggregated 
-00014e70: 696e 746f 206f 6e65 206c 6973 7420 616e  into one list an
-00014e80: 6420 7265 7475 726e 6564 602e 0a20 2020  d returned`..   
-00014e90: 2020 2020 2054 6865 2027 6d61 785f 7265       The 'max_re
-00014ea0: 7375 6c74 7327 2070 6172 616d 6574 6572  sults' parameter
-00014eb0: 2064 6566 696e 6573 2074 6865 206d 6178   defines the max
-00014ec0: 696d 756d 2064 6573 6972 6564 206e 756d  imum desired num
-00014ed0: 6265 7220 6f66 2072 6573 756c 7473 2074  ber of results t
-00014ee0: 6f20 6265 2072 6574 7572 6e65 642e 0a20  o be returned.. 
-00014ef0: 2020 2020 2020 2020 2020 2051 7565 7279             Query
-00014f00: 2073 7472 696e 6720 6578 616d 706c 653a   string example:
-00014f10: 0a20 2020 2020 2020 2020 2020 2027 6176  .            'av
-00014f20: 2d63 6f75 6e74 3a35 2061 7661 696c 6162  -count:5 availab
-00014f30: 6c65 3a54 5255 4527 0a0a 2020 2020 2020  le:TRUE'..      
-00014f40: 2020 2020 2020 3a70 6172 616d 2071 7565        :param que
-00014f50: 7279 5f73 7472 696e 673a 2073 6561 7263  ry_string: searc
-00014f60: 6820 7175 6572 7920 2d20 7365 6520 4150  h query - see AP
-00014f70: 4920 646f 6375 6d65 6e74 6174 696f 6e20  I documentation 
-00014f80: 666f 7220 6465 7461 696c 7320 6f6e 2077  for details on w
-00014f90: 7269 7469 6e67 2073 6561 7263 6820 7175  riting search qu
-00014fa0: 6572 6965 730a 2020 2020 2020 2020 2020  eries.          
-00014fb0: 2020 3a74 7970 6520 7175 6572 795f 7374    :type query_st
-00014fc0: 7269 6e67 3a20 7374 720a 2020 2020 2020  ring: str.      
-00014fd0: 2020 2020 2020 3a70 6172 616d 2074 6963        :param tic
-00014fe0: 6c6f 7564 3a20 7368 6f77 206f 6e6c 7920  loud: show only 
-00014ff0: 636c 6f75 6420 7265 7375 6c74 730a 2020  cloud results.  
-00015000: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
-00015010: 7469 636c 6f75 643a 2062 6f6f 6c0a 2020  ticloud: bool.  
-00015020: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00015030: 206d 6178 5f72 6573 756c 7473 3a20 6d61   max_results: ma
-00015040: 7869 6d75 6d20 7265 7375 6c74 7320 746f  ximum results to
-00015050: 2062 6520 7265 7475 726e 6564 2069 6e20   be returned in 
-00015060: 6120 6c69 7374 3b20 6465 6661 756c 7420  a list; default 
-00015070: 7661 6c75 6520 6973 2035 3030 300a 2020  value is 5000.  
-00015080: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
-00015090: 6d61 785f 7265 7375 6c74 733a 2069 6e74  max_results: int
-000150a0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-000150b0: 7261 6d20 736f 7274 696e 675f 6372 6974  ram sorting_crit
-000150c0: 6572 6961 3a20 6465 6669 6e65 2074 6865  eria: define the
-000150d0: 2063 7269 7465 7269 6120 7573 6564 2069   criteria used i
-000150e0: 6e20 736f 7274 696e 673b 2070 6f73 7369  n sorting; possi
-000150f0: 626c 6520 7661 6c75 6573 2061 7265 2027  ble values are '
-00015100: 7368 6131 272c 2027 6669 7273 7473 6565  sha1', 'firstsee
-00015110: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
-00015120: 2774 6872 6561 746e 616d 6527 2c20 2773  'threatname', 's
-00015130: 616d 706c 6574 7970 6527 2c20 2766 696c  ampletype', 'fil
-00015140: 6563 6f75 6e74 272c 2027 7369 7a65 270a  ecount', 'size'.
-00015150: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
-00015160: 6520 736f 7274 696e 675f 6372 6974 6572  e sorting_criter
-00015170: 6961 3a20 7374 720a 2020 2020 2020 2020  ia: str.        
-00015180: 2020 2020 3a70 6172 616d 2073 6f72 7469      :param sorti
-00015190: 6e67 5f6f 7264 6572 3a20 736f 7274 696e  ng_order: sortin
-000151a0: 6720 6f72 6465 723b 2070 6f73 7369 626c  g order; possibl
-000151b0: 6520 7661 6c75 6573 2061 7265 2027 6465  e values are 'de
-000151c0: 7363 272c 2027 6173 6327 0a20 2020 2020  sc', 'asc'.     
-000151d0: 2020 2020 2020 203a 7479 7065 2073 6f72         :type sor
-000151e0: 7469 6e67 5f6f 7264 6572 3a20 7374 720a  ting_order: str.
-000151f0: 2020 2020 2020 2020 2020 2020 3a72 6574              :ret
-00015200: 7572 6e3a 206c 6973 7420 6f66 2072 6573  urn: list of res
-00015210: 756c 7473 0a20 2020 2020 2020 2020 2020  ults.           
-00015220: 203a 7274 7970 653a 206c 6973 740a 2020   :rtype: list.  
-00015230: 2020 2020 2020 2020 2020 2020 2020 2222                ""
-00015240: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-00015250: 2069 7369 6e73 7461 6e63 6528 6d61 785f   isinstance(max_
-00015260: 7265 7375 6c74 732c 2069 6e74 293a 0a20  results, int):. 
-00015270: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00015280: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
-00015290: 2822 6d61 785f 7265 7375 6c74 7320 7061  ("max_results pa
-000152a0: 7261 6d65 7465 7220 6d75 7374 2062 6520  rameter must be 
-000152b0: 696e 7465 6765 722e 2229 0a0a 2020 2020  integer.")..    
-000152c0: 2020 2020 7265 7375 6c74 7320 3d20 5b5d      results = []
-000152d0: 0a20 2020 2020 2020 206e 6578 745f 7061  .        next_pa
-000152e0: 6765 203d 2031 0a20 2020 2020 2020 206d  ge = 1.        m
-000152f0: 6f72 655f 7061 6765 7320 3d20 5472 7565  ore_pages = True
-00015300: 0a0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
-00015310: 6d6f 7265 5f70 6167 6573 3a0a 2020 2020  more_pages:.    
-00015320: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00015330: 203d 2073 656c 662e 6164 7661 6e63 6564   = self.advanced
-00015340: 5f73 6561 7263 685f 7632 280a 2020 2020  _search_v2(.    
-00015350: 2020 2020 2020 2020 2020 2020 7175 6572              quer
-00015360: 795f 7374 7269 6e67 3d71 7565 7279 5f73  y_string=query_s
-00015370: 7472 696e 672c 0a20 2020 2020 2020 2020  tring,.         
-00015380: 2020 2020 2020 2074 6963 6c6f 7564 3d74         ticloud=t
-00015390: 6963 6c6f 7564 2c0a 2020 2020 2020 2020  icloud,.        
-000153a0: 2020 2020 2020 2020 7061 6765 5f6e 756d          page_num
-000153b0: 6265 723d 6e65 7874 5f70 6167 652c 0a20  ber=next_page,. 
-000153c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000153d0: 6563 6f72 6473 5f70 6572 5f70 6167 653d  ecords_per_page=
-000153e0: 3130 302c 0a20 2020 2020 2020 2020 2020  100,.           
-000153f0: 2020 2020 2073 6f72 7469 6e67 5f63 7269       sorting_cri
-00015400: 7465 7269 613d 736f 7274 696e 675f 6372  teria=sorting_cr
-00015410: 6974 6572 6961 2c0a 2020 2020 2020 2020  iteria,.        
-00015420: 2020 2020 2020 2020 736f 7274 696e 675f          sorting_
-00015430: 6f72 6465 723d 736f 7274 696e 675f 6f72  order=sorting_or
-00015440: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
-00015450: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00015460: 6573 706f 6e73 655f 6a73 6f6e 203d 2072  esponse_json = r
-00015470: 6573 706f 6e73 652e 6a73 6f6e 2829 0a0a  esponse.json()..
-00015480: 2020 2020 2020 2020 2020 2020 656e 7472              entr
-00015490: 6965 7320 3d20 7265 7370 6f6e 7365 5f6a  ies = response_j
-000154a0: 736f 6e2e 6765 7428 2272 6c22 292e 6765  son.get("rl").ge
-000154b0: 7428 2277 6562 5f73 6561 7263 685f 6170  t("web_search_ap
-000154c0: 6922 292e 6765 7428 2265 6e74 7269 6573  i").get("entries
-000154d0: 222c 205b 5d29 0a20 2020 2020 2020 2020  ", []).         
-000154e0: 2020 2072 6573 756c 7473 2e65 7874 656e     results.exten
-000154f0: 6428 656e 7472 6965 7329 0a0a 2020 2020  d(entries)..    
-00015500: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-00015510: 6573 756c 7473 2920 3e20 6d61 785f 7265  esults) > max_re
-00015520: 7375 6c74 733a 0a20 2020 2020 2020 2020  sults:.         
-00015530: 2020 2020 2020 2072 6573 756c 7473 203d         results =
-00015540: 2072 6573 756c 7473 5b3a 6d61 785f 7265   results[:max_re
-00015550: 7375 6c74 735d 0a20 2020 2020 2020 2020  sults].         
-00015560: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00015570: 7375 6c74 730a 0a20 2020 2020 2020 2020  sults..         
-00015580: 2020 206e 6578 745f 7061 6765 203d 2072     next_page = r
-00015590: 6573 706f 6e73 655f 6a73 6f6e 2e67 6574  esponse_json.get
-000155a0: 2822 726c 2229 2e67 6574 2822 7765 625f  ("rl").get("web_
-000155b0: 7365 6172 6368 5f61 7069 2229 2e67 6574  search_api").get
-000155c0: 2822 6e65 7874 5f70 6167 6522 2c20 4e6f  ("next_page", No
-000155d0: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-000155e0: 6d6f 7265 5f70 6167 6573 203d 2072 6573  more_pages = res
-000155f0: 706f 6e73 655f 6a73 6f6e 2e67 6574 2822  ponse_json.get("
-00015600: 726c 2229 2e67 6574 2822 7765 625f 7365  rl").get("web_se
-00015610: 6172 6368 5f61 7069 2229 2e67 6574 2822  arch_api").get("
-00015620: 6d6f 7265 5f70 6167 6573 222c 2046 616c  more_pages", Fal
-00015630: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
-00015640: 7572 6e20 7265 7375 6c74 730a 0a20 2020  urn results..   
-00015650: 2064 6566 206c 6973 745f 636f 6e74 6169   def list_contai
-00015660: 6e65 7273 5f66 6f72 5f68 6173 6865 7328  ners_for_hashes(
-00015670: 7365 6c66 2c20 7361 6d70 6c65 5f68 6173  self, sample_has
-00015680: 6865 7329 3a0a 2020 2020 2020 2020 2222  hes):.        ""
-00015690: 2247 6574 7320 6120 6c69 7374 206f 6620  "Gets a list of 
-000156a0: 616c 6c20 746f 702d 6c65 7665 6c20 636f  all top-level co
-000156b0: 6e74 6169 6e65 7273 2066 726f 6d20 7768  ntainers from wh
-000156c0: 6963 6820 7468 6520 7265 7175 6573 7465  ich the requeste
-000156d0: 6420 7361 6d70 6c65 2068 6173 2062 6565  d sample has bee
-000156e0: 6e20 6578 7472 6163 7465 6420 6475 7269  n extracted duri
-000156f0: 6e67 2061 6e61 6c79 7369 732e 0a20 2020  ng analysis..   
-00015700: 2020 2020 2054 6869 7320 6973 2061 2062       This is a b
-00015710: 756c 6b20 4150 492c 206d 6561 6e69 6e67  ulk API, meaning
-00015720: 2074 6861 7420 6120 7369 6e67 6c65 2072   that a single r
-00015730: 6571 7565 7374 2063 616e 2062 6520 7573  equest can be us
-00015740: 6564 2074 6f20 7369 6d75 6c74 616e 656f  ed to simultaneo
-00015750: 7573 6c79 2071 7565 7279 2063 6f6e 7461  usly query conta
-00015760: 696e 6572 7320 666f 7220 6d75 6c74 6970  iners for multip
-00015770: 6c65 0a20 2020 2020 2020 2066 696c 6520  le.        file 
-00015780: 6861 7368 6573 2e20 4966 2061 2072 6571  hashes. If a req
-00015790: 7565 7374 6564 2068 6173 6820 646f 6573  uested hash does
-000157a0: 6ee2 8099 7420 6861 7665 2061 2063 6f6e  n...t have a con
-000157b0: 7461 696e 6572 2c20 6974 2077 696c 6c20  tainer, it will 
-000157c0: 6e6f 7420 6265 2069 6e63 6c75 6465 6420  not be included 
-000157d0: 696e 2074 6865 2072 6573 706f 6e73 652e  in the response.
-000157e0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-000157f0: 7261 6d20 7361 6d70 6c65 5f68 6173 6865  ram sample_hashe
-00015800: 733a 2061 206c 6973 7420 6f66 206f 6e65  s: a list of one
-00015810: 206f 7220 6d6f 7265 2068 6173 6820 7661   or more hash va
-00015820: 6c75 6573 2c20 6275 7420 6d75 7374 2061  lues, but must a
-00015830: 6c6c 2062 6520 6f66 2074 6865 2073 616d  ll be of the sam
-00015840: 6520 7479 7065 2853 4841 312c 2053 4841  e type(SHA1, SHA
-00015850: 3235 362c 0a20 2020 2020 2020 2020 2020  256,.           
-00015860: 206f 7220 4d44 3529 0a20 2020 2020 2020   or MD5).       
-00015870: 2020 2020 203a 7479 7065 2073 616d 706c       :type sampl
-00015880: 655f 6861 7368 6573 206c 6973 745b 7374  e_hashes list[st
-00015890: 725d 0a20 2020 2020 2020 2020 2020 203a  r].            :
-000158a0: 7265 7475 726e 3a20 7265 7370 6f6e 7365  return: response
-000158b0: 0a20 2020 2020 2020 2020 2020 203a 7274  .            :rt
-000158c0: 7970 653a 2072 6571 7565 7374 732e 5265  ype: requests.Re
-000158d0: 7370 6f6e 7365 0a20 2020 2020 2020 2022  sponse.        "
-000158e0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-000158f0: 7420 6973 696e 7374 616e 6365 2873 616d  t isinstance(sam
-00015900: 706c 655f 6861 7368 6573 2c20 6c69 7374  ple_hashes, list
-00015910: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00015920: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
-00015930: 7272 6f72 2822 7361 6d70 6c65 5f68 6173  rror("sample_has
-00015940: 6865 7320 7061 7261 6d65 7465 7220 6d75  hes parameter mu
-00015950: 7374 2062 6520 6120 6c69 7374 206f 6620  st be a list of 
-00015960: 7374 7269 6e67 732e 2229 0a0a 2020 2020  strings.")..    
-00015970: 2020 2020 7661 6c69 6461 7465 5f68 6173      validate_has
-00015980: 6865 7328 0a20 2020 2020 2020 2020 2020  hes(.           
-00015990: 2068 6173 685f 696e 7075 743d 7361 6d70   hash_input=samp
-000159a0: 6c65 5f68 6173 6865 732c 0a20 2020 2020  le_hashes,.     
-000159b0: 2020 2020 2020 2061 6c6c 6f77 6564 5f68         allowed_h
-000159c0: 6173 685f 7479 7065 733d 284d 4435 2c20  ash_types=(MD5, 
-000159d0: 5348 4131 2c20 5348 4132 3536 290a 2020  SHA1, SHA256).  
-000159e0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000159f0: 2065 6e64 706f 696e 7420 3d20 7365 6c66   endpoint = self
-00015a00: 2e5f 5f4c 4953 545f 434f 4e54 4149 4e45  .__LIST_CONTAINE
-00015a10: 5253 5f45 4e44 504f 494e 540a 0a20 2020  RS_ENDPOINT..   
-00015a20: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
-00015a30: 5f75 726c 2e66 6f72 6d61 7428 656e 6470  _url.format(endp
-00015a40: 6f69 6e74 3d65 6e64 706f 696e 7429 0a0a  oint=endpoint)..
-00015a50: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00015a60: 203d 2073 656c 662e 5f5f 706f 7374 5f72   = self.__post_r
-00015a70: 6571 7565 7374 2875 726c 3d75 726c 2c20  equest(url=url, 
-00015a80: 6461 7461 3d7b 2268 6173 685f 7661 6c75  data={"hash_valu
-00015a90: 6573 223a 2073 616d 706c 655f 6861 7368  es": sample_hash
-00015aa0: 6573 7d29 0a0a 2020 2020 2020 2020 7365  es})..        se
-00015ab0: 6c66 2e5f 5f72 6169 7365 5f6f 6e5f 6572  lf.__raise_on_er
-00015ac0: 726f 7228 7265 7370 6f6e 7365 290a 0a20  ror(response).. 
-00015ad0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00015ae0: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
-00015af0: 6e65 7477 6f72 6b5f 7572 6c5f 7265 706f  network_url_repo
-00015b00: 7274 2873 656c 662c 2072 6571 7565 7374  rt(self, request
-00015b10: 6564 5f75 726c 293a 0a20 2020 2020 2020  ed_url):.       
-00015b20: 2022 2222 4163 6365 7074 7320 6120 5552   """Accepts a UR
-00015b30: 4c20 7374 7269 6e67 2061 6e64 2072 6574  L string and ret
-00015b40: 7572 6e73 2061 2072 6570 6f72 7420 6162  urns a report ab
-00015b50: 6f75 7420 7468 6520 7265 7175 6573 7465  out the requeste
-00015b60: 6420 5552 4c2e 0a20 2020 2020 2020 2020  d URL..         
-00015b70: 2020 203a 7061 7261 6d20 7265 7175 6573     :param reques
-00015b80: 7465 645f 7572 6c3a 2055 524c 2066 6f72  ted_url: URL for
-00015b90: 2061 6e61 6c79 7369 730a 2020 2020 2020   analysis.      
-00015ba0: 2020 2020 2020 3a74 7970 6520 7265 7175        :type requ
-00015bb0: 6573 7465 645f 7572 6c3a 2073 7472 0a20  ested_url: str. 
-00015bc0: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
-00015bd0: 726e 3a20 7265 7370 6f6e 7365 0a20 2020  rn: response.   
-00015be0: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
-00015bf0: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
-00015c00: 7365 0a20 2020 2020 2020 2022 2222 0a0a  se.        """..
-00015c10: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00015c20: 7369 6e73 7461 6e63 6528 7265 7175 6573  sinstance(reques
-00015c30: 7465 645f 7572 6c2c 2073 7472 293a 0a20  ted_url, str):. 
-00015c40: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00015c50: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
-00015c60: 2822 7572 6c20 7061 7261 6d65 7465 7220  ("url parameter 
-00015c70: 6d75 7374 2062 6520 7374 7269 6e67 2e22  must be string."
-00015c80: 290a 0a20 2020 2020 2020 2065 6e63 6f64  )..        encod
-00015c90: 6564 5f75 726c 203d 2070 6172 7365 2e71  ed_url = parse.q
-00015ca0: 756f 7465 5f70 6c75 7328 7265 7175 6573  uote_plus(reques
-00015cb0: 7465 645f 7572 6c29 0a0a 2020 2020 2020  ted_url)..      
-00015cc0: 2020 656e 6470 6f69 6e74 203d 2022 7b65    endpoint = "{e
-00015cd0: 6e64 706f 696e 747d 3f75 726c 3d7b 7572  ndpoint}?url={ur
-00015ce0: 6c7d 222e 666f 726d 6174 280a 2020 2020  l}".format(.    
-00015cf0: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
-00015d00: 3d73 656c 662e 5f5f 5552 4c5f 5245 504f  =self.__URL_REPO
-00015d10: 5254 5f45 4e44 504f 494e 542c 0a20 2020  RT_ENDPOINT,.   
-00015d20: 2020 2020 2020 2020 2075 726c 3d65 6e63           url=enc
-00015d30: 6f64 6564 5f75 726c 0a20 2020 2020 2020  oded_url.       
-00015d40: 2029 0a0a 2020 2020 2020 2020 7572 6c20   )..        url 
-00015d50: 3d20 7365 6c66 2e5f 7572 6c2e 666f 726d  = self._url.form
-00015d60: 6174 2865 6e64 706f 696e 743d 656e 6470  at(endpoint=endp
-00015d70: 6f69 6e74 290a 0a20 2020 2020 2020 2072  oint)..        r
-00015d80: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-00015d90: 5f67 6574 5f72 6571 7565 7374 2875 726c  _get_request(url
-00015da0: 3d75 726c 290a 0a20 2020 2020 2020 2073  =url)..        s
-00015db0: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
-00015dc0: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
-00015dd0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00015de0: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
-00015df0: 206e 6574 776f 726b 5f64 6f6d 6169 6e5f   network_domain_
-00015e00: 7265 706f 7274 2873 656c 662c 2064 6f6d  report(self, dom
-00015e10: 6169 6e29 3a0a 2020 2020 2020 2020 2222  ain):.        ""
-00015e20: 2241 6363 6570 7473 2061 2064 6f6d 6169  "Accepts a domai
-00015e30: 6e20 7374 7269 6e67 2061 6e64 2072 6574  n string and ret
-00015e40: 7572 6e73 2061 2072 6570 6f72 7420 6162  urns a report ab
-00015e50: 6f75 7420 7468 6520 7265 7175 6573 7465  out the requeste
-00015e60: 6420 646f 6d61 696e 2e0a 2020 2020 2020  d domain..      
-00015e70: 2020 2020 2020 3a70 6172 616d 2064 6f6d        :param dom
-00015e80: 6169 6e3a 2064 6f6d 6169 6e20 666f 7220  ain: domain for 
-00015e90: 616e 616c 7973 6973 0a20 2020 2020 2020  analysis.       
-00015ea0: 2020 2020 203a 7479 7065 2064 6f6d 6169       :type domai
-00015eb0: 6e3a 2073 7472 0a20 2020 2020 2020 2020  n: str.         
-00015ec0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
-00015ed0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
-00015ee0: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
-00015ef0: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
-00015f00: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00015f10: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00015f20: 2864 6f6d 6169 6e2c 2073 7472 293a 0a20  (domain, str):. 
-00015f30: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00015f40: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
-00015f50: 2822 646f 6d61 696e 2070 6172 616d 6574  ("domain paramet
-00015f60: 6572 206d 7573 7420 6265 2073 7472 696e  er must be strin
-00015f70: 672e 2229 0a0a 2020 2020 2020 2020 656e  g.")..        en
-00015f80: 6470 6f69 6e74 203d 2073 656c 662e 5f5f  dpoint = self.__
-00015f90: 444f 4d41 494e 5f52 4550 4f52 545f 454e  DOMAIN_REPORT_EN
-00015fa0: 4450 4f49 4e54 2e66 6f72 6d61 7428 646f  DPOINT.format(do
-00015fb0: 6d61 696e 3d64 6f6d 6169 6e29 0a0a 2020  main=domain)..  
-00015fc0: 2020 2020 2020 7572 6c20 3d20 7365 6c66        url = self
-00015fd0: 2e5f 7572 6c2e 666f 726d 6174 2865 6e64  ._url.format(end
-00015fe0: 706f 696e 743d 656e 6470 6f69 6e74 290a  point=endpoint).
-00015ff0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-00016000: 6520 3d20 7365 6c66 2e5f 5f67 6574 5f72  e = self.__get_r
-00016010: 6571 7565 7374 2875 726c 3d75 726c 290a  equest(url=url).
-00016020: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
-00016030: 7261 6973 655f 6f6e 5f65 7272 6f72 2872  raise_on_error(r
-00016040: 6573 706f 6e73 6529 0a0a 2020 2020 2020  esponse)..      
-00016050: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-00016060: 650a 0a20 2020 2064 6566 206e 6574 776f  e..    def netwo
-00016070: 726b 5f69 705f 6164 6472 5f72 6570 6f72  rk_ip_addr_repor
-00016080: 7428 7365 6c66 2c20 6970 5f61 6464 7229  t(self, ip_addr)
-00016090: 3a0a 2020 2020 2020 2020 2222 2241 6363  :.        """Acc
-000160a0: 6570 7473 2061 6e20 4950 2061 6464 7265  epts an IP addre
-000160b0: 7373 2073 7472 696e 6720 616e 6420 7265  ss string and re
-000160c0: 7475 726e 7320 6120 7265 706f 7274 2061  turns a report a
-000160d0: 626f 7574 2074 6865 2072 6571 7565 7374  bout the request
-000160e0: 6564 2049 5020 6164 6472 6573 732e 0a20  ed IP address.. 
-000160f0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00016100: 6d20 6970 5f61 6464 723a 2049 5020 6164  m ip_addr: IP ad
-00016110: 6472 6573 7320 666f 7220 616e 616c 7973  dress for analys
-00016120: 6973 0a20 2020 2020 2020 2020 2020 203a  is.            :
-00016130: 7479 7065 2069 705f 6164 6472 3a20 7374  type ip_addr: st
-00016140: 720a 2020 2020 2020 2020 2020 2020 3a72  r.            :r
-00016150: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
-00016160: 2020 2020 2020 2020 2020 2020 3a72 7479              :rty
-00016170: 7065 3a20 7265 7175 6573 7473 2e52 6573  pe: requests.Res
-00016180: 706f 6e73 650a 2020 2020 2020 2020 2222  ponse.        ""
-00016190: 220a 2020 2020 2020 2020 7265 7370 6f6e  ".        respon
-000161a0: 7365 203d 2073 656c 662e 5f5f 6970 5f61  se = self.__ip_a
-000161b0: 6464 725f 656e 6470 6f69 6e74 7328 0a20  ddr_endpoints(. 
-000161c0: 2020 2020 2020 2020 2020 2069 705f 6164             ip_ad
-000161d0: 6472 3d69 705f 6164 6472 2c0a 2020 2020  dr=ip_addr,.    
-000161e0: 2020 2020 2020 2020 7370 6563 6966 6963          specific
-000161f0: 5f65 6e64 706f 696e 743d 7365 6c66 2e5f  _endpoint=self._
-00016200: 5f49 505f 5245 504f 5254 5f45 4e44 504f  _IP_REPORT_ENDPO
-00016210: 494e 540a 2020 2020 2020 2020 290a 0a20  INT.        ).. 
-00016220: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00016230: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
-00016240: 6e65 7477 6f72 6b5f 6970 5f74 6f5f 646f  network_ip_to_do
-00016250: 6d61 696e 2873 656c 662c 2069 705f 6164  main(self, ip_ad
-00016260: 6472 293a 0a20 2020 2020 2020 2022 2222  dr):.        """
-00016270: 4163 6365 7074 7320 616e 2049 5020 6164  Accepts an IP ad
-00016280: 6472 6573 7320 7374 7269 6e67 2061 6e64  dress string and
-00016290: 2072 6574 7572 6e73 2061 206c 6973 7420   returns a list 
-000162a0: 6f66 2049 502d 746f 2d64 6f6d 6169 6e20  of IP-to-domain 
-000162b0: 6d61 7070 696e 6773 2e0a 2020 2020 2020  mappings..      
-000162c0: 2020 2020 2020 3a70 6172 616d 2069 705f        :param ip_
-000162d0: 6164 6472 3a20 7265 7175 6573 7465 6420  addr: requested 
-000162e0: 4950 2061 6464 7265 7373 0a20 2020 2020  IP address.     
-000162f0: 2020 2020 2020 203a 7479 7065 2069 705f         :type ip_
-00016300: 6164 6472 3a20 7374 720a 2020 2020 2020  addr: str.      
-00016310: 2020 2020 2020 3a72 6574 7572 6e3a 2072        :return: r
-00016320: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-00016330: 2020 2020 3a72 7479 7065 3a20 7265 7175      :rtype: requ
-00016340: 6573 7473 2e52 6573 706f 6e73 650a 2020  ests.Response.  
-00016350: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00016360: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00016370: 662e 5f5f 6970 5f61 6464 725f 656e 6470  f.__ip_addr_endp
-00016380: 6f69 6e74 7328 0a20 2020 2020 2020 2020  oints(.         
-00016390: 2020 2069 705f 6164 6472 3d69 705f 6164     ip_addr=ip_ad
-000163a0: 6472 2c0a 2020 2020 2020 2020 2020 2020  dr,.            
-000163b0: 7370 6563 6966 6963 5f65 6e64 706f 696e  specific_endpoin
-000163c0: 743d 7365 6c66 2e5f 5f49 505f 544f 5f44  t=self.__IP_TO_D
-000163d0: 4f4d 4149 4e5f 454e 4450 4f49 4e54 0a20  OMAIN_ENDPOINT. 
-000163e0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000163f0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-00016400: 650a 0a20 2020 2064 6566 206e 6574 776f  e..    def netwo
-00016410: 726b 5f75 726c 735f 6672 6f6d 5f69 7028  rk_urls_from_ip(
-00016420: 7365 6c66 2c20 6970 5f61 6464 7229 3a0a  self, ip_addr):.
-00016430: 2020 2020 2020 2020 2222 2241 6363 6570          """Accep
-00016440: 7473 2061 6e20 4950 2061 6464 7265 7373  ts an IP address
-00016450: 2073 7472 696e 6720 616e 6420 7265 7475   string and retu
-00016460: 726e 7320 6120 6c69 7374 206f 6620 5552  rns a list of UR
-00016470: 4c73 2068 6f73 7465 6420 6f6e 2074 6865  Ls hosted on the
-00016480: 2072 6571 7565 7374 6564 2049 5020 6164   requested IP ad
-00016490: 6472 6573 732e 0a20 2020 2020 2020 2020  dress..         
-000164a0: 2020 203a 7061 7261 6d20 6970 5f61 6464     :param ip_add
-000164b0: 723a 2072 6571 7565 7374 6564 2049 5020  r: requested IP 
-000164c0: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
-000164d0: 2020 2020 3a74 7970 6520 6970 5f61 6464      :type ip_add
-000164e0: 723a 2073 7472 0a20 2020 2020 2020 2020  r: str.         
-000164f0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
-00016500: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
-00016510: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
-00016520: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
-00016530: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00016540: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-00016550: 5f69 705f 6164 6472 5f65 6e64 706f 696e  _ip_addr_endpoin
-00016560: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
-00016570: 6970 5f61 6464 723d 6970 5f61 6464 722c  ip_addr=ip_addr,
-00016580: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
-00016590: 6369 6669 635f 656e 6470 6f69 6e74 3d73  cific_endpoint=s
-000165a0: 656c 662e 5f5f 5552 4c53 5f46 524f 4d5f  elf.__URLS_FROM_
-000165b0: 4950 5f45 4e44 504f 494e 540a 2020 2020  IP_ENDPOINT.    
-000165c0: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
-000165d0: 6574 7572 6e20 7265 7370 6f6e 7365 0a0a  eturn response..
-000165e0: 2020 2020 6465 6620 6e65 7477 6f72 6b5f      def network_
-000165f0: 6669 6c65 735f 6672 6f6d 5f69 7028 7365  files_from_ip(se
-00016600: 6c66 2c20 6970 5f61 6464 7229 3a0a 2020  lf, ip_addr):.  
-00016610: 2020 2020 2020 2222 2241 6363 6570 7473        """Accepts
-00016620: 2061 6e20 4950 2061 6464 7265 7373 2073   an IP address s
-00016630: 7472 696e 6720 616e 6420 7265 7475 726e  tring and return
-00016640: 7320 6120 6c69 7374 206f 6620 6861 7368  s a list of hash
-00016650: 6573 2061 6e64 0a20 2020 2020 2020 2063  es and.        c
-00016660: 6c61 7373 6966 6963 6174 696f 6e73 2066  lassifications f
-00016670: 6f72 2066 696c 6573 2066 6f75 6e64 206f  or files found o
-00016680: 6e20 7468 6520 7265 7175 6573 7465 6420  n the requested 
-00016690: 4950 2061 6464 7265 7373 2e0a 2020 2020  IP address..    
-000166a0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-000166b0: 705f 6164 6472 3a20 7265 7175 6573 7465  p_addr: requeste
-000166c0: 6420 4950 2061 6464 7265 7373 0a20 2020  d IP address.   
-000166d0: 2020 2020 2020 2020 203a 7479 7065 2069           :type i
-000166e0: 705f 6164 6472 3a20 7374 720a 2020 2020  p_addr: str.    
-000166f0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00016700: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
-00016710: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
-00016720: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
-00016730: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00016740: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-00016750: 656c 662e 5f5f 6970 5f61 6464 725f 656e  elf.__ip_addr_en
-00016760: 6470 6f69 6e74 7328 0a20 2020 2020 2020  dpoints(.       
-00016770: 2020 2020 2069 705f 6164 6472 3d69 705f       ip_addr=ip_
-00016780: 6164 6472 2c0a 2020 2020 2020 2020 2020  addr,.          
-00016790: 2020 7370 6563 6966 6963 5f65 6e64 706f    specific_endpo
-000167a0: 696e 743d 7365 6c66 2e5f 5f46 494c 4553  int=self.__FILES
-000167b0: 5f46 524f 4d5f 4950 5f45 4e44 504f 494e  _FROM_IP_ENDPOIN
-000167c0: 540a 2020 2020 2020 2020 290a 0a20 2020  T.        )..   
-000167d0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
-000167e0: 6f6e 7365 0a0a 2020 2020 6465 6620 5f5f  onse..    def __
-000167f0: 6970 5f61 6464 725f 656e 6470 6f69 6e74  ip_addr_endpoint
-00016800: 7328 7365 6c66 2c20 6970 5f61 6464 722c  s(self, ip_addr,
-00016810: 2073 7065 6369 6669 635f 656e 6470 6f69   specific_endpoi
-00016820: 6e74 293a 0a20 2020 2020 2020 2022 2222  nt):.        """
-00016830: 5072 6976 6174 6520 6d65 7468 6f64 2066  Private method f
-00016840: 6f72 2061 6c6c 2049 5020 7265 6c61 7465  or all IP relate
-00016850: 6420 656e 6470 6f69 6e74 7320 6672 6f6d  d endpoints from
-00016860: 2074 6865 204e 6574 776f 726b 2054 6872   the Network Thr
-00016870: 6561 7420 496e 7465 6c6c 6967 656e 6365  eat Intelligence
-00016880: 2041 5049 2e0a 2020 2020 2020 2020 2020   API..          
-00016890: 2020 3a70 6172 616d 2069 705f 6164 6472    :param ip_addr
-000168a0: 3a20 7265 7175 6573 7465 6420 4950 2061  : requested IP a
-000168b0: 6464 7265 7373 0a20 2020 2020 2020 2020  ddress.         
-000168c0: 2020 203a 7479 7065 2069 705f 6164 6472     :type ip_addr
-000168d0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-000168e0: 2020 3a70 6172 616d 2073 7065 6369 6669    :param specifi
-000168f0: 635f 656e 6470 6f69 6e74 3a20 7265 7175  c_endpoint: requ
-00016900: 6573 7465 6420 656e 6470 6f69 6e74 2073  ested endpoint s
-00016910: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00016920: 2020 3a74 7970 6520 7370 6563 6966 6963    :type specific
-00016930: 5f65 6e64 706f 696e 743a 2073 7472 0a20  _endpoint: str. 
-00016940: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
-00016950: 726e 3a20 7265 7370 6f6e 7365 0a20 2020  rn: response.   
-00016960: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
-00016970: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
-00016980: 7365 0a20 2020 2020 2020 2022 2222 0a20  se.        """. 
-00016990: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-000169a0: 696e 7374 616e 6365 2869 705f 6164 6472  instance(ip_addr
-000169b0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-000169c0: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-000169d0: 6e70 7574 4572 726f 7228 2269 705f 6164  nputError("ip_ad
-000169e0: 6472 2070 6172 616d 6574 6572 206d 7573  dr parameter mus
-000169f0: 7420 6265 2073 7472 696e 672e 2229 0a0a  t be string.")..
-00016a00: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
-00016a10: 203d 2073 7065 6369 6669 635f 656e 6470   = specific_endp
-00016a20: 6f69 6e74 2e66 6f72 6d61 7428 6970 3d69  oint.format(ip=i
-00016a30: 705f 6164 6472 290a 0a20 2020 2020 2020  p_addr)..       
-00016a40: 2075 726c 203d 2073 656c 662e 5f75 726c   url = self._url
-00016a50: 2e66 6f72 6d61 7428 656e 6470 6f69 6e74  .format(endpoint
-00016a60: 3d65 6e64 706f 696e 7429 0a0a 2020 2020  =endpoint)..    
-00016a70: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-00016a80: 656c 662e 5f5f 6765 745f 7265 7175 6573  elf.__get_reques
-00016a90: 7428 7572 6c3d 7572 6c29 0a0a 2020 2020  t(url=url)..    
-00016aa0: 2020 2020 7365 6c66 2e5f 5f72 6169 7365      self.__raise
-00016ab0: 5f6f 6e5f 6572 726f 7228 7265 7370 6f6e  _on_error(respon
-00016ac0: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
-00016ad0: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
-00016ae0: 2020 6465 6620 5f5f 6765 745f 746f 6b65    def __get_toke
-00016af0: 6e28 7365 6c66 2c20 7573 6572 6e61 6d65  n(self, username
-00016b00: 2c20 7061 7373 776f 7264 293a 0a20 2020  , password):.   
-00016b10: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
-00016b20: 616e 206f 6274 6169 6e65 6420 746f 6b65  an obtained toke
-00016b30: 6e20 7573 696e 6720 7468 6520 7072 6f76  n using the prov
-00016b40: 6964 6564 2075 7365 726e 616d 6520 616e  ided username an
-00016b50: 6420 7061 7373 776f 7264 2e0a 2020 2020  d password..    
-00016b60: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00016b70: 2074 6f6b 656e 2073 7472 696e 670a 2020   token string.  
-00016b80: 2020 2020 2020 2020 2020 3a72 7479 7065            :rtype
-00016b90: 3a20 7374 720a 2020 2020 2020 2020 2222  : str.        ""
-00016ba0: 220a 2020 2020 2020 2020 6372 6564 656e  ".        creden
-00016bb0: 7469 616c 7320 3d20 7b22 7573 6572 6e61  tials = {"userna
-00016bc0: 6d65 223a 2075 7365 726e 616d 652c 2022  me": username, "
-00016bd0: 7061 7373 776f 7264 223a 2070 6173 7377  password": passw
-00016be0: 6f72 647d 0a0a 2020 2020 2020 2020 7265  ord}..        re
-00016bf0: 7370 6f6e 7365 203d 2072 6571 7565 7374  sponse = request
-00016c00: 732e 706f 7374 280a 2020 2020 2020 2020  s.post(.        
-00016c10: 2020 2020 7572 6c3d 7365 6c66 2e5f 686f      url=self._ho
-00016c20: 7374 202b 2073 656c 662e 5f5f 544f 4b45  st + self.__TOKE
-00016c30: 4e5f 454e 4450 4f49 4e54 2c0a 2020 2020  N_ENDPOINT,.    
-00016c40: 2020 2020 2020 2020 6461 7461 3d63 7265          data=cre
-00016c50: 6465 6e74 6961 6c73 2c0a 2020 2020 2020  dentials,.      
-00016c60: 2020 2020 2020 7665 7269 6679 3d73 656c        verify=sel
-00016c70: 662e 5f76 6572 6966 792c 0a20 2020 2020  f._verify,.     
-00016c80: 2020 2020 2020 2070 726f 7869 6573 3d73         proxies=s
-00016c90: 656c 662e 5f70 726f 7869 6573 0a20 2020  elf._proxies.   
-00016ca0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00016cb0: 7365 6c66 2e5f 5f72 6169 7365 5f6f 6e5f  self.__raise_on_
-00016cc0: 6572 726f 7228 7265 7370 6f6e 7365 290a  error(response).
-00016cd0: 0a20 2020 2020 2020 2074 6f6b 656e 203d  .        token =
-00016ce0: 2072 6573 706f 6e73 652e 6a73 6f6e 2829   response.json()
-00016cf0: 2e67 6574 2822 746f 6b65 6e22 290a 0a20  .get("token").. 
-00016d00: 2020 2020 2020 2072 6574 7572 6e20 746f         return to
-00016d10: 6b65 6e0a 0a20 2020 2040 7374 6174 6963  ken..    @static
-00016d20: 6d65 7468 6f64 0a20 2020 2064 6566 205f  method.    def _
-00016d30: 5f63 7265 6174 655f 706f 7374 5f70 6179  _create_post_pay
-00016d40: 6c6f 6164 2863 7573 746f 6d5f 6669 6c65  load(custom_file
-00016d50: 6e61 6d65 3d4e 6f6e 652c 2066 696c 655f  name=None, file_
-00016d60: 7572 6c3d 4e6f 6e65 2c20 2063 7261 776c  url=None,  crawl
-00016d70: 6572 3d4e 6f6e 652c 2061 7263 6869 7665  er=None, archive
-00016d80: 5f70 6173 7377 6f72 643d 4e6f 6e65 2c0a  _password=None,.
-00016d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016da0: 2020 2020 2020 2020 2020 2020 2020 726c                rl
-00016db0: 5f63 6c6f 7564 5f73 616e 6462 6f78 5f70  _cloud_sandbox_p
-00016dc0: 6c61 7466 6f72 6d3d 4e6f 6e65 2c20 7461  latform=None, ta
-00016dd0: 6773 3d4e 6f6e 652c 2063 6f6d 6d65 6e74  gs=None, comment
-00016de0: 3d4e 6f6e 652c 2063 6c6f 7564 5f61 6e61  =None, cloud_ana
-00016df0: 6c79 7369 733d 5472 7565 2c0a 2020 2020  lysis=True,.    
-00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e10: 2020 2020 2020 2020 2020 636c 6173 7369            classi
-00016e20: 6669 6361 7469 6f6e 3d4e 6f6e 652c 2072  fication=None, r
-00016e30: 6973 6b5f 7363 6f72 653d 4e6f 6e65 2c20  isk_score=None, 
-00016e40: 7468 7265 6174 5f70 6c61 7466 6f72 6d3d  threat_platform=
-00016e50: 4e6f 6e65 2c20 7468 7265 6174 5f74 7970  None, threat_typ
-00016e60: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
-00016e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e80: 2020 2020 2020 7468 7265 6174 5f6e 616d        threat_nam
-00016e90: 653d 4e6f 6e65 2c20 6e61 6d65 3d4e 6f6e  e=None, name=Non
-00016ea0: 652c 2063 6f6e 7465 6e74 3d4e 6f6e 652c  e, content=None,
-00016eb0: 2070 7562 6c69 7368 3d4e 6f6e 652c 2074   publish=None, t
-00016ec0: 6963 6c6f 7564 3d4e 6f6e 6529 3a0a 2020  icloud=None):.  
-00016ed0: 2020 2020 2020 2222 2241 6363 6570 7473        """Accepts
-00016ee0: 206f 7074 696f 6e61 6c20 6669 656c 6473   optional fields
-00016ef0: 2061 6e64 2072 6574 7572 6e73 2061 2066   and returns a f
-00016f00: 6f72 6d65 6420 6469 6374 696f 6e61 7279  ormed dictionary
-00016f10: 206f 6620 7468 6f73 6520 6669 656c 6473   of those fields
-00016f20: 2e0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
-00016f30: 6172 616d 2063 7573 746f 6d5f 6669 6c65  aram custom_file
-00016f40: 6e61 6d65 3a20 6375 7374 6f6d 2066 696c  name: custom fil
-00016f50: 6520 6e61 6d65 2066 6f72 2075 706c 6f61  e name for uploa
-00016f60: 640a 2020 2020 2020 2020 2020 2020 3a74  d.            :t
-00016f70: 7970 6520 6375 7374 6f6d 5f66 696c 656e  ype custom_filen
-00016f80: 616d 653a 2073 7472 0a20 2020 2020 2020  ame: str.       
-00016f90: 2020 2020 203a 7061 7261 6d20 6669 6c65       :param file
-00016fa0: 5f75 726c 3a20 5552 4c20 6672 6f6d 2077  _url: URL from w
-00016fb0: 6869 6368 2074 6865 2061 7070 6c69 616e  hich the applian
-00016fc0: 6365 2073 686f 756c 6420 646f 776e 6c6f  ce should downlo
-00016fd0: 6164 2074 6865 2064 6174 610a 2020 2020  ad the data.    
-00016fe0: 2020 2020 2020 2020 3a74 7970 6520 6669          :type fi
-00016ff0: 6c65 5f75 726c 3a20 7374 720a 2020 2020  le_url: str.    
-00017000: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-00017010: 7261 776c 6572 3a20 6372 6177 6c65 7220  rawler: crawler 
-00017020: 6d65 7468 6f64 2028 6c6f 6361 6c20 6f72  method (local or
-00017030: 2063 6c6f 7564 290a 2020 2020 2020 2020   cloud).        
-00017040: 2020 2020 3a74 7970 6520 6372 6177 6c65      :type crawle
-00017050: 723a 2073 7472 0a20 2020 2020 2020 2020  r: str.         
-00017060: 2020 203a 7061 7261 6d20 6172 6368 6976     :param archiv
-00017070: 655f 7061 7373 776f 7264 3a20 7061 7373  e_password: pass
-00017080: 776f 7264 2c20 6966 2066 696c 6520 6973  word, if file is
-00017090: 2061 2070 6173 7377 6f72 642d 7072 6f74   a password-prot
-000170a0: 6563 7465 6420 6172 6368 6976 650a 2020  ected archive.  
-000170b0: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
-000170c0: 6172 6368 6976 655f 7061 7373 776f 7264  archive_password
-000170d0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-000170e0: 2020 3a70 6172 616d 2072 6c5f 636c 6f75    :param rl_clou
-000170f0: 645f 7361 6e64 626f 785f 706c 6174 666f  d_sandbox_platfo
-00017100: 726d 3a20 436c 6f75 6420 5361 6e64 626f  rm: Cloud Sandbo
-00017110: 7820 706c 6174 666f 726d 2028 7769 6e64  x platform (wind
-00017120: 6f77 7337 2c20 7769 6e64 6f77 7331 3020  ows7, windows10 
-00017130: 6f72 206d 6163 6f73 5f31 3129 0a20 2020  or macos_11).   
-00017140: 2020 2020 2020 2020 203a 7479 7065 2072           :type r
-00017150: 6c5f 636c 6f75 645f 7361 6e64 626f 785f  l_cloud_sandbox_
-00017160: 706c 6174 666f 726d 3a20 7374 720a 2020  platform: str.  
-00017170: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00017180: 2074 6167 733a 2061 2073 7472 696e 6720   tags: a string 
-00017190: 6f66 2063 6f6d 6d61 2073 6570 6172 6174  of comma separat
-000171a0: 6564 2074 6167 730a 2020 2020 2020 2020  ed tags.        
-000171b0: 2020 2020 3a74 7970 6520 7461 6773 3a20      :type tags: 
-000171c0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-000171d0: 3a70 6172 616d 2063 6f6d 6d65 6e74 3a20  :param comment: 
-000171e0: 636f 6d6d 656e 7420 7374 7269 6e67 0a20  comment string. 
-000171f0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00017200: 2063 6f6d 6d65 6e74 3a20 7374 720a 2020   comment: str.  
-00017210: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00017220: 2063 6c6f 7564 5f61 6e61 6c79 7369 733a   cloud_analysis:
-00017230: 2075 7365 2063 6c6f 7564 2061 6e61 6c79   use cloud analy
-00017240: 7369 730a 2020 2020 2020 2020 2020 2020  sis.            
-00017250: 3a74 7970 6520 636c 6f75 645f 616e 616c  :type cloud_anal
-00017260: 7973 6973 3a20 626f 6f6c 0a20 2020 2020  ysis: bool.     
-00017270: 2020 2020 2020 203a 7061 7261 6d20 636c         :param cl
-00017280: 6173 7369 6669 6361 7469 6f6e 3a20 2767  assification: 'g
-00017290: 6f6f 6477 6172 6527 2c20 2773 7573 7069  oodware', 'suspi
-000172a0: 6369 6f75 7327 206f 7220 276d 616c 6963  cious' or 'malic
-000172b0: 696f 7573 270a 2020 2020 2020 2020 2020  ious'.          
-000172c0: 2020 3a74 7970 6520 636c 6173 7369 6669    :type classifi
-000172d0: 6361 7469 6f6e 3a20 7374 720a 2020 2020  cation: str.    
-000172e0: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
-000172f0: 6973 6b5f 7363 6f72 653a 2049 6620 7370  isk_score: If sp
-00017300: 6563 6966 6965 642c 2069 7420 6d75 7374  ecified, it must
-00017310: 2062 6520 7769 7468 696e 2072 616e 6765   be within range
-00017320: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
-00017330: 6564 2063 6c61 7373 6966 6963 6174 696f  ed classificatio
-00017340: 6e2e 2049 6620 6e6f 7420 7370 6563 6966  n. If not specif
-00017350: 6965 642c 0a20 2020 2020 2020 2020 2020  ied,.           
-00017360: 2061 2064 6566 6175 6c74 2076 616c 7565   a default value
-00017370: 2069 7320 7573 6564 3a20 476f 6f64 7761   is used: Goodwa
-00017380: 7265 3a20 302c 2053 7573 7069 6369 6f75  re: 0, Suspiciou
-00017390: 733a 2036 2c20 4d61 6c69 6369 6f75 733a  s: 6, Malicious:
-000173a0: 2031 300a 2020 2020 2020 2020 2020 2020   10.            
-000173b0: 3a74 7970 6520 7269 736b 5f73 636f 7265  :type risk_score
-000173c0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-000173d0: 2020 3a70 6172 616d 2074 6872 6561 745f    :param threat_
-000173e0: 706c 6174 666f 726d 3a20 6966 2073 7065  platform: if spe
-000173f0: 6369 6669 6564 2c20 6974 206d 7573 7420  cified, it must 
-00017400: 6265 206f 6e20 7468 6520 7375 7070 6f72  be on the suppor
-00017410: 7465 6420 6c69 7374 2028 706c 6174 666f  ted list (platfo
-00017420: 726d 7320 616e 6420 7375 6270 6c61 7466  rms and subplatf
-00017430: 6f72 6d73 202d 2073 6565 0a20 2020 2020  orms - see.     
-00017440: 2020 2020 2020 206f 6666 6963 6961 6c20         official 
-00017450: 4150 4920 646f 6373 292e 2049 6620 6e6f  API docs). If no
-00017460: 7420 7370 6563 6966 6965 642c 2074 6865  t specified, the
-00017470: 2064 6566 6175 6c74 2076 616c 7565 2069   default value i
-00017480: 7320 2757 696e 3332 272e 0a20 2020 2020  s 'Win32'..     
-00017490: 2020 2020 2020 203a 7479 7065 2074 6872         :type thr
-000174a0: 6561 745f 706c 6174 666f 726d 3a20 7374  eat_platform: st
-000174b0: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
-000174c0: 6172 616d 2074 6872 6561 745f 7479 7065  aram threat_type
-000174d0: 3a20 4966 2073 7065 6369 6669 6564 2c20  : If specified, 
-000174e0: 6974 206d 7573 7420 6265 206f 6e20 7468  it must be on th
-000174f0: 6520 7375 7070 6f72 7465 6420 6c69 7374  e supported list
-00017500: 2028 6d61 6c77 6172 6520 7479 7065 7320   (malware types 
-00017510: 2d20 7365 6520 7066 6669 6369 616c 2041  - see pfficial A
-00017520: 5049 2064 6f63 7329 2e0a 2020 2020 2020  PI docs)..      
-00017530: 2020 2020 2020 4966 206e 6f74 2073 7065        If not spe
-00017540: 6369 6669 6564 2c20 7468 6520 6465 6661  cified, the defa
-00017550: 756c 7420 7661 6c75 6520 6973 2027 4d61  ult value is 'Ma
-00017560: 6c77 6172 6527 2e0a 2020 2020 2020 2020  lware'..        
-00017570: 2020 2020 3a74 7970 6520 7468 7265 6174      :type threat
-00017580: 5f74 7970 653a 2073 7472 0a20 2020 2020  _type: str.     
-00017590: 2020 2020 2020 203a 7061 7261 6d20 7468         :param th
-000175a0: 7265 6174 5f6e 616d 653a 2049 6620 7370  reat_name: If sp
-000175b0: 6563 6966 6965 642c 206d 7573 7420 6265  ecified, must be
-000175c0: 2061 6e20 616c 7068 616e 756d 6572 6963   an alphanumeric
-000175d0: 2073 7472 696e 6720 6e6f 7420 6c6f 6e67   string not long
-000175e0: 6572 2074 6861 6e20 3332 2063 6861 7261  er than 32 chara
-000175f0: 6374 6572 732e 2049 6620 6e6f 740a 2020  cters. If not.  
-00017600: 2020 2020 2020 2020 2020 7370 6563 6966            specif
-00017610: 6965 642c 2074 6865 2064 6566 6175 6c74  ied, the default
-00017620: 2076 616c 7565 2069 7320 2747 656e 6572   value is 'Gener
-00017630: 6963 272e 0a20 2020 2020 2020 2020 2020  ic'..           
-00017640: 203a 7479 7065 2074 6872 6561 745f 6e61   :type threat_na
-00017650: 6d65 3a20 7374 720a 2020 2020 2020 2020  me: str.        
-00017660: 2020 2020 3a70 6172 616d 206e 616d 653a      :param name:
-00017670: 206e 616d 6520 6f66 2074 6865 2072 756c   name of the rul
-00017680: 6573 6574 2074 6f20 6372 6561 7465 206f  eset to create o
-00017690: 7220 7570 6461 7465 0a20 2020 2020 2020  r update.       
-000176a0: 2020 2020 203a 7479 7065 206e 616d 653a       :type name:
-000176b0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
-000176c0: 203a 7061 7261 6d20 636f 6e74 656e 743a   :param content:
-000176d0: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
-000176e0: 5941 5241 2072 756c 6573 6574 2074 6f20  YARA ruleset to 
-000176f0: 6372 6561 7465 206f 7220 7570 6461 7465  create or update
-00017700: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
-00017710: 7065 2063 6f6e 7465 6e74 3a20 7374 720a  pe content: str.
-00017720: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00017730: 616d 2070 7562 6c69 7368 3a20 6465 7465  am publish: dete
-00017740: 726d 696e 6573 2077 6865 7468 6572 2074  rmines whether t
-00017750: 6865 2072 756c 6573 6574 2073 686f 756c  he ruleset shoul
-00017760: 6420 6265 2073 796e 6368 726f 6e69 7a65  d be synchronize
-00017770: 6420 746f 206f 7468 6572 2061 7070 6c69  d to other appli
-00017780: 616e 6365 7320 696e 2074 6865 2073 616d  ances in the sam
-00017790: 650a 2020 2020 2020 2020 2020 2020 4331  e.            C1
-000177a0: 3030 3020 636c 7573 7465 720a 2020 2020  000 cluster.    
-000177b0: 2020 2020 2020 2020 3a74 7970 6520 7075          :type pu
-000177c0: 626c 6973 683a 2062 6f6f 6c0a 2020 2020  blish: bool.    
-000177d0: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-000177e0: 6963 6c6f 7564 3a20 6465 7465 726d 696e  icloud: determin
-000177f0: 6573 2077 6865 7468 6572 2074 6865 2072  es whether the r
-00017800: 756c 6573 6574 2073 686f 756c 6420 6265  uleset should be
-00017810: 2073 796e 6368 726f 6e69 7a65 6420 7769   synchronized wi
-00017820: 7468 2054 6974 616e 6975 6d43 6c6f 7564  th TitaniumCloud
-00017830: 206f 7220 6e6f 740a 2020 2020 2020 2020   or not.        
-00017840: 2020 2020 3a74 7970 6520 7469 636c 6f75      :type ticlou
-00017850: 643a 2062 6f6f 6c0a 2020 2020 2020 2020  d: bool.        
-00017860: 2020 2020 3a72 6574 7572 6e3a 2064 6963      :return: dic
-00017870: 7469 6f6e 6172 7920 6f66 2064 6566 696e  tionary of defin
-00017880: 6564 206f 7074 696f 6e61 6c20 6669 656c  ed optional fiel
-00017890: 6473 206f 7220 4e6f 6e65 0a20 2020 2020  ds or None.     
-000178a0: 2020 2020 2020 203a 7274 7970 653a 2064         :rtype: d
-000178b0: 6963 7420 6f72 204e 6f6e 650a 2020 2020  ict or None.    
-000178c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000178d0: 6966 2063 7573 746f 6d5f 6669 6c65 6e61  if custom_filena
-000178e0: 6d65 2061 6e64 206e 6f74 2069 7369 6e73  me and not isins
-000178f0: 7461 6e63 6528 6375 7374 6f6d 5f66 696c  tance(custom_fil
-00017900: 656e 616d 652c 2073 7472 293a 0a20 2020  ename, str):.   
-00017910: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
-00017920: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
-00017930: 6375 7374 6f6d 5f66 696c 656e 616d 6520  custom_filename 
-00017940: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
-00017950: 6520 7374 7269 6e67 2e22 290a 0a20 2020  e string.")..   
-00017960: 2020 2020 2069 6620 7461 6773 2061 6e64       if tags and
-00017970: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00017980: 7461 6773 2c20 7374 7229 3a0a 2020 2020  tags, str):.    
-00017990: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
-000179a0: 6f6e 6749 6e70 7574 4572 726f 7228 2274  ongInputError("t
-000179b0: 6167 7320 7061 7261 6d65 7465 7220 6d75  ags parameter mu
-000179c0: 7374 2062 6520 7374 7269 6e67 2e22 290a  st be string.").
-000179d0: 0a20 2020 2020 2020 2069 6620 6669 6c65  .        if file
-000179e0: 5f75 726c 3a0a 2020 2020 2020 2020 2020  _url:.          
-000179f0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00017a00: 6e63 6528 6669 6c65 5f75 726c 2c20 7374  nce(file_url, st
-00017a10: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00017a20: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00017a30: 6e70 7574 4572 726f 7228 2266 696c 655f  nputError("file_
-00017a40: 7572 6c20 7061 7261 6d65 7465 7220 6d75  url parameter mu
-00017a50: 7374 2062 6520 7374 7269 6e67 2e22 290a  st be string.").
-00017a60: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00017a70: 6f74 2066 696c 655f 7572 6c2e 7374 6172  ot file_url.star
-00017a80: 7473 7769 7468 2828 2268 7474 703a 2f2f  tswith(("http://
-00017a90: 222c 2022 6874 7470 733a 2f2f 2229 293a  ", "https://")):
-00017aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017ab0: 2072 6169 7365 2057 726f 6e67 496e 7075   raise WrongInpu
-00017ac0: 7445 7272 6f72 2822 5375 7070 6f72 7465  tError("Supporte
-00017ad0: 6420 6669 6c65 5f75 726c 2070 726f 746f  d file_url proto
-00017ae0: 636f 6c73 2061 7265 2048 5454 5020 616e  cols are HTTP an
-00017af0: 6420 4854 5450 532e 2229 0a0a 2020 2020  d HTTPS.")..    
-00017b00: 2020 2020 6966 2063 7261 776c 6572 2061      if crawler a
-00017b10: 6e64 2063 7261 776c 6572 206e 6f74 2069  nd crawler not i
-00017b20: 6e20 2822 636c 6f75 6422 2c20 226c 6f63  n ("cloud", "loc
-00017b30: 616c 2229 3a0a 2020 2020 2020 2020 2020  al"):.          
-00017b40: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
-00017b50: 7574 4572 726f 7228 2263 7261 776c 6572  utError("crawler
-00017b60: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
-00017b70: 6265 2065 6974 6865 7220 2763 6c6f 7564  be either 'cloud
-00017b80: 2720 6f72 2027 6c6f 6361 6c27 2e22 290a  ' or 'local'.").
-00017b90: 0a20 2020 2020 2020 2069 6620 6172 6368  .        if arch
-00017ba0: 6976 655f 7061 7373 776f 7264 2061 6e64  ive_password and
-00017bb0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00017bc0: 6172 6368 6976 655f 7061 7373 776f 7264  archive_password
-00017bd0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-00017be0: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00017bf0: 6e70 7574 4572 726f 7228 2261 7263 6869  nputError("archi
-00017c00: 7665 5f70 6173 7377 6f72 6420 7061 7261  ve_password para
-00017c10: 6d65 7465 7220 6d75 7374 2062 6520 7374  meter must be st
-00017c20: 7269 6e67 2e22 290a 0a20 2020 2020 2020  ring.")..       
-00017c30: 2069 6620 726c 5f63 6c6f 7564 5f73 616e   if rl_cloud_san
-00017c40: 6462 6f78 5f70 6c61 7466 6f72 6d20 616e  dbox_platform an
-00017c50: 6420 726c 5f63 6c6f 7564 5f73 616e 6462  d rl_cloud_sandb
-00017c60: 6f78 5f70 6c61 7466 6f72 6d20 6e6f 7420  ox_platform not 
-00017c70: 696e 2041 5641 494c 4142 4c45 5f50 4c41  in AVAILABLE_PLA
-00017c80: 5446 4f52 4d53 3a0a 2020 2020 2020 2020  TFORMS:.        
-00017c90: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00017ca0: 6e70 7574 4572 726f 7228 2272 6c5f 636c  nputError("rl_cl
-00017cb0: 6f75 645f 7361 6e64 626f 785f 706c 6174  oud_sandbox_plat
-00017cc0: 666f 726d 2070 6172 616d 6574 6572 206d  form parameter m
-00017cd0: 7573 7420 6265 206f 6e65 206f 6420 7468  ust be one od th
-00017ce0: 6520 666f 6c6c 6f77 696e 673a 2022 0a20  e following: ". 
-00017cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d10: 2022 7b70 6c61 7466 6f72 6d73 7d22 2e66   "{platforms}".f
-00017d20: 6f72 6d61 7428 706c 6174 666f 726d 733d  ormat(platforms=
-00017d30: 4156 4149 4c41 424c 455f 504c 4154 464f  AVAILABLE_PLATFO
-00017d40: 524d 5329 290a 0a20 2020 2020 2020 2069  RMS))..        i
-00017d50: 6620 636f 6d6d 656e 7420 616e 6420 6e6f  f comment and no
-00017d60: 7420 6973 696e 7374 616e 6365 2863 6f6d  t isinstance(com
-00017d70: 6d65 6e74 2c20 7374 7229 3a0a 2020 2020  ment, str):.    
-00017d80: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
-00017d90: 6f6e 6749 6e70 7574 4572 726f 7228 2263  ongInputError("c
-00017da0: 6f6d 6d65 6e74 2070 6172 616d 6574 6572  omment parameter
-00017db0: 206d 7573 7420 6265 2073 7472 696e 672e   must be string.
-00017dc0: 2229 0a0a 2020 2020 2020 2020 6966 2063  ")..        if c
-00017dd0: 6c6f 7564 5f61 6e61 6c79 7369 7320 6e6f  loud_analysis no
-00017de0: 7420 696e 2028 5472 7565 2c20 4661 6c73  t in (True, Fals
-00017df0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00017e00: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
-00017e10: 4572 726f 7228 2263 6c6f 7564 5f61 6e61  Error("cloud_ana
-00017e20: 6c79 7369 7320 7061 7261 6d65 7465 7220  lysis parameter 
-00017e30: 6d75 7374 2062 6520 626f 6f6c 6561 6e2e  must be boolean.
-00017e40: 2229 0a0a 2020 2020 2020 2020 616c 6c6f  ")..        allo
-00017e50: 7765 645f 636c 6173 7369 6669 6361 7469  wed_classificati
-00017e60: 6f6e 735f 616e 645f 7269 736b 5f73 636f  ons_and_risk_sco
-00017e70: 7265 7320 3d20 7b27 676f 6f64 7761 7265  res = {'goodware
-00017e80: 273a 205b 302c 2031 2c20 322c 2033 2c20  ': [0, 1, 2, 3, 
-00017e90: 342c 2035 5d2c 0a20 2020 2020 2020 2020  4, 5],.         
-00017ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ec0: 2020 2020 2020 2020 2020 2773 7573 7069            'suspi
-00017ed0: 6369 6f75 7327 3a20 5b36 2c20 372c 2038  cious': [6, 7, 8
-00017ee0: 2c20 392c 2031 305d 2c0a 2020 2020 2020  , 9, 10],.      
-00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f10: 2020 2020 2020 2020 2020 2020 2027 6d61               'ma
-00017f20: 6c69 6369 6f75 7327 3a20 5b36 2c20 372c  licious': [6, 7,
-00017f30: 2038 2c20 392c 2031 305d 7d0a 0a20 2020   8, 9, 10]}..   
-00017f40: 2020 2020 2069 6620 636c 6173 7369 6669       if classifi
-00017f50: 6361 7469 6f6e 2061 6e64 2063 6c61 7373  cation and class
-00017f60: 6966 6963 6174 696f 6e20 6e6f 7420 696e  ification not in
-00017f70: 2061 6c6c 6f77 6564 5f63 6c61 7373 6966   allowed_classif
-00017f80: 6963 6174 696f 6e73 5f61 6e64 5f72 6973  ications_and_ris
-00017f90: 6b5f 7363 6f72 6573 2e6b 6579 7328 293a  k_scores.keys():
-00017fa0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00017fb0: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-00017fc0: 6f72 2822 636c 6173 7369 6669 6361 7469  or("classificati
-00017fd0: 6f6e 2070 6172 616d 6574 6572 206d 7573  on parameter mus
-00017fe0: 7420 6265 2073 6f6d 6520 6f66 2074 6865  t be some of the
-00017ff0: 2066 6f6c 6c6f 7769 6e67 2076 616c 7565   following value
-00018000: 733a 2220 2b0a 2020 2020 2020 2020 2020  s:" +.          
-00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018020: 2020 2020 2020 2020 2220 222e 6a6f 696e          " ".join
-00018030: 2873 7472 286b 6579 2920 666f 7220 6b65  (str(key) for ke
-00018040: 7920 696e 2061 6c6c 6f77 6564 5f63 6c61  y in allowed_cla
-00018050: 7373 6966 6963 6174 696f 6e73 5f61 6e64  ssifications_and
-00018060: 5f72 6973 6b5f 7363 6f72 6573 2e6b 6579  _risk_scores.key
-00018070: 7328 2929 290a 2020 2020 2020 2020 656c  s())).        el
-00018080: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00018090: 6966 2072 6973 6b5f 7363 6f72 6520 616e  if risk_score an
-000180a0: 6420 7269 736b 5f73 636f 7265 206e 6f74  d risk_score not
-000180b0: 2069 6e20 616c 6c6f 7765 645f 636c 6173   in allowed_clas
-000180c0: 7369 6669 6361 7469 6f6e 735f 616e 645f  sifications_and_
-000180d0: 7269 736b 5f73 636f 7265 735b 636c 6173  risk_scores[clas
-000180e0: 7369 6669 6361 7469 6f6e 5d3a 0a20 2020  sification]:.   
-000180f0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00018100: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-00018110: 6f72 2866 2272 6973 6b5f 7363 6f72 6520  or(f"risk_score 
-00018120: 7b72 6973 6b5f 7363 6f72 657d 2069 7320  {risk_score} is 
-00018130: 6e6f 7420 616c 6c6f 7765 6420 666f 7220  not allowed for 
-00018140: 636c 6173 7369 6669 6361 7469 6f6e 2027  classification '
-00018150: 7b63 6c61 7373 6966 6963 6174 696f 6e7d  {classification}
-00018160: 272e 2229 0a0a 2020 2020 2020 2020 6966  '.")..        if
-00018170: 2074 6872 6561 745f 706c 6174 666f 726d   threat_platform
-00018180: 2061 6e64 206e 6f74 2069 7369 6e73 7461   and not isinsta
-00018190: 6e63 6528 7468 7265 6174 5f70 6c61 7466  nce(threat_platf
-000181a0: 6f72 6d2c 2073 7472 293a 0a20 2020 2020  orm, str):.     
-000181b0: 2020 2020 2020 2072 6169 7365 2057 726f         raise Wro
-000181c0: 6e67 496e 7075 7445 7272 6f72 2822 7468  ngInputError("th
-000181d0: 7265 6174 5f70 6c61 7466 6f72 6d20 7061  reat_platform pa
-000181e0: 7261 6d65 7465 7220 6d75 7374 2062 6520  rameter must be 
-000181f0: 7374 7269 6e67 2e22 290a 0a20 2020 2020  string.")..     
-00018200: 2020 2069 6620 7468 7265 6174 5f74 7970     if threat_typ
-00018210: 6520 616e 6420 6e6f 7420 6973 696e 7374  e and not isinst
-00018220: 616e 6365 2874 6872 6561 745f 7479 7065  ance(threat_type
-00018230: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-00018240: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
-00018250: 6e70 7574 4572 726f 7228 2274 6872 6561  nputError("threa
-00018260: 745f 7479 7065 2070 6172 616d 6574 6572  t_type parameter
-00018270: 206d 7573 7420 6265 2073 7472 696e 672e   must be string.
-00018280: 2229 0a0a 2020 2020 2020 2020 6966 2074  ")..        if t
-00018290: 6872 6561 745f 6e61 6d65 2061 6e64 206e  hreat_name and n
-000182a0: 6f74 2069 7369 6e73 7461 6e63 6528 7468  ot isinstance(th
-000182b0: 7265 6174 5f6e 616d 652c 2073 7472 293a  reat_name, str):
-000182c0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000182d0: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-000182e0: 6f72 2822 7468 7265 6174 5f74 7970 6520  or("threat_type 
-000182f0: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
-00018300: 6520 7374 7269 6e67 2e22 290a 0a20 2020  e string.")..   
-00018310: 2020 2020 2069 6620 6e61 6d65 2061 6e64       if name and
-00018320: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00018330: 6e61 6d65 2c20 7374 7229 3a0a 2020 2020  name, str):.    
-00018340: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
-00018350: 6f6e 6749 6e70 7574 4572 726f 7228 226e  ongInputError("n
-00018360: 616d 6520 7061 7261 6d65 7465 7220 6d75  ame parameter mu
-00018370: 7374 2062 6520 7374 7269 6e67 2e22 290a  st be string.").
-00018380: 0a20 2020 2020 2020 2069 6620 636f 6e74  .        if cont
-00018390: 656e 7420 616e 6420 6e6f 7420 6973 696e  ent and not isin
-000183a0: 7374 616e 6365 2863 6f6e 7465 6e74 2c20  stance(content, 
-000183b0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-000183c0: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
-000183d0: 7574 4572 726f 7228 2263 6f6e 7465 6e74  utError("content
-000183e0: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
-000183f0: 6265 2073 7472 696e 672e 2229 0a0a 2020  be string.")..  
-00018400: 2020 2020 2020 6966 2070 7562 6c69 7368        if publish
-00018410: 2061 6e64 2070 7562 6c69 7368 206e 6f74   and publish not
-00018420: 2069 6e20 2854 7275 652c 2046 616c 7365   in (True, False
-00018430: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00018440: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
-00018450: 7272 6f72 2822 7075 626c 6973 6820 7061  rror("publish pa
-00018460: 7261 6d65 7465 7220 6d75 7374 2062 6520  rameter must be 
-00018470: 626f 6f6c 6561 6e2e 2229 0a0a 2020 2020  boolean.")..    
-00018480: 2020 2020 6966 2074 6963 6c6f 7564 2061      if ticloud a
-00018490: 6e64 2074 6963 6c6f 7564 206e 6f74 2069  nd ticloud not i
-000184a0: 6e20 2854 7275 652c 2046 616c 7365 293a  n (True, False):
-000184b0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000184c0: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
-000184d0: 6f72 2822 7469 636c 6f75 6420 7061 7261  or("ticloud para
-000184e0: 6d65 7465 7220 6d75 7374 2062 6520 626f  meter must be bo
-000184f0: 6f6c 6561 6e2e 2229 0a0a 2020 2020 2020  olean.")..      
-00018500: 2020 6461 7461 203d 207b 7d0a 0a20 2020    data = {}..   
-00018510: 2020 2020 2069 6620 6375 7374 6f6d 5f66       if custom_f
-00018520: 696c 656e 616d 653a 0a20 2020 2020 2020  ilename:.       
-00018530: 2020 2020 2064 6174 615b 2266 696c 656e       data["filen
-00018540: 616d 6522 5d20 3d20 6375 7374 6f6d 5f66  ame"] = custom_f
-00018550: 696c 656e 616d 650a 0a20 2020 2020 2020  ilename..       
-00018560: 2069 6620 6372 6177 6c65 723a 0a20 2020   if crawler:.   
-00018570: 2020 2020 2020 2020 2064 6174 615b 2263           data["c
-00018580: 7261 776c 6572 225d 203d 2063 7261 776c  rawler"] = crawl
-00018590: 6572 0a0a 2020 2020 2020 2020 6966 2061  er..        if a
-000185a0: 7263 6869 7665 5f70 6173 7377 6f72 643a  rchive_password:
-000185b0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-000185c0: 615b 2261 7263 6869 7665 5f70 6173 7377  a["archive_passw
-000185d0: 6f72 6422 5d20 3d20 6172 6368 6976 655f  ord"] = archive_
-000185e0: 7061 7373 776f 7264 0a0a 2020 2020 2020  password..      
-000185f0: 2020 6966 2072 6c5f 636c 6f75 645f 7361    if rl_cloud_sa
-00018600: 6e64 626f 785f 706c 6174 666f 726d 3a0a  ndbox_platform:.
-00018610: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00018620: 5b22 726c 5f63 6c6f 7564 5f73 616e 6462  ["rl_cloud_sandb
-00018630: 6f78 5f70 6c61 7466 6f72 6d22 5d20 3d20  ox_platform"] = 
-00018640: 726c 5f63 6c6f 7564 5f73 616e 6462 6f78  rl_cloud_sandbox
-00018650: 5f70 6c61 7466 6f72 6d0a 0a20 2020 2020  _platform..     
-00018660: 2020 2069 6620 7461 6773 3a0a 2020 2020     if tags:.    
-00018670: 2020 2020 2020 2020 6461 7461 5b22 7461          data["ta
-00018680: 6773 225d 203d 2074 6167 730a 0a20 2020  gs"] = tags..   
-00018690: 2020 2020 2069 6620 636f 6d6d 656e 743a       if comment:
-000186a0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-000186b0: 615b 2263 6f6d 6d65 6e74 225d 203d 2063  a["comment"] = c
-000186c0: 6f6d 6d65 6e74 0a0a 2020 2020 2020 2020  omment..        
-000186d0: 6966 2063 6c6f 7564 5f61 6e61 6c79 7369  if cloud_analysi
-000186e0: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
-000186f0: 6174 615b 2261 6e61 6c79 7369 7322 5d20  ata["analysis"] 
-00018700: 3d20 2263 6c6f 7564 220a 0a20 2020 2020  = "cloud"..     
-00018710: 2020 2069 6620 6669 6c65 5f75 726c 3a0a     if file_url:.
-00018720: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00018730: 5b22 7572 6c22 5d20 3d20 6669 6c65 5f75  ["url"] = file_u
-00018740: 726c 0a0a 2020 2020 2020 2020 6966 2063  rl..        if c
-00018750: 6c61 7373 6966 6963 6174 696f 6e3a 0a20  lassification:. 
-00018760: 2020 2020 2020 2020 2020 2064 6174 615b             data[
-00018770: 2763 6c61 7373 6966 6963 6174 696f 6e27  'classification'
-00018780: 5d20 3d20 636c 6173 7369 6669 6361 7469  ] = classificati
-00018790: 6f6e 0a0a 2020 2020 2020 2020 6966 2072  on..        if r
-000187a0: 6973 6b5f 7363 6f72 653a 0a20 2020 2020  isk_score:.     
-000187b0: 2020 2020 2020 2064 6174 615b 2772 6973         data['ris
-000187c0: 6b5f 7363 6f72 6527 5d20 3d20 7269 736b  k_score'] = risk
-000187d0: 5f73 636f 7265 0a0a 2020 2020 2020 2020  _score..        
-000187e0: 6966 2074 6872 6561 745f 706c 6174 666f  if threat_platfo
-000187f0: 726d 3a0a 2020 2020 2020 2020 2020 2020  rm:.            
-00018800: 6461 7461 5b27 7468 7265 6174 5f70 6c61  data['threat_pla
-00018810: 7466 6f72 6d27 5d20 3d20 7468 7265 6174  tform'] = threat
-00018820: 5f70 6c61 7466 6f72 6d0a 0a20 2020 2020  _platform..     
-00018830: 2020 2069 6620 7468 7265 6174 5f74 7970     if threat_typ
-00018840: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
-00018850: 6174 615b 2774 6872 6561 745f 7479 7065  ata['threat_type
-00018860: 275d 203d 2074 6872 6561 745f 7479 7065  '] = threat_type
-00018870: 0a0a 2020 2020 2020 2020 6966 2074 6872  ..        if thr
-00018880: 6561 745f 6e61 6d65 3a0a 2020 2020 2020  eat_name:.      
-00018890: 2020 2020 2020 6461 7461 5b27 7468 7265        data['thre
-000188a0: 6174 5f6e 616d 6527 5d20 3d20 7468 7265  at_name'] = thre
-000188b0: 6174 5f6e 616d 650a 0a20 2020 2020 2020  at_name..       
-000188c0: 2069 6620 6e61 6d65 3a0a 2020 2020 2020   if name:.      
-000188d0: 2020 2020 2020 6461 7461 5b27 6e61 6d65        data['name
-000188e0: 275d 203d 206e 616d 650a 0a20 2020 2020  '] = name..     
-000188f0: 2020 2069 6620 636f 6e74 656e 743a 0a20     if content:. 
-00018900: 2020 2020 2020 2020 2020 2064 6174 615b             data[
-00018910: 2763 6f6e 7465 6e74 275d 203d 2063 6f6e  'content'] = con
-00018920: 7465 6e74 0a0a 2020 2020 2020 2020 6966  tent..        if
-00018930: 2070 7562 6c69 7368 3a0a 2020 2020 2020   publish:.      
-00018940: 2020 2020 2020 6461 7461 5b27 7075 626c        data['publ
-00018950: 6973 6827 5d20 3d20 7075 626c 6973 680a  ish'] = publish.
-00018960: 0a20 2020 2020 2020 2069 6620 7469 636c  .        if ticl
-00018970: 6f75 643a 0a20 2020 2020 2020 2020 2020  oud:.           
-00018980: 2064 6174 615b 2774 6963 6c6f 7564 275d   data['ticloud']
-00018990: 203d 2074 6963 6c6f 7564 0a0a 2020 2020   = ticloud..    
-000189a0: 2020 2020 6966 206e 6f74 2064 6174 613a      if not data:
-000189b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000189c0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
-000189d0: 2020 7265 7475 726e 2064 6174 610a 0a20    return data.. 
-000189e0: 2020 2064 6566 205f 5f61 6e61 6c79 7369     def __analysi
-000189f0: 735f 6973 5f66 696e 6973 6865 6428 7365  s_is_finished(se
-00018a00: 6c66 2c20 7361 6d70 6c65 5f68 6173 6865  lf, sample_hashe
-00018a10: 7329 3a0a 2020 2020 2020 2020 2222 2241  s):.        """A
-00018a20: 6363 6570 7473 2061 206c 6973 7420 6f66  ccepts a list of
-00018a30: 2068 6173 6865 7320 616e 6420 7265 7475   hashes and retu
-00018a40: 726e 7320 626f 6f6c 6561 6e20 666f 7220  rns boolean for 
-00018a50: 7468 6520 6765 745f 7265 7375 6c74 7320  the get_results 
-00018a60: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
-00018a70: 2020 2020 3a70 6172 616d 2073 616d 706c      :param sampl
-00018a80: 655f 6861 7368 6573 3a20 6c69 7374 206f  e_hashes: list o
-00018a90: 6620 6861 7368 2073 7472 696e 6773 0a20  f hash strings. 
-00018aa0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00018ab0: 2073 616d 706c 655f 6861 7368 6573 3a20   sample_hashes: 
-00018ac0: 6c69 7374 5b73 7472 5d0a 2020 2020 2020  list[str].      
-00018ad0: 2020 2020 2020 3a72 6574 7572 6e3a 2062        :return: b
-00018ae0: 6f6f 6c65 616e 2066 6f72 2070 726f 6365  oolean for proce
-00018af0: 7373 696e 6720 7374 6174 7573 2e0a 2020  ssing status..  
-00018b00: 2020 2020 2020 2020 2020 3a72 7479 7065            :rtype
-00018b10: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-00018b20: 2222 0a20 2020 2020 2020 2064 6174 6120  "".        data 
-00018b30: 3d20 7b22 6861 7368 5f76 616c 7565 7322  = {"hash_values"
-00018b40: 3a20 7361 6d70 6c65 5f68 6173 6865 737d  : sample_hashes}
-00018b50: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00018b60: 3d20 7b22 7374 6174 7573 223a 2022 7072  = {"status": "pr
-00018b70: 6f63 6573 7365 6422 7d0a 0a20 2020 2020  ocessed"}..     
-00018b80: 2020 2075 726c 203d 2073 656c 662e 5f75     url = self._u
-00018b90: 726c 2e66 6f72 6d61 7428 656e 6470 6f69  rl.format(endpoi
-00018ba0: 6e74 3d73 656c 662e 5f5f 4348 4543 4b5f  nt=self.__CHECK_
-00018bb0: 5354 4154 5553 5f45 4e44 504f 494e 5429  STATUS_ENDPOINT)
-00018bc0: 0a0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-00018bd0: 7365 203d 2073 656c 662e 5f5f 706f 7374  se = self.__post
-00018be0: 5f72 6571 7565 7374 280a 2020 2020 2020  _request(.      
-00018bf0: 2020 2020 2020 7572 6c3d 7572 6c2c 0a20        url=url,. 
-00018c00: 2020 2020 2020 2020 2020 2064 6174 613d             data=
-00018c10: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-00018c20: 2020 7061 7261 6d73 3d70 6172 616d 730a    params=params.
-00018c30: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00018c40: 2020 2073 656c 662e 5f5f 7261 6973 655f     self.__raise_
-00018c50: 6f6e 5f65 7272 6f72 2872 6573 706f 6e73  on_error(respons
-00018c60: 6529 0a0a 2020 2020 2020 2020 6966 206c  e)..        if l
-00018c70: 656e 2872 6573 706f 6e73 652e 6a73 6f6e  en(response.json
-00018c80: 2829 2e67 6574 2822 7265 7375 6c74 7322  ().get("results"
-00018c90: 2929 203d 3d20 6c65 6e28 7361 6d70 6c65  )) == len(sample
-00018ca0: 5f68 6173 6865 7329 3a0a 2020 2020 2020  _hashes):.      
-00018cb0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00018cc0: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
-00018cd0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00018ce0: 205f 5f67 6574 5f72 6571 7565 7374 2873   __get_request(s
-00018cf0: 656c 662c 2075 726c 293a 0a20 2020 2020  elf, url):.     
-00018d00: 2020 2022 2222 4120 6765 6e65 7269 6320     """A generic 
-00018d10: 4745 5420 7265 7175 6573 7420 6d65 7468  GET request meth
-00018d20: 6f64 2066 6f72 2061 6c6c 2041 3130 3030  od for all A1000
-00018d30: 206d 6574 686f 6473 2e0a 2020 2020 2020   methods..      
-00018d40: 2020 2020 2020 3a70 6172 616d 2075 726c        :param url
-00018d50: 3a20 7265 7175 6573 7420 5552 4c0a 2020  : request URL.  
-00018d60: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
-00018d70: 7572 6c3a 2073 7472 0a20 2020 2020 2020  url: str.       
-00018d80: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
-00018d90: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
-00018da0: 2020 203a 7274 7970 653a 2072 6571 7565     :rtype: reque
-00018db0: 7374 732e 5265 7370 6f6e 7365 0a20 2020  sts.Response.   
-00018dc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00018dd0: 2072 6573 706f 6e73 6520 3d20 7265 7175   response = requ
-00018de0: 6573 7473 2e67 6574 280a 2020 2020 2020  ests.get(.      
-00018df0: 2020 2020 2020 7572 6c3d 7572 6c2c 0a20        url=url,. 
-00018e00: 2020 2020 2020 2020 2020 2076 6572 6966             verif
-00018e10: 793d 7365 6c66 2e5f 7665 7269 6679 2c0a  y=self._verify,.
-00018e20: 2020 2020 2020 2020 2020 2020 7072 6f78              prox
-00018e30: 6965 733d 7365 6c66 2e5f 7072 6f78 6965  ies=self._proxie
-00018e40: 732c 0a20 2020 2020 2020 2020 2020 2068  s,.            h
-00018e50: 6561 6465 7273 3d73 656c 662e 5f68 6561  eaders=self._hea
-00018e60: 6465 7273 0a20 2020 2020 2020 2029 0a0a  ders.        )..
-00018e70: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00018e80: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
-00018e90: 205f 5f70 6f73 745f 7265 7175 6573 7428   __post_request(
-00018ea0: 7365 6c66 2c20 7572 6c2c 2070 6f73 745f  self, url, post_
-00018eb0: 6a73 6f6e 3d4e 6f6e 652c 2066 696c 6573  json=None, files
-00018ec0: 3d4e 6f6e 652c 2064 6174 613d 4e6f 6e65  =None, data=None
-00018ed0: 2c20 7061 7261 6d73 3d4e 6f6e 6529 3a0a  , params=None):.
-00018ee0: 2020 2020 2020 2020 2222 2241 2067 656e          """A gen
-00018ef0: 6572 6963 2050 4f53 5420 7265 7175 6573  eric POST reques
-00018f00: 7420 6d65 7468 6f64 2066 6f72 2061 6c6c  t method for all
-00018f10: 2041 3130 3030 206d 6574 686f 6473 2e0a   A1000 methods..
-00018f20: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00018f30: 616d 2075 726c 3a20 7265 7175 6573 7420  am url: request 
-00018f40: 5552 4c0a 2020 2020 2020 2020 2020 2020  URL.            
-00018f50: 3a74 7970 6520 7572 6c3a 2073 7472 0a20  :type url: str. 
-00018f60: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00018f70: 6d20 706f 7374 5f6a 736f 6e3a 204a 534f  m post_json: JSO
-00018f80: 4e20 626f 6479 0a20 2020 2020 2020 2020  N body.         
-00018f90: 2020 203a 7479 7065 2070 6f73 745f 6a73     :type post_js
-00018fa0: 6f6e 3a20 6469 6374 0a20 2020 2020 2020  on: dict.       
-00018fb0: 2020 2020 203a 7061 7261 6d20 6669 6c65       :param file
-00018fc0: 733a 2066 696c 6573 2074 6f20 7365 6e64  s: files to send
-00018fd0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
-00018fe0: 7261 6d20 6461 7461 3a20 6461 7461 2074  ram data: data t
-00018ff0: 6f20 7365 6e64 0a20 2020 2020 2020 2020  o send.         
-00019000: 2020 203a 7061 7261 6d20 7061 7261 6d73     :param params
-00019010: 3a20 6164 6469 7469 6f6e 616c 2070 6172  : additional par
-00019020: 616d 7320 746f 2073 656e 640a 2020 2020  ams to send.    
-00019030: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00019040: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
-00019050: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
-00019060: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
-00019070: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00019080: 2020 2020 7265 7370 6f6e 7365 203d 2072      response = r
-00019090: 6571 7565 7374 732e 706f 7374 280a 2020  equests.post(.  
-000190a0: 2020 2020 2020 2020 2020 7572 6c3d 7572            url=ur
-000190b0: 6c2c 0a20 2020 2020 2020 2020 2020 206a  l,.            j
-000190c0: 736f 6e3d 706f 7374 5f6a 736f 6e2c 0a20  son=post_json,. 
-000190d0: 2020 2020 2020 2020 2020 2066 696c 6573             files
-000190e0: 3d66 696c 6573 2c0a 2020 2020 2020 2020  =files,.        
-000190f0: 2020 2020 6461 7461 3d64 6174 612c 0a20      data=data,. 
-00019100: 2020 2020 2020 2020 2020 2070 6172 616d             param
-00019110: 733d 7061 7261 6d73 2c0a 2020 2020 2020  s=params,.      
-00019120: 2020 2020 2020 7665 7269 6679 3d73 656c        verify=sel
-00019130: 662e 5f76 6572 6966 792c 0a20 2020 2020  f._verify,.     
-00019140: 2020 2020 2020 2070 726f 7869 6573 3d73         proxies=s
-00019150: 656c 662e 5f70 726f 7869 6573 2c0a 2020  elf._proxies,.  
-00019160: 2020 2020 2020 2020 2020 6865 6164 6572            header
-00019170: 733d 7365 6c66 2e5f 6865 6164 6572 730a  s=self._headers.
-00019180: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00019190: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-000191a0: 7365 0a0a 2020 2020 6465 6620 5f5f 6465  se..    def __de
-000191b0: 6c65 7465 5f72 6571 7565 7374 2873 656c  lete_request(sel
-000191c0: 662c 2075 726c 2c20 706f 7374 5f6a 736f  f, url, post_jso
-000191d0: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
-000191e0: 2022 2222 4120 6765 6e65 7269 6320 4445   """A generic DE
-000191f0: 4c45 5445 2072 6571 7565 7374 206d 6574  LETE request met
-00019200: 686f 6420 666f 7220 616c 6c20 4131 3030  hod for all A100
-00019210: 3020 6d65 7468 6f64 732e 0a20 2020 2020  0 methods..     
-00019220: 2020 203a 7061 7261 6d20 7572 6c3a 2072     :param url: r
-00019230: 6571 7565 7374 2055 524c 0a20 2020 2020  equest URL.     
-00019240: 2020 203a 7479 7065 2075 726c 3a20 7374     :type url: st
-00019250: 720a 2020 2020 2020 2020 3a72 6574 7572  r.        :retur
-00019260: 6e3a 2072 6573 706f 6e73 650a 2020 2020  n: response.    
-00019270: 2020 2020 3a72 7479 7065 3a20 7265 7175      :rtype: requ
-00019280: 6573 7473 2e52 6573 706f 6e73 650a 2020  ests.Response.  
-00019290: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000192a0: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
-000192b0: 7565 7374 732e 6465 6c65 7465 280a 2020  uests.delete(.  
-000192c0: 2020 2020 2020 2020 2020 7572 6c3d 7572            url=ur
-000192d0: 6c2c 0a20 2020 2020 2020 2020 2020 206a  l,.            j
-000192e0: 736f 6e3d 706f 7374 5f6a 736f 6e2c 0a20  son=post_json,. 
-000192f0: 2020 2020 2020 2020 2020 2076 6572 6966             verif
-00019300: 793d 7365 6c66 2e5f 7665 7269 6679 2c0a  y=self._verify,.
-00019310: 2020 2020 2020 2020 2020 2020 7072 6f78              prox
-00019320: 6965 733d 7365 6c66 2e5f 7072 6f78 6965  ies=self._proxie
-00019330: 732c 0a20 2020 2020 2020 2020 2020 2068  s,.            h
-00019340: 6561 6465 7273 3d73 656c 662e 5f68 6561  eaders=self._hea
-00019350: 6465 7273 0a20 2020 2020 2020 2029 0a0a  ders.        )..
-00019360: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00019370: 6573 706f 6e73 650a 0a20 2020 2040 7374  esponse..    @st
-00019380: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00019390: 6566 205f 5f72 6169 7365 5f6f 6e5f 6572  ef __raise_on_er
-000193a0: 726f 7228 7265 7370 6f6e 7365 293a 0a20  ror(response):. 
-000193b0: 2020 2020 2020 2022 2222 4163 6365 7074         """Accept
-000193c0: 7320 6120 7265 7370 6f6e 7365 206f 626a  s a response obj
-000193d0: 6563 7420 666f 7220 7661 6c69 6461 7469  ect for validati
-000193e0: 6f6e 2061 6e64 2072 6169 7365 7320 616e  on and raises an
-000193f0: 2065 7863 6570 7469 6f6e 2069 6620 616e   exception if an
-00019400: 2065 7272 6f72 2073 7461 7475 7320 636f   error status co
-00019410: 6465 2069 7320 7265 6365 6976 6564 2e0a  de is received..
-00019420: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
-00019430: 616d 2072 6573 706f 6e73 653a 2072 6573  am response: res
-00019440: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
-00019450: 2020 2020 2020 2020 203a 7479 7065 2072           :type r
-00019460: 6573 706f 6e73 653a 2072 6571 7565 7374  esponse: request
-00019470: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
-00019480: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
-00019490: 7863 6570 7469 6f6e 203d 2052 4553 504f  xception = RESPO
-000194a0: 4e53 455f 434f 4445 5f45 5252 4f52 5f4d  NSE_CODE_ERROR_M
-000194b0: 4150 2e67 6574 2872 6573 706f 6e73 652e  AP.get(response.
-000194c0: 7374 6174 7573 5f63 6f64 652c 204e 6f6e  status_code, Non
-000194d0: 6529 0a20 2020 2020 2020 2069 6620 6e6f  e).        if no
-000194e0: 7420 6578 6365 7074 696f 6e3a 0a20 2020  t exception:.   
-000194f0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00019500: 2020 2020 2020 2020 7261 6973 6520 6578          raise ex
-00019510: 6365 7074 696f 6e0a                      ception.
+00014ab0: 2020 2020 2020 2020 2020 6372 6974 6572            criter
+00014ac0: 6961 3d41 4456 414e 4345 445f 5345 4152  ia=ADVANCED_SEAR
+00014ad0: 4348 5f53 4f52 5449 4e47 5f43 5249 5445  CH_SORTING_CRITE
+00014ae0: 5249 410a 2020 2020 2020 2020 2020 2020  RIA.            
+00014af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b00: 2020 2020 2020 2020 2020 2929 0a20 2020            )).   
+00014b10: 2020 2020 2020 2020 2073 6f72 7469 6e67           sorting
+00014b20: 5f65 7870 7265 7373 696f 6e20 3d20 227b  _expression = "{
+00014b30: 6372 6974 6572 6961 7d20 7b6f 7264 6572  criteria} {order
+00014b40: 7d22 2e66 6f72 6d61 7428 0a20 2020 2020  }".format(.     
+00014b50: 2020 2020 2020 2020 2020 2063 7269 7465             crite
+00014b60: 7269 613d 736f 7274 696e 675f 6372 6974  ria=sorting_crit
+00014b70: 6572 6961 2c0a 2020 2020 2020 2020 2020  eria,.          
+00014b80: 2020 2020 2020 6f72 6465 723d 736f 7274        order=sort
+00014b90: 696e 675f 6f72 6465 720a 2020 2020 2020  ing_order.      
+00014ba0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00014bb0: 2020 2020 2070 6f73 745f 6a73 6f6e 5b22       post_json["
+00014bc0: 736f 7274 225d 203d 2073 6f72 7469 6e67  sort"] = sorting
+00014bd0: 5f65 7870 7265 7373 696f 6e0a 0a20 2020  _expression..   
+00014be0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+00014bf0: 7365 6c66 2e5f 5f70 6f73 745f 7265 7175  self.__post_requ
+00014c00: 6573 7428 7572 6c3d 7572 6c2c 2070 6f73  est(url=url, pos
+00014c10: 745f 6a73 6f6e 3d70 6f73 745f 6a73 6f6e  t_json=post_json
+00014c20: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00014c30: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
+00014c40: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+00014c50: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00014c60: 6e73 650a 0a20 2020 2064 6566 2061 6476  nse..    def adv
+00014c70: 616e 6365 645f 7365 6172 6368 5f76 325f  anced_search_v2_
+00014c80: 6167 6772 6567 6174 6564 2873 656c 662c  aggregated(self,
+00014c90: 2020 7175 6572 795f 7374 7269 6e67 2c20    query_string, 
+00014ca0: 7469 636c 6f75 643d 4661 6c73 652c 206d  ticloud=False, m
+00014cb0: 6178 5f72 6573 756c 7473 3d35 3030 302c  ax_results=5000,
+00014cc0: 2073 6f72 7469 6e67 5f63 7269 7465 7269   sorting_criteri
+00014cd0: 613d 4e6f 6e65 2c0a 2020 2020 2020 2020  a=None,.        
+00014ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cf0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00014d00: 7274 696e 675f 6f72 6465 723d 2264 6573  rting_order="des
+00014d10: 6322 293a 0a20 2020 2020 2020 2022 2222  c"):.        """
+00014d20: 5365 6e64 7320 6120 7175 6572 7920 7374  Sends a query st
+00014d30: 7269 6e67 2074 6f20 7468 6520 4131 3030  ring to the A100
+00014d40: 3020 4164 7661 6e63 6564 2053 6561 7263  0 Advanced Searc
+00014d50: 6820 4150 4920 7632 2e0a 2020 2020 2020  h API v2..      
+00014d60: 2020 5468 6520 7175 6572 7920 7374 7269    The query stri
+00014d70: 6e67 206d 7573 7420 6265 2063 6f6d 706f  ng must be compo
+00014d80: 7365 6420 6f66 206b 6579 2d76 616c 7565  sed of key-value
+00014d90: 2070 6169 7273 2073 6570 6172 6174 6564   pairs separated
+00014da0: 2062 7920 7370 6163 652e 0a20 2020 2020   by space..     
+00014db0: 2020 2041 206b 6579 2069 7320 7365 7061     A key is sepa
+00014dc0: 7261 7465 6420 6672 6f6d 2069 7473 2076  rated from its v
+00014dd0: 616c 7565 2062 7920 6120 636f 6c6f 6e20  alue by a colon 
+00014de0: 7379 6d62 6f6c 2061 6e64 206e 6f20 7370  symbol and no sp
+00014df0: 6163 6573 2e0a 2020 2020 2020 2020 466f  aces..        Fo
+00014e00: 7220 6469 7265 6374 696f 6e73 206f 6e20  r directions on 
+00014e10: 686f 7720 746f 2077 7269 7465 2061 6476  how to write adv
+00014e20: 616e 6365 6420 7365 6172 6368 2071 7565  anced search que
+00014e30: 7269 6573 2c20 636f 6e73 756c 7420 7468  ries, consult th
+00014e40: 6520 4131 3030 3020 646f 6375 6d65 6e74  e A1000 document
+00014e50: 6174 696f 6e2e 0a20 2020 2020 2020 2050  ation..        P
+00014e60: 6167 696e 6720 6973 2064 6f6e 6520 6175  aging is done au
+00014e70: 746f 6d61 7469 6361 6c6c 7920 616e 6420  tomatically and 
+00014e80: 7265 7375 6c74 7320 6672 6f6d 2069 6e64  results from ind
+00014e90: 6976 6964 7561 6c0a 2020 2020 2020 2020  ividual.        
+00014ea0: 7265 7370 6f6e 7365 7320 6167 6772 6567  responses aggreg
+00014eb0: 6174 6564 2069 6e74 6f20 6f6e 6520 6c69  ated into one li
+00014ec0: 7374 2061 6e64 2072 6574 7572 6e65 6460  st and returned`
+00014ed0: 2e0a 2020 2020 2020 2020 5468 6520 276d  ..        The 'm
+00014ee0: 6178 5f72 6573 756c 7473 2720 7061 7261  ax_results' para
+00014ef0: 6d65 7465 7220 6465 6669 6e65 7320 7468  meter defines th
+00014f00: 6520 6d61 7869 6d75 6d20 6465 7369 7265  e maximum desire
+00014f10: 6420 6e75 6d62 6572 206f 6620 7265 7375  d number of resu
+00014f20: 6c74 7320 746f 2062 6520 7265 7475 726e  lts to be return
+00014f30: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00014f40: 5175 6572 7920 7374 7269 6e67 2065 7861  Query string exa
+00014f50: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
+00014f60: 2020 2761 762d 636f 756e 743a 3520 6176    'av-count:5 av
+00014f70: 6169 6c61 626c 653a 5452 5545 270a 0a20  ailable:TRUE'.. 
+00014f80: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00014f90: 6d20 7175 6572 795f 7374 7269 6e67 3a20  m query_string: 
+00014fa0: 7365 6172 6368 2071 7565 7279 202d 2073  search query - s
+00014fb0: 6565 2041 5049 2064 6f63 756d 656e 7461  ee API documenta
+00014fc0: 7469 6f6e 2066 6f72 2064 6574 6169 6c73  tion for details
+00014fd0: 206f 6e20 7772 6974 696e 6720 7365 6172   on writing sear
+00014fe0: 6368 2071 7565 7269 6573 0a20 2020 2020  ch queries.     
+00014ff0: 2020 2020 2020 203a 7479 7065 2071 7565         :type que
+00015000: 7279 5f73 7472 696e 673a 2073 7472 0a20  ry_string: str. 
+00015010: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00015020: 6d20 7469 636c 6f75 643a 2073 686f 7720  m ticloud: show 
+00015030: 6f6e 6c79 2063 6c6f 7564 2072 6573 756c  only cloud resul
+00015040: 7473 0a20 2020 2020 2020 2020 2020 203a  ts.            :
+00015050: 7479 7065 2074 6963 6c6f 7564 3a20 626f  type ticloud: bo
+00015060: 6f6c 0a20 2020 2020 2020 2020 2020 203a  ol.            :
+00015070: 7061 7261 6d20 6d61 785f 7265 7375 6c74  param max_result
+00015080: 733a 206d 6178 696d 756d 2072 6573 756c  s: maximum resul
+00015090: 7473 2074 6f20 6265 2072 6574 7572 6e65  ts to be returne
+000150a0: 6420 696e 2061 206c 6973 743b 2064 6566  d in a list; def
+000150b0: 6175 6c74 2076 616c 7565 2069 7320 3530  ault value is 50
+000150c0: 3030 0a20 2020 2020 2020 2020 2020 203a  00.            :
+000150d0: 7479 7065 206d 6178 5f72 6573 756c 7473  type max_results
+000150e0: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
+000150f0: 2020 3a70 6172 616d 2073 6f72 7469 6e67    :param sorting
+00015100: 5f63 7269 7465 7269 613a 2064 6566 696e  _criteria: defin
+00015110: 6520 7468 6520 6372 6974 6572 6961 2075  e the criteria u
+00015120: 7365 6420 696e 2073 6f72 7469 6e67 3b20  sed in sorting; 
+00015130: 706f 7373 6962 6c65 2076 616c 7565 7320  possible values 
+00015140: 6172 6520 2773 6861 3127 2c20 2766 6972  are 'sha1', 'fir
+00015150: 7374 7365 656e 272c 0a20 2020 2020 2020  stseen',.       
+00015160: 2020 2020 2027 7468 7265 6174 6e61 6d65       'threatname
+00015170: 272c 2027 7361 6d70 6c65 7479 7065 272c  ', 'sampletype',
+00015180: 2027 6669 6c65 636f 756e 7427 2c20 2773   'filecount', 's
+00015190: 697a 6527 0a20 2020 2020 2020 2020 2020  ize'.           
+000151a0: 203a 7479 7065 2073 6f72 7469 6e67 5f63   :type sorting_c
+000151b0: 7269 7465 7269 613a 2073 7472 0a20 2020  riteria: str.   
+000151c0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+000151d0: 736f 7274 696e 675f 6f72 6465 723a 2073  sorting_order: s
+000151e0: 6f72 7469 6e67 206f 7264 6572 3b20 706f  orting order; po
+000151f0: 7373 6962 6c65 2076 616c 7565 7320 6172  ssible values ar
+00015200: 6520 2764 6573 6327 2c20 2761 7363 270a  e 'desc', 'asc'.
+00015210: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+00015220: 6520 736f 7274 696e 675f 6f72 6465 723a  e sorting_order:
+00015230: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+00015240: 203a 7265 7475 726e 3a20 6c69 7374 206f   :return: list o
+00015250: 6620 7265 7375 6c74 730a 2020 2020 2020  f results.      
+00015260: 2020 2020 2020 3a72 7479 7065 3a20 6c69        :rtype: li
+00015270: 7374 0a20 2020 2020 2020 2020 2020 2020  st.             
+00015280: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00015290: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+000152a0: 286d 6178 5f72 6573 756c 7473 2c20 696e  (max_results, in
+000152b0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000152c0: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
+000152d0: 4572 726f 7228 226d 6178 5f72 6573 756c  Error("max_resul
+000152e0: 7473 2070 6172 616d 6574 6572 206d 7573  ts parameter mus
+000152f0: 7420 6265 2069 6e74 6567 6572 2e22 290a  t be integer.").
+00015300: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+00015310: 203d 205b 5d0a 2020 2020 2020 2020 6e65   = [].        ne
+00015320: 7874 5f70 6167 6520 3d20 310a 2020 2020  xt_page = 1.    
+00015330: 2020 2020 6d6f 7265 5f70 6167 6573 203d      more_pages =
+00015340: 2054 7275 650a 0a20 2020 2020 2020 2077   True..        w
+00015350: 6869 6c65 206d 6f72 655f 7061 6765 733a  hile more_pages:
+00015360: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00015370: 706f 6e73 6520 3d20 7365 6c66 2e61 6476  ponse = self.adv
+00015380: 616e 6365 645f 7365 6172 6368 5f76 3228  anced_search_v2(
+00015390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000153a0: 2071 7565 7279 5f73 7472 696e 673d 7175   query_string=qu
+000153b0: 6572 795f 7374 7269 6e67 2c0a 2020 2020  ery_string,.    
+000153c0: 2020 2020 2020 2020 2020 2020 7469 636c              ticl
+000153d0: 6f75 643d 7469 636c 6f75 642c 0a20 2020  oud=ticloud,.   
+000153e0: 2020 2020 2020 2020 2020 2020 2070 6167               pag
+000153f0: 655f 6e75 6d62 6572 3d6e 6578 745f 7061  e_number=next_pa
+00015400: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
+00015410: 2020 2020 7265 636f 7264 735f 7065 725f      records_per_
+00015420: 7061 6765 3d31 3030 2c0a 2020 2020 2020  page=100,.      
+00015430: 2020 2020 2020 2020 2020 736f 7274 696e            sortin
+00015440: 675f 6372 6974 6572 6961 3d73 6f72 7469  g_criteria=sorti
+00015450: 6e67 5f63 7269 7465 7269 612c 0a20 2020  ng_criteria,.   
+00015460: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
+00015470: 7469 6e67 5f6f 7264 6572 3d73 6f72 7469  ting_order=sorti
+00015480: 6e67 5f6f 7264 6572 0a20 2020 2020 2020  ng_order.       
+00015490: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000154a0: 2020 2020 7265 7370 6f6e 7365 5f6a 736f      response_jso
+000154b0: 6e20 3d20 7265 7370 6f6e 7365 2e6a 736f  n = response.jso
+000154c0: 6e28 290a 0a20 2020 2020 2020 2020 2020  n()..           
+000154d0: 2065 6e74 7269 6573 203d 2072 6573 706f   entries = respo
+000154e0: 6e73 655f 6a73 6f6e 2e67 6574 2822 726c  nse_json.get("rl
+000154f0: 2229 2e67 6574 2822 7765 625f 7365 6172  ").get("web_sear
+00015500: 6368 5f61 7069 2229 2e67 6574 2822 656e  ch_api").get("en
+00015510: 7472 6965 7322 2c20 5b5d 290a 2020 2020  tries", []).    
+00015520: 2020 2020 2020 2020 7265 7375 6c74 732e          results.
+00015530: 6578 7465 6e64 2865 6e74 7269 6573 290a  extend(entries).
+00015540: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00015550: 6c65 6e28 7265 7375 6c74 7329 203e 206d  len(results) > m
+00015560: 6178 5f72 6573 756c 7473 3a0a 2020 2020  ax_results:.    
+00015570: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00015580: 6c74 7320 3d20 7265 7375 6c74 735b 3a6d  lts = results[:m
+00015590: 6178 5f72 6573 756c 7473 5d0a 2020 2020  ax_results].    
+000155a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000155b0: 726e 2072 6573 756c 7473 0a0a 2020 2020  rn results..    
+000155c0: 2020 2020 2020 2020 6e65 7874 5f70 6167          next_pag
+000155d0: 6520 3d20 7265 7370 6f6e 7365 5f6a 736f  e = response_jso
+000155e0: 6e2e 6765 7428 2272 6c22 292e 6765 7428  n.get("rl").get(
+000155f0: 2277 6562 5f73 6561 7263 685f 6170 6922  "web_search_api"
+00015600: 292e 6765 7428 226e 6578 745f 7061 6765  ).get("next_page
+00015610: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
+00015620: 2020 2020 206d 6f72 655f 7061 6765 7320       more_pages 
+00015630: 3d20 7265 7370 6f6e 7365 5f6a 736f 6e2e  = response_json.
+00015640: 6765 7428 2272 6c22 292e 6765 7428 2277  get("rl").get("w
+00015650: 6562 5f73 6561 7263 685f 6170 6922 292e  eb_search_api").
+00015660: 6765 7428 226d 6f72 655f 7061 6765 7322  get("more_pages"
+00015670: 2c20 4661 6c73 6529 0a0a 2020 2020 2020  , False)..      
+00015680: 2020 7265 7475 726e 2072 6573 756c 7473    return results
+00015690: 0a0a 2020 2020 6465 6620 6c69 7374 5f63  ..    def list_c
+000156a0: 6f6e 7461 696e 6572 735f 666f 725f 6861  ontainers_for_ha
+000156b0: 7368 6573 2873 656c 662c 2073 616d 706c  shes(self, sampl
+000156c0: 655f 6861 7368 6573 293a 0a20 2020 2020  e_hashes):.     
+000156d0: 2020 2022 2222 4765 7473 2061 206c 6973     """Gets a lis
+000156e0: 7420 6f66 2061 6c6c 2074 6f70 2d6c 6576  t of all top-lev
+000156f0: 656c 2063 6f6e 7461 696e 6572 7320 6672  el containers fr
+00015700: 6f6d 2077 6869 6368 2074 6865 2072 6571  om which the req
+00015710: 7565 7374 6564 2073 616d 706c 6520 6861  uested sample ha
+00015720: 7320 6265 656e 2065 7874 7261 6374 6564  s been extracted
+00015730: 2064 7572 696e 6720 616e 616c 7973 6973   during analysis
+00015740: 2e0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
+00015750: 7320 6120 6275 6c6b 2041 5049 2c20 6d65  s a bulk API, me
+00015760: 616e 696e 6720 7468 6174 2061 2073 696e  aning that a sin
+00015770: 676c 6520 7265 7175 6573 7420 6361 6e20  gle request can 
+00015780: 6265 2075 7365 6420 746f 2073 696d 756c  be used to simul
+00015790: 7461 6e65 6f75 736c 7920 7175 6572 7920  taneously query 
+000157a0: 636f 6e74 6169 6e65 7273 2066 6f72 206d  containers for m
+000157b0: 756c 7469 706c 650a 2020 2020 2020 2020  ultiple.        
+000157c0: 6669 6c65 2068 6173 6865 732e 2049 6620  file hashes. If 
+000157d0: 6120 7265 7175 6573 7465 6420 6861 7368  a requested hash
+000157e0: 2064 6f65 736e e280 9974 2068 6176 6520   doesn...t have 
+000157f0: 6120 636f 6e74 6169 6e65 722c 2069 7420  a container, it 
+00015800: 7769 6c6c 206e 6f74 2062 6520 696e 636c  will not be incl
+00015810: 7564 6564 2069 6e20 7468 6520 7265 7370  uded in the resp
+00015820: 6f6e 7365 2e0a 2020 2020 2020 2020 2020  onse..          
+00015830: 2020 3a70 6172 616d 2073 616d 706c 655f    :param sample_
+00015840: 6861 7368 6573 3a20 6120 6c69 7374 206f  hashes: a list o
+00015850: 6620 6f6e 6520 6f72 206d 6f72 6520 6861  f one or more ha
+00015860: 7368 2076 616c 7565 732c 2062 7574 206d  sh values, but m
+00015870: 7573 7420 616c 6c20 6265 206f 6620 7468  ust all be of th
+00015880: 6520 7361 6d65 2074 7970 6528 5348 4131  e same type(SHA1
+00015890: 2c20 5348 4132 3536 2c0a 2020 2020 2020  , SHA256,.      
+000158a0: 2020 2020 2020 6f72 204d 4435 290a 2020        or MD5).  
+000158b0: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+000158c0: 7361 6d70 6c65 5f68 6173 6865 7320 6c69  sample_hashes li
+000158d0: 7374 5b73 7472 5d0a 2020 2020 2020 2020  st[str].        
+000158e0: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
+000158f0: 706f 6e73 650a 2020 2020 2020 2020 2020  ponse.          
+00015900: 2020 3a72 7479 7065 3a20 7265 7175 6573    :rtype: reques
+00015910: 7473 2e52 6573 706f 6e73 650a 2020 2020  ts.Response.    
+00015920: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00015930: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00015940: 6528 7361 6d70 6c65 5f68 6173 6865 732c  e(sample_hashes,
+00015950: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
+00015960: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
+00015970: 6e70 7574 4572 726f 7228 2273 616d 706c  nputError("sampl
+00015980: 655f 6861 7368 6573 2070 6172 616d 6574  e_hashes paramet
+00015990: 6572 206d 7573 7420 6265 2061 206c 6973  er must be a lis
+000159a0: 7420 6f66 2073 7472 696e 6773 2e22 290a  t of strings.").
+000159b0: 0a20 2020 2020 2020 2076 616c 6964 6174  .        validat
+000159c0: 655f 6861 7368 6573 280a 2020 2020 2020  e_hashes(.      
+000159d0: 2020 2020 2020 6861 7368 5f69 6e70 7574        hash_input
+000159e0: 3d73 616d 706c 655f 6861 7368 6573 2c0a  =sample_hashes,.
+000159f0: 2020 2020 2020 2020 2020 2020 616c 6c6f              allo
+00015a00: 7765 645f 6861 7368 5f74 7970 6573 3d28  wed_hash_types=(
+00015a10: 4d44 352c 2053 4841 312c 2053 4841 3235  MD5, SHA1, SHA25
+00015a20: 3629 0a20 2020 2020 2020 2029 0a0a 2020  6).        )..  
+00015a30: 2020 2020 2020 656e 6470 6f69 6e74 203d        endpoint =
+00015a40: 2073 656c 662e 5f5f 4c49 5354 5f43 4f4e   self.__LIST_CON
+00015a50: 5441 494e 4552 535f 454e 4450 4f49 4e54  TAINERS_ENDPOINT
+00015a60: 0a0a 2020 2020 2020 2020 7572 6c20 3d20  ..        url = 
+00015a70: 7365 6c66 2e5f 7572 6c2e 666f 726d 6174  self._url.format
+00015a80: 2865 6e64 706f 696e 743d 656e 6470 6f69  (endpoint=endpoi
+00015a90: 6e74 290a 0a20 2020 2020 2020 2072 6573  nt)..        res
+00015aa0: 706f 6e73 6520 3d20 7365 6c66 2e5f 5f70  ponse = self.__p
+00015ab0: 6f73 745f 7265 7175 6573 7428 7572 6c3d  ost_request(url=
+00015ac0: 7572 6c2c 2064 6174 613d 7b22 6861 7368  url, data={"hash
+00015ad0: 5f76 616c 7565 7322 3a20 7361 6d70 6c65  _values": sample
+00015ae0: 5f68 6173 6865 737d 290a 0a20 2020 2020  _hashes})..     
+00015af0: 2020 2073 656c 662e 5f5f 7261 6973 655f     self.__raise_
+00015b00: 6f6e 5f65 7272 6f72 2872 6573 706f 6e73  on_error(respons
+00015b10: 6529 0a0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00015b20: 726e 2072 6573 706f 6e73 650a 0a20 2020  rn response..   
+00015b30: 2064 6566 206e 6574 776f 726b 5f75 726c   def network_url
+00015b40: 5f72 6570 6f72 7428 7365 6c66 2c20 7265  _report(self, re
+00015b50: 7175 6573 7465 645f 7572 6c29 3a0a 2020  quested_url):.  
+00015b60: 2020 2020 2020 2222 2241 6363 6570 7473        """Accepts
+00015b70: 2061 2055 524c 2073 7472 696e 6720 616e   a URL string an
+00015b80: 6420 7265 7475 726e 7320 6120 7265 706f  d returns a repo
+00015b90: 7274 2061 626f 7574 2074 6865 2072 6571  rt about the req
+00015ba0: 7565 7374 6564 2055 524c 2e0a 2020 2020  uested URL..    
+00015bb0: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
+00015bc0: 6571 7565 7374 6564 5f75 726c 3a20 5552  equested_url: UR
+00015bd0: 4c20 666f 7220 616e 616c 7973 6973 0a20  L for analysis. 
+00015be0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00015bf0: 2072 6571 7565 7374 6564 5f75 726c 3a20   requested_url: 
+00015c00: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00015c10: 3a72 6574 7572 6e3a 2072 6573 706f 6e73  :return: respons
+00015c20: 650a 2020 2020 2020 2020 2020 2020 3a72  e.            :r
+00015c30: 7479 7065 3a20 7265 7175 6573 7473 2e52  type: requests.R
+00015c40: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
+00015c50: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+00015c60: 6e6f 7420 6973 696e 7374 616e 6365 2872  not isinstance(r
+00015c70: 6571 7565 7374 6564 5f75 726c 2c20 7374  equested_url, st
+00015c80: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00015c90: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
+00015ca0: 4572 726f 7228 2275 726c 2070 6172 616d  Error("url param
+00015cb0: 6574 6572 206d 7573 7420 6265 2073 7472  eter must be str
+00015cc0: 696e 672e 2229 0a0a 2020 2020 2020 2020  ing.")..        
+00015cd0: 656e 636f 6465 645f 7572 6c20 3d20 7061  encoded_url = pa
+00015ce0: 7273 652e 7175 6f74 655f 706c 7573 2872  rse.quote_plus(r
+00015cf0: 6571 7565 7374 6564 5f75 726c 290a 0a20  equested_url).. 
+00015d00: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
+00015d10: 3d20 227b 656e 6470 6f69 6e74 7d3f 7572  = "{endpoint}?ur
+00015d20: 6c3d 7b75 726c 7d22 2e66 6f72 6d61 7428  l={url}".format(
+00015d30: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
+00015d40: 706f 696e 743d 7365 6c66 2e5f 5f55 524c  point=self.__URL
+00015d50: 5f52 4550 4f52 545f 454e 4450 4f49 4e54  _REPORT_ENDPOINT
+00015d60: 2c0a 2020 2020 2020 2020 2020 2020 7572  ,.            ur
+00015d70: 6c3d 656e 636f 6465 645f 7572 6c0a 2020  l=encoded_url.  
+00015d80: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00015d90: 2075 726c 203d 2073 656c 662e 5f75 726c   url = self._url
+00015da0: 2e66 6f72 6d61 7428 656e 6470 6f69 6e74  .format(endpoint
+00015db0: 3d65 6e64 706f 696e 7429 0a0a 2020 2020  =endpoint)..    
+00015dc0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+00015dd0: 656c 662e 5f5f 6765 745f 7265 7175 6573  elf.__get_reques
+00015de0: 7428 7572 6c3d 7572 6c29 0a0a 2020 2020  t(url=url)..    
+00015df0: 2020 2020 7365 6c66 2e5f 5f72 6169 7365      self.__raise
+00015e00: 5f6f 6e5f 6572 726f 7228 7265 7370 6f6e  _on_error(respon
+00015e10: 7365 290a 0a20 2020 2020 2020 2072 6574  se)..        ret
+00015e20: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+00015e30: 2020 6465 6620 6e65 7477 6f72 6b5f 646f    def network_do
+00015e40: 6d61 696e 5f72 6570 6f72 7428 7365 6c66  main_report(self
+00015e50: 2c20 646f 6d61 696e 293a 0a20 2020 2020  , domain):.     
+00015e60: 2020 2022 2222 4163 6365 7074 7320 6120     """Accepts a 
+00015e70: 646f 6d61 696e 2073 7472 696e 6720 616e  domain string an
+00015e80: 6420 7265 7475 726e 7320 6120 7265 706f  d returns a repo
+00015e90: 7274 2061 626f 7574 2074 6865 2072 6571  rt about the req
+00015ea0: 7565 7374 6564 2064 6f6d 6169 6e2e 0a20  uested domain.. 
+00015eb0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00015ec0: 6d20 646f 6d61 696e 3a20 646f 6d61 696e  m domain: domain
+00015ed0: 2066 6f72 2061 6e61 6c79 7369 730a 2020   for analysis.  
+00015ee0: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00015ef0: 646f 6d61 696e 3a20 7374 720a 2020 2020  domain: str.    
+00015f00: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00015f10: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+00015f20: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
+00015f30: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
+00015f40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015f50: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00015f60: 7461 6e63 6528 646f 6d61 696e 2c20 7374  tance(domain, st
+00015f70: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00015f80: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
+00015f90: 4572 726f 7228 2264 6f6d 6169 6e20 7061  Error("domain pa
+00015fa0: 7261 6d65 7465 7220 6d75 7374 2062 6520  rameter must be 
+00015fb0: 7374 7269 6e67 2e22 290a 0a20 2020 2020  string.")..     
+00015fc0: 2020 2065 6e64 706f 696e 7420 3d20 7365     endpoint = se
+00015fd0: 6c66 2e5f 5f44 4f4d 4149 4e5f 5245 504f  lf.__DOMAIN_REPO
+00015fe0: 5254 5f45 4e44 504f 494e 542e 666f 726d  RT_ENDPOINT.form
+00015ff0: 6174 2864 6f6d 6169 6e3d 646f 6d61 696e  at(domain=domain
+00016000: 290a 0a20 2020 2020 2020 2075 726c 203d  )..        url =
+00016010: 2073 656c 662e 5f75 726c 2e66 6f72 6d61   self._url.forma
+00016020: 7428 656e 6470 6f69 6e74 3d65 6e64 706f  t(endpoint=endpo
+00016030: 696e 7429 0a0a 2020 2020 2020 2020 7265  int)..        re
+00016040: 7370 6f6e 7365 203d 2073 656c 662e 5f5f  sponse = self.__
+00016050: 6765 745f 7265 7175 6573 7428 7572 6c3d  get_request(url=
+00016060: 7572 6c29 0a0a 2020 2020 2020 2020 7365  url)..        se
+00016070: 6c66 2e5f 5f72 6169 7365 5f6f 6e5f 6572  lf.__raise_on_er
+00016080: 726f 7228 7265 7370 6f6e 7365 290a 0a20  ror(response).. 
+00016090: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000160a0: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
+000160b0: 6e65 7477 6f72 6b5f 6970 5f61 6464 725f  network_ip_addr_
+000160c0: 7265 706f 7274 2873 656c 662c 2069 705f  report(self, ip_
+000160d0: 6164 6472 293a 0a20 2020 2020 2020 2022  addr):.        "
+000160e0: 2222 4163 6365 7074 7320 616e 2049 5020  ""Accepts an IP 
+000160f0: 6164 6472 6573 7320 7374 7269 6e67 2061  address string a
+00016100: 6e64 2072 6574 7572 6e73 2061 2072 6570  nd returns a rep
+00016110: 6f72 7420 6162 6f75 7420 7468 6520 7265  ort about the re
+00016120: 7175 6573 7465 6420 4950 2061 6464 7265  quested IP addre
+00016130: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
+00016140: 3a70 6172 616d 2069 705f 6164 6472 3a20  :param ip_addr: 
+00016150: 4950 2061 6464 7265 7373 2066 6f72 2061  IP address for a
+00016160: 6e61 6c79 7369 730a 2020 2020 2020 2020  nalysis.        
+00016170: 2020 2020 3a74 7970 6520 6970 5f61 6464      :type ip_add
+00016180: 723a 2073 7472 0a20 2020 2020 2020 2020  r: str.         
+00016190: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
+000161a0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
+000161b0: 203a 7274 7970 653a 2072 6571 7565 7374   :rtype: request
+000161c0: 732e 5265 7370 6f6e 7365 0a20 2020 2020  s.Response.     
+000161d0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+000161e0: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+000161f0: 5f69 705f 6164 6472 5f65 6e64 706f 696e  _ip_addr_endpoin
+00016200: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
+00016210: 6970 5f61 6464 723d 6970 5f61 6464 722c  ip_addr=ip_addr,
+00016220: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
+00016230: 6369 6669 635f 656e 6470 6f69 6e74 3d73  cific_endpoint=s
+00016240: 656c 662e 5f5f 4950 5f52 4550 4f52 545f  elf.__IP_REPORT_
+00016250: 454e 4450 4f49 4e54 0a20 2020 2020 2020  ENDPOINT.       
+00016260: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
+00016270: 726e 2072 6573 706f 6e73 650a 0a20 2020  rn response..   
+00016280: 2064 6566 206e 6574 776f 726b 5f69 705f   def network_ip_
+00016290: 746f 5f64 6f6d 6169 6e28 7365 6c66 2c20  to_domain(self, 
+000162a0: 6970 5f61 6464 722c 2070 6167 653d 4e6f  ip_addr, page=No
+000162b0: 6e65 2c20 7061 6765 5f73 697a 653d 3530  ne, page_size=50
+000162c0: 3029 3a0a 2020 2020 2020 2020 2222 2241  0):.        """A
+000162d0: 6363 6570 7473 2061 6e20 4950 2061 6464  ccepts an IP add
+000162e0: 7265 7373 2073 7472 696e 6720 616e 6420  ress string and 
+000162f0: 7265 7475 726e 7320 6120 6c69 7374 206f  returns a list o
+00016300: 6620 4950 2d74 6f2d 646f 6d61 696e 206d  f IP-to-domain m
+00016310: 6170 7069 6e67 732e 0a20 2020 2020 2020  appings..       
+00016320: 2020 2020 203a 7061 7261 6d20 6970 5f61       :param ip_a
+00016330: 6464 723a 2072 6571 7565 7374 6564 2049  ddr: requested I
+00016340: 5020 6164 6472 6573 730a 2020 2020 2020  P address.      
+00016350: 2020 2020 2020 3a74 7970 6520 6970 5f61        :type ip_a
+00016360: 6464 723a 2073 7472 0a20 2020 2020 2020  ddr: str.       
+00016370: 2020 2020 203a 7061 7261 6d20 7061 6765       :param page
+00016380: 3a20 7061 6765 2073 7472 696e 670a 2020  : page string.  
+00016390: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+000163a0: 7061 6765 3a20 7374 7220 6f72 204e 6f6e  page: str or Non
+000163b0: 650a 2020 2020 2020 2020 2020 2020 3a70  e.            :p
+000163c0: 6172 616d 2070 6167 655f 7369 7a65 3a20  aram page_size: 
+000163d0: 6e75 6d62 6572 206f 6620 7265 7375 6c74  number of result
+000163e0: 7320 7065 7220 7061 6765 0a20 2020 2020  s per page.     
+000163f0: 2020 2020 2020 203a 7479 7065 2070 6167         :type pag
+00016400: 655f 7369 7a65 3a20 696e 740a 2020 2020  e_size: int.    
+00016410: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00016420: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+00016430: 2020 2020 2020 3a72 7479 7065 3a20 7265        :rtype: re
+00016440: 7175 6573 7473 2e52 6573 706f 6e73 650a  quests.Response.
+00016450: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00016460: 2020 2020 6966 2070 6167 6520 616e 6420      if page and 
+00016470: 6e6f 7420 6973 696e 7374 616e 6365 2870  not isinstance(p
+00016480: 6167 652c 2073 7472 293a 0a20 2020 2020  age, str):.     
+00016490: 2020 2020 2020 2072 6169 7365 2057 726f         raise Wro
+000164a0: 6e67 496e 7075 7445 7272 6f72 2822 7061  ngInputError("pa
+000164b0: 6765 2070 6172 616d 6574 6572 206d 7573  ge parameter mus
+000164c0: 7420 6265 2073 7472 696e 672e 2229 0a0a  t be string.")..
+000164d0: 2020 2020 2020 2020 6966 2070 6167 655f          if page_
+000164e0: 7369 7a65 2061 6e64 206e 6f74 2069 7369  size and not isi
+000164f0: 6e73 7461 6e63 6528 7061 6765 5f73 697a  nstance(page_siz
+00016500: 652c 2069 6e74 293a 0a20 2020 2020 2020  e, int):.       
+00016510: 2020 2020 2072 6169 7365 2057 726f 6e67       raise Wrong
+00016520: 496e 7075 7445 7272 6f72 2822 7061 6765  InputError("page
+00016530: 5f73 697a 6520 7061 7261 6d65 7465 7220  _size parameter 
+00016540: 6d75 7374 2062 6520 696e 7465 6765 722e  must be integer.
+00016550: 2229 0a0a 2020 2020 2020 2020 7061 7261  ")..        para
+00016560: 6d73 203d 207b 0a20 2020 2020 2020 2020  ms = {.         
+00016570: 2020 2022 7061 6765 223a 2070 6167 652c     "page": page,
+00016580: 0a20 2020 2020 2020 2020 2020 2022 7061  .            "pa
+00016590: 6765 5f73 697a 6522 3a20 7061 6765 5f73  ge_size": page_s
+000165a0: 697a 650a 2020 2020 2020 2020 7d0a 0a20  ize.        }.. 
+000165b0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+000165c0: 3d20 7365 6c66 2e5f 5f69 705f 6164 6472  = self.__ip_addr
+000165d0: 5f65 6e64 706f 696e 7473 280a 2020 2020  _endpoints(.    
+000165e0: 2020 2020 2020 2020 6970 5f61 6464 723d          ip_addr=
+000165f0: 6970 5f61 6464 722c 0a20 2020 2020 2020  ip_addr,.       
+00016600: 2020 2020 2073 7065 6369 6669 635f 656e       specific_en
+00016610: 6470 6f69 6e74 3d73 656c 662e 5f5f 4950  dpoint=self.__IP
+00016620: 5f54 4f5f 444f 4d41 494e 5f45 4e44 504f  _TO_DOMAIN_ENDPO
+00016630: 494e 542c 0a20 2020 2020 2020 2020 2020  INT,.           
+00016640: 2070 6172 616d 733d 7061 7261 6d73 0a20   params=params. 
+00016650: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00016660: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+00016670: 650a 0a20 2020 2064 6566 206e 6574 776f  e..    def netwo
+00016680: 726b 5f69 705f 746f 5f64 6f6d 6169 6e5f  rk_ip_to_domain_
+00016690: 6167 6772 6567 6174 6564 2873 656c 662c  aggregated(self,
+000166a0: 2069 705f 6164 6472 2c20 7061 6765 5f73   ip_addr, page_s
+000166b0: 697a 653d 3530 302c 206d 6178 5f72 6573  ize=500, max_res
+000166c0: 756c 7473 3d35 3030 3029 3a0a 2020 2020  ults=5000):.    
+000166d0: 2020 2020 2222 2241 6363 6570 7473 2061      """Accepts a
+000166e0: 6e20 4950 2061 6464 7265 7373 2073 7472  n IP address str
+000166f0: 696e 6720 616e 6420 7265 7475 726e 7320  ing and returns 
+00016700: 6120 6c69 7374 206f 6620 4950 2d74 6f2d  a list of IP-to-
+00016710: 646f 6d61 696e 206d 6170 7069 6e67 732e  domain mappings.
+00016720: 0a20 2020 2020 2020 2054 6869 7320 6d65  .        This me
+00016730: 7468 6f64 2070 6572 666f 726d 7320 7468  thod performs th
+00016740: 6520 7061 6769 6e67 2061 7574 6f6d 6174  e paging automat
+00016750: 6963 616c 6c79 2061 6e64 2072 6574 7572  ically and retur
+00016760: 6e73 2061 2073 7065 6369 6669 6564 206d  ns a specified m
+00016770: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+00016780: 2072 6563 6f72 6473 2e0a 2020 2020 2020   records..      
+00016790: 2020 2020 2020 3a70 6172 616d 2069 705f        :param ip_
+000167a0: 6164 6472 3a20 7265 7175 6573 7465 6420  addr: requested 
+000167b0: 4950 2061 6464 7265 7373 0a20 2020 2020  IP address.     
+000167c0: 2020 2020 2020 203a 7479 7065 2069 705f         :type ip_
+000167d0: 6164 6472 3a20 7374 720a 2020 2020 2020  addr: str.      
+000167e0: 2020 2020 2020 3a70 6172 616d 2070 6167        :param pag
+000167f0: 655f 7369 7a65 3a20 6e75 6d62 6572 206f  e_size: number o
+00016800: 6620 7265 636f 7264 7320 7065 7220 7061  f records per pa
+00016810: 6765 0a20 2020 2020 2020 2020 2020 203a  ge.            :
+00016820: 7479 7065 2070 6167 655f 7369 7a65 3a20  type page_size: 
+00016830: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+00016840: 3a70 6172 616d 206d 6178 5f72 6573 756c  :param max_resul
+00016850: 7473 3a20 6d61 7869 6d75 6d20 6e75 6d62  ts: maximum numb
+00016860: 6572 206f 6620 7265 7475 726e 6564 2072  er of returned r
+00016870: 6563 6f72 6473 0a20 2020 2020 2020 2020  ecords.         
+00016880: 2020 203a 7479 7065 206d 6178 5f72 6573     :type max_res
+00016890: 756c 7473 3a20 696e 740a 2020 2020 2020  ults: int.      
+000168a0: 2020 2020 2020 3a72 6574 7572 6e3a 206c        :return: l
+000168b0: 6973 7420 6f66 2072 6573 756c 7473 0a20  ist of results. 
+000168c0: 2020 2020 2020 2020 2020 203a 7274 7970             :rtyp
+000168d0: 653a 206c 6973 740a 2020 2020 2020 2020  e: list.        
+000168e0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+000168f0: 6f74 2069 7369 6e73 7461 6e63 6528 6d61  ot isinstance(ma
+00016900: 785f 7265 7375 6c74 732c 2069 6e74 293a  x_results, int):
+00016910: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00016920: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
+00016930: 6f72 2822 6d61 785f 7265 7375 6c74 7320  or("max_results 
+00016940: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
+00016950: 6520 696e 7465 6765 722e 2229 0a0a 2020  e integer.")..  
+00016960: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
+00016970: 5b5d 0a20 2020 2020 2020 206e 6578 745f  [].        next_
+00016980: 7061 6765 203d 204e 6f6e 650a 0a20 2020  page = None..   
+00016990: 2020 2020 2077 6869 6c65 2054 7275 653a       while True:
+000169a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000169b0: 706f 6e73 6520 3d20 7365 6c66 2e6e 6574  ponse = self.net
+000169c0: 776f 726b 5f69 705f 746f 5f64 6f6d 6169  work_ip_to_domai
+000169d0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+000169e0: 2020 2069 705f 6164 6472 3d69 705f 6164     ip_addr=ip_ad
+000169f0: 6472 2c0a 2020 2020 2020 2020 2020 2020  dr,.            
+00016a00: 2020 2020 7061 6765 3d6e 6578 745f 7061      page=next_pa
+00016a10: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
+00016a20: 2020 2020 7061 6765 5f73 697a 653d 7061      page_size=pa
+00016a30: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
+00016a40: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+00016a50: 2020 2072 6573 706f 6e73 655f 6a73 6f6e     response_json
+00016a60: 203d 2072 6573 706f 6e73 652e 6a73 6f6e   = response.json
+00016a70: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00016a80: 7265 736f 6c75 7469 6f6e 7320 3d20 7265  resolutions = re
+00016a90: 7370 6f6e 7365 5f6a 736f 6e2e 6765 7428  sponse_json.get(
+00016aa0: 2272 6573 6f6c 7574 696f 6e73 222c 205b  "resolutions", [
+00016ab0: 5d29 0a20 2020 2020 2020 2020 2020 2072  ]).            r
+00016ac0: 6573 756c 7473 2e65 7874 656e 6428 7265  esults.extend(re
+00016ad0: 736f 6c75 7469 6f6e 7329 0a0a 2020 2020  solutions)..    
+00016ae0: 2020 2020 2020 2020 6e65 7874 5f70 6167          next_pag
+00016af0: 6520 3d20 7265 7370 6f6e 7365 5f6a 736f  e = response_jso
+00016b00: 6e2e 6765 7428 226e 6578 745f 7061 6765  n.get("next_page
+00016b10: 222c 204e 6f6e 6529 0a0a 2020 2020 2020  ", None)..      
+00016b20: 2020 2020 2020 6966 206c 656e 2872 6573        if len(res
+00016b30: 756c 7473 2920 3e3d 206d 6178 5f72 6573  ults) >= max_res
+00016b40: 756c 7473 206f 7220 6e6f 7420 6e65 7874  ults or not next
+00016b50: 5f70 6167 653a 0a20 2020 2020 2020 2020  _page:.         
+00016b60: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+00016b70: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00016b80: 756c 7473 5b3a 6d61 785f 7265 7375 6c74  ults[:max_result
+00016b90: 735d 0a0a 2020 2020 6465 6620 6e65 7477  s]..    def netw
+00016ba0: 6f72 6b5f 7572 6c73 5f66 726f 6d5f 6970  ork_urls_from_ip
+00016bb0: 2873 656c 662c 2069 705f 6164 6472 2c20  (self, ip_addr, 
+00016bc0: 7061 6765 3d4e 6f6e 652c 2070 6167 655f  page=None, page_
+00016bd0: 7369 7a65 3d35 3030 293a 0a20 2020 2020  size=500):.     
+00016be0: 2020 2022 2222 4163 6365 7074 7320 616e     """Accepts an
+00016bf0: 2049 5020 6164 6472 6573 7320 7374 7269   IP address stri
+00016c00: 6e67 2061 6e64 2072 6574 7572 6e73 2061  ng and returns a
+00016c10: 206c 6973 7420 6f66 2055 524c 7320 686f   list of URLs ho
+00016c20: 7374 6564 206f 6e20 7468 6520 7265 7175  sted on the requ
+00016c30: 6573 7465 6420 4950 2061 6464 7265 7373  ested IP address
+00016c40: 2e0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
+00016c50: 6172 616d 2069 705f 6164 6472 3a20 7265  aram ip_addr: re
+00016c60: 7175 6573 7465 6420 4950 2061 6464 7265  quested IP addre
+00016c70: 7373 0a20 2020 2020 2020 2020 2020 203a  ss.            :
+00016c80: 7479 7065 2069 705f 6164 6472 3a20 7374  type ip_addr: st
+00016c90: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
+00016ca0: 6172 616d 2070 6167 653a 2070 6167 6520  aram page: page 
+00016cb0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+00016cc0: 2020 203a 7479 7065 2070 6167 653a 2073     :type page: s
+00016cd0: 7472 206f 7220 4e6f 6e65 0a20 2020 2020  tr or None.     
+00016ce0: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
+00016cf0: 6765 5f73 697a 653a 206e 756d 6265 7220  ge_size: number 
+00016d00: 6f66 2072 6563 6f72 6473 2070 6572 2070  of records per p
+00016d10: 6167 650a 2020 2020 2020 2020 2020 2020  age.            
+00016d20: 3a74 7970 6520 7061 6765 5f73 697a 653a  :type page_size:
+00016d30: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+00016d40: 203a 7265 7475 726e 3a20 7265 7370 6f6e   :return: respon
+00016d50: 7365 0a20 2020 2020 2020 2020 2020 203a  se.            :
+00016d60: 7274 7970 653a 2072 6571 7565 7374 732e  rtype: requests.
+00016d70: 5265 7370 6f6e 7365 0a20 2020 2020 2020  Response.       
+00016d80: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00016d90: 7061 6765 2061 6e64 206e 6f74 2069 7369  page and not isi
+00016da0: 6e73 7461 6e63 6528 7061 6765 2c20 7374  nstance(page, st
+00016db0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00016dc0: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
+00016dd0: 4572 726f 7228 2270 6167 6520 7061 7261  Error("page para
+00016de0: 6d65 7465 7220 6d75 7374 2062 6520 7374  meter must be st
+00016df0: 7269 6e67 2e22 290a 0a20 2020 2020 2020  ring.")..       
+00016e00: 2069 6620 7061 6765 5f73 697a 6520 616e   if page_size an
+00016e10: 6420 6e6f 7420 6973 696e 7374 616e 6365  d not isinstance
+00016e20: 2870 6167 655f 7369 7a65 2c20 696e 7429  (page_size, int)
+00016e30: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00016e40: 6973 6520 5772 6f6e 6749 6e70 7574 4572  ise WrongInputEr
+00016e50: 726f 7228 2270 6167 655f 7369 7a65 2070  ror("page_size p
+00016e60: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+00016e70: 2069 6e74 6567 6572 2e22 290a 0a20 2020   integer.")..   
+00016e80: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
+00016e90: 2020 2020 2020 2020 2020 2020 2270 6167              "pag
+00016ea0: 6522 3a20 7061 6765 2c0a 2020 2020 2020  e": page,.      
+00016eb0: 2020 2020 2020 2270 6167 655f 7369 7a65        "page_size
+00016ec0: 223a 2070 6167 655f 7369 7a65 0a20 2020  ": page_size.   
+00016ed0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00016ee0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00016ef0: 5f5f 6970 5f61 6464 725f 656e 6470 6f69  __ip_addr_endpoi
+00016f00: 6e74 7328 0a20 2020 2020 2020 2020 2020  nts(.           
+00016f10: 2069 705f 6164 6472 3d69 705f 6164 6472   ip_addr=ip_addr
+00016f20: 2c0a 2020 2020 2020 2020 2020 2020 7370  ,.            sp
+00016f30: 6563 6966 6963 5f65 6e64 706f 696e 743d  ecific_endpoint=
+00016f40: 7365 6c66 2e5f 5f55 524c 535f 4652 4f4d  self.__URLS_FROM
+00016f50: 5f49 505f 454e 4450 4f49 4e54 2c0a 2020  _IP_ENDPOINT,.  
+00016f60: 2020 2020 2020 2020 2020 7061 7261 6d73            params
+00016f70: 3d70 6172 616d 730a 2020 2020 2020 2020  =params.        
+00016f80: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00016f90: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
+00016fa0: 6465 6620 6e65 7477 6f72 6b5f 7572 6c73  def network_urls
+00016fb0: 5f66 726f 6d5f 6970 5f61 6767 7265 6761  _from_ip_aggrega
+00016fc0: 7465 6428 7365 6c66 2c20 6970 5f61 6464  ted(self, ip_add
+00016fd0: 722c 2070 6167 655f 7369 7a65 3d35 3030  r, page_size=500
+00016fe0: 2c20 6d61 785f 7265 7375 6c74 733d 3530  , max_results=50
+00016ff0: 3030 293a 0a20 2020 2020 2020 2022 2222  00):.        """
+00017000: 4163 6365 7074 7320 616e 2049 5020 6164  Accepts an IP ad
+00017010: 6472 6573 7320 7374 7269 6e67 2061 6e64  dress string and
+00017020: 2072 6574 7572 6e73 2061 206c 6973 7420   returns a list 
+00017030: 6f66 2055 524c 7320 686f 7374 6564 206f  of URLs hosted o
+00017040: 6e20 7468 6520 7265 7175 6573 7465 6420  n the requested 
+00017050: 4950 2061 6464 7265 7373 2e0a 2020 2020  IP address..    
+00017060: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
+00017070: 7065 7266 6f72 6d73 2074 6865 2070 6167  performs the pag
+00017080: 696e 6720 6175 746f 6d61 7469 6361 6c6c  ing automaticall
+00017090: 7920 616e 6420 7265 7475 726e 7320 6120  y and returns a 
+000170a0: 7370 6563 6966 6965 6420 6d61 7869 6d75  specified maximu
+000170b0: 6d20 6e75 6d62 6572 206f 6620 7265 636f  m number of reco
+000170c0: 7264 732e 0a20 2020 2020 2020 2020 2020  rds..           
+000170d0: 203a 7061 7261 6d20 6970 5f61 6464 723a   :param ip_addr:
+000170e0: 2072 6571 7565 7374 6564 2049 5020 6164   requested IP ad
+000170f0: 6472 6573 730a 2020 2020 2020 2020 2020  dress.          
+00017100: 2020 3a74 7970 6520 6970 5f61 6464 723a    :type ip_addr:
+00017110: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+00017120: 203a 7061 7261 6d20 7061 6765 5f73 697a   :param page_siz
+00017130: 653a 206e 756d 6265 7220 6f66 2072 6563  e: number of rec
+00017140: 6f72 6473 2070 6572 2070 6167 650a 2020  ords per page.  
+00017150: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00017160: 7061 6765 5f73 697a 653a 2069 6e74 0a20  page_size: int. 
+00017170: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00017180: 6d20 6d61 785f 7265 7375 6c74 733a 206d  m max_results: m
+00017190: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+000171a0: 2072 6574 7572 6e65 6420 7265 636f 7264   returned record
+000171b0: 730a 2020 2020 2020 2020 2020 2020 3a74  s.            :t
+000171c0: 7970 6520 6d61 785f 7265 7375 6c74 733a  ype max_results:
+000171d0: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+000171e0: 203a 7265 7475 726e 3a20 6c69 7374 206f   :return: list o
+000171f0: 6620 7265 7375 6c74 730a 2020 2020 2020  f results.      
+00017200: 2020 2020 2020 3a72 7479 7065 3a20 6c69        :rtype: li
+00017210: 7374 0a20 2020 2020 2020 2022 2222 0a20  st.        """. 
+00017220: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+00017230: 696e 7374 616e 6365 286d 6178 5f72 6573  instance(max_res
+00017240: 756c 7473 2c20 696e 7429 3a0a 2020 2020  ults, int):.    
+00017250: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
+00017260: 6f6e 6749 6e70 7574 4572 726f 7228 226d  ongInputError("m
+00017270: 6178 5f72 6573 756c 7473 2070 6172 616d  ax_results param
+00017280: 6574 6572 206d 7573 7420 6265 2069 6e74  eter must be int
+00017290: 6567 6572 2e22 290a 0a20 2020 2020 2020  eger.")..       
+000172a0: 2072 6573 756c 7473 203d 205b 5d0a 2020   results = [].  
+000172b0: 2020 2020 2020 6e65 7874 5f70 6167 6520        next_page 
+000172c0: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
+000172d0: 7768 696c 6520 5472 7565 3a0a 2020 2020  while True:.    
+000172e0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+000172f0: 203d 2073 656c 662e 6e65 7477 6f72 6b5f   = self.network_
+00017300: 7572 6c73 5f66 726f 6d5f 6970 280a 2020  urls_from_ip(.  
+00017310: 2020 2020 2020 2020 2020 2020 2020 6970                ip
+00017320: 5f61 6464 723d 6970 5f61 6464 722c 0a20  _addr=ip_addr,. 
+00017330: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00017340: 6167 653d 6e65 7874 5f70 6167 652c 0a20  age=next_page,. 
+00017350: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00017360: 6167 655f 7369 7a65 3d70 6167 655f 7369  age_size=page_si
+00017370: 7a65 0a20 2020 2020 2020 2020 2020 2029  ze.            )
+00017380: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00017390: 7370 6f6e 7365 5f6a 736f 6e20 3d20 7265  sponse_json = re
+000173a0: 7370 6f6e 7365 2e6a 736f 6e28 290a 0a20  sponse.json().. 
+000173b0: 2020 2020 2020 2020 2020 2075 726c 7320             urls 
+000173c0: 3d20 7265 7370 6f6e 7365 5f6a 736f 6e2e  = response_json.
+000173d0: 6765 7428 2275 726c 7322 2c20 5b5d 290a  get("urls", []).
+000173e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000173f0: 6c74 732e 6578 7465 6e64 2875 726c 7329  lts.extend(urls)
+00017400: 0a0a 2020 2020 2020 2020 2020 2020 6e65  ..            ne
+00017410: 7874 5f70 6167 6520 3d20 7265 7370 6f6e  xt_page = respon
+00017420: 7365 5f6a 736f 6e2e 6765 7428 226e 6578  se_json.get("nex
+00017430: 745f 7061 6765 222c 204e 6f6e 6529 0a0a  t_page", None)..
+00017440: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00017450: 656e 2872 6573 756c 7473 2920 3e3d 206d  en(results) >= m
+00017460: 6178 5f72 6573 756c 7473 206f 7220 6e6f  ax_results or no
+00017470: 7420 6e65 7874 5f70 6167 653a 0a20 2020  t next_page:.   
+00017480: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00017490: 616b 0a0a 2020 2020 2020 2020 7265 7475  ak..        retu
+000174a0: 726e 2072 6573 756c 7473 5b3a 6d61 785f  rn results[:max_
+000174b0: 7265 7375 6c74 735d 0a0a 2020 2020 6465  results]..    de
+000174c0: 6620 6e65 7477 6f72 6b5f 6669 6c65 735f  f network_files_
+000174d0: 6672 6f6d 5f69 7028 7365 6c66 2c20 6970  from_ip(self, ip
+000174e0: 5f61 6464 722c 2065 7874 656e 6465 645f  _addr, extended_
+000174f0: 7265 7375 6c74 733d 5472 7565 2c20 636c  results=True, cl
+00017500: 6173 7369 6669 6361 7469 6f6e 3d4e 6f6e  assification=Non
+00017510: 652c 2070 6167 653d 4e6f 6e65 2c20 7061  e, page=None, pa
+00017520: 6765 5f73 697a 653d 3530 3029 3a0a 2020  ge_size=500):.  
+00017530: 2020 2020 2020 2222 2241 6363 6570 7473        """Accepts
+00017540: 2061 6e20 4950 2061 6464 7265 7373 2073   an IP address s
+00017550: 7472 696e 6720 616e 6420 7265 7475 726e  tring and return
+00017560: 7320 6120 6c69 7374 206f 6620 6861 7368  s a list of hash
+00017570: 6573 2061 6e64 0a20 2020 2020 2020 2063  es and.        c
+00017580: 6c61 7373 6966 6963 6174 696f 6e73 2066  lassifications f
+00017590: 6f72 2066 696c 6573 2066 6f75 6e64 206f  or files found o
+000175a0: 6e20 7468 6520 7265 7175 6573 7465 6420  n the requested 
+000175b0: 4950 2061 6464 7265 7373 2e0a 2020 2020  IP address..    
+000175c0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+000175d0: 705f 6164 6472 3a20 7265 7175 6573 7465  p_addr: requeste
+000175e0: 6420 4950 2061 6464 7265 7373 0a20 2020  d IP address.   
+000175f0: 2020 2020 2020 2020 203a 7479 7065 2069           :type i
+00017600: 705f 6164 6472 3a20 7374 720a 2020 2020  p_addr: str.    
+00017610: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
+00017620: 7874 656e 6465 645f 7265 7375 6c74 733a  xtended_results:
+00017630: 2072 6574 7572 6e20 6578 7465 6e64 6564   return extended
+00017640: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
+00017650: 2020 2020 203a 7479 7065 2065 7874 656e       :type exten
+00017660: 6465 645f 7265 7375 6c74 733a 2062 6f6f  ded_results: boo
+00017670: 6c0a 2020 2020 2020 2020 2020 2020 3a70  l.            :p
+00017680: 6172 616d 2063 6c61 7373 6966 6963 6174  aram classificat
+00017690: 696f 6e3a 2072 6574 7572 6e20 6f6e 6c79  ion: return only
+000176a0: 2072 6563 6f72 6473 2077 6974 6820 7468   records with th
+000176b0: 6973 2063 6c61 7373 6966 6963 6174 696f  is classificatio
+000176c0: 6e0a 2020 2020 2020 2020 2020 2020 3a74  n.            :t
+000176d0: 7970 6520 636c 6173 7369 6669 6361 7469  ype classificati
+000176e0: 6f6e 3a20 7374 720a 2020 2020 2020 2020  on: str.        
+000176f0: 2020 2020 3a70 6172 616d 2070 6167 653a      :param page:
+00017700: 2070 6167 6520 7374 7269 6e67 0a20 2020   page string.   
+00017710: 2020 2020 2020 2020 203a 7479 7065 2070           :type p
+00017720: 6167 653a 2073 7472 206f 7220 4e6f 6e65  age: str or None
+00017730: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+00017740: 7261 6d20 7061 6765 5f73 697a 653a 206e  ram page_size: n
+00017750: 756d 6265 7220 6f66 2072 6563 6f72 6473  umber of records
+00017760: 2070 6572 2070 6167 650a 2020 2020 2020   per page.      
+00017770: 2020 2020 2020 3a74 7970 6520 7061 6765        :type page
+00017780: 5f73 697a 653a 2069 6e74 0a20 2020 2020  _size: int.     
+00017790: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+000177a0: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+000177b0: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
+000177c0: 7565 7374 732e 5265 7370 6f6e 7365 0a20  uests.Response. 
+000177d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000177e0: 2020 2069 6620 7061 6765 2061 6e64 206e     if page and n
+000177f0: 6f74 2069 7369 6e73 7461 6e63 6528 7061  ot isinstance(pa
+00017800: 6765 2c20 7374 7229 3a0a 2020 2020 2020  ge, str):.      
+00017810: 2020 2020 2020 7261 6973 6520 5772 6f6e        raise Wron
+00017820: 6749 6e70 7574 4572 726f 7228 2270 6167  gInputError("pag
+00017830: 6520 7061 7261 6d65 7465 7220 6d75 7374  e parameter must
+00017840: 2062 6520 7374 7269 6e67 2e22 290a 0a20   be string.").. 
+00017850: 2020 2020 2020 2069 6620 7061 6765 5f73         if page_s
+00017860: 697a 6520 616e 6420 6e6f 7420 6973 696e  ize and not isin
+00017870: 7374 616e 6365 2870 6167 655f 7369 7a65  stance(page_size
+00017880: 2c20 696e 7429 3a0a 2020 2020 2020 2020  , int):.        
+00017890: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
+000178a0: 6e70 7574 4572 726f 7228 2270 6167 655f  nputError("page_
+000178b0: 7369 7a65 2070 6172 616d 6574 6572 206d  size parameter m
+000178c0: 7573 7420 6265 2069 6e74 6567 6572 2e22  ust be integer."
+000178d0: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+000178e0: 7420 6973 696e 7374 616e 6365 2865 7874  t isinstance(ext
+000178f0: 656e 6465 645f 7265 7375 6c74 732c 2062  ended_results, b
+00017900: 6f6f 6c29 3a0a 2020 2020 2020 2020 2020  ool):.          
+00017910: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+00017920: 7574 4572 726f 7228 2265 7874 656e 6465  utError("extende
+00017930: 645f 7265 7375 6c74 7320 7061 7261 6d65  d_results parame
+00017940: 7465 7220 6d75 7374 2062 6520 626f 6f6c  ter must be bool
+00017950: 6561 6e2e 2229 0a0a 2020 2020 2020 2020  ean.")..        
+00017960: 6966 2063 6c61 7373 6966 6963 6174 696f  if classificatio
+00017970: 6e20 616e 6420 636c 6173 7369 6669 6361  n and classifica
+00017980: 7469 6f6e 206e 6f74 2069 6e20 434c 4153  tion not in CLAS
+00017990: 5349 4649 4341 5449 4f4e 533a 0a20 2020  SIFICATIONS:.   
+000179a0: 2020 2020 2020 2020 2072 6169 7365 2057           raise W
+000179b0: 726f 6e67 496e 7075 7445 7272 6f72 2822  rongInputError("
+000179c0: 4f6e 6c79 207b 636c 6173 7369 6669 6361  Only {classifica
+000179d0: 7469 6f6e 737d 2069 7320 616c 6c6f 7765  tions} is allowe
+000179e0: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
+000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a00: 2020 2020 2020 2261 7320 7468 6520 636c        "as the cl
+00017a10: 6173 7369 6669 6361 7469 6f6e 2069 6e70  assification inp
+00017a20: 7574 2e22 2e66 6f72 6d61 7428 636c 6173  ut.".format(clas
+00017a30: 7369 6669 6361 7469 6f6e 733d 434c 4153  sifications=CLAS
+00017a40: 5349 4649 4341 5449 4f4e 5329 290a 0a20  SIFICATIONS)).. 
+00017a50: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
+00017a60: 7b0a 2020 2020 2020 2020 2020 2020 2265  {.            "e
+00017a70: 7874 656e 6465 6422 3a20 6578 7465 6e64  xtended": extend
+00017a80: 6564 5f72 6573 756c 7473 2c0a 2020 2020  ed_results,.    
+00017a90: 2020 2020 2020 2020 2263 6c61 7373 6966          "classif
+00017aa0: 6963 6174 696f 6e22 3a20 636c 6173 7369  ication": classi
+00017ab0: 6669 6361 7469 6f6e 2c0a 2020 2020 2020  fication,.      
+00017ac0: 2020 2020 2020 2270 6167 6522 3a20 7061        "page": pa
+00017ad0: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
+00017ae0: 2270 6167 655f 7369 7a65 223a 2070 6167  "page_size": pag
+00017af0: 655f 7369 7a65 0a20 2020 2020 2020 207d  e_size.        }
+00017b00: 0a0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
+00017b10: 7365 203d 2073 656c 662e 5f5f 6970 5f61  se = self.__ip_a
+00017b20: 6464 725f 656e 6470 6f69 6e74 7328 0a20  ddr_endpoints(. 
+00017b30: 2020 2020 2020 2020 2020 2069 705f 6164             ip_ad
+00017b40: 6472 3d69 705f 6164 6472 2c0a 2020 2020  dr=ip_addr,.    
+00017b50: 2020 2020 2020 2020 7370 6563 6966 6963          specific
+00017b60: 5f65 6e64 706f 696e 743d 7365 6c66 2e5f  _endpoint=self._
+00017b70: 5f46 494c 4553 5f46 524f 4d5f 4950 5f45  _FILES_FROM_IP_E
+00017b80: 4e44 504f 494e 542c 0a20 2020 2020 2020  NDPOINT,.       
+00017b90: 2020 2020 2070 6172 616d 733d 7061 7261       params=para
+00017ba0: 6d73 0a20 2020 2020 2020 2029 0a0a 2020  ms.        )..  
+00017bb0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00017bc0: 706f 6e73 650a 0a20 2020 2064 6566 206e  ponse..    def n
+00017bd0: 6574 776f 726b 5f66 696c 6573 5f66 726f  etwork_files_fro
+00017be0: 6d5f 6970 5f61 6767 7265 6761 7465 6428  m_ip_aggregated(
+00017bf0: 7365 6c66 2c20 6970 5f61 6464 722c 2065  self, ip_addr, e
+00017c00: 7874 656e 6465 645f 7265 7375 6c74 733d  xtended_results=
+00017c10: 5472 7565 2c20 636c 6173 7369 6669 6361  True, classifica
+00017c20: 7469 6f6e 3d4e 6f6e 652c 2070 6167 655f  tion=None, page_
+00017c30: 7369 7a65 3d35 3030 2c0a 2020 2020 2020  size=500,.      
+00017c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c60: 2020 206d 6178 5f72 6573 756c 7473 3d35     max_results=5
+00017c70: 3030 3029 3a0a 2020 2020 2020 2020 2222  000):.        ""
+00017c80: 2241 6363 6570 7473 2061 6e20 4950 2061  "Accepts an IP a
+00017c90: 6464 7265 7373 2073 7472 696e 6720 616e  ddress string an
+00017ca0: 6420 7265 7475 726e 7320 6120 6c69 7374  d returns a list
+00017cb0: 206f 6620 6861 7368 6573 2061 6e64 0a20   of hashes and. 
+00017cc0: 2020 2020 2020 2063 6c61 7373 6966 6963         classific
+00017cd0: 6174 696f 6e73 2066 6f72 2066 696c 6573  ations for files
+00017ce0: 2066 6f75 6e64 206f 6e20 7468 6520 7265   found on the re
+00017cf0: 7175 6573 7465 6420 4950 2061 6464 7265  quested IP addre
+00017d00: 7373 2e0a 2020 2020 2020 2020 5468 6973  ss..        This
+00017d10: 206d 6574 686f 6420 7065 7266 6f72 6d73   method performs
+00017d20: 2074 6865 2070 6167 696e 6720 6175 746f   the paging auto
+00017d30: 6d61 7469 6361 6c6c 7920 616e 6420 7265  matically and re
+00017d40: 7475 726e 7320 6120 7370 6563 6966 6965  turns a specifie
+00017d50: 6420 6d61 7869 6d75 6d20 6e75 6d62 6572  d maximum number
+00017d60: 206f 6620 7265 636f 7264 732e 0a20 2020   of records..   
+00017d70: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00017d80: 6970 5f61 6464 723a 2072 6571 7565 7374  ip_addr: request
+00017d90: 6564 2049 5020 6164 6472 6573 730a 2020  ed IP address.  
+00017da0: 2020 2020 2020 2020 2020 3a74 7970 6520            :type 
+00017db0: 6970 5f61 6464 723a 2073 7472 0a20 2020  ip_addr: str.   
+00017dc0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00017dd0: 6578 7465 6e64 6564 5f72 6573 756c 7473  extended_results
+00017de0: 3a20 7265 7475 726e 2065 7874 656e 6465  : return extende
+00017df0: 6420 7265 7375 6c74 730a 2020 2020 2020  d results.      
+00017e00: 2020 2020 2020 3a74 7970 6520 6578 7465        :type exte
+00017e10: 6e64 6564 5f72 6573 756c 7473 3a20 626f  nded_results: bo
+00017e20: 6f6c 0a20 2020 2020 2020 2020 2020 203a  ol.            :
+00017e30: 7061 7261 6d20 636c 6173 7369 6669 6361  param classifica
+00017e40: 7469 6f6e 3a20 7265 7475 726e 206f 6e6c  tion: return onl
+00017e50: 7920 7265 636f 7264 7320 7769 7468 2074  y records with t
+00017e60: 6869 7320 636c 6173 7369 6669 6361 7469  his classificati
+00017e70: 6f6e 0a20 2020 2020 2020 2020 2020 203a  on.            :
+00017e80: 7479 7065 2063 6c61 7373 6966 6963 6174  type classificat
+00017e90: 696f 6e3a 2073 7472 0a20 2020 2020 2020  ion: str.       
+00017ea0: 2020 2020 203a 7061 7261 6d20 7061 6765       :param page
+00017eb0: 5f73 697a 653a 206e 756d 6265 7220 6f66  _size: number of
+00017ec0: 2072 6563 6f72 6473 2070 6572 2070 6167   records per pag
+00017ed0: 650a 2020 2020 2020 2020 2020 2020 3a74  e.            :t
+00017ee0: 7970 6520 7061 6765 5f73 697a 653a 2069  ype page_size: i
+00017ef0: 6e74 0a20 2020 2020 2020 2020 2020 203a  nt.            :
+00017f00: 7061 7261 6d20 6d61 785f 7265 7375 6c74  param max_result
+00017f10: 733a 206d 6178 696d 756d 206e 756d 6265  s: maximum numbe
+00017f20: 7220 6f66 2072 6574 7572 6e65 6420 7265  r of returned re
+00017f30: 636f 7264 730a 2020 2020 2020 2020 2020  cords.          
+00017f40: 2020 3a74 7970 6520 6d61 785f 7265 7375    :type max_resu
+00017f50: 6c74 733a 2069 6e74 0a20 2020 2020 2020  lts: int.       
+00017f60: 2020 2020 203a 7265 7475 726e 3a20 6c69       :return: li
+00017f70: 7374 206f 6620 7265 7375 6c74 730a 2020  st of results.  
+00017f80: 2020 2020 2020 2020 2020 3a72 7479 7065            :rtype
+00017f90: 3a20 6c69 7374 0a20 2020 2020 2020 2022  : list.        "
+00017fa0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+00017fb0: 7420 6973 696e 7374 616e 6365 286d 6178  t isinstance(max
+00017fc0: 5f72 6573 756c 7473 2c20 696e 7429 3a0a  _results, int):.
+00017fd0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00017fe0: 6520 5772 6f6e 6749 6e70 7574 4572 726f  e WrongInputErro
+00017ff0: 7228 226d 6178 5f72 6573 756c 7473 2070  r("max_results p
+00018000: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+00018010: 2069 6e74 6567 6572 2e22 290a 0a20 2020   integer.")..   
+00018020: 2020 2020 2072 6573 756c 7473 203d 205b       results = [
+00018030: 5d0a 2020 2020 2020 2020 6e65 7874 5f70  ].        next_p
+00018040: 6167 6520 3d20 4e6f 6e65 0a0a 2020 2020  age = None..    
+00018050: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
+00018060: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+00018070: 6f6e 7365 203d 2073 656c 662e 6e65 7477  onse = self.netw
+00018080: 6f72 6b5f 6669 6c65 735f 6672 6f6d 5f69  ork_files_from_i
+00018090: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
+000180a0: 2020 2069 705f 6164 6472 3d69 705f 6164     ip_addr=ip_ad
+000180b0: 6472 2c0a 2020 2020 2020 2020 2020 2020  dr,.            
+000180c0: 2020 2020 6578 7465 6e64 6564 5f72 6573      extended_res
+000180d0: 756c 7473 3d65 7874 656e 6465 645f 7265  ults=extended_re
+000180e0: 7375 6c74 732c 0a20 2020 2020 2020 2020  sults,.         
+000180f0: 2020 2020 2020 2063 6c61 7373 6966 6963         classific
+00018100: 6174 696f 6e3d 636c 6173 7369 6669 6361  ation=classifica
+00018110: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+00018120: 2020 2020 2020 7061 6765 3d6e 6578 745f        page=next_
+00018130: 7061 6765 2c0a 2020 2020 2020 2020 2020  page,.          
+00018140: 2020 2020 2020 7061 6765 5f73 697a 653d        page_size=
+00018150: 7061 6765 5f73 697a 650a 2020 2020 2020  page_size.      
+00018160: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00018170: 2020 2020 2072 6573 706f 6e73 655f 6a73       response_js
+00018180: 6f6e 203d 2072 6573 706f 6e73 652e 6a73  on = response.js
+00018190: 6f6e 2829 0a0a 2020 2020 2020 2020 2020  on()..          
+000181a0: 2020 646f 776e 6c6f 6164 6564 5f66 696c    downloaded_fil
+000181b0: 6573 203d 2072 6573 706f 6e73 655f 6a73  es = response_js
+000181c0: 6f6e 2e67 6574 2822 646f 776e 6c6f 6164  on.get("download
+000181d0: 6564 5f66 696c 6573 222c 205b 5d29 0a20  ed_files", []). 
+000181e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000181f0: 7473 2e65 7874 656e 6428 646f 776e 6c6f  ts.extend(downlo
+00018200: 6164 6564 5f66 696c 6573 290a 0a20 2020  aded_files)..   
+00018210: 2020 2020 2020 2020 206e 6578 745f 7061           next_pa
+00018220: 6765 203d 2072 6573 706f 6e73 655f 6a73  ge = response_js
+00018230: 6f6e 2e67 6574 2822 6e65 7874 5f70 6167  on.get("next_pag
+00018240: 6522 2c20 4e6f 6e65 290a 0a20 2020 2020  e", None)..     
+00018250: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
+00018260: 7375 6c74 7329 203e 3d20 6d61 785f 7265  sults) >= max_re
+00018270: 7375 6c74 7320 6f72 206e 6f74 206e 6578  sults or not nex
+00018280: 745f 7061 6765 3a0a 2020 2020 2020 2020  t_page:.        
+00018290: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
+000182a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000182b0: 7375 6c74 735b 3a6d 6178 5f72 6573 756c  sults[:max_resul
+000182c0: 7473 5d0a 0a20 2020 2064 6566 205f 5f69  ts]..    def __i
+000182d0: 705f 6164 6472 5f65 6e64 706f 696e 7473  p_addr_endpoints
+000182e0: 2873 656c 662c 2069 705f 6164 6472 2c20  (self, ip_addr, 
+000182f0: 7370 6563 6966 6963 5f65 6e64 706f 696e  specific_endpoin
+00018300: 742c 2070 6172 616d 733d 4e6f 6e65 293a  t, params=None):
+00018310: 0a20 2020 2020 2020 2022 2222 5072 6976  .        """Priv
+00018320: 6174 6520 6d65 7468 6f64 2066 6f72 2061  ate method for a
+00018330: 6c6c 2049 5020 7265 6c61 7465 6420 656e  ll IP related en
+00018340: 6470 6f69 6e74 7320 6672 6f6d 2074 6865  dpoints from the
+00018350: 204e 6574 776f 726b 2054 6872 6561 7420   Network Threat 
+00018360: 496e 7465 6c6c 6967 656e 6365 2041 5049  Intelligence API
+00018370: 2e0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
+00018380: 6172 616d 2069 705f 6164 6472 3a20 7265  aram ip_addr: re
+00018390: 7175 6573 7465 6420 4950 2061 6464 7265  quested IP addre
+000183a0: 7373 0a20 2020 2020 2020 2020 2020 203a  ss.            :
+000183b0: 7479 7065 2069 705f 6164 6472 3a20 7374  type ip_addr: st
+000183c0: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
+000183d0: 6172 616d 2073 7065 6369 6669 635f 656e  aram specific_en
+000183e0: 6470 6f69 6e74 3a20 7265 7175 6573 7465  dpoint: requeste
+000183f0: 6420 656e 6470 6f69 6e74 2073 7472 696e  d endpoint strin
+00018400: 670a 2020 2020 2020 2020 2020 2020 3a74  g.            :t
+00018410: 7970 6520 7370 6563 6966 6963 5f65 6e64  ype specific_end
+00018420: 706f 696e 743a 2073 7472 0a20 2020 2020  point: str.     
+00018430: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00018440: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+00018450: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
+00018460: 7565 7374 732e 5265 7370 6f6e 7365 0a20  uests.Response. 
+00018470: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00018480: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00018490: 616e 6365 2869 705f 6164 6472 2c20 7374  ance(ip_addr, st
+000184a0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000184b0: 7261 6973 6520 5772 6f6e 6749 6e70 7574  raise WrongInput
+000184c0: 4572 726f 7228 2269 705f 6164 6472 2070  Error("ip_addr p
+000184d0: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+000184e0: 2073 7472 696e 672e 2229 0a0a 2020 2020   string.")..    
+000184f0: 2020 2020 656e 6470 6f69 6e74 203d 2073      endpoint = s
+00018500: 7065 6369 6669 635f 656e 6470 6f69 6e74  pecific_endpoint
+00018510: 2e66 6f72 6d61 7428 6970 3d69 705f 6164  .format(ip=ip_ad
+00018520: 6472 290a 0a20 2020 2020 2020 2075 726c  dr)..        url
+00018530: 203d 2073 656c 662e 5f75 726c 2e66 6f72   = self._url.for
+00018540: 6d61 7428 656e 6470 6f69 6e74 3d65 6e64  mat(endpoint=end
+00018550: 706f 696e 7429 0a0a 2020 2020 2020 2020  point)..        
+00018560: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00018570: 5f5f 6765 745f 7265 7175 6573 7428 7572  __get_request(ur
+00018580: 6c3d 7572 6c2c 2070 6172 616d 733d 7061  l=url, params=pa
+00018590: 7261 6d73 290a 0a20 2020 2020 2020 2073  rams)..        s
+000185a0: 656c 662e 5f5f 7261 6973 655f 6f6e 5f65  elf.__raise_on_e
+000185b0: 7272 6f72 2872 6573 706f 6e73 6529 0a0a  rror(response)..
+000185c0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000185d0: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
+000185e0: 205f 5f67 6574 5f74 6f6b 656e 2873 656c   __get_token(sel
+000185f0: 662c 2075 7365 726e 616d 652c 2070 6173  f, username, pas
+00018600: 7377 6f72 6429 3a0a 2020 2020 2020 2020  sword):.        
+00018610: 2222 2252 6574 7572 6e73 2061 6e20 6f62  """Returns an ob
+00018620: 7461 696e 6564 2074 6f6b 656e 2075 7369  tained token usi
+00018630: 6e67 2074 6865 2070 726f 7669 6465 6420  ng the provided 
+00018640: 7573 6572 6e61 6d65 2061 6e64 2070 6173  username and pas
+00018650: 7377 6f72 642e 0a20 2020 2020 2020 2020  sword..         
+00018660: 2020 203a 7265 7475 726e 3a20 746f 6b65     :return: toke
+00018670: 6e20 7374 7269 6e67 0a20 2020 2020 2020  n string.       
+00018680: 2020 2020 203a 7274 7970 653a 2073 7472       :rtype: str
+00018690: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000186a0: 2020 2020 2063 7265 6465 6e74 6961 6c73       credentials
+000186b0: 203d 207b 2275 7365 726e 616d 6522 3a20   = {"username": 
+000186c0: 7573 6572 6e61 6d65 2c20 2270 6173 7377  username, "passw
+000186d0: 6f72 6422 3a20 7061 7373 776f 7264 7d0a  ord": password}.
+000186e0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+000186f0: 6520 3d20 7265 7175 6573 7473 2e70 6f73  e = requests.pos
+00018700: 7428 0a20 2020 2020 2020 2020 2020 2075  t(.            u
+00018710: 726c 3d73 656c 662e 5f68 6f73 7420 2b20  rl=self._host + 
+00018720: 7365 6c66 2e5f 5f54 4f4b 454e 5f45 4e44  self.__TOKEN_END
+00018730: 504f 494e 542c 0a20 2020 2020 2020 2020  POINT,.         
+00018740: 2020 2064 6174 613d 6372 6564 656e 7469     data=credenti
+00018750: 616c 732c 0a20 2020 2020 2020 2020 2020  als,.           
+00018760: 2076 6572 6966 793d 7365 6c66 2e5f 7665   verify=self._ve
+00018770: 7269 6679 2c0a 2020 2020 2020 2020 2020  rify,.          
+00018780: 2020 7072 6f78 6965 733d 7365 6c66 2e5f    proxies=self._
+00018790: 7072 6f78 6965 730a 2020 2020 2020 2020  proxies.        
+000187a0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000187b0: 5f5f 7261 6973 655f 6f6e 5f65 7272 6f72  __raise_on_error
+000187c0: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+000187d0: 2020 2020 746f 6b65 6e20 3d20 7265 7370      token = resp
+000187e0: 6f6e 7365 2e6a 736f 6e28 292e 6765 7428  onse.json().get(
+000187f0: 2274 6f6b 656e 2229 0a0a 2020 2020 2020  "token")..      
+00018800: 2020 7265 7475 726e 2074 6f6b 656e 0a0a    return token..
+00018810: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+00018820: 640a 2020 2020 6465 6620 5f5f 6372 6561  d.    def __crea
+00018830: 7465 5f70 6f73 745f 7061 796c 6f61 6428  te_post_payload(
+00018840: 6375 7374 6f6d 5f66 696c 656e 616d 653d  custom_filename=
+00018850: 4e6f 6e65 2c20 6669 6c65 5f75 726c 3d4e  None, file_url=N
+00018860: 6f6e 652c 2020 6372 6177 6c65 723d 4e6f  one,  crawler=No
+00018870: 6e65 2c20 6172 6368 6976 655f 7061 7373  ne, archive_pass
+00018880: 776f 7264 3d4e 6f6e 652c 0a20 2020 2020  word=None,.     
+00018890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188a0: 2020 2020 2020 2020 2072 6c5f 636c 6f75           rl_clou
+000188b0: 645f 7361 6e64 626f 785f 706c 6174 666f  d_sandbox_platfo
+000188c0: 726d 3d4e 6f6e 652c 2074 6167 733d 4e6f  rm=None, tags=No
+000188d0: 6e65 2c20 636f 6d6d 656e 743d 4e6f 6e65  ne, comment=None
+000188e0: 2c20 636c 6f75 645f 616e 616c 7973 6973  , cloud_analysis
+000188f0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00018900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018910: 2020 2020 2063 6c61 7373 6966 6963 6174       classificat
+00018920: 696f 6e3d 4e6f 6e65 2c20 7269 736b 5f73  ion=None, risk_s
+00018930: 636f 7265 3d4e 6f6e 652c 2074 6872 6561  core=None, threa
+00018940: 745f 706c 6174 666f 726d 3d4e 6f6e 652c  t_platform=None,
+00018950: 2074 6872 6561 745f 7479 7065 3d4e 6f6e   threat_type=Non
+00018960: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00018970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018980: 2074 6872 6561 745f 6e61 6d65 3d4e 6f6e   threat_name=Non
+00018990: 652c 206e 616d 653d 4e6f 6e65 2c20 636f  e, name=None, co
+000189a0: 6e74 656e 743d 4e6f 6e65 2c20 7075 626c  ntent=None, publ
+000189b0: 6973 683d 4e6f 6e65 2c20 7469 636c 6f75  ish=None, ticlou
+000189c0: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
+000189d0: 2022 2222 4163 6365 7074 7320 6f70 7469   """Accepts opti
+000189e0: 6f6e 616c 2066 6965 6c64 7320 616e 6420  onal fields and 
+000189f0: 7265 7475 726e 7320 6120 666f 726d 6564  returns a formed
+00018a00: 2064 6963 7469 6f6e 6172 7920 6f66 2074   dictionary of t
+00018a10: 686f 7365 2066 6965 6c64 732e 0a20 2020  hose fields..   
+00018a20: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00018a30: 6375 7374 6f6d 5f66 696c 656e 616d 653a  custom_filename:
+00018a40: 2063 7573 746f 6d20 6669 6c65 206e 616d   custom file nam
+00018a50: 6520 666f 7220 7570 6c6f 6164 0a20 2020  e for upload.   
+00018a60: 2020 2020 2020 2020 203a 7479 7065 2063           :type c
+00018a70: 7573 746f 6d5f 6669 6c65 6e61 6d65 3a20  ustom_filename: 
+00018a80: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00018a90: 3a70 6172 616d 2066 696c 655f 7572 6c3a  :param file_url:
+00018aa0: 2055 524c 2066 726f 6d20 7768 6963 6820   URL from which 
+00018ab0: 7468 6520 6170 706c 6961 6e63 6520 7368  the appliance sh
+00018ac0: 6f75 6c64 2064 6f77 6e6c 6f61 6420 7468  ould download th
+00018ad0: 6520 6461 7461 0a20 2020 2020 2020 2020  e data.         
+00018ae0: 2020 203a 7479 7065 2066 696c 655f 7572     :type file_ur
+00018af0: 6c3a 2073 7472 0a20 2020 2020 2020 2020  l: str.         
+00018b00: 2020 203a 7061 7261 6d20 6372 6177 6c65     :param crawle
+00018b10: 723a 2063 7261 776c 6572 206d 6574 686f  r: crawler metho
+00018b20: 6420 286c 6f63 616c 206f 7220 636c 6f75  d (local or clou
+00018b30: 6429 0a20 2020 2020 2020 2020 2020 203a  d).            :
+00018b40: 7479 7065 2063 7261 776c 6572 3a20 7374  type crawler: st
+00018b50: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
+00018b60: 6172 616d 2061 7263 6869 7665 5f70 6173  aram archive_pas
+00018b70: 7377 6f72 643a 2070 6173 7377 6f72 642c  sword: password,
+00018b80: 2069 6620 6669 6c65 2069 7320 6120 7061   if file is a pa
+00018b90: 7373 776f 7264 2d70 726f 7465 6374 6564  ssword-protected
+00018ba0: 2061 7263 6869 7665 0a20 2020 2020 2020   archive.       
+00018bb0: 2020 2020 203a 7479 7065 2061 7263 6869       :type archi
+00018bc0: 7665 5f70 6173 7377 6f72 643a 2073 7472  ve_password: str
+00018bd0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+00018be0: 7261 6d20 726c 5f63 6c6f 7564 5f73 616e  ram rl_cloud_san
+00018bf0: 6462 6f78 5f70 6c61 7466 6f72 6d3a 2043  dbox_platform: C
+00018c00: 6c6f 7564 2053 616e 6462 6f78 2070 6c61  loud Sandbox pla
+00018c10: 7466 6f72 6d20 2877 696e 646f 7773 372c  tform (windows7,
+00018c20: 2077 696e 646f 7773 3130 206f 7220 6d61   windows10 or ma
+00018c30: 636f 735f 3131 290a 2020 2020 2020 2020  cos_11).        
+00018c40: 2020 2020 3a74 7970 6520 726c 5f63 6c6f      :type rl_clo
+00018c50: 7564 5f73 616e 6462 6f78 5f70 6c61 7466  ud_sandbox_platf
+00018c60: 6f72 6d3a 2073 7472 0a20 2020 2020 2020  orm: str.       
+00018c70: 2020 2020 203a 7061 7261 6d20 7461 6773       :param tags
+00018c80: 3a20 6120 7374 7269 6e67 206f 6620 636f  : a string of co
+00018c90: 6d6d 6120 7365 7061 7261 7465 6420 7461  mma separated ta
+00018ca0: 6773 0a20 2020 2020 2020 2020 2020 203a  gs.            :
+00018cb0: 7479 7065 2074 6167 733a 2073 7472 0a20  type tags: str. 
+00018cc0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+00018cd0: 6d20 636f 6d6d 656e 743a 2063 6f6d 6d65  m comment: comme
+00018ce0: 6e74 2073 7472 696e 670a 2020 2020 2020  nt string.      
+00018cf0: 2020 2020 2020 3a74 7970 6520 636f 6d6d        :type comm
+00018d00: 656e 743a 2073 7472 0a20 2020 2020 2020  ent: str.       
+00018d10: 2020 2020 203a 7061 7261 6d20 636c 6f75       :param clou
+00018d20: 645f 616e 616c 7973 6973 3a20 7573 6520  d_analysis: use 
+00018d30: 636c 6f75 6420 616e 616c 7973 6973 0a20  cloud analysis. 
+00018d40: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00018d50: 2063 6c6f 7564 5f61 6e61 6c79 7369 733a   cloud_analysis:
+00018d60: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
+00018d70: 2020 3a70 6172 616d 2063 6c61 7373 6966    :param classif
+00018d80: 6963 6174 696f 6e3a 2027 676f 6f64 7761  ication: 'goodwa
+00018d90: 7265 272c 2027 7375 7370 6963 696f 7573  re', 'suspicious
+00018da0: 2720 6f72 2027 6d61 6c69 6369 6f75 7327  ' or 'malicious'
+00018db0: 0a20 2020 2020 2020 2020 2020 203a 7479  .            :ty
+00018dc0: 7065 2063 6c61 7373 6966 6963 6174 696f  pe classificatio
+00018dd0: 6e3a 2073 7472 0a20 2020 2020 2020 2020  n: str.         
+00018de0: 2020 203a 7061 7261 6d20 7269 736b 5f73     :param risk_s
+00018df0: 636f 7265 3a20 4966 2073 7065 6369 6669  core: If specifi
+00018e00: 6564 2c20 6974 206d 7573 7420 6265 2077  ed, it must be w
+00018e10: 6974 6869 6e20 7261 6e67 6520 666f 7220  ithin range for 
+00018e20: 7468 6520 7370 6563 6966 6965 6420 636c  the specified cl
+00018e30: 6173 7369 6669 6361 7469 6f6e 2e20 4966  assification. If
+00018e40: 206e 6f74 2073 7065 6369 6669 6564 2c0a   not specified,.
+00018e50: 2020 2020 2020 2020 2020 2020 6120 6465              a de
+00018e60: 6661 756c 7420 7661 6c75 6520 6973 2075  fault value is u
+00018e70: 7365 643a 2047 6f6f 6477 6172 653a 2030  sed: Goodware: 0
+00018e80: 2c20 5375 7370 6963 696f 7573 3a20 362c  , Suspicious: 6,
+00018e90: 204d 616c 6963 696f 7573 3a20 3130 0a20   Malicious: 10. 
+00018ea0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00018eb0: 2072 6973 6b5f 7363 6f72 653a 2073 7472   risk_score: str
+00018ec0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+00018ed0: 7261 6d20 7468 7265 6174 5f70 6c61 7466  ram threat_platf
+00018ee0: 6f72 6d3a 2069 6620 7370 6563 6966 6965  orm: if specifie
+00018ef0: 642c 2069 7420 6d75 7374 2062 6520 6f6e  d, it must be on
+00018f00: 2074 6865 2073 7570 706f 7274 6564 206c   the supported l
+00018f10: 6973 7420 2870 6c61 7466 6f72 6d73 2061  ist (platforms a
+00018f20: 6e64 2073 7562 706c 6174 666f 726d 7320  nd subplatforms 
+00018f30: 2d20 7365 650a 2020 2020 2020 2020 2020  - see.          
+00018f40: 2020 6f66 6669 6369 616c 2041 5049 2064    official API d
+00018f50: 6f63 7329 2e20 4966 206e 6f74 2073 7065  ocs). If not spe
+00018f60: 6369 6669 6564 2c20 7468 6520 6465 6661  cified, the defa
+00018f70: 756c 7420 7661 6c75 6520 6973 2027 5769  ult value is 'Wi
+00018f80: 6e33 3227 2e0a 2020 2020 2020 2020 2020  n32'..          
+00018f90: 2020 3a74 7970 6520 7468 7265 6174 5f70    :type threat_p
+00018fa0: 6c61 7466 6f72 6d3a 2073 7472 0a20 2020  latform: str.   
+00018fb0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00018fc0: 7468 7265 6174 5f74 7970 653a 2049 6620  threat_type: If 
+00018fd0: 7370 6563 6966 6965 642c 2069 7420 6d75  specified, it mu
+00018fe0: 7374 2062 6520 6f6e 2074 6865 2073 7570  st be on the sup
+00018ff0: 706f 7274 6564 206c 6973 7420 286d 616c  ported list (mal
+00019000: 7761 7265 2074 7970 6573 202d 2073 6565  ware types - see
+00019010: 2070 6666 6963 6961 6c20 4150 4920 646f   pfficial API do
+00019020: 6373 292e 0a20 2020 2020 2020 2020 2020  cs)..           
+00019030: 2049 6620 6e6f 7420 7370 6563 6966 6965   If not specifie
+00019040: 642c 2074 6865 2064 6566 6175 6c74 2076  d, the default v
+00019050: 616c 7565 2069 7320 274d 616c 7761 7265  alue is 'Malware
+00019060: 272e 0a20 2020 2020 2020 2020 2020 203a  '..            :
+00019070: 7479 7065 2074 6872 6561 745f 7479 7065  type threat_type
+00019080: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+00019090: 2020 3a70 6172 616d 2074 6872 6561 745f    :param threat_
+000190a0: 6e61 6d65 3a20 4966 2073 7065 6369 6669  name: If specifi
+000190b0: 6564 2c20 6d75 7374 2062 6520 616e 2061  ed, must be an a
+000190c0: 6c70 6861 6e75 6d65 7269 6320 7374 7269  lphanumeric stri
+000190d0: 6e67 206e 6f74 206c 6f6e 6765 7220 7468  ng not longer th
+000190e0: 616e 2033 3220 6368 6172 6163 7465 7273  an 32 characters
+000190f0: 2e20 4966 206e 6f74 0a20 2020 2020 2020  . If not.       
+00019100: 2020 2020 2073 7065 6369 6669 6564 2c20       specified, 
+00019110: 7468 6520 6465 6661 756c 7420 7661 6c75  the default valu
+00019120: 6520 6973 2027 4765 6e65 7269 6327 2e0a  e is 'Generic'..
+00019130: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+00019140: 6520 7468 7265 6174 5f6e 616d 653a 2073  e threat_name: s
+00019150: 7472 0a20 2020 2020 2020 2020 2020 203a  tr.            :
+00019160: 7061 7261 6d20 6e61 6d65 3a20 6e61 6d65  param name: name
+00019170: 206f 6620 7468 6520 7275 6c65 7365 7420   of the ruleset 
+00019180: 746f 2063 7265 6174 6520 6f72 2075 7064  to create or upd
+00019190: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
+000191a0: 3a74 7970 6520 6e61 6d65 3a20 7374 720a  :type name: str.
+000191b0: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+000191c0: 616d 2063 6f6e 7465 6e74 3a20 636f 6e74  am content: cont
+000191d0: 656e 7420 6f66 2074 6865 2059 4152 4120  ent of the YARA 
+000191e0: 7275 6c65 7365 7420 746f 2063 7265 6174  ruleset to creat
+000191f0: 6520 6f72 2075 7064 6174 650a 2020 2020  e or update.    
+00019200: 2020 2020 2020 2020 3a74 7970 6520 636f          :type co
+00019210: 6e74 656e 743a 2073 7472 0a20 2020 2020  ntent: str.     
+00019220: 2020 2020 2020 203a 7061 7261 6d20 7075         :param pu
+00019230: 626c 6973 683a 2064 6574 6572 6d69 6e65  blish: determine
+00019240: 7320 7768 6574 6865 7220 7468 6520 7275  s whether the ru
+00019250: 6c65 7365 7420 7368 6f75 6c64 2062 6520  leset should be 
+00019260: 7379 6e63 6872 6f6e 697a 6564 2074 6f20  synchronized to 
+00019270: 6f74 6865 7220 6170 706c 6961 6e63 6573  other appliances
+00019280: 2069 6e20 7468 6520 7361 6d65 0a20 2020   in the same.   
+00019290: 2020 2020 2020 2020 2043 3130 3030 2063           C1000 c
+000192a0: 6c75 7374 6572 0a20 2020 2020 2020 2020  luster.         
+000192b0: 2020 203a 7479 7065 2070 7562 6c69 7368     :type publish
+000192c0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+000192d0: 2020 203a 7061 7261 6d20 7469 636c 6f75     :param ticlou
+000192e0: 643a 2064 6574 6572 6d69 6e65 7320 7768  d: determines wh
+000192f0: 6574 6865 7220 7468 6520 7275 6c65 7365  ether the rulese
+00019300: 7420 7368 6f75 6c64 2062 6520 7379 6e63  t should be sync
+00019310: 6872 6f6e 697a 6564 2077 6974 6820 5469  hronized with Ti
+00019320: 7461 6e69 756d 436c 6f75 6420 6f72 206e  taniumCloud or n
+00019330: 6f74 0a20 2020 2020 2020 2020 2020 203a  ot.            :
+00019340: 7479 7065 2074 6963 6c6f 7564 3a20 626f  type ticloud: bo
+00019350: 6f6c 0a20 2020 2020 2020 2020 2020 203a  ol.            :
+00019360: 7265 7475 726e 3a20 6469 6374 696f 6e61  return: dictiona
+00019370: 7279 206f 6620 6465 6669 6e65 6420 6f70  ry of defined op
+00019380: 7469 6f6e 616c 2066 6965 6c64 7320 6f72  tional fields or
+00019390: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+000193a0: 2020 3a72 7479 7065 3a20 6469 6374 206f    :rtype: dict o
+000193b0: 7220 4e6f 6e65 0a20 2020 2020 2020 2022  r None.        "
+000193c0: 2222 0a20 2020 2020 2020 2069 6620 6375  "".        if cu
+000193d0: 7374 6f6d 5f66 696c 656e 616d 6520 616e  stom_filename an
+000193e0: 6420 6e6f 7420 6973 696e 7374 616e 6365  d not isinstance
+000193f0: 2863 7573 746f 6d5f 6669 6c65 6e61 6d65  (custom_filename
+00019400: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+00019410: 2020 2020 7261 6973 6520 5772 6f6e 6749      raise WrongI
+00019420: 6e70 7574 4572 726f 7228 2263 7573 746f  nputError("custo
+00019430: 6d5f 6669 6c65 6e61 6d65 2070 6172 616d  m_filename param
+00019440: 6574 6572 206d 7573 7420 6265 2073 7472  eter must be str
+00019450: 696e 672e 2229 0a0a 2020 2020 2020 2020  ing.")..        
+00019460: 6966 2074 6167 7320 616e 6420 6e6f 7420  if tags and not 
+00019470: 6973 696e 7374 616e 6365 2874 6167 732c  isinstance(tags,
+00019480: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+00019490: 2020 2072 6169 7365 2057 726f 6e67 496e     raise WrongIn
+000194a0: 7075 7445 7272 6f72 2822 7461 6773 2070  putError("tags p
+000194b0: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+000194c0: 2073 7472 696e 672e 2229 0a0a 2020 2020   string.")..    
+000194d0: 2020 2020 6966 2066 696c 655f 7572 6c3a      if file_url:
+000194e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000194f0: 6e6f 7420 6973 696e 7374 616e 6365 2866  not isinstance(f
+00019500: 696c 655f 7572 6c2c 2073 7472 293a 0a20  ile_url, str):. 
+00019510: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00019520: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
+00019530: 7272 6f72 2822 6669 6c65 5f75 726c 2070  rror("file_url p
+00019540: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+00019550: 2073 7472 696e 672e 2229 0a20 2020 2020   string.").     
+00019560: 2020 2020 2020 2069 6620 6e6f 7420 6669         if not fi
+00019570: 6c65 5f75 726c 2e73 7461 7274 7377 6974  le_url.startswit
+00019580: 6828 2822 6874 7470 3a2f 2f22 2c20 2268  h(("http://", "h
+00019590: 7474 7073 3a2f 2f22 2929 3a0a 2020 2020  ttps://")):.    
+000195a0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000195b0: 6520 5772 6f6e 6749 6e70 7574 4572 726f  e WrongInputErro
+000195c0: 7228 2253 7570 706f 7274 6564 2066 696c  r("Supported fil
+000195d0: 655f 7572 6c20 7072 6f74 6f63 6f6c 7320  e_url protocols 
+000195e0: 6172 6520 4854 5450 2061 6e64 2048 5454  are HTTP and HTT
+000195f0: 5053 2e22 290a 0a20 2020 2020 2020 2069  PS.")..        i
+00019600: 6620 6372 6177 6c65 7220 616e 6420 6372  f crawler and cr
+00019610: 6177 6c65 7220 6e6f 7420 696e 2028 2263  awler not in ("c
+00019620: 6c6f 7564 222c 2022 6c6f 6361 6c22 293a  loud", "local"):
+00019630: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00019640: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
+00019650: 6f72 2822 6372 6177 6c65 7220 7061 7261  or("crawler para
+00019660: 6d65 7465 7220 6d75 7374 2062 6520 6569  meter must be ei
+00019670: 7468 6572 2027 636c 6f75 6427 206f 7220  ther 'cloud' or 
+00019680: 276c 6f63 616c 272e 2229 0a0a 2020 2020  'local'.")..    
+00019690: 2020 2020 6966 2061 7263 6869 7665 5f70      if archive_p
+000196a0: 6173 7377 6f72 6420 616e 6420 6e6f 7420  assword and not 
+000196b0: 6973 696e 7374 616e 6365 2861 7263 6869  isinstance(archi
+000196c0: 7665 5f70 6173 7377 6f72 642c 2073 7472  ve_password, str
+000196d0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+000196e0: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
+000196f0: 7272 6f72 2822 6172 6368 6976 655f 7061  rror("archive_pa
+00019700: 7373 776f 7264 2070 6172 616d 6574 6572  ssword parameter
+00019710: 206d 7573 7420 6265 2073 7472 696e 672e   must be string.
+00019720: 2229 0a0a 2020 2020 2020 2020 6966 2072  ")..        if r
+00019730: 6c5f 636c 6f75 645f 7361 6e64 626f 785f  l_cloud_sandbox_
+00019740: 706c 6174 666f 726d 2061 6e64 2072 6c5f  platform and rl_
+00019750: 636c 6f75 645f 7361 6e64 626f 785f 706c  cloud_sandbox_pl
+00019760: 6174 666f 726d 206e 6f74 2069 6e20 4156  atform not in AV
+00019770: 4149 4c41 424c 455f 504c 4154 464f 524d  AILABLE_PLATFORM
+00019780: 533a 0a20 2020 2020 2020 2020 2020 2072  S:.            r
+00019790: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
+000197a0: 7272 6f72 2822 726c 5f63 6c6f 7564 5f73  rror("rl_cloud_s
+000197b0: 616e 6462 6f78 5f70 6c61 7466 6f72 6d20  andbox_platform 
+000197c0: 7061 7261 6d65 7465 7220 6d75 7374 2062  parameter must b
+000197d0: 6520 6f6e 6520 6f64 2074 6865 2066 6f6c  e one od the fol
+000197e0: 6c6f 7769 6e67 3a20 220a 2020 2020 2020  lowing: ".      
+000197f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019800: 2020 2020 2020 2020 2020 2020 227b 706c              "{pl
+00019810: 6174 666f 726d 737d 222e 666f 726d 6174  atforms}".format
+00019820: 2870 6c61 7466 6f72 6d73 3d41 5641 494c  (platforms=AVAIL
+00019830: 4142 4c45 5f50 4c41 5446 4f52 4d53 2929  ABLE_PLATFORMS))
+00019840: 0a0a 2020 2020 2020 2020 6966 2063 6f6d  ..        if com
+00019850: 6d65 6e74 2061 6e64 206e 6f74 2069 7369  ment and not isi
+00019860: 6e73 7461 6e63 6528 636f 6d6d 656e 742c  nstance(comment,
+00019870: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+00019880: 2020 2072 6169 7365 2057 726f 6e67 496e     raise WrongIn
+00019890: 7075 7445 7272 6f72 2822 636f 6d6d 656e  putError("commen
+000198a0: 7420 7061 7261 6d65 7465 7220 6d75 7374  t parameter must
+000198b0: 2062 6520 7374 7269 6e67 2e22 290a 0a20   be string.").. 
+000198c0: 2020 2020 2020 2069 6620 636c 6f75 645f         if cloud_
+000198d0: 616e 616c 7973 6973 206e 6f74 2069 6e20  analysis not in 
+000198e0: 2854 7275 652c 2046 616c 7365 293a 0a20  (True, False):. 
+000198f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00019900: 2057 726f 6e67 496e 7075 7445 7272 6f72   WrongInputError
+00019910: 2822 636c 6f75 645f 616e 616c 7973 6973  ("cloud_analysis
+00019920: 2070 6172 616d 6574 6572 206d 7573 7420   parameter must 
+00019930: 6265 2062 6f6f 6c65 616e 2e22 290a 0a20  be boolean.").. 
+00019940: 2020 2020 2020 2061 6c6c 6f77 6564 5f63         allowed_c
+00019950: 6c61 7373 6966 6963 6174 696f 6e73 5f61  lassifications_a
+00019960: 6e64 5f72 6973 6b5f 7363 6f72 6573 203d  nd_risk_scores =
+00019970: 207b 2767 6f6f 6477 6172 6527 3a20 5b30   {'goodware': [0
+00019980: 2c20 312c 2032 2c20 332c 2034 2c20 355d  , 1, 2, 3, 4, 5]
+00019990: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000199a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199c0: 2020 2020 2027 7375 7370 6963 696f 7573       'suspicious
+000199d0: 273a 205b 362c 2037 2c20 382c 2039 2c20  ': [6, 7, 8, 9, 
+000199e0: 3130 5d2c 0a20 2020 2020 2020 2020 2020  10],.           
+000199f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a10: 2020 2020 2020 2020 276d 616c 6963 696f          'malicio
+00019a20: 7573 273a 205b 362c 2037 2c20 382c 2039  us': [6, 7, 8, 9
+00019a30: 2c20 3130 5d7d 0a0a 2020 2020 2020 2020  , 10]}..        
+00019a40: 6966 2063 6c61 7373 6966 6963 6174 696f  if classificatio
+00019a50: 6e20 616e 6420 636c 6173 7369 6669 6361  n and classifica
+00019a60: 7469 6f6e 206e 6f74 2069 6e20 616c 6c6f  tion not in allo
+00019a70: 7765 645f 636c 6173 7369 6669 6361 7469  wed_classificati
+00019a80: 6f6e 735f 616e 645f 7269 736b 5f73 636f  ons_and_risk_sco
+00019a90: 7265 732e 6b65 7973 2829 3a0a 2020 2020  res.keys():.    
+00019aa0: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
+00019ab0: 6f6e 6749 6e70 7574 4572 726f 7228 2263  ongInputError("c
+00019ac0: 6c61 7373 6966 6963 6174 696f 6e20 7061  lassification pa
+00019ad0: 7261 6d65 7465 7220 6d75 7374 2062 6520  rameter must be 
+00019ae0: 736f 6d65 206f 6620 7468 6520 666f 6c6c  some of the foll
+00019af0: 6f77 696e 6720 7661 6c75 6573 3a22 202b  owing values:" +
+00019b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b20: 2020 2022 2022 2e6a 6f69 6e28 7374 7228     " ".join(str(
+00019b30: 6b65 7929 2066 6f72 206b 6579 2069 6e20  key) for key in 
+00019b40: 616c 6c6f 7765 645f 636c 6173 7369 6669  allowed_classifi
+00019b50: 6361 7469 6f6e 735f 616e 645f 7269 736b  cations_and_risk
+00019b60: 5f73 636f 7265 732e 6b65 7973 2829 2929  _scores.keys()))
+00019b70: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00019b80: 2020 2020 2020 2020 2020 2069 6620 7269             if ri
+00019b90: 736b 5f73 636f 7265 2061 6e64 2072 6973  sk_score and ris
+00019ba0: 6b5f 7363 6f72 6520 6e6f 7420 696e 2061  k_score not in a
+00019bb0: 6c6c 6f77 6564 5f63 6c61 7373 6966 6963  llowed_classific
+00019bc0: 6174 696f 6e73 5f61 6e64 5f72 6973 6b5f  ations_and_risk_
+00019bd0: 7363 6f72 6573 5b63 6c61 7373 6966 6963  scores[classific
+00019be0: 6174 696f 6e5d 3a0a 2020 2020 2020 2020  ation]:.        
+00019bf0: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
+00019c00: 6f6e 6749 6e70 7574 4572 726f 7228 6622  ongInputError(f"
+00019c10: 7269 736b 5f73 636f 7265 207b 7269 736b  risk_score {risk
+00019c20: 5f73 636f 7265 7d20 6973 206e 6f74 2061  _score} is not a
+00019c30: 6c6c 6f77 6564 2066 6f72 2063 6c61 7373  llowed for class
+00019c40: 6966 6963 6174 696f 6e20 277b 636c 6173  ification '{clas
+00019c50: 7369 6669 6361 7469 6f6e 7d27 2e22 290a  sification}'.").
+00019c60: 0a20 2020 2020 2020 2069 6620 7468 7265  .        if thre
+00019c70: 6174 5f70 6c61 7466 6f72 6d20 616e 6420  at_platform and 
+00019c80: 6e6f 7420 6973 696e 7374 616e 6365 2874  not isinstance(t
+00019c90: 6872 6561 745f 706c 6174 666f 726d 2c20  hreat_platform, 
+00019ca0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00019cb0: 2020 7261 6973 6520 5772 6f6e 6749 6e70    raise WrongInp
+00019cc0: 7574 4572 726f 7228 2274 6872 6561 745f  utError("threat_
+00019cd0: 706c 6174 666f 726d 2070 6172 616d 6574  platform paramet
+00019ce0: 6572 206d 7573 7420 6265 2073 7472 696e  er must be strin
+00019cf0: 672e 2229 0a0a 2020 2020 2020 2020 6966  g.")..        if
+00019d00: 2074 6872 6561 745f 7479 7065 2061 6e64   threat_type and
+00019d10: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+00019d20: 7468 7265 6174 5f74 7970 652c 2073 7472  threat_type, str
+00019d30: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00019d40: 6169 7365 2057 726f 6e67 496e 7075 7445  aise WrongInputE
+00019d50: 7272 6f72 2822 7468 7265 6174 5f74 7970  rror("threat_typ
+00019d60: 6520 7061 7261 6d65 7465 7220 6d75 7374  e parameter must
+00019d70: 2062 6520 7374 7269 6e67 2e22 290a 0a20   be string.").. 
+00019d80: 2020 2020 2020 2069 6620 7468 7265 6174         if threat
+00019d90: 5f6e 616d 6520 616e 6420 6e6f 7420 6973  _name and not is
+00019da0: 696e 7374 616e 6365 2874 6872 6561 745f  instance(threat_
+00019db0: 6e61 6d65 2c20 7374 7229 3a0a 2020 2020  name, str):.    
+00019dc0: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
+00019dd0: 6f6e 6749 6e70 7574 4572 726f 7228 2274  ongInputError("t
+00019de0: 6872 6561 745f 7479 7065 2070 6172 616d  hreat_type param
+00019df0: 6574 6572 206d 7573 7420 6265 2073 7472  eter must be str
+00019e00: 696e 672e 2229 0a0a 2020 2020 2020 2020  ing.")..        
+00019e10: 6966 206e 616d 6520 616e 6420 6e6f 7420  if name and not 
+00019e20: 6973 696e 7374 616e 6365 286e 616d 652c  isinstance(name,
+00019e30: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+00019e40: 2020 2072 6169 7365 2057 726f 6e67 496e     raise WrongIn
+00019e50: 7075 7445 7272 6f72 2822 6e61 6d65 2070  putError("name p
+00019e60: 6172 616d 6574 6572 206d 7573 7420 6265  arameter must be
+00019e70: 2073 7472 696e 672e 2229 0a0a 2020 2020   string.")..    
+00019e80: 2020 2020 6966 2063 6f6e 7465 6e74 2061      if content a
+00019e90: 6e64 206e 6f74 2069 7369 6e73 7461 6e63  nd not isinstanc
+00019ea0: 6528 636f 6e74 656e 742c 2073 7472 293a  e(content, str):
+00019eb0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00019ec0: 7365 2057 726f 6e67 496e 7075 7445 7272  se WrongInputErr
+00019ed0: 6f72 2822 636f 6e74 656e 7420 7061 7261  or("content para
+00019ee0: 6d65 7465 7220 6d75 7374 2062 6520 7374  meter must be st
+00019ef0: 7269 6e67 2e22 290a 0a20 2020 2020 2020  ring.")..       
+00019f00: 2069 6620 7075 626c 6973 6820 616e 6420   if publish and 
+00019f10: 7075 626c 6973 6820 6e6f 7420 696e 2028  publish not in (
+00019f20: 5472 7565 2c20 4661 6c73 6529 3a0a 2020  True, False):.  
+00019f30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00019f40: 5772 6f6e 6749 6e70 7574 4572 726f 7228  WrongInputError(
+00019f50: 2270 7562 6c69 7368 2070 6172 616d 6574  "publish paramet
+00019f60: 6572 206d 7573 7420 6265 2062 6f6f 6c65  er must be boole
+00019f70: 616e 2e22 290a 0a20 2020 2020 2020 2069  an.")..        i
+00019f80: 6620 7469 636c 6f75 6420 616e 6420 7469  f ticloud and ti
+00019f90: 636c 6f75 6420 6e6f 7420 696e 2028 5472  cloud not in (Tr
+00019fa0: 7565 2c20 4661 6c73 6529 3a0a 2020 2020  ue, False):.    
+00019fb0: 2020 2020 2020 2020 7261 6973 6520 5772          raise Wr
+00019fc0: 6f6e 6749 6e70 7574 4572 726f 7228 2274  ongInputError("t
+00019fd0: 6963 6c6f 7564 2070 6172 616d 6574 6572  icloud parameter
+00019fe0: 206d 7573 7420 6265 2062 6f6f 6c65 616e   must be boolean
+00019ff0: 2e22 290a 0a20 2020 2020 2020 2064 6174  .")..        dat
+0001a000: 6120 3d20 7b7d 0a0a 2020 2020 2020 2020  a = {}..        
+0001a010: 6966 2063 7573 746f 6d5f 6669 6c65 6e61  if custom_filena
+0001a020: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+0001a030: 6461 7461 5b22 6669 6c65 6e61 6d65 225d  data["filename"]
+0001a040: 203d 2063 7573 746f 6d5f 6669 6c65 6e61   = custom_filena
+0001a050: 6d65 0a0a 2020 2020 2020 2020 6966 2063  me..        if c
+0001a060: 7261 776c 6572 3a0a 2020 2020 2020 2020  rawler:.        
+0001a070: 2020 2020 6461 7461 5b22 6372 6177 6c65      data["crawle
+0001a080: 7222 5d20 3d20 6372 6177 6c65 720a 0a20  r"] = crawler.. 
+0001a090: 2020 2020 2020 2069 6620 6172 6368 6976         if archiv
+0001a0a0: 655f 7061 7373 776f 7264 3a0a 2020 2020  e_password:.    
+0001a0b0: 2020 2020 2020 2020 6461 7461 5b22 6172          data["ar
+0001a0c0: 6368 6976 655f 7061 7373 776f 7264 225d  chive_password"]
+0001a0d0: 203d 2061 7263 6869 7665 5f70 6173 7377   = archive_passw
+0001a0e0: 6f72 640a 0a20 2020 2020 2020 2069 6620  ord..        if 
+0001a0f0: 726c 5f63 6c6f 7564 5f73 616e 6462 6f78  rl_cloud_sandbox
+0001a100: 5f70 6c61 7466 6f72 6d3a 0a20 2020 2020  _platform:.     
+0001a110: 2020 2020 2020 2064 6174 615b 2272 6c5f         data["rl_
+0001a120: 636c 6f75 645f 7361 6e64 626f 785f 706c  cloud_sandbox_pl
+0001a130: 6174 666f 726d 225d 203d 2072 6c5f 636c  atform"] = rl_cl
+0001a140: 6f75 645f 7361 6e64 626f 785f 706c 6174  oud_sandbox_plat
+0001a150: 666f 726d 0a0a 2020 2020 2020 2020 6966  form..        if
+0001a160: 2074 6167 733a 0a20 2020 2020 2020 2020   tags:.         
+0001a170: 2020 2064 6174 615b 2274 6167 7322 5d20     data["tags"] 
+0001a180: 3d20 7461 6773 0a0a 2020 2020 2020 2020  = tags..        
+0001a190: 6966 2063 6f6d 6d65 6e74 3a0a 2020 2020  if comment:.    
+0001a1a0: 2020 2020 2020 2020 6461 7461 5b22 636f          data["co
+0001a1b0: 6d6d 656e 7422 5d20 3d20 636f 6d6d 656e  mment"] = commen
+0001a1c0: 740a 0a20 2020 2020 2020 2069 6620 636c  t..        if cl
+0001a1d0: 6f75 645f 616e 616c 7973 6973 3a0a 2020  oud_analysis:.  
+0001a1e0: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
+0001a1f0: 616e 616c 7973 6973 225d 203d 2022 636c  analysis"] = "cl
+0001a200: 6f75 6422 0a0a 2020 2020 2020 2020 6966  oud"..        if
+0001a210: 2066 696c 655f 7572 6c3a 0a20 2020 2020   file_url:.     
+0001a220: 2020 2020 2020 2064 6174 615b 2275 726c         data["url
+0001a230: 225d 203d 2066 696c 655f 7572 6c0a 0a20  "] = file_url.. 
+0001a240: 2020 2020 2020 2069 6620 636c 6173 7369         if classi
+0001a250: 6669 6361 7469 6f6e 3a0a 2020 2020 2020  fication:.      
+0001a260: 2020 2020 2020 6461 7461 5b27 636c 6173        data['clas
+0001a270: 7369 6669 6361 7469 6f6e 275d 203d 2063  sification'] = c
+0001a280: 6c61 7373 6966 6963 6174 696f 6e0a 0a20  lassification.. 
+0001a290: 2020 2020 2020 2069 6620 7269 736b 5f73         if risk_s
+0001a2a0: 636f 7265 3a0a 2020 2020 2020 2020 2020  core:.          
+0001a2b0: 2020 6461 7461 5b27 7269 736b 5f73 636f    data['risk_sco
+0001a2c0: 7265 275d 203d 2072 6973 6b5f 7363 6f72  re'] = risk_scor
+0001a2d0: 650a 0a20 2020 2020 2020 2069 6620 7468  e..        if th
+0001a2e0: 7265 6174 5f70 6c61 7466 6f72 6d3a 0a20  reat_platform:. 
+0001a2f0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+0001a300: 2774 6872 6561 745f 706c 6174 666f 726d  'threat_platform
+0001a310: 275d 203d 2074 6872 6561 745f 706c 6174  '] = threat_plat
+0001a320: 666f 726d 0a0a 2020 2020 2020 2020 6966  form..        if
+0001a330: 2074 6872 6561 745f 7479 7065 3a0a 2020   threat_type:.  
+0001a340: 2020 2020 2020 2020 2020 6461 7461 5b27            data['
+0001a350: 7468 7265 6174 5f74 7970 6527 5d20 3d20  threat_type'] = 
+0001a360: 7468 7265 6174 5f74 7970 650a 0a20 2020  threat_type..   
+0001a370: 2020 2020 2069 6620 7468 7265 6174 5f6e       if threat_n
+0001a380: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+0001a390: 2064 6174 615b 2774 6872 6561 745f 6e61   data['threat_na
+0001a3a0: 6d65 275d 203d 2074 6872 6561 745f 6e61  me'] = threat_na
+0001a3b0: 6d65 0a0a 2020 2020 2020 2020 6966 206e  me..        if n
+0001a3c0: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+0001a3d0: 2064 6174 615b 276e 616d 6527 5d20 3d20   data['name'] = 
+0001a3e0: 6e61 6d65 0a0a 2020 2020 2020 2020 6966  name..        if
+0001a3f0: 2063 6f6e 7465 6e74 3a0a 2020 2020 2020   content:.      
+0001a400: 2020 2020 2020 6461 7461 5b27 636f 6e74        data['cont
+0001a410: 656e 7427 5d20 3d20 636f 6e74 656e 740a  ent'] = content.
+0001a420: 0a20 2020 2020 2020 2069 6620 7075 626c  .        if publ
+0001a430: 6973 683a 0a20 2020 2020 2020 2020 2020  ish:.           
+0001a440: 2064 6174 615b 2770 7562 6c69 7368 275d   data['publish']
+0001a450: 203d 2070 7562 6c69 7368 0a0a 2020 2020   = publish..    
+0001a460: 2020 2020 6966 2074 6963 6c6f 7564 3a0a      if ticloud:.
+0001a470: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0001a480: 5b27 7469 636c 6f75 6427 5d20 3d20 7469  ['ticloud'] = ti
+0001a490: 636c 6f75 640a 0a20 2020 2020 2020 2069  cloud..        i
+0001a4a0: 6620 6e6f 7420 6461 7461 3a0a 2020 2020  f not data:.    
+0001a4b0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+0001a4c0: 6f6e 650a 0a20 2020 2020 2020 2072 6574  one..        ret
+0001a4d0: 7572 6e20 6461 7461 0a0a 2020 2020 6465  urn data..    de
+0001a4e0: 6620 5f5f 616e 616c 7973 6973 5f69 735f  f __analysis_is_
+0001a4f0: 6669 6e69 7368 6564 2873 656c 662c 2073  finished(self, s
+0001a500: 616d 706c 655f 6861 7368 6573 293a 0a20  ample_hashes):. 
+0001a510: 2020 2020 2020 2022 2222 4163 6365 7074         """Accept
+0001a520: 7320 6120 6c69 7374 206f 6620 6861 7368  s a list of hash
+0001a530: 6573 2061 6e64 2072 6574 7572 6e73 2062  es and returns b
+0001a540: 6f6f 6c65 616e 2066 6f72 2074 6865 2067  oolean for the g
+0001a550: 6574 5f72 6573 756c 7473 206d 6574 686f  et_results metho
+0001a560: 642e 0a20 2020 2020 2020 2020 2020 203a  d..            :
+0001a570: 7061 7261 6d20 7361 6d70 6c65 5f68 6173  param sample_has
+0001a580: 6865 733a 206c 6973 7420 6f66 2068 6173  hes: list of has
+0001a590: 6820 7374 7269 6e67 730a 2020 2020 2020  h strings.      
+0001a5a0: 2020 2020 2020 3a74 7970 6520 7361 6d70        :type samp
+0001a5b0: 6c65 5f68 6173 6865 733a 206c 6973 745b  le_hashes: list[
+0001a5c0: 7374 725d 0a20 2020 2020 2020 2020 2020  str].           
+0001a5d0: 203a 7265 7475 726e 3a20 626f 6f6c 6561   :return: boolea
+0001a5e0: 6e20 666f 7220 7072 6f63 6573 7369 6e67  n for processing
+0001a5f0: 2073 7461 7475 732e 0a20 2020 2020 2020   status..       
+0001a600: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+0001a610: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
+0001a620: 2020 2020 2020 6461 7461 203d 207b 2268        data = {"h
+0001a630: 6173 685f 7661 6c75 6573 223a 2073 616d  ash_values": sam
+0001a640: 706c 655f 6861 7368 6573 7d0a 2020 2020  ple_hashes}.    
+0001a650: 2020 2020 7061 7261 6d73 203d 207b 2273      params = {"s
+0001a660: 7461 7475 7322 3a20 2270 726f 6365 7373  tatus": "process
+0001a670: 6564 227d 0a0a 2020 2020 2020 2020 7572  ed"}..        ur
+0001a680: 6c20 3d20 7365 6c66 2e5f 7572 6c2e 666f  l = self._url.fo
+0001a690: 726d 6174 2865 6e64 706f 696e 743d 7365  rmat(endpoint=se
+0001a6a0: 6c66 2e5f 5f43 4845 434b 5f53 5441 5455  lf.__CHECK_STATU
+0001a6b0: 535f 454e 4450 4f49 4e54 290a 0a20 2020  S_ENDPOINT)..   
+0001a6c0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0001a6d0: 7365 6c66 2e5f 5f70 6f73 745f 7265 7175  self.__post_requ
+0001a6e0: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
+0001a6f0: 2075 726c 3d75 726c 2c0a 2020 2020 2020   url=url,.      
+0001a700: 2020 2020 2020 6461 7461 3d64 6174 612c        data=data,
+0001a710: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+0001a720: 616d 733d 7061 7261 6d73 0a20 2020 2020  ams=params.     
+0001a730: 2020 2029 0a0a 2020 2020 2020 2020 7365     )..        se
+0001a740: 6c66 2e5f 5f72 6169 7365 5f6f 6e5f 6572  lf.__raise_on_er
+0001a750: 726f 7228 7265 7370 6f6e 7365 290a 0a20  ror(response).. 
+0001a760: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
+0001a770: 7370 6f6e 7365 2e6a 736f 6e28 292e 6765  sponse.json().ge
+0001a780: 7428 2272 6573 756c 7473 2229 2920 3d3d  t("results")) ==
+0001a790: 206c 656e 2873 616d 706c 655f 6861 7368   len(sample_hash
+0001a7a0: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+0001a7b0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
+0001a7c0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001a7d0: 7365 0a0a 2020 2020 6465 6620 5f5f 6765  se..    def __ge
+0001a7e0: 745f 7265 7175 6573 7428 7365 6c66 2c20  t_request(self, 
+0001a7f0: 7572 6c2c 2070 6172 616d 733d 4e6f 6e65  url, params=None
+0001a800: 293a 0a20 2020 2020 2020 2022 2222 4120  ):.        """A 
+0001a810: 6765 6e65 7269 6320 4745 5420 7265 7175  generic GET requ
+0001a820: 6573 7420 6d65 7468 6f64 2066 6f72 2061  est method for a
+0001a830: 6c6c 2041 3130 3030 206d 6574 686f 6473  ll A1000 methods
+0001a840: 2e0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
+0001a850: 6172 616d 2075 726c 3a20 7265 7175 6573  aram url: reques
+0001a860: 7420 5552 4c0a 2020 2020 2020 2020 2020  t URL.          
+0001a870: 2020 3a74 7970 6520 7572 6c3a 2073 7472    :type url: str
+0001a880: 0a20 2020 2020 2020 2020 2020 203a 7265  .            :re
+0001a890: 7475 726e 3a20 7265 7370 6f6e 7365 0a20  turn: response. 
+0001a8a0: 2020 2020 2020 2020 2020 203a 7274 7970             :rtyp
+0001a8b0: 653a 2072 6571 7565 7374 732e 5265 7370  e: requests.Resp
+0001a8c0: 6f6e 7365 0a20 2020 2020 2020 2022 2222  onse.        """
+0001a8d0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+0001a8e0: 6520 3d20 7265 7175 6573 7473 2e67 6574  e = requests.get
+0001a8f0: 280a 2020 2020 2020 2020 2020 2020 7572  (.            ur
+0001a900: 6c3d 7572 6c2c 0a20 2020 2020 2020 2020  l=url,.         
+0001a910: 2020 2076 6572 6966 793d 7365 6c66 2e5f     verify=self._
+0001a920: 7665 7269 6679 2c0a 2020 2020 2020 2020  verify,.        
+0001a930: 2020 2020 7072 6f78 6965 733d 7365 6c66      proxies=self
+0001a940: 2e5f 7072 6f78 6965 732c 0a20 2020 2020  ._proxies,.     
+0001a950: 2020 2020 2020 2068 6561 6465 7273 3d73         headers=s
+0001a960: 656c 662e 5f68 6561 6465 7273 2c0a 2020  elf._headers,.  
+0001a970: 2020 2020 2020 2020 2020 7061 7261 6d73            params
+0001a980: 3d70 6172 616d 730a 2020 2020 2020 2020  =params.        
+0001a990: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0001a9a0: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
+0001a9b0: 6465 6620 5f5f 706f 7374 5f72 6571 7565  def __post_reque
+0001a9c0: 7374 2873 656c 662c 2075 726c 2c20 706f  st(self, url, po
+0001a9d0: 7374 5f6a 736f 6e3d 4e6f 6e65 2c20 6669  st_json=None, fi
+0001a9e0: 6c65 733d 4e6f 6e65 2c20 6461 7461 3d4e  les=None, data=N
+0001a9f0: 6f6e 652c 2070 6172 616d 733d 4e6f 6e65  one, params=None
+0001aa00: 293a 0a20 2020 2020 2020 2022 2222 4120  ):.        """A 
+0001aa10: 6765 6e65 7269 6320 504f 5354 2072 6571  generic POST req
+0001aa20: 7565 7374 206d 6574 686f 6420 666f 7220  uest method for 
+0001aa30: 616c 6c20 4131 3030 3020 6d65 7468 6f64  all A1000 method
+0001aa40: 732e 0a20 2020 2020 2020 2020 2020 203a  s..            :
+0001aa50: 7061 7261 6d20 7572 6c3a 2072 6571 7565  param url: reque
+0001aa60: 7374 2055 524c 0a20 2020 2020 2020 2020  st URL.         
+0001aa70: 2020 203a 7479 7065 2075 726c 3a20 7374     :type url: st
+0001aa80: 720a 2020 2020 2020 2020 2020 2020 3a70  r.            :p
+0001aa90: 6172 616d 2070 6f73 745f 6a73 6f6e 3a20  aram post_json: 
+0001aaa0: 4a53 4f4e 2062 6f64 790a 2020 2020 2020  JSON body.      
+0001aab0: 2020 2020 2020 3a74 7970 6520 706f 7374        :type post
+0001aac0: 5f6a 736f 6e3a 2064 6963 740a 2020 2020  _json: dict.    
+0001aad0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
+0001aae0: 696c 6573 3a20 6669 6c65 7320 746f 2073  iles: files to s
+0001aaf0: 656e 640a 2020 2020 2020 2020 2020 2020  end.            
+0001ab00: 3a70 6172 616d 2064 6174 613a 2064 6174  :param data: dat
+0001ab10: 6120 746f 2073 656e 640a 2020 2020 2020  a to send.      
+0001ab20: 2020 2020 2020 3a70 6172 616d 2070 6172        :param par
+0001ab30: 616d 733a 2061 6464 6974 696f 6e61 6c20  ams: additional 
+0001ab40: 7061 7261 6d73 2074 6f20 7365 6e64 0a20  params to send. 
+0001ab50: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
+0001ab60: 726e 3a20 7265 7370 6f6e 7365 0a20 2020  rn: response.   
+0001ab70: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
+0001ab80: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
+0001ab90: 7365 0a20 2020 2020 2020 2022 2222 0a20  se.        """. 
+0001aba0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0001abb0: 3d20 7265 7175 6573 7473 2e70 6f73 7428  = requests.post(
+0001abc0: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
+0001abd0: 3d75 726c 2c0a 2020 2020 2020 2020 2020  =url,.          
+0001abe0: 2020 6a73 6f6e 3d70 6f73 745f 6a73 6f6e    json=post_json
+0001abf0: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
+0001ac00: 6c65 733d 6669 6c65 732c 0a20 2020 2020  les=files,.     
+0001ac10: 2020 2020 2020 2064 6174 613d 6461 7461         data=data
+0001ac20: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+0001ac30: 7261 6d73 3d70 6172 616d 732c 0a20 2020  rams=params,.   
+0001ac40: 2020 2020 2020 2020 2076 6572 6966 793d           verify=
+0001ac50: 7365 6c66 2e5f 7665 7269 6679 2c0a 2020  self._verify,.  
+0001ac60: 2020 2020 2020 2020 2020 7072 6f78 6965            proxie
+0001ac70: 733d 7365 6c66 2e5f 7072 6f78 6965 732c  s=self._proxies,
+0001ac80: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
+0001ac90: 6465 7273 3d73 656c 662e 5f68 6561 6465  ders=self._heade
+0001aca0: 7273 0a20 2020 2020 2020 2029 0a0a 2020  rs.        )..  
+0001acb0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0001acc0: 706f 6e73 650a 0a20 2020 2064 6566 205f  ponse..    def _
+0001acd0: 5f64 656c 6574 655f 7265 7175 6573 7428  _delete_request(
+0001ace0: 7365 6c66 2c20 7572 6c2c 2070 6f73 745f  self, url, post_
+0001acf0: 6a73 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  json=None):.    
+0001ad00: 2020 2020 2222 2241 2067 656e 6572 6963      """A generic
+0001ad10: 2044 454c 4554 4520 7265 7175 6573 7420   DELETE request 
+0001ad20: 6d65 7468 6f64 2066 6f72 2061 6c6c 2041  method for all A
+0001ad30: 3130 3030 206d 6574 686f 6473 2e0a 2020  1000 methods..  
+0001ad40: 2020 2020 2020 3a70 6172 616d 2075 726c        :param url
+0001ad50: 3a20 7265 7175 6573 7420 5552 4c0a 2020  : request URL.  
+0001ad60: 2020 2020 2020 3a74 7970 6520 7572 6c3a        :type url:
+0001ad70: 2073 7472 0a20 2020 2020 2020 203a 7265   str.        :re
+0001ad80: 7475 726e 3a20 7265 7370 6f6e 7365 0a20  turn: response. 
+0001ad90: 2020 2020 2020 203a 7274 7970 653a 2072         :rtype: r
+0001ada0: 6571 7565 7374 732e 5265 7370 6f6e 7365  equests.Response
+0001adb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001adc0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0001add0: 7265 7175 6573 7473 2e64 656c 6574 6528  requests.delete(
+0001ade0: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
+0001adf0: 3d75 726c 2c0a 2020 2020 2020 2020 2020  =url,.          
+0001ae00: 2020 6a73 6f6e 3d70 6f73 745f 6a73 6f6e    json=post_json
+0001ae10: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+0001ae20: 7269 6679 3d73 656c 662e 5f76 6572 6966  rify=self._verif
+0001ae30: 792c 0a20 2020 2020 2020 2020 2020 2070  y,.            p
+0001ae40: 726f 7869 6573 3d73 656c 662e 5f70 726f  roxies=self._pro
+0001ae50: 7869 6573 2c0a 2020 2020 2020 2020 2020  xies,.          
+0001ae60: 2020 6865 6164 6572 733d 7365 6c66 2e5f    headers=self._
+0001ae70: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+0001ae80: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0001ae90: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
+0001aea0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+0001aeb0: 2020 6465 6620 5f5f 7261 6973 655f 6f6e    def __raise_on
+0001aec0: 5f65 7272 6f72 2872 6573 706f 6e73 6529  _error(response)
+0001aed0: 3a0a 2020 2020 2020 2020 2222 2241 6363  :.        """Acc
+0001aee0: 6570 7473 2061 2072 6573 706f 6e73 6520  epts a response 
+0001aef0: 6f62 6a65 6374 2066 6f72 2076 616c 6964  object for valid
+0001af00: 6174 696f 6e20 616e 6420 7261 6973 6573  ation and raises
+0001af10: 2061 6e20 6578 6365 7074 696f 6e20 6966   an exception if
+0001af20: 2061 6e20 6572 726f 7220 7374 6174 7573   an error status
+0001af30: 2063 6f64 6520 6973 2072 6563 6569 7665   code is receive
+0001af40: 642e 0a20 2020 2020 2020 2020 2020 203a  d..            :
+0001af50: 7061 7261 6d20 7265 7370 6f6e 7365 3a20  param response: 
+0001af60: 7265 7370 6f6e 7365 206f 626a 6563 740a  response object.
+0001af70: 2020 2020 2020 2020 2020 2020 3a74 7970              :typ
+0001af80: 6520 7265 7370 6f6e 7365 3a20 7265 7175  e response: requ
+0001af90: 6573 7473 2e52 6573 706f 6e73 650a 2020  ests.Response.  
+0001afa0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001afb0: 2020 6578 6365 7074 696f 6e20 3d20 5245    exception = RE
+0001afc0: 5350 4f4e 5345 5f43 4f44 455f 4552 524f  SPONSE_CODE_ERRO
+0001afd0: 525f 4d41 502e 6765 7428 7265 7370 6f6e  R_MAP.get(respon
+0001afe0: 7365 2e73 7461 7475 735f 636f 6465 2c20  se.status_code, 
+0001aff0: 4e6f 6e65 290a 2020 2020 2020 2020 6966  None).        if
+0001b000: 206e 6f74 2065 7863 6570 7469 6f6e 3a0a   not exception:.
+0001b010: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001b020: 726e 0a20 2020 2020 2020 2072 6169 7365  rn.        raise
+0001b030: 2065 7863 6570 7469 6f6e 0a               exception.
```

### Comparing `reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/clouddeepscan.py` & `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/clouddeepscan.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/helper.py` & `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/ticloud.py` & `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.1/ReversingLabs/SDK/tiscale.py` & `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/tiscale.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.1/logo.jpg` & `reversinglabs-sdk-py3-2.1.2/logo.jpg`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.1/reversinglabs_sdk_py3.egg-info/PKG-INFO` & `reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python SDK for using ReversingLabs services - Python 3 version.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -170,15 +170,15 @@
 - `create_or_update_yara_ruleset`
   - Creates a new YARA ruleset if it doesn’t exist
   - If a ruleset with the specified name already exists, a new revision (update) of the ruleset is created
 - `delete_yara_ruleset`
   - Deletes the specified YARA ruleset and its matches from the appliance
 - `enable_or_disable_yara_ruleset`
   - Enables/disables ruleset on the appliance
-  - Administrators can manage any ruleset while regular A1000 users can only menage their own rulesets
+  - Administrators can manage any ruleset while regular A1000 users can only manage their own rulesets
 - `get_yara_ruleset_synchronization_time`
   - Gets information about the current synchronization status for TitaniumCloud-enabled rulesets
 - `update_yara_ruleset_synchronization_time`
   - Updates the TitaniumCloud synchronization time for TitaniumCloud-enabled YARA rulesets
 - `start_or_stop_yara_local_retro_scan`
   - Allows users to initiate the Local Retro scan on the A1000 appliance, and stop the Local Retro scan that is
         in progress on the appliance
@@ -204,18 +204,27 @@
   - Accepts a URL string and returns a report about the requested URL
 - `network_domain_report`
   - Accepts a domain string and returns a report about the requested domain
 - `network_ip_addr_report`
   - Accepts an IP address string and returns a report about the requested IP address
 - `network_ip_to_domain`
   - Accepts an IP address string and returns a list of IP-to-domain mappings
+- `network_ip_to_domain_aggregated`
+  - Accepts an IP address string and returns a list of IP-to-domain mappings. 
+  - This method performs the paging automatically and returns a specified maximum number of records
 - `network_urls_from_ip`
   - Accepts an IP address string and returns a list of URLs hosted on the requested IP address
+- `network_urls_from_ip_aggregated`
+  - Accepts an IP address string and returns a list of URLs hosted on the requested IP address
+  - This method performs the paging automatically and returns a specified maximum number of records
 - `network_files_from_ip`
   - Accepts an IP address string and returns a list of hashes and classifications for files found on the requested IP address
+- `network_files_from_ip_aggregated`
+  - Accepts an IP address string and returns a list of hashes and classifications for files found on the requested IP address
+  - This method performs the paging automatically and returns a specified maximum number of records
 
 ***
 
 
 ## Module: ticloud
 A Python module representing the ReversingLabs TitaniumCloud API-s.
```

### Comparing `reversinglabs-sdk-py3-2.1.1/reversinglabs_sdk_py3.egg-info/SOURCES.txt` & `reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.1/setup.py` & `reversinglabs-sdk-py3-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             "ReversingLabs.SDK"]
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name="reversinglabs-sdk-py3",
-    version="2.1.1",
+    version="2.1.2",
     description="Python SDK for using ReversingLabs services - Python 3 version.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ReversingLabs",
     author_email="support@reversinglabs.com",
     url="https://github.com/reversinglabs/reversinglabs-sdk-py3",
     packages=packages,
```

