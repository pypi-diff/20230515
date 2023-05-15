# Comparing `tmp/recon_lw-2.0.0.dev4948681311.tar.gz` & `tmp/recon_lw-2.0.0.dev4977997714.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4948681311.tar", last modified: Thu May 11 13:58:40 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4977997714.tar", last modified: Mon May 15 08:07:46 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4948681311.tar` & `recon_lw-2.0.0.dev4977997714.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-11 13:58:16.000000 recon_lw-2.0.0.dev4948681311/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    23837 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14757 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:58:40.000000 recon_lw-2.0.0.dev4948681311/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-11 13:58:07.000000 recon_lw-2.0.0.dev4948681311/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 08:07:24.000000 recon_lw-2.0.0.dev4977997714/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26644 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 08:07:46.000000 recon_lw-2.0.0.dev4977997714/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-15 08:07:00.000000 recon_lw-2.0.0.dev4977997714/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4948681311/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4977997714/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4948681311/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4977997714/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4948681311/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4977997714/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4948681311/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4977997714/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4948681311/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4977997714/recon_lw/recon_ob.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,41 +59,47 @@
 
 def flush_sequence_clear_cache(processed_len: int, sequence_cache: dict) -> None:
     sequence = sequence_cache["sequence"]
     for i in range(0, processed_len):
         sequence.pop(0)
 
 
-def process_market_data_update(mess: dict, events: list, books_cache: dict, get_book_id_func,
-                               update_book_rule,
-                               check_book_rule, event_sequence: dict, parent_event: dict,
-                               initial_book_params: dict, log_books_filter,
-                               aggregate_batch_updates) -> None:
-    book_ids_list, result = get_book_id_func(mess)
-    if result is not None:
-        book_id_event = recon_lw.create_event("GetBookEroor:" + parent_event["eventName"], "GetBookEroor",
-                                              event_sequence,
-                                              ok=False,
-                                              body=result,
-                                              parentId=parent_event["eventId"])
-        book_id_event["attachedMessageIds"] = [mess["messageId"]]
-        events.append(book_id_event)
-
-    if book_ids_list is None:
-        return
-    for book_id in book_ids_list:
+def process_market_data_update(mess_batch, events,  books_cache, get_book_id_func ,update_book_rule,
+                               check_book_rule, event_sequence, parent_event, initial_book_params, log_books_filter,
+                               aggregate_batch_updates):
+    books_updates = {}
+    for m in mess_batch:
+        book_ids_list, result = get_book_id_func(m)
+        if result is not None:
+            book_id_event = recon_lw.create_event("GetBookEroor:" + parent_event["eventName"], "GetBookEroor",
+                                                  event_sequence,
+                                                  ok=False,
+                                                  body=result,
+                                                  parentId=parent_event["eventId"])
+            book_id_event["attachedMessageIds"] = [m["messageId"]]
+            events.append(book_id_event)
+        if book_ids_list is not None:
+            for book_id in book_ids_list:
+                if book_id not in books_updates:
+                    books_updates[book_id] = [m]
+                else:
+                    books_updates[book_id].append(m)
+
+    for book_id in books_updates.keys():
         if book_id not in books_cache:
             books_cache[book_id] = copy.deepcopy(initial_book_params)
             # books_cache[book_id] = {"ask": {}, "bid": {}, "status": "?"}
         book = books_cache[book_id]
-        operations = update_book_rule(book, mess)
-        if operations is None:
-            return
+        operations = []
+        for m in books_updates[book_id]:
+            m_operations = update_book_rule(book, m)
+            for op, par in m_operations:
+                operations.append((op, par, m))
         obs = []
-        for operation, parameters in operations:
+        for operation, parameters, mess in operations:
             initial_book = copy.deepcopy(book)
             initial_parameters = copy.copy(parameters)
             parameters["order_book"] = book
             result, log_entries = operation(**parameters)
             if len(result) > 0:
                 result["operation"] = operation.__name__
                 result["operation_params"] = initial_parameters
