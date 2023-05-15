# Comparing `tmp/capitalpayments-0.1.0.tar.gz` & `tmp/capitalpayments-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capitalpayments-0.1.0.tar", last modified: Sun May 14 05:16:30 2023, max compression
+gzip compressed data, was "capitalpayments-0.1.1.tar", last modified: Mon May 15 20:12:15 2023, max compression
```

## Comparing `capitalpayments-0.1.0.tar` & `capitalpayments-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-14 05:16:30.311008 capitalpayments-0.1.0/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.1.0/LICENSE
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-14 05:16:30.310810 capitalpayments-0.1.0/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-12 00:01:07.000000 capitalpayments-0.1.0/README.md
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-14 05:16:30.309745 capitalpayments-0.1.0/capitalpayments/
--rw-r--r--   0 javierfernandez   (501) staff       (20)       36 2023-05-12 00:50:40.000000 capitalpayments-0.1.0/capitalpayments/__init__.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     4177 2023-05-12 00:58:50.000000 capitalpayments-0.1.0/capitalpayments/capitalpaymentscore.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.1.0/capitalpayments/ipn.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)      977 2023-05-14 05:15:35.000000 capitalpayments-0.1.0/capitalpayments/url_manager.py
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-14 05:16:30.310520 capitalpayments-0.1.0/capitalpayments.egg-info/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/SOURCES.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/dependency_links.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/requires.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/top_level.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-14 05:16:30.311053 capitalpayments-0.1.0/setup.cfg
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-14 05:16:28.000000 capitalpayments-0.1.0/setup.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 20:12:15.383836 capitalpayments-0.1.1/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.1.1/LICENSE
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-15 20:12:15.383707 capitalpayments-0.1.1/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-12 00:01:07.000000 capitalpayments-0.1.1/README.md
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 20:12:15.382559 capitalpayments-0.1.1/capitalpayments/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       36 2023-05-12 00:50:40.000000 capitalpayments-0.1.1/capitalpayments/__init__.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     7475 2023-05-15 20:11:52.000000 capitalpayments-0.1.1/capitalpayments/capitalpaymentscore.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.1.1/capitalpayments/ipn.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1757 2023-05-15 20:08:53.000000 capitalpayments-0.1.1/capitalpayments/url_manager.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 20:12:15.383473 capitalpayments-0.1.1/capitalpayments.egg-info/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/SOURCES.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/dependency_links.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/requires.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/top_level.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-15 20:12:15.383872 capitalpayments-0.1.1/setup.cfg
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-15 20:12:13.000000 capitalpayments-0.1.1/setup.py
```

### Comparing `capitalpayments-0.1.0/LICENSE` & `capitalpayments-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.1.0/PKG-INFO` & `capitalpayments-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.1.0
+Version: 0.1.1
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.1.0/README.md` & `capitalpayments-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.1.0/capitalpayments/capitalpaymentscore.py` & `capitalpayments-0.1.1/capitalpayments/capitalpaymentscore.py`

 * *Files 26% similar despite different names*

```diff
@@ -51,14 +51,30 @@
         response = requests.post(
             url_manager['create_invoice'], 
             headers = {'Content-Type': 'application/json'},
             auth = (self.api_key, self.api_secret),
             json = data
         )
         return response.json()
+    def createCustomer(self,data):
+        response = requests.post(
+            url_manager['create_customer'], 
+            headers = {'Content-Type': 'application/json'},
+            auth = (self.api_key, self.api_secret),
+            json = data
+        )
+        return response.json()
+    def createItem(self,data):
+        response = requests.post(
+            url_manager['create_item'], 
+            headers = {'Content-Type': 'application/json'},
+            auth = (self.api_key, self.api_secret),
+            json = data
+        )
+        return response.json()
     def cancelInvoice(self,data):
         if data.get('invoice_id'):
             response = requests.post(
                 url_manager['cancel_invoice'], 
                 headers = {'Content-Type': 'application/json'},
                 auth = (self.api_key, self.api_secret),
                 json = data
@@ -73,39 +89,115 @@
                 headers = {'Content-Type': 'application/json'},
                 auth = (self.api_key, self.api_secret),
                 json = data
             )
             return response.json()
         else: 
             raise TypeError("Not invoice id")
+    def getCustomer(self,data):
+        if data.get('customer_id'):
+            response = requests.post(
+                url_manager['get_customer'], 
+                headers = {'Content-Type': 'application/json'},
+                auth = (self.api_key, self.api_secret),
+                json = data
+            )
+            return response.json()
+        else: 
+            raise TypeError("Not customer id")
+    def getCustomers(self):
+        response = requests.post(
+            url_manager['get_customers'], 
+            headers = {'Content-Type': 'application/json'},
+            auth = (self.api_key, self.api_secret)
+        )
+        return response.json()
+    def getItems(self):
+        response = requests.post(
+            url_manager['get_items'], 
+            headers = {'Content-Type': 'application/json'},
+            auth = (self.api_key, self.api_secret)
+        )
+        return response.json()
+    def getItem(self,data):
+        if data.get('item_id'):
+            response = requests.post(
+                url_manager['get_item'], 
+                headers = {'Content-Type': 'application/json'},
+                auth = (self.api_key, self.api_secret),
+                json = data
+            )
+            return response.json()
+        else: 
+            raise TypeError("Not customer id")
     def createPayout(self,data):
         if data.get('amount'):
             if data.get('address'):
                 response = requests.post(
                     url_manager['create_payout'], 
                     headers = {'Content-Type': 'application/json'},
                     auth = (self.api_key, self.api_secret),
                     json = data
                 )
                 return response.json()
             else: 
                 raise TypeError("Not address")
         else: 
             raise TypeError("Not ammount")
