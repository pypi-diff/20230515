# Comparing `tmp/aw-core-0.5.8.tar.gz` & `tmp/aw-core-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aw-core-0.5.8.tar", max compression
+gzip compressed data, was "aw-core-0.5.9.tar", max compression
```

## Comparing `aw-core-0.5.8.tar` & `aw-core-0.5.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    16726 2017-03-29 21:23:05.967488 aw-core-0.5.8/LICENSE.txt
--rw-r--r--   0        0        0     1582 2021-11-12 12:37:05.178597 aw-core-0.5.8/README.md
--rw-r--r--   0        0        0      557 2021-06-15 10:54:24.171958 aw-core-0.5.8/aw_core/__about__.py
--rw-r--r--   0        0        0      230 2021-06-15 10:32:34.995597 aw-core-0.5.8/aw_core/__init__.py
--rw-r--r--   0        0        0     3292 2022-02-03 11:52:09.447316 aw-core-0.5.8/aw_core/config.py
--rw-r--r--   0        0        0     1620 2022-02-03 11:59:37.205036 aw-core-0.5.8/aw_core/decorators.py
--rw-r--r--   0        0        0     1357 2021-06-15 10:32:34.995597 aw-core-0.5.8/aw_core/dirs.py
--rw-r--r--   0        0        0     4552 2022-02-03 11:52:09.467316 aw-core-0.5.8/aw_core/log.py
--rw-r--r--   0        0        0     4668 2022-02-03 11:59:37.265037 aw-core-0.5.8/aw_core/models.py
--rw-r--r--   0        0        0        0 2021-06-15 10:32:34.995597 aw-core-0.5.8/aw_core/py.typed
--rw-r--r--   0        0        0      422 2017-07-06 20:50:56.847873 aw-core-0.5.8/aw_core/schema.py
--rw-r--r--   0        0        0     1272 2019-03-03 12:37:18.392081 aw-core-0.5.8/aw_core/schemas/bucket.json
--rw-r--r--   0        0        0      382 2017-06-14 21:12:20.094284 aw-core-0.5.8/aw_core/schemas/event.json
--rw-r--r--   0        0        0      411 2019-03-03 12:37:18.392081 aw-core-0.5.8/aw_core/schemas/export.json
--rw-r--r--   0        0        0      747 2022-02-03 11:52:09.480650 aw-core-0.5.8/aw_core/util.py
--rw-r--r--   0        0        0      995 2021-06-15 10:32:34.998930 aw-core-0.5.8/aw_datastore/__init__.py
--rwxr-xr-x   0        0        0     2918 2022-02-03 11:52:36.157591 aw-core-0.5.8/aw_datastore/benchmark.py
--rw-r--r--   0        0        0     6922 2022-03-02 17:08:32.952040 aw-core-0.5.8/aw_datastore/datastore.py
--rw-r--r--   0        0        0     1904 2022-02-03 11:59:37.238370 aw-core-0.5.8/aw_datastore/migration.py
--rw-r--r--   0        0        0        0 2021-06-15 10:32:34.998930 aw-core-0.5.8/aw_datastore/py.typed
--rw-r--r--   0        0        0      261 2019-10-21 05:35:59.703626 aw-core-0.5.8/aw_datastore/storages/__init__.py
--rw-r--r--   0        0        0     2242 2022-03-02 17:08:32.952040 aw-core-0.5.8/aw_datastore/storages/abstract.py
--rw-r--r--   0        0        0     4781 2022-03-02 17:08:32.952040 aw-core-0.5.8/aw_datastore/storages/memory.py
--rw-r--r--   0        0        0     5765 2022-03-02 17:08:32.952040 aw-core-0.5.8/aw_datastore/storages/mongodb.py
--rw-r--r--   0        0        0    10857 2022-03-02 17:08:32.952040 aw-core-0.5.8/aw_datastore/storages/peewee.py
--rw-r--r--   0        0        0    11705 2022-03-02 17:08:32.952040 aw-core-0.5.8/aw_datastore/storages/sqlite.py
--rw-r--r--   0        0        0       73 2019-07-11 18:53:08.085535 aw-core-0.5.8/aw_query/__init__.py
--rw-r--r--   0        0        0      211 2019-07-11 18:53:08.085535 aw-core-0.5.8/aw_query/exceptions.py
--rw-r--r--   0        0        0     8137 2022-02-03 11:52:36.270926 aw-core-0.5.8/aw_query/functions.py
--rw-r--r--   0        0        0        0 2021-06-15 10:32:34.998930 aw-core-0.5.8/aw_query/py.typed
--rw-r--r--   0        0        0    13299 2022-02-03 11:52:36.307593 aw-core-0.5.8/aw_query/query2.py
--rw-r--r--   0        0        0     1107 2021-06-15 10:32:34.998930 aw-core-0.5.8/aw_transform/__init__.py
--rw-r--r--   0        0        0      918 2020-06-30 10:43:25.411451 aw-core-0.5.8/aw_transform/chunk.py
--rw-r--r--   0        0        0     1352 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/chunk_events_by_key.py
--rw-r--r--   0        0        0     2115 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/classify.py
--rw-r--r--   0        0        0      682 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/filter_keyvals.py
--rw-r--r--   0        0        0     5165 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/filter_period_intersect.py
--rw-r--r--   0        0        0     4004 2021-09-02 11:34:38.319851 aw-core-0.5.8/aw_transform/flood.py
--rw-r--r--   0        0        0     1973 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/heartbeats.py
--rw-r--r--   0        0        0     1431 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/merge_events_by_keys.py
--rw-r--r--   0        0        0        0 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/py.typed
--rw-r--r--   0        0        0     1106 2019-07-11 18:53:08.092202 aw-core-0.5.8/aw_transform/simplify.py
--rw-r--r--   0        0        0      908 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/sort_by.py
--rw-r--r--   0        0        0      858 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/split_url_events.py
--rw-r--r--   0        0        0     2650 2021-06-15 10:32:35.002263 aw-core-0.5.8/aw_transform/union_no_overlap.py
--rw-r--r--   0        0        0     1111 2022-03-02 17:08:34.838722 aw-core-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2678 2022-03-02 17:09:36.104932 aw-core-0.5.8/setup.py
--rw-r--r--   0        0        0     2748 2022-03-02 17:09:36.105186 aw-core-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    16726 2017-03-29 21:23:05.967488 aw-core-0.5.9/LICENSE.txt
+-rw-r--r--   0        0        0     1582 2021-11-12 12:37:05.178597 aw-core-0.5.9/README.md
+-rw-r--r--   0        0        0      557 2021-06-15 10:54:24.171958 aw-core-0.5.9/aw_core/__about__.py
+-rw-r--r--   0        0        0      230 2021-06-15 10:32:34.995597 aw-core-0.5.9/aw_core/__init__.py
+-rw-r--r--   0        0        0     3292 2022-02-03 11:52:09.447316 aw-core-0.5.9/aw_core/config.py
+-rw-r--r--   0        0        0     1620 2022-02-03 11:59:37.205036 aw-core-0.5.9/aw_core/decorators.py
+-rw-r--r--   0        0        0     1357 2021-06-15 10:32:34.995597 aw-core-0.5.9/aw_core/dirs.py
+-rw-r--r--   0        0        0     4552 2022-02-03 11:52:09.467316 aw-core-0.5.9/aw_core/log.py
+-rw-r--r--   0        0        0     4668 2022-02-03 11:59:37.265037 aw-core-0.5.9/aw_core/models.py
+-rw-r--r--   0        0        0        0 2021-06-15 10:32:34.995597 aw-core-0.5.9/aw_core/py.typed
+-rw-r--r--   0        0        0      422 2017-07-06 20:50:56.847873 aw-core-0.5.9/aw_core/schema.py
+-rw-r--r--   0        0        0     1272 2019-03-03 12:37:18.392081 aw-core-0.5.9/aw_core/schemas/bucket.json
+-rw-r--r--   0        0        0      382 2017-06-14 21:12:20.094284 aw-core-0.5.9/aw_core/schemas/event.json
+-rw-r--r--   0        0        0      411 2019-03-03 12:37:18.392081 aw-core-0.5.9/aw_core/schemas/export.json
+-rw-r--r--   0        0        0      747 2022-02-03 11:52:09.480650 aw-core-0.5.9/aw_core/util.py
+-rw-r--r--   0        0        0      995 2021-06-15 10:32:34.998930 aw-core-0.5.9/aw_datastore/__init__.py
+-rwxr-xr-x   0        0        0     2918 2022-02-03 11:52:36.157591 aw-core-0.5.9/aw_datastore/benchmark.py
+-rw-r--r--   0        0        0     7012 2022-03-03 10:03:48.145242 aw-core-0.5.9/aw_datastore/datastore.py
+-rw-r--r--   0        0        0     1904 2022-02-03 11:59:37.238370 aw-core-0.5.9/aw_datastore/migration.py
+-rw-r--r--   0        0        0        0 2021-06-15 10:32:34.998930 aw-core-0.5.9/aw_datastore/py.typed
+-rw-r--r--   0        0        0      261 2019-10-21 05:35:59.703626 aw-core-0.5.9/aw_datastore/storages/__init__.py
+-rw-r--r--   0        0        0     2252 2022-03-03 09:51:31.372277 aw-core-0.5.9/aw_datastore/storages/abstract.py
+-rw-r--r--   0        0        0     4858 2022-03-03 09:52:30.586093 aw-core-0.5.9/aw_datastore/storages/memory.py
+-rw-r--r--   0        0        0     5765 2022-03-02 17:08:32.952040 aw-core-0.5.9/aw_datastore/storages/mongodb.py
+-rw-r--r--   0        0        0    11000 2022-03-03 10:04:20.592250 aw-core-0.5.9/aw_datastore/storages/peewee.py
+-rw-r--r--   0        0        0    11776 2022-03-03 10:05:48.356489 aw-core-0.5.9/aw_datastore/storages/sqlite.py
+-rw-r--r--   0        0        0       73 2019-07-11 18:53:08.085535 aw-core-0.5.9/aw_query/__init__.py
+-rw-r--r--   0        0        0      211 2019-07-11 18:53:08.085535 aw-core-0.5.9/aw_query/exceptions.py
+-rw-r--r--   0        0        0     8137 2022-02-03 11:52:36.270926 aw-core-0.5.9/aw_query/functions.py
+-rw-r--r--   0        0        0        0 2021-06-15 10:32:34.998930 aw-core-0.5.9/aw_query/py.typed
+-rw-r--r--   0        0        0    13299 2022-02-03 11:52:36.307593 aw-core-0.5.9/aw_query/query2.py
+-rw-r--r--   0        0        0     1107 2021-06-15 10:32:34.998930 aw-core-0.5.9/aw_transform/__init__.py
+-rw-r--r--   0        0        0      918 2020-06-30 10:43:25.411451 aw-core-0.5.9/aw_transform/chunk.py
+-rw-r--r--   0        0        0     1352 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/chunk_events_by_key.py
+-rw-r--r--   0        0        0     2115 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/classify.py
+-rw-r--r--   0        0        0      682 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/filter_keyvals.py
+-rw-r--r--   0        0        0     5165 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/filter_period_intersect.py
+-rw-r--r--   0        0        0     4004 2021-09-02 11:34:38.319851 aw-core-0.5.9/aw_transform/flood.py
+-rw-r--r--   0        0        0     1973 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/heartbeats.py
+-rw-r--r--   0        0        0     1431 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/merge_events_by_keys.py
+-rw-r--r--   0        0        0        0 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/py.typed
+-rw-r--r--   0        0        0     1106 2019-07-11 18:53:08.092202 aw-core-0.5.9/aw_transform/simplify.py
+-rw-r--r--   0        0        0      908 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/sort_by.py
+-rw-r--r--   0        0        0      858 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/split_url_events.py
+-rw-r--r--   0        0        0     2650 2021-06-15 10:32:35.002263 aw-core-0.5.9/aw_transform/union_no_overlap.py
+-rw-r--r--   0        0        0     1111 2022-03-03 10:09:18.158557 aw-core-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2678 2022-03-03 10:09:48.918494 aw-core-0.5.9/setup.py
+-rw-r--r--   0        0        0     2748 2022-03-03 10:09:48.918742 aw-core-0.5.9/PKG-INFO
```

### Comparing `aw-core-0.5.8/LICENSE.txt` & `aw-core-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/README.md` & `aw-core-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_core/__about__.py` & `aw-core-0.5.9/aw_core/__about__.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_core/config.py` & `aw-core-0.5.9/aw_core/config.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_core/decorators.py` & `aw-core-0.5.9/aw_core/decorators.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_core/dirs.py` & `aw-core-0.5.9/aw_core/dirs.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_core/log.py` & `aw-core-0.5.9/aw_core/log.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_core/models.py` & `aw-core-0.5.9/aw_core/models.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_core/schemas/bucket.json` & `aw-core-0.5.9/aw_core/schemas/bucket.json`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_core/util.py` & `aw-core-0.5.9/aw_core/util.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_datastore/__init__.py` & `aw-core-0.5.9/aw_datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_datastore/benchmark.py` & `aw-core-0.5.9/aw_datastore/benchmark.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_datastore/datastore.py` & `aw-core-0.5.9/aw_datastore/datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,16 @@
                 seconds=second_offset
             )
 
         return self.ds.storage_strategy.get_events(
             self.bucket_id, limit, starttime, endtime
         )
 
-    def get_by_id(self, event_id) -> Event:
+    def get_by_id(self, event_id) -> Optional[Event]:
+        """Will return the event with the provided ID, or None if not found."""
         return self.ds.storage_strategy.get_event(self.bucket_id, event_id)
 
     def get_eventcount(
         self, starttime: datetime = None, endtime: datetime = None
     ) -> int:
         return self.ds.storage_strategy.get_eventcount(
             self.bucket_id, starttime, endtime
```

