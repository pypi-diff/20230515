# Comparing `tmp/lumigo_log_shipper-1.0.8-py3-none-any.whl.zip` & `tmp/lumigo_log_shipper-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 12942 bytes, number of entries: 17
--rw-r--r--  2.0 unx        0 b- defN 19-Oct-13 14:10 lumigo_log_shipper/__init__.py
--rw-r--r--  2.0 unx     1602 b- defN 19-Oct-13 14:10 lumigo_log_shipper/lumigo_shipper.py
--rw-r--r--  2.0 unx      786 b- defN 19-Oct-13 14:10 lumigo_log_shipper/models.py
--rw-r--r--  2.0 unx        0 b- defN 19-Oct-13 14:10 lumigo_log_shipper/utils/__init__.py
--rw-r--r--  2.0 unx     1489 b- defN 19-Oct-13 14:10 lumigo_log_shipper/utils/aws_utils.py
--rw-r--r--  2.0 unx      703 b- defN 19-Oct-13 14:10 lumigo_log_shipper/utils/consts.py
--rw-r--r--  2.0 unx      225 b- defN 19-Oct-13 14:10 lumigo_log_shipper/utils/encoder.py
--rw-r--r--  2.0 unx     5171 b- defN 19-Oct-13 14:10 lumigo_log_shipper/utils/firehose_dal.py
--rw-r--r--  2.0 unx      876 b- defN 19-Oct-13 14:10 lumigo_log_shipper/utils/model_builder.py
--rw-r--r--  2.0 unx     1211 b- defN 19-Oct-13 14:10 lumigo_log_shipper/utils/shipper_utils.py
--rw-r--r--  2.0 unx      337 b- defN 19-Oct-13 14:10 lumigo_log_shipper/utils/sts.py
--rw-r--r--  2.0 unx      304 b- defN 19-Oct-13 14:10 lumigo_log_shipper/utils/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 19-Oct-13 14:11 lumigo_log_shipper-1.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1809 b- defN 19-Oct-13 14:11 lumigo_log_shipper-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Oct-13 14:11 lumigo_log_shipper-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 19-Oct-13 14:11 lumigo_log_shipper-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1536 b- defN 19-Oct-13 14:11 lumigo_log_shipper-1.0.8.dist-info/RECORD
-17 files, 27517 bytes uncompressed, 10356 bytes compressed:  62.4%
+Zip file size: 12974 bytes, number of entries: 17
+-rw-r--r--  2.0 unx        0 b- defN 19-Dec-22 08:52 lumigo_log_shipper/__init__.py
+-rw-r--r--  2.0 unx     1602 b- defN 19-Dec-22 08:52 lumigo_log_shipper/lumigo_shipper.py
+-rw-r--r--  2.0 unx      806 b- defN 19-Dec-22 08:52 lumigo_log_shipper/models.py
+-rw-r--r--  2.0 unx        0 b- defN 19-Dec-22 08:52 lumigo_log_shipper/utils/__init__.py
+-rw-r--r--  2.0 unx     1489 b- defN 19-Dec-22 08:52 lumigo_log_shipper/utils/aws_utils.py
+-rw-r--r--  2.0 unx      744 b- defN 19-Dec-22 08:52 lumigo_log_shipper/utils/consts.py
+-rw-r--r--  2.0 unx      225 b- defN 19-Dec-22 08:52 lumigo_log_shipper/utils/encoder.py
+-rw-r--r--  2.0 unx     5171 b- defN 19-Dec-22 08:52 lumigo_log_shipper/utils/firehose_dal.py
+-rw-r--r--  2.0 unx      927 b- defN 19-Dec-22 08:52 lumigo_log_shipper/utils/model_builder.py
+-rw-r--r--  2.0 unx     1211 b- defN 19-Dec-22 08:52 lumigo_log_shipper/utils/shipper_utils.py
+-rw-r--r--  2.0 unx      337 b- defN 19-Dec-22 08:52 lumigo_log_shipper/utils/sts.py
+-rw-r--r--  2.0 unx      304 b- defN 19-Dec-22 08:52 lumigo_log_shipper/utils/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 19-Dec-22 08:52 lumigo_log_shipper-1.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1809 b- defN 19-Dec-22 08:52 lumigo_log_shipper-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 19-Dec-22 08:52 lumigo_log_shipper-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 19-Dec-22 08:52 lumigo_log_shipper-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1536 b- defN 19-Dec-22 08:52 lumigo_log_shipper-1.0.9.dist-info/RECORD
+17 files, 27629 bytes uncompressed, 10388 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: lumigo_log_shipper/utils/sts.py
 Comment: 
 
 Filename: lumigo_log_shipper/utils/utils.py
 Comment: 
 
-Filename: lumigo_log_shipper-1.0.8.dist-info/LICENSE
+Filename: lumigo_log_shipper-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: lumigo_log_shipper-1.0.8.dist-info/METADATA
+Filename: lumigo_log_shipper-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: lumigo_log_shipper-1.0.8.dist-info/WHEEL
+Filename: lumigo_log_shipper-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: lumigo_log_shipper-1.0.8.dist-info/top_level.txt
+Filename: lumigo_log_shipper-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: lumigo_log_shipper-1.0.8.dist-info/RECORD
+Filename: lumigo_log_shipper-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lumigo_log_shipper/models.py

```diff
@@ -33,7 +33,8 @@
 
 
 @dataclass(frozen=True)
 class ShipperOutput:
     event_details: EventDetails
     timestamp: int
     message: str
+    log_stream: str
```

