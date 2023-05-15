# Comparing `tmp/smpp_gateway-1.0.3.tar.gz` & `tmp/smpp_gateway-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpp_gateway-1.0.3.tar", max compression
+gzip compressed data, was "smpp_gateway-1.0.4.tar", max compression
```

## Comparing `smpp_gateway-1.0.3.tar` & `smpp_gateway-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1085 2022-12-20 18:05:14.950147 smpp_gateway-1.0.3/LICENSE
--rw-r--r--   0        0        0     1082 2022-12-20 18:05:14.950147 smpp_gateway-1.0.3/README.md
--rw-r--r--   0        0        0     1282 2022-12-20 18:05:14.950147 smpp_gateway-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       22 2022-12-20 18:05:14.950147 smpp_gateway-1.0.3/src/smpp_gateway/__init__.py
--rw-r--r--   0        0        0     2452 2022-12-20 18:05:14.950147 smpp_gateway-1.0.3/src/smpp_gateway/admin.py
--rw-r--r--   0        0        0      189 2022-12-20 18:05:14.950147 smpp_gateway-1.0.3/src/smpp_gateway/apps.py
--rw-r--r--   0        0        0     9543 2022-12-20 18:05:14.950147 smpp_gateway-1.0.3/src/smpp_gateway/client.py
--rw-r--r--   0        0        0      404 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/management/commands/listen_mo_messages.py
--rw-r--r--   0        0        0     1993 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/management/commands/smpp_client.py
--rw-r--r--   0        0        0     2975 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/migrations/0001_initial.py
--rw-r--r--   0        0        0     2303 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/migrations/0002_mtmessagestatus.py
--rw-r--r--   0        0        0     2173 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/migrations/0003_big_pks_and_help_texts.py
--rw-r--r--   0        0        0     5435 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/migrations/0004_translations.py
--rw-r--r--   0        0        0     3660 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/migrations/0005_alter_mtmessagestatus_command_status.py
--rw-r--r--   0        0        0        0 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/migrations/__init__.py
--rw-r--r--   0        0        0     4351 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/models.py
--rw-r--r--   0        0        0     1846 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/outgoing.py
--rw-r--r--   0        0        0     2616 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/queries.py
--rw-r--r--   0        0        0     1563 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/smpp.py
--rw-r--r--   0        0        0     2218 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/subscribers.py
--rw-r--r--   0        0        0     1894 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/src/smpp_gateway/utils.py
--rw-r--r--   0        0        0        0 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1697 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/tests/factories.py
--rw-r--r--   0        0        0      450 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/tests/settings.py
--rw-r--r--   0        0        0     3669 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/tests/test_client.py
--rw-r--r--   0        0        0     7435 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/tests/test_queries.py
--rw-r--r--   0        0        0       93 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/tests/test_smpp_gateway.py
--rw-r--r--   0        0        0     2633 2022-12-20 18:05:14.954147 smpp_gateway-1.0.3/tests/test_subscribers.py
--rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 smpp_gateway-1.0.3/setup.py
--rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 smpp_gateway-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-15 01:52:32.518883 smpp_gateway-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1082 2023-05-15 01:52:32.518883 smpp_gateway-1.0.4/README.md
+-rw-r--r--   0        0        0     1282 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/__init__.py
+-rw-r--r--   0        0        0     2452 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/admin.py
+-rw-r--r--   0        0        0      189 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/apps.py
+-rw-r--r--   0        0        0     9550 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/client.py
+-rw-r--r--   0        0        0      404 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/management/commands/listen_mo_messages.py
+-rw-r--r--   0        0        0     1993 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/management/commands/smpp_client.py
+-rw-r--r--   0        0        0     2975 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2303 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0002_mtmessagestatus.py
+-rw-r--r--   0        0        0     2173 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0003_big_pks_and_help_texts.py
+-rw-r--r--   0        0        0     5435 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0004_translations.py
+-rw-r--r--   0        0        0     3660 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0005_alter_mtmessagestatus_command_status.py
+-rw-r--r--   0        0        0        0 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/__init__.py
+-rw-r--r--   0        0        0     4351 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/models.py
+-rw-r--r--   0        0        0     1846 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/outgoing.py
+-rw-r--r--   0        0        0     2616 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/queries.py
+-rw-r--r--   0        0        0     1563 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/smpp.py
+-rw-r--r--   0        0        0     2218 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/subscribers.py
+-rw-r--r--   0        0        0     1894 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1697 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/factories.py
+-rw-r--r--   0        0        0      450 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/settings.py
+-rw-r--r--   0        0        0     4648 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/test_client.py
+-rw-r--r--   0        0        0     7435 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/test_queries.py
+-rw-r--r--   0        0        0       93 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/test_smpp_gateway.py
+-rw-r--r--   0        0        0     2633 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/test_subscribers.py
+-rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 smpp_gateway-1.0.4/PKG-INFO
```

### Comparing `smpp_gateway-1.0.3/LICENSE` & `smpp_gateway-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/README.md` & `smpp_gateway-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/pyproject.toml` & `smpp_gateway-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smpp_gateway"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = [ "Caktus Group <team@caktusgroup.com>" ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/caktus/rapidsms-smpp-gateway"
 
 packages = [ { include = "smpp_gateway", from = "src" } ]
