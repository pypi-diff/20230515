# Comparing `tmp/drive-0.4.0.tar.gz` & `tmp/drive-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive-0.4.0.tar", max compression
+gzip compressed data, was "drive-0.4.1.tar", max compression
```

## Comparing `drive-0.4.0.tar` & `drive-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1069 2022-10-12 17:11:58.162482 drive-0.4.0/LICENSE
--rw-r--r--   0        0        0     3681 2022-10-12 17:11:58.162482 drive-0.4.0/README.md
--rw-r--r--   0        0        0      128 2022-10-12 17:11:58.162482 drive-0.4.0/drive/__init__.py
--rw-r--r--   0        0        0     1178 2022-10-12 17:11:58.162482 drive-0.4.0/drive/auth.py
--rw-r--r--   0        0        0    17207 2022-10-12 17:11:58.162482 drive-0.4.0/drive/client.py
--rw-r--r--   0        0        0      124 2022-10-12 17:11:58.166482 drive-0.4.0/drive/exceptions.py
--rw-r--r--   0        0        0     8972 2022-10-12 17:11:58.166482 drive-0.4.0/drive/files.py
--rw-r--r--   0        0        0     1076 2022-10-12 17:11:58.166482 drive-0.4.0/drive/mimetypes.py
--rw-r--r--   0        0        0        0 2022-10-12 17:11:58.166482 drive-0.4.0/drive/py.typed
--rw-r--r--   0        0        0      893 2022-10-12 17:11:58.166482 drive-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 drive-0.4.0/setup.py
--rw-r--r--   0        0        0     4488 1970-01-01 00:00:00.000000 drive-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-15 10:18:02.983487 drive-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4045 2023-05-15 10:18:02.983487 drive-0.4.1/README.md
+-rw-r--r--   0        0        0      128 2023-05-15 10:18:02.983487 drive-0.4.1/drive/__init__.py
+-rw-r--r--   0        0        0     1178 2023-05-15 10:18:02.983487 drive-0.4.1/drive/auth.py
+-rw-r--r--   0        0        0    17494 2023-05-15 10:18:02.983487 drive-0.4.1/drive/client.py
+-rw-r--r--   0        0        0      124 2023-05-15 10:18:02.983487 drive-0.4.1/drive/exceptions.py
+-rw-r--r--   0        0        0     9562 2023-05-15 10:18:02.983487 drive-0.4.1/drive/files.py
+-rw-r--r--   0        0        0     1076 2023-05-15 10:18:02.983487 drive-0.4.1/drive/mimetypes.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:18:02.983487 drive-0.4.1/drive/py.typed
+-rw-r--r--   0        0        0     1053 2023-05-15 10:18:02.983487 drive-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 drive-0.4.1/PKG-INFO
```

### Comparing `drive-0.4.0/LICENSE` & `drive-0.4.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2016-2022 – Baptiste Fontaine
+Copyright © 2016-2023 – Baptiste Fontaine
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `drive-0.4.0/README.md` & `drive-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
     python -m pip install drive
 
 With Poetry:
 
     poetry add drive
 
+You also need to have `libmagic` installed to get automatic detection of uploaded files’ MIME types. If you don’t have
+it, you must provide the `original_mime_type` keyword argument when you upload a file.
+On Linux, if you do have `libmagic` but Python can’t see it, see this [StackOverflow question][so].
+
+[so]: https://stackoverflow.com/q/7880454/735926
+
 ## Usage
 
 The API exposes a client as `drive.client.Client` that manipulates instances of
 `drive.files.File`. A `File` represent a Google Drive file. Note that both
 regular files and directories are represented as `File`s, and a file can have
 multiple parent directories. You can check if a `File` is a directory using the
 `is_directory` attribute.
@@ -24,15 +30,14 @@
 
 By default, the client reads your service account key JSON file at the location
 given by the environment variable `GOOGLE_APPLICATION_CREDENTIALS`. You can
 override this behavior by passing it directly:
 
     client = Client("/path/to/your/service-account-key.json")
 
-
 See Google’s documentation on [how to create a service account key][k].
 
 [k]: https://cloud.google.com/iam/docs/creating-managing-service-account-keys
 
 ### Client
 
 High-level `Client` methods:
@@ -82,16 +87,16 @@
 
 # Uses credentials from the path in the environment variable
 # GOOGLE_APPLICATION_CREDENTIALS.
 cl = Client()
 
 # Get the root directory
 d = cl.root()
-print(d.is_directory) # True
-print(d.name) # e.g. "My Drive"
+print(d.is_directory)  # True
+print(d.name)  # e.g. "My Drive"
 
 # Get a directory's content
 for f in d.list():
     print(f.name)
 
 # Get a shared directory
 d = cl.get_shared_directory("My Shared Dir")
@@ -125,10 +130,10 @@
 cl = Client()
 # download a Drawing in a png image
 cl.download_file("11AASomeFileId", "localfile.png", "image/png")
 ```
 
 ## License
 