### Comparing `aw-core-0.5.8/aw_datastore/migration.py` & `aw-core-0.5.9/aw_datastore/migration.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_datastore/storages/abstract.py` & `aw-core-0.5.9/aw_datastore/storages/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         raise NotImplementedError
 
     @abstractmethod
     def get_event(
         self,
         bucket_id: str,
         event_id: int,
-    ) -> Event:
+    ) -> Optional[Event]:
         raise NotImplementedError
 
     @abstractmethod
     def get_events(
         self,
         bucket_id: str,
         limit: int,
```

### Comparing `aw-core-0.5.8/aw_datastore/storages/memory.py` & `aw-core-0.5.9/aw_datastore/storages/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import copy
 from datetime import datetime
-from typing import List, Dict
+from typing import List, Dict, Optional
 
 from aw_core.models import Event
 
 from . import logger
 from .abstract import AbstractStorage
 
 
@@ -49,15 +49,15 @@
             buckets[bucket_id] = self.get_metadata(bucket_id)
         return buckets
 
     def get_event(
         self,
         bucket_id: str,
         event_id: int,
-    ) -> Event:
+    ) -> Optional[Event]:
         event = self._get_event(bucket_id, event_id)
         return copy.deepcopy(event)
 
     def get_events(
         self,
         bucket: str,
         limit: int,
@@ -121,22 +121,24 @@
             for idx, event in reversed(list(enumerate(self.db[bucket_id])))
             if event.id == event_id
         ):
             self.db[bucket_id].pop(idx)
             return True
         return False
 
