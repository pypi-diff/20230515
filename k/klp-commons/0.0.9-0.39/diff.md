# Comparing `tmp/klp-commons-0.0.9.tar.gz` & `tmp/klp_commons-0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klp-commons-0.0.9.tar", last modified: Thu Mar 16 18:07:10 2023, max compression
+gzip compressed data, was "klp_commons-0.39.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `klp-commons-0.0.9.tar` & `klp_commons-0.39.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0     1082 2023-03-11 16:29:59.052345 klp-commons-0.0.9/LICENSE
--rw-r--r--   0        0        0     4840 2023-03-11 17:02:05.306612 klp-commons-0.0.9/README.md
--rw-r--r--   0        0        0    10244 2023-03-15 02:52:05.661685 klp-commons-0.0.9/klp_commons/.DS_Store
--rw-r--r--   0        0        0      624 2023-03-16 18:05:31.245053 klp-commons-0.0.9/klp_commons/__init__.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:21.254936 klp-commons-0.0.9/klp_commons/controllers/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/controllers/__init__.py
--rw-r--r--   0        0        0    31510 2023-03-13 05:25:25.017217 klp-commons-0.0.9/klp_commons/controllers/controller_dynamodb.py
--rw-r--r--   0        0        0      260 2023-02-16 19:52:02.340344 klp-commons-0.0.9/klp_commons/controllers/controller_mlflow.py
--rw-r--r--   0        0        0     6591 2023-03-14 16:59:36.965113 klp-commons-0.0.9/klp_commons/controllers/controller_mongodb.py
--rw-r--r--   0        0        0    49187 2023-03-12 05:47:13.143660 klp-commons-0.0.9/klp_commons/controllers/controller_postgresdb.py
--rw-r--r--   0        0        0    34378 2023-03-16 17:06:01.490903 klp-commons-0.0.9/klp_commons/controllers/controller_redshift.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:23.888578 klp-commons-0.0.9/klp_commons/cryptools/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/cryptools/__init__.py
--rw-r--r--   0        0        0      795 2022-11-14 19:44:11.325419 klp-commons-0.0.9/klp_commons/cryptools/cryptology.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:26.531304 klp-commons-0.0.9/klp_commons/datadict/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/datadict/__init__.py
--rw-r--r--   0        0        0    24123 2023-03-14 04:27:56.957869 klp-commons-0.0.9/klp_commons/datadict/struct_dicts.py
--rw-r--r--   0        0        0    18932 2023-03-12 05:47:05.332172 klp-commons-0.0.9/klp_commons/datefinder/__init__.py
--rw-r--r--   0        0        0     8208 2023-01-03 03:53:19.224934 klp-commons-0.0.9/klp_commons/datefinder/constants.py
--rw-r--r--   0        0        0      628 2023-01-03 03:53:19.225149 klp-commons-0.0.9/klp_commons/datefinder/date_fragment.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:29.092392 klp-commons-0.0.9/klp_commons/log/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/log/__init__.py
--rw-r--r--   0        0        0     2384 2023-02-16 19:52:02.267127 klp-commons-0.0.9/klp_commons/log/log.py
--rw-r--r--   0        0        0      350 2022-12-28 18:14:36.139801 klp-commons-0.0.9/klp_commons/log/structuredMessage.py
--rw-r--r--   0        0        0        0 2023-01-03 03:53:19.226945 klp-commons-0.0.9/klp_commons/places/__init__.py
--rw-r--r--   0        0        0      396 2023-01-03 03:53:19.263289 klp-commons-0.0.9/klp_commons/places/apis.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:31.869752 klp-commons-0.0.9/klp_commons/scripts/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/scripts/__init__.py
--rw-r--r--   0        0        0    14823 2023-02-21 13:40:03.843358 klp-commons-0.0.9/klp_commons/scripts/detect_recurrency.py
--rw-r--r--   0        0        0     6173 2023-02-21 13:40:03.843531 klp-commons-0.0.9/klp_commons/scripts/get_send_kw_group.py
--rw-r--r--   0        0        0    22232 2023-03-16 16:11:46.946090 klp-commons-0.0.9/klp_commons/scripts/ingest_dwh.py
--rw-r--r--   0        0        0    30962 2023-03-14 14:00:46.771225 klp-commons-0.0.9/klp_commons/scripts/summary.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:36.942806 klp-commons-0.0.9/klp_commons/streaming/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/streaming/__init__.py
--rw-r--r--   0        0        0     3747 2023-02-21 13:40:03.842168 klp-commons-0.0.9/klp_commons/streaming/consumer.py
--rw-r--r--   0        0        0      959 2023-03-12 06:38:51.960204 klp-commons-0.0.9/klp_commons/streaming/producer.py
--rw-r--r--   0        0        0     6148 2023-03-11 15:04:19.230154 klp-commons-0.0.9/klp_commons/utils/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-03 03:53:19.227104 klp-commons-0.0.9/klp_commons/utils/__init__.py
--rw-r--r--   0        0        0      408 2023-02-16 19:52:02.303071 klp-commons-0.0.9/klp_commons/utils/utils.py
--rw-r--r--   0        0        0      470 2023-03-12 05:35:00.941176 klp-commons-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 klp-commons-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-03-11 16:29:59.052345 klp_commons-0.39/LICENSE
+-rw-r--r--   0        0        0     4840 2023-03-11 17:02:05.306612 klp_commons-0.39/README.md
+-rw-r--r--   0        0        0    10244 2023-04-04 00:02:28.383456 klp_commons-0.39/klp_commons/.DS_Store
+-rw-r--r--   0        0        0      624 2023-05-15 01:58:24.649923 klp_commons-0.39/klp_commons/__init__.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:21.254936 klp_commons-0.39/klp_commons/controllers/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp_commons-0.39/klp_commons/controllers/__init__.py
+-rw-r--r--   0        0        0    31495 2023-04-18 21:43:28.811601 klp_commons-0.39/klp_commons/controllers/controller_dynamodb.py
+-rw-r--r--   0        0        0      260 2023-02-16 19:52:02.340344 klp_commons-0.39/klp_commons/controllers/controller_mlflow.py
+-rw-r--r--   0        0        0    10047 2023-05-15 01:58:00.377865 klp_commons-0.39/klp_commons/controllers/controller_mongodb.py
+-rw-r--r--   0        0        0    51677 2023-04-26 17:23:32.712933 klp_commons-0.39/klp_commons/controllers/controller_postgresdb.py
+-rw-r--r--   0        0        0    40312 2023-05-04 16:43:17.912366 klp_commons-0.39/klp_commons/controllers/controller_redshift.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:23.888578 klp_commons-0.39/klp_commons/cryptools/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp_commons-0.39/klp_commons/cryptools/__init__.py
+-rw-r--r--   0        0        0      795 2022-11-14 19:44:11.325419 klp_commons-0.39/klp_commons/cryptools/cryptology.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:26.531304 klp_commons-0.39/klp_commons/datadict/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp_commons-0.39/klp_commons/datadict/__init__.py
+-rw-r--r--   0        0        0    25764 2023-05-03 23:08:10.607891 klp_commons-0.39/klp_commons/datadict/struct_dicts.py
+-rw-r--r--   0        0        0    18932 2023-03-12 05:47:05.332172 klp_commons-0.39/klp_commons/datefinder/__init__.py
+-rw-r--r--   0        0        0     8208 2023-01-03 03:53:19.224934 klp_commons-0.39/klp_commons/datefinder/constants.py
+-rw-r--r--   0        0        0      628 2023-01-03 03:53:19.225149 klp_commons-0.39/klp_commons/datefinder/date_fragment.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:29.092392 klp_commons-0.39/klp_commons/log/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp_commons-0.39/klp_commons/log/__init__.py
+-rw-r--r--   0        0        0     2384 2023-02-16 19:52:02.267127 klp_commons-0.39/klp_commons/log/log.py
+-rw-r--r--   0        0        0      350 2022-12-28 18:14:36.139801 klp_commons-0.39/klp_commons/log/structuredMessage.py
+-rw-r--r--   0        0        0        0 2023-01-03 03:53:19.226945 klp_commons-0.39/klp_commons/places/__init__.py
+-rw-r--r--   0        0        0      396 2023-01-03 03:53:19.263289 klp_commons-0.39/klp_commons/places/apis.py
+-rw-r--r--   0        0        0     6148 2023-04-05 13:14:51.122885 klp_commons-0.39/klp_commons/scripts/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp_commons-0.39/klp_commons/scripts/__init__.py
+-rw-r--r--   0        0        0    14823 2023-02-21 13:40:03.843358 klp_commons-0.39/klp_commons/scripts/detect_recurrency.py
+-rw-r--r--   0        0        0     6028 2023-03-30 23:42:51.602596 klp_commons-0.39/klp_commons/scripts/get_send_kw_group.py
+-rw-r--r--   0        0        0    21184 2023-04-05 13:13:30.504595 klp_commons-0.39/klp_commons/scripts/ingest_dwh.py
+-rw-r--r--   0        0        0    30962 2023-03-14 14:00:46.771225 klp_commons-0.39/klp_commons/scripts/summary.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:36.942806 klp_commons-0.39/klp_commons/streaming/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp_commons-0.39/klp_commons/streaming/__init__.py
+-rw-r--r--   0        0        0     3747 2023-02-21 13:40:03.842168 klp_commons-0.39/klp_commons/streaming/consumer.py
+-rw-r--r--   0        0        0      959 2023-03-12 06:38:51.960204 klp_commons-0.39/klp_commons/streaming/producer.py
+-rw-r--r--   0        0        0 13017595 2023-04-04 01:32:22.563678 klp_commons-0.39/klp_commons/streaming/topics.log
+-rw-r--r--   0        0        0    11644 2023-04-05 13:13:36.175660 klp_commons-0.39/klp_commons/streaming/topics.py
+-rw-r--r--   0        0        0     6148 2023-03-11 15:04:19.230154 klp_commons-0.39/klp_commons/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-03 03:53:19.227104 klp_commons-0.39/klp_commons/utils/__init__.py
+-rw-r--r--   0        0        0      411 2023-04-02 02:52:35.126978 klp_commons-0.39/klp_commons/utils/utils.py
+-rw-r--r--   0        0        0      470 2023-03-12 05:35:00.941176 klp_commons-0.39/pyproject.toml
+-rw-r--r--   0        0        0     5220 1970-01-01 00:00:00.000000 klp_commons-0.39/PKG-INFO
```

### Comparing `klp-commons-0.0.9/LICENSE` & `klp_commons-0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/README.md` & `klp_commons-0.39/README.md`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/.DS_Store` & `klp_commons-0.39/klp_commons/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -437,16 +437,16 @@
 00001b40: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 00001b50: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
 00001b60: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
 00001b70: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 00001b80: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 00001b90: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
 00001ba0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-00001bb0: 177b 7b30 2c20 3131 377d 2c20 7b31 3434  .{{0, 117}, {144
-00001bc0: 302c 2037 3436 7d7d 0908 1725 313d 4960  0, 746}}...%1=I`
+00001bb0: 177b 7b30 2c20 3132 357d 2c20 7b31 3433  .{{0, 125}, {143
+00001bc0: 392c 2037 3530 7d7d 0908 1725 313d 4960  9, 750}}...%1=I`
 00001bd0: 6d79 7a7b 7c7d 7e98 0000 0000 0000 0101  myz{|}~.........
 00001be0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 00001bf0: 0000 0000 0000 0099 0000 0009 0073 0074  .............s.t
 00001c00: 0072 0065 0061 006d 0069 006e 0067 6473  .r.e.a.m.i.n.gds
 00001c10: 636c 626f 6f6c 0000 0000 0900 7300 7400  clbool......s.t.
 00001c20: 7200 6500 6100 6d00 6900 6e00 676c 6731  r.e.a.m.i.n.glg1
 00001c30: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
@@ -465,16 +465,16 @@
 00001d00: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 00001d10: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
 00001d20: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
 00001d30: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
 00001d40: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
 00001d50: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
 00001d60: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00001d70: 095f 1017 7b7b 302c 2031 3137 7d2c 207b  ._..{{0, 117}, {
-00001d80: 3134 3430 2c20 3734 367d 7d09 0817 2531  1440, 746}}...%1
+00001d70: 095f 1017 7b7b 302c 2031 3235 7d2c 207b  ._..{{0, 125}, {
+00001d80: 3134 3339 2c20 3735 307d 7d09 0817 2531  1439, 750}}...%1
 00001d90: 3d49 606d 797a 7b7c 7d7e 9800 0000 0000  =I`myz{|}~......
 00001da0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
 00001db0: 0000 0000 0000 0000 0000 9900 0000 0500  ................
 00001dc0: 7500 7400 6900 6c00 7364 7363 6c62 6f6f  u.t.i.l.sdsclboo
 00001dd0: 6c00 0000 0005 0075 0074 0069 006c 0073  l......u.t.i.l.s
 00001de0: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `klp-commons-0.0.9/klp_commons/__init__.py` & `klp_commons-0.39/klp_commons/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
     from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
 
 try:
     __version__ = version(__name__)
 except PackageNotFoundError:  # pragma: no cover
-    __version__ = "0.0.9"
+    __version__ = "0.039"
 
     log = logging.getLogger(__name__)
```