-Copyright © 2016-2022 Baptiste Fontaine
+Copyright © 2016-2023 Baptiste Fontaine
 
 Distributed under the MIT License.
```

### Comparing `drive-0.4.0/drive/auth.py` & `drive-0.4.1/drive/auth.py`

 * *Files identical despite different names*

### Comparing `drive-0.4.0/drive/client.py` & `drive-0.4.1/drive/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: UTF-8 -*-
 
 import io
 import os.path
 import random
 import sys
 import time
-from typing import Optional, List, Any, Tuple, Dict, cast, Iterable
+from typing import Optional, List, Any, Tuple, Dict, cast, Iterable, Union
 
 import httplib2  # type: ignore
 import openpyxl  # type: ignore
 from apiclient import discovery  # type: ignore
 from googleapiclient.errors import HttpError  # type: ignore
 from googleapiclient.http import MediaIoBaseDownload, MediaIoBaseUpload  # type: ignore
 
 from drive import mimetypes
 from drive.auth import authorize, get_credentials
 from drive.exceptions import FileNotFoundException
-from drive.files import File
+from drive.files import File, guess_original_mime_type
 
 # Retry transport and file IO errors.
 RETRYABLE_ERRORS = (httplib2.HttpLib2Error, IOError)
 # Default number of bytes to send/receive in each request.
 CHUNKSIZE = 2 * 1024 * 1024
 
 QueryClause = Tuple[str, str, Any]
@@ -68,14 +68,20 @@
     else:
         p = "%s %s %s" % (field, op, serialized_value)
     if negation:
         p = "not %s" % p
     return p
 
 
+def _resolve_parent_id(parent: Union[File, str]):
+    if isinstance(parent, File):
+        return parent.id
+    return parent
+
+
 def _serialize_query_value(value):
     """
     Serialize a query value.
     """
     if isinstance(value, bool):
         return "true" if value else "false"
 
@@ -126,46 +132,46 @@
 
             raise RuntimeError("Unable to find folder %s" % folder_name)
 
         return self.create_folder(folder_name, parent_id)
 
     def remove_file(self, file_id: str):
         """
-        Remove a file by its id.
+        Remove a file by its ID.
         """
         return self._files.delete(fileId=file_id).execute()
 
     def get_file_metadata(self, file_id, raise_if_not_found=True, **kw):
         try:
             return self._files.get(fileId=file_id, **kw).execute()
         except HttpError:
             if not raise_if_not_found:
                 return None
             raise
 
     def get_file(self, file_id: str, raise_if_not_found=True) -> Optional[File]:
         """
-        Get a file by its id.
+        Get a file by its ID.
 
         :param file_id:
         :param raise_if_not_found: if ``True`` (default), raise an exception if the file doesn’t exist
         """
         fm = self.get_file_metadata(file_id, raise_if_not_found)
         if fm:
             return File(fm, client=self)
         return None
 
     def get_file_by_name(self, name: str, parent_id: Optional[str] = None) -> Optional[File]:
         """
         Get a file by name.
-        Note that, unlike ids, names are not guaranteed to be unique: you can have multiple files with the same name
+        Note that, unlike IDs, names are not guaranteed to be unique: you can have multiple files with the same name
         on Google Drive.
 
         :param name: Drive filename
-        :param parent_id: optional parent id.
+        :param parent_id: optional parent ID.
         :raise: ``drive.exceptions.FileNotFoundException`` if the file doesn’t exist
         """
         ls = self.list_files(name_equals=name, n=1, parents_in=parent_id)
         if not ls:
             raise FileNotFoundException(name)
 
         return ls[0]
