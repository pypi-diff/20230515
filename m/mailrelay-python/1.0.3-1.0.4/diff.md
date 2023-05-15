# Comparing `tmp/mailrelay_python-1.0.3.tar.gz` & `tmp/mailrelay_python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailrelay_python-1.0.3.tar", max compression
+gzip compressed data, was "mailrelay_python-1.0.4.tar", max compression
```

## Comparing `mailrelay_python-1.0.3.tar` & `mailrelay_python-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-03-28 14:48:21.137523 mailrelay_python-1.0.3/LICENSE
--rw-r--r--   0        0        0     5204 2023-03-28 14:48:21.137756 mailrelay_python-1.0.3/README.md
--rw-r--r--   0        0        0    12052 2023-03-28 14:48:21.137929 mailrelay_python-1.0.3/mailrelay/client.py
--rw-r--r--   0        0        0     1072 2023-03-28 14:48:21.138036 mailrelay_python-1.0.3/mailrelay/exceptions.py
--rw-r--r--   0        0        0      400 2023-03-28 14:50:13.787117 mailrelay_python-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 mailrelay_python-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-28 14:48:21.137523 mailrelay_python-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5204 2023-03-28 14:48:21.137756 mailrelay_python-1.0.4/README.md
+-rw-r--r--   0        0        0    12303 2023-05-15 16:07:44.396850 mailrelay_python-1.0.4/mailrelay/client.py
+-rw-r--r--   0        0        0     1072 2023-03-28 14:48:21.138036 mailrelay_python-1.0.4/mailrelay/exceptions.py
+-rw-r--r--   0        0        0      400 2023-05-15 16:07:44.397402 mailrelay_python-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 mailrelay_python-1.0.4/PKG-INFO
```

### Comparing `mailrelay_python-1.0.3/LICENSE` & `mailrelay_python-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mailrelay_python-1.0.3/README.md` & `mailrelay_python-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mailrelay_python-1.0.3/mailrelay/client.py` & `mailrelay_python-1.0.4/mailrelay/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 from urllib import response
 import requests
 
 
 class Client(object):
     def __init__(self, api_key, domain):
         self.api_key = api_key
-        self.base_url = f"https://{domain}/api/v1/"
+        if domain.startswith("http://") or domain.startswith("https://"):
+            if domain.endswith("/"):
+                self.base_url = f"{domain}api/v1/"
+            else:
+                self.base_url = f"{domain}/api/v1/"
+
+        else:
+            self.base_url = f"https://{domain}/api/v1/"
 
     def _compose_endpoint(self, endpoint, id=None):
         if id:
             url = self.base_url + endpoint + "/{id}".format(id=id)
         else:
             url = self.base_url + endpoint
         return url
```

### Comparing `mailrelay_python-1.0.3/mailrelay/exceptions.py` & `mailrelay_python-1.0.4/mailrelay/exceptions.py`

 * *Files identical despite different names*

### Comparing `mailrelay_python-1.0.3/PKG-INFO` & `mailrelay_python-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailrelay-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: API wrapper for MailRelay written in Python
 License: MIT
 Author: Miguel Ferrer
 Author-email: ingferrermiguel@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