## lumigo_log_shipper/utils/consts.py

```diff
@@ -19,8 +19,10 @@
 
 SELF_ACCOUNT_ID = "SELF"
 
 FILTER_KEYWORDS = [
     "Task timed out",
     "Process exited before completing request",
     "REPORT RequestId",
+    "[ERROR]",
+    "ERROR	Invoke Error",
 ]
```

## lumigo_log_shipper/utils/model_builder.py

```diff
@@ -6,23 +6,24 @@
     EventDetails,
     FunctionDetails,
 )
 from lumigo_log_shipper.utils.aws_utils import get_function_arn
 
 
 def parse_aws_extracted_data(
-    extracted_data: AwsLogSubscriptionEvent
+    extracted_data: AwsLogSubscriptionEvent,
 ) -> List[ShipperOutput]:
     result: List[ShipperOutput] = []
     function_arn = get_function_arn(extracted_data)
     for log_event in extracted_data.log_events:
         shipper_output = ShipperOutput(
             message=log_event.message,
             timestamp=log_event.timestamp,
             event_details=EventDetails(
                 aws_account_id=extracted_data.owner,
                 timestamp=log_event.timestamp,
                 function_details=FunctionDetails(resource_id=function_arn),
             ),
+            log_stream=extracted_data.log_stream,
         )
         result.append(shipper_output)
     return result
```

## Comparing `lumigo_log_shipper-1.0.8.dist-info/LICENSE` & `lumigo_log_shipper-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lumigo_log_shipper-1.0.8.dist-info/METADATA` & `lumigo_log_shipper-1.0.9.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumigo-log-shipper
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ship logs to lumigo platform
 Home-page: https://github.com/lumigo-io/lumigo-python-log-shipper.git
 Author: Lumigo LTD (https://lumigo.io)
 Author-email: support@lumigo.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `lumigo_log_shipper-1.0.8.dist-info/RECORD` & `lumigo_log_shipper-1.0.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 lumigo_log_shipper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lumigo_log_shipper/lumigo_shipper.py,sha256=OL3JoGkEltdyC6-fFJv4_ibAZhs-7ABrsnVuHvalNs8,1602
-lumigo_log_shipper/models.py,sha256=SSKWQm6OxtqPF23bQfGrTWF_o4etMQVbRVJ4xl6ot3U,786
+lumigo_log_shipper/models.py,sha256=Hhb7183T3I7rbbz_Xba_1gPagUAELITuSbQ6zcfSAuc,806
 lumigo_log_shipper/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lumigo_log_shipper/utils/aws_utils.py,sha256=acruO9n2mePCRu6NDOUe62ove1aESwijw7JLrtE9kbk,1489
-lumigo_log_shipper/utils/consts.py,sha256=Bw92aLxuO5Rf0toFLh3GE3ni4Kuws8WFrwqvJSl3VzY,703
+lumigo_log_shipper/utils/consts.py,sha256=VXhGJ_T1CXg4JTEMTEXKviluaNGD5YA6-V9ECqpE09Y,744
 lumigo_log_shipper/utils/encoder.py,sha256=hgokpsn8i3MjSxnU9PxGqOTx_f1CxJPsHLyk5wcvTzY,225
 lumigo_log_shipper/utils/firehose_dal.py,sha256=GZG4OOLM1z-cpnisKgSOfssnH4olowRdOllYv_SCLO8,5171
-lumigo_log_shipper/utils/model_builder.py,sha256=UeA8qF1ME0BSnGM_8G1dWkOyVGlin5HFYFt39-yQz_M,876
+lumigo_log_shipper/utils/model_builder.py,sha256=N5jg7Ky8ZvRMnwsNTkd9buObXNDllgoyCqCOQHWS3hg,927
 lumigo_log_shipper/utils/shipper_utils.py,sha256=uRcVQ6XKIcYGtct5PHKuk_JPWdMfbmfNp6Iez52UP6A,1211
 lumigo_log_shipper/utils/sts.py,sha256=NY27Xg6P9r9HFeWPCgcn9PY9gOIKljaNucLY_-kSWqQ,337
 lumigo_log_shipper/utils/utils.py,sha256=DBCFXLHXXrWeTM2JBqagoFwhrzEKPivqg9qdEPquhMI,304
-lumigo_log_shipper-1.0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-lumigo_log_shipper-1.0.8.dist-info/METADATA,sha256=iB-v5g2lJhAB3b6qHZdXP1NbhHFjl-pjwN1m0FGojZY,1809
-lumigo_log_shipper-1.0.8.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
-lumigo_log_shipper-1.0.8.dist-info/top_level.txt,sha256=M5jFKVYd5872RMp8a2OKTP7EuvhdR5PC5Y_mref8tB0,19
-lumigo_log_shipper-1.0.8.dist-info/RECORD,,
+lumigo_log_shipper-1.0.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+lumigo_log_shipper-1.0.9.dist-info/METADATA,sha256=yWCogtdjYNFuSDitpefqmJcPeR14ys4Y7-gMpmcx08Q,1809
+lumigo_log_shipper-1.0.9.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
+lumigo_log_shipper-1.0.9.dist-info/top_level.txt,sha256=M5jFKVYd5872RMp8a2OKTP7EuvhdR5PC5Y_mref8tB0,19
+lumigo_log_shipper-1.0.9.dist-info/RECORD,,
```

