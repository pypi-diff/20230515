# Comparing `tmp/recon_lw-2.0.0.dev4978172035.tar.gz` & `tmp/recon_lw-2.0.0.dev4978443614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4978172035.tar", last modified: Mon May 15 08:25:49 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4978443614.tar", last modified: Mon May 15 08:57:01 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4978172035.tar` & `recon_lw-2.0.0.dev4978443614.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 08:25:31.000000 recon_lw-2.0.0.dev4978172035/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    26662 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:25:49.000000 recon_lw-2.0.0.dev4978172035/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-15 08:25:10.000000 recon_lw-2.0.0.dev4978172035/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 08:56:39.000000 recon_lw-2.0.0.dev4978443614/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26662 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:57:01.000000 recon_lw-2.0.0.dev4978443614/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-15 08:56:15.000000 recon_lw-2.0.0.dev4978443614/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4978172035/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4978443614/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4978172035/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4978443614/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4978172035/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4978443614/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4978172035/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4978443614/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4978172035/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4978443614/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4978172035/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4978443614/recon_lw/recon_ob_cross_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         save_events([error_event])
     elif match[1] is not None:
         error_event = create_event("StreamMismatchNoFull",
                                    "StreamMismatchNoFull",
                                    False,
                                    {"aggr_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
-                                    "time_of_event": match[0]["body"]["time_of_event"],
+                                    "time_of_event": match[1]["body"]["time_of_event"],
                                    "limit_v2": match[1]["body"]["aggr_seq"]["limit_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
 
 
 def ob_compare_interpret_match_top(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
@@ -183,15 +183,15 @@
         save_events([error_event])
     elif match[1] is not None:
         error_event = create_event("StreamMismatchNoFull",
                                    "StreamMismatchNoFull",
                                    False,
                                    {"top_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
-                                    "time_of_event": match[0]["body"]["time_of_event"],
+                                    "time_of_event": match[1]["body"]["time_of_event"],
                                     "top_v2": match[1]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
 
 
 def split_every(n, data):
     iterable = iter(data)
```

### Comparing `recon_lw-2.0.0.dev4978172035/setup.py` & `recon_lw-2.0.0.dev4978443614/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4978172035/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4978443614/test/test_recon_ob.py`

 * *Files identical despite different names*