### Comparing `klp-commons-0.0.9/klp_commons/controllers/.DS_Store` & `klp_commons-0.39/klp_commons/controllers/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/controllers/controller_dynamodb.py` & `klp_commons-0.39/klp_commons/controllers/controller_dynamodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 content=e.response["Error"], status_code=500
             )
             self.logger.error(fmt("transaction : ", json=transaction))
 
     def insert_batch_hash_in_userTable(self, items_list: list) -> dict:
 
         try:
-            with self.active_conection_table.batch_writer(overwrite_by_pkeys=["user_uid", "hash"]) as writer:
+            with self.active_conection_table.batch_writer(overwrite_by_pkeys=["user_uid", "description_embedding"]) as writer:
                 for item in items_list:
                     writer.put_item(Item=item)
             self.logger.info("Loaded data into table %s.",
                              self.active_conection_table.name)
         except ClientError:
             self.logger.exception(
                 "Couldn't load data into table %s.", self.active_conection_table.name)
@@ -525,19 +525,18 @@
                     partition_key_value
                 )
                 & Key(self.sort_key_name).eq(sort_key_value),
                 # ProjectionExpression = self.hash
             )
 
         except ClientError as e:
-            self.r_query_dydb = JSONResponse(
-                content=e.response["Error"], status_code=500
-            )
-            self.logger.error(fmt("user iud ", json={
-                'partition_key_value': partition_key_value, 'sort_key_value': sort_key_value}))
+            self.r_query_dydb = e.response["Error"]
+
+            self.logger.error(fmt("error:  user iud ", json={
+                'partition_key_value': partition_key_value, 'sort_key_value': sort_key_value,"error":e.response["Error"]}))
 
         self.logger.info(
             "done get_hash_in_transactionTable method of ControllerDynamoDB ")
 
     def created_info_in_userTable(self, info: dict = None):
         """
         Updates user table.
```

### Comparing `klp-commons-0.0.9/klp_commons/controllers/controller_postgresdb.py` & `klp_commons-0.39/klp_commons/controllers/controller_postgresdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,35 @@
 from logging import getLogger
 
 fmt = StructuredMessage
 message = 'postgresDBController'
 
 class ControllerPostgresDB:
 
-    def __init__(self):
+    def __init__(self, conf = None):
 
         self.conn = None
         self.logger = getLogger('categorization.ControllerPosgrestDB')
 
         # Init ()
         self.logger.info('ControllerPosgrestDB.init()')
         self.logger.info('creating an instance of ControllerPosgrestDB')
-        self.PG_HOST = getenv('PG_HOST')
-        self.PG_DATABASE = getenv('PG_DATABASE')
-        self.PG_USER = getenv('PG_USER')
-        self.PG_PASSWORD = getenv('PG_PASSWORD')
-        self.PG_PORT = getenv('PG_PORT')
+        if conf is None:
+            self.PG_HOST = getenv('PG_HOST')
+            self.PG_DATABASE = getenv('PG_DATABASE')
+            self.PG_USER = getenv('PG_USER')
+            self.PG_PASSWORD = getenv('PG_PASSWORD')
+            self.PG_PORT = getenv('PG_PORT')
+        else :
+            self.PG_HOST = conf['PG_HOST']
+            self.PG_DATABASE = conf['PG_DATABASE']
+            self.PG_USER = conf['PG_USER']
+            self.PG_PASSWORD = conf['PG_PASSWORD']
+            self.PG_PORT = conf['PG_PORT']
+        
         self.format_exter = '%Y-%m-%dT%H:%M:%S' # .%f%z'
         self.format_inter = '%Y-%m-%dT%H:%M:%S'
         self.logger.info('donecreating an instance of ControllerPosgrestDB')
 
     def get_conection(self) -> None:
         self.logger.info('call get_conection method ')
 
@@ -43,14 +51,97 @@
         except BaseException as e:
             self.conn.rollback()
             self.logger.exception(e, exc_info=True)
             self.logger.error('Error conection postgres DB ', self.conn)
 
         self.logger.info('done call get_conection')
 
+    def execute_query(
+            self, query=None) -> None:
+
+        self.logger.info('call execute_query ')
+        self.get_conection()
+        obj = None  
+
+        try :
+            with self.conn.cursor() as cur:
+
+                cur.execute(query)
+
+                obj = cur.fetchone()
+
+        except Exception as e:
+            self.logger.exception(e, exc_info=True)
+
+        finally:
+            self.conn.close()
+            return obj
+
+    def execute_query_(
+            self, query=None) -> None:
+
+        self.logger.info('call execute_query ')
+        self.get_conection()
+        obj = None  
+
+        try :
+            with self.conn.cursor() as cur:
+
+                cur.execute(query)
+                colnames = [desc[0] for desc in cur.description]
+
+                obj = cur.fetchall()
+
+        except Exception as e:
+            self.logger.exception(e, exc_info=True)
+
+        finally:
+            self.conn.close()
+            return obj,colnames
+        
+
+    def get_subcategory_info_by_mappingCode(
+            self, clase_predict: int = None) -> None:
+
+        self.logger.info('call get_subcategory_info_by_mappingCode method ')
+        self.get_conection()
+        obj = None  
+
+        try :
+            with self.conn.cursor() as cur:
+
+                postgres_select_query = '''
+
+                            SELECT uid, name, keywords, category_uid, icon_uid
+                            FROM public.subcategory
+                            WHERE mapping_code=%(clase_predict)s;
+                            '''
+
+                param_select = {'clase_predict': clase_predict}
+                cur.execute(postgres_select_query, param_select)
+
+                obj = cur.fetchone()
+
+        except Exception as e:
+            self.logger.exception(e, exc_info=True)
+
+        finally:
+            self.conn.close()
+
+            if obj is None:
+                    self.logger.info(fmt('No found code subcategory: ',
+                                    json={'code : ': clase_predict}))
+                    return 0
+
+            else :
+                self.logger.info('done call get_subcategory_info_by_mappingCode')
+                return obj
+
+
+
     def get_subcategory_info_by_mappingCode(
             self, clase_predict: int = None) -> None:
 
         self.logger.info('call get_subcategory_info_by_mappingCode method ')
         self.get_conection()
         obj = None
```

### Comparing `klp-commons-0.0.9/klp_commons/controllers/controller_redshift.py` & `klp_commons-0.39/klp_commons/controllers/controller_redshift.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,19 @@
             raise TypeError('error  get_conection RedShift')
 
         self.logger.info(" Done get_conection() method of RedShift")
 
     def close_conection(self):          
         self.session.close() 
         self.engine.dispose()
-        
+
+    def execute_query(self,query=None):        
+
+        return read_sql_query(text(query),self.engine)    
+
     def insert_dim_user(self,dict_values):
         with self.engine.connect() as cur:
             redshift_insert_query = '''
                         INSERT INTO dim_user (user_uid,postcode)
                         VALUES (%s,%s)
                                     '''
             record_to_insert = (
@@ -300,15 +304,15 @@
             'category_custom_type' : dict_values['category_custom_type'],
             'category_uid_collective' : dict_values['category_uid_def_collect'],
             'category_uid_custom' : dict_values['category_uid_def_usr'],
             'category_uid_recommended' : dict_values['category_uid_def_algo'],
             'classified_date' : dict_values['classified_date'],
             'clean_description' : dict_values['clean_description'],
             'country_code' : dict_values['country_code'],
-            'created_holomogation_date' : dict_values['created_holomogation_date'],
+            'created_homologation_date' : dict_values['created_homologation_date'],
             'flow_type' : dict_values['flow_type'],
             'frequency_uid_collective' : dict_values['frequency_uid_def_collect'],
             'frequency_uid_custom' : dict_values['frequency_uid_def_usr'],
             'frequency_uid_recommended' : dict_values['frequency_uid_def_algo'],
             'income_source_uid_collective' : dict_values['income_source_uid_def_collect'],
             'income_source_uid_custom' : dict_values['income_source_uid_def_usr'],
             'income_source_uid_recommended' : dict_values['income_source_uid_def_algo'],
@@ -377,22 +381,23 @@
                         category_custom_type,
                         category_uid_collective,
                         category_uid_custom,
                         category_uid_recommended,
                         classified_date,
                         clean_description,
                         country_code,
-                        created_holomogation_date,
+                        created_homologation_date,
                         flow_type,
                         frequency_uid_collective,
                         frequency_uid_custom,
                         frequency_uid_recommended,
                         income_source_uid_collective,
                         income_source_uid_custom,
                         income_source_uid_recommended,
+                        is_autocategorized,
                         is_essential_collective,
                         is_essential_custom,
                         is_essential_recommended,
                         is_loan_received_collective,
                         is_loan_received_custom,
                         is_loan_received_recommended,
                         is_loan_requested_collective,
@@ -494,103 +499,222 @@
                                 %s,
                                 %s,
                                 %s,
                                 %s,
                                 %s,
                                 %s,
                                 %s,
+                                %s,
                                 %s
                                 )
                                     '''
             record_to_insert = (
-                            dict_values['approved_asset'],
-                            dict_values['approved_business'],
-                            dict_values['approved_category'],
-                            dict_values['approved_frequency'],
-                            dict_values['approved_income_source'],
-                            dict_values['approved_is_essential'],
-                            dict_values['approved_is_loan_received'],
-                            dict_values['approved_is_loan_requested'],
-                            dict_values['approved_is_membership'],
-                            dict_values['approved_nickname'],
-                            dict_values['approved_person'],
-                            dict_values['approved_special_moment'],
-                            dict_values['approved_subcategory'],
-                            dict_values['asset_uid_def_collect'],
-                            dict_values['asset_uid_def_usr'],
-                            dict_values['asset_uid_def_algo'],
-                            dict_values['business_uid_def_collect'],
-                            dict_values['business_uid_def_usr'],
-                            dict_values['business_uid_def_algo'],
-                            dict_values['category_custom_type'],
-                            dict_values['cat_uid_def_collect'],
-                            dict_values['cat_uid_def_usr'],
-                            dict_values['cat_uid_def_algo'],
-                            dict_values['classified_at'],
-                            dict_values['clean_description'],
-                            dict_values['country_code'],
-                            dict_values['created_at_homologation'],
-                            dict_values['flow_type'],
-                            dict_values['frequency_uid_def_collect'],
-                            dict_values['frequency_uid_def_usr'],
-                            dict_values['frequency_uid_def_algo'],
-                            dict_values['income_source_uid_def_collect'],
-                            dict_values['income_source_uid_def_usr'],
-                            dict_values['income_source_uid_def_algo'],
-                            dict_values['is_essential_def_collect'],
-                            dict_values['is_essential_def_usr'],
-                            dict_values['is_essential_def_algo'],
-                            dict_values['is_loan_received_def_collect'],
-                            dict_values['is_loan_received_def_usr'],
-                            dict_values['is_loan_received_def_algo'],
-                            dict_values['is_loan_requested_def_collect'],
-                            dict_values['is_loan_requested_def_usr'],
-                            dict_values['is_loan_requested_def_algo'],
-                            dict_values['is_membership_def_collect'],
-                            dict_values['is_membership_def_usr'],
-                            dict_values['is_membership_def_algo'],
-                            dict_values['language_code'],
-                            dict_values['message_type'],
-                            dict_values['model_classification_version'],
-                            dict_values['model_collective_version'],
-                            dict_values['model_nickname_version'],
-                            dict_values['model_nlp_version'],
-                            dict_values['nickname_collect'],
-                            dict_values['nickname_usr'],
-                            dict_values['nickname_algo'],
-                            dict_values['original_created_date'],
-                            dict_values['person_uid_def_collect'],
-                            dict_values['person_uid_def_usr'],
-                            dict_values['person_uid_def_algo'],
-                            dict_values['source_description'],
-                            dict_values['special_moment_uid_def_collect'],
-                            dict_values['special_moment_uid_def_usr'],
-                            dict_values['special_moment_uid_def_algo'],
-                            dict_values['subcategory_custom_type'],
-                            dict_values['subcat_uid_def_collect'],
-                            dict_values['subcat_uid_def_usr'],
-                            dict_values['subcat_uid_def_algo'],
-                            dict_values['transaction_uid'],
-                            dict_values['updated_at'],
-                            dict_values['validated'],
-                            dict_values['created_at']
+                                 dict_values['approved_asset'],
+                                dict_values['approved_business'],
+                                dict_values['approved_category'],
+                                dict_values['approved_frequency'],
+                                dict_values['approved_income_source'],
+                                dict_values['approved_is_essential'],
+                                dict_values['approved_is_loan_received'],
+                                dict_values['approved_is_loan_requested'],
+                                dict_values['approved_is_membership'],
+                                dict_values['approved_nickname'],
+                                dict_values['approved_person'],
+                                dict_values['approved_special_moment'],
+                                dict_values['approved_subcategory'],
+                                dict_values['asset_uid_def_collect'],
+                                dict_values['asset_uid_def_usr'],
+                                dict_values['asset_uid_def_algo'],
+                                dict_values['business_uid_def_collect'],
+                                dict_values['business_uid_def_usr'],
+                                dict_values['business_uid_def_algo'],
+                                dict_values['category_custom_type'],
+                                dict_values['cat_uid_def_collect'],
+                                dict_values['cat_uid_def_usr'],
+                                dict_values['cat_uid_def_algo'],
+                                dict_values['classified_at'],
+                                dict_values['clean_description'],
+                                dict_values['country_code'],
+                                dict_values['created_at_homologation'],
+                                dict_values['flow_type'],
+                                dict_values['frequency_uid_def_collect'],
+                                dict_values['frequency_uid_def_usr'],
+                                dict_values['frequency_uid_def_algo'],
+                                dict_values['income_source_uid_def_collect'],
+                                dict_values['income_source_uid_def_usr'],
+                                dict_values['income_source_uid_def_algo'],
+                                dict_values['is_autocategorized'],
+                                dict_values['is_essential_def_collect'],
+                                dict_values['is_essential_def_usr'],
+                                dict_values['is_essential_def_algo'],
+                                dict_values['is_loan_received_def_collect'],
+                                dict_values['is_loan_received_def_usr'],
+                                dict_values['is_loan_received_def_algo'],
+                                dict_values['is_loan_requested_def_collect'],
+                                dict_values['is_loan_requested_def_usr'],
+                                dict_values['is_loan_requested_def_algo'],
+                                dict_values['is_membership_def_collect'],
+                                dict_values['is_membership_def_usr'],
+                                dict_values['is_membership_def_algo'],
+                                dict_values['language_code'],
+                                dict_values['message_type'],
+                                dict_values['model_classification_version'],
+                                dict_values['model_collective_version'],
+                                dict_values['model_nickname_version'],
+                                dict_values['model_nlp_version'],
+                                dict_values['nickname_collect'],
+                                dict_values['nickname_usr'],
+                                dict_values['nickname_algo'],
+                                dict_values['original_created_date'],
+                                dict_values['person_uid_def_collect'],
+                                dict_values['person_uid_def_usr'],
+                                dict_values['person_uid_def_algo'],
+                                dict_values['source_description'],
+                                dict_values['special_moment_uid_def_collect'],
+                                dict_values['special_moment_uid_def_usr'],
+                                dict_values['special_moment_uid_def_algo'],
+                                dict_values['subcategory_custom_type'],
+                                dict_values['subcat_uid_def_collect'],
+                                dict_values['subcat_uid_def_usr'],
+                                dict_values['subcat_uid_def_algo'],
+                                dict_values['transaction_uid'],
+                                dict_values['updated_at'],
+                                dict_values['validated'],
+                                dict_values['created_at']                               
+                                                       )
+            cur.execute(redshift_insert_query, record_to_insert)
+
+    def insert_dim_visualization(self,dict_values):
+        with self.engine.connect() as cur:
+            redshift_insert_query = '''
+                        INSERT INTO dim_visualization (
+                                asset_uid,
+                                business_uid,
+                                category_uid,
+                                classified_date,
+                                clean_description,
+                                country_code,
+                                created_homologation_date,
+                                description,
+                                flow_type,
+                                frequency_uid,
+                                is_autocategorized,
+                                income_source_uid,
+                                is_essential,
+                                is_loan_received,
+                                is_loan_requested,
+                                is_membership,
+                                language_code,
+                                message_type,
+                                original_created_date,
+                                person_uid,
+                                source_description,
+                                special_moment_uid,
+                                subcategory_uid,
+                                transaction_uid,
+                                updated_date,
+                                validated,
+                                validated_date
+                                )
+                        VALUES (
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s,
+                                %s
+                                )
+                                    '''
+            record_to_insert = (
+                        dict_values['asset_uid'],
+                        dict_values['business_uid'],
+                        dict_values['category_uid'],
+                        dict_values['classified_at'],
+                        dict_values['clean_description'],
+                        dict_values['country_code'],
+                        dict_values['created_at_homologation'],
+                        dict_values['description'],
+                        dict_values['flow_type'],
+                        dict_values['frequency_uid'],
+                        dict_values['is_autocategorized'],
+                        dict_values['income_source_uid'],
+                        dict_values['is_essential'],
+                        dict_values['is_loan_received'],
+                        dict_values['is_loan_requested'],
+                        dict_values['is_membership'],
+                        dict_values['language_code'],
+                        dict_values['message_type'],
+                        dict_values['original_created_date'],
+                        dict_values['person_uid'],
+                        dict_values['source_description'],
+                        dict_values['special_moment_uid'],
+                        dict_values['subcategory_uid'],
+                        dict_values['transaction_uid'],
+                        dict_values['updated_at'],
+                        dict_values['validated'],
+                        dict_values['created_at']
+
                             )
             cur.execute(redshift_insert_query, record_to_insert)
-            
+
     def insert_fact_transactions(self,dict_values):
         with self.engine.connect() as cur:
             redshift_insert_query = '''
                         INSERT INTO fact_transactions (
                                                 transaction_date,
                                                 transaction_uid,
                                                 user_uid,
                                                 account_uid,
                                                 amount,
                                                 currency
                                                 )
+                        VALUES (%s,%s,%s,%s,%s,%s)
+                                    '''
+            record_to_insert = (
+                        dict_values['transaction_date'],
+                        dict_values['transaction_uid'],
+                        dict_values['user_uid'],
+                        dict_values['account_uid'],
+                        dict_values['amount'],
+                        dict_values['currency']
+                                )
+            cur.execute(redshift_insert_query, record_to_insert)
+
+    def insert_fact_visualization(self,dict_values):
+        with self.engine.connect() as cur:
+            redshift_insert_query = '''
+                        INSERT INTO fact_visualization (
+                                                transaction_date,
+                                                transaction_uid,
+                                                user_uid,
+                                                account_uid,
+                                                amount,
+                                                currency
+                                                )
                         VALUES (%s,%s,%s,%s,%s,%s)
                                     '''
             record_to_insert = (
                         dict_values['transaction_date'],
                         dict_values['transaction_uid'],
                         dict_values['user_uid'],
                         dict_values['account_uid'],
```

### Comparing `klp-commons-0.0.9/klp_commons/cryptools/.DS_Store` & `klp_commons-0.39/klp_commons/cryptools/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/cryptools/cryptology.py` & `klp_commons-0.39/klp_commons/cryptools/cryptology.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/datadict/.DS_Store` & `klp_commons-0.39/klp_commons/datadict/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/datadict/struct_dicts.py` & `klp_commons-0.39/klp_commons/datadict/struct_dicts.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class TypeTransEnrichment:
     def __init__(self):
         self.NAME_SPACE_TRANS = {
             # delegar a MS-Report
             'user_uid': None,
             # delegar a MS-Report
             'transaction_uid': None,
-            'message-type' : None,
+            'message-type':None,
             'offset': None,
             'data': None,
             'dynamo': None
             }
 
     def get(self):
         return self.NAME_SPACE_TRANS
@@ -104,14 +104,16 @@
     """
     def __init__(self):
         self.ERROR_ = dict()
         self.ERROR_['type'] = 'transaction-process-error' 
         self.ERROR_['data'] = {}
         self.ERROR_['data']['institution'] = None
         self.ERROR_['data']['user_uid'] = None
