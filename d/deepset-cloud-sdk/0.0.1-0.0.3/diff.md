# Comparing `tmp/deepset_cloud_sdk-0.0.1.tar.gz` & `tmp/deepset_cloud_sdk-0.0.3.tar.gz`

## Comparing `deepset_cloud_sdk-0.0.1.tar` & `deepset_cloud_sdk-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,29 @@
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/assets/logo.png
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/__about__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/models.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/api/config.py
--rw-r--r--   0        0        0     6675 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/api/deepset_cloud_api.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/api/files.py
--rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/api/upload_sessions.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/service/files_service.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/workflows/__init__.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/workflows/async_client/files.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/workflows/sync_client/files.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/examples/README.md
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/examples/upload.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/examples/data/example.pdf
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/examples/data/example.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/examples/data/example.txt.meta.json
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/.gitignore
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/README.md
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/assets/logo.png
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/README.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/__init__.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/cli.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/models.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/api/config.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/api/deepset_cloud_api.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/api/files.py
+-rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/api/upload_sessions.py
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/s3/upload.py
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/service/files_service.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/workflows/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/workflows/async_client/__init__.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/workflows/async_client/files.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/workflows/sync_client/__init__.py
+-rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/workflows/sync_client/files.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/examples/cli/README.md
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/examples/data/example.pdf
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/examples/data/example.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/examples/data/example.txt.meta.json
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/examples/sdk/README.md
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/examples/sdk/upload.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/.gitignore
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/README.md
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.3/PKG-INFO
```

### Comparing `deepset_cloud_sdk-0.0.1/.pre-commit-config.yaml` & `deepset_cloud_sdk-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.1/assets/logo.png` & `deepset_cloud_sdk-0.0.3/assets/logo.png`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/api/deepset_cloud_api.py` & `deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/api/deepset_cloud_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,29 +64,29 @@
 
         :param config: CommonConfig object.
         """
         async with httpx.AsyncClient() as client:
             yield cls(config, client)
 
     async def get(
-        self, workspace_name: str, endpoint: str, params: Optional[Dict[str, Any]] = None, timeout: int = 20
+        self, workspace_name: str, endpoint: str, params: Optional[Dict[str, Any]] = None, timeout_s: int = 20
     ) -> Response:
         """Make a GET request to the deepset Cloud API.
 
         :param workspace_name: Name of the workspace to use.
         :param endpoint: Endpoint to call.
         :param params: Query parameters to pass.
-        :param timeout: Timeout in seconds.
+        :param timeout_s: Timeout in seconds.
         :return: Response object.
         """
         response = await self.client.get(
             f"{self.base_url(workspace_name)}/{endpoint}",
             params=params or {},
             headers=self.headers,
-            timeout=timeout,
+            timeout=timeout_s,
         )
         logger.debug(
             "Called deepset Cloud API",
             method="GET",
             workspace=workspace_name,
             endpoint=endpoint,
             params=params,
@@ -97,62 +97,62 @@
     async def post(
         self,
         workspace_name: str,
         endpoint: str,
         params: Optional[Dict[str, Any]] = None,
         data: Optional[Dict[str, Any]] = None,
         files: Optional[Dict[str, Any]] = None,
-        timeout: int = 20,
+        timeout_s: int = 20,
     ) -> Response:
         """Make a POST request to the deepset Cloud API.
 
         :param workspace_name: Name of the workspace to use.
         :param endpoint: Endpoint to call.
         :param params: Query parameters to pass.
         :param data: Data to pass.
         :param files: Files to pass.
-        :param timeout: Timeout in seconds.
+        :param timeout_s: Timeout in seconds.
         :return: Response object.
         """
         response = await self.client.post(
             f"{self.base_url(workspace_name)}/{endpoint}",
             params=params or {},
             json=data or {},
             files=files,
             headers=self.headers,
-            timeout=timeout,
+            timeout=timeout_s,
         )
         logger.debug(
             "Called deepset Cloud API",
             method="POST",
             workspace=workspace_name,
             endpoint=endpoint,
             data=data or {},
             files=files,
             status=response.status_code,
         )
         return response
 
     async def delete(
-        self, workspace_name: str, endpoint: str, params: Optional[Dict[str, Any]] = None, timeout: int = 20
+        self, workspace_name: str, endpoint: str, params: Optional[Dict[str, Any]] = None, timeout_s: int = 20
     ) -> Response:
         """
         Make a DELETE request to the deepset Cloud API.
 
         :param workspace_name: Name of the workspace to use.
         :param endpoint: Endpoint to call.
         :param params: Query parameters to pass.
-        :param timeout: Timeout in seconds.
+        :param timeout_s: Timeout in seconds.
         :return: Response object.
         """
         response = await self.client.delete(
             f"{self.base_url(workspace_name)}/{endpoint}",
             params=params or {},
             headers=self.headers,
-            timeout=timeout,
+            timeout=timeout_s,
         )
         logger.debug(
             "Called deepset Cloud API",
             method="DELETE",
             workspace=workspace_name,
             endpoint=endpoint,
             params=params,
@@ -162,31 +162,31 @@
 
     async def put(
         self,
         workspace_name: str,
         endpoint: str,
         params: Optional[Dict[str, Any]] = None,
         data: Optional[Dict[str, Any]] = None,
-        timeout: int = 20,
+        timeout_s: int = 20,
     ) -> Response:
         """Make a PUT request to the deepset Cloud API.
 
         :param workspace_name: Name of the workspace to use.
         :param endpoint: Endpoint to call.
         :param params: Query parameters to pass.
         :param data: Data to pass.
-        :param timeout: Timeout in seconds.
+        :param timeout_s: Timeout in seconds.
         :return: Response object.
         """
         response = await self.client.put(
             f"{self.base_url(workspace_name)}/{endpoint}",
             params=params or {},
             json=data or {},
             headers=self.headers,
-            timeout=timeout,
+            timeout=timeout_s,
         )
         logger.debug(
             "Called deepset Cloud API",
             method="PUT",
             workspace=workspace_name,
             endpoint=endpoint,
             data=data or {},
```