-    def _get_event(self, bucket_id, event_id):
+    def _get_event(self, bucket_id, event_id) -> Optional[Event]:
         events = [
             event
             for idx, event in reversed(list(enumerate(self.db[bucket_id])))
             if event.id == event_id
         ]
-        assert len(events) == 1
-        return events[0]
+        if len(events) < 1:
+            return None
+        else:
+            return events[0]
 
     def replace(self, bucket_id, event_id, event):
         for idx in (
             idx
             for idx, event in reversed(list(enumerate(self.db[bucket_id])))
             if event.id == event_id
         ):
```

### Comparing `aw-core-0.5.8/aw_datastore/storages/mongodb.py` & `aw-core-0.5.9/aw_datastore/storages/mongodb.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_datastore/storages/peewee.py` & `aw-core-0.5.9/aw_datastore/storages/peewee.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,21 +208,24 @@
 
         # Chunking into lists of length 100 is needed here due to SQLITE_MAX_COMPOUND_SELECT
         # and SQLITE_LIMIT_VARIABLE_NUMBER under Windows.
         # See: https://github.com/coleifer/peewee/issues/948
         for chunk in chunks(events_dictlist, 100):
             EventModel.insert_many(chunk).execute()
 
-    def _get_event(self, bucket_id, event_id) -> EventModel:
-        return (
-            EventModel.select()
-            .where(EventModel.id == event_id)
-            .where(EventModel.bucket == self.bucket_keys[bucket_id])
-            .get()
-        )
+    def _get_event(self, bucket_id, event_id) -> Optional[EventModel]:
+        try:
+            return (
+                EventModel.select()
+                .where(EventModel.id == event_id)
+                .where(EventModel.bucket == self.bucket_keys[bucket_id])
+                .get()
+            )
+        except peewee.DoesNotExist:
+            return None
 
     def _get_last(self, bucket_id) -> EventModel:
         return (
             EventModel.select()
             .where(EventModel.bucket == self.bucket_keys[bucket_id])
             .order_by(EventModel.timestamp.desc())
             .get()
@@ -254,20 +257,20 @@
         event.id = e.id
         return event
 
     def get_event(
         self,
         bucket_id: str,
         event_id: int,
-    ):
+    ) -> Optional[Event]:
         """
         Fetch a single event from a bucket.
         """
         res = self._get_event(bucket_id, event_id)
