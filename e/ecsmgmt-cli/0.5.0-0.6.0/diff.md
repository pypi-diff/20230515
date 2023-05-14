# Comparing `tmp/ecsmgmt_cli-0.5.0.tar.gz` & `tmp/ecsmgmt_cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecsmgmt_cli-0.5.0.tar", max compression
+gzip compressed data, was "ecsmgmt_cli-0.6.0.tar", max compression
```

## Comparing `ecsmgmt_cli-0.5.0.tar` & `ecsmgmt_cli-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    16725 2023-05-10 01:03:02.448024 ecsmgmt_cli-0.5.0/LICENSE
--rw-r--r--   0        0        0      641 2023-05-10 01:03:02.448024 ecsmgmt_cli-0.5.0/README.md
--rw-r--r--   0        0        0     1611 2023-05-10 01:03:02.448024 ecsmgmt_cli-0.5.0/ecsmgmt/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/__init__.py
--rw-r--r--   0        0        0     1111 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/callbacks.py
--rw-r--r--   0        0        0       85 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/const.py
--rw-r--r--   0        0        0     2704 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/core.py
--rw-r--r--   0        0        0      128 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/echo.py
--rw-r--r--   0        0        0      447 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/exceptions.py
--rw-r--r--   0        0        0      705 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/format.py
--rw-r--r--   0        0        0     1210 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/types.py
--rw-r--r--   0        0        0      246 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/__init__.py
--rw-r--r--   0        0        0      247 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/acl/__init__.py
--rw-r--r--   0        0        0      439 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/acl/get.py
--rw-r--r--   0        0        0     2071 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/acl/set.py
--rw-r--r--   0        0        0      705 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/chown.py
--rw-r--r--   0        0        0      960 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/create.py
--rw-r--r--   0        0        0      617 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/delete.py
--rw-r--r--   0        0        0      439 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/get.py
--rw-r--r--   0        0        0      518 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/list.py
--rw-r--r--   0        0        0      259 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/retention/__init__.py
--rw-r--r--   0        0        0      457 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/retention/get.py
--rw-r--r--   0        0        0      734 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/retention/set.py
--rw-r--r--   0        0        0      307 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/get_acl_permissions.py
--rw-r--r--   0        0        0      254 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/__init__.py
--rw-r--r--   0        0        0     1350 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/create.py
--rw-r--r--   0        0        0     2348 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/delete.py
--rw-r--r--   0        0        0     1164 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/list.py
--rw-r--r--   0        0        0      249 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/__init__.py
--rw-r--r--   0        0        0      913 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/create.py
--rw-r--r--   0        0        0      589 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/delete.py
--rw-r--r--   0        0        0      420 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/get.py
--rw-r--r--   0        0        0      482 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/list.py
--rw-r--r--   0        0        0     1942 2023-05-10 01:06:15.288843 ecsmgmt_cli-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 ecsmgmt_cli-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-05-10 01:03:02.448024 ecsmgmt_cli-0.6.0/LICENSE
+-rw-r--r--   0        0        0      641 2023-05-10 01:03:02.448024 ecsmgmt_cli-0.6.0/README.md
+-rw-r--r--   0        0        0     1611 2023-05-10 01:03:02.448024 ecsmgmt_cli-0.6.0/ecsmgmt/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/_util/__init__.py
+-rw-r--r--   0        0        0     1111 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/_util/callbacks.py
+-rw-r--r--   0        0        0       85 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/_util/const.py
+-rw-r--r--   0        0        0     2704 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/_util/core.py
+-rw-r--r--   0        0        0      128 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/_util/echo.py
+-rw-r--r--   0        0        0      447 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/_util/exceptions.py
+-rw-r--r--   0        0        0      705 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/_util/format.py
+-rw-r--r--   0        0        0     1210 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/_util/types.py
+-rw-r--r--   0        0        0      246 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/__init__.py
+-rw-r--r--   0        0        0      247 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/acl/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/acl/get.py
+-rw-r--r--   0        0        0     2071 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/acl/set.py
+-rw-r--r--   0        0        0      705 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/chown.py
+-rw-r--r--   0        0        0     1154 2023-05-14 22:23:07.238026 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/create.py
+-rw-r--r--   0        0        0      617 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/delete.py
+-rw-r--r--   0        0        0      439 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/get.py
+-rw-r--r--   0        0        0      641 2023-05-14 22:26:00.278726 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/list.py
+-rw-r--r--   0        0        0      259 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/retention/__init__.py
+-rw-r--r--   0        0        0      457 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/retention/get.py
+-rw-r--r--   0        0        0      734 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/bucket/retention/set.py
+-rw-r--r--   0        0        0      307 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/get_acl_permissions.py
+-rw-r--r--   0        0        0      254 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/secret_key/__init__.py
+-rw-r--r--   0        0        0     1350 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/secret_key/create.py
+-rw-r--r--   0        0        0     2348 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/secret_key/delete.py
+-rw-r--r--   0        0        0     1164 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/secret_key/list.py
+-rw-r--r--   0        0        0      249 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/user/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/user/create.py
+-rw-r--r--   0        0        0      589 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/user/delete.py
+-rw-r--r--   0        0        0      420 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/user/get.py
+-rw-r--r--   0        0        0      482 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.6.0/ecsmgmt/user/list.py
+-rw-r--r--   0        0        0     1942 2023-05-14 22:26:00.278726 ecsmgmt_cli-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 ecsmgmt_cli-0.6.0/PKG-INFO
```

### Comparing `ecsmgmt_cli-0.5.0/LICENSE` & `ecsmgmt_cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/README.md` & `ecsmgmt_cli-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/__init__.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/_util/callbacks.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/_util/callbacks.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/_util/core.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/_util/core.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/_util/format.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/_util/format.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/_util/types.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/_util/types.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/acl/set.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/bucket/acl/set.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/chown.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/bucket/chown.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/create.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/bucket/retention/set.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import click
 from ecsclient.common.exceptions import ECSClientException
 
