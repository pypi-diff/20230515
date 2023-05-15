# Comparing `tmp/macrometa-source-postgres-0.0.46.tar.gz` & `tmp/macrometa-source-postgres-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.46.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-0.0.47.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.46.tar` & `macrometa-source-postgres-0.0.47.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-04-21 12:21:39.896312 macrometa-source-postgres-0.0.46/LICENSE
--rw-r--r--   0        0        0    35128 2023-04-21 12:21:39.896312 macrometa-source-postgres-0.0.46/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8580 2023-04-21 12:21:39.896312 macrometa-source-postgres-0.0.46/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-04-21 12:21:39.900313 macrometa-source-postgres-0.0.46/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-04-21 12:21:39.900313 macrometa-source-postgres-0.0.46/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-21 12:21:39.900313 macrometa-source-postgres-0.0.46/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     8974 2023-04-21 12:21:39.900313 macrometa-source-postgres-0.0.46/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    28921 2023-04-21 12:21:39.900313 macrometa-source-postgres-0.0.46/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3698 2023-04-21 12:21:39.900313 macrometa-source-postgres-0.0.46/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1512 2023-04-21 12:21:40.204316 macrometa-source-postgres-0.0.46/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.46/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.46/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/LICENSE
+-rw-r--r--   0        0        0    34891 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8580 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     8974 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    27687 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3698 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1512 2023-05-15 03:01:57.725279 macrometa-source-postgres-0.0.47/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.47/setup.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.47/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.46/LICENSE` & `macrometa-source-postgres-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.46/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-0.0.47/macrometa_source_postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,25 +205,23 @@
             ConfigProperty('ssl_client_key', 'SSL Client Key', ConfigAttributeType.FILE, False, False,
                            description='Specific client key in PEM string format.',
                            placeholder_value="my_client_key"),
             ConfigProperty('ssl_client_password', 'SSL Client Password', ConfigAttributeType.PASSWORD, False, False,
                            description='If the private key contained in the SSL Client Key is encrypted, users can provide a '
                                        'password or passphrase to decrypt the encrypted private keys.',
                            placeholder_value="my_client_password"),
-            ConfigProperty('logical_poll_total_seconds', 'Break at No Data Received (Seconds)',
-                           ConfigAttributeType.INT, False, False,
-                           description='Stop running when no data received from WAL after certain number of seconds.',
-                           default_value='10800'),
             ConfigProperty('break_at_end_lsn', 'Break at End LSN', ConfigAttributeType.BOOLEAN, False, False,
                            description='Stop running if the newly received LSN is after the max LSN that was initially'
                                        ' detected.',
                            default_value='false'),
-            ConfigProperty('max_run_seconds', 'Maximum Runtime (Seconds)', ConfigAttributeType.INT, False, False,
-                           description='Stop running after a specified amount of time.',
-                           default_value='43200'),
+            ConfigProperty('wal_sender_timeout', 'WAL Sender Timeout (milliseconds)', ConfigAttributeType.INT, False, False,
+                           description='Terminate replication connections that are inactive for longer than this amount of time.'
+                                       ' This is useful for the sending server to detect a standby crash or network outage.'
+                                       ' Unit is milliseconds. The default value is 3600000 ms.',
+                           default_value='3600000'),
             ConfigProperty('debug_lsn', 'Debug LSN', ConfigAttributeType.STRING, False, False,
                            description='If set to "true" then add _sdc_lsn property to the singer messages '
                                        'to debug postgres LSN position in the WAL stream.',
                            default_value='false'),
             ConfigProperty('itersize', 'Iterator Size', ConfigAttributeType.INT, False, False,
                            description='PG cursor size for FULL_TABLE.',
                            default_value='20000'),
@@ -260,17 +258,16 @@
                 'ssl': integration.get('ssl', False),
                 'ssl_root_ca_cert': integration.get('ssl_root_ca_cert'),
                 'ssl_client_certificate': integration.get('ssl_client_certificate'),
                 'ssl_client_key': integration.get('ssl_client_key'),
                 'ssl_client_password': integration.get('ssl_client_password'),
                 'tap_id': integration.get('tap_id'),
                 'debug_lsn': integration.get('debug_lsn') == 'true',
-                'max_run_seconds': integration.get('max_run_seconds', 43200),
+                'wal_sender_timeout': integration.get('wal_sender_timeout', 3600000),
                 'break_at_end_lsn': integration.get('break_at_end_lsn', True),
-                'logical_poll_total_seconds': float(integration.get('logical_poll_total_seconds', 0)),
                 'use_secondary': integration.get('use_secondary', False),
             }
         except KeyError as e:
             raise KeyError(f'Integration property `{e}` not found.') from e
 
 
 def do_discovery(conn_config):
@@ -731,17 +728,16 @@
         'ssl': args.config.get('ssl', False),
         'ssl_root_ca_cert': args.config.get('ssl_root_ca_cert'),
         'ssl_client_certificate': args.config.get('ssl_client_certificate'),
         'ssl_client_key': args.config.get('ssl_client_key'),
         'ssl_client_password': args.config.get('ssl_client_password'),
         'tap_id': args.config.get('tap_id'),
         'debug_lsn': args.config.get('debug_lsn') == 'true',
