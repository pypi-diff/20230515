# Comparing `tmp/boto3-helpers-1.3.0.tar.gz` & `tmp/boto3-helpers-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-helpers-1.3.0.tar", last modified: Thu Apr  6 15:28:30 2023, max compression
+gzip compressed data, was "boto3-helpers-1.4.0.tar", last modified: Mon May 15 16:15:33 2023, max compression
```

## Comparing `boto3-helpers-1.3.0.tar` & `boto3-helpers-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-04-06 15:28:30.084214 boto3-helpers-1.3.0/
--rw-r--r--   0 bo.bayles   (501) staff       (20)    10174 2022-08-24 20:40:12.000000 boto3-helpers-1.3.0/LICENSE
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2578 2023-04-06 15:28:30.084468 boto3-helpers-1.3.0/PKG-INFO
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2099 2022-09-22 19:00:18.000000 boto3-helpers-1.3.0/README.rst
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-04-06 15:28:30.065202 boto3-helpers-1.3.0/boto3_helpers/
--rw-r--r--   0 bo.bayles   (501) staff       (20)        0 2022-12-15 15:18:48.000000 boto3-helpers-1.3.0/boto3_helpers/__init__.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3851 2022-09-22 21:23:05.000000 boto3-helpers-1.3.0/boto3_helpers/arn.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1792 2022-09-22 19:00:18.000000 boto3-helpers-1.3.0/boto3_helpers/awslambda.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3217 2022-09-23 13:50:11.000000 boto3-helpers-1.3.0/boto3_helpers/cloudwatch.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3694 2022-09-01 21:23:37.000000 boto3-helpers-1.3.0/boto3_helpers/dynamodb.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     6306 2023-01-11 18:57:17.000000 boto3-helpers-1.3.0/boto3_helpers/events.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1810 2022-09-22 19:00:18.000000 boto3-helpers-1.3.0/boto3_helpers/mediatailor.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1674 2022-09-02 14:20:47.000000 boto3-helpers-1.3.0/boto3_helpers/pagination.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2861 2022-10-17 19:48:22.000000 boto3-helpers-1.3.0/boto3_helpers/s3.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3271 2023-04-06 15:28:10.000000 boto3-helpers-1.3.0/boto3_helpers/signed_requests.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     7087 2022-09-23 13:50:11.000000 boto3-helpers-1.3.0/boto3_helpers/sqs.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     4469 2022-09-01 20:24:17.000000 boto3-helpers-1.3.0/boto3_helpers/sts.py
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-04-06 15:28:30.070183 boto3-helpers-1.3.0/boto3_helpers.egg-info/
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2578 2023-04-06 15:28:29.000000 boto3-helpers-1.3.0/boto3_helpers.egg-info/PKG-INFO
--rw-r--r--   0 bo.bayles   (501) staff       (20)      785 2023-04-06 15:28:29.000000 boto3-helpers-1.3.0/boto3_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)        1 2023-04-06 15:28:29.000000 boto3-helpers-1.3.0/boto3_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)       15 2023-04-06 15:28:29.000000 boto3-helpers-1.3.0/boto3_helpers.egg-info/requires.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)       14 2023-04-06 15:28:29.000000 boto3-helpers-1.3.0/boto3_helpers.egg-info/top_level.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)      171 2022-09-01 20:18:16.000000 boto3-helpers-1.3.0/pyproject.toml
--rw-r--r--   0 bo.bayles   (501) staff       (20)      689 2023-04-06 15:28:30.085846 boto3-helpers-1.3.0/setup.cfg
--rw-r--r--   0 bo.bayles   (501) staff       (20)       38 2022-09-01 20:23:34.000000 boto3-helpers-1.3.0/setup.py
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-04-06 15:28:30.083160 boto3-helpers-1.3.0/tests/
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2075 2022-09-22 21:23:05.000000 boto3-helpers-1.3.0/tests/test_arn.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1806 2022-09-22 19:00:18.000000 boto3-helpers-1.3.0/tests/test_awslambda.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3749 2022-09-23 13:50:11.000000 boto3-helpers-1.3.0/tests/test_cloudwatch.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     5538 2022-09-01 21:23:46.000000 boto3-helpers-1.3.0/tests/test_dynamodb.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     9813 2022-09-22 19:00:18.000000 boto3-helpers-1.3.0/tests/test_events.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3468 2022-09-01 21:00:54.000000 boto3-helpers-1.3.0/tests/test_mediatailor.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2200 2022-08-25 15:02:02.000000 boto3-helpers-1.3.0/tests/test_pagination.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2369 2022-10-17 19:48:22.000000 boto3-helpers-1.3.0/tests/test_s3.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1997 2023-04-06 15:28:10.000000 boto3-helpers-1.3.0/tests/test_signed_requests.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     6180 2022-09-22 19:00:18.000000 boto3-helpers-1.3.0/tests/test_sqs.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     4106 2022-08-25 21:06:36.000000 boto3-helpers-1.3.0/tests/test_sts.py
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-05-15 16:15:33.809904 boto3-helpers-1.4.0/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)    10174 2022-08-24 20:40:12.000000 boto3-helpers-1.4.0/LICENSE
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2578 2023-05-15 16:15:33.810172 boto3-helpers-1.4.0/PKG-INFO
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2099 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/README.rst
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-05-15 16:15:33.790717 boto3-helpers-1.4.0/boto3_helpers/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)        0 2022-12-15 15:18:48.000000 boto3-helpers-1.4.0/boto3_helpers/__init__.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3851 2022-09-22 21:23:05.000000 boto3-helpers-1.4.0/boto3_helpers/arn.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1792 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/boto3_helpers/awslambda.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3217 2022-09-23 13:50:11.000000 boto3-helpers-1.4.0/boto3_helpers/cloudwatch.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4713 2023-05-15 15:59:52.000000 boto3-helpers-1.4.0/boto3_helpers/dynamodb.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     6306 2023-01-11 18:57:17.000000 boto3-helpers-1.4.0/boto3_helpers/events.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1810 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/boto3_helpers/mediatailor.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2213 2023-05-15 15:59:52.000000 boto3-helpers-1.4.0/boto3_helpers/pagination.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2861 2022-10-17 19:48:22.000000 boto3-helpers-1.4.0/boto3_helpers/s3.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3271 2023-04-06 15:28:10.000000 boto3-helpers-1.4.0/boto3_helpers/signed_requests.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     7087 2022-09-23 13:50:11.000000 boto3-helpers-1.4.0/boto3_helpers/sqs.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4469 2022-09-01 20:24:17.000000 boto3-helpers-1.4.0/boto3_helpers/sts.py
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-05-15 16:15:33.795251 boto3-helpers-1.4.0/boto3_helpers.egg-info/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2578 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 bo.bayles   (501) staff       (20)      785 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)        1 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)       15 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/requires.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)       14 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/top_level.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)      171 2022-09-01 20:18:16.000000 boto3-helpers-1.4.0/pyproject.toml
+-rw-r--r--   0 bo.bayles   (501) staff       (20)      689 2023-05-15 16:15:33.811583 boto3-helpers-1.4.0/setup.cfg
+-rw-r--r--   0 bo.bayles   (501) staff       (20)       38 2022-09-01 20:23:34.000000 boto3-helpers-1.4.0/setup.py
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-05-15 16:15:33.808873 boto3-helpers-1.4.0/tests/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2075 2022-09-22 21:23:05.000000 boto3-helpers-1.4.0/tests/test_arn.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1806 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/tests/test_awslambda.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3749 2022-09-23 13:50:11.000000 boto3-helpers-1.4.0/tests/test_cloudwatch.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     5664 2023-05-15 15:59:52.000000 boto3-helpers-1.4.0/tests/test_dynamodb.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     9813 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/tests/test_events.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3468 2022-09-01 21:00:54.000000 boto3-helpers-1.4.0/tests/test_mediatailor.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2200 2023-04-28 15:58:17.000000 boto3-helpers-1.4.0/tests/test_pagination.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2369 2022-10-17 19:48:22.000000 boto3-helpers-1.4.0/tests/test_s3.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1997 2023-04-06 15:28:10.000000 boto3-helpers-1.4.0/tests/test_signed_requests.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     6180 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/tests/test_sqs.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4106 2022-08-25 21:06:36.000000 boto3-helpers-1.4.0/tests/test_sts.py
```

### Comparing `boto3-helpers-1.3.0/LICENSE` & `boto3-helpers-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/PKG-INFO` & `boto3-helpers-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boto3-helpers
-Version: 1.3.0
+Version: 1.4.0
 Summary: Helper utilities for boto3
 Author: Bo Bayles
 Author-email: bo.bayles@wurl.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/openwurl/boto3-helpers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boto3-helpers-1.3.0/README.rst` & `boto3-helpers-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers/arn.py` & `boto3-helpers-1.4.0/boto3_helpers/arn.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers/awslambda.py` & `boto3-helpers-1.4.0/boto3_helpers/awslambda.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers/cloudwatch.py` & `boto3-helpers-1.4.0/boto3_helpers/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers/dynamodb.py` & `boto3-helpers-1.4.0/boto3_helpers/dynamodb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+from boto3 import resource as boto3_resource
