# Comparing `tmp/recon_lw-2.0.0.dev4979175441.tar.gz` & `tmp/recon_lw-2.0.0.dev4979754584.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4979175441.tar", last modified: Mon May 15 10:16:15 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4979754584.tar", last modified: Mon May 15 11:23:29 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4979175441.tar` & `recon_lw-2.0.0.dev4979754584.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 10:15:58.000000 recon_lw-2.0.0.dev4979175441/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    26660 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:16:15.000000 recon_lw-2.0.0.dev4979175441/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-15 10:15:36.000000 recon_lw-2.0.0.dev4979175441/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 11:23:06.000000 recon_lw-2.0.0.dev4979754584/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26875 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 11:23:29.000000 recon_lw-2.0.0.dev4979754584/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-15 11:22:39.000000 recon_lw-2.0.0.dev4979754584/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4979175441/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4979754584/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4979175441/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4979754584/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4979175441/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4979754584/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4979175441/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4979754584/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4979175441/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4979754584/recon_lw/recon_ob.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,18 @@
                     r["attachedMessageIds"] = [mess["messageId"]]
                     events.append(r)
         
         dbg_event = recon_lw.create_event("DebugEvent",
                                           "DebugEvent",
                                           event_sequence,
                                           ok=True,
-                                          body={"operations": operations, "len(obs)": len(obs), "book_id": book_id},
+                                          body={"operations": [(op[0], op[2]["messageId"]) for op in operations],
+                                                "len(batch)": len(mess_batch),
+                                                "len(obs)": len(obs),
+                                                "book_id": book_id},
                                           parentId=parent_event["eventId"])
         dbg_event["attachedMessageIds"] = list({mess["messageId"] for mess in mess_batch})
         events.append(dbg_event)
 
         if len(obs) >1 and aggregate_batch_updates:
             same_side = all(obs[i]["body"]["aggr_seq"]["affected_side"] == obs[0]["body"]["aggr_seq"]["affected_side"] for i in range(1, len(obs)))
             same_level = all(obs[i]["body"]["aggr_seq"]["affected_level"] == obs[0]["body"]["aggr_seq"]["affected_level"] for i in range(1, len(obs)))
```

### Comparing `recon_lw-2.0.0.dev4979175441/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4979754584/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4979175441/setup.py` & `recon_lw-2.0.0.dev4979754584/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4979175441/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4979754584/test/test_recon_ob.py`

 * *Files identical despite different names*

