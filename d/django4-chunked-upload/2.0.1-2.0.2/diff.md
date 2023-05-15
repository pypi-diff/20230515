# Comparing `tmp/django4-chunked-upload-2.0.1.tar.gz` & `tmp/django4-chunked-upload-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django4-chunked-upload-2.0.1.tar", last modified: Sun May 14 04:29:07 2023, max compression
+gzip compressed data, was "django4-chunked-upload-2.0.2.tar", last modified: Mon May 15 06:47:13 2023, max compression
```

## Comparing `django4-chunked-upload-2.0.1.tar` & `django4-chunked-upload-2.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 04:29:07.554982 django4-chunked-upload-2.0.1/
--rw-rw-rw-   0        0        0      934 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       64 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5747 2023-05-14 04:29:07.554982 django4-chunked-upload-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5196 2023-05-14 04:28:56.000000 django4-chunked-upload-2.0.1/README.rst
--rw-rw-rw-   0        0        0        7 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/VERSION.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 04:29:07.522527 django4-chunked-upload-2.0.1/chunked_upload/
--rw-rw-rw-   0        0        0       21 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/__init__.py
--rw-rw-rw-   0        0        0      325 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/admin.py
--rw-rw-rw-   0        0        0      317 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/constants.py
--rw-rw-rw-   0        0        0      275 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:29:07.524524 django4-chunked-upload-2.0.1/chunked_upload/management/
--rw-rw-rw-   0        0        0        0 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:29:07.527497 django4-chunked-upload-2.0.1/chunked_upload/management/commands/
--rw-rw-rw-   0        0        0        0 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1776 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/management/commands/delete_expired_uploads.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:29:07.530990 django4-chunked-upload-2.0.1/chunked_upload/migrations/
--rw-rw-rw-   0        0        0     1830 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/migrations/__init__.py
--rw-rw-rw-   0        0        0     3561 2023-05-14 03:51:53.000000 django4-chunked-upload-2.0.1/chunked_upload/models.py
--rw-rw-rw-   0        0        0      392 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/response.py
--rw-rw-rw-   0        0        0     2334 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/settings.py
--rw-rw-rw-   0        0        0      115 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/tests.py
--rw-rw-rw-   0        0        0    11190 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.1/chunked_upload/views.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:29:07.551975 django4-chunked-upload-2.0.1/django4_chunked_upload.egg-info/
--rw-rw-rw-   0        0        0     5747 2023-05-14 04:29:07.000000 django4-chunked-upload-2.0.1/django4_chunked_upload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2023-05-14 04:29:07.000000 django4-chunked-upload-2.0.1/django4_chunked_upload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 04:29:07.000000 django4-chunked-upload-2.0.1/django4_chunked_upload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-14 04:29:07.000000 django4-chunked-upload-2.0.1/django4_chunked_upload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2023-05-14 04:29:07.556974 django4-chunked-upload-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-05-14 04:21:49.000000 django4-chunked-upload-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:47:13.149575 django4-chunked-upload-2.0.2/
+-rw-rw-rw-   0        0        0      934 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       64 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5747 2023-05-15 06:47:13.149575 django4-chunked-upload-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5196 2023-05-14 04:28:56.000000 django4-chunked-upload-2.0.2/README.rst
+-rw-rw-rw-   0        0        0        7 2023-05-15 06:35:12.000000 django4-chunked-upload-2.0.2/VERSION.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 06:47:13.113576 django4-chunked-upload-2.0.2/chunked_upload/
+-rw-rw-rw-   0        0        0       21 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/__init__.py
+-rw-rw-rw-   0        0        0      325 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/admin.py
+-rw-rw-rw-   0        0        0      317 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/constants.py
+-rw-rw-rw-   0        0        0      275 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:47:13.116580 django4-chunked-upload-2.0.2/chunked_upload/management/
+-rw-rw-rw-   0        0        0        0 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:47:13.124576 django4-chunked-upload-2.0.2/chunked_upload/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1776 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/management/commands/delete_expired_uploads.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:47:13.133574 django4-chunked-upload-2.0.2/chunked_upload/migrations/
+-rw-rw-rw-   0        0        0     1830 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3578 2023-05-15 06:27:51.000000 django4-chunked-upload-2.0.2/chunked_upload/models.py
+-rw-rw-rw-   0        0        0      392 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/response.py
+-rw-rw-rw-   0        0        0     2416 2023-05-15 06:27:13.000000 django4-chunked-upload-2.0.2/chunked_upload/settings.py
+-rw-rw-rw-   0        0        0      115 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/tests.py
+-rw-rw-rw-   0        0        0    11190 2023-05-14 03:26:16.000000 django4-chunked-upload-2.0.2/chunked_upload/views.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:47:13.147576 django4-chunked-upload-2.0.2/django4_chunked_upload.egg-info/
+-rw-rw-rw-   0        0        0     5747 2023-05-15 06:47:12.000000 django4-chunked-upload-2.0.2/django4_chunked_upload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2023-05-15 06:47:12.000000 django4-chunked-upload-2.0.2/django4_chunked_upload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 06:47:12.000000 django4-chunked-upload-2.0.2/django4_chunked_upload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-15 06:47:12.000000 django4-chunked-upload-2.0.2/django4_chunked_upload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       87 2023-05-15 06:47:13.152576 django4-chunked-upload-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-05-14 04:21:49.000000 django4-chunked-upload-2.0.2/setup.py
```

### Comparing `django4-chunked-upload-2.0.1/LICENSE.txt` & `django4-chunked-upload-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django4-chunked-upload-2.0.1/PKG-INFO` & `django4-chunked-upload-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django4-chunked-upload
-Version: 2.0.1
+Version: 2.0.2
 Summary: Upload large files to Django in multiple chunks, with the ability to resume if the upload is interrupted. Updated to support newer versions on Django. Based on the project of Julio M Alegria.
 Home-page: https://github.com/fredito1212/django-chunked-upload