+
+
+def _table_or_name(x):
+    if isinstance(x, str):
+        return boto3_resource('dynamodb').Table(x)
+
+    return x
+
+
 def _page_helper(method, **kwargs):
     while True:
         resp = method(**kwargs)
         yield from resp.get('Items', [])
         start_key = resp.get('LastEvaluatedKey')
         if not start_key:
             break
         kwargs['ExclusiveStartKey'] = start_key
 
 
 def query_table(ddb_table, **kwargs):
     """Yield all of the items that match the DynamoDB query:
 
-    * *ddb_table* is a ``boto3.resource('dynamodb').Table`` instance.
+    * *ddb_table* is a table name or a ``boto3.resource('dynamodb').Table`` instance.
     * *kwargs* are passed directly to the ``Table.query`` method.
 
     Usage:
 
     .. code-block:: python
 
         from boto3 import resource as boto3_resource
@@ -25,21 +35,22 @@
         ddb_resource = boto3_resource('dynamodb')
         ddb_table = ddb_resource.Table('example-table')
         condition = Key('username').eq('johndoe')
         all_items = list(
             query_table(ddb_table, KeyConditionExpression=condition)
         )
     """
-    yield from _page_helper(ddb_table.query, **kwargs)
+    t = _table_or_name(ddb_table)
+    yield from _page_helper(t.query, **kwargs)
 
 
 def scan_table(ddb_table, **kwargs):
     """Yield all of the items that match the DynamoDB query:
 
-    * *ddb_table* is a ``boto3.resource('dynamodb').Table`` instance.
+    * *ddb_table* is a table name or a ``boto3.resource('dynamodb').Table`` instance.
     * *kwargs* are passed directly to the ``Table.scan`` method.
 
     Usage:
 
     .. code-block:: python
 
         from boto3 import resource as boto3_resource
@@ -49,23 +60,24 @@
         ddb_resource = boto3_resource('dynamodb')
         ddb_table = ddb_resource.Table('example-table')
         condition = Attr('username').eq('johndoe')
         all_items = list(
             scan_table(ddb_table, FilterExpression=condition)
         )
     """
