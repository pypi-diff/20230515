# Comparing `tmp/numbers-c2pa-0.0.5.tar.gz` & `tmp/numbers-c2pa-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/numbers-c2pa/numbers-c2pa/dist/.tmp-7t903ixl/numbers-c2pa-0.0.5.tar", last modified: Thu May  4 09:48:52 2023, max compression
+gzip compressed data, was "/home/runner/work/numbers-c2pa/numbers-c2pa/dist/.tmp-u5ex6h_3/numbers-c2pa-0.0.6.tar", last modified: Mon May 15 10:34:39 2023, max compression
```

## Comparing `numbers-c2pa-0.0.5.tar` & `numbers-c2pa-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 09:48:36.000000 numbers-c2pa-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-04 09:48:36.000000 numbers-c2pa-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 09:48:36.000000 numbers-c2pa-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 09:48:36.000000 numbers-c2pa-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/src/numbers_c2pa/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-04 09:48:36.000000 numbers-c2pa-0.0.5/src/numbers_c2pa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-04 09:48:36.000000 numbers-c2pa-0.0.5/src/numbers_c2pa/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 09:48:36.000000 numbers-c2pa-0.0.5/src/numbers_c2pa/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-04 09:48:36.000000 numbers-c2pa-0.0.5/src/numbers_c2pa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/src/numbers_c2pa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/src/numbers_c2pa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/src/numbers_c2pa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/src/numbers_c2pa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/src/numbers_c2pa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/src/numbers_c2pa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/src/numbers_c2pa.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:48:52.000000 numbers-c2pa-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 09:48:36.000000 numbers-c2pa-0.0.5/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/tests/test_core.py
```

### Comparing `numbers-c2pa-0.0.5/LICENSE` & `numbers-c2pa-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.5/PKG-INFO` & `numbers-c2pa-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.5
+Version: 0.0.6
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `numbers-c2pa-0.0.5/README.md` & `numbers-c2pa-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.5/setup.cfg` & `numbers-c2pa-0.0.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = numbers-c2pa
-version = 0.0.5
+version = 0.0.6
 author = Numbers Co., Inc
 author_email = dev@numbersprotocol.io
 description = Numbers C2PA tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = authenticity
 url = https://github.com/numbersprotocol/numbers-c2pa
```

### Comparing `numbers-c2pa-0.0.5/src/numbers_c2pa/__init__.py` & `numbers-c2pa-0.0.6/src/numbers_c2pa/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from .core import (create_c2pa_manifest, inject, inject_file, read_c2pa,
-                   read_c2pa_file)
+from .core import (create_c2pa_manifest, create_custom_c2pa_manifest, inject,
+                   inject_file, read_c2pa, read_c2pa_file)
 from .exceptions import NoClaimFound, UnknownError
 from .utils import (create_es256_private_key_file,
                     create_self_signed_certificate, generate_es256_private_key)
 
 __all__ = [
     'create_c2pa_manifest',
+    'create_custom_c2pa_manifest',
     'inject',
     'inject_file',
     'read_c2pa',
     'read_c2pa_file',
     'create_es256_private_key_file',
     'create_self_signed_certificate',
     'generate_es256_private_key',
```

### Comparing `numbers-c2pa-0.0.5/src/numbers_c2pa/core.py` & `numbers-c2pa-0.0.6/src/numbers_c2pa/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import mimetypes
 import os
 import subprocess
 from datetime import datetime
 from tempfile import NamedTemporaryFile, TemporaryDirectory
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 from .exceptions import NoClaimFound, UnknownError
 
 
 def _mimetype_to_ext(asset_mime_type: str):
     ext = mimetypes.guess_extension(asset_mime_type)
     if not ext:
@@ -21,20 +21,22 @@
     creator_public_key: str,
     asset_hash: str,
     date_created: datetime,
     location_created: str,
     date_captured: Optional[datetime],
     alg: str = 'es256',
     ta_url: str = 'http://timestamp.digicert.com',
+    vendor: str = 'numbersprotocol',
     claim_generator: str = 'Numbers_Protocol',
 ):
     captureTimestamp = date_captured.timestamp() if date_captured else None
     manifest = {
         'alg': alg,
         'ta_url': ta_url,
+        'vendor': vendor,
         'claim_generator': claim_generator,
         'title': nid,
         'assertions': [
             {
                 'label': 'stds.schema-org.CreativeWork',
                 'data': {
                     '@context': 'https://schema.org',
@@ -60,14 +62,67 @@
                 }
             }
         ]
     }
     return manifest
 
 
+def create_custom_c2pa_manifest(
+    alg: str = 'es256',
+    ta_url: str = 'http://timestamp.digicert.com',
+    vendor: str = 'numbersprotocol',
+    claim_generator: str = 'Numbers_Protocol',
+    title: Optional[str] = None,
+    author_type: str = 'Person',
+    author_credential: Optional[List] = None,
+    author_identifier: Optional[str] = None,
+    author_name: Optional[str] = None,
+    c2pa_actions: Optional[List] = None,
+    custom_assertions: Optional[List] = None,
+):
+    manifest = {
+        'alg': alg,
+        'ta_url': ta_url,
+        'vendor': vendor,
+        'claim_generator': claim_generator,
+        'title': title,
+        'assertions': [
+            {
+                'label': 'stds.schema-org.CreativeWork',
+                'data': {
+                    '@context': 'https://schema.org',
+                    '@type': 'CreativeWork',
+                    'author': [
+                        {
+                            '@type': author_type,
+                            'credential': author_credential or [],
+                            'identifier': author_identifier,
+                            'name': author_name,
+                        }
+                    ],
+                }
+            },
+        ]
+    }
+    manifest = {k: v for k, v in manifest.items() if v is not None}
+    if c2pa_actions:
+        manifest['assertions'].append(
+            {
+                'label': 'c2pa.actions',
+                'data':
+                {
+                    'actions': c2pa_actions,
+                }
+            }
+        )
+    if custom_assertions:
+        manifest['assertions'] += custom_assertions
+    return manifest
+
+
 def inject(
     asset_bytes: bytes,
     asset_mime_type: str,
     manifest: Dict,
     private_key: Optional[str] = None,
     sign_cert: Optional[str] = None,
     force_overwrite: bool = True,
```

### Comparing `numbers-c2pa-0.0.5/src/numbers_c2pa/utils.py` & `numbers-c2pa-0.0.6/src/numbers_c2pa/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import BinaryIO, Optional
+from typing import Optional
 
 from cryptography import x509
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.x509.oid import NameOID
 
 
@@ -34,16 +34,16 @@
     private_key = serialization.load_pem_private_key(
         private_key_pem,
         password=None,
     )
 
     subject = x509.Name([
         x509.NameAttribute(NameOID.COUNTRY_NAME, 'US'),
-        #x509.NameAttribute(NameOID.STATE_OR_PROVINCE_NAME, u"California"),
-        #x509.NameAttribute(NameOID.LOCALITY_NAME, u"San Francisco"),
+        # x509.NameAttribute(NameOID.STATE_OR_PROVINCE_NAME, u"California"),
+        # x509.NameAttribute(NameOID.LOCALITY_NAME, u"San Francisco"),
         x509.NameAttribute(NameOID.ORGANIZATION_NAME, 'Numbers Protocol'),
         x509.NameAttribute(NameOID.COMMON_NAME, 'numbersprotocol.io'),
     ])
 
     certificate = (
         x509.CertificateBuilder()
         .subject_name(subject)
```

### Comparing `numbers-c2pa-0.0.5/src/numbers_c2pa.egg-info/PKG-INFO` & `numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.5
+Version: 0.0.6
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

