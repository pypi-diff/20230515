# Comparing `tmp/transaction-accounts-0.1.2.tar.gz` & `tmp/transaction-accounts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction-accounts-0.1.2.tar", last modified: Mon May 15 03:17:11 2023, max compression
+gzip compressed data, was "transaction-accounts-0.1.3.tar", last modified: Mon May 15 04:09:37 2023, max compression
```

## Comparing `transaction-accounts-0.1.2.tar` & `transaction-accounts-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 03:17:11.759168 transaction-accounts-0.1.2/
--rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.1.2/LICENSE.txt
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-15 03:17:11.759357 transaction-accounts-0.1.2/PKG-INFO
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 03:17:11.750410 transaction-accounts-0.1.2/accounts/
--rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.1.2/accounts/__init__.py
--rw-r--r--   0 igormusic   (501) staff       (20)    10292 2023-05-03 05:01:15.000000 transaction-accounts-0.1.2/accounts/metadata.py
--rw-r--r--   0 igormusic   (501) staff       (20)    21470 2023-05-03 04:40:24.000000 transaction-accounts-0.1.2/accounts/runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)      201 2023-04-24 01:19:31.000000 transaction-accounts-0.1.2/accounts/utility.py
--rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-05-15 03:17:11.759909 transaction-accounts-0.1.2/setup.cfg
--rw-r--r--   0 igormusic   (501) staff       (20)     7631 2023-05-15 03:16:59.000000 transaction-accounts-0.1.2/setup.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 03:17:11.756587 transaction-accounts-0.1.2/tests/
--rw-r--r--   0 igormusic   (501) staff       (20)     2834 2023-04-27 01:51:20.000000 transaction-accounts-0.1.2/tests/test_calendar.py
--rw-r--r--   0 igormusic   (501) staff       (20)    18462 2023-05-03 03:32:40.000000 transaction-accounts-0.1.2/tests/test_config.py
--rw-r--r--   0 igormusic   (501) staff       (20)     1054 2023-05-01 04:20:09.000000 transaction-accounts-0.1.2/tests/test_configuration.py
--rw-r--r--   0 igormusic   (501) staff       (20)     4542 2023-05-11 23:19:20.000000 transaction-accounts-0.1.2/tests/test_loanGiven.py
--rw-r--r--   0 igormusic   (501) staff       (20)     2197 2023-04-24 02:01:02.000000 transaction-accounts-0.1.2/tests/test_rate_type.py
--rw-r--r--   0 igormusic   (501) staff       (20)     6171 2023-05-01 09:24:39.000000 transaction-accounts-0.1.2/tests/test_runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)     3942 2023-04-23 19:46:30.000000 transaction-accounts-0.1.2/tests/test_schedule.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 03:17:11.758787 transaction-accounts-0.1.2/transaction_accounts.egg-info/
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-15 03:17:11.000000 transaction-accounts-0.1.2/transaction_accounts.egg-info/PKG-INFO
--rw-r--r--   0 igormusic   (501) staff       (20)      496 2023-05-15 03:17:11.000000 transaction-accounts-0.1.2/transaction_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-05-15 03:17:11.000000 transaction-accounts-0.1.2/transaction_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 igormusic   (501) staff       (20)       31 2023-05-15 03:17:11.000000 transaction-accounts-0.1.2/transaction_accounts.egg-info/requires.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-05-15 03:17:11.000000 transaction-accounts-0.1.2/transaction_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 04:09:37.012588 transaction-accounts-0.1.3/
+-rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.1.3/LICENSE.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-15 04:09:37.012729 transaction-accounts-0.1.3/PKG-INFO
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 04:09:37.003661 transaction-accounts-0.1.3/accounts/
+-rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.1.3/accounts/__init__.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    10292 2023-05-03 05:01:15.000000 transaction-accounts-0.1.3/accounts/metadata.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    21745 2023-05-15 04:05:33.000000 transaction-accounts-0.1.3/accounts/runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)      201 2023-04-24 01:19:31.000000 transaction-accounts-0.1.3/accounts/utility.py
+-rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-05-15 04:09:37.013797 transaction-accounts-0.1.3/setup.cfg
+-rw-r--r--   0 igormusic   (501) staff       (20)     7631 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/setup.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 04:09:37.010083 transaction-accounts-0.1.3/tests/
+-rw-r--r--   0 igormusic   (501) staff       (20)     2834 2023-04-27 01:51:20.000000 transaction-accounts-0.1.3/tests/test_calendar.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    18462 2023-05-03 03:32:40.000000 transaction-accounts-0.1.3/tests/test_config.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     1054 2023-05-01 04:20:09.000000 transaction-accounts-0.1.3/tests/test_configuration.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     4595 2023-05-15 03:57:18.000000 transaction-accounts-0.1.3/tests/test_loanGiven.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     2197 2023-04-24 02:01:02.000000 transaction-accounts-0.1.3/tests/test_rate_type.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     6171 2023-05-01 09:24:39.000000 transaction-accounts-0.1.3/tests/test_runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     3942 2023-04-23 19:46:30.000000 transaction-accounts-0.1.3/tests/test_schedule.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 04:09:37.012290 transaction-accounts-0.1.3/transaction_accounts.egg-info/
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 igormusic   (501) staff       (20)      496 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)       31 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/requires.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/top_level.txt
```

### Comparing `transaction-accounts-0.1.2/LICENSE.txt` & `transaction-accounts-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.2/PKG-INFO` & `transaction-accounts-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