-    yield from _page_helper(ddb_table.scan, **kwargs)
+    t = _table_or_name(ddb_table)
+    yield from _page_helper(t.scan, **kwargs)
 
 
 def update_attributes(ddb_table, key, update_map, **kwargs):
-    """Update a DyanmoDB table item and return the result:
+    """Update a DyanmoDB table item and return the ``update_item`` response:
 
-    * *ddb_table* is a ``boto3.resource('dynamodb').Table`` instance.
+    * *ddb_table* is a table name or a ``boto3.resource('dynamodb').Table`` instance.
     * *key* is a mapping that identifies the item to update.
-    * *update_map* is a mapping of item attributes to target values.
+    * *update_map* is a mapping of top-level item attributes to target values.
     * *kwargs* are passed directly to the the ``Table.update_item`` method.
 
     Usage:
 
     .. code-block:: python
 
         from boto3 import resource as boto3_resource
@@ -82,31 +94,53 @@
     This function constructs equivalent ``UpdateExpression`` and
     ``ExpressionAttributeValues`` parameters.
 
     Equivalent to:
 
     .. code-block:: python
 
-        from boto3 import resource as boto3_resource
-
         ddb_resource = boto3_resource('dynamodb')
         ddb_table = ddb_resource.Table('example-table')
         key = {'username': 'janedoe', 'last_name': 'Doe'}
         resp = ddb_table.update_item(
             Key=key,
             UpdateExpression='SET age = :val1',
             ExpressionAttributeValues={':val1': 26},
         )
