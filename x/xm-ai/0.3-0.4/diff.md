# Comparing `tmp/xm_ai-0.3-py3-none-any.whl.zip` & `tmp/xm_ai-0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5416 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 21:52 xm_ai/__init__.py
--rw-r--r--  2.0 unx      523 b- defN 23-May-05 21:52 xm_ai/aws_utils.py
--rw-r--r--  2.0 unx     2240 b- defN 23-May-05 21:52 xm_ai/database_utils.py
--rw-r--r--  2.0 unx     2285 b- defN 23-May-05 21:52 xm_ai/email_utils.py
--rw-r--r--  2.0 unx      238 b- defN 23-May-05 21:52 xm_ai/excel_utils.py
--rw-r--r--  2.0 unx     1891 b- defN 23-May-05 21:52 xm_ai/query_utils.py
--rw-r--r--  2.0 unx      134 b- defN 23-May-05 21:52 xm_ai/syntax_utils.py
--rw-r--r--  2.0 unx      600 b- defN 23-May-05 21:52 xm_ai/time_utils.py
--rw-r--r--  2.0 unx      471 b- defN 23-May-05 21:52 xm_ai-0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 21:52 xm_ai-0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-05 21:52 xm_ai-0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      887 b- defN 23-May-05 21:52 xm_ai-0.3.dist-info/RECORD
-12 files, 9367 bytes uncompressed, 3942 bytes compressed:  57.9%
+Zip file size: 5635 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-15 16:45 xm_ai/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 23-May-15 16:45 xm_ai/aws_utils.py
+-rw-r--r--  2.0 unx     2225 b- defN 23-May-15 16:45 xm_ai/database_utils.py
+-rw-r--r--  2.0 unx     2285 b- defN 23-May-15 16:45 xm_ai/email_utils.py
+-rw-r--r--  2.0 unx      238 b- defN 23-May-15 16:45 xm_ai/excel_utils.py
+-rw-r--r--  2.0 unx     1891 b- defN 23-May-15 16:45 xm_ai/query_utils.py
+-rw-r--r--  2.0 unx      134 b- defN 23-May-15 16:45 xm_ai/syntax_utils.py
+-rw-r--r--  2.0 unx      600 b- defN 23-May-15 16:45 xm_ai/time_utils.py
+-rw-r--r--  2.0 unx      471 b- defN 23-May-15 16:45 xm_ai-0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 16:45 xm_ai-0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-15 16:45 xm_ai-0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      888 b- defN 23-May-15 16:45 xm_ai-0.4.dist-info/RECORD
+12 files, 10030 bytes uncompressed, 4161 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: xm_ai/syntax_utils.py
 Comment: 
 
 Filename: xm_ai/time_utils.py
 Comment: 
 
-Filename: xm_ai-0.3.dist-info/METADATA
+Filename: xm_ai-0.4.dist-info/METADATA
 Comment: 
 
-Filename: xm_ai-0.3.dist-info/WHEEL
+Filename: xm_ai-0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xm_ai-0.3.dist-info/top_level.txt
+Filename: xm_ai-0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xm_ai-0.3.dist-info/RECORD
+Filename: xm_ai-0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xm_ai/aws_utils.py

```diff
@@ -1,15 +1,38 @@
+import base64
+import json
+
 import boto3
+from botocore.exceptions import ClientError
 
 s3 = boto3.client('s3')  # Create an S3 client
 
 bucket_name = 'trial-report'  # specify the S3 bucket you want to download from
 
 
 # Download the file
 def download_from_s3(file_name, local_file_name):
     s3.download_file(bucket_name, file_name, local_file_name)  # 3rd argument is the local file name
 
 
 # Re-upload the file to the same s3 bucket
 def upload_to_s3(local_file_name, foreign_file_name):
     s3.upload_file(local_file_name, bucket_name, foreign_file_name)  # local file name, bucket, foreign name
+
+
+def get_secret(keyname: str) -> dict or bytes:
+    # Create a Secrets Manager client
+    session = boto3.session.Session()
+    client = session.client(
+        service_name='secretsmanager',
+        region_name="us-east-2"
+    )
+    try:
+        get_secret_value_response = client.get_secret_value(
+            SecretId=keyname
+        )
+        if 'SecretString' in get_secret_value_response:
+            return json.loads(get_secret_value_response['SecretString'])
+        else:
+            return base64.b64decode(get_secret_value_response['SecretBinary'])
+    except ClientError as e:
+        raise e
```

## xm_ai/database_utils.py