### Comparing `deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/api/files.py` & `deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/api/files.py`

 * *Files 15% similar despite different names*

```diff
@@ -73,26 +73,26 @@
 
     async def list_paginated(
         self,
         workspace_name: str,
         limit: int = 100,
         name: Optional[str] = None,
         content: Optional[str] = None,
-        filter: Optional[str] = None,
+        odata_filter: Optional[str] = None,
         after_value: Optional[Any] = None,
         after_file_id: Optional[UUID] = None,
     ) -> FileList:
         """
         List files in a workspace, paginated with cursor based pagination.
 
         :param workspace_name: Name of the workspace to use.
         :param limit: Number of files to return per page.
-        :param name: Name of the file to filter by.
-        :param content: Content of the file to filter by.
-        :param filter: Odata Filter to apply.
+        :param name: Name of the file to odata_filter by.
+        :param content: Content of the file to odata_filter by.
+        :param odata_filter: Odata odata_filter to apply.
         :param after_value: Value to start after.
         :param after_file_id: File ID to start after.
         """
         params: Dict[str, Union[str, int]] = {"limit": limit}
         if after_value and after_file_id:
             params["after_value"] = (
                 after_value.isoformat() if isinstance(after_value, datetime.datetime) else str(after_value)
@@ -103,47 +103,18 @@
         if name:
             params["name"] = name
 
         # content search file
         if content:
             params["content"] = content
 
-        # odata filter for file meta
-        if filter:
-            params["filter"] = filter
+        # odata odata_filter for file meta
+        if odata_filter:
+            params["odata_filter"] = odata_filter
 
         response = await self._deepset_cloud_api.get(workspace_name, "files", params=params)
         assert response.status_code == codes.OK, f"Failed to list files: {response.text}"
         response_body = response.json()
         total = response_body["total"]
         data = response_body["data"]
         has_more = response_body["has_more"]
         return FileList(total=total, data=[File.from_dict(d) for d in data], has_more=has_more)
-
-    async def list_all(
-        self, workspace_name: str, batch_size: int = 100, timeout: int = 20
-    ) -> AsyncGenerator[List[File], None]:
-        """
-        List all files in a workspace.
-
-        TODO: move this one level up to deepset_cloud_api since this is
-        logic on top of the raw API.
-        TODO: Take care of raising a timeout exception if the timeout is reached.
-
-        :param workspace_name: Name of the workspace to use.
-        """
-        start = time.time()
-        has_more = True
-
-        after_value = None
-        after_file_id = None
-        while time.time() - start < timeout and has_more:
-            response = await self.list_paginated(
-                workspace_name,
-                limit=batch_size,
-                after_file_id=after_file_id,
-                after_value=after_value,
-            )
-            has_more = response.has_more
-            after_value = response.data[-1].created_at
-            after_file_id = response.data[-1].file_id
-            yield response.data
```