+
+    Note that nested attributes (i.e. map attributes) can be updated, but that you need
+    to provide values for the entire map.
+
+    .. code-block:: python
+
+        # Suppose that DDB had this before:
+        # {
+        #   "username": "janedoe",
+        #   "parameters": {
+        #     "age": 25,
+        #     "weight_kg": 70
+        #   }
+        # }
+        # After this call, `parameters.age` will be 26, but there will
+        # no longer be a `paramters.weight_kg`.
+
+        ddb_resource = boto3_resource('dynamodb')
+        ddb_table = ddb_resource.Table('example-table')
+        key = {'username': 'janedoe', 'last_name': 'Doe'}
+        update_map = {'parameters': {'age': 26}}
+        resp = update_attributes(ddb_table, key, update_map)
+
     """
+    t = _table_or_name(ddb_table)
     set_parts = []
     attrib_values = {}
     for i, (k, v) in enumerate(update_map.items(), 1):
         set_parts.append(f'{k} = :val{i}')
         attrib_values[f':val{i}'] = v
     set_stmt = ', '.join(set_parts)
 
-    return ddb_table.update_item(
+    return t.update_item(
         Key=key,
         UpdateExpression=f"SET {set_stmt}",
         ExpressionAttributeValues=attrib_values,
         **kwargs,
     )
```

### Comparing `boto3-helpers-1.3.0/boto3_helpers/events.py` & `boto3-helpers-1.4.0/boto3_helpers/events.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers/mediatailor.py` & `boto3-helpers-1.4.0/boto3_helpers/mediatailor.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers/pagination.py` & `boto3-helpers-1.4.0/boto3_helpers/pagination.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from jmespath import search as json_search
+
+
 def yield_all_items(boto_client, method_name, list_key, **kwargs):
     """A helper function that simplifies retrieving items from API endpoints that
     require paging. Yields each item from every page:
 
     * *boto_client* is a ``boto3.client()`` instance for the relevant service.
     * *method_name* is the name of the client method that requires paging.
     * *list_key* is the name of the top-level key in the method's response that
-      corresponds to the desired list of items.
+      corresponds to the desired list of items. If the method's response has multiple
+      levels, use a ``jmespath`` expression.
     * *kwargs* are passed through to the appropriate ``paginate`` method.
 
     EC2 example:
 
     .. code-block:: python
 
         from boto3 import client as boto3_client
@@ -39,11 +43,26 @@
             Bucket='example-bucket',
             Prefix='example-prefix/'
         ):
             print(item['Key'])
 
     In this example, the ``list_key`` for S3's ``list_objects_v2`` is ``'Contents'``.
 