-        return Event(**EventModel.json(res))
+        return Event(**EventModel.json(res)) if res else None
 
     def get_events(
         self,
         bucket_id: str,
         limit: int,
         starttime: Optional[datetime] = None,
         endtime: Optional[datetime] = None,
```

### Comparing `aw-core-0.5.8/aw_datastore/storages/sqlite.py` & `aw-core-0.5.9/aw_datastore/storages/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,26 +268,29 @@
         self.conditional_commit(1)
         return True
 
     def get_event(
         self,
         bucket_id: str,
         event_id: int,
-    ) -> Event:
+    ) -> Optional[Event]:
         self.commit()
         c = self.conn.cursor()
         query = """
             SELECT id, starttime, endtime, datastr
             FROM events
             WHERE bucketrow = (SELECT rowid FROM buckets WHERE id = ?) AND id = ?
             LIMIT 1
         """
         rows = c.execute(query, [bucket_id, event_id])
         events = _rows_to_events(rows)
-        return events[0]
+        if events:
+            return events[0]
+        else:
+            return None
 
     def get_events(
         self,
         bucket_id: str,
         limit: int,
         starttime: Optional[datetime] = None,
         endtime: Optional[datetime] = None,
```

### Comparing `aw-core-0.5.8/aw_query/functions.py` & `aw-core-0.5.9/aw_query/functions.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_query/query2.py` & `aw-core-0.5.9/aw_query/query2.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/__init__.py` & `aw-core-0.5.9/aw_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/chunk.py` & `aw-core-0.5.9/aw_transform/chunk.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/chunk_events_by_key.py` & `aw-core-0.5.9/aw_transform/chunk_events_by_key.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/classify.py` & `aw-core-0.5.9/aw_transform/classify.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/filter_keyvals.py` & `aw-core-0.5.9/aw_transform/filter_keyvals.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/filter_period_intersect.py` & `aw-core-0.5.9/aw_transform/filter_period_intersect.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/flood.py` & `aw-core-0.5.9/aw_transform/flood.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/heartbeats.py` & `aw-core-0.5.9/aw_transform/heartbeats.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/merge_events_by_keys.py` & `aw-core-0.5.9/aw_transform/merge_events_by_keys.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/simplify.py` & `aw-core-0.5.9/aw_transform/simplify.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/sort_by.py` & `aw-core-0.5.9/aw_transform/sort_by.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/split_url_events.py` & `aw-core-0.5.9/aw_transform/split_url_events.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/aw_transform/union_no_overlap.py` & `aw-core-0.5.9/aw_transform/union_no_overlap.py`

 * *Files identical despite different names*

### Comparing `aw-core-0.5.8/pyproject.toml` & `aw-core-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aw-core"
-version = "0.5.8"
+version = "0.5.9"
 description = "Core library for ActivityWatch"
 authors = ["Erik Bjäreholt <erik@bjareho.lt>", "Johan Bjäreholt <johan@bjareho.lt>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://activitywatch.net/"
 repository = "https://github.com/ActivityWatch/aw-core/"
 documentation = "https://docs.activitywatch.net/"
```

### Comparing `aw-core-0.5.8/setup.py` & `aw-core-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tomlkit']
 
 extras_require = \
 {'mongo': ['pymongo>=3.10.0,<4.0.0']}
 
 setup_kwargs = {
     'name': 'aw-core',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'Core library for ActivityWatch',
     'long_description': 'aw-core\n=======\n\n[![GitHub Actions badge](https://github.com/ActivityWatch/aw-core/workflows/Build/badge.svg)](https://github.com/ActivityWatch/aw-core/actions)\n[![Code coverage](https://codecov.io/gh/ActivityWatch/aw-core/branch/master/graph/badge.svg)](https://codecov.io/gh/ActivityWatch/aw-core)\n[![PyPI](https://img.shields.io/pypi/v/aw-core)](https://pypi.org/project/aw-core/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Typechecking: Mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n\n\nCore library for ActivityWatch.\n\n\n## Modules\n\n - `aw_core`, contains basic datatypes and utilities, such as the `Event` class, helpers for configuration and logging, as well as schemas for buckets, events, and exports.\n - `aw_datastore`, contains the datastore classes used by aw-server-python.\n - `aw_transform`, all event-transforms used in queries.\n - `aw_query`, the query-language used by ActivityWatch.\n\n## Logging\n\nRun python with `LOG_LEVEL=debug` to use change the log level across all AW components\n\n## How to install\n\nTo install the latest git version directly from github without cloning, run\n`pip install git+https://github.com/ActivityWatch/aw-core.git`\n\nTo install from a cloned version, cd into the directory and run\n`poetry install` to install inside an virtualenv. If you want to install it\nsystem-wide it can be installed with `pip install .`, but that has the issue\nthat it might not get the exact version of the dependencies due to not reading\nthe poetry.lock file.\n\n',
     'author': 'Erik Bjäreholt',
     'author_email': 'erik@bjareho.lt',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://activitywatch.net/',
```

### Comparing `aw-core-0.5.8/PKG-INFO` & `aw-core-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aw-core
-Version: 0.5.8
+Version: 0.5.9
 Summary: Core library for ActivityWatch
 Home-page: https://activitywatch.net/
 License: MPL-2.0
 Author: Erik Bjäreholt
 Author-email: erik@bjareho.lt
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved
```

