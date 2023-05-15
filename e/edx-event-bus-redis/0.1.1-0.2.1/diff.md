# Comparing `tmp/edx_event_bus_redis-0.1.1.tar.gz` & `tmp/edx_event_bus_redis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_redis-0.1.1.tar", last modified: Fri May 12 13:15:22 2023, max compression
+gzip compressed data, was "edx_event_bus_redis-0.2.1.tar", last modified: Mon May 15 13:30:40 2023, max compression
```

## Comparing `edx_event_bus_redis-0.1.1.tar` & `edx_event_bus_redis-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8196 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6583 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    20908 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/message.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/producer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.525420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/templates/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8196 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8372 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6583 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.396540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20866 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/message.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/producer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.396540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis/templates/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8372 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-15 13:30:40.000000 edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-15 13:30:40.404540 edx_event_bus_redis-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 13:30:40.400540 edx_event_bus_redis-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-05-15 13:30:29.000000 edx_event_bus_redis-0.2.1/tests/test_models.py
```

### Comparing `edx_event_bus_redis-0.1.1/CHANGELOG.rst` & `edx_event_bus_redis-0.2.1/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.2.1] - 2023-05-12
+************************************************
+
+Changed
+=======
+* Deprecated ``signal`` argument in consumer (made optional in preparation for removal)
+
 [0.1.1] - 2023-05-12
 ************************************************
 
 Added
 =====
 
 * Option to claim messages from other consumers based on idle time.
```

### Comparing `edx_event_bus_redis-0.1.1/LICENSE.txt` & `edx_event_bus_redis-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.1/PKG-INFO` & `edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: edx_event_bus_redis
-Version: 0.1.1
+Name: edx-event-bus-redis
+Version: 0.2.1
 Summary: Redis Streams implementation for the Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-redis
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -236,14 +236,21 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.2.1] - 2023-05-12
+************************************************
+
+Changed
+=======
+* Deprecated ``signal`` argument in consumer (made optional in preparation for removal)
+
 [0.1.1] - 2023-05-12
 ************************************************
 
 Added
 =====
 
 * Option to claim messages from other consumers based on idle time.
```

### Comparing `edx_event_bus_redis-0.1.1/README.rst` & `edx_event_bus_redis-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/config.py` & `edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/consumer.py` & `edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,41 +75,40 @@
     requires_reconnect = has_connection and not connection.is_usable()
     if requires_reconnect:
         connection.connect()
 
 
 class RedisEventConsumer(EventBusConsumer):
     """
-    Construct consumer for the given topic, group, and signal. The consumer can then
-    emit events from the event bus using the configured signal.
+    Construct consumer for the given topic and group. The consumer can then
+    emit events coming from the topic.
 
     Note that the topic should be specified here *without* the optional environment prefix.
 
     Can also consume messages indefinitely off the queue.
 
     Attributes:
         topic: Topic/stream name.
         group_id: consumer group name.
-        signal: openedx_events signal.
+        signal: DEPRECATED, will be removed in a future release
         consumer_name: unique name for consumer within a group.
         last_read_msg_id: Start reading msgs from a specific redis msg id.
         check_backlog: flag to process all messages that were not read by this consumer group.
         claim_msgs_older_than: claim pending msgs from other consumers in the group with idle time older
             than a specific time (in milliseconds).
         has_pending_msgs: flag to process pending msgs first.
         db: Walrus object for redis connection.
         full_topic: topic prefixed with environment name.
         consumer: consumer instance.
     """
 
-    def __init__(self, topic, group_id, signal, consumer_name, last_read_msg_id=None, check_backlog=False,
-                 claim_msgs_older_than=None):
+    def __init__(self, topic, group_id, consumer_name, signal=None,  # pylint: disable=unused-argument
+                 last_read_msg_id=None, check_backlog=False, claim_msgs_older_than=None):
         self.topic = topic
         self.group_id = group_id
-        self.signal = signal
         self.consumer_name = consumer_name
         self.last_read_msg_id = last_read_msg_id
         self.check_backlog = check_backlog
         # always process read but pending msgs first for the consumer in the group.
         self.has_pending_msgs = True
         self.claim_msgs_older_than = claim_msgs_older_than
         self.db = self._create_db()
@@ -124,15 +123,15 @@
         config = load_common_settings()
         if config is None:
             raise ValueError("Missing redis connection url")
         return Database.from_url(config['url'])
 
     def _create_consumer(self, db: Database, full_topic: str) -> ConsumerGroupStream:
         """
-        Create a redis stream consumer group and a consumer for events of the given signal instance.
+        Create a redis stream consumer group and a consumer for the given topic
 
         Returns
             ConsumerGroupStream
         """
 
         # It is possible to track multiple streams using single consumer group.
         # But for simplicity, we are only supporting one stream till the need arises.
@@ -189,15 +188,14 @@
         #   include failure to poll, failure to decode events, or errors returned by signal handlers.
         #   This does not prevent committing of offsets back to the broker; any messages that caused an
         #   error will still be marked as consumed, and may need to be replayed.
         CONSECUTIVE_ERRORS_LIMIT = getattr(settings, 'EVENT_BUS_REDIS_CONSUMER_CONSECUTIVE_ERRORS_LIMIT', None)
         run_context = {
             'full_topic': self.full_topic,
             'consumer_group': self.group_id,
-            'expected_signal': self.signal,
             'consumer_name': self.consumer_name,
         }
 
         try:  # pylint: disable=too-many-nested-blocks
             logger.info(f"Running consumer for {run_context!r}")
 
             # How many errors have we seen in a row? If this climbs too high, exit with error.