@@ -132,21 +138,21 @@
                         r["body"]["initial_book"] = initial_book
                     r["body"]["operation"] = operation.__name__
                     r["body"]["book_id"] = book_id
                     r["parentEventId"] = parent_event["eventId"]
                     r["attachedMessageIds"] = [mess["messageId"]]
                     events.append(r)
         
-        dbg_event = recon_lw.create_event("DebugEvent:" + mess["sessionId"],
+        dbg_event = recon_lw.create_event("DebugEvent",
                                           "DebugEvent",
                                           event_sequence,
                                           ok=True,
                                           body={"operations": operations, "len(obs)": len(obs), "book_id": book_id},
                                           parentId=parent_event["eventId"])
-        dbg_event["attachedMessageIds"] = [mess["messageId"]]
+        dbg_event["attachedMessageIds"] = list({mess["messageId"] for mess in mess_batch})
         events.append(dbg_event)
 
         if len(obs) >1 and aggregate_batch_updates:
             same_side = all(obs[i]["body"]["aggr_seq"]["affected_side"] == obs[0]["body"]["aggr_seq"]["affected_side"] for i in range(1, len(obs)))
             same_level = all(obs[i]["body"]["aggr_seq"]["affected_level"] == obs[0]["body"]["aggr_seq"]["affected_level"] for i in range(1, len(obs)))
             obs[0]["body"]["debug_batch_updates"] = len(obs)
             obs[0]["body"]["debug_same_side"] = same_side
@@ -188,18 +194,21 @@
         if "gap" in mess:
             gap_event = recon_lw.create_event("SeqGap:" + parent_event["eventName"], "SeqGap", event_sequence, ok=False,
                                               body={"seq_num": seq}, parentId=parent_event["eventId"])
             events.append(gap_event)
             n_processed += 1
             continue
         chunk = message_utils.expand_message(mess)
-        for m_upd in chunk:
-            process_market_data_update(m_upd, events, books_cache, get_book_id_func, update_book_rule,
-                                       check_book_rule, event_sequence, parent_event, initial_book_params,
-                                       log_books_filter, aggregate_batch_updates)
+        process_market_data_update(chunk, events, books_cache, get_book_id_func, update_book_rule,
+                                   check_book_rule, event_sequence, parent_event, initial_book_params,
+                                   log_books_filter, aggregate_batch_updates)
+        #for m_upd in chunk:
+        #    process_market_data_update(m_upd, events, books_cache, get_book_id_func, update_book_rule,
+        #                               check_book_rule, event_sequence, parent_event, initial_book_params,
+        #                               log_books_filter, aggregate_batch_updates)
         n_processed += 1
 
     send_events_func(events)
     return n_processed
 
 
 def init_ob_stream(rule_settings: dict) -> None:
@@ -249,112 +258,129 @@
         dupl_events.append(d_ev)
     save_events_func(dupl_events)
     duplicates.clear()
     flush_sequence_clear_cache(n_processed, rule_settings["sequence_cache"])
 
 
 def init_aggr_seq(order_book: dict) -> None:
-    order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0}
+    order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0, "limit_v2" : 0, "top_v2" : 0}
 
 
 def reset_aggr_seq(order_book):
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0, "affected_side": "na", "affected_level": -1})
 
 
-def reflect_price_update_in_version(side: str, price: float, order_book: dict):
+def reflect_price_update_in_version(side: str, price: float,str_time_of_event,order_book: dict):
     level = get_price_level(side, price, order_book)
     order_book["aggr_seq"]["affected_side"] = side
     order_book["aggr_seq"]["affected_level"] = level
 
     max_levels = order_book["aggr_max_levels"]
     if level <= max_levels:
         order_book["aggr_seq"]["limit_v"] += 1
         order_book["aggr_seq"]["limit_delta"] = 1
     if level == 1:
         order_book["aggr_seq"]["top_v"] += 1
         order_book["aggr_seq"]["top_delta"] = 1
 
