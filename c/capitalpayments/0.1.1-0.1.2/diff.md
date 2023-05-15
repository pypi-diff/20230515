# Comparing `tmp/capitalpayments-0.1.1.tar.gz` & `tmp/capitalpayments-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capitalpayments-0.1.1.tar", last modified: Mon May 15 20:12:15 2023, max compression
+gzip compressed data, was "capitalpayments-0.1.2.tar", last modified: Mon May 15 21:47:15 2023, max compression
```

## Comparing `capitalpayments-0.1.1.tar` & `capitalpayments-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 20:12:15.383836 capitalpayments-0.1.1/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.1.1/LICENSE
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-15 20:12:15.383707 capitalpayments-0.1.1/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-12 00:01:07.000000 capitalpayments-0.1.1/README.md
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 20:12:15.382559 capitalpayments-0.1.1/capitalpayments/
--rw-r--r--   0 javierfernandez   (501) staff       (20)       36 2023-05-12 00:50:40.000000 capitalpayments-0.1.1/capitalpayments/__init__.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     7475 2023-05-15 20:11:52.000000 capitalpayments-0.1.1/capitalpayments/capitalpaymentscore.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.1.1/capitalpayments/ipn.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1757 2023-05-15 20:08:53.000000 capitalpayments-0.1.1/capitalpayments/url_manager.py
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 20:12:15.383473 capitalpayments-0.1.1/capitalpayments.egg-info/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/SOURCES.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/dependency_links.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/requires.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-15 20:12:15.000000 capitalpayments-0.1.1/capitalpayments.egg-info/top_level.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-15 20:12:15.383872 capitalpayments-0.1.1/setup.cfg
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-15 20:12:13.000000 capitalpayments-0.1.1/setup.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 21:47:15.347551 capitalpayments-0.1.2/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.1.2/LICENSE
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-15 21:47:15.347410 capitalpayments-0.1.2/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-12 00:01:07.000000 capitalpayments-0.1.2/README.md
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 21:47:15.346411 capitalpayments-0.1.2/capitalpayments/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       36 2023-05-12 00:50:40.000000 capitalpayments-0.1.2/capitalpayments/__init__.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     7598 2023-05-15 21:41:57.000000 capitalpayments-0.1.2/capitalpayments/capitalpaymentscore.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.1.2/capitalpayments/ipn.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1757 2023-05-15 21:47:02.000000 capitalpayments-0.1.2/capitalpayments/url_manager.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 21:47:15.347196 capitalpayments-0.1.2/capitalpayments.egg-info/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-15 21:47:15.000000 capitalpayments-0.1.2/capitalpayments.egg-info/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-05-15 21:47:15.000000 capitalpayments-0.1.2/capitalpayments.egg-info/SOURCES.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-15 21:47:15.000000 capitalpayments-0.1.2/capitalpayments.egg-info/dependency_links.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-15 21:47:15.000000 capitalpayments-0.1.2/capitalpayments.egg-info/requires.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-15 21:47:15.000000 capitalpayments-0.1.2/capitalpayments.egg-info/top_level.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-15 21:47:15.347775 capitalpayments-0.1.2/setup.cfg
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-15 21:46:57.000000 capitalpayments-0.1.2/setup.py
```

### Comparing `capitalpayments-0.1.1/LICENSE` & `capitalpayments-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.1.1/PKG-INFO` & `capitalpayments-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.1.1
+Version: 0.1.2
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.1.1/README.md` & `capitalpayments-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.1.1/capitalpayments/capitalpaymentscore.py` & `capitalpayments-0.1.2/capitalpayments/capitalpaymentscore.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     def createCustomer(self,data):
         response = requests.post(
             url_manager['create_customer'], 
             headers = {'Content-Type': 'application/json'},
             auth = (self.api_key, self.api_secret),
             json = data
         )
+
         return response.json()
     def createItem(self,data):
         response = requests.post(
             url_manager['create_item'], 
             headers = {'Content-Type': 'application/json'},
             auth = (self.api_key, self.api_secret),
             json = data
@@ -140,28 +141,34 @@
                 )
                 return response.json()
             else: 
                 raise TypeError("Not address")
         else: 
             raise TypeError("Not ammount")
     def createPayouts(self,data):
+        payouts = {}
+        payouts['payouts'] = data
+
         response = requests.post(
             url_manager['create_payouts'], 
             headers = {'Content-Type': 'application/json'},
             auth = (self.api_key, self.api_secret),
-            json = data
+            json = payouts
         )
         
         return response.json()
     def createInvoices(self,data):
+        invoices = {}
+        invoices['invoices'] = data
+
         response = requests.post(
             url_manager['create_invoices'], 
             headers = {'Content-Type': 'application/json'},
             auth = (self.api_key, self.api_secret),
-            json = data
+            json = invoices
         )
 
         return response.json()
     def cancelPayout(self,data):
         if data.get('payout_id'):
             response = requests.post(
                 url_manager['cancel_payout'],
```

### Comparing `capitalpayments-0.1.1/capitalpayments/ipn.py` & `capitalpayments-0.1.2/capitalpayments/ipn.py`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.1.1/capitalpayments/url_manager.py` & `capitalpayments-0.1.2/capitalpayments/url_manager.py`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.1.1/capitalpayments.egg-info/PKG-INFO` & `capitalpayments-0.1.2/capitalpayments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.1.1
+Version: 0.1.2
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.1.1/setup.py` & `capitalpayments-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'For Api Capital Payments'
 LONG_DESCRIPTION = 'This SDK connects to Capital Payments Payment Processor Api.'
 
 # Setting up
 setup(
     name="capitalpayments",
     version=VERSION,
```