### Comparing `deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/api/upload_sessions.py` & `deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/api/upload_sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 @dataclass
 class AWSPrefixedRequesetConfig:
     """AWS prefixed request config.
 
     This prefixed request config can be used to send authenticated requests to AWS S3.
     """
 
-    fields: Dict[str, Any]
+    fields: Dict[str, str]
     url: str
 
 
 @dataclass
 class UploadSession:
     """Upload session object."""
```

### Comparing `deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/service/files_service.py` & `deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/service/files_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 """Module for all file related operations."""
 from __future__ import annotations
 
 import asyncio
 import enum
+import os
 import time
 from contextlib import asynccontextmanager
 from dataclasses import dataclass
+from functools import partial
+from io import BufferedReader
 from pathlib import Path
-from typing import Any, AsyncGenerator, Dict, List, Optional
-from unittest.mock import AsyncMock, Mock
+from typing import Any, AsyncGenerator, Callable, Dict, List, Optional, Tuple
+from unittest.mock import AsyncMock
 from uuid import UUID
 
 import httpx
 import structlog
 
 from deepset_cloud_sdk.api.config import CommonConfig
 from deepset_cloud_sdk.api.deepset_cloud_api import DeepsetCloudAPI
-from deepset_cloud_sdk.api.files import FilesAPI
+from deepset_cloud_sdk.api.files import File, FilesAPI
 from deepset_cloud_sdk.api.upload_sessions import (
     UploadSession,
     UploadSessionsAPI,
     UploadSessionStatus,
     WriteMode,
 )
+from deepset_cloud_sdk.models import DeepsetCloudFile
+from deepset_cloud_sdk.s3.upload import S3
 
 logger = structlog.get_logger(__name__)
 
 
-@dataclass
-class DeepsetCloudFile:
-    """Dataclass for files in deepsetCloud."""
-
-    text: str
-    name: str
-    meta: Optional[Dict[str, Any]] = None
-
-
 class FilesService:
     """Service for all file related operations."""
 
-    def __init__(self, upload_sessions: UploadSessionsAPI, files: FilesAPI, aws: Mock):
+    def __init__(self, upload_sessions: UploadSessionsAPI, files: FilesAPI, s3: S3):
         """Initialize the service.
 
         :param upload_sessions: API for upload sessions.
         :param files: API for files.
         :param aws: AWS client.
         """
         self._upload_sessions = upload_sessions
         self._files = files
-        self._aws = aws
+        self._s3 = s3
 
     @classmethod
     @asynccontextmanager
     async def factory(cls, config: CommonConfig) -> AsyncGenerator[FilesService, None]:
         """Create a new instance of the service.
 
         :param config: CommonConfig object.
         :param client: httpx client.
         :return: New instance of the service.
         """
         async with DeepsetCloudAPI.factory(config) as deepset_cloud_api:
             files_api = FilesAPI(deepset_cloud_api)
             upload_sessions_api = UploadSessionsAPI(deepset_cloud_api)
 
