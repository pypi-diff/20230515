# Comparing `tmp/transaction-accounts-0.1.0.tar.gz` & `tmp/transaction-accounts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction-accounts-0.1.0.tar", last modified: Thu May  4 11:57:41 2023, max compression
+gzip compressed data, was "transaction-accounts-0.1.1.tar", last modified: Mon May 15 03:13:05 2023, max compression
```

## Comparing `transaction-accounts-0.1.0.tar` & `transaction-accounts-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-04 11:57:41.830059 transaction-accounts-0.1.0/
--rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.1.0/LICENSE.txt
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-04 11:57:41.830221 transaction-accounts-0.1.0/PKG-INFO
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-04 11:57:41.820908 transaction-accounts-0.1.0/accounts/
--rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.1.0/accounts/__init__.py
--rw-r--r--   0 igormusic   (501) staff       (20)    10292 2023-05-03 05:01:15.000000 transaction-accounts-0.1.0/accounts/metadata.py
--rw-r--r--   0 igormusic   (501) staff       (20)    21470 2023-05-03 04:40:24.000000 transaction-accounts-0.1.0/accounts/runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)      201 2023-04-24 01:19:31.000000 transaction-accounts-0.1.0/accounts/utility.py
--rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-05-04 11:57:41.830803 transaction-accounts-0.1.0/setup.cfg
--rw-r--r--   0 igormusic   (501) staff       (20)     7614 2023-05-01 09:44:05.000000 transaction-accounts-0.1.0/setup.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-04 11:57:41.827565 transaction-accounts-0.1.0/tests/
--rw-r--r--   0 igormusic   (501) staff       (20)     2834 2023-04-27 01:51:20.000000 transaction-accounts-0.1.0/tests/test_calendar.py
--rw-r--r--   0 igormusic   (501) staff       (20)    18462 2023-05-03 03:32:40.000000 transaction-accounts-0.1.0/tests/test_config.py
--rw-r--r--   0 igormusic   (501) staff       (20)     1054 2023-05-01 04:20:09.000000 transaction-accounts-0.1.0/tests/test_configuration.py
--rw-r--r--   0 igormusic   (501) staff       (20)     4250 2023-05-03 04:48:05.000000 transaction-accounts-0.1.0/tests/test_loanGiven.py
--rw-r--r--   0 igormusic   (501) staff       (20)     2197 2023-04-24 02:01:02.000000 transaction-accounts-0.1.0/tests/test_rate_type.py
--rw-r--r--   0 igormusic   (501) staff       (20)     6171 2023-05-01 09:24:39.000000 transaction-accounts-0.1.0/tests/test_runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)     3942 2023-04-23 19:46:30.000000 transaction-accounts-0.1.0/tests/test_schedule.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-04 11:57:41.829691 transaction-accounts-0.1.0/transaction_accounts.egg-info/
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/PKG-INFO
--rw-r--r--   0 igormusic   (501) staff       (20)      496 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 igormusic   (501) staff       (20)       25 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/requires.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 03:13:05.672298 transaction-accounts-0.1.1/
+-rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.1.1/LICENSE.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-15 03:13:05.672443 transaction-accounts-0.1.1/PKG-INFO
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 03:13:05.663227 transaction-accounts-0.1.1/accounts/
+-rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.1.1/accounts/__init__.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    10292 2023-05-03 05:01:15.000000 transaction-accounts-0.1.1/accounts/metadata.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    21470 2023-05-03 04:40:24.000000 transaction-accounts-0.1.1/accounts/runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)      201 2023-04-24 01:19:31.000000 transaction-accounts-0.1.1/accounts/utility.py
+-rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-05-15 03:13:05.673020 transaction-accounts-0.1.1/setup.cfg
+-rw-r--r--   0 igormusic   (501) staff       (20)     7614 2023-05-15 03:12:38.000000 transaction-accounts-0.1.1/setup.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 03:13:05.669729 transaction-accounts-0.1.1/tests/
+-rw-r--r--   0 igormusic   (501) staff       (20)     2834 2023-04-27 01:51:20.000000 transaction-accounts-0.1.1/tests/test_calendar.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    18462 2023-05-03 03:32:40.000000 transaction-accounts-0.1.1/tests/test_config.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     1054 2023-05-01 04:20:09.000000 transaction-accounts-0.1.1/tests/test_configuration.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     4542 2023-05-11 23:19:20.000000 transaction-accounts-0.1.1/tests/test_loanGiven.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     2197 2023-04-24 02:01:02.000000 transaction-accounts-0.1.1/tests/test_rate_type.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     6171 2023-05-01 09:24:39.000000 transaction-accounts-0.1.1/tests/test_runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     3942 2023-04-23 19:46:30.000000 transaction-accounts-0.1.1/tests/test_schedule.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 03:13:05.671919 transaction-accounts-0.1.1/transaction_accounts.egg-info/
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-15 03:13:05.000000 transaction-accounts-0.1.1/transaction_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 igormusic   (501) staff       (20)      496 2023-05-15 03:13:05.000000 transaction-accounts-0.1.1/transaction_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-05-15 03:13:05.000000 transaction-accounts-0.1.1/transaction_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)       25 2023-05-15 03:13:05.000000 transaction-accounts-0.1.1/transaction_accounts.egg-info/requires.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-05-15 03:13:05.000000 transaction-accounts-0.1.1/transaction_accounts.egg-info/top_level.txt
```

### Comparing `transaction-accounts-0.1.0/LICENSE.txt` & `transaction-accounts-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.0/PKG-INFO` & `transaction-accounts-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.1.0
+Version: 0.1.1
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

