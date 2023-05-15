# Comparing `tmp/luno-python-0.0.8.tar.gz` & `tmp/luno-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luno-python-0.0.8.tar", last modified: Sun Dec  5 19:08:53 2021, max compression
+gzip compressed data, was "luno-python-0.0.9.tar", last modified: Tue May  3 11:46:46 2022, max compression
```

## Comparing `luno-python-0.0.8.tar` & `luno-python-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 neil       (503) staff       (20)        0 2021-12-05 19:08:53.482943 luno-python-0.0.8/
--rw-r--r--   0 neil       (503) staff       (20)     1062 2021-12-05 19:07:25.000000 luno-python-0.0.8/LICENSE.txt
--rw-r--r--   0 neil       (503) staff       (20)      353 2021-12-05 19:08:53.483006 luno-python-0.0.8/PKG-INFO
--rw-r--r--   0 neil       (503) staff       (20)      775 2021-12-05 19:07:25.000000 luno-python-0.0.8/README.md
-drwxr-xr-x   0 neil       (503) staff       (20)        0 2021-12-05 19:08:53.482040 luno-python-0.0.8/luno_python/
--rw-r--r--   0 neil       (503) staff       (20)       18 2021-12-05 19:07:25.000000 luno-python-0.0.8/luno_python/__init__.py
--rw-r--r--   0 neil       (503) staff       (20)     3001 2021-12-05 19:07:25.000000 luno-python-0.0.8/luno_python/base_client.py
--rw-r--r--   0 neil       (503) staff       (20)    37600 2021-12-05 19:07:25.000000 luno-python-0.0.8/luno_python/client.py
--rw-r--r--   0 neil       (503) staff       (20)      122 2021-12-05 19:07:25.000000 luno-python-0.0.8/luno_python/error.py
-drwxr-xr-x   0 neil       (503) staff       (20)        0 2021-12-05 19:08:53.482822 luno-python-0.0.8/luno_python.egg-info/
--rw-r--r--   0 neil       (503) staff       (20)      353 2021-12-05 19:08:53.000000 luno-python-0.0.8/luno_python.egg-info/PKG-INFO
--rw-r--r--   0 neil       (503) staff       (20)      308 2021-12-05 19:08:53.000000 luno-python-0.0.8/luno_python.egg-info/SOURCES.txt
--rw-r--r--   0 neil       (503) staff       (20)        1 2021-12-05 19:08:53.000000 luno-python-0.0.8/luno_python.egg-info/dependency_links.txt
--rw-r--r--   0 neil       (503) staff       (20)       29 2021-12-05 19:08:53.000000 luno-python-0.0.8/luno_python.egg-info/requires.txt
--rw-r--r--   0 neil       (503) staff       (20)       12 2021-12-05 19:08:53.000000 luno-python-0.0.8/luno_python.egg-info/top_level.txt
--rw-r--r--   0 neil       (503) staff       (20)      113 2021-12-05 19:08:53.483264 luno-python-0.0.8/setup.cfg
--rw-r--r--   0 neil       (503) staff       (20)      655 2021-12-05 19:07:25.000000 luno-python-0.0.8/setup.py
+drwxr-xr-x   0 neil       (503) staff       (20)        0 2022-05-03 11:46:46.452149 luno-python-0.0.9/
+-rw-------   0 neil       (503) staff       (20)     1062 2019-12-11 08:09:48.000000 luno-python-0.0.9/LICENSE.txt
+-rw-r--r--   0 neil       (503) staff       (20)      353 2022-05-03 11:46:46.452203 luno-python-0.0.9/PKG-INFO
+-rw-------   0 neil       (503) staff       (20)      775 2019-12-11 09:49:09.000000 luno-python-0.0.9/README.md
+drwxr-xr-x   0 neil       (503) staff       (20)        0 2022-05-03 11:46:46.451135 luno-python-0.0.9/luno_python/
+-rw-r--r--   0 neil       (503) staff       (20)       18 2022-05-03 11:46:44.000000 luno-python-0.0.9/luno_python/__init__.py
+-rw-r--r--   0 neil       (503) staff       (20)     3001 2020-06-18 13:48:14.000000 luno-python-0.0.9/luno_python/base_client.py
+-rw-r--r--   0 neil       (503) staff       (20)    38767 2022-05-03 10:09:04.000000 luno-python-0.0.9/luno_python/client.py
+-rw-------   0 neil       (503) staff       (20)      122 2019-12-11 08:09:48.000000 luno-python-0.0.9/luno_python/error.py
+drwxr-xr-x   0 neil       (503) staff       (20)        0 2022-05-03 11:46:46.452022 luno-python-0.0.9/luno_python.egg-info/
+-rw-------   0 neil       (503) staff       (20)      353 2022-05-03 11:46:46.000000 luno-python-0.0.9/luno_python.egg-info/PKG-INFO
+-rw-------   0 neil       (503) staff       (20)      308 2022-05-03 11:46:46.000000 luno-python-0.0.9/luno_python.egg-info/SOURCES.txt
+-rw-------   0 neil       (503) staff       (20)        1 2022-05-03 11:46:46.000000 luno-python-0.0.9/luno_python.egg-info/dependency_links.txt
+-rw-------   0 neil       (503) staff       (20)       29 2022-05-03 11:46:46.000000 luno-python-0.0.9/luno_python.egg-info/requires.txt
+-rw-------   0 neil       (503) staff       (20)       12 2022-05-03 11:46:46.000000 luno-python-0.0.9/luno_python.egg-info/top_level.txt
+-rw-------   0 neil       (503) staff       (20)      113 2022-05-03 11:46:46.452536 luno-python-0.0.9/setup.cfg
+-rw-------   0 neil       (503) staff       (20)      655 2019-12-11 08:09:48.000000 luno-python-0.0.9/setup.py
```

### Comparing `luno-python-0.0.8/LICENSE.txt` & `luno-python-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `luno-python-0.0.8/README.md` & `luno-python-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `luno-python-0.0.8/luno_python/base_client.py` & `luno-python-0.0.9/luno_python/base_client.py`

 * *Files identical despite different names*

### Comparing `luno-python-0.0.8/luno_python/client.py` & `luno-python-0.0.9/luno_python/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -818,14 +818,44 @@
             'destination_tag': destination_tag,
             'external_id': external_id,
             'has_destination_tag': has_destination_tag,
             'message': message,
         }
         return self.do('POST', '/api/1/send', req=req, auth=True)
 
