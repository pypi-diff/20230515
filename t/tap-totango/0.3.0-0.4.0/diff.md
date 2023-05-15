# Comparing `tmp/tap_totango-0.3.0.tar.gz` & `tmp/tap_totango-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_totango-0.3.0.tar", max compression
+gzip compressed data, was "tap_totango-0.4.0.tar", max compression
```

## Comparing `tap_totango-0.3.0.tar` & `tap_totango-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     9247 2023-05-14 23:55:50.616372 tap_totango-0.3.0/README.md
--rw-r--r--   0        0        0     1141 2023-05-15 00:56:24.204530 tap_totango-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-13 00:04:24.083057 tap_totango-0.3.0/tap_totango/__init__.py
--rw-r--r--   0        0        0     4583 2023-05-13 16:21:54.720246 tap_totango-0.3.0/tap_totango/client.py
--rw-r--r--   0        0        0      431 2023-05-13 22:00:37.289103 tap_totango-0.3.0/tap_totango/schemas/accounts.json
--rw-r--r--   0        0        0     1878 2023-05-13 16:35:50.832342 tap_totango-0.3.0/tap_totango/schemas/events.json
--rw-r--r--   0        0        0      918 2023-05-14 01:35:34.115672 tap_totango-0.3.0/tap_totango/schemas/users.json
--rw-r--r--   0        0        0     4764 2023-05-14 01:28:57.199660 tap_totango-0.3.0/tap_totango/streams.py
--rw-r--r--   0        0        0    10271 2023-05-15 00:40:19.613886 tap_totango-0.3.0/tap_totango/tap.py
--rw-r--r--   0        0        0     9996 1970-01-01 00:00:00.000000 tap_totango-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     9247 2023-05-14 23:55:50.616372 tap_totango-0.4.0/README.md
+-rw-r--r--   0        0        0     1141 2023-05-15 02:11:10.834867 tap_totango-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-13 00:04:24.083057 tap_totango-0.4.0/tap_totango/__init__.py
+-rw-r--r--   0        0        0     4583 2023-05-13 16:21:54.720246 tap_totango-0.4.0/tap_totango/client.py
+-rw-r--r--   0        0        0      431 2023-05-13 22:00:37.289103 tap_totango-0.4.0/tap_totango/schemas/accounts.json
+-rw-r--r--   0        0        0     1878 2023-05-13 16:35:50.832342 tap_totango-0.4.0/tap_totango/schemas/events.json
+-rw-r--r--   0        0        0      918 2023-05-14 01:35:34.115672 tap_totango-0.4.0/tap_totango/schemas/users.json
+-rw-r--r--   0        0        0     5012 2023-05-15 01:57:19.700153 tap_totango-0.4.0/tap_totango/streams.py
+-rw-r--r--   0        0        0    10270 2023-05-15 02:05:54.608654 tap_totango-0.4.0/tap_totango/tap.py
+-rw-r--r--   0        0        0     9996 1970-01-01 00:00:00.000000 tap_totango-0.4.0/PKG-INFO
```

### Comparing `tap_totango-0.3.0/README.md` & `tap_totango-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tap_totango-0.3.0/pyproject.toml` & `tap_totango-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-totango"
-version = "0.3.0"
+version = "0.4.0"
 description = "`tap-totango` is a Singer tap for the Totango API, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Edson Nogueira"]
 keywords = [
     "ELT",
     "totango",
 ]
```

### Comparing `tap_totango-0.3.0/tap_totango/client.py` & `tap_totango-0.4.0/tap_totango/client.py`

 * *Files identical despite different names*

### Comparing `tap_totango-0.3.0/tap_totango/schemas/events.json` & `tap_totango-0.4.0/tap_totango/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap_totango-0.3.0/tap_totango/schemas/users.json` & `tap_totango-0.4.0/tap_totango/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap_totango-0.3.0/tap_totango/streams.py` & `tap_totango-0.4.0/tap_totango/streams.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 
 # TODO: Delete this is if not using json files for schema definition
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 # TODO: - Override `UsersStream` and `GroupsStream` with your own stream definition.
 #       - Copy-paste as many times as needed to create multiple stream types.
 
 
-class EventsStream(totangoStream):
+class AccountsStream(totangoStream):
     """Define custom stream."""
 
-    name = "events"
+    name = "accounts"
     rest_method = "POST"
 
-    path = "/api/v2/events/search"
+    path = "/api/v1/search/accounts"
 
-    records_jsonpath = "$.response.events.hits[*]"
-    primary_keys = ["id"]
+    records_jsonpath = "$.response.accounts.hits[*]"
+    primary_keys = ["name"]
     replication_key = None
     # Optionally, you may also use `schema_filepath` in place of `schema`:
-    schema_filepath = SCHEMAS_DIR / "events.json"  # noqa: ERA001
+    schema_filepath = SCHEMAS_DIR / "accounts.json"  # noqa: ERA001
 
     def prepare_request_payload(
         self,
         context: dict | None,  # noqa: ARG002
         next_page_token: t.Any | None,  # noqa: ARG002
     ) -> dict | None:
         """Prepare the data payload for the REST API request.
@@ -48,38 +48,44 @@
 
         Returns:
             A dictionary with the JSON body for a POST requests.
         """
         # TODO: Delete this method if no payload is required. (Most REST APIs.)
         params = self.config
         query = {
-            "terms": params["events_terms"],
-            "fields": [],
-            "offset": params["events_offset"],
-            "count": params["events_count"],
+            "terms": params["accounts_terms"],
+            "fields": params["accounts_fields"],
+            "offset": params["accounts_offset"],
+            "count": params["accounts_count"],
+            "sort_by": params["accounts_sort_by"],
+            "sort_order": params["accounts_sort_order"],
         }
         data = {"query": json.dumps(query)}