+        self.ERROR_['data']['offset'] = None
+
     def get(self):
         return self.ERROR_
 
 class Error:
     """
     Mensaje de error enviado al type :'report-error-ms-categorization'
     lo utiliza reporting (MS monitoring) para almacenar en Mongo los 
@@ -222,20 +224,20 @@
             "asset_uid": None,  # 
             "business_uid": None, #
             "person_uid": None, # ID de la persona asociada a la transacción
             "special_moment_uid": None, # ID de el momento especial asociado a la transacción
             "frequency_uid": None, # ID de la frecuencia asociada a la transacción
             "is_essential": None, # True| False  si el gasto es escencial
             "is_membership": None, # True| False si el gasto pertence a un menbresía
-            "income_source_uid" : None,
-            "is_loan_received" : None,
+            "income_source_uid":None,
+            "is_loan_received":None,
             "is_loan_requested": None,
-            "collective_subcategory_uid" : None,
-            "collective_description" : None,
-            "collective_is_essential" : None,
+            "collective_subcategory_uid":None,
+            "collective_description":None,
+            "collective_is_essential":None,
             "collective_is_membership" : None
 			}
 
     def get(self):
         return self.Item
 
 class Message:
@@ -263,155 +265,159 @@
 # RedShift DataWare House
 class DimTransactions:
     """
     For RedShift Dimension Transactions
     """
     def __init__(self) -> None:
         self.Item = {
-        "transaction_uid": None,
-        "language_code": None,
-        "country_code": None,
-        "flow_type": None,
-        "message_type": None,
-        "validated": None,
-        "source_description": None,
-        "clean_description": None,
-        "model_nlp_version": None,
-        "model_classification_version": None,
-        "model_nickname_version": None,
-        "model_collective_version": None,
-        "approved_asset": None,
-        "approved_business": None,
-        "approved_category": None,
-        "approved_frequency": None,
-        "approved_is_essential": None,
-        "approved_is_membership": None,
-        "approved_nickname": None,
-        "approved_person": None,
-        "approved_special_moment": None,
-        "approved_subcategory": None,
-        "approved_is_loan_received": None,
-        "approved_is_loan_requested": None,
-        "approved_income_source": None,
-        "is_loan_requested_recommended": None,
-        "is_membership_recommended": None,
-        "subcategory_uid_recommended": None,
-        "category_uid_recommended": None,
-        "special_moment_uid_recommended": None,
-        "is_essential_recommended": None,
-        "frequency_uid_recommended": None,
-        "asset_uid_recommended": None,
-        "person_uid_recommended": None,
-        "business_uid_recommended": None,
-        "income_source_uid_recommended": None,
-        "is_loan_received_recommended": None,
-        "nickname_recommended": None,
-        "subcategory_custom_type": None,
-        "category_custom_type": None,
-        "is_essential_custom": None,
-        "is_membership_custom": None,
-        "person_uid_custom": None,
-        "is_loan_requested_custom": None,
-        "special_moment_uid_custom": None,
-        "business_uid_custom": None,
-        "asset_uid_custom": None,
-        "subcategory_uid_custom": None,
-        "frequency_uid_custom": None,
-        "category_uid_custom": None,
-        "income_source_uid_custom": None,
-        "is_loan_received_custom": None,
-        "nickname_custom": None,
-        "category_uid_collective": None,
-        "subcategory_uid_collective": None,
-        "nickname_collective": None,
-        "income_source_uid_collective": None,
-        "is_loan_requested_collective": None,
-        "is_essential_collective": None,
-        "is_membership_collective": None,
-        "frequency_uid_collective": None,
-        "is_loan_received_collective": None,
-        "person_uid_collective": None,
-        "asset_uid_collective": None,
-        "business_uid_collective": None,
-        "special_moment_uid_collective": None,
-        "original_created_date": None,
-        "created_holomogation_date": None,
-        "classified_date": None,
-        "validated_date": None,
-        "updated_date": None,
-        "created_at": None,
-        "updated_at": None,
-        "deleted_at": None
+            "approved_asset": None,
+            "approved_business": None,
+            "approved_category": None,
+            "approved_frequency": None,
+            "approved_income_source": None,
+            "approved_is_essential": None,
+            "approved_is_loan_received": None,
+            "approved_is_loan_requested": None,
+            "approved_is_membership": None,
+            "approved_nickname": None,
+            "approved_person": None,
+            "approved_special_moment": None,
+            "approved_subcategory": None,
+            "asset_uid_collective": None,
+            "asset_uid_custom": None,
+            "asset_uid_recommended": None,
+            "business_uid_collective": None,
+            "business_uid_custom": None,
+            "business_uid_recommended": None,
+            "category_custom_type": None,
+            "category_uid_collective": None,
+            "category_uid_custom": None,
+            "category_uid_recommended": None,
+            "classified_date": None,
+            "clean_description": None,
+            "country_code": None,
+            "created_at": None,
+            "created_homologation_date": None,
+            "deleted_at": None,
+            "flow_type": None,
+            "frequency_uid_collective": None,
+            "frequency_uid_custom": None,
+            "frequency_uid_recommended": None,
+            "income_source_uid_collective": None,
+            "income_source_uid_custom": None,
+            "income_source_uid_recommended": None,
+            'is_autocategorized':None,
+            "is_essential_collective": None,
+            "is_essential_custom": None,
+            "is_essential_recommended": None,
+            "is_loan_received_collective": None,
+            "is_loan_received_custom": None,
+            "is_loan_received_recommended": None,
+            "is_loan_requested_collective": None,
+            "is_loan_requested_custom": None,
+            "is_loan_requested_recommended": None,
+            "is_membership_collective": None,
+            "is_membership_custom": None,
+            "is_membership_recommended": None,
+            "language_code": None,
+            "message_type": None,
+            "model_classification_version": None,
+            "model_collective_version": None,
+            "model_nickname_version": None,
+            "model_nlp_version": None,
+            "nickname_collective": None,
+            "nickname_custom": None,
+            "nickname_recommended": None,
+            "original_created_date": None,
+            "person_uid_collective": None,
+            "person_uid_custom": None,
+            "person_uid_recommended": None,
+            "source_description": None,
+            "special_moment_uid_collective": None,
+            "special_moment_uid_custom": None,
+            "special_moment_uid_recommended": None,
+            "subcategory_custom_type": None,
+            "subcategory_uid_collective": None,
+            "subcategory_uid_custom": None,
+            "subcategory_uid_recommended": None,
+            "transaction_uid": None,
+            "updated_at": None,
+            "updated_date": None,
+            "validated": None,
+            "validated_date": None
             }
     def get(self):
         return self.Item
 
 class DimAccount:
     """
     """
     def __init__(self) -> None:
         self.Item = {
-    "account_uid" : None,
-    "bank_name" : None,
-    "account_type" : None,
-    "bank_type" : None,
-    "created_at" : None,
-    "updated_at" : None,
+    "account_uid":None,
+    "bank_name":None,
+    "account_type":None,
+    "bank_type":None,
+    "created_at":None,
+    "updated_at":None,
     "deleted_at" : None
     }
     def get(self):
         return self.Item
 
+# fix
 class DimUser:
     """
     """
     def __init__(self) -> None:
         self.Item = {
-    "user_uid" : None,
-    # "postcode" : None,
-    # "created_at" : None,
-    # "updated_at" : None,
+    "user_uid":None,
+    # "postcode":None,
+    # "created_at":None,
+    # "updated_at":None,
     # "deleted_at" : None
     }
     def get(self):
         return self.Item
     
 class DimDates:
     """
     """
     def __init__(self) -> None:
         self.Item = {
-    "transaction_date" : None,# validated or updated
-    "day_of_month" : None,
-    "month_of_year" : None,
-    "month_name"  : None,
-    "year" : None,
-    "week_of_month" : None,
-    "quarter_of_year" : None,
-    # "created_at" : None,
-    # "updated_at" : None,
+    "transaction_date":None,# validated or updated
+    "day_of_month":None,
+    "month_of_year":None,
+    "month_name": None,
+    "year":None,
+    "week_of_month":None,
+    "quarter_of_year":None,
+    # "created_at":None,
+    # "updated_at":None,
     # "deleted_at" : None
     }
     def get(self):
         return self.Item
 
+# fix
 class FactTransactions:
 
     def __init__(self) -> None:
         
         self.Item = {
             "transaction_date": None,
             "transaction_uid": None,
             "user_uid": None,
             "account_uid": None
         }
 
     def get(self):
         return self.Item
 
+
 # MongoDB History Facts
 class TransactionFact:
     """
     For mongoDB 
     """
     def __init__(self) -> None:
         self.Item = {
@@ -462,16 +468,16 @@
             "asset_uid": None,  # 
             "business_uid": None, #
             "person_uid": None, # ID de la persona asociada a la transacción
             "special_moment_uid": None, # ID de el momento especial asociado a la transacción
             "frequency_uid": None, # ID de la frecuencia asociada a la transacción
             "is_essential": None, # True| False  si el gasto es escencial
             "is_membership": None, # True| False si el gasto pertence a un menbresía
-            "income_source_uid" : None,
-            "is_loan_received" : None,
+            "income_source_uid":None,
+            "is_loan_received":None,
             "is_loan_requested": None,
             "status": None,
             "categorized": None,
             "replica_type": None,
             "message_type": None,
             "classified_at": None,
             "model_nlp_version": None,
@@ -503,15 +509,14 @@
         {
       
         }
 
         }
     def get(self):
         return self.Item
-
 # DynamoDB
 class DetailsUser:
     """
     Objeto  DetailsUser, el cual es un objeto anidado del super Objeto ItemUser
     """
 
     def __init__(self) -> None:
@@ -565,18 +570,20 @@
         "is_loan_received_def_usr": None,
         "is_loan_received_def_collect": None,
 
         "is_loan_requested_def_algo": None,
         "is_loan_requested_def_usr": None,
         "is_loan_requested_def_collect": None,
 
-        "created_at": None,# type:expense-created
-        "updated_at": None,# type:expense-updated
+        "created_at": None,#  None for transactio-categorized, type:expense-created
+        "updated_at": None,#  None for transactio-categorized, type:expense-updated
         
-        "message_type": None,
+        "is_autocategorized":None, # categorización automática
+
+        "message_type": None, # None for transactio-categorized, save expense/income created/updated
         "clean_description": None,
         "merchant_name": None,
         "classified_at": None, # type:transaction-categorized
         "source_embedding": None,
         "kw_group":None
 
         }
@@ -675,17 +682,16 @@
         self.Item = {
             'user_uid': None,
             'transaction_uid': None,
             'hash': None
                     }
     def get(self):
         return self.Item
-
-# Diccionarios
-class Transaction_:
+# Dims Diccionarios
+class Transaction_Map_DWH:
 
     def __init__(self) -> None:
 
         self.Item = {
             'approved_asset': None,
             'approved_business': None,
             'approved_category': None,
@@ -717,14 +723,15 @@
             'flow_type': None,
             'frequency_uid_def_collect': None,
             'frequency_uid_def_algo': None,
             'frequency_uid_def_usr': None,
             'income_source_uid_def_collect': None,
             'income_source_uid_def_algo': None,
             'income_source_uid_def_usr': None,
+            'is_autocategorized':None,
             'is_essential_def_collect': None,
             'is_essential_def_algo': None,
             'is_essential_def_usr': None,
             'is_loan_received_def_collect': None,
             'is_loan_received_def_algo': None,
             'is_loan_received_def_usr': None,
             'is_loan_requested_def_collect': None,
@@ -756,8 +763,48 @@
             'subcat_uid_def_algo': None,
             'updated_at': None,
             'validated': None,
             'transaction_uid': None,
             }
     
     def get(self):
-        return self.Item
+        return self.Item
+    
+class Visualization_Map_DWH:
+
+    def __init__(self) -> None:
+
+        self.Item = {
+        'asset_uid': None,
+        'business_uid':None,
+        'category_uid': None,
+        'classified_at': None,
+        'clean_description':None,
+        'country_code': None,
+        'created_at': None, #validate ()
+        'created_at_homologation': None,
+        'description': None,
+        'flow_type':None,
+        'frequency_uid': None,
+        'income_source_uid': None,
+        'is_autocategorized':None,
+        'is_essential':None,
+        'is_loan_received': None,
+        'is_loan_requested': None,
+        'is_membership':None,
+        'language_code':None,
+        'message_type': None,
+        'original_created_date':None,
+        'person_uid': None,
+        'source_description': None,
+        'special_moment_uid': None,
+        'subcategory_uid': None,
+        'transaction_uid':None,
+        'updated_at': None, #update expense or income 
+        'validated':None,
+        }
+    
+    def get(self):
+        return self.Item
+
+
+
```

### Comparing `klp-commons-0.0.9/klp_commons/datefinder/__init__.py` & `klp_commons-0.39/klp_commons/datefinder/__init__.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/datefinder/constants.py` & `klp_commons-0.39/klp_commons/datefinder/constants.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/datefinder/date_fragment.py` & `klp_commons-0.39/klp_commons/datefinder/date_fragment.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/log/.DS_Store` & `klp_commons-0.39/klp_commons/log/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/log/log.py` & `klp_commons-0.39/klp_commons/log/log.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/scripts/.DS_Store` & `klp_commons-0.39/klp_commons/scripts/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/scripts/detect_recurrency.py` & `klp_commons-0.39/klp_commons/scripts/detect_recurrency.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/scripts/get_send_kw_group.py` & `klp_commons-0.39/klp_commons/scripts/get_send_kw_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,16 @@
     for message in islice(consumer, last_num_messages):
         print("offset: ",message.offset)
         current_offset = message.offset
         message = json.loads(message.value)
         if message['type'] ==  'transaction-categorized':
             message_categorized_count += 1
             for transaction in message['data']['transactions']:
-                list_content_messages.append({'uid':transaction['uid'],'kw_group':transaction['categorization']['kw_group']})
+                pass
+                # list_content_messages.append({'uid':transaction['uid'],'kw_group':transaction['categorization']['kw_group']})
 
         message_count += 1
         list_type_messages.append(message["type"])
         
         if message_count == last_num_messages :
             break
 
@@ -145,36 +146,32 @@
     api_version = (2,6,1)
     group_id  = 'categorization-'
     topic_set = 'transaction'
 
     topics_get = ['transaction']
     message_type = 'transaction-update-kw-group'
     earliest_available_offsets,latest_offsets = get_offset_latest(topics_get,kafka_brokers)
-    message_struct = {'data':{
-                            'transactions':None
-                            },
-                   'type': 'transaction-update-kw-group'
-                  }
 
 
 
 
     print(earliest_available_offsets )
     print(latest_offsets)
 
     
     for topic in topics_get :
         print("topic: ", topic)
         last_num_messages = latest_offsets[topic] - earliest_available_offsets[topic]
         print("last_num_messages: ", last_num_messages)
-        _,list_content_messages = get_send_messages(topic,last_num_messages,kafka_brokers)
+        list_type_messages,list_content_messages = get_send_messages(topic,last_num_messages,kafka_brokers)
 
         
-        print("Número de transacciones: ",len(list_content_messages))
+        print("list_type_messages: ",list_type_messages)
 
+    """ 
         # d_unique = pd.DataFrame(d).drop_duplicates().to_dict('records')
         set_of_jsons = {json.dumps(d, sort_keys=True) for d in list_content_messages}
         list_content_messages = [json.loads(t) for t in set_of_jsons]
         
         print("Remover duplicados... \nNúmero de transacciones: ",len(list_content_messages))
         
         message_struct['data']['transactions'] = list_content_messages