+    if "time_of_event" not in order_book:
+        order_book["time_of_event"] = str_time_of_event
+        order_book["aggr_seq"]["limit_v2"] = 0
+        order_book["aggr_seq"]["limit_v2"] = 0
+    else:
+        if str_time_of_event == order_book["time_of_event"]:
+            if level <= max_levels:
+                order_book["aggr_seq"]["limit_v2"] += 1
+            if level == 1:
+                order_book["aggr_seq"]["top_v2"] += 1
+        else:
+            order_book["time_of_event"] = str_time_of_event
+            order_book["aggr_seq"]["limit_v2"] = 0
+            order_book["aggr_seq"]["limit_v2"] = 0
+
 
-def ob_add_order(order_id: str, price: float, size: int, side: str, order_book: dict) -> tuple:
+def ob_add_order(order_id: str, price: float, size: int, side: str, str_time_of_event ,order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     if find_order_position(order_id, order_book)[0] is not None:
         return {"error": order_id + " already exists"}, []
     if price not in order_book[side]:
         order_book[side][price] = {order_id: size}
     else:
         order_book[side][price][order_id] = size
 
-    reflect_price_update_in_version(side, price, order_book)
+    reflect_price_update_in_version(side, price, str_time_of_event ,order_book)
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_update_order(order_id: str, price: float, size: int, order_book: dict) -> tuple:
+def ob_update_order(order_id: str, price: float, size: int, str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
         return {"error": order_id + " not found"}, []
 
     log = []
     if price == old_price:
         order_book[old_side][old_price][order_id] = size
-        reflect_price_update_in_version(old_side, old_price, order_book)
+        reflect_price_update_in_version(old_side, old_price, str_time_of_event, order_book)
         log.append(copy.deepcopy(order_book))
     else:
         # should no get here but will monitor
-        reflect_price_update_in_version(old_side, old_price, order_book)
+        reflect_price_update_in_version(old_side, old_price, str_time_of_event, order_book)
         order_book[old_side][old_price].pop(order_id)
         if len(order_book[old_side][old_price]) == 0:
             order_book[old_side].pop(old_price)
         log.append(copy.deepcopy(order_book))
         if price not in order_book[old_side]:
             order_book[old_side][price] = {}
         order_book[old_side][price][order_id] = size
-        reflect_price_update_in_version(old_side, price, order_book)
+        reflect_price_update_in_version(old_side, price, str_time_of_event, order_book)
         log.append(copy.deepcopy(order_book))
 
     return {}, log
 
 
-def ob_delete_order(order_id: str, order_book: dict) -> tuple:
+def ob_delete_order(order_id: str, str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
         return {"error": order_id + " not found"}, []
 
     log = []
-    reflect_price_update_in_version(old_side, old_price, order_book)
+    reflect_price_update_in_version(old_side, old_price,str_time_of_event,order_book)
     order_book[old_side][old_price].pop(order_id)
     if len(order_book[old_side][old_price]) == 0:
         order_book[old_side].pop(old_price)
         log.append(copy.deepcopy(order_book))
         max_levels = order_book["aggr_max_levels"]
         if len(order_book[old_side]) >= max_levels and order_book["aggr_seq"]["limit_delta"] == 1:
             # back from horizon update
             order_book["aggr_seq"]["limit_delta"] = 2
             order_book["aggr_seq"]["limit_v"] += 1
+            order_book["aggr_seq"]["limit_v2"] += 1
+
             log.append(copy.deepcopy(order_book))
     else:
         log.append(copy.deepcopy(order_book))
 
     return {}, log
 
 
-def ob_trade_order(order_id: str, traded_size: int, order_book: dict) -> tuple:
+def ob_trade_order(order_id: str, traded_size: int, str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     log = []
@@ -369,47 +395,52 @@
             order_book[old_side].pop(old_price)
             log.append(copy.deepcopy(order_book))
             max_levels = order_book["aggr_max_levels"]
             if len(order_book[old_side]) >= max_levels and order_book["aggr_seq"]["limit_delta"] == 1:
                 # back from horizon update
                 order_book["aggr_seq"]["limit_delta"] = 2
                 order_book["aggr_seq"]["limit_v"] += 1
+                order_book["aggr_seq"]["limit_v2"] += 1
                 log.append(copy.deepcopy(order_book))
         else:
             log.append(copy.deepcopy(order_book))
     else:
-        reflect_price_update_in_version(old_side, old_price, order_book)
+        reflect_price_update_in_version(old_side, old_price, str_time_of_event ,order_book)
         order_book[old_side][old_price][order_id] -= traded_size
         log.append(copy.deepcopy(order_book))
     return {}, log
 
 
-def ob_clean_book(order_book: dict) -> tuple:
+def ob_clean_book(str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     for side_key in ["ask", "bid"]:
         if side_key in order_book:
             order_book[side_key].clear()
+
+    update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_change_status(new_status: str, order_book: dict) -> tuple:
+def ob_change_status(new_status: str, str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     order_book["status"] = new_status
+
+    update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
@@ -426,16 +457,31 @@
     if p not in order_book[side]:
         return -1
     levels = list(order_book[side].keys())
     levels.sort()
     return levels.index(p) + 1 if side == "ask" else len(levels) - levels.index(p)
 
 
+def update_time_and_version(str_time_of_event, order_book):
+    if "time_of_event" not in order_book:
+        order_book["time_of_event"] = str_time_of_event
+        order_book["aggr_seq"]["limit_v2"] = 0
+        order_book["aggr_seq"]["top_v2"] = 0
+    else:
+        if str_time_of_event == order_book["time_of_event"]:
+            order_book["aggr_seq"]["limit_v2"] += 1
+            order_book["aggr_seq"]["top_v2"] += 1
+        else:
+            order_book["aggr_seq"]["limit_v2"] = 0
+            order_book["aggr_seq"]["top_v2"] = 0
+            order_book["time_of_event"] = str_time_of_event
+
+
 def ob_aggr_add_level(side: str, level: int, price: float, real_qty: int, real_num_orders: int, impl_qty: int,
-                      impl_num_orders: int, order_book: dict):
+                      impl_num_orders: int, str_time_of_event, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
@@ -446,41 +492,45 @@
         return result_body, []
 
     new_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, "impl_qty": impl_qty,
                  "impl_num_orders": impl_num_orders}
     order_book[side_key].insert(new_index, new_level)
     if len(order_book[side_key]) == max_levels + 1:
         order_book[side_key].pop()
+
+    update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_aggr_delete_level(side: str, level: int, order_book: dict) -> tuple:
+def ob_aggr_delete_level(side: str, level: int, str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     result_body = {}
     side_key = side + "_aggr"
     del_index = level - 1
     if not 0 <= del_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
 
     order_book[side_key].pop(del_index)
 
+    update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_update_level(side: str, level: int, price: float, real_qty: int, real_num_orders: int, impl_qty: int,
-                         impl_num_orders: int, order_book: dict) -> tuple:
+                         impl_num_orders: int,
+                         str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
@@ -489,35 +539,37 @@
     if not 0 <= update_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
 
     upd_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders,
                  "impl_qty": impl_qty, "impl_num_orders": impl_num_orders}
     order_book[side_key][update_index].update(upd_level)
+    update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
 
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_aggr_clean_book(order_book: dict) -> tuple:
+def ob_aggr_clean_book(str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     for side_key in ["ask_aggr", "bid_aggr"]:
         if side_key in order_book:
             order_book[side_key].clear()
+    update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_top_clean_book(order_book: dict) -> tuple:
+def ob_top_clean_book(str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     order_book["ask_price"] = 0
     order_book["ask_real_qty"] = 0
@@ -526,23 +578,24 @@
     order_book["ask_impl_n_orders"] = 0
     order_book["bid_price"] = 0
     order_book["bid_real_qty"] = 0
     order_book["bid_impl_qty"] = 0
     order_book["bid_real_n_orders"] = 0
     order_book["bid_impl_n_orders"] = 0
 
+    update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
 
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_top_update(ask_price: str, ask_real_qty: str, ask_impl_qty: str, ask_real_n_orders: str, ask_impl_n_orders: str,
                   bid_price: int, bid_real_qty: str, bid_impl_qty: str, bid_real_n_orders: int, bid_impl_n_orders: str,
-                  order_book: dict) -> tuple:
+                  str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
@@ -551,11 +604,12 @@
     order_book["ask_impl_n_orders"] = ask_impl_n_orders
     order_book["bid_price"] = bid_price
     order_book["bid_real_qty"] = bid_real_qty
     order_book["bid_impl_qty"] = bid_impl_qty
     order_book["bid_real_n_orders"] = bid_real_n_orders
     order_book["bid_impl_n_orders"] = bid_impl_n_orders
 
+    update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
 
     return {}, [copy.deepcopy(order_book)]
```

### Comparing `recon_lw-2.0.0.dev4948681311/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4977997714/recon_lw/recon_ob_cross_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,108 +83,116 @@
     else:
         if top_book["bid_real_qty"] != 0 or top_book["bid_impl_qty"] != 0:
             problems.append({"synopsys": "full_miss_level", "side": "bid"})
     return problems
 
 
 def ob_compare_get_timestamp_key1_key2_aggr(o, custom_settings):
-    if o["body"]["aggr_seq"]["limit_delta"] != 1:
+    if o["body"]["aggr_seq"]["limit_delta"] not in [1, 2]:
         return None, None, None
     if o["body"]["sessionId"] == custom_settings["full_session"]:
-        return o["body"]["timestamp"], "{0}_{1}".format(o["body"]["book_id"], o["body"]["aggr_seq"]["limit_v"]), None
+        return o["body"]["timestamp"], "{0}_{1}_{2}".format(o["body"]["book_id"],
+                                                            o["body"]["time_of_event"],
+                                                            o["body"]["aggr_seq"]["limit_v2"]), None
 
     if o["body"]["sessionId"] == custom_settings["comp_session"]:
-        return o["body"]["timestamp"], None, "{0}_{1}".format(o["body"]["book_id"], o["body"]["aggr_seq"]["limit_v"])
+        return o["body"]["timestamp"], None, "{0}_{1}_{2}".format(o["body"]["book_id"],
+                                                                  o["body"]["time_of_event"],
+                                                                  o["body"]["aggr_seq"]["limit_v2"])
 
     return None, None, None
 
 
 def ob_compare_get_timestamp_key1_key2_top(o, custom_settings):
-    if o["body"]["aggr_seq"]["top_delta"] != 1:
+    if o["body"]["aggr_seq"]["top_delta"] not in [1, 2]:
         return None, None, None
 
     if o["body"]["sessionId"] == custom_settings["full_session"]:
-        return o["body"]["timestamp"], "{0}_{1}".format(o["body"]["book_id"], o["body"]["aggr_seq"]["top_v"]), None
+        return o["body"]["timestamp"], "{0}_{1}_{2}".format(o["body"]["book_id"],
+                                                            o["body"]["time_of_event"],
+                                                            o["body"]["aggr_seq"]["top_v2"]), None
 
     if o["body"]["sessionId"] == custom_settings["comp_session"]:
-        return o["body"]["timestamp"], None, "{0}_{1}".format(o["body"]["book_id"], o["body"]["aggr_seq"]["top_v"])
+        return o["body"]["timestamp"], None, "{0}_{1}_{2}".format(o["body"]["book_id"],
+                                                                  o["body"]["time_of_event"],
+                                                                  o["body"]["aggr_seq"]["top_v2"])
 
     return None, None, None
 
 
 def ob_compare_interpret_match_aggr(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_full_vs_aggr(match[0]["body"], match[1]["body"])
         if len(comp_res) > 0:
             error_event = create_event("StreamMismatchAggr",
                                        "StreamMismatchAggr",
                                        False,
                                        {"full_book_event": match[0]["eventId"],
                                         "aggr_book_event": match[1]["eventId"],
                                         "book_id": match[0]["body"]["book_id"],
-                                        "limit_v": match[0]["body"]["aggr_seq"]["limit_v"],
-                                        "top_v": match[0]["body"]["aggr_seq"]["top_v"],
+                                        "time_of_event": match[0]["body"]["time_of_event"],
+                                        "limit_v2": match[0]["body"]["aggr_seq"]["limit_v2"],
                                         "errors": comp_res})
             save_events([error_event])
     elif match[0] is not None:
         tech_info = ob_compare_get_timestamp_key1_key2_aggr(match[0], custom_settings)
         error_event = create_event("StreamMismatchNoAggr",
                                    "StreamMismatchNoAggr",
                                    False,
                                    {"full_book_event": match[0]["eventId"],
                                     "book_id": match[0]["body"]["book_id"],
-                                    "limit_v": match[0]["body"]["aggr_seq"]["limit_v"],
-                                    "top_v": match[0]["body"]["aggr_seq"]["top_v"],
+                                    "time_of_event": match[0]["body"]["time_of_event"],
+                                    "limit_v2": match[0]["body"]["aggr_seq"]["limit_v2"],
                                     "sessionId": match[0]["body"]["sessionId"],
                                     "tech_info": tech_info})
         save_events([error_event])
     elif match[1] is not None:
         error_event = create_event("StreamMismatchNoFull",
                                    "StreamMismatchNoFull",
                                    False,
                                    {"aggr_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
-                                    "limit_v": match[1]["body"]["aggr_seq"]["limit_v"],
-                                   "top_v": match[1]["body"]["aggr_seq"]["top_v"],
+                                    "time_of_event": match[0]["body"]["time_of_event"],
+                                   "limit_v2": match[1]["body"]["aggr_seq"]["limit_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
 
 
 def ob_compare_interpret_match_top(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_full_vs_top(match[0]["body"], match[1]["body"])
         if len(comp_res) > 0:
             error_event = create_event("StreamMismatchTop",
                                        "StreamMismatchTop",
                                        False,
                                        {"full_book_event": match[0]["eventId"],
                                         "top_book_event": match[1]["eventId"],
                                         "book_id": match[0]["body"]["book_id"],
-                                        "limit_v": match[0]["body"]["aggr_seq"]["limit_v"],
-                                        "top_v": match[0]["body"]["aggr_seq"]["top_v"],
+                                        "time_of_event": match[0]["body"]["time_of_event"],
+                                        "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
                                         "errors": comp_res})
             save_events([error_event])
     elif match[0] is not None:
         error_event = create_event("StreamMismatchNoTop",
                                    "StreamMismatchNoTop",
                                    False,
                                    {"full_book_event": match[0]["eventId"],
                                     "book_id": match[0]["body"]["book_id"],
-                                    "limit_v": match[0]["body"]["aggr_seq"]["limit_v"],
-                                    "top_v": match[0]["body"]["aggr_seq"]["top_v"],
+                                    "time_of_event": match[0]["body"]["time_of_event"],
+                                    "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[0]["body"]["sessionId"]})
         save_events([error_event])
     elif match[1] is not None:
         error_event = create_event("StreamMismatchNoFull",
                                    "StreamMismatchNoFull",
                                    False,
                                    {"top_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
-                                    "limit_v": match[1]["body"]["aggr_seq"]["limit_v"],
-                                    "top_v": match[1]["body"]["aggr_seq"]["limit_v"],
+                                    "time_of_event": match[0]["body"]["time_of_event"],
+                                    "top_v2": match[1]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
 
 
 def split_every(n, data):
     iterable = iter(data)
     while 1:
```

### Comparing `recon_lw-2.0.0.dev4948681311/setup.py` & `recon_lw-2.0.0.dev4977997714/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4948681311/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4977997714/test/test_recon_ob.py`

 * *Files identical despite different names*