```diff
@@ -1,62 +1,55 @@
-from botocore.exceptions import ClientError, EndpointConnectionError
+import pymongo.errors
+from botocore.exceptions import EndpointConnectionError
 from pymongo import MongoClient
-import base64
-import boto3
-import json
+from pymongo.database import Database
 from enum import Enum
+from xm_ai.aws_utils import get_secret
 
 
 class xMentiumMongoSecret(Enum):
     username = 'username'
     password = 'password'
     address = 'address'
     port = 'port'
     database = 'database'
     production_name: str = 'production'
 
 
-def get_secret(keyname: str) -> dict or bytes:
-    # Create a Secrets Manager client
-    session = boto3.session.Session()
-    client = session.client(
-        service_name='secretsmanager',
-        region_name="us-east-2"
-    )
+def get_database(server_name: str) -> Database:
+    database_name = server_name
+    if server_name == "production" or server_name == "staging":
+        secret = get_secret("xmentium_mongo")
+        connstring = f"mongodb:" \
+                     f"//{secret[xMentiumMongoSecret.username.value]}" \
+                     f":{secret[xMentiumMongoSecret.password.value]}" \
+                     f"@{secret[xMentiumMongoSecret.address.value]}" \
+                     f":{secret[xMentiumMongoSecret.port.value]}" \
+                     f"/{secret[xMentiumMongoSecret.database.value]}"
+        database_name = secret[
+            xMentiumMongoSecret.production_name.value] if server_name == "production" else server_name
+    elif server_name == "develop":
+        connstring = "mongodb://localhost:27017"
+    elif server_name == "ai":
+        secret = get_secret("ai_mongo")
+        connstring = f"mongodb+srv:" \
+                     f"//{secret[xMentiumMongoSecret.username.value]}" \
+                     f":{secret[xMentiumMongoSecret.password.value]}" \
+                     f"@{secret[xMentiumMongoSecret.address.value]}" \
+                     f"/{secret[xMentiumMongoSecret.database.value]}"
+    else:
+        raise ValueError("Invalid Option Selected")
+
     try:
-        get_secret_value_response = client.get_secret_value(
-            SecretId=keyname
-        )
-        if 'SecretString' in get_secret_value_response:
-            return json.loads(get_secret_value_response['SecretString'])
-        else:
-            return base64.b64decode(get_secret_value_response['SecretBinary'])
-    except ClientError as e:
-        raise e
-
-
-try:
-    # connstring for production/staging
-    secret = get_secret("xmentium_mongo")
-    remote_db_connstring = f"mongodb:" \
-                           f"//{secret[xMentiumMongoSecret.username.value]}" \
-                           f":{secret[xMentiumMongoSecret.password.value]}" \
-                           f"@{secret[xMentiumMongoSecret.address.value]}" \
-                           f":{secret[xMentiumMongoSecret.port.value]}" \
-                           f"/{secret[xMentiumMongoSecret.database.value]}"
-
-    # noinspection PyTypeChecker
-    db = MongoClient(remote_db_connstring)[secret[xMentiumMongoSecret.production_name.value]]
-    staging_db = MongoClient(remote_db_connstring)["staging"]
-
-    # connstring for ai database
-    secret = get_secret("ai_mongo")
-    ai_db_connstring = f"mongodb+srv:" \
-                       f"//{secret[xMentiumMongoSecret.username.value]}" \
-                       f":{secret[xMentiumMongoSecret.password.value]}" \
-                       f"@{secret[xMentiumMongoSecret.address.value]}" \
-                       f"/{secret[xMentiumMongoSecret.database.value]}"
-    ai_db = MongoClient(ai_db_connstring)
-
-except EndpointConnectionError as error:
-    print(error)
-    print("You are offline, so Boto3 could not create a session")
+        client = MongoClient(connstring)[database_name]
+        try:
+            client.templates.find_one({})
+            return client
+        except pymongo.errors.ServerSelectionTimeoutError as error:
+            print(error)
+            print("This connection string likely does not have access to the database")
+            raise pymongo.errors.ServerSelectionTimeoutError
+
+    except EndpointConnectionError as error:
+        print(error)
+        print("You are offline, so Boto3 could not create a session")
+        raise EndpointConnectionError
```

## Comparing `xm_ai-0.3.dist-info/RECORD` & `xm_ai-0.4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 xm_ai/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xm_ai/aws_utils.py,sha256=lh8dfbaiZCgKwuIMXS39vZvwN6rfp1qfQcbp6A_XOO8,523
-xm_ai/database_utils.py,sha256=eQNQAz-xQ0hCL5ftfGaw9hQbyLw7aWjFMvZRs0T_tCI,2240
+xm_ai/aws_utils.py,sha256=BZ8lqidsBhckW2Jy6-eJVbomt5yyo7LWqmKuGu2Ewe0,1200
+xm_ai/database_utils.py,sha256=bbvXUyyF-1ZNPnvcFiRWCkbBy08zfPZB-YZZZdqcSw8,2225
 xm_ai/email_utils.py,sha256=H23WsR-nvWdB-OW5ZmIdIDoZX6m91NoItuTnA4YG3uU,2285
 xm_ai/excel_utils.py,sha256=xafW_NtNMq6qETFisMDPohPfs34BbekUdyM1qQefr7o,238
 xm_ai/query_utils.py,sha256=tNALaP99OznJ3l3UaajT643RRZ2lhPwhM3Fb2PvD6sg,1891
 xm_ai/syntax_utils.py,sha256=aWGhKkLLZQSOO4_gee_9EGO1b1KI8-KXZd45Ts2jNj4,134
 xm_ai/time_utils.py,sha256=qEsWIjq3GRG3a4L8yxQe2b_gJszsmXRDSsBZKR4b9cs,600
-xm_ai-0.3.dist-info/METADATA,sha256=66-d9Ggp9kSjcPhfyAPjMkvrmJNBdIctIa-LU5pMgq0,471
-xm_ai-0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xm_ai-0.3.dist-info/top_level.txt,sha256=0tH-EgTFu93crY6L8lAB9az_LQotSkuUdG1rObgP0iA,6
-xm_ai-0.3.dist-info/RECORD,,
+xm_ai-0.4.dist-info/METADATA,sha256=RjeGU463JrTUIcCT8EBxEvk-i3IOEn5DV-T0W90sXoU,471
+xm_ai-0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xm_ai-0.4.dist-info/top_level.txt,sha256=0tH-EgTFu93crY6L8lAB9az_LQotSkuUdG1rObgP0iA,6
+xm_ai-0.4.dist-info/RECORD,,
```