-from .._util.echo import success
-from .._util.exceptions import EcsmgmtClickException
+from ..._util import types
+from ..._util.echo import success
+from ..._util.exceptions import EcsmgmtClickException
 
 
 @click.command()
 @click.argument('bucket-name', type=click.STRING)
+@click.argument('period', type=types.TIME)
 @click.pass_obj
-def cli(obj: dict, bucket_name: str):
-    """Create bucket
+def cli(obj: dict, bucket_name: str, period: int):
+    """Set bucket retention
     """
     client = obj['client']
     namespace = obj['namespace']
 
-    if len(bucket_name) > 255:
-        raise EcsmgmtClickException('Bucket name too long. Maximum allowed length is 255 chars.')
-    if not all(x.isalnum() or x == '.' or x == '-' or x == '_' for x in bucket_name):
-        raise EcsmgmtClickException('Bucket name contains invalid characters. Only alphanumeric, ".", "-" or "_" is allowed.')
-
     try:
-        client.bucket.create(bucket_name=bucket_name, namespace=namespace)
-        success(f'created bucket "{bucket_name}" in namespace "{namespace}"')
+        client.bucket.set_retention(bucket_name=bucket_name, namespace=namespace, period=period)
+        success(f'Set retention for bucket "{bucket_name}" to {period} seconds')
     except ECSClientException as e:
         raise EcsmgmtClickException(e.message)
```

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/delete.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/bucket/delete.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/list.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/bucket/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,11 +8,13 @@
 def cli(obj: dict):
     """List all buckets in namespace
     """
     client = obj['client']
     namespace = obj['namespace']
 
     bucket_request = client.bucket.list(namespace=namespace)
-    bucket_list = [(bucket['namespace'], bucket['name'], bucket['owner']) for bucket in bucket_request['object_bucket']]
-    headers = ['Namespace', 'Bucket Name', 'Owner']
+    bucket_list = [(bucket['namespace'], bucket['name'], bucket['owner'],
+                    '🔒 yes' if bucket['is_encryption_enabled'] == 'true' else '❌ no') for bucket in
+                   bucket_request['object_bucket']]
+    headers = ['Namespace', 'Bucket Name', 'Owner', 'Encrypted']
     table = pretty_table(bucket_list, headers)
     click.echo(table)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/create.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/secret_key/create.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/delete.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/secret_key/delete.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/list.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/secret_key/list.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/user/create.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/user/create.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/ecsmgmt/user/delete.py` & `ecsmgmt_cli-0.6.0/ecsmgmt/user/delete.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.5.0/pyproject.toml` & `ecsmgmt_cli-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecsmgmt-cli"
-version = "0.5.0"
+version = "0.6.0"
 description = "Small CLI tool for interacting with the ECS Management API"
 authors = ["Dominik Rimpf <dev@drimpf.de>"]
 license = "MPL-2.0"
 
 readme = "README.md"
 repository = "https://gitlab.com/domrim/ecsmgmt-cli"
 homepage = "https://gitlab.com/domrim/ecsmgmt-cli"
```

### Comparing `ecsmgmt_cli-0.5.0/PKG-INFO` & `ecsmgmt_cli-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecsmgmt-cli
-Version: 0.5.0
+Version: 0.6.0
 Summary: Small CLI tool for interacting with the ECS Management API
 Home-page: https://gitlab.com/domrim/ecsmgmt-cli
 License: MPL-2.0
 Author: Dominik Rimpf
 Author-email: dev@drimpf.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

