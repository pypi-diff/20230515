# Comparing `tmp/deale_shared_library-0.0.5.tar.gz` & `tmp/deale_shared_library-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deale_shared_library-0.0.5.tar", last modified: Mon May 15 07:58:52 2023, max compression
+gzip compressed data, was "deale_shared_library-0.0.6.tar", last modified: Mon May 15 08:10:59 2023, max compression
```

## Comparing `deale_shared_library-0.0.5.tar` & `deale_shared_library-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 07:58:52.211422 deale_shared_library-0.0.5/
--rw-r--r--   0 caaarlxs   (501) staff       (20)     2155 2023-05-15 07:58:52.211295 deale_shared_library-0.0.5/PKG-INFO
--rw-r--r--   0 caaarlxs   (501) staff       (20)     1810 2023-05-15 07:57:56.000000 deale_shared_library-0.0.5/README.md
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 07:58:52.209858 deale_shared_library-0.0.5/deale_shared_library/
--rw-r--r--   0 caaarlxs   (501) staff       (20)     2292 2023-05-15 07:43:29.000000 deale_shared_library-0.0.5/deale_shared_library/Cognito.py
--rw-r--r--   0 caaarlxs   (501) staff       (20)     1550 2023-05-15 07:36:31.000000 deale_shared_library-0.0.5/deale_shared_library/DynamoDB.py
--rw-r--r--   0 caaarlxs   (501) staff       (20)     2034 2023-05-15 07:56:50.000000 deale_shared_library-0.0.5/deale_shared_library/Lambda.py
--rw-r--r--   0 caaarlxs   (501) staff       (20)        0 2023-05-11 07:15:28.000000 deale_shared_library-0.0.5/deale_shared_library/__init__.py
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 07:58:52.210489 deale_shared_library-0.0.5/deale_shared_library.egg-info/
--rw-r--r--   0 caaarlxs   (501) staff       (20)     2155 2023-05-15 07:58:52.000000 deale_shared_library-0.0.5/deale_shared_library.egg-info/PKG-INFO
--rw-r--r--   0 caaarlxs   (501) staff       (20)      430 2023-05-15 07:58:52.000000 deale_shared_library-0.0.5/deale_shared_library.egg-info/SOURCES.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)        1 2023-05-15 07:58:52.000000 deale_shared_library-0.0.5/deale_shared_library.egg-info/dependency_links.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)        6 2023-05-15 07:58:52.000000 deale_shared_library-0.0.5/deale_shared_library.egg-info/requires.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)       21 2023-05-15 07:58:52.000000 deale_shared_library-0.0.5/deale_shared_library.egg-info/top_level.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)       38 2023-05-15 07:58:52.211460 deale_shared_library-0.0.5/setup.cfg
--rw-r--r--   0 caaarlxs   (501) staff       (20)      538 2023-05-15 07:58:43.000000 deale_shared_library-0.0.5/setup.py
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 07:58:52.211001 deale_shared_library-0.0.5/tests/
--rw-r--r--   0 caaarlxs   (501) staff       (20)     1550 2023-05-15 07:33:55.000000 deale_shared_library-0.0.5/tests/test_Cognito.py
--rw-r--r--   0 caaarlxs   (501) staff       (20)     1233 2023-05-15 07:38:55.000000 deale_shared_library-0.0.5/tests/test_Dynamo.py
--rw-r--r--   0 caaarlxs   (501) staff       (20)      574 2023-05-15 07:56:23.000000 deale_shared_library-0.0.5/tests/test_Lambda.py
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 08:10:59.715542 deale_shared_library-0.0.6/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     2155 2023-05-15 08:10:59.715376 deale_shared_library-0.0.6/PKG-INFO
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1810 2023-05-15 07:57:56.000000 deale_shared_library-0.0.6/README.md
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 08:10:59.713817 deale_shared_library-0.0.6/deale_shared_library/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     2292 2023-05-15 07:43:29.000000 deale_shared_library-0.0.6/deale_shared_library/Cognito.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1414 2023-05-15 08:02:54.000000 deale_shared_library-0.0.6/deale_shared_library/DynamoDB.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     2034 2023-05-15 07:56:50.000000 deale_shared_library-0.0.6/deale_shared_library/Lambda.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        0 2023-05-11 07:15:28.000000 deale_shared_library-0.0.6/deale_shared_library/__init__.py
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 08:10:59.714426 deale_shared_library-0.0.6/deale_shared_library.egg-info/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     2155 2023-05-15 08:10:59.000000 deale_shared_library-0.0.6/deale_shared_library.egg-info/PKG-INFO
+-rw-r--r--   0 caaarlxs   (501) staff       (20)      430 2023-05-15 08:10:59.000000 deale_shared_library-0.0.6/deale_shared_library.egg-info/SOURCES.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        1 2023-05-15 08:10:59.000000 deale_shared_library-0.0.6/deale_shared_library.egg-info/dependency_links.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        6 2023-05-15 08:10:59.000000 deale_shared_library-0.0.6/deale_shared_library.egg-info/requires.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)       21 2023-05-15 08:10:59.000000 deale_shared_library-0.0.6/deale_shared_library.egg-info/top_level.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)       38 2023-05-15 08:10:59.715583 deale_shared_library-0.0.6/setup.cfg
+-rw-r--r--   0 caaarlxs   (501) staff       (20)      538 2023-05-15 08:03:19.000000 deale_shared_library-0.0.6/setup.py
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-15 08:10:59.715083 deale_shared_library-0.0.6/tests/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1550 2023-05-15 07:33:55.000000 deale_shared_library-0.0.6/tests/test_Cognito.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1233 2023-05-15 07:38:55.000000 deale_shared_library-0.0.6/tests/test_Dynamo.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)      574 2023-05-15 07:56:23.000000 deale_shared_library-0.0.6/tests/test_Lambda.py
```

### Comparing `deale_shared_library-0.0.5/PKG-INFO` & `deale_shared_library-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deale_shared_library
-Version: 0.0.5
+Version: 0.0.6
 Summary: A shared library for Deale microservices
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `deale_shared_library-0.0.5/README.md` & `deale_shared_library-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `deale_shared_library-0.0.5/deale_shared_library/Cognito.py` & `deale_shared_library-0.0.6/deale_shared_library/Cognito.py`

 * *Files identical despite different names*

### Comparing `deale_shared_library-0.0.5/deale_shared_library/DynamoDB.py` & `deale_shared_library-0.0.6/deale_shared_library/DynamoDB.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 import boto3
 from boto3.dynamodb.conditions import Attr, Key
 
