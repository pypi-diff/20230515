# Comparing `tmp/recon_lw-2.0.0.dev4977997714.tar.gz` & `tmp/recon_lw-2.0.0.dev4978172035.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4977997714.tar", last modified: Mon May 15 08:07:46 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4978172035.tar", last modified: Mon May 15 08:25:49 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4977997714.tar` & `recon_lw-2.0.0.dev4978172035.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 08:07:24.000000 recon_lw-2.0.0.dev4977997714/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    26644 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 08:25:31.000000 recon_lw-2.0.0.dev4978172035/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26662 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4977997714/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4978172035/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4977997714/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4978172035/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4977997714/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4978172035/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4977997714/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4978172035/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4977997714/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4978172035/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     log = []
     if old_side is None:
         return {"error": order_id + " not found"}, []
     if traded_size > old_size:
         return {"error": "traded size > resting size"}, []
     elif traded_size == old_size:
-        reflect_price_update_in_version(old_side, old_price, order_book)
+        reflect_price_update_in_version(old_side, old_price, str_time_of_event,order_book)
         order_book[old_side][old_price].pop(order_id)
         if len(order_book[old_side][old_price]) == 0:
             order_book[old_side].pop(old_price)
             log.append(copy.deepcopy(order_book))
             max_levels = order_book["aggr_max_levels"]
             if len(order_book[old_side]) >= max_levels and order_book["aggr_seq"]["limit_delta"] == 1:
                 # back from horizon update
```

### Comparing `recon_lw-2.0.0.dev4977997714/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4978172035/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4977997714/setup.py` & `recon_lw-2.0.0.dev4978172035/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4977997714/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4978172035/test/test_recon_ob.py`

 * *Files identical despite different names*