```

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/admin.py` & `smpp_gateway-1.0.4/src/smpp_gateway/admin.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/client.py` & `smpp_gateway-1.0.4/src/smpp_gateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         listen_mo_messages process.
         """
         now = timezone.now()
         MOMessage.objects.create(
             create_time=now,
             modify_time=now,
             backend=self.backend,
-            short_message=pdu.short_message,
+            short_message=pdu.short_message or b"",
             params=params,
             status=MOMessage.Status.NEW,
         )
         pg_notify(self.notify_mo_channel)
 
     def message_sent_handler(self, pdu: SubmitSMResp):
         """Called by smpplib base Client."""
```

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/management/commands/smpp_client.py` & `smpp_gateway-1.0.4/src/smpp_gateway/management/commands/smpp_client.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/migrations/0001_initial.py` & `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/migrations/0002_mtmessagestatus.py` & `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0002_mtmessagestatus.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/migrations/0003_big_pks_and_help_texts.py` & `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0003_big_pks_and_help_texts.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/migrations/0004_translations.py` & `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0004_translations.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/migrations/0005_alter_mtmessagestatus_command_status.py` & `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0005_alter_mtmessagestatus_command_status.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/models.py` & `smpp_gateway-1.0.4/src/smpp_gateway/models.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/outgoing.py` & `smpp_gateway-1.0.4/src/smpp_gateway/outgoing.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/queries.py` & `smpp_gateway-1.0.4/src/smpp_gateway/queries.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/smpp.py` & `smpp_gateway-1.0.4/src/smpp_gateway/smpp.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/subscribers.py` & `smpp_gateway-1.0.4/src/smpp_gateway/subscribers.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/src/smpp_gateway/utils.py` & `smpp_gateway-1.0.4/src/smpp_gateway/utils.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/tests/factories.py` & `smpp_gateway-1.0.4/tests/factories.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/tests/test_client.py` & `smpp_gateway-1.0.4/tests/test_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -78,14 +78,45 @@
 
         assert outbound_msg.status == MTMessage.Status.DELIVERED
         assert (
             outbound_msg_status.delivery_report.tobytes()
             == b"this is a delivery receipt"
         )
 
+    def test_received_null_short_message(self):
+        """When a message is received with a null short_message, persist it
+        and notify the MO listener."""
+        backend = BackendFactory()
+        client = get_smpplib_client(
+            "127.0.0.1",
+            8000,
+            "notify_mo_channel",
+            backend,
+            {},
+        )
+
+        pdu = DeliverSM("deliver_sm")
+        pdu.short_message = None
+        pdu.source_addr = "+46166371876"
+
+        listen_conn = pg_listen("notify_mo_channel")
+
+        client.message_received_handler(pdu)
+
+        # should notify the MO listener
+        listen_conn.poll()
+        assert len(listen_conn.notifies) == 1
+
+        # there should be a message for the MO listener to process
+        msg = MOMessage.objects.get()
+        assert msg.backend == backend
+        assert msg.short_message == b""
+        assert msg.params["source_addr"] == "+46166371876"
+        assert msg.status == MOMessage.Status.NEW
+
 
 @pytest.mark.django_db(transaction=True)
 def test_message_sent_handler():
     """The associated MTMessageStatus should be updated with the submission
     status and message_id.
     """
     backend = BackendFactory()
```

### Comparing `smpp_gateway-1.0.3/tests/test_queries.py` & `smpp_gateway-1.0.4/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/tests/test_subscribers.py` & `smpp_gateway-1.0.4/tests/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.3/PKG-INFO` & `smpp_gateway-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smpp-gateway
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Home-page: https://github.com/caktus/rapidsms-smpp-gateway
 License: MIT
 Author: Caktus Group
 Author-email: team@caktusgroup.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