@@ -226,15 +232,15 @@
         """
         Retrieve a shared directory. This is a shortcut for ``get_shared_file(name, is_directory=True)``.
         """
         return self.get_shared_file(name, is_directory=True)
 
     def root(self) -> File:
         """
-        Return the root directory. Note the alias ``"root"`` works as an alias file id for the root directory.
+        Return the root directory. Note the alias ``"root"`` works as an alias file ID for the root directory.
         """
         return cast(File, self.get_file("root"))
 
     def list_files(self,
                    name_equals: Optional[str] = None,
                    name_contains: Optional[str] = None,
                    mimetype: Optional[str] = None,
@@ -264,18 +270,18 @@
                     add_parents_ids=None,
                     name: Optional[str] = None,
                     media=None,
                     force=False):
         """
         Update a file.
 
-        Note: calling this function with only a file id (e.g.: `update_file(my_id)`) without any modification is a no-op
+        Note: calling this function with only a file ID (e.g.: `update_file(my_id)`) without any modification is a no-op
           unless `force=True` is passed.
 
-        :param file_id: id of the file to update
+        :param file_id: ID of the file to update
         :param remove_parents_ids:
         :param add_parents_ids:
         :param name: new name of the file
         :param media:
         :param force: force update even if there are no modifications
         :return:
         """
@@ -297,17 +303,16 @@
         if media:
             kw["media_body"] = media
 
         return self._execute_file_request(self._files.update(fileId=file_id, **kw))
 
     def move_file_to_folder(self, file_id: str, folder_id: str):
         # Retrieve the existing parents to remove
-        resp = self._files.get(fileId=file_id, fields='parents').execute()
-
-        return self.update_file(file_id, add_parents_ids=[folder_id], remove_parents_ids=resp["parents"])
+        parent_ids = self._get_file_field(file_id, "parents")
+        return self.update_file(file_id, add_parents_ids=[folder_id], remove_parents_ids=parent_ids)
 
     def rename_file(self, file_id: str, name: str):
         """
         Rename a file.
         """
         return self.update_file(file_id, name=name)
 
@@ -336,118 +341,110 @@
         # bypass the downloader; there appear to be a bug for large files
         # noinspection PyProtectedMember
         writer.write(downloader._request.execute())
 
     def download_file(self, file_id: str, path: str, mime_type: Optional[str] = None) -> None:
         """
         Download a file and save it locally.
-        :param file_id: file id
+        :param file_id: file ID
         :param path: local path where to save the file.
         :param mime_type: optional mime type
         :return:
         """
         with open(path, "wb") as f:
             self.download(file_id, f, mime_type=mime_type)
 
     def download_excel_workbook(self, file_id: str, read_only=False):
         """
         Download a Google Spreadsheet as an openpyxl workbook.
+
         :param file_id:
         :param read_only: set this to ``True`` if you don't plan to save or edit the workbook.
         :return: ``openpyxl.Workbook`` object.
         """
         buff = io.BytesIO()
         self.download(file_id, buff, mimetypes.XLSX)
         buff.seek(0)
         return openpyxl.load_workbook(buff, read_only=read_only)
 