@@ -230,15 +228,15 @@
                             self.claim_msgs_older_than = None
                     else:
                         # poll for msg
                         redis_raw_msg = self.consumer.read(count=1, block=CONSUMER_POLL_TIMEOUT * 1000)
                     if redis_raw_msg:
                         if isinstance(redis_raw_msg, list):
                             redis_raw_msg = redis_raw_msg[0]
-                        msg = RedisMessage.parse(redis_raw_msg, self.full_topic, expected_signal=self.signal)
+                        msg = RedisMessage.parse(redis_raw_msg, self.full_topic)
                         # Before processing, make sure our db connection is still active
                         _reconnect_to_db_if_needed()
                         self.emit_signals_from_message(msg)
                         consecutive_errors = 0
 
                     self._add_message_monitoring(run_context=run_context, message=msg)
                 except Exception as e:  # pylint: disable=broad-except
@@ -277,29 +275,30 @@
 
         signal = OpenEdxPublicSignal.get_signal_by_type(msg.event_metadata.event_type)
         event_data = deserialize_bytes_to_event_data(msg.event_data, signal)
         send_results = signal.send_event_with_custom_metadata(msg.event_metadata, **event_data)
         # Raise an exception if any receivers errored out. This allows logging of the receivers
         # along with partition, offset, etc. in record_event_consuming_error. Hopefully the
         # receiver code is idempotent and we can just replay any messages that were involved.
-        self._check_receiver_results(send_results)
+        self._check_receiver_results(send_results, signal)
 
         # At the very end, log that a message was processed successfully.
         # Since we're single-threaded, no other information is needed;
         # we just need the logger to spit this out with a timestamp.
         # See ADR: docs/decisions/0010_audit_logging.rst
         if AUDIT_LOGGING_ENABLED.is_enabled():
             logger.info('Message from Redis processed successfully')
 
-    def _check_receiver_results(self, send_results: list):
+    def _check_receiver_results(self, send_results: list, signal: OpenEdxPublicSignal):
         """
         Raises exception if any of the receivers produced an exception.
 
         Arguments:
             send_results: Output of ``send_events``, a list of ``(receiver, response)`` tuples.
+            signal: The signal used to send the events
         """
         error_descriptions = []
         errors = []
         for receiver, response in send_results:
             if not isinstance(response, BaseException):
                 continue
 
@@ -314,15 +313,15 @@
             error_descriptions.append(f"{receiver_name}={response!r}")
             errors.append(response)
 
         if len(error_descriptions) > 0:
             raise ReceiverError(
                 f"{len(error_descriptions)} receiver(s) out of {len(send_results)} "
                 "produced errors (stack trace elsewhere in logs) "
-                f"when handling signal {self.signal}: {', '.join(error_descriptions)}",
+                f"when handling signal {signal}: {', '.join(error_descriptions)}",
                 errors
             )
 
     def _log_message_received(self, msg: RedisMessage):
         """
         Log that a message was received, for audit log purposes.
 
@@ -352,15 +351,15 @@
 
     def record_event_consuming_error(self, run_context, error, maybe_message):
         """
         Record an error caught while consuming an event, both to the logs and to telemetry.
 
         Arguments:
             run_context: Dictionary of contextual information: full_topic, consumer_group,
-              and expected_signal.
+              and consumer_name.
             error: An exception instance
             maybe_message: None if event could not be fetched or decoded, or a Redis Message if
               one was successfully deserialized but could not be processed for some reason
         """
         context_msg = ", ".join(f"{k}={v!r}" for k, v in run_context.items())
         # Pulls the event message off the error for certain exceptions.
         if maybe_message is None:
@@ -381,15 +380,14 @@
 
     def _add_message_monitoring(self, run_context, message, error=None):
         """
         Record additional details for monitoring.
 
         Arguments:
             run_context: Dictionary of contextual information: full_topic, consumer_group,
-              and expected_signal.
             message: None if event could not be fetched or decoded, or a Message if one
               was successfully deserialized but could not be processed for some reason
             error: (Optional) An exception instance, or None if no error.
         """
         try:
             fatal = self._is_fatal_redis_error(error=error)
```

### Comparing `edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/producer.py` & `edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/utils.py` & `edx_event_bus_redis-0.2.1/edx_event_bus_redis/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/commands/produce_event.py` & `edx_event_bus_redis-0.2.1/edx_event_bus_redis/management/commands/produce_event.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html` & `edx_event_bus_redis-0.2.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/PKG-INFO` & `edx_event_bus_redis-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: edx-event-bus-redis
-Version: 0.1.1
+Name: edx_event_bus_redis
+Version: 0.2.1
 Summary: Redis Streams implementation for the Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-redis
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -236,14 +236,21 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.2.1] - 2023-05-12
+************************************************
+
+Changed
+=======
+* Deprecated ``signal`` argument in consumer (made optional in preparation for removal)
+
 [0.1.1] - 2023-05-12
 ************************************************
 
 Added
 =====
 
 * Option to claim messages from other consumers based on idle time.
```

### Comparing `edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/SOURCES.txt` & `edx_event_bus_redis-0.2.1/edx_event_bus_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.1/requirements/constraints.txt` & `edx_event_bus_redis-0.2.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.1/setup.py` & `edx_event_bus_redis-0.2.1/setup.py`

 * *Files identical despite different names*