-        'max_run_seconds': args.config.get('max_run_seconds', 43200),
+        'wal_sender_timeout': args.config.get('wal_sender_timeout', 3600000),
         'break_at_end_lsn': args.config.get('break_at_end_lsn', True),
-        'logical_poll_total_seconds': float(args.config.get('logical_poll_total_seconds', 0)),
         'use_secondary': args.config.get('use_secondary', False),
     }
 
     if conn_config['use_secondary']:
         try:
             conn_config |= {
                 # Secondary Host and Port are mandatory to use secondary connection.
```

### Comparing `macrometa-source-postgres-0.0.46/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-0.0.47/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.46/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-0.0.47/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.46/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.46/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.46/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,36 +517,32 @@
     )
     start_lsn = lsn_committed
     lsn_to_flush = None
     time_extracted = utils.now()
     slot = locate_replication_slot(conn_info)
     lsn_last_processed = None
     lsn_currently_processing = None
-    lsn_received_timestamp = None
     lsn_processed_count = 0
-    start_run_timestamp = datetime.datetime.utcnow()
-    max_run_seconds = conn_info['max_run_seconds']
     break_at_end_lsn = conn_info['break_at_end_lsn']
-    logical_poll_total_seconds = conn_info.get('logical_poll_total_seconds', 10800)  # 3 hours
     poll_interval = 10
     poll_timestamp = None
+    wal_sender_timeout = conn_info.get('wal_sender_timeout', 3600000)  # default 3600000 ms, i.e. 1 hour
 
     # Send schema message for each logical replication stream
     for s in logical_streams:
         sync_common.send_schema_message(s, ['lsn'])
 
     # Determine PostgreSQL version
     version = get_pg_version(conn_info)
 
     conn = postgres.connect(conn_info, True, True)
     cur = conn.cursor()
 
     # Adjust session wal_sender_timeout for PostgreSQL 12 and newer versions.
     if version >= 120000:
-        wal_sender_timeout = 10800000  # 10800000ms = 3 hours
         LOGGER.info('Set the value of wal_sender_timeout session parameter to %i milliseconds.', wal_sender_timeout)
         cur.execute(f"SET SESSION wal_sender_timeout = {wal_sender_timeout}")
 
     # Start replication with logical replication stream
     try:
         LOGGER.info('Initiate streaming of Write-Ahead-Log (WAL) from %s up to %s using slot %s.',
                     int_to_lsn(start_lsn),
@@ -563,37 +559,18 @@
             }
         )
 
     except psycopg2.ProgrammingError as ex:
         raise Exception(f"Failed to initiate logical replication with the replication slot {ex}.") from ex
 
     # Initialize timestamp
-    lsn_received_timestamp = datetime.datetime.utcnow()
     poll_timestamp = datetime.datetime.utcnow()
 
     try:
         while True:
-            # Disconnect the replication connection if no data is received for the logical_poll_total_seconds duration.
-            # This timeout should be long enough to accommodate the largest single WAL payload
-            # to prevent unexpected timeouts.
-            poll_duration = (
-                datetime.datetime.utcnow()
-                - lsn_received_timestamp
-            ).total_seconds()
-            if poll_duration > logical_poll_total_seconds:
-                LOGGER.info('No data received during the past %i seconds of polling, stopping replication',
-                            poll_duration)
-                break
-
-            if datetime.datetime.utcnow() >= start_run_timestamp + datetime.timedelta(
-                seconds=max_run_seconds
-            ):
-                LOGGER.info('Encountered max_run_seconds limit of %i, stopping replication...', max_run_seconds)
-                break
-
             try:
                 msg = cur.read_message()
             except Exception as e:
                 LOGGER.error(e)
                 raise
 
             if msg:
@@ -621,15 +598,14 @@
                                 int_to_lsn(lsn_to_flush),
                                 int_to_lsn(lsn_to_flush))
                     cur.send_feedback(write_lsn=lsn_to_flush, flush_lsn=lsn_to_flush, reply=True, force=True)
 
                 elif int(msg.data_start) > lsn_currently_processing:
                     lsn_last_processed = lsn_currently_processing
                     lsn_currently_processing = msg.data_start
-                    lsn_received_timestamp = datetime.datetime.utcnow()
                     lsn_processed_count = lsn_processed_count + 1
                     if lsn_processed_count >= 10000:
                         LOGGER.debug('Bookmarks for all streams are being updated to LSN = %s (%s)',
                                      lsn_last_processed,
                                      int_to_lsn(lsn_last_processed))
                         for s in logical_streams:
                             state = singer.write_bookmark(state, s['tap_stream_id'], 'lsn', lsn_last_processed)
```

### Comparing `macrometa-source-postgres-0.0.46/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.46/pyproject.toml` & `macrometa-source-postgres-0.0.47/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.46'
+version='0.0.47'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-postgres-0.0.46/setup.py` & `macrometa-source-postgres-0.0.47/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.46',
+    'version': '0.0.47',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.46/PKG-INFO` & `macrometa-source-postgres-0.0.47/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.46
+Version: 0.0.47
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

