# Comparing `tmp/zebedee-0.0.4.tar.gz` & `tmp/zebedee-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zebedee-0.0.4.tar", last modified: Fri May 12 18:57:05 2023, max compression
+gzip compressed data, was "zebedee-0.0.5.tar", last modified: Mon May 15 04:03:37 2023, max compression
```

## Comparing `zebedee-0.0.4.tar` & `zebedee-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-12 18:57:05.063788 zebedee-0.0.4/
--rw-r--r--   0 santos     (501) staff       (20)     1065 2023-04-03 00:04:47.000000 zebedee-0.0.4/LICENSE
--rw-r--r--   0 santos     (501) staff       (20)     7008 2023-05-12 18:57:05.063618 zebedee-0.0.4/PKG-INFO
--rw-r--r--   0 santos     (501) staff       (20)     6420 2023-05-11 06:00:25.000000 zebedee-0.0.4/README.md
--rw-r--r--   0 santos     (501) staff       (20)       38 2023-05-12 18:57:05.063846 zebedee-0.0.4/setup.cfg
--rw-r--r--   0 santos     (501) staff       (20)     1167 2023-05-12 18:57:01.000000 zebedee-0.0.4/setup.py
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-12 18:57:05.062493 zebedee-0.0.4/zebedee/
--rw-r--r--   0 santos     (501) staff       (20)       19 2023-05-11 05:51:33.000000 zebedee-0.0.4/zebedee/__init__.py
--rw-r--r--   0 santos     (501) staff       (20)    10974 2023-05-12 18:52:57.000000 zebedee-0.0.4/zebedee/main.py
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-12 18:57:05.063318 zebedee-0.0.4/zebedee.egg-info/
--rw-r--r--   0 santos     (501) staff       (20)     7008 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/PKG-INFO
--rw-r--r--   0 santos     (501) staff       (20)      216 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/SOURCES.txt
--rw-r--r--   0 santos     (501) staff       (20)        1 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/dependency_links.txt
--rw-r--r--   0 santos     (501) staff       (20)       49 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/requires.txt
--rw-r--r--   0 santos     (501) staff       (20)        8 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/top_level.txt
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-15 04:03:37.151878 zebedee-0.0.5/
+-rw-r--r--   0 santos     (501) staff       (20)     1065 2023-04-03 00:04:47.000000 zebedee-0.0.5/LICENSE
+-rw-r--r--   0 santos     (501) staff       (20)     7008 2023-05-15 04:03:37.151721 zebedee-0.0.5/PKG-INFO
+-rw-r--r--   0 santos     (501) staff       (20)     6420 2023-05-11 06:00:25.000000 zebedee-0.0.5/README.md
+-rw-r--r--   0 santos     (501) staff       (20)       38 2023-05-15 04:03:37.151923 zebedee-0.0.5/setup.cfg
+-rw-r--r--   0 santos     (501) staff       (20)     1167 2023-05-15 04:03:08.000000 zebedee-0.0.5/setup.py
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-15 04:03:37.150704 zebedee-0.0.5/zebedee/
+-rw-r--r--   0 santos     (501) staff       (20)       19 2023-05-11 05:51:33.000000 zebedee-0.0.5/zebedee/__init__.py
+-rw-r--r--   0 santos     (501) staff       (20)    11240 2023-05-15 04:00:08.000000 zebedee-0.0.5/zebedee/main.py
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-15 04:03:37.151527 zebedee-0.0.5/zebedee.egg-info/
+-rw-r--r--   0 santos     (501) staff       (20)     7008 2023-05-15 04:03:37.000000 zebedee-0.0.5/zebedee.egg-info/PKG-INFO
+-rw-r--r--   0 santos     (501) staff       (20)      216 2023-05-15 04:03:37.000000 zebedee-0.0.5/zebedee.egg-info/SOURCES.txt
+-rw-r--r--   0 santos     (501) staff       (20)        1 2023-05-15 04:03:37.000000 zebedee-0.0.5/zebedee.egg-info/dependency_links.txt
+-rw-r--r--   0 santos     (501) staff       (20)       49 2023-05-15 04:03:37.000000 zebedee-0.0.5/zebedee.egg-info/requires.txt
+-rw-r--r--   0 santos     (501) staff       (20)        8 2023-05-15 04:03:37.000000 zebedee-0.0.5/zebedee.egg-info/top_level.txt
```

### Comparing `zebedee-0.0.4/LICENSE` & `zebedee-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zebedee-0.0.4/PKG-INFO` & `zebedee-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebedee
-Version: 0.0.4
+Version: 0.0.5
 Summary: Move Money at the Speed of the Internet 
 Author: zantoshi (Santos Hernandez)
 Author-email: <santosdhernandez@gmail.com>
 Keywords: python,payments,bitcoin,lightning network,django,lightning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zebedee-0.0.4/README.md` & `zebedee-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zebedee-0.0.4/setup.py` & `zebedee-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Move Money at the Speed of the Internet '
 LONG_DESCRIPTION = 'A package that allows for faster integration of the ZEBEDEE API.'
 
 # Setting up
 setup(
     name="zebedee",
     version=VERSION,
```

### Comparing `zebedee-0.0.4/zebedee/main.py` & `zebedee-0.0.5/zebedee/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,8 +281,13 @@
         payload = json.dumps({
             "amount": str(amount_msats),
             "receiverWalletId": recevier_wallet_id
         })
 
         return requests.post(URL, headers=heads, data=payload).json()["data"]
     
+    def get_static_charge_metadata(self, id):
+        url = f"https://api.zebedee.io/v0/request-static-charges/{id}"
+        heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
+        res = requests.get(url, headers=heads).json()
+        return res
```

### Comparing `zebedee-0.0.4/zebedee.egg-info/PKG-INFO` & `zebedee-0.0.5/zebedee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebedee
-Version: 0.0.4
+Version: 0.0.5
 Summary: Move Money at the Speed of the Internet 
 Author: zantoshi (Santos Hernandez)
 Author-email: <santosdhernandez@gmail.com>
 Keywords: python,payments,bitcoin,lightning network,django,lightning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