### Comparing `transaction-accounts-0.1.2/accounts/metadata.py` & `transaction-accounts-0.1.3/accounts/metadata.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.2/accounts/runtime.py` & `transaction-accounts-0.1.3/accounts/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import timedelta
 from itertools import groupby
 from typing import Mapping, Any
 from dateutil.relativedelta import *
+from pydantic import Field
+
 from accounts.metadata import *
 import scipy.optimize
 
 
 class Position(BaseModel):
     amount: Decimal = Decimal(0)
 
@@ -45,15 +47,19 @@
     frequency: ScheduleFrequency
     interval: int = 0,
     adjustment: BusinessDayAdjustment = BusinessDayAdjustment.NO_ADJUSTMENT
     end_date: Optional[date]
     number_of_repeats: int = 0
     include_dates: list[date] = []
     exclude_dates: list[date] = []
-    cached_dates: dict[date, date] = {}
+    cached_dates: dict[date, date] = Field(default_factory=dict,  exclude=True)
+
+    class Config:
+        # exclude the "cached_dates" field from JSON serialization
+        exclude = {"cached_dates"}
 
     def __is_simple_daily_schedule(self):
         return (self.frequency == ScheduleFrequency.DAILY and
                 self.interval == 1 and
                 self.adjustment == BusinessDayAdjustment.NO_ADJUSTMENT)
 
     def __last_date(self):
@@ -150,15 +156,15 @@
     account_type_name: str
     positions: dict[str, Position] = {}
     value_dated_properties: dict[str, PropertyValue] = {}
     properties: dict[str, Any] = {}
     dates: dict[str, date] = {}
     schedules: dict[str, Schedule] = {}
     transactions: list[Transaction] = []
-    instalments: dict[date, Instalment] = {}
+    instalments: dict[str, Instalment] = {}
 
     def __init__(self, **kw):
         super().__init__(**kw)
         if "account_type" in kw:
             account_type: AccountType = kw["account_type"]
             self.__validate_properties(account_type)
             self.__initialize_positions(account_type)
@@ -212,15 +218,15 @@
     def __initialize_instalment(self, account_type: AccountType):
         instalment_type = account_type.instalment_type
 
         # if no instalments create default one
         if instalment_type and len(self.instalments.items()) == 0:
             for date_value in self.schedules[instalment_type.schedule_name].get_all_dates(
                     self.start_date + relativedelta(years=+50)):
-                self.instalments[date_value] = Instalment(amount=Decimal(0), is_fixed=False)
+                self.instalments[date_value.strftime("%Y-%m-%d")] = Instalment(amount=Decimal(0), is_fixed=False)
 
     def apply_calculated_installment(self, amount: Decimal):
         # set all instalments to calculated amount if fixed is false
         for instalment in self.instalments.values():
             if not instalment.is_fixed:
                 instalment.amount = amount
 
@@ -371,18 +377,20 @@
                 self.__create_transaction(transaction_type, value_date, external_transaction.amount, False)
 
     def start_of_day(self, value_date):
         for scheduled_transaction in self.account_type.scheduled_transactions:
             if scheduled_transaction.timing == ScheduledTransactionTiming.START_OF_DAY:
                 self.__create_transaction_if_due(value_date, scheduled_transaction)
 
+        value_date_str = value_date.strftime('%Y-%m-%d')
+
         if self.account_type.instalment_type:
             if self.account_type.instalment_type.timing == ScheduledTransactionTiming.START_OF_DAY \
-                    and value_date in self.account.instalments:
-                instalment = self.account.instalments[value_date]
+                    and value_date_str in self.account.instalments:
+                instalment = self.account.instalments[value_date_str]
                 transaction_type = self.account_type.get_transaction_type(
                     self.account_type.instalment_type.transaction_type)
                 self.__create_transaction(transaction_type, value_date, instalment.amount, True)
 
     def __create_transaction_if_due(self, value_date: date, scheduled_transaction: ScheduledTransaction):
         schedule = self.account.schedules[scheduled_transaction.schedule_name]
```

### Comparing `transaction-accounts-0.1.2/setup.py` & `transaction-accounts-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='transaction-accounts',
-    version='0.1.2',
+    version='0.1.3',
     description='Create configuration for transactional accounts and implement account runtime',
     long_description='''
 Transaction Accounts
 ====================
 
 This library provides basic functionality for working with transaction accounts.
```

### Comparing `transaction-accounts-0.1.2/tests/test_calendar.py` & `transaction-accounts-0.1.3/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.2/tests/test_config.py` & `transaction-accounts-0.1.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.2/tests/test_configuration.py` & `transaction-accounts-0.1.3/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.2/tests/test_loanGiven.py` & `transaction-accounts-0.1.3/tests/test_loanGiven.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,17 @@
                       account_type_name=account_type.name,
                       account_type=account_type,
                       dates=dates,
                       properties=properties,
                       schedules={"interest": interest_schedule,
                                  "redemption": redemption_schedule})
 
+    dict = account.dict()
+    json = account.json()
+
     return account, end_date
 
 
 class TestConfiguration(unittest.TestCase):
 
     def test_serialize(self):
         account_type = None
```

### Comparing `transaction-accounts-0.1.2/tests/test_rate_type.py` & `transaction-accounts-0.1.3/tests/test_rate_type.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.2/tests/test_runtime.py` & `transaction-accounts-0.1.3/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.2/tests/test_schedule.py` & `transaction-accounts-0.1.3/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.2/transaction_accounts.egg-info/PKG-INFO` & `transaction-accounts-0.1.3/transaction_accounts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