-            yield cls(upload_sessions_api, files_api, AsyncMock())
+            yield cls(upload_sessions_api, files_api, S3(concurrency=30))
 
     async def _wait_for_finished(self, workspace_name: str, session_id: UUID, total_files: int, timeout_s: int) -> None:
         start = time.time()
         ingested_files = 0
         while ingested_files < total_files:
             if time.time() - start > timeout_s:
                 raise TimeoutError("Ingestion timed out.")
@@ -122,22 +118,33 @@
         :file_paths: List of file paths to upload.
         :blocking: If True, blocks until the ingestion is finished.
         :timeout_s: Timeout in seconds for the blocking ingestion.
         :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
         """
         # create session to upload files to
         async with self._create_upload_session(workspace_name=workspace_name, write_mode=write_mode) as upload_session:
-            await self._aws.upload_files(upload_session=upload_session, file_paths=file_paths)
+            # upload file paths to session
+
+            upload_summary = await self._s3.upload_files_from_paths(
+                upload_session=upload_session, file_paths=file_paths
+            )
+            logger.info(
+                "Summary of S3 Uploads",
+                successful_uploads=upload_summary.successful_upload_count,
+                failed_uploads=upload_summary.failed_upload_count,
+                failed=upload_summary.failed,
+            )
 
         # wait for ingestion to finish
         if blocking:
+            total_files = len(list(filter(lambda x: not os.path.basename(x).endswith(".meta.json"), file_paths)))
             await self._wait_for_finished(
                 workspace_name=workspace_name,
                 session_id=upload_session.session_id,
-                total_files=len(file_paths),
+                total_files=total_files,
                 timeout_s=timeout_s,
             )
 
     async def upload_folder(
         self,
         workspace_name: str,
         folder_path: Path,
@@ -201,16 +208,60 @@
         :dc_files: List of DeepsetCloudFiles to upload.
         :blocking: If True, blocks until the ingestion is finished.
         :timeout_s: Timeout in seconds for the blocking ingestion.
         :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
         """
         # create session to upload files to
         async with self._create_upload_session(workspace_name=workspace_name, write_mode=write_mode) as upload_session:
-            await self._aws.upload_texts(upload_session=upload_session, dc_files=dc_files)
+            await self._s3.upload_texts(upload_session=upload_session, dc_files=dc_files)
 
         if blocking:
             await self._wait_for_finished(
                 workspace_name=workspace_name,
                 session_id=upload_session.session_id,
                 total_files=len(dc_files),
                 timeout_s=timeout_s,
             )
+
+    async def list_all(
+        self,
+        workspace_name: str,
+        name: Optional[str] = None,
+        content: Optional[str] = None,
+        odata_filter: Optional[str] = None,
+        batch_size: int = 100,
+        timeout_s: int = 20,
+    ) -> AsyncGenerator[List[File], None]:
+        """List all files in a workspace.
+
+        Returns an async generator that yields lists of files. The generator is finished when all files are listed.
+        The batch size per number of returned files can be specified with batch_size.
+
+        :param workspace_name: Name of the workspace to use.
+        :param name: odata_filter by file name.
+        :param content: odata_filter by file content.
+        :param odata_filter: odata_filter by file meta data.
+        :param batch_size: Number of files to return per request.
+        :param timeout_s: Timeout in seconds for the listing.
+        :raises TimeoutError: If the listing takes longer than timeout_s.
+        """
+        start = time.time()
+        has_more = True
+
+        after_value = None
+        after_file_id = None
+        while has_more:
+            if time.time() - start > timeout_s:
+                raise TimeoutError(f"Listing all files in workspace {workspace_name} timed out.")
+            response = await self._files.list_paginated(
+                workspace_name,
+                name=name,
+                content=content,
+                odata_filter=odata_filter,
+                limit=batch_size,
+                after_file_id=after_file_id,
+                after_value=after_value,
+            )
+            has_more = response.has_more
+            after_value = response.data[-1].created_at
+            after_file_id = response.data[-1].file_id
+            yield response.data
```

### Comparing `deepset_cloud_sdk-0.0.1/deepset_cloud_sdk/workflows/async_client/files.py` & `deepset_cloud_sdk-0.0.3/deepset_cloud_sdk/workflows/async_client/files.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,57 @@
+# pylint:disable=too-many-arguments
 """This module contains async functions for uploading files and folders to the Deepset Cloud."""
 from pathlib import Path