+resource = boto3.resource("dynamodb", region_name="eu-west-1")
+
 
 class DynamoDB:
     """
     A class to handle operations on AWS DynamoDB tables.
     """
 
-    def __init__(self):
-        """
-        Initialize a DynamoDB resource for a specific AWS region.
-
-        :param region_name: The name of the AWS region.
-        """
-        self.dynamodb = boto3.resource("dynamodb", region_name="eu-west-1")
-
-    def scan(self, table_name, **kwargs):
+    @staticmethod
+    def scan(table_name, **kwargs):
         """
         Scan a DynamoDB table.
 
         :param table_name: The name of the DynamoDB table.
         :param **kwargs: Any keyword arguments accepted by the boto3 Table.scan() method.
         :return: The response from the scan operation.
         """
-        table = self.dynamodb.Table(table_name)
+        table = resource.dynamodb.Table(table_name)
         return table.scan(**kwargs)
 
-    def query(self, table_name, **kwargs):
+    @staticmethod
+    def query(table_name, **kwargs):
         """
         Query a DynamoDB table.
 
         :param table_name: The name of the DynamoDB table.
         :param **kwargs: Any keyword arguments accepted by the boto3 Table.query() method.
         :return: The response from the query operation.
         """
-        table = self.dynamodb.Table(table_name)
+        table = resource.dynamodb.Table(table_name)
         return table.query(**kwargs)
 
-    def put_item(self, table_name, item):
+    @staticmethod
+    def put_item(table_name, item):
         """
         Put an item into a DynamoDB table.
 
         :param table_name: The name of the DynamoDB table.
         :param item: The item to put into the table.
         :return: The response from the put_item operation.
         """
-        table = self.dynamodb.Table(table_name)
+        table = resource.dynamodb.Table(table_name)
         return table.put_item(Item=item)
```

### Comparing `deale_shared_library-0.0.5/deale_shared_library/Lambda.py` & `deale_shared_library-0.0.6/deale_shared_library/Lambda.py`

 * *Files identical despite different names*

### Comparing `deale_shared_library-0.0.5/deale_shared_library.egg-info/PKG-INFO` & `deale_shared_library-0.0.6/deale_shared_library.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deale-shared-library
-Version: 0.0.5
+Version: 0.0.6
 Summary: A shared library for Deale microservices
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `deale_shared_library-0.0.5/setup.py` & `deale_shared_library-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="deale_shared_library",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     description="A shared library for Deale microservices",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=["boto3"],
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `deale_shared_library-0.0.5/tests/test_Cognito.py` & `deale_shared_library-0.0.6/tests/test_Cognito.py`

 * *Files identical despite different names*

### Comparing `deale_shared_library-0.0.5/tests/test_Dynamo.py` & `deale_shared_library-0.0.6/tests/test_Dynamo.py`

 * *Files identical despite different names*

### Comparing `deale_shared_library-0.0.5/tests/test_Lambda.py` & `deale_shared_library-0.0.6/tests/test_Lambda.py`

 * *Files identical despite different names*