@@ -193,7 +190,8 @@
         api_version = (2,6,1)
         group_id  = 'categorization-update-kw-group'
         client_id = None
         ProdTrans = Producer('transaction', kafka_brokers, acks, api_version , client_id)
         ProdTrans.init_producer()
         ProdTrans.send_message(message_struct)
         print(message_struct)
+    """
```

### Comparing `klp-commons-0.0.9/klp_commons/scripts/ingest_dwh.py` & `klp_commons-0.39/klp_commons/scripts/ingest_dwh.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,39 +25,47 @@
 PGDB = ControllerPostgresDB()
 RedShift = ControllerRedShift()
 
 MongoDB.get_con_collect(collection_name='fact')
 
 
 def get_info_by_transaction_uid(transaction_uid):
+
     MongoDB.get_con_collect(collection_name='analytic')
     
     responde_transaction = MongoDB.con_db.find_one({'_id': transaction_uid})
 
     if not responde_transaction:
         responde_transaction = MongoDB.con_db.find_one({"history-track.USER.transaction_uid": transaction_uid})
-
     
     if responde_transaction is None :
         return 
 
     reponse = dict()
     reponse['account_uid'] =responde_transaction['history-track'][0]['USER']['account_uid']
+
+    if not 'raw' in responde_transaction['history-track'][0]['USER']:
+        print("No raw")
+        return None
+    
+    if not 'amount' in responde_transaction['history-track'][0]['USER']['raw']:
+        print("responde_transaction: ", responde_transaction)
+        print("---------------------------______________________________-----------------")
+        return None
+
     reponse['amount'] =responde_transaction['history-track'][0]['USER']['raw']['amount']
     reponse['currency'] =responde_transaction['history-track'][0]['USER']['raw']['currency']
     reponse['bank_name'] =responde_transaction['history-track'][0]['USER']['raw']['account']['institution']['name']
     reponse['account_type'] =responde_transaction['history-track'][0]['USER']['raw']['account']['type']
     reponse['bank_type'] =responde_transaction['history-track'][0]['USER']['raw']['account']['institution']['type']
+    
     if 'message_type' in responde_transaction['history-track'][0]['CASE']:
         reponse['message_type'] =responde_transaction['history-track'][0]['CASE']['message_type']
-
-
-    print(reponse)
-
-    
+    else :
+        reponse['message_type'] = 'transaction-categorized'
 
     # ['raw']['account']['name']
     # ['raw']['account']['number']
     # ['raw']['account']['id']
     # ['raw']['account']['category']
     
     reponse['collected_at'] =responde_transaction['history-track'][0]['USER']['raw']['collected_at']
@@ -247,15 +255,15 @@
 
 today = date.today()
 front_date = today.strftime("%Y-%m-%d")
 
 print(today)
 print("front_date: " , front_date)
 
-s = Summary(front_date,num_days = 75)
+s = Summary(front_date,num_days = 250)
 r = s.agg_master()
 
 
 def refill():
     r['business_uid_def_usr'] = r['business_uid_def_usr'].apply(lambda x: x) + r['business_uid_def_usr_'].apply(lambda x: x) + r['business_uid_def_usr_info'].apply(lambda x: x)
 
     del r['business_uid_def_usr_']
@@ -308,98 +316,69 @@
 
 
 for col in sorted(r.columns.tolist()):
     r[col] = r.explode(col).reset_index()[col]
 
     
 #r[cols].set_index(['nickname_def_usr','category_uid_def_algo']).apply(pd.Series.explode).reset_index()
-# .sort_values(by=['created_at_head'], ascending = False)
-print("shape: ", r.shape)
 
 r.replace(np.nan, None, inplace=True)
 r.replace(pd.NaT, None, inplace=True)
 tmp = {'created_at_homologation': pd.NaT}
 
-
-
 for idx ,item in enumerate(r.to_dict(orient='records')):
-    print(idx, "user_uid:",item['user_uid'],"\n transaction_uid:",item['transaction_uid'])
-    print("... ")
     if 'classification_datetime' in item:
         item['classified_at'] = item['classification_datetime']
 
     if not item['lang_code']:
         item['language_code'] = 'es-MX'
     else :
         item['language_code'] = 'es-MX'
     
-    
     response = get_info_by_transaction_uid(item['transaction_uid'])
     
     if response is None :
         continue 
-    
-    print(response)
+
     # Dict to necessary data
     transaction_dict = Transaction_().get()
     transaction_dict.update(item)
     
     transaction_dict.update(response)
 
-    
-    
-    
-    if not 'message_type' in response:
-        if transaction_dict['message_type_head'] is not None:
-            transaction_dict['message_type'] = transaction_dict['message_type_head'] 
-        elif transaction_dict['message_type_history']  is not None:
-            transaction_dict['message_type'] = transaction_dict['message_type_history'] 
-        elif transaction_dict['message_type_old']  is not None:
-            transaction_dict['message_type'] = transaction_dict['message_type_old']
-        else: 
-            transaction_dict['message_type'] = 'ingest'
-    
-    
-
-
     if transaction_dict['clean_description'] is None:
         transaction_dict['clean_description'] = ''
 
-
-
     if transaction_dict['model_classification_version'] is None:
         transaction_dict['model_classification_version'] = 'bf24e9bff6ac4750b1daab8cd57f396d'
 
     if transaction_dict['model_nickname_version'] is None :
         transaction_dict['model_nickname_version'] = 'cM8zVveZ8bnlx4fuBLPH0gJZDh1wem_d0GBAv3f7'
 
     if transaction_dict['model_nlp_version'] is None:
         transaction_dict['model_nlp_version'] = '0grVmHxHgmD8-ad2pz9-HiNE1gKN_htomj5ktzSj'
 
     if transaction_dict['model_collective_version'] is None:
         transaction_dict['model_collective_version'] = '7Sdt1KJFB4DVVV4kqnSO5AEMVJF66q9ASUAAJG'
 
-        
     format_inter = '%Y-%m-%dT%H:%M:%S'
     
-    
     if not transaction_dict['created_at_homologation'] or transaction_dict['created_at_homologation'] is pd.NaT:
         transaction_dict['created_at_homologation'] = datetime.strptime('2023-01-01T00:00:00',format_inter).replace(microsecond=0).isoformat()
         
     if not transaction_dict['classified_at']:
         transaction_dict['classified_at'] = datetime.strptime('2023-01-01T00:00:00',format_inter).replace(microsecond=0).isoformat()
 
     if not transaction_dict['updated_at']:
         transaction_dict['updated_at'] = datetime.strptime('2023-01-01T00:00:00',format_inter).replace(microsecond=0).isoformat()
         
         
     if not transaction_dict['created_at']:
         transaction_dict['created_at'] = datetime.strptime('2023-01-01T00:00:00',format_inter).replace(microsecond=0).isoformat()
         
-
     keys = Transaction_().get().keys()
 
     rm_list = list()
     for key in transaction_dict.keys():
         if not key in keys:
             #print("No key : ", key)
             rm_list.append(key)
@@ -426,48 +405,28 @@
                     'account_uid': response['account_uid'],
                     'bank_name':  response['bank_name'],
                     'account_type': response['account_type'],
                     'bank_type': response['bank_type']
                     }
     
         RedShift.insert_dim_account(dict_values = account_dict)
-    
-    print("****************************************\n")
-    print(account_dict)
-    print("****************************************\n")
-    print(user_dict)
-    print("****************************************\n")
-    print(transaction_dict)
-    print("****************************************\n")
 
-
-    date_dict = RedShift.date_decomposition(str(item['created_at_head']).replace(" ","T").split(".")[0])
+    date_dict = RedShift.date_descomposition(str(response['collected_at']).replace(" ","T").split(".")[0])
     table_name = 'dim_dates'
     column_name = 'transaction_date'
 
     if not RedShift.exists(table_name,column_name ,value = str(date_dict['transaction_date']) ):
         RedShift.insert_dim_dates(dict_values = date_dict)
 
-
     fact_transactions_dict = dict ()
     fact_transactions_dict['transaction_date'] = str(date_dict['transaction_date'])
     fact_transactions_dict['transaction_uid'] = item['transaction_uid']
     fact_transactions_dict['user_uid'] = item['user_uid']
     fact_transactions_dict['account_uid'] = response['account_uid']
     fact_transactions_dict['amount'] = response['amount']
     fact_transactions_dict['currency'] = response['currency']
 
-
- 
-    print("\n\nfact_transactions_dict: ")
-    print(fact_transactions_dict)
-    print("----------------------------------------------")
-
     # Validación o updated de una transacción 
     # poner la bandera de Categorización automática
     RedShift.insert_dim_transaction(dict_values = transaction_dict)
 
-    RedShift.insert_fact_transactions(dict_values = fact_transactions_dict)
-    
-    print("+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++")
-    print("+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++")
-    
+    RedShift.insert_fact_transactions(dict_values = fact_transactions_dict)
```

### Comparing `klp-commons-0.0.9/klp_commons/scripts/summary.py` & `klp_commons-0.39/klp_commons/scripts/summary.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/streaming/.DS_Store` & `klp_commons-0.39/klp_commons/streaming/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/streaming/consumer.py` & `klp_commons-0.39/klp_commons/streaming/consumer.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/streaming/producer.py` & `klp_commons-0.39/klp_commons/streaming/producer.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/klp_commons/utils/.DS_Store` & `klp_commons-0.39/klp_commons/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.9/PKG-INFO` & `klp_commons-0.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klp-commons
-Version: 0.0.9
+Version: 0.39
 Summary: Modulo Commons del ecosistema Kloop. Contiene los modulos de uso común para los paquetes 
 Author-email: Omar Santa Cruz <omar.castellanos@kolpp.mx>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://gitlab.com/klopp1/backend/microservices/commons
 
 ## Commons
```