-        if params.get("account_id"):
-            data["account_id"] = params["account_id"]
         return data
 
+    def get_child_context(self, record: dict, context: t.Optional[dict]) -> dict:
+        """Return a context dictionary for child streams."""
+        return {
+            "account_id": record["name"],
+        }
 
-class AccountsStream(totangoStream):
+
+class UsersStream(totangoStream):
     """Define custom stream."""
 
-    name = "accounts"
+    name = "users"
     rest_method = "POST"
 
-    path = "/api/v1/search/accounts"
+    path = "/api/v1/search/users"
 
-    records_jsonpath = "$.response.accounts.hits[*]"
+    records_jsonpath = "$.response.users.hits[*]"
     primary_keys = ["name"]
     replication_key = None
     # Optionally, you may also use `schema_filepath` in place of `schema`:
-    schema_filepath = SCHEMAS_DIR / "accounts.json"  # noqa: ERA001
+    schema_filepath = SCHEMAS_DIR / "users.json"  # noqa: ERA001
 
     def prepare_request_payload(
         self,
         context: dict | None,  # noqa: ARG002
         next_page_token: t.Any | None,  # noqa: ARG002
     ) -> dict | None:
         """Prepare the data payload for the REST API request.
@@ -92,38 +98,41 @@
 
         Returns:
             A dictionary with the JSON body for a POST requests.
         """
         # TODO: Delete this method if no payload is required. (Most REST APIs.)
         params = self.config
         query = {
-            "terms": params["accounts_terms"],
-            "fields": params["accounts_fields"],
-            "offset": params["accounts_offset"],
-            "count": params["accounts_count"],
-            "sort_by": params["accounts_sort_by"],
-            "sort_order": params["accounts_sort_order"],
+            "terms": params["users_terms"],
+            "fields": params["users_fields"],
+            "offset": params["users_offset"],
+            "count": params["users_count"],
+            "sort_by": params["users_sort_by"],
+            "sort_order": params["users_sort_order"],
         }
         data = {"query": json.dumps(query)}
         return data
 
 
-class UsersStream(totangoStream):
+class EventsStream(totangoStream):
     """Define custom stream."""
 
-    name = "users"
+    name = "events"
     rest_method = "POST"
 
-    path = "/api/v1/search/users"
+    path = "/api/v2/events/search"
 
-    records_jsonpath = "$.response.users.hits[*]"
-    primary_keys = ["name"]
+    records_jsonpath = "$.response.events.hits[*]"
+    primary_keys = ["id"]
     replication_key = None
     # Optionally, you may also use `schema_filepath` in place of `schema`:
-    schema_filepath = SCHEMAS_DIR / "users.json"  # noqa: ERA001
+    schema_filepath = SCHEMAS_DIR / "events.json"  # noqa: ERA001
+
+    parent_stream_type = AccountsStream
+    ignore_parent_replication_key = True
 
     def prepare_request_payload(
         self,
         context: dict | None,  # noqa: ARG002
         next_page_token: t.Any | None,  # noqa: ARG002
     ) -> dict | None:
         """Prepare the data payload for the REST API request.
@@ -136,16 +145,15 @@
 
         Returns:
             A dictionary with the JSON body for a POST requests.
         """
         # TODO: Delete this method if no payload is required. (Most REST APIs.)
         params = self.config
         query = {
-            "terms": params["users_terms"],
-            "fields": params["users_fields"],
-            "offset": params["users_offset"],
-            "count": params["users_count"],
-            "sort_by": params["users_sort_by"],
-            "sort_order": params["users_sort_order"],
+            "terms": params["events_terms"],
+            "fields": [],
+            "offset": params["events_offset"],
+            "count": params["events_count"],
         }
         data = {"query": json.dumps(query)}
+        data["account_id"] = "{account_id}"
         return data
```

### Comparing `tap_totango-0.3.0/tap_totango/tap.py` & `tap_totango-0.4.0/tap_totango/tap.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                     },
                 ]
             ],
         ),
         th.Property(
             "accounts_count",
             th.IntegerType,
-            default=1000,
+            default=100,
             description="The maximum number of accounts to return in the accounts result set. The max. value for count is 1000.",
         ),
         th.Property(
             "accounts_offset",
             th.IntegerType,
             default=0,
             description='Record number (0 states "start at record 0"). The record size can be defined using the count parameter (and limited to 1000). Tip: To page through results, ask for 1000 records (count: 1000). If you receive 1000 records, assume there’s more, in which case you want to pull the next 1000 records (offset: 1000…then 2000…etc.). Repeat paging until the number of records returned is less than 1000.',
```

### Comparing `tap_totango-0.3.0/PKG-INFO` & `tap_totango-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-totango
-Version: 0.3.0
+Version: 0.4.0
 Summary: `tap-totango` is a Singer tap for the Totango API, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,totango
 Author: Edson Nogueira
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