+    def send_fee(self, address, amount, currency):
+        """Makes a call to GET /api/1/send_fee.
+
+        Calculate fees involved with a crypto send request.
+
+        Send address can be to a cryptocurrency receive address, or the email address of another Luno platform user.
+
+        Permissions required: <code>MP_None</code>
+
+        :param address: Destination address or email address.
+
+                        <b>Note</b>:
+                        <ul>
+                        <li>Ethereum addresses must be
+                        <a href="https://github.com/ethereum/EIPs/blob/master/EIPS/eip-55.md" target="_blank" rel="nofollow">checksummed</a>.</li>
+                        <li>Ethereum sends to email addresses are not supported.</li>
+                        </ul>
+        :type address: str
+        :param amount: Amount to send as a decimal string.
+        :type amount: float
+        :param currency: Currency to send.
+        :type currency: str
+        """
+        req = {
+            'address': address,
+            'amount': amount,
+            'currency': currency,
+        }
+        return self.do('GET', '/api/1/send_fee', req=req, auth=True)
+
     def stop_order(self, order_id):
         """Makes a call to POST /api/1/stoporder.
 
         Request to cancel an Order.
 
         <b>Note!</b>: Once an Order has been completed, it can not be reversed.
         The return value from this request will indicate if the Stop request was successful or not.
```

### Comparing `luno-python-0.0.8/setup.py` & `luno-python-0.0.9/setup.py`

 * *Files identical despite different names*