-from typing import List, Optional
+from typing import AsyncGenerator, List, Optional
 
 from deepset_cloud_sdk.api.config import (
     API_KEY,
     API_URL,
     DEFAULT_WORKSPACE_NAME,
     CommonConfig,
 )
+from deepset_cloud_sdk.api.files import File
 from deepset_cloud_sdk.api.upload_sessions import WriteMode
 from deepset_cloud_sdk.service.files_service import DeepsetCloudFile, FilesService
 
 
 def _get_config(api_key: Optional[str] = None, api_url: Optional[str] = None) -> CommonConfig:
     return CommonConfig(api_key=api_key or API_KEY, api_url=api_url or API_URL)
 
 
+async def list_files(
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+    name: Optional[str] = None,
+    content: Optional[str] = None,
+    odata_filter: Optional[str] = None,
+    batch_size: int = 100,
+    timeout_s: int = 300,
+) -> AsyncGenerator[List[File], None]:
+    """List all files in a workspace.
+
+    :param api_key: API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param workspace_name: Name of the workspace to list the files from.
+    :param batch_size: Batch size for the listing.
+    :return: List of files.
+    """
+    async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
+        async for file_batch in file_service.list_all(
+            workspace_name=workspace_name,
+            name=name,
+            content=content,
+            odata_filter=odata_filter,
+            batch_size=batch_size,
+            timeout_s=timeout_s,
+        ):
+            yield file_batch
+
+
 async def upload_file_paths(
     file_paths: List[Path],
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     write_mode: WriteMode = WriteMode.KEEP,
     blocking: bool = True,
```

### Comparing `deepset_cloud_sdk-0.0.1/examples/README.md` & `deepset_cloud_sdk-0.0.3/examples/sdk/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 
 You can upload files in three different ways:
 1. Upload multiple files by providing explicit file paths.
 2. Upload all files from a folder.
 3. Upload raw text.
 
 All three methods have the same parameters:
-- `workspace_name`: str = None 
+- `workspace_name`: str = None
     Optional. Specifies the deepset Cloud workspace where you want to upload the files. You can set it through environment variable. If you don't provide any value, the files are uploaded to the `default` workspace.
 - `blocking`: bool = True
-    Optional. Specifies if you want to wait until your files are listed in deepset Cloud. This can take up to one hour, depending on the size and number of files. 
+    Optional. Specifies if you want to wait until your files are listed in deepset Cloud. This can take up to one hour, depending on the size and number of files.
 - `timeout_s`: int = 300
-    Optional. A custom timeout for file upload in seconds. 
+    Optional. A custom timeout for file upload in seconds.
 - `api_key`: str = None
     Optional. The API key to deepset Cloud. You can configure it through an environment variable.
 - `api_url`: str = None
     Optional. The production URL. It's useful for running tests against a dev environment or your own domain. You can configure it through an environment variable. For other cases, you can just ignore it.
-
-
```

### Comparing `deepset_cloud_sdk-0.0.1/examples/upload.py` & `deepset_cloud_sdk-0.0.3/examples/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.1/examples/data/example.pdf` & `deepset_cloud_sdk-0.0.3/examples/data/example.pdf`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.1/.gitignore` & `deepset_cloud_sdk-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.1/README.md` & `deepset_cloud_sdk-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 This README provides an overview of the SDK and its features, and information on contributing to the project and exploring related resources.
 
 # Supported Features
 The current version of the SDK focuses on providing an easy way to upload files to deepset Cloud for further processing and analysis. For detailed instructions and examples, see file_uploads/README.md.
 
 ## Examples
 The following examples demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud.
-- [Upload datasets to deepset Cloud](/examples/upload.py)
+- [Upload datasets to deepset Cloud via SDK](/examples/sdk/upload.py)
+- [Upload datasets to deepset Cloud via CLI](/examples/cli/README.md)
+
+## CLI
+You can use the deepset Cloud SDK in the command line as well. For more information, see the [CLI documentation](/examples/cli/README.md).
 
 ## Installation
 The deepset Cloud SDK is available on PyPI and can be installed using pip:
 ```bash
 pip install deepset-cloud-sdk
 ```
```

#### html2text {}

```diff
@@ -12,21 +12,24 @@
 various natural language processing (NLP) tasks. This README provides an
 overview of the SDK and its features, and information on contributing to the
 project and exploring related resources. # Supported Features The current
 version of the SDK focuses on providing an easy way to upload files to deepset
 Cloud for further processing and analysis. For detailed instructions and
 examples, see file_uploads/README.md. ## Examples The following examples
 demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud. -
-[Upload datasets to deepset Cloud](/examples/upload.py) ## Installation The
-deepset Cloud SDK is available on PyPI and can be installed using pip: ```bash
-pip install deepset-cloud-sdk ``` ## Contributing We welcome contributions from
-the open source community to enhance the deepset Cloud SDK. I f you would like
-to contribute, refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for
-guidelines and instructions on how to get started. We appreciate your
-contributions, whether they're bug fixes, new features, or documentation
-improvements. --- ## Interested in deepset Cloud? If you are interested in
-exploring deepset Cloud, visit cloud.deepset.ai. deepset Cloud provides a range
-of NLP capabilities and services to help you build and deploy powerful natural
-language processing applications. ## Interested in Haystack? deepset Cloud is
-powered by Haystack, an open source framework for building end-to-end NLP
-pipelines. - [Project website](https://haystack.deepset.ai/) - [GitHub
-repository](https://github.com/deepset-ai/haystack)
+[Upload datasets to deepset Cloud via SDK](/examples/sdk/upload.py) - [Upload
+datasets to deepset Cloud via CLI](/examples/cli/README.md) ## CLI You can use
+the deepset Cloud SDK in the command line as well. For more information, see
+the [CLI documentation](/examples/cli/README.md). ## Installation The deepset
+Cloud SDK is available on PyPI and can be installed using pip: ```bash pip
+install deepset-cloud-sdk ``` ## Contributing We welcome contributions from the
+open source community to enhance the deepset Cloud SDK. I f you would like to
+contribute, refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines
+and instructions on how to get started. We appreciate your contributions,
+whether they're bug fixes, new features, or documentation improvements. --- ##
+Interested in deepset Cloud? If you are interested in exploring deepset Cloud,
+visit cloud.deepset.ai. deepset Cloud provides a range of NLP capabilities and
+services to help you build and deploy powerful natural language processing
+applications. ## Interested in Haystack? deepset Cloud is powered by Haystack,
+an open source framework for building end-to-end NLP pipelines. - [Project
+website](https://haystack.deepset.ai/) - [GitHub repository](https://
+github.com/deepset-ai/haystack)
```

### Comparing `deepset_cloud_sdk-0.0.1/pyproject.toml` & `deepset_cloud_sdk-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -23,40 +23,63 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "structlog==23.1.0",
   "httpx==0.24.0",
   "python-dotenv==1.0.0",
+  "typer==0.9.0",
+  "tenacity==8.2.2",
+  "aiohttp==3.8.4"
 ]
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/deepset-cloud-sdk#readme"
 Issues = "https://github.com/deepset-ai/deepset-cloud-sdk/issues"
 Source = "https://github.com/deepset-ai/deepset-cloud-sdk"
 