### Comparing `transaction-accounts-0.1.0/accounts/metadata.py` & `transaction-accounts-0.1.1/accounts/metadata.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.0/accounts/runtime.py` & `transaction-accounts-0.1.1/accounts/runtime.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.0/setup.py` & `transaction-accounts-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='transaction-accounts',
-    version='0.1.0',
+    version='0.1.1',
     description='Create configuration for transactional accounts and implement account runtime',
     long_description='''
 Transaction Accounts
 ====================
 
 This library provides basic functionality for working with transaction accounts.
```

### Comparing `transaction-accounts-0.1.0/tests/test_calendar.py` & `transaction-accounts-0.1.1/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.0/tests/test_config.py` & `transaction-accounts-0.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.0/tests/test_configuration.py` & `transaction-accounts-0.1.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.0/tests/test_loanGiven.py` & `transaction-accounts-0.1.1/tests/test_loanGiven.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,27 @@
                           account_type=account_type,
                           dates={"accrual_start": start_date,
                                  "end_date": end_date}
                           )
 
         self.assertEqual(3, len(account.positions.keys()))
 
+    def test_serialize_to_json(self):
+        account_type = create_loan_given_account()
+
+        json = account_type.json()
+
+        self.assertIsNotNone(json)
+
+        account_type2 = AccountType.parse_raw(json)
+
+        json2 = account_type2.json()
+
+        self.assertEqual(json, json2)
+
     def test_mandatory_properties(self):
         self.assertRaises(ValueError, create_without_mandatory_properties)
 
     def test_forecast(self):
         account_type = create_loan_given_account()
 
         account, end_date = create_loan_account(account_type, date(2013, 3, 8))
```

### Comparing `transaction-accounts-0.1.0/tests/test_rate_type.py` & `transaction-accounts-0.1.1/tests/test_rate_type.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.0/tests/test_runtime.py` & `transaction-accounts-0.1.1/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.0/tests/test_schedule.py` & `transaction-accounts-0.1.1/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.0/transaction_accounts.egg-info/PKG-INFO` & `transaction-accounts-0.1.1/transaction_accounts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.1.0
+Version: 0.1.1
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