+    CloudFront example:
+
+    .. code-block:: python
+
+        from boto3 import client as boto3_client
+        from boto3_helpers.pagination import yield_all_items
+
+        cloudfront_client = boto3_client('cloudfront')
+        for item in yield_all_items(
+            cloudfront_client,
+            'list_distributions',
+            'DistributionList.Items'
+        ):
+            print(item['Id'])
+
     """
     paginator = boto_client.get_paginator(method_name)
     for page in paginator.paginate(**kwargs):
-        yield from page.get(list_key, [])
+        yield from json_search(list_key, page) or []
```

### Comparing `boto3-helpers-1.3.0/boto3_helpers/s3.py` & `boto3-helpers-1.4.0/boto3_helpers/s3.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers/signed_requests.py` & `boto3-helpers-1.4.0/boto3_helpers/signed_requests.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers/sqs.py` & `boto3-helpers-1.4.0/boto3_helpers/sqs.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers/sts.py` & `boto3-helpers-1.4.0/boto3_helpers/sts.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/boto3_helpers.egg-info/PKG-INFO` & `boto3-helpers-1.4.0/boto3_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boto3-helpers
-Version: 1.3.0
+Version: 1.4.0
 Summary: Helper utilities for boto3
 Author: Bo Bayles
 Author-email: bo.bayles@wurl.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/openwurl/boto3-helpers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boto3-helpers-1.3.0/boto3_helpers.egg-info/SOURCES.txt` & `boto3-helpers-1.4.0/boto3_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/setup.cfg` & `boto3-helpers-1.4.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = boto3-helpers
-version = 1.3.0
+version = 1.4.0
 description = Helper utilities for boto3
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Bo Bayles
 author_email = bo.bayles@wurl.com
 license = Apache 2.0
 license_files =
```

### Comparing `boto3-helpers-1.3.0/tests/test_arn.py` & `boto3-helpers-1.4.0/tests/test_arn.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/tests/test_awslambda.py` & `boto3-helpers-1.4.0/tests/test_awslambda.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/tests/test_cloudwatch.py` & `boto3-helpers-1.4.0/tests/test_cloudwatch.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/tests/test_dynamodb.py` & `boto3-helpers-1.4.0/tests/test_dynamodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from decimal import Decimal
 from unittest import TestCase
+from unittest.mock import patch
 
 from boto3.dynamodb.conditions import Attr as ddb_attr, Key as ddb_key
 from boto3 import resource as boto3_resource
 from botocore.stub import Stubber
 
 from boto3_helpers.dynamodb import query_table, scan_table, update_attributes
 
@@ -105,19 +106,20 @@
         expected = [
             {'username': 'ExampleUser', 'age': Decimal(26)},
             {'username': 'ExampleUser', 'age': Decimal(25)},
             {'username': 'ExampleUser', 'age': Decimal(24)},
         ]
         self.assertEqual(actual, expected)
 
-    def test_update_attributes(self):
+    @patch('boto3_helpers.dynamodb.boto3_resource', autospec=True)
+    def test_update_attributes(self, mock_boto3_resource):
         # Set up the stubber
         ddb_resource = boto3_resource('dynamodb', region_name='not-a-region')
-        ddb_table = ddb_resource.Table('test-table')
         stubber = Stubber(ddb_resource.meta.client)
+        mock_boto3_resource.return_value = ddb_resource
 
         # The function will create a string for UpdateExpression
         # and a dict for ExpressionAttributeValues
         update_resp = {
             'Attributes': {
                 'username': {'S': 'janedoe'},
                 'last_name': {'S': 'Doe'},
@@ -133,15 +135,15 @@
             'ReturnValues': 'ALL_NEW',
         }
         stubber.add_response('update_item', update_resp, update_params)
 
         # Do the deed
         with stubber:
             actual = update_attributes(
-                ddb_table,
+                'test-table',
                 {'username': 'janedoe', 'last_name': 'Doe'},
                 {'age': 26, 'weight_kg': 70},
                 ReturnValues='ALL_NEW',
             )
         expected = {
             'Attributes': {
                 'username': 'janedoe',
```

### Comparing `boto3-helpers-1.3.0/tests/test_events.py` & `boto3-helpers-1.4.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/tests/test_mediatailor.py` & `boto3-helpers-1.4.0/tests/test_mediatailor.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/tests/test_pagination.py` & `boto3-helpers-1.4.0/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/tests/test_s3.py` & `boto3-helpers-1.4.0/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/tests/test_signed_requests.py` & `boto3-helpers-1.4.0/tests/test_signed_requests.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/tests/test_sqs.py` & `boto3-helpers-1.4.0/tests/test_sqs.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.3.0/tests/test_sts.py` & `boto3-helpers-1.4.0/tests/test_sts.py`

 * *Files identical despite different names*