-Download-URL: https://github.com/fredito1212/django-chunked-upload/tarball/2.0.1
+Download-URL: https://github.com/fredito1212/django-chunked-upload/tarball/2.0.2
 Author: Julio M Alegria & Jesus A Bravo
 Author-email: isc.alfredobravo@gmail.com
 License: MIT-Zero
 License-File: LICENSE.txt
 
 django-chunked-upload
 =====================
```

### Comparing `django4-chunked-upload-2.0.1/README.rst` & `django4-chunked-upload-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django4-chunked-upload-2.0.1/chunked_upload/management/commands/delete_expired_uploads.py` & `django4-chunked-upload-2.0.2/chunked_upload/management/commands/delete_expired_uploads.py`

 * *Files identical despite different names*

### Comparing `django4-chunked-upload-2.0.1/chunked_upload/migrations/0001_initial.py` & `django4-chunked-upload-2.0.2/chunked_upload/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django4-chunked-upload-2.0.1/chunked_upload/models.py` & `django4-chunked-upload-2.0.2/chunked_upload/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import uuid
 
 from django.db import models
 from django.conf import settings
 from django.core.files.uploadedfile import UploadedFile
 from django.utils import timezone
 
-from .settings import EXPIRATION_DELTA, UPLOAD_TO, STORAGE, DEFAULT_MODEL_USER_FIELD_NULL, DEFAULT_MODEL_USER_FIELD_BLANK
+from .settings import EXPIRATION_DELTA, UPLOAD_TO, STORAGE, DEFAULT_MODEL_USER_FIELD_NULL, DEFAULT_MODEL_USER_FIELD_BLANK, DEFAULT_CUSTOM_USER_MODEL
 from .constants import CHUNKED_UPLOAD_CHOICES, UPLOADING
 
 
 def generate_upload_id():
     return uuid.uuid4().hex
 
 def getUserModel():
-    if settings.CUSTOM_USER_MODEL:
-        return settings.CHUNKED_CUSTOM_USER_MODEL
+    if DEFAULT_CUSTOM_USER_MODEL:
+        return DEFAULT_CUSTOM_USER_MODEL
     else:
         return settings.AUTH_USER_MODEL
 
 
 class AbstractChunkedUpload(models.Model):
     """
     Base chunked upload model. This model is abstract (doesn't create a table
```

### Comparing `django4-chunked-upload-2.0.1/chunked_upload/settings.py` & `django4-chunked-upload-2.0.2/chunked_upload/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,7 +53,8 @@
 # Max amount of data (in bytes) that can be uploaded. `None` means no limit
 DEFAULT_MAX_BYTES = None
 MAX_BYTES = getattr(settings, 'CHUNKED_UPLOAD_MAX_BYTES', DEFAULT_MAX_BYTES)
 
 # determine the "null" and "blank" properties of "user" field in the "ChunkedUpload" model
 DEFAULT_MODEL_USER_FIELD_NULL = getattr(settings, 'CHUNKED_UPLOAD_MODEL_USER_FIELD_NULL', True)
 DEFAULT_MODEL_USER_FIELD_BLANK = getattr(settings, 'CHUNKED_UPLOAD_MODEL_USER_FIELD_BLANK', True)
+DEFAULT_CUSTOM_USER_MODEL = getattr(settings, 'CHUNKED_CUSTOM_USER_MODEL', None)
```

### Comparing `django4-chunked-upload-2.0.1/chunked_upload/views.py` & `django4-chunked-upload-2.0.2/chunked_upload/views.py`

 * *Files identical despite different names*

### Comparing `django4-chunked-upload-2.0.1/django4_chunked_upload.egg-info/PKG-INFO` & `django4-chunked-upload-2.0.2/django4_chunked_upload.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django4-chunked-upload
-Version: 2.0.1
+Version: 2.0.2
 Summary: Upload large files to Django in multiple chunks, with the ability to resume if the upload is interrupted. Updated to support newer versions on Django. Based on the project of Julio M Alegria.
 Home-page: https://github.com/fredito1212/django-chunked-upload
-Download-URL: https://github.com/fredito1212/django-chunked-upload/tarball/2.0.1
+Download-URL: https://github.com/fredito1212/django-chunked-upload/tarball/2.0.2
 Author: Julio M Alegria & Jesus A Bravo
 Author-email: isc.alfredobravo@gmail.com
 License: MIT-Zero
 License-File: LICENSE.txt
 
 django-chunked-upload
 =====================
```

### Comparing `django4-chunked-upload-2.0.1/django4_chunked_upload.egg-info/SOURCES.txt` & `django4-chunked-upload-2.0.2/django4_chunked_upload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django4-chunked-upload-2.0.1/setup.py` & `django4-chunked-upload-2.0.2/setup.py`

 * *Files identical despite different names*