-    def upload(self, parent_id: str, name: str,
+    def upload(self, parent_id: Union[str, File], name: str,
                reader,
                mime_type: Optional[str] = None,
                original_mime_type: Optional[str] = None,
                update_existing=False,
                resumable=False):
         """
-
         :param parent_id:
         :param name: remote filename
         :param reader: binary file reader
-        :param mime_type:
-        :param original_mime_type:
+        :param mime_type: target MIME type.
+        :param original_mime_type: Original MIME type. If ``None``, it is determined using libmagic, which must be
+            installed.
         :param update_existing:
         :param resumable:
         :return:
         """
-
-        if isinstance(parent_id, File):
-            parent_id = parent_id.id
+        parent_id_str = _resolve_parent_id(parent_id)
 
         if not original_mime_type:
-            import magic
-            pos = reader.tell()
-            buff = reader.read(1024)
-            reader.seek(pos)
-            original_mime_type = magic.from_buffer(buff, mime=True)
+            original_mime_type = guess_original_mime_type(reader)
 
         media = MediaIoBaseUpload(reader, mimetype=original_mime_type,
                                   chunksize=CHUNKSIZE,
                                   resumable=resumable)
 
         if update_existing:
-            f = self.file_exists(name=name, parent_id=parent_id)
+            f = self.file_exists(name=name, parent_id=parent_id_str)
             if f:
                 return self.update_file(f.id, media=media)
 
         metadata = {
             'name': name,
-            'parents': [parent_id],
+            'parents': [parent_id_str],
         }
 
         if mime_type:
             metadata['mimeType'] = mime_type
 
         return self._execute_file_request(self._files.create(body=metadata,
                                                              media_body=media))
 
-    def upload_file(self, parent_id: str, path: str,
+    def upload_file(self, parent_id: Union[str, File], path: str,
                     name: Optional[str] = None,
                     mime_type: Optional[str] = None,
                     original_mime_type: Optional[str] = None,
                     update_existing=False):
         """
-
         :param parent_id:
         :param path: local path
         :param name: remote filename. If ``None``, use the local basename.
         :param mime_type:
-        :param original_mime_type:
+        :param original_mime_type: Original MIME type. If ``None``, it is determined using libmagic, which must be
+            installed.
         :param update_existing:
         :return:
         """
-        if isinstance(parent_id, File):
-            parent_id = parent_id.id
-
         if name is None:
             name = os.path.basename(path)
 
         with open(path, "rb") as f:
             return self.upload(parent_id, name, f, mime_type,
                                original_mime_type,
                                update_existing=update_existing)
 
     def upload_excel_workbook(self,
-                              parent: str,
+                              parent: Union[str, File],
                               name: str,
                               workbook: openpyxl.Workbook,
                               as_spreadsheet=True,
                               update_existing=False):
         """
         Upload an openpyxl (Excel) workbook and convert it to a Google Spreadsheet, unless ``as_spreadsheet`` is false.
 
-        :param parent: parent id
+        :param parent: parent ID
         :param name: remote filename
         :param workbook: ``openpyxl.Workbook`` object
         :param as_spreadsheet: if ``True`` (default), convert the document to a Google Spreadsheet
         :param update_existing:
         :return:
         """
         buff = io.BytesIO()
@@ -459,16 +456,19 @@
         return self.upload(parent, name, buff, target_mimetype,
                            mimetypes.XLSX, update_existing=update_existing)
 
     def grant_file_permissions(self, file_id: str, role: str, type_: str):
         return self._permissions.create(fileId=file_id, body={"role": role, "type": type_}).execute()
 
     def get_web_view_link(self, file_id: str) -> str:
-        resp = self._files.get(fileId=file_id, fields='webViewLink').execute()
-        return resp['webViewLink']
+        return self._get_file_field(file_id, "webViewLink")
+
+    def _get_file_field(self, file_id: str, field: str):
+        resp = self._files.get(fileId=file_id, fields=field).execute()
+        return resp[field]
 
     # Private API
 
     def _execute_file_request(self, req):
         if not req.resumable:
             resp = req.execute()
             if "files" in resp:
```

### Comparing `drive-0.4.0/drive/files.py` & `drive-0.4.1/drive/files.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: UTF-8 -*-
 
 import io
 import json
-from typing import Optional, Union, cast, Dict, Any
+from typing import Optional, Union, cast, Dict, Any, BinaryIO
 
 from openpyxl.workbook import Workbook  # type: ignore
 
 import drive
 from drive import mimetypes
 
 
@@ -327,7 +327,25 @@
         name = attrs.get("name")
         if name:
             self._name = name
 
         parents = attrs.get("parents")
         if parents:
             self.parents_ids = parents
+
+
+def guess_original_mime_type(reader: BinaryIO):
+    """
+    Guess the MIME type of the content in a reader. Read 1024 bits, then seek the reader back to its original position.
+    """
+    try:
+        import magic
+    except ImportError as e:
+        if str(e).startswith("failed to find libmagic"):
+            raise RuntimeError("original_mime_type is None and we can't guess it because libmagic is not installed.") \
+                from e
+        raise
+
+    pos = reader.tell()
+    buff = reader.read(1024)
+    reader.seek(pos)
+    return magic.from_buffer(buff, mime=True)
```

### Comparing `drive-0.4.0/drive/mimetypes.py` & `drive-0.4.1/drive/mimetypes.py`

 * *Files identical despite different names*

### Comparing `drive-0.4.0/pyproject.toml` & `drive-0.4.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [tool.poetry]
 name = "drive"
-version = "0.4.0"
+version = "0.4.1"
 description = "Google Drive client"
 authors = ["Baptiste Fontaine <b@ptistefontaine.fr>"]
 license = "MIT"
 include = ["drive/py.typed"]
 readme = "README.md"
 packages = [
     { include = "drive" },
 ]
 classifiers = [
     'License :: OSI Approved :: MIT License',
+    'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 google-api-python-client = "^2.64.0"
 httplib2 = "^0.20.4"
 oauth2client = "^4.1.3"
 openpyxl = "^3.0.10"
 python-magic = "^0.4.27"
+python-magic-bin = {version = "^0.4.14", platform = "windows"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 mypy = "^0"
 
 [tool.coverage.report]
```

### Comparing `drive-0.4.0/PKG-INFO` & `drive-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 Metadata-Version: 2.1
 Name: drive
-Version: 0.4.0
+Version: 0.4.1
 Summary: Google Drive client
 License: MIT
 Author: Baptiste Fontaine
 Author-email: b@ptistefontaine.fr
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: google-api-python-client (>=2.64.0,<3.0.0)
 Requires-Dist: httplib2 (>=0.20.4,<0.21.0)
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
+Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "windows"
 Description-Content-Type: text/markdown
 
 # Drive
 
 Google Drive client.
 
 ## Install
 
     python -m pip install drive
 
 With Poetry:
 
     poetry add drive
 
+You also need to have `libmagic` installed to get automatic detection of uploaded files’ MIME types. If you don’t have
+it, you must provide the `original_mime_type` keyword argument when you upload a file.
+On Linux, if you do have `libmagic` but Python can’t see it, see this [StackOverflow question][so].
+
+[so]: https://stackoverflow.com/q/7880454/735926
+
 ## Usage
 
 The API exposes a client as `drive.client.Client` that manipulates instances of
 `drive.files.File`. A `File` represent a Google Drive file. Note that both
 regular files and directories are represented as `File`s, and a file can have
 multiple parent directories. You can check if a `File` is a directory using the
 `is_directory` attribute.
@@ -46,15 +55,14 @@
 
 By default, the client reads your service account key JSON file at the location
 given by the environment variable `GOOGLE_APPLICATION_CREDENTIALS`. You can
 override this behavior by passing it directly:
 
     client = Client("/path/to/your/service-account-key.json")
 
-
 See Google’s documentation on [how to create a service account key][k].
 
 [k]: https://cloud.google.com/iam/docs/creating-managing-service-account-keys
 
 ### Client
 
 High-level `Client` methods:
@@ -104,16 +112,16 @@
 
 # Uses credentials from the path in the environment variable
 # GOOGLE_APPLICATION_CREDENTIALS.
 cl = Client()
 
 # Get the root directory
 d = cl.root()
-print(d.is_directory) # True
-print(d.name) # e.g. "My Drive"
+print(d.is_directory)  # True
+print(d.name)  # e.g. "My Drive"
 
 # Get a directory's content
 for f in d.list():
     print(f.name)
 
 # Get a shared directory
 d = cl.get_shared_directory("My Shared Dir")
@@ -147,11 +155,11 @@
 cl = Client()
 # download a Drawing in a png image
 cl.download_file("11AASomeFileId", "localfile.png", "image/png")
 ```
 
 ## License
 
-Copyright © 2016-2022 Baptiste Fontaine
+Copyright © 2016-2023 Baptiste Fontaine
 
 Distributed under the MIT License.
```