+    def createPayouts(self,data):
+        response = requests.post(
+            url_manager['create_payouts'], 
+            headers = {'Content-Type': 'application/json'},
+            auth = (self.api_key, self.api_secret),
+            json = data
+        )
+        
+        return response.json()
+    def createInvoices(self,data):
+        response = requests.post(
+            url_manager['create_invoices'], 
+            headers = {'Content-Type': 'application/json'},
+            auth = (self.api_key, self.api_secret),
+            json = data
+        )
+
+        return response.json()
     def cancelPayout(self,data):
         if data.get('payout_id'):
             response = requests.post(
                 url_manager['cancel_payout'], 
                 headers = {'Content-Type': 'application/json'},
                 auth = (self.api_key, self.api_secret),
                 json = data
             )
             return response.json()
         else: 
             raise TypeError("Not payout id")
+    def deleteItem(self,data):
+        if data.get('item_id'):
+            response = requests.post(
+                url_manager['delete_item'], 
+                headers = {'Content-Type': 'application/json'},
+                auth = (self.api_key, self.api_secret),
+                json = data
+            )
+            return response.json()
+        else: 
+            raise TypeError("Not item id")
+    def deleteCustomer(self,data):
+        if data.get('customer_id'):
+            response = requests.post(
+                url_manager['delete_customer'], 
+                headers = {'Content-Type': 'application/json'},
+                auth = (self.api_key, self.api_secret),
+                json = data
+            )
+            return response.json()
+        else: 
+            raise TypeError("Not customer id")
     def getPayoutStatus(self,data):
         if data.get('payout_id'):
             response = requests.post(
                 url_manager['get_payout_status'], 
                 headers = {'Content-Type': 'application/json'},
                 auth = (self.api_key, self.api_secret),
                 json = data
```

### Comparing `capitalpayments-0.1.0/capitalpayments/ipn.py` & `capitalpayments-0.1.1/capitalpayments/ipn.py`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.1.0/capitalpayments/url_manager.py` & `capitalpayments-0.1.1/capitalpayments/url_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 url_manager = {
     'get_environment': 'https://www.capitalpayments.me/app/api/getEnvironment',
     'get_account': 'https://www.capitalpayments.me/app/api/getAccount',
     'login': 'https://www.capitalpayments.me/app/api/login',
 
     # invoices
     'create_invoice': 'https://www.capitalpayments.me/app/api/createInvoice',
+    'create_invoices' : 'https://www.capitalpayments.me/app/api/createInvoices',
     'get_invoice_status': 'https://www.capitalpayments.me/app/api/getInvoiceStatus',
     'cancel_invoice': 'https://www.capitalpayments.me/app/api/cancelInvoice',
     
     # payouts
     'create_payout': 'https://www.capitalpayments.me/app/api/createPayout',
+    'create_payouts': 'https://www.capitalpayments.me/app/api/createPayouts',
     'get_payout_status': 'https://www.capitalpayments.me/app/api/getPayoutStatus',
     'cancel_payout': 'https://www.capitalpayments.me/app/api/cancelPayout',
 
     # wallet
     'get_balance': 'https://www.capitalpayments.me/app/api/getBalance',
     'get_main_wallet': 'https://www.capitalpayments.me/app/api/getMainWallet',
-    'get_wallets': 'https://www.capitalpayments.me/app/api/getWallets'
+    'get_wallets': 'https://www.capitalpayments.me/app/api/getWallets',
+ 
+    # customer 
+    'get_customers' : 'https://www.capitalpayments.me/app/api/getCustomers',
+    'get_customer' : 'https://www.capitalpayments.me/app/api/getCustomer',
+    'delete_customer' : 'https://www.capitalpayments.me/app/api/deleteCustomer',
+    'create_customer' : 'https://www.capitalpayments.me/app/api/addCustomer',
+
+    # item
+    'get_items' : 'https://www.capitalpayments.me/app/api/getItems',
+    'get_item' : 'https://www.capitalpayments.me/app/api/getItem',
+    'delete_item' : 'https://www.capitalpayments.me/app/api/deleteItem',
+    'create_item' : 'https://www.capitalpayments.me/app/api/addItem',
 }
```

### Comparing `capitalpayments-0.1.0/capitalpayments.egg-info/PKG-INFO` & `capitalpayments-0.1.1/capitalpayments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.1.0
+Version: 0.1.1
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.1.0/setup.py` & `capitalpayments-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'For Api Capital Payments'
 LONG_DESCRIPTION = 'This SDK connects to Capital Payments Payment Processor Api.'
 
 # Setting up
 setup(
     name="capitalpayments",
     version=VERSION,
```