+
+[project.scripts]
+deepset-cloud-cli  = "deepset_cloud_sdk.cli:run_packaged"
+
 [tool.hatch.version]
 path = "deepset_cloud_sdk/__about__.py"
 
 [tool.hatch.envs.default.scripts]
 tests-with-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/unit"
 tests-integration = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/integration"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.10"]
 
 [tool.hatch.envs.default]
 dependencies = [
+  "structlog==23.1.0",
+  "httpx==0.24.0",
+  "python-dotenv==1.0.0",
+  "tenacity==8.2.2",
+  "aiohttp==3.8.4",
+]
+
+[tool.hatch.envs.test.scripts]
+unit-with-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/unit"
+integration = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/integration"
+
+[tool.hatch.envs.test]
+template='default'
+dependencies = [
   "pytest-cov==4.0.0",
   "pytest==7.3.1",
   "pytest-asyncio==0.21.0",
 ]
 
+
 [tool.hatch.envs.code-quality]
-detached = true
+template='default'
+detached = false
 # Please keep these aligned with the versions defined in .pre-commit-config.yaml
 dependencies = [
   "pylint==2.15.2",
   "pydocstyle==6.3.0",
   "black==23.3.0",
   "isort==5.12.0",
   "mypy==1.1.1",
@@ -69,15 +92,15 @@
 format-fix = "black deepset_cloud_sdk tests"
 lint = "pylint deepset_cloud_sdk"
 sort = "isort --check --profile black ."
 hooks = "pre-commit install"
 docstrings = "pydocstyle deepset_cloud_sdk"
 
 [tool.hatch.envs.tools]
-detached = true
+detached = false
 # Please keep these aligned with the versions defined in .pre-commit-config.yaml
 dependencies = [
   "pip-tools==6.13.0",
 ]
 
 [tool.hatch.envs.tools.scripts]
 requirements = "pip-compile -o requirements.txt pyproject.toml"
```

### Comparing `deepset_cloud_sdk-0.0.1/PKG-INFO` & `deepset_cloud_sdk-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepset-cloud-sdk
-Version: 0.0.1
+Version: 0.0.3
 Summary: deepset cloud SDK
 Project-URL: Documentation, https://github.com/deepset-ai/deepset-cloud-sdk#readme
 Project-URL: Issues, https://github.com/deepset-ai/deepset-cloud-sdk/issues
 Project-URL: Source, https://github.com/deepset-ai/deepset-cloud-sdk
 Author-email: deepset <rohan.janjua@deepset.ai>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -12,17 +12,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: aiohttp==3.8.4
 Requires-Dist: httpx==0.24.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: structlog==23.1.0
+Requires-Dist: tenacity==8.2.2
+Requires-Dist: typer==0.9.0
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://cloud.deepset.ai/"><img src="/assets/logo.png"  alt="deepset Cloud SDK"></a>
 </p>
 
 [![Tests](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-integration.yml)
@@ -33,15 +36,19 @@
 This README provides an overview of the SDK and its features, and information on contributing to the project and exploring related resources.
 
 # Supported Features
 The current version of the SDK focuses on providing an easy way to upload files to deepset Cloud for further processing and analysis. For detailed instructions and examples, see file_uploads/README.md.
 
 ## Examples
 The following examples demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud.
-- [Upload datasets to deepset Cloud](/examples/upload.py)
+- [Upload datasets to deepset Cloud via SDK](/examples/sdk/upload.py)
+- [Upload datasets to deepset Cloud via CLI](/examples/cli/README.md)
+
+## CLI
+You can use the deepset Cloud SDK in the command line as well. For more information, see the [CLI documentation](/examples/cli/README.md).
 
 ## Installation
 The deepset Cloud SDK is available on PyPI and can be installed using pip:
 ```bash
 pip install deepset-cloud-sdk
 ```
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: deepset-cloud-sdk Version: 0.0.1 Summary: deepset
+Metadata-Version: 2.1 Name: deepset-cloud-sdk Version: 0.0.3 Summary: deepset
 cloud SDK Project-URL: Documentation, https://github.com/deepset-ai/deepset-
 cloud-sdk#readme Project-URL: Issues, https://github.com/deepset-ai/deepset-
 cloud-sdk/issues Project-URL: Source, https://github.com/deepset-ai/deepset-
 cloud-sdk Author-email: deepset
 janjua@deepset.ai> License-Expression: MIT Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
-Implementation :: PyPy Requires-Python: >=3.8 Requires-Dist: httpx==0.24.0
-Requires-Dist: python-dotenv==1.0.0 Requires-Dist: structlog==23.1.0
+Implementation :: PyPy Requires-Python: >=3.8 Requires-Dist: aiohttp==3.8.4
+Requires-Dist: httpx==0.24.0 Requires-Dist: python-dotenv==1.0.0 Requires-Dist:
+structlog==23.1.0 Requires-Dist: tenacity==8.2.2 Requires-Dist: typer==0.9.0
 Description-Content-Type: text/markdown
                               [deepset_Cloud_SDK]
 [![Tests](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/
 continuous-integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-
 cloud-sdk/actions/workflows/continuous-integration.yml) [![Deploy PyPi](https:/
 /github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/
 badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/
@@ -26,21 +27,24 @@
 various natural language processing (NLP) tasks. This README provides an
 overview of the SDK and its features, and information on contributing to the
 project and exploring related resources. # Supported Features The current
 version of the SDK focuses on providing an easy way to upload files to deepset
 Cloud for further processing and analysis. For detailed instructions and
 examples, see file_uploads/README.md. ## Examples The following examples
 demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud. -
-[Upload datasets to deepset Cloud](/examples/upload.py) ## Installation The
-deepset Cloud SDK is available on PyPI and can be installed using pip: ```bash
-pip install deepset-cloud-sdk ``` ## Contributing We welcome contributions from
-the open source community to enhance the deepset Cloud SDK. I f you would like
-to contribute, refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for
-guidelines and instructions on how to get started. We appreciate your
-contributions, whether they're bug fixes, new features, or documentation
-improvements. --- ## Interested in deepset Cloud? If you are interested in
-exploring deepset Cloud, visit cloud.deepset.ai. deepset Cloud provides a range
-of NLP capabilities and services to help you build and deploy powerful natural
-language processing applications. ## Interested in Haystack? deepset Cloud is
-powered by Haystack, an open source framework for building end-to-end NLP
-pipelines. - [Project website](https://haystack.deepset.ai/) - [GitHub
-repository](https://github.com/deepset-ai/haystack)
+[Upload datasets to deepset Cloud via SDK](/examples/sdk/upload.py) - [Upload
+datasets to deepset Cloud via CLI](/examples/cli/README.md) ## CLI You can use
+the deepset Cloud SDK in the command line as well. For more information, see
+the [CLI documentation](/examples/cli/README.md). ## Installation The deepset
+Cloud SDK is available on PyPI and can be installed using pip: ```bash pip
+install deepset-cloud-sdk ``` ## Contributing We welcome contributions from the
+open source community to enhance the deepset Cloud SDK. I f you would like to
+contribute, refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines
+and instructions on how to get started. We appreciate your contributions,
+whether they're bug fixes, new features, or documentation improvements. --- ##
+Interested in deepset Cloud? If you are interested in exploring deepset Cloud,
+visit cloud.deepset.ai. deepset Cloud provides a range of NLP capabilities and
+services to help you build and deploy powerful natural language processing
+applications. ## Interested in Haystack? deepset Cloud is powered by Haystack,
+an open source framework for building end-to-end NLP pipelines. - [Project
+website](https://haystack.deepset.ai/) - [GitHub repository](https://
+github.com/deepset-ai/haystack)
```

