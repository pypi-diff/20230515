# Comparing `tmp/deale_shared_library-0.0.3.tar.gz` & `tmp/deale_shared_library-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deale_shared_library-0.0.3.tar", last modified: Fri May 12 08:16:17 2023, max compression
+gzip compressed data, was "deale_shared_library-0.0.4.tar", last modified: Mon May 15 07:49:41 2023, max compression
```

## Comparing `deale_shared_library-0.0.3.tar` & `deale_shared_library-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-12 08:16:17.510661 deale_shared_library-0.0.3/
--rw-r--r--   0 caaarlxs   (501) staff       (20)      347 2023-05-12 08:16:17.510512 deale_shared_library-0.0.3/PKG-INFO
--rw-r--r--   0 caaarlxs   (501) staff       (20)        2 2023-05-11 08:12:29.000000 deale_shared_library-0.0.3/README.md
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-12 08:16:17.508822 deale_shared_library-0.0.3/deale_shared_library/
--rw-r--r--   0 caaarlxs   (501) staff       (20)     1571 2023-05-12 08:12:54.000000 deale_shared_library-0.0.3/deale_shared_library/DynamoDB.py
--rw-r--r--   0 caaarlxs   (501) staff       (20)     5412 2023-05-11 07:52:30.000000 deale_shared_library-0.0.3/deale_shared_library/DynamoDB_test.py
--rw-r--r--   0 caaarlxs   (501) staff       (20)        0 2023-05-11 07:15:28.000000 deale_shared_library-0.0.3/deale_shared_library/__init__.py
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-12 08:16:17.510164 deale_shared_library-0.0.3/deale_shared_library.egg-info/
--rw-r--r--   0 caaarlxs   (501) staff       (20)      347 2023-05-12 08:16:17.000000 deale_shared_library-0.0.3/deale_shared_library.egg-info/PKG-INFO
--rw-r--r--   0 caaarlxs   (501) staff       (20)      313 2023-05-12 08:16:17.000000 deale_shared_library-0.0.3/deale_shared_library.egg-info/SOURCES.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)        1 2023-05-12 08:16:17.000000 deale_shared_library-0.0.3/deale_shared_library.egg-info/dependency_links.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)       21 2023-05-12 08:16:17.000000 deale_shared_library-0.0.3/deale_shared_library.egg-info/top_level.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)       38 2023-05-12 08:16:17.510705 deale_shared_library-0.0.3/setup.cfg
--rw-r--r--   0 caaarlxs   (501) staff       (20)      582 2023-05-12 08:14:12.000000 deale_shared_library-0.0.3/setup.py
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-12 08:16:17.510339 deale_shared_library-0.0.3/tests/
--rw-r--r--   0 caaarlxs   (501) staff       (20)        0 2023-05-11 07:15:46.000000 deale_shared_library-0.0.3/tests/tests.py
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 07:49:41.594572 deale_shared_library-0.0.4/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1745 2023-05-15 07:49:41.594449 deale_shared_library-0.0.4/PKG-INFO
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1400 2023-05-15 07:48:21.000000 deale_shared_library-0.0.4/README.md
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 07:49:41.593366 deale_shared_library-0.0.4/deale_shared_library/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     2292 2023-05-15 07:43:29.000000 deale_shared_library-0.0.4/deale_shared_library/Cognito.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1550 2023-05-15 07:36:31.000000 deale_shared_library-0.0.4/deale_shared_library/DynamoDB.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        0 2023-05-11 07:15:28.000000 deale_shared_library-0.0.4/deale_shared_library/__init__.py
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 07:49:41.593942 deale_shared_library-0.0.4/deale_shared_library.egg-info/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1745 2023-05-15 07:49:41.000000 deale_shared_library-0.0.4/deale_shared_library.egg-info/PKG-INFO
+-rw-r--r--   0 caaarlxs   (501) staff       (20)      378 2023-05-15 07:49:41.000000 deale_shared_library-0.0.4/deale_shared_library.egg-info/SOURCES.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        1 2023-05-15 07:49:41.000000 deale_shared_library-0.0.4/deale_shared_library.egg-info/dependency_links.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        6 2023-05-15 07:49:41.000000 deale_shared_library-0.0.4/deale_shared_library.egg-info/requires.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)       21 2023-05-15 07:49:41.000000 deale_shared_library-0.0.4/deale_shared_library.egg-info/top_level.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)       38 2023-05-15 07:49:41.594609 deale_shared_library-0.0.4/setup.cfg
+-rw-r--r--   0 caaarlxs   (501) staff       (20)      538 2023-05-15 07:49:26.000000 deale_shared_library-0.0.4/setup.py
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 07:49:41.594265 deale_shared_library-0.0.4/tests/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1550 2023-05-15 07:33:55.000000 deale_shared_library-0.0.4/tests/test_Cognito.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1233 2023-05-15 07:38:55.000000 deale_shared_library-0.0.4/tests/test_Dynamo.py
```

### Comparing `deale_shared_library-0.0.3/deale_shared_library/DynamoDB.py` & `deale_shared_library-0.0.4/deale_shared_library/DynamoDB.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import boto3
 from boto3.dynamodb.conditions import Attr, Key
 
 
-class DynamoDBHandler:
+class DynamoDB:
     """
     A class to handle operations on AWS DynamoDB tables.
     """
-    
+
     def __init__(self):
         """
         Initialize a DynamoDB resource for a specific AWS region.
 
         :param region_name: The name of the AWS region.
         """
-        self.dynamodb = boto3.resource('dynamodb', region_name='eu-west-1')
-    
+        self.dynamodb = boto3.resource("dynamodb", region_name="eu-west-1")
 
     def scan(self, table_name, **kwargs):
         """
         Scan a DynamoDB table.
 
         :param table_name: The name of the DynamoDB table.
         :param **kwargs: Any keyword arguments accepted by the boto3 Table.scan() method.
@@ -33,19 +32,18 @@
 
         :param table_name: The name of the DynamoDB table.
         :param **kwargs: Any keyword arguments accepted by the boto3 Table.query() method.
         :return: The response from the query operation.
         """
         table = self.dynamodb.Table(table_name)
         return table.query(**kwargs)
-    
+
     def put_item(self, table_name, item):
         """
         Put an item into a DynamoDB table.
 
         :param table_name: The name of the DynamoDB table.
         :param item: The item to put into the table.
         :return: The response from the put_item operation.
         """
         table = self.dynamodb.Table(table_name)
         return table.put_item(Item=item)
-
```

### Comparing `deale_shared_library-0.0.3/setup.py` & `deale_shared_library-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from setuptools import find_packages, setup
 
 setup(
     name="deale_shared_library",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     description="A shared library for Deale microservices",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    install_requires=[
-        # List your library dependencies here
-    ],
+    install_requires=["boto3"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
     ],
 )
```

