# Comparing `tmp/wf-video-io-3.2.2.tar.gz` & `tmp/wf_video_io-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf-video-io-3.2.2.tar", max compression
+gzip compressed data, was "wf_video_io-3.2.3.tar", max compression
```

## Comparing `wf-video-io-3.2.2.tar` & `wf_video_io-3.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1088 2022-02-09 16:43:30.670294 wf-video-io-3.2.2/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:10:14.730152 wf-video-io-3.2.2/README.md
--rw-r--r--   0        0        0     1113 2023-01-27 17:15:35.220335 wf-video-io-3.2.2/pyproject.toml
--rwxr-xr-x   0        0        0       28 2022-02-09 16:43:44.499328 wf-video-io-3.2.2/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-10 16:50:49.527465 wf-video-io-3.2.2/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    12586 2023-01-27 17:15:19.709428 wf-video-io-3.2.2/video_io/client/core.py
--rw-r--r--   0        0        0      265 2022-10-10 16:33:33.459443 wf-video-io-3.2.2/video_io/client/errors.py
--rw-r--r--   0        0        0     3319 2022-10-13 18:02:28.972794 wf-video-io-3.2.2/video_io/client/utils.py
--rw-r--r--   0        0        0     1653 2022-10-06 19:06:06.558171 wf-video-io-3.2.2/video_io/config.py
--rwxr-xr-x   0        0        0    46826 2023-01-27 17:15:19.710107 wf-video-io-3.2.2/video_io/core.py
--rw-r--r--   0        0        0      360 2022-10-10 16:45:06.201511 wf-video-io-3.2.2/video_io/log_retry.py
--rw-r--r--   0        0        0     9794 2023-01-27 16:10:14.733391 wf-video-io-3.2.2/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:10:14.733486 wf-video-io-3.2.2/video_io/video_reader.py
--rw-r--r--   0        0        0     1229 1970-01-01 00:00:00.000000 wf-video-io-3.2.2/setup.py
--rw-r--r--   0        0        0     1248 1970-01-01 00:00:00.000000 wf-video-io-3.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.2.3/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.2.3/README.md
+-rw-r--r--   0        0        0     1162 2023-05-15 18:29:11.418209 wf_video_io-3.2.3/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.2.3/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.2.3/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    14986 2023-05-15 17:34:04.908392 wf_video_io-3.2.3/video_io/client/core.py
+-rw-r--r--   0        0        0      265 2023-05-15 17:34:04.808749 wf_video_io-3.2.3/video_io/client/errors.py
+-rw-r--r--   0        0        0     3787 2023-05-15 17:34:04.829824 wf_video_io-3.2.3/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.2.3/video_io/config.py
+-rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.2.3/video_io/core.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.2.3/video_io/log_retry.py
+-rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.2.3/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.2.3/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.2.3/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.2.3/PKG-INFO
```

### Comparing `wf-video-io-3.2.2/LICENSE` & `wf_video_io-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wf-video-io-3.2.2/pyproject.toml` & `wf_video_io-3.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 [project]
 name = "wf-video-io"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.2.2"
+version = "3.2.3"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<3.12"
 jmespath = "^1.0.1"
 tenacity = "^8.1.0"
 urllib3 = "^1.26.12"
 wf-honeycomb-io = ">=2.0.0"
+wf-gqlpycgen = "^0.7.4"
 wf-cv-utils = ">=3.4.0"
 opencv-python = ">=4.6.0"
 wf-fastapi-auth0 = ">=1.0"
 pyyaml = "^6.0"
 ffmpeg-python = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 behave = "^1.2.6"
 pymongo = ">=4.0.1"
 auth0-python = "^3.23.1"
 cachetools = "^5.2.0"
 python-jose = "^3.3.0"
 pylint = "^2.15.4"
 pytest = "^7.2.0"
+black = "^23.3.0"
 
 [tool.setuptools]
 py-modules = []
 
 [build-system]
 requires = ["poetry-core", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wf-video-io-3.2.2/video_io/client/core.py` & `wf_video_io-3.2.3/video_io/client/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,132 +4,194 @@
 import json
 from json.decoder import JSONDecodeError
 import logging
 import os
 from pathlib import Path
 from typing import List, Dict
 
+from cachetools import TTLCache
 import requests
 from requests.adapters import HTTPAdapter
 import yaml
 
 import video_io.config
 from video_io.log_retry import LogRetry
 from video_io.client.errors import SyncError
-from video_io.client.utils import client_token, parse_path, get_video_file_details, chunks, FPS_PATH
-
-
-parse_path("06403ab8-8300-456f-802a-1f4228f69042/2022/10/25/16/03-50.mp4")
-
+from video_io.client.utils import (
+    client_token,
+    parse_path,
+    get_video_file_details,
+    chunks,
+    FPS_PATH,
+)
 
 
 logger = logging.getLogger(__name__)
 
 
 class VideoStorageClient:
-
     def __init__(
         self,
         token=None,
         cache_directory=video_io.config.VIDEO_STORAGE_LOCAL_CACHE_DIRECTORY,
         url=video_io.config.VIDEO_STORAGE_URL,
         auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
         audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
         client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
-        client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET
+        client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     ):
         self.CACHE_DIRECTORY = cache_directory
         self.URL = url
+
+        self.auth_domain = auth_domain
+        self.audience = audience
+        self.client_id = client_id
+        self.client_secret = client_secret
+
+        self.headers = {}  # {"Content-Type": "application/json"}
+
+        self.tokens = {}
         if token is not None:
-            self.token = token
-        else:
-            self.token = client_token(
-                auth_domain=auth_domain,
-                audience=audience,
-                client_id=client_id,
-                client_secret=client_secret
-            )
+            self.tokens["access_token"] = token
+
         self.request_session = self.init_request_session()
 
     @staticmethod
     def init_request_session():
         retry_strategy = LogRetry(
             total=6,
             status_forcelist=[429, 500, 502, 503, 504],
             method_whitelist=["HEAD", "GET", "OPTIONS", "POST"],
-            backoff_factor=0.5
+            backoff_factor=0.5,
         )
         adapter = HTTPAdapter(max_retries=retry_strategy)
         request_session = requests.Session()
         request_session.mount("https://", adapter)
         request_session.mount("http://", adapter)
         return request_session
 
+    def refresh_token(self):
+        try:
+            (token, expires_in) = client_token(
+                auth_domain=self.auth_domain,
+                audience=self.audience,
+                client_id=self.client_id,
+                client_secret=self.client_secret,
+            )
+            if token is None:
+                raise Exception("invalid client_credentials")
+
+            # Refresh token once TTL is less than 5 minutes
+            self.tokens = TTLCache(maxsize=1, ttl=expires_in - 300)
+            self.tokens["access_token"] = token
+        except Exception as err:
+            import traceback
+
+            logger.error("An exception occurred during Authorization")
+            traceback.print_exception(err)
+            raise Exception("invalid client_credentials") from err
+
+    @property
+    def headers(self):
+        if "access_token" not in self.tokens:
+            self.refresh_token()
+
+        return {
+            "Authorization": f"Bearer {self.tokens['access_token']}",
+            **self._headers,
+        }
 
-    async def get_videos(self, environment_id, start_date, end_date, camera_id=None, destination=None):
+    @headers.setter
+    def headers(self, header_dict: dict):
+        self._headers = header_dict
+
+    async def get_videos(
+        self, environment_id, start_date, end_date, camera_id=None, destination=None
+    ):
         if destination is None:
-            destination=self.CACHE_DIRECTORY
+            destination = self.CACHE_DIRECTORY
         if not hasattr(destination, "mkdir"):
             destination = Path(destination)
         destination.mkdir(parents=True, exist_ok=True)
-        meta = self.get_videos_metadata_paginated(environment_id, start_date, end_date, camera_id)
+        meta = self.get_videos_metadata_paginated(
+            environment_id, start_date, end_date, camera_id
+        )
         futures = []
         with concurrent.futures.ThreadPoolExecutor(max_workers=4) as e:
             async for vid_meta in meta:
-                f = e.submit(asyncio.run, self.get_video(path=vid_meta["meta"]["path"], destination=destination))
+                f = e.submit(
+                    asyncio.run,
+                    self.get_video(
+                        path=vid_meta["meta"]["path"], destination=destination
+                    ),
+                )
                 futures.append(f)
         list(concurrent.futures.as_completed(futures))
 
     async def get_video(self, path: str, destination: str, overwrite: bool = False):
         p = Path(destination) / path
         if not p.is_file() or overwrite:
-            logger.info('Downloading video file %s', path)
+            logger.info("Downloading video file %s", path)
             request = {
                 "method": "GET",
-                "url": f'{self.URL}/video/{path}/data',
-                "headers": {
-                    "Authorization": f"bearer {self.token}",
-                },
+                "url": f"{self.URL}/video/{path}/data",
+                "headers": self.headers,
             }
             try:
                 response = self.request_session.request(**request)
                 response.raise_for_status()
 
                 pp = p.parent
                 if not pp.exists():
                     pp.mkdir(parents=True, exist_ok=True)
                 p.write_bytes(response.content)
-                logger.info('Video file %s finished downloading', path)
+                logger.info("Video file %s finished downloading", path)
             except requests.exceptions.HTTPError as e:
-                logger.error('Failing fetching video file %s with HTTP error code %s', path, e.response.status_code)
+                logger.error(
+                    "Failing fetching video file %s with HTTP error code %s",
+                    path,
+                    e.response.status_code,
+                )
                 raise e
             except requests.exceptions.RequestException as e:
-                logger.error('Failing fetching video file %s with exception %s', path, e)
+                logger.error(
+                    "Failing fetching video file %s with exception %s", path, e
+                )
                 raise e
         else:
-            logger.info('Video file %s already exists', path)
+            logger.info("Video file %s already exists", path)
 
-
-    async def get_videos_metadata_paginated(self, environment_id, start_date, end_date, camera_id=None, skip=0, limit=100):
+    async def get_videos_metadata_paginated(
+        self, environment_id, start_date, end_date, camera_id=None, skip=0, limit=100
+    ):
         current_skip = skip
         while True:
-            page = await self.get_videos_metadata(environment_id, start_date, end_date, camera_id=camera_id, skip=current_skip, limit=limit)
+            page = await self.get_videos_metadata(
+                environment_id,
+                start_date,
+                end_date,
+                camera_id=camera_id,
+                skip=current_skip,
+                limit=limit,
+            )
             for item in page:
                 yield item
             current_skip += limit
             if len(page) == 0:
                 break
 
-    async def get_videos_metadata(self, environment_id, start_date, end_date, camera_id=None, skip=0, limit=100):
+    async def get_videos_metadata(
+        self, environment_id, start_date, end_date, camera_id=None, skip=0, limit=100
+    ):
         request = {
             "method": "GET",
-            "url": f'{self.URL}/videos/{environment_id}/device/{camera_id}' if camera_id is not None else f'{self.URL}/videos/{environment_id}',
-            "headers": {
-                "Authorization": f"bearer {self.token}",
-            },
+            "url": f"{self.URL}/videos/{environment_id}/device/{camera_id}"
+            if camera_id is not None
+            else f"{self.URL}/videos/{environment_id}",
+            "headers": self.headers,
             "params": {
                 "start_date": start_date,
                 "end_date": end_date,
                 "skip": skip,
                 "limit": limit,
             },
             "timeout": 120,
@@ -137,159 +199,212 @@
         try:
             response = requests.request(**request)
             response.raise_for_status()
 
             data = response.json()
             return data
         except requests.exceptions.HTTPError as e:
-            logger.error('Failing fetching video metadata for %s from %s to %s with HTTP error code %s', environment_id, start_date, end_date, e.response.status_code)
+            logger.error(
+                "Failing fetching video metadata for %s from %s to %s with HTTP error code %s",
+                environment_id,
+                start_date,
+                end_date,
+                e.response.status_code,
+            )
             raise e
         except requests.exceptions.RequestException as e:
-            logger.error('Failing fetching video metadata for %s from %s to %s with exception %s', environment_id, start_date, end_date, e)
+            logger.error(
+                "Failing fetching video metadata for %s from %s to %s with exception %s",
+                environment_id,
+                start_date,
+                end_date,
+                e,
+            )
             raise e
 
     async def upload_video(self, path, local_cache_directory=None):
         if local_cache_directory is None:
-            local_cache_directory=self.CACHE_DIRECTORY
+            local_cache_directory = self.CACHE_DIRECTORY
         full_path = local_cache_directory / path
         ptype, file_details = parse_path(path)
         if ptype == "file":
             file_details["ptype"] = ptype
             file_details["path"] = full_path
             file_details["filepath"] = path
             resp = await self.upload_videos([file_details])
             return resp[0]
-        return {"error": "invalid path. doesn't match pattern [environment_id]/[camera_id]/[year]/[month]/[day]/[hour]/[min]-[second].mp4"}
+        return {
+            "error": "invalid path. doesn't match pattern [environment_id]/[camera_id]/[year]/[month]/[day]/[hour]/[min]-[second].mp4"
+        }
 
     def prepare_video(self, file_details: Dict) -> (Dict, BytesIO):
         path = file_details["path"]
         video_properties = get_video_file_details(path)
         if file_details["ptype"] == "file":
             ts = f"{file_details['year']}-{file_details['month']}-{file_details['day']}T{file_details['hour']}:{file_details['file'][0:2]}:{file_details['file'][3:5]}.0000"
             meta = {
                 "timestamp": ts,
                 "meta": {
                     "environment_id": file_details["environment_id"],
                     "camera_id": file_details["camera_id"],
                     "duration_seconds": video_properties["format"]["duration"],
-                    "fps": eval(FPS_PATH.search(video_properties)[0]),  # pylint: disable=W0123
+                    "fps": eval(
+                        FPS_PATH.search(video_properties)[0]
+                    ),  # pylint: disable=W0123
                     "path": file_details["filepath"],
                 },
             }
         else:
             p = Path(f"{path}.meta")
             if not p.exists():
-                logger.error('missing meta file for video %s', path)
+                logger.error("missing meta file for video %s", path)
                 return {"error": f"meta is missing for {path}"}
-            with p.open('r', encoding="utf8") as fp:
+            with p.open("r", encoding="utf8") as fp:
                 meta = yaml.safe_load(fp.read())
         return (
             meta,
-            open(path, 'rb'),  # pylint: disable=R1732
+            open(path, "rb"),  # pylint: disable=R1732
         )
 
-
     async def upload_videos(self, file_details: List[Dict]):
         request = {
             "method": "POST",
             "url": f"{self.URL}/videos",
-            "headers": {
-                "Authorization": f"bearer {self.token}",
-            }
+            "headers": self.headers,
         }
         files = []
         videos = []
         for details in file_details:
             meta, fileio = self.prepare_video(details)
-            files.append(("files", fileio, ))
+            files.append(
+                (
+                    "files",
+                    fileio,
+                )
+            )
             videos.append(meta)
         results = []
         request["files"] = files
         request["data"] = {"videos": json.dumps(videos)}
         try:
             request = requests.Request(**request)
             r = request.prepare()
             response = self.request_session.send(r)
             for i, vr in enumerate(response.json()):
-                results.append({"path": videos[i]['meta']['path'], "uploaded": True, "id": vr["id"], "disposition": "ok" if "disposition" not in vr else vr["disposition"]})
+                results.append(
+                    {
+                        "path": videos[i]["meta"]["path"],
+                        "uploaded": True,
+                        "id": vr["id"],
+                        "disposition": "ok"
+                        if "disposition" not in vr
+                        else vr["disposition"],
+                    }
+                )
             return results
         except JSONDecodeError as je:
-            logger.error('Unusual response from video-service for %s: %s', file_details, response.text)
+            logger.error(
+                "Unusual response from video-service for %s: %s",
+                file_details,
+                response.text,
+            )
         except requests.exceptions.HTTPError as e:
-            logger.error('Failing uploading videos %s with HTTP error code %s', file_details, e.response.status_code)
+            logger.error(
+                "Failing uploading videos %s with HTTP error code %s",
+                file_details,
+                e.response.status_code,
+            )
             raise e
         except requests.exceptions.RequestException as e:
-            logger.error('Failing uploading videos %s with exception %s', file_details, e)
+            logger.error(
+                "Failing uploading videos %s with exception %s", file_details, e
+            )
             raise e
 
     async def video_existence_check(self, paths: List[str]):
         request = {
             "method": "POST",
             "url": f"{self.URL}/videos/check",
-            "headers": {
-                "Authorization": f"bearer {self.token}",
-            },
+            "headers": self.headers,
             "json": paths,
         }
         try:
             r = requests.Request(**request).prepare()
             response = self.request_session.send(r)
             try:
                 return response.json()
             except Exception:
                 print(response.text)
-                return [{"err": "response error", "path": p, "exists": False} for p in paths]
+                return [
+                    {"err": "response error", "path": p, "exists": False} for p in paths
+                ]
         except requests.exceptions.HTTPError as e:
-            logger.error('Failing validating video existence %s with HTTP error code %s', paths, e.response.status_code)
+            logger.error(
+                "Failing validating video existence %s with HTTP error code %s",
+                paths,
+                e.response.status_code,
+            )
             raise e
         except requests.exceptions.RequestException as e:
-            logger.error('Failing validating video existence %s exception %s', paths, e)
+            logger.error("Failing validating video existence %s exception %s", paths, e)
             raise e
 
     async def upload_videos_in(
         self,
         path,
         local_cache_directory=None,
         batch_size=video_io.config.SYNC_BATCH_SIZE,
-        max_workers=video_io.config.MAX_SYNC_WORKERS
+        max_workers=video_io.config.MAX_SYNC_WORKERS,
     ):
         if local_cache_directory is None:
             local_cache_directory = self.CACHE_DIRECTORY
         local_cache_directory = Path(local_cache_directory)
         strpath = str(path)
-        t, details = parse_path(strpath[:-1] if strpath[-1] == '/' else strpath)
+        t, details = parse_path(strpath[:-1] if strpath[-1] == "/" else strpath)
         logging.info("ptype is %s", t)
         if details:
             if t in ("file", "fileV2"):
-                raise SyncError("didn't expect file, expected directory, try `upload_video`")
+                raise SyncError(
+                    "didn't expect file, expected directory, try `upload_video`"
+                )
             if t == "year":
                 raise SyncError("cannot sync a year of videos, try limiting to a day")
             if t == "month":
                 raise SyncError("cannot sync a month of videos, try limiting to a day")
             if t == "environment":
-                logger.warning("syncing an entire environment is crazy, I hope you know what you are doing.")
+                logger.warning(
+                    "syncing an entire environment is crazy, I hope you know what you are doing."
+                )
             files_found = []
             for root, _, files in os.walk(local_cache_directory / path):
                 for file in files:
                     full_path = Path(os.path.join(root, file))
-                    ptype, file_details = parse_path(str(full_path.relative_to(local_cache_directory)))
-                    if ptype in ("file", "fileV2") and full_path.suffix in [".h264", ".mp4"]:
+                    ptype, file_details = parse_path(
+                        str(full_path.relative_to(local_cache_directory))
+                    )
+                    if ptype in ("file", "fileV2") and full_path.suffix in [
+                        ".h264",
+                        ".mp4",
+                    ]:
                         file_details["ptype"] = ptype
                         file_details["path"] = full_path
                         file_details["filepath"] = path
                         files_found.append(file_details)
             details["files_found"] = len(files_found)
             details["files_uploaded"] = 0
             details["details"] = []
             logger.debug("found %s files to be uploaded", len(files_found))
-            with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
-                results = executor.map(self.upload_videos, chunks(files_found, batch_size))
+            with concurrent.futures.ThreadPoolExecutor(
+                max_workers=max_workers
+            ) as executor:
+                results = executor.map(
+                    self.upload_videos, chunks(files_found, batch_size)
+                )
                 logger.debug(results)
                 for result in await asyncio.gather(*results):
                     logger.debug(result)
                     for data in result:
                         if data["uploaded"]:
                             details["files_uploaded"] += 1
                         details["details"].append(data)
             return details
         raise SyncError("path {path} was not parsable")
-
```

### Comparing `wf-video-io-3.2.2/video_io/client/utils.py` & `wf_video_io-3.2.3/video_io/client/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,79 +4,127 @@
 
 from tenacity import retry, wait_random, stop_after_attempt
 from auth0.v3.authentication import GetToken
 from cachetools.func import ttl_cache
 import jmespath
 
 
-
 @ttl_cache(ttl=60 * 60 * 4)
 def is_v2_directory(path):
     index_file = path / "wf-video-index.yml"
     return index_file.exists()
 
+
 @ttl_cache(ttl=60 * 60 * 4)
 @retry(wait=wait_random(min=1, max=3), stop=stop_after_attempt(7))
-def client_token(auth_domain, audience, client_id=None, client_secret=None):
+def client_token(
+    auth_domain, audience, client_id=None, client_secret=None
+) -> (str, int):
     get_token = GetToken(auth_domain, timeout=10)
-    token = get_token.client_credentials(
-        client_id,
-        client_secret,
-        audience
-    )
-    api_token = token['access_token']
-    return api_token
+    token = get_token.client_credentials(client_id, client_secret, audience)
+    api_token = token["access_token"]
+    expires_in = token["expires_in"]
+    return api_token, expires_in
 
 
 @ttl_cache(ttl=60 * 60 * 4)
 def get_video_file_details(path):
     # check for meta-file if it exists load that and return it's contents.
     # if not then run ffprobe and return a new meta document
-    ffprobe_out = subprocess.run([
-        "ffprobe",
-        "-v",
-        "error",
-        "-show_entries",
-        "format=duration:stream=nb_read_frames,r_frame_rate,codec_type",
-        "-count_frames",
-        "-of",
-        "json=compact=1",
-        path,
-    ], capture_output=True, check=True)
+    ffprobe_out = subprocess.run(
+        [
+            "ffprobe",
+            "-v",
+            "error",
+            "-show_entries",
+            "format=duration:stream=nb_read_frames,r_frame_rate,codec_type",
+            "-count_frames",
+            "-of",
+            "json=compact=1",
+            path,
+        ],
+        capture_output=True,
+        check=True,
+    )
     return json.loads(ffprobe_out.stdout)
 
-CACHE_PATH_FILE = re.compile('^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})/(?P<hour>[0-9]{2})/(?P<file>.*)$')
-CACHE_PATH_HOUR = re.compile('^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})/(?P<hour>[0-9]{2})$')
-CACHE_PATH_DAY_V2 = re.compile('^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})-(?P<month>[0-9]{2})-(?P<day>[0-9]{2})$')
-CACHE_PATH_FILE_V2 = re.compile('^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})-(?P<month>[0-9]{2})-(?P<day>[0-9]{2})/(?P<file>.*)$')
-CACHE_PATH_DAY = re.compile('^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})$')
-CACHE_PATH_MONTH = re.compile('^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})$')
-CACHE_PATH_YEAR = re.compile('^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})$')
-CACHE_PATH_CAM = re.compile('^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)$')
-CACHE_PATH_ENV = re.compile('^(?P<environment_id>[a-fA-F0-9-]*)$')
+
+CACHE_PATH_FILE = re.compile(
+    "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})/(?P<hour>[0-9]{2})/(?P<file>.*)$"
+)
+CACHE_PATH_HOUR = re.compile(
+    "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})/(?P<hour>[0-9]{2})$"
+)
+CACHE_PATH_DAY_V2 = re.compile(
+    "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})-(?P<month>[0-9]{2})-(?P<day>[0-9]{2})$"
+)
+CACHE_PATH_FILE_V2 = re.compile(
+    "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})-(?P<month>[0-9]{2})-(?P<day>[0-9]{2})/(?P<file>.*)$"
+)
+CACHE_PATH_DAY = re.compile(
+    "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})$"
+)
+CACHE_PATH_MONTH = re.compile(
+    "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})$"
+)
+CACHE_PATH_YEAR = re.compile(
+    "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})$"
+)
+CACHE_PATH_CAM = re.compile(
+    "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)$"
+)
+CACHE_PATH_ENV = re.compile("^(?P<environment_id>[a-fA-F0-9-]*)$")
 
 FPS_PATH = jmespath.compile("streams[?codec_type=='video'].r_frame_rate")
 
+
 def parse_path(path: str) -> (str, dict):
-    result = ('none', None)
+    result = ("none", None)
     for name, pattern in [
-        ('fileV2', CACHE_PATH_FILE_V2,),
-        ('dayV2', CACHE_PATH_DAY_V2,),
-        ('file', CACHE_PATH_FILE,),
-        ('hour', CACHE_PATH_HOUR,),
-        ('day', CACHE_PATH_DAY,),
-        ('month', CACHE_PATH_MONTH,),
-        ('year', CACHE_PATH_YEAR,),
-        ('camera', CACHE_PATH_CAM,),
-        ('environment', CACHE_PATH_ENV,),
+        (
+            "fileV2",
+            CACHE_PATH_FILE_V2,
+        ),
+        (
+            "dayV2",
+            CACHE_PATH_DAY_V2,
+        ),
+        (
+            "file",
+            CACHE_PATH_FILE,
+        ),
+        (
+            "hour",
+            CACHE_PATH_HOUR,
+        ),
+        (
+            "day",
+            CACHE_PATH_DAY,
+        ),
+        (
+            "month",
+            CACHE_PATH_MONTH,
+        ),
+        (
+            "year",
+            CACHE_PATH_YEAR,
+        ),
+        (
+            "camera",
+            CACHE_PATH_CAM,
+        ),
+        (
+            "environment",
+            CACHE_PATH_ENV,
+        ),
     ]:
         match = pattern.match(path)
         if match:
             result = (name, match.groupdict())
             continue
     return result
 
 
 def chunks(lst, n):
     """Yield successive n-sized chunks from lst."""
     for i in range(0, len(lst), n):
-        yield lst[i:i + n]
+        yield lst[i : i + n]
```

### Comparing `wf-video-io-3.2.2/video_io/config.py` & `wf_video_io-3.2.3/video_io/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,29 +2,58 @@
 import multiprocessing
 import os
 from pathlib import Path
 
 
 VIDEO_DURATION = datetime.timedelta(seconds=10)
 
-VIDEO_STORAGE_URL = os.environ.get('VIDEO_STORAGE_URL', 'https://video.api.wildflower-tech.org')
-
-VIDEO_STORAGE_AUTH_DOMAIN = os.environ.get('VIDEO_STORAGE_AUTH_DOMAIN', os.environ.get('AUTH0_DOMAIN'))
-VIDEO_STORAGE_TOKEN_URI = os.environ.get('VIDEO_STORAGE_TOKEN_URI', os.environ.get('AUTH0_TOKEN_URI'))
-VIDEO_STORAGE_AUDIENCE = os.environ.get('VIDEO_STORAGE_AUDIENCE', os.environ.get('API_AUDIENCE'))
-VIDEO_STORAGE_CLIENT_ID = os.environ.get('VIDEO_STORAGE_CLIENT_ID', os.environ.get('AUTH0_CLIENT_ID'))
-VIDEO_STORAGE_CLIENT_SECRET = os.environ.get('VIDEO_STORAGE_CLIENT_SECRET', os.environ.get('AUTH0_CLIENT_SECRET'))
-
-HONEYCOMB_URI = os.environ.get('HONEYCOMB_URI')
-
-HONEYCOMB_AUTH_DOMAIN = os.environ.get('HONEYCOMB_AUTH_DOMAIN', os.environ.get('AUTH0_DOMAIN'))
-HONEYCOMB_TOKEN_URI = os.environ.get('HONEYCOMB_TOKEN_URI', os.environ.get('AUTH0_TOKEN_URI'))
-HONEYCOMB_AUDIENCE = os.environ.get('HONEYCOMB_AUDIENCE', os.environ.get('API_AUDIENCE'))
-HONEYCOMB_CLIENT_ID = os.environ.get('HONEYCOMB_CLIENT_ID', os.environ.get('AUTH0_CLIENT_ID'))
-HONEYCOMB_CLIENT_SECRET = os.environ.get('HONEYCOMB_CLIENT_SECRET', os.environ.get('AUTH0_CLIENT_SECRET'))
-
-VIDEO_STORAGE_LOCAL_CACHE_DIRECTORY = Path(os.environ.get('VIDEO_STORAGE_LOCAL_CACHE_DIRECTORY', '/data'))
+VIDEO_STORAGE_URL = os.environ.get(
+    "VIDEO_STORAGE_URL", "https://video.api.wildflower-tech.org"
+)
+
+VIDEO_STORAGE_AUTH_DOMAIN = os.environ.get(
+    "VIDEO_STORAGE_AUTH_DOMAIN", os.environ.get("AUTH0_DOMAIN")
+)
+VIDEO_STORAGE_TOKEN_URI = os.environ.get(
+    "VIDEO_STORAGE_TOKEN_URI", os.environ.get("AUTH0_TOKEN_URI")
+)
+VIDEO_STORAGE_AUDIENCE = os.environ.get(
+    "VIDEO_STORAGE_AUDIENCE", os.environ.get("API_AUDIENCE")
+)
+VIDEO_STORAGE_CLIENT_ID = os.environ.get(
+    "VIDEO_STORAGE_CLIENT_ID", os.environ.get("AUTH0_CLIENT_ID")
+)
+VIDEO_STORAGE_CLIENT_SECRET = os.environ.get(
+    "VIDEO_STORAGE_CLIENT_SECRET", os.environ.get("AUTH0_CLIENT_SECRET")
+)
+
+HONEYCOMB_URI = os.environ.get("HONEYCOMB_URI")
+
+HONEYCOMB_AUTH_DOMAIN = os.environ.get(
+    "HONEYCOMB_AUTH_DOMAIN", os.environ.get("AUTH0_DOMAIN")
+)
+HONEYCOMB_TOKEN_URI = os.environ.get(
+    "HONEYCOMB_TOKEN_URI", os.environ.get("AUTH0_TOKEN_URI")
+)
+HONEYCOMB_AUDIENCE = os.environ.get(
+    "HONEYCOMB_AUDIENCE", os.environ.get("API_AUDIENCE")
+)
+HONEYCOMB_CLIENT_ID = os.environ.get(
+    "HONEYCOMB_CLIENT_ID", os.environ.get("AUTH0_CLIENT_ID")
+)
+HONEYCOMB_CLIENT_SECRET = os.environ.get(
+    "HONEYCOMB_CLIENT_SECRET", os.environ.get("AUTH0_CLIENT_SECRET")
+)
+
+VIDEO_STORAGE_LOCAL_CACHE_DIRECTORY = Path(
+    os.environ.get("VIDEO_STORAGE_LOCAL_CACHE_DIRECTORY", "/data")
+)
 
 SYNC_BATCH_SIZE = 4
-MAX_SYNC_WORKERS = os.environ.get('MAX_SYNC_WORKERS', os.environ.get('MAX_WORKERS', multiprocessing.cpu_count() - 1))
-
-MAX_DOWNLOAD_WORKERS = os.environ.get('MAX_DOWNLOAD_WORKERS', os.environ.get('MAX_WORKERS', multiprocessing.cpu_count() - 1))
+MAX_SYNC_WORKERS = os.environ.get(
+    "MAX_SYNC_WORKERS", os.environ.get("MAX_WORKERS", multiprocessing.cpu_count() - 1)
+)
+
+MAX_DOWNLOAD_WORKERS = os.environ.get(
+    "MAX_DOWNLOAD_WORKERS",
+    os.environ.get("MAX_WORKERS", multiprocessing.cpu_count() - 1),
+)
```

### Comparing `wf-video-io-3.2.2/video_io/core.py` & `wf_video_io-3.2.3/video_io/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,28 +28,28 @@
     environment_id=None,
     environment_name=None,
     camera_device_types=None,
     camera_device_ids=None,
     camera_part_numbers=None,
     camera_names=None,
     camera_serial_numbers=None,
-    local_video_directory='./videos',
+    local_video_directory="./videos",
     video_filename_extension=None,
     max_workers=video_io.config.MAX_DOWNLOAD_WORKERS,
     client=None,
     uri=video_io.config.HONEYCOMB_URI,
     token_uri=video_io.config.HONEYCOMB_TOKEN_URI,
     audience=video_io.config.HONEYCOMB_AUDIENCE,
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
-    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET
+    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
 ):
     """
     Downloads videos that match search parameters and returns their metadata.
 
     This function simply combines the operations of fetch_video_metadata() and
     download_video_files(). See documentation of those functions for details.
 
@@ -79,15 +79,15 @@
         video_storage_audience (str): Auth0 audience for video service (default is value of VIDEO_STORAGE_AUDIENCE or API_AUDIENCE environment variable)
         video_storage_client_id (str): Auth0 client ID for video service (default is value of VIDEO_STORAGE_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         video_storage_client_secret (str): Auth0 client secret for video service (default is value of VIDEO_STORAGE_CLIENT_SECRET or AUTH0_CLIENT_SECRET environment variable)
 
     Returns:
         (list of dict): Metadata for videos with local path information appended
     """
-    logger.info('Fetching metadata for videos that match specified parameters')
+    logger.info("Fetching metadata for videos that match specified parameters")
     video_metadata = fetch_video_metadata(
         start=start,
         end=end,
         video_timestamps=video_timestamps,
         camera_assignment_ids=camera_assignment_ids,
         environment_id=environment_id,
         environment_name=environment_name,
@@ -102,56 +102,57 @@
         audience=audience,
         client_id=client_id,
         client_secret=client_secret,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
-        video_storage_client_secret=video_storage_client_secret
+        video_storage_client_secret=video_storage_client_secret,
     )
-    logger.info('Downloading video files')
+    logger.info("Downloading video files")
     video_metadata_with_local_paths = download_video_files(
         video_metadata=video_metadata,
         local_video_directory=local_video_directory,
         video_filename_extension=video_filename_extension,
         max_workers=max_workers,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
-        video_storage_client_secret=video_storage_client_secret
+        video_storage_client_secret=video_storage_client_secret,
     )
     return video_metadata_with_local_paths
 
+
 def fetch_images(
     image_timestamps,
     camera_assignment_ids=None,
     environment_id=None,
     environment_name=None,
     camera_device_types=None,
     camera_device_ids=None,
     camera_part_numbers=None,
     camera_names=None,
     camera_serial_numbers=None,
-    local_image_directory='./images',
-    image_filename_extension='png',
-    local_video_directory='./videos',
+    local_image_directory="./images",
+    image_filename_extension="png",
+    local_video_directory="./videos",
     video_filename_extension=None,
     max_workers=video_io.config.MAX_DOWNLOAD_WORKERS,
     client=None,
     uri=video_io.config.HONEYCOMB_URI,
     token_uri=video_io.config.HONEYCOMB_TOKEN_URI,
     audience=video_io.config.HONEYCOMB_AUDIENCE,
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
-    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET
+    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
 ):
     """
     Downloads images that match search parameters and returns their metadata.
 
     This function simply combines the operations of fetch_image_metadata() and
     download_image_files(). See documentation of those functions for details.
 
@@ -181,15 +182,15 @@
         video_storage_audience (str): Auth0 audience for video service (default is value of VIDEO_STORAGE_AUDIENCE or API_AUDIENCE environment variable)
         video_storage_client_id (str): Auth0 client ID for video service (default is value of VIDEO_STORAGE_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         video_storage_client_secret (str): Auth0 client secret for video service (default is value of VIDEO_STORAGE_CLIENT_SECRET or AUTH0_CLIENT_SECRET environment variable)
 
     Returns:
         (list of dict): Metadata for images with local path information appended
     """
-    logger.info('Fetching metadata for images that match specified parameters')
+    logger.info("Fetching metadata for images that match specified parameters")
     image_metadata = fetch_image_metadata(
         image_timestamps=image_timestamps,
         camera_assignment_ids=camera_assignment_ids,
         environment_id=environment_id,
         environment_name=environment_name,
         camera_device_types=camera_device_types,
         camera_device_ids=camera_device_ids,
@@ -202,32 +203,33 @@
         audience=audience,
         client_id=client_id,
         client_secret=client_secret,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
-        video_storage_client_secret=video_storage_client_secret
+        video_storage_client_secret=video_storage_client_secret,
     )
-    logger.info('Downloading image files')
+    logger.info("Downloading image files")
     image_metadata_with_local_paths = download_image_files(
         image_metadata=image_metadata,
         local_image_directory=local_image_directory,
         image_filename_extension=image_filename_extension,
         local_video_directory=local_video_directory,
         video_filename_extension=video_filename_extension,
         max_workers=max_workers,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
-        video_storage_client_secret=video_storage_client_secret
+        video_storage_client_secret=video_storage_client_secret,
     )
     return image_metadata_with_local_paths
 
+
 def fetch_video_metadata(
     start=None,
     end=None,
     video_timestamps=None,
     camera_assignment_ids=None,
     environment_id=None,
     environment_name=None,
@@ -242,15 +244,15 @@
     audience=video_io.config.HONEYCOMB_AUDIENCE,
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
-    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET
+    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
 ):
     """
     Searches Honeycomb for videos that match specified search parameters and
     returns their metadata.
 
     If start and end are specified, returns all videos that overlap with
     specified start and end (e.g., if start is 10:32:56 and end is 10:33:20,
@@ -311,33 +313,38 @@
         audience=audience,
         client_id=client_id,
         client_secret=client_secret,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
-        video_storage_client_secret=video_storage_client_secret
+        video_storage_client_secret=video_storage_client_secret,
     )
-    logger.info('Parsing %s returned video metadata', len(video_metadata_raw))
+    logger.info("Parsing %s returned video metadata", len(video_metadata_raw))
     video_metadata = list()
     for datum in video_metadata_raw:
-        meta = datum.get('meta', {})
-        video_metadata.append({
-            'data_id': datum.get('id'),
-            'video_timestamp': datetime.datetime.fromisoformat(datum.get('timestamp')),
-            'environment_id': meta.get('environment_id'),
-            'assignment_id': meta.get('assignment_id'),
-            'device_id': meta.get('camera_id'),
-            'path': meta.get('path'),
-            'duration_seconds': meta.get('duration_seconds'),
-            'fps': meta.get('fps'),
-            'frame_offsets': meta.get('frame_offsets')
-        })
+        meta = datum.get("meta", {})
+        video_metadata.append(
+            {
+                "data_id": datum.get("id"),
+                "video_timestamp": datetime.datetime.fromisoformat(
+                    datum.get("timestamp")
+                ),
+                "environment_id": meta.get("environment_id"),
+                "assignment_id": meta.get("assignment_id"),
+                "device_id": meta.get("camera_id"),
+                "path": meta.get("path"),
+                "duration_seconds": meta.get("duration_seconds"),
+                "fps": meta.get("fps"),
+                "frame_offsets": meta.get("frame_offsets"),
+            }
+        )
     return video_metadata
 
+
 def fetch_video_metadata_raw(
     start=None,
     end=None,
     video_timestamps=None,
     camera_assignment_ids=None,
     environment_id=None,
     environment_name=None,
@@ -352,47 +359,57 @@
     audience=video_io.config.HONEYCOMB_AUDIENCE,
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
-    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET
+    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
 ):
     if (start is not None or end is not None) and video_timestamps is not None:
-        raise ValueError('Cannot specify start/end and list of video timestamps')
+        raise ValueError("Cannot specify start/end and list of video timestamps")
     if video_timestamps is None and (start is None or end is None):
-        raise ValueError('If not specifying specific timestamps, must specify both start and end times')
+        raise ValueError(
+            "If not specifying specific timestamps, must specify both start and end times"
+        )
     if camera_assignment_ids is not None:
-        raise NotImplementedError('Specification of cameras by assignment ID no longer supported')
+        raise NotImplementedError(
+            "Specification of cameras by assignment ID no longer supported"
+        )
     if camera_part_numbers is not None:
-        raise NotImplementedError('Specification of cameras by part numbers no longer supported')
+        raise NotImplementedError(
+            "Specification of cameras by part numbers no longer supported"
+        )
     if environment_id is None and environment_name is None:
-        raise NotImplementedError('Now that specification of cameras by assignment ID is no longer supported, you must specify an environment ID or environment name')
+        raise NotImplementedError(
+            "Now that specification of cameras by assignment ID is no longer supported, you must specify an environment ID or environment name"
+        )
     if environment_id is not None and environment_name is not None:
-        raise ValueError('Cannot specify both an environment ID and an environment_name')
-    if (
-        camera_device_ids is not None and
-        (
-            camera_device_types is not None or
-            camera_names is not None or
-            camera_serial_numbers is not None
+        raise ValueError(
+            "Cannot specify both an environment ID and an environment_name"
         )
+    if camera_device_ids is not None and (
+        camera_device_types is not None
+        or camera_names is not None
+        or camera_serial_numbers is not None
     ):
-        raise ValueError('Cannot specify both camera device IDs and camera device types/part numbers/names/serial numbers')
-    if (
-        camera_device_types is not None and
-        (
-            camera_names is not None or
-            camera_serial_numbers is not None
+        raise ValueError(
+            "Cannot specify both camera device IDs and camera device types/part numbers/names/serial numbers"
         )
+    if camera_device_types is not None and (
+        camera_names is not None or camera_serial_numbers is not None
     ):
-        raise ValueError('Cannot specify both camera device types and part numbers/names/serial numbers')
+        raise ValueError(
+            "Cannot specify both camera device types and part numbers/names/serial numbers"
+        )
     if video_timestamps is not None:
-        video_timestamps_utc = [video_timestamp.astimezone(datetime.timezone.utc) for video_timestamp in video_timestamps]
+        video_timestamps_utc = [
+            video_timestamp.astimezone(datetime.timezone.utc)
+            for video_timestamp in video_timestamps
+        ]
         video_timestamp_min_utc = min(video_timestamps)
         video_timestamp_max_utc = max(video_timestamps)
         start_utc = video_timestamp_min_utc
         end_utc = video_timestamp_max_utc + video_io.config.VIDEO_DURATION
     else:
         video_timestamps_utc = None
         start_utc = start.astimezone(datetime.timezone.utc)
@@ -403,130 +420,141 @@
         environment_id = honeycomb_io.fetch_environment_id(
             environment_name=environment_name,
             client=client,
             uri=uri,
             token_uri=token_uri,
             audience=audience,
             client_id=client_id,
-            client_secret=client_secret
+            client_secret=client_secret,
         )
     if camera_device_types is not None:
         camera_device_ids = honeycomb_io.fetch_camera_ids_from_environment(
             start=start_utc,
             end=end_utc,
             environment_id=environment_id,
             camera_device_types=camera_device_types,
             client=client,
             uri=uri,
             token_uri=token_uri,
             audience=audience,
             client_id=client_id,
-            client_secret=client_secret
+            client_secret=client_secret,
         )
-    if (
-        camera_names is not None or
-        camera_serial_numbers is not None
-    ):
+    if camera_names is not None or camera_serial_numbers is not None:
         camera_device_ids = honeycomb_io.fetch_camera_ids_from_camera_properties(
             camera_names=camera_names,
             camera_serial_numbers=camera_serial_numbers,
             client=client,
             uri=uri,
             token_uri=token_uri,
             audience=audience,
             client_id=client_id,
-            client_secret=client_secret
+            client_secret=client_secret,
         )
-    video_metadata_raw = asyncio.run(_fetch_video_metadata(
-        video_timestamp_min_utc=video_timestamp_min_utc,
-        video_timestamp_max_utc=video_timestamp_max_utc,
-        video_timestamps_utc=video_timestamps_utc,
-        environment_id=environment_id,
-        camera_device_ids=camera_device_ids,
-        video_storage_url=video_storage_url,
-        video_storage_auth_domain=video_storage_auth_domain,
-        video_storage_audience=video_storage_audience,
-        video_storage_client_id=video_storage_client_id,
-        video_storage_client_secret=video_storage_client_secret
-    ))
+    video_metadata_raw = asyncio.run(
+        _fetch_video_metadata(
+            video_timestamp_min_utc=video_timestamp_min_utc,
+            video_timestamp_max_utc=video_timestamp_max_utc,
+            video_timestamps_utc=video_timestamps_utc,
+            environment_id=environment_id,
+            camera_device_ids=camera_device_ids,
+            video_storage_url=video_storage_url,
+            video_storage_auth_domain=video_storage_auth_domain,
+            video_storage_audience=video_storage_audience,
+            video_storage_client_id=video_storage_client_id,
+            video_storage_client_secret=video_storage_client_secret,
+        )
+    )
     return video_metadata_raw
 
+
 async def _fetch_video_metadata(
     video_timestamp_min_utc,
     video_timestamp_max_utc,
     video_timestamps_utc,
     environment_id,
     camera_device_ids,
     video_storage_url,
     video_storage_auth_domain,
     video_storage_audience,
     video_storage_client_id,
-    video_storage_client_secret
+    video_storage_client_secret,
 ):
     video_client = video_io.client.VideoStorageClient(
         token=None,
         url=video_storage_url,
         auth_domain=video_storage_auth_domain,
         audience=video_storage_audience,
         client_id=video_storage_client_id,
-        client_secret=video_storage_client_secret
-
+        client_secret=video_storage_client_secret,
     )
     result = []
     if video_timestamps_utc is None:
         if camera_device_ids is None:
-            logger.info('Fetching video metadata for all cameras in specified environment')
+            logger.info(
+                "Fetching video metadata for all cameras in specified environment"
+            )
             video_metadata_pages = video_client.get_videos_metadata_paginated(
                 environment_id=environment_id,
                 start_date=video_timestamp_min_utc,
-                end_date=video_timestamp_max_utc
+                end_date=video_timestamp_max_utc,
             )
             async for video_metadata_page in video_metadata_pages:
                 result.append(video_metadata_page)
         else:
-            logger.info('Fetching video metadata for specific cameras')
+            logger.info("Fetching video metadata for specific cameras")
             for camera_id in camera_device_ids:
-                logger.info('Fetching video metadata for camera device ID %s', camera_id)
+                logger.info(
+                    "Fetching video metadata for camera device ID %s", camera_id
+                )
                 video_metadata_pages = video_client.get_videos_metadata_paginated(
                     environment_id=environment_id,
                     start_date=video_timestamp_min_utc,
                     end_date=video_timestamp_max_utc,
-                    camera_id=camera_id
+                    camera_id=camera_id,
                 )
                 async for video_metadata_page in video_metadata_pages:
                     result.append(video_metadata_page)
     else:
         for video_timestamp_utc in video_timestamps_utc:
-            logger.info('Fetching video metadata for video timestamp %s', video_timestamp_utc.isoformat())
+            logger.info(
+                "Fetching video metadata for video timestamp %s",
+                video_timestamp_utc.isoformat(),
+            )
             if camera_device_ids is None:
-                logger.info('Fetching video metadata for all cameras in specified environment')
+                logger.info(
+                    "Fetching video metadata for all cameras in specified environment"
+                )
                 video_metadata_pages = video_client.get_videos_metadata_paginated(
                     environment_id=environment_id,
                     start_date=video_timestamp_utc,
-                    end_date=video_timestamp_utc + video_io.config.VIDEO_DURATION
+                    end_date=video_timestamp_utc + video_io.config.VIDEO_DURATION,
                 )
                 async for video_metadata_page in video_metadata_pages:
                     result.append(video_metadata_page)
             else:
-                logger.info('Fetching video metadata for specific cameras')
+                logger.info("Fetching video metadata for specific cameras")
                 for camera_id in camera_device_ids:
-                    logger.info('Fetching video metadata for camera device ID %s', camera_id)
+                    logger.info(
+                        "Fetching video metadata for camera device ID %s", camera_id
+                    )
                     video_metadata_pages = video_client.get_videos_metadata_paginated(
                         environment_id=environment_id,
                         start_date=video_timestamp_utc,
                         end_date=video_timestamp_utc + video_io.config.VIDEO_DURATION,
-                        camera_id=camera_id
+                        camera_id=camera_id,
                     )
                     async for video_metadata_page in video_metadata_pages:
                         result.append(video_metadata_page)
     return result
 
+
 def download_video_files(
     video_metadata,
-    local_video_directory='./videos',
+    local_video_directory="./videos",
     video_filename_extension=None,
     max_workers=video_io.config.MAX_DOWNLOAD_WORKERS,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
     video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
@@ -560,28 +588,33 @@
         video_storage_client_secret (str): Auth0 client secret for video service (default is value of VIDEO_STORAGE_CLIENT_SECRET or AUTH0_CLIENT_SECRET environment variable)
         overwrite (bool): If set to true, any cached video snippets will be overwritten
 
     Returns:
         (list of dict): Metadata for videos with local path information appended
     """
     if video_filename_extension is not None:
-        raise NotImplementedError('Specifying video filename extension is no longer supported')
-    video_metadata = asyncio.run(_download_video_files(
-        video_metadata=video_metadata,
-        local_video_directory=local_video_directory,
-        max_workers=max_workers,
-        video_storage_url=video_storage_url,
-        video_storage_auth_domain=video_storage_auth_domain,
-        video_storage_audience=video_storage_audience,
-        video_storage_client_id=video_storage_client_id,
-        video_storage_client_secret=video_storage_client_secret,
-        overwrite=overwrite
-    ))
+        raise NotImplementedError(
+            "Specifying video filename extension is no longer supported"
+        )
+    video_metadata = asyncio.run(
+        _download_video_files(
+            video_metadata=video_metadata,
+            local_video_directory=local_video_directory,
+            max_workers=max_workers,
+            video_storage_url=video_storage_url,
+            video_storage_auth_domain=video_storage_auth_domain,
+            video_storage_audience=video_storage_audience,
+            video_storage_client_id=video_storage_client_id,
+            video_storage_client_secret=video_storage_client_secret,
+            overwrite=overwrite,
+        )
+    )
     return video_metadata
 
+
 async def _download_video_files(
     video_metadata,
     local_video_directory,
     max_workers,
     video_storage_url,
     video_storage_auth_domain,
     video_storage_audience,
@@ -591,28 +624,35 @@
 ):
     video_client = video_io.client.VideoStorageClient(
         token=None,
         url=video_storage_url,
         auth_domain=video_storage_auth_domain,
         audience=video_storage_audience,
         client_id=video_storage_client_id,
-        client_secret=video_storage_client_secret
+        client_secret=video_storage_client_secret,
     )
     futures = []
     with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as e:
         for video_metadatum in video_metadata:
-            f = e.submit(asyncio.run, video_client.get_video(
-                path=video_metadatum['path'],
-                destination=local_video_directory,
-                overwrite=overwrite))
-            video_metadatum['video_local_path'] = os.path.join(local_video_directory, video_metadatum['path'])
+            f = e.submit(
+                asyncio.run,
+                video_client.get_video(
+                    path=video_metadatum["path"],
+                    destination=local_video_directory,
+                    overwrite=overwrite,
+                ),
+            )
+            video_metadatum["video_local_path"] = os.path.join(
+                local_video_directory, video_metadatum["path"]
+            )
             futures.append(f)
     list(concurrent.futures.as_completed(futures))
     return video_metadata
 
+
 def fetch_image_metadata(
     image_timestamps,
     camera_assignment_ids=None,
     environment_id=None,
     environment_name=None,
     camera_device_types=None,
     camera_device_ids=None,
@@ -625,15 +665,15 @@
     audience=video_io.config.HONEYCOMB_AUDIENCE,
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
-    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET
+    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
 ):
     """
     Searches Honeycomb for videos containing images that match specified search
     parameters and returns video/image metadata.
 
     Image timestamps are rounded to the nearest tenth of a second to synchronize
     with video frames. Videos containing these images must match all specified
@@ -672,22 +712,25 @@
     Returns:
         (list of dict): Metadata for images that match search parameters
     """
     image_metadata_by_video_timestamp = {}
     for image_timestamp in image_timestamps:
         image_timestamp = image_timestamp.astimezone(datetime.timezone.utc)
         timestamp_floor = image_timestamp.replace(second=0, microsecond=0)
-        video_timestamp = timestamp_floor + math.floor((image_timestamp - timestamp_floor)/datetime.timedelta(seconds=10))*datetime.timedelta(seconds=10)
-        frame_number = round((image_timestamp - video_timestamp)/datetime.timedelta(milliseconds=100))
+        video_timestamp = timestamp_floor + math.floor(
+            (image_timestamp - timestamp_floor) / datetime.timedelta(seconds=10)
+        ) * datetime.timedelta(seconds=10)
+        frame_number = round(
+            (image_timestamp - video_timestamp) / datetime.timedelta(milliseconds=100)
+        )
         if video_timestamp not in image_metadata_by_video_timestamp:
             image_metadata_by_video_timestamp[video_timestamp] = []
-        image_metadata_by_video_timestamp[video_timestamp].append({
-            'image_timestamp': image_timestamp,
-            'frame_number': frame_number
-        })
+        image_metadata_by_video_timestamp[video_timestamp].append(
+            {"image_timestamp": image_timestamp, "frame_number": frame_number}
+        )
     video_timestamps = list(image_metadata_by_video_timestamp.keys())
     video_metadata = fetch_video_metadata(
         video_timestamps=video_timestamps,
         camera_assignment_ids=camera_assignment_ids,
         environment_id=environment_id,
         environment_name=environment_name,
         camera_device_types=camera_device_types,
@@ -701,34 +744,35 @@
         audience=audience,
         client_id=client_id,
         client_secret=client_secret,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
-        video_storage_client_secret=video_storage_client_secret
+        video_storage_client_secret=video_storage_client_secret,
     )
     image_metadata = []
     for video in video_metadata:
-        for image in image_metadata_by_video_timestamp[video['video_timestamp']]:
+        for image in image_metadata_by_video_timestamp[video["video_timestamp"]]:
             image_metadata.append({**video, **image})
     return image_metadata
 
+
 def download_image_files(
     image_metadata,
-    local_image_directory='./images',
-    image_filename_extension='png',
-    local_video_directory='./videos',
+    local_image_directory="./images",
+    image_filename_extension="png",
+    local_video_directory="./videos",
     video_filename_extension=None,
     max_workers=video_io.config.MAX_DOWNLOAD_WORKERS,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
-    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET
+    video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
 ):
     """
     Downloads videos from video service to local directory tree, extract images,
     saves images to local directory tree, and returns metadata with local path
     information added.
 
     Images are specified as a list of dictionaries, as returned by the function
@@ -765,96 +809,111 @@
         local_video_directory=local_video_directory,
         video_filename_extension=video_filename_extension,
         max_workers=max_workers,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
-        video_storage_client_secret=video_storage_client_secret
+        video_storage_client_secret=video_storage_client_secret,
     )
     image_metadata_with_local_paths = []
     for image in image_metadata_with_local_video_paths:
         download_path = image_local_path(
             local_image_directory=local_image_directory,
-            environment_id=image.get('environment_id'),
-            device_id = image.get('device_id'),
-            video_timestamp=image.get('video_timestamp'),
-            frame_number=image.get('frame_number'),
-            image_filename_extension=image_filename_extension
+            environment_id=image.get("environment_id"),
+            device_id=image.get("device_id"),
+            video_timestamp=image.get("video_timestamp"),
+            frame_number=image.get("frame_number"),
+            image_filename_extension=image_filename_extension,
         )
         if not os.path.exists(download_path):
-            video_input = cv_utils.VideoInput(image.get('video_local_path'))
-            image_data = video_input.get_frame_by_frame_number(image.get('frame_number'))
+            video_input = cv_utils.VideoInput(image.get("video_local_path"))
+            image_data = video_input.get_frame_by_frame_number(
+                image.get("frame_number")
+            )
             os.makedirs(os.path.dirname(download_path), exist_ok=True)
-            cv.imwrite(download_path, image_data) # pylint: disable=E1101
+            cv.imwrite(download_path, image_data)  # pylint: disable=E1101
         else:
-            logger.info('File %s already exists', download_path)
-        image['image_local_path'] = download_path
+            logger.info("File %s already exists", download_path)
+        image["image_local_path"] = download_path
         image_metadata_with_local_paths.append(image)
     return image_metadata_with_local_paths
 
+
 def image_local_path(
     local_image_directory,
     environment_id,
     device_id,
     video_timestamp,
     frame_number,
-    image_filename_extension='png'
+    image_filename_extension="png",
 ):
     return os.path.join(
         local_image_directory,
         environment_id,
         device_id,
-        f'{video_timestamp.strftime("%Y/%m/%d/%H-%M-%S")}_{frame_number:03}.{image_filename_extension}'
+        f'{video_timestamp.strftime("%Y/%m/%d/%H-%M-%S")}_{frame_number:03}.{image_filename_extension}',
     )
 
+
 def video_timestamp_min(start):
     original_tzinfo = start.tzinfo
     if original_tzinfo:
         start_naive = start.astimezone(datetime.timezone.utc).replace(tzinfo=None)
     else:
         start_naive = start
     timestamp_min_naive = (
-        datetime.datetime.min +
-        math.floor((start_naive - datetime.datetime.min)/video_io.config.VIDEO_DURATION)*video_io.config.VIDEO_DURATION
+        datetime.datetime.min
+        + math.floor(
+            (start_naive - datetime.datetime.min) / video_io.config.VIDEO_DURATION
+        )
+        * video_io.config.VIDEO_DURATION
     )
     if original_tzinfo:
-        timestamp_min = timestamp_min_naive.replace(tzinfo=datetime.timezone.utc).astimezone(original_tzinfo)
+        timestamp_min = timestamp_min_naive.replace(
+            tzinfo=datetime.timezone.utc
+        ).astimezone(original_tzinfo)
     else:
         timestamp_min = timestamp_min_naive
     return timestamp_min
 
 
 def video_timestamp_max(end):
     original_tzinfo = end.tzinfo
     if original_tzinfo:
         end_naive = end.astimezone(datetime.timezone.utc).replace(tzinfo=None)
     else:
         end_naive = end
     timestamp_max_naive = (
-        datetime.datetime.min +
-        math.ceil((end_naive - datetime.datetime.min)/video_io.config.VIDEO_DURATION)*video_io.config.VIDEO_DURATION
+        datetime.datetime.min
+        + math.ceil(
+            (end_naive - datetime.datetime.min) / video_io.config.VIDEO_DURATION
+        )
+        * video_io.config.VIDEO_DURATION
     )
     if original_tzinfo:
-        timestamp_max = timestamp_max_naive.replace(tzinfo=datetime.timezone.utc).astimezone(original_tzinfo)
+        timestamp_max = timestamp_max_naive.replace(
+            tzinfo=datetime.timezone.utc
+        ).astimezone(original_tzinfo)
     else:
         timestamp_max = timestamp_max_naive
     return timestamp_max
 
 
 def fetch_concatenated_video(
-        environment_name: str,
-        start: datetime,
-        end: datetime,
-        output_directory: str,
-        camera_names: Optional[List[str]] = None,
-        workers: int = cpu_count() - 1,
-        video_snippet_directory: str = None,
-        overwrite_video_snippets: bool = False,
-        overwrite_concatenated_video: bool = False) -> Optional[pd.DataFrame]:
+    environment_name: str,
+    start: datetime,
+    end: datetime,
+    output_directory: str,
+    camera_names: Optional[List[str]] = None,
+    workers: int = cpu_count() - 1,
+    video_snippet_directory: str = None,
+    overwrite_video_snippets: bool = False,
+    overwrite_concatenated_video: bool = False,
+) -> Optional[pd.DataFrame]:
     """
     Create concatenated video files for each camera in a particular environment given a provided start and end time.
 
     Function will download individual video snippets across each camera, concatenate those snippets, and trim the videos
     to exactly match the provided start and end time.
 
     Args:
@@ -874,47 +933,50 @@
     """
     os.makedirs(output_directory, exist_ok=True)
 
     video_metadata = fetch_video_metadata(
         start=start,
         end=end,
         environment_name=environment_name,
-        camera_names=camera_names
+        camera_names=camera_names,
     )
     if video_metadata is None or len(video_metadata) == 0:
-        logger.warning(f"Found 0 videos for {environment_name} between {start} and {end}")
+        logger.warning(
+            f"Found 0 videos for {environment_name} between {start} and {end}"
+        )
         return None
 
     with tempfile.TemporaryDirectory() as tmp_dir:
         video_snippet_storage_dir = video_snippet_directory
         if video_snippet_directory is None:
             video_snippet_storage_dir = tmp_dir
         else:
             os.makedirs(video_snippet_storage_dir, exist_ok=True)
 
         video_metadata_with_file_paths = download_video_files(
             video_metadata=video_metadata,
             local_video_directory=video_snippet_storage_dir,
             max_workers=workers,
-            overwrite=overwrite_video_snippets
+            overwrite=overwrite_video_snippets,
         )
 
         concatenated_video_output = concat_videos(
             video_metadata=video_metadata_with_file_paths,
             start=start,
             end=end,
             output_directory=output_directory,
-            overwrite=overwrite_concatenated_video
+            overwrite=overwrite_concatenated_video,
         )
 
     return pd.DataFrame(concatenated_video_output)
 
+
 def combine_videos(
-    video_inputs:List[str],
+    video_inputs: List[str],
     output_directory: Optional[str] = None,
-    output_path: Optional[str] = None
+    output_path: Optional[str] = None,
 ):
     return generate_video_mosaic(
         video_inputs=video_inputs,
         output_directory=output_directory,
-        output_path=output_path
-    )
+        output_path=output_path,
+    )
```

### Comparing `wf-video-io-3.2.2/video_io/utils.py` & `wf_video_io-3.2.3/video_io/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 
 from video_io.video_reader import VideoReader
 
 logger = logging.getLogger(__name__)
 
 
 def concat_videos(
-        video_metadata: List[dict],
-        start: datetime,
-        end: datetime,
-        output_directory: str,
-        overwrite: bool = False) -> Optional[List]:
+    video_metadata: List[dict],
+    start: datetime,
+    end: datetime,
+    output_directory: str,
+    overwrite: bool = False,
+) -> Optional[List]:
     """
     Use the output of core.download_video_files() to concatenate videos for each camera into a single video file.
 
     Function will trim video to exactly match the given start and end times.
 
     Args:
         video_metadata (list of dict): Data in the format output by core.download_video_files()
@@ -38,77 +39,101 @@
     """
     video_snippet_length = 10.0
     video_snippet_fps = 10
 
     concatenated_video_output = []
 
     with tempfile.TemporaryDirectory() as tmp_dir:
-        for (environment_id, camera_assignment_id, camera_device_id), df_video_files_by_device in pd.DataFrame(video_metadata).sort_values(by=['device_id', 'video_timestamp']).groupby(['environment_id', 'assignment_id', 'device_id'], dropna=False):
+        for (
+            environment_id,
+            camera_assignment_id,
+            camera_device_id,
+        ), df_video_files_by_device in (
+            pd.DataFrame(video_metadata)
+            .sort_values(by=["device_id", "video_timestamp"])
+            .groupby(["environment_id", "assignment_id", "device_id"], dropna=False)
+        ):
             video_output_path = f"{output_directory}/{environment_id}_{camera_device_id}_{start.strftime('%m%d%YT%H%M%S%f%z')}_{end.strftime('%m%d%YT%H%M%S%f%z')}.mp4"
 
             if not os.path.exists(video_output_path) or overwrite:
                 # tmp_concat_demuxer_file is a temp file containing a list of video files to concatenate. This file
                 # gets input into ffmpeg.
                 with tempfile.NamedTemporaryFile() as tmp_concat_demuxer_file:
                     for idx, video_file_row in df_video_files_by_device.iterrows():
-                        video_path = video_file_row['video_local_path']
+                        video_path = video_file_row["video_local_path"]
                         final_video_snippet_path = video_path
 
                         # TODO: There's an assumption in the following logic that video snippets will be always be 10.0 seconds long, but that may not be true. We should trim/pad videos appropriately before executing the next piece of code
 
-                        video_start_time = video_file_row['video_timestamp']
-                        video_end_time = video_file_row['video_timestamp'] + datetime.timedelta(seconds=video_snippet_length)
+                        video_start_time = video_file_row["video_timestamp"]
+                        video_end_time = video_file_row[
+                            "video_timestamp"
+                        ] + datetime.timedelta(seconds=video_snippet_length)
 
                         start_trim = 0.0
                         end_trim = video_snippet_length
 
                         if start > video_start_time:
-                            start_trim = (start - video_file_row['video_timestamp']).total_seconds()
+                            start_trim = (
+                                start - video_file_row["video_timestamp"]
+                            ).total_seconds()
 
                         if end < video_end_time:
-                            end_trim = video_snippet_length - (video_end_time - end).total_seconds()
+                            end_trim = (
+                                video_snippet_length
+                                - (video_end_time - end).total_seconds()
+                            )
 
                         duration = end_trim - start_trim
                         if duration != video_snippet_length:
                             final_video_snippet_path = f"{tmp_dir}/{environment_id}_{camera_device_id}_{idx}_trimmed_video.mp4"
-                            trim_video(input_path=video_path,
-                                       output_path=final_video_snippet_path,
-                                       start_trim=start_trim,
-                                       end_trim=end_trim,
-                                       fps=video_snippet_fps)
-
-                        tmp_concat_demuxer_file.write(str.encode(f"file \'file:{final_video_snippet_path}'\n"))
+                            trim_video(
+                                input_path=video_path,
+                                output_path=final_video_snippet_path,
+                                start_trim=start_trim,
+                                end_trim=end_trim,
+                                fps=video_snippet_fps,
+                            )
+
+                        tmp_concat_demuxer_file.write(
+                            str.encode(f"file 'file:{final_video_snippet_path}'\n")
+                        )
                         tmp_concat_demuxer_file.flush()
 
-                    ffmpeg.input(f"file:{tmp_concat_demuxer_file.name}",
-                                 format='concat',
-                                 safe=0,
-                                 r=video_snippet_fps) \
-                        .output(f"file:{video_output_path}",
-                                c="copy",
-                                r=video_snippet_fps,
-                                vsync=0) \
-                        .overwrite_output() \
-                        .run()
-
-            concatenated_video_output.append({
-                "environment_id": environment_id,
-                "camera_assignment_id": camera_assignment_id,
-                "camera_device_id": camera_device_id,
-                "file_path": video_output_path})
+                    ffmpeg.input(
+                        f"file:{tmp_concat_demuxer_file.name}",
+                        format="concat",
+                        safe=0,
+                        r=video_snippet_fps,
+                    ).output(
+                        f"file:{video_output_path}",
+                        c="copy",
+                        r=video_snippet_fps,
+                        vsync=0,
+                    ).overwrite_output().run()
+
+            concatenated_video_output.append(
+                {
+                    "environment_id": environment_id,
+                    "camera_assignment_id": camera_assignment_id,
+                    "camera_device_id": camera_device_id,
+                    "file_path": video_output_path,
+                }
+            )
 
     return concatenated_video_output
 
 
 def trim_video(
-        input_path: str,
-        output_path: str,
-        start_trim: float = 0.0,
-        end_trim: Optional[float] = None,
-        fps: int = 10) -> bool:
+    input_path: str,
+    output_path: str,
+    start_trim: float = 0.0,
+    end_trim: Optional[float] = None,
+    fps: int = 10,
+) -> bool:
     """
     Trims video from a given start offset (in seconds) to a given end offset (in seconds).
 
     Trimmed video will be output to the provided output_path. Or, you can overwrite a video file
     by using the same input and output path.
 
     Function also accepts a FPS value. The trimmed output video will be written with this FPS.
@@ -123,68 +148,67 @@
         fps (int): Desired frames per second of output file (default is 10)
 
     Returns:
         (boolean): True if video could be trimmed and output to the given output_path
     """
     logging.info(
         "Trimming video '{}' from {} seconds to {} seconds".format(
-            input_path, start_trim, end_trim))
+            input_path, start_trim, end_trim
+        )
+    )
 
     if not os.path.exists(input_path):
         err = f"'{input_path}' does not exist, unable to trim video. Raising FileNotFoundError exception."
         logger.error(err)
-        raise(FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), err))
+        raise (FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), err))
 
     if end_trim is None:
         video_reader = VideoReader(input_path)
         end_trim = video_reader.duration()
 
     tmp_file = None
     should_overwrite_input = input_path == output_path
     ffmpeg_output_path = output_path
     try:
         if should_overwrite_input:
-            tmp_file = tempfile.NamedTemporaryFile(suffix='.mp4')
+            tmp_file = tempfile.NamedTemporaryFile(suffix=".mp4")
             ffmpeg_output_path = tmp_file.name
 
-        duration_seconds = (end_trim - start_trim)
-        ffmpeg.input(
-                input_path,
-                ss=start_trim,
-                to=end_trim)\
-            .output(
-                ffmpeg_output_path,
-                r=fps,
-                vframes=int(duration_seconds * fps))\
-            .overwrite_output().run()
+        duration_seconds = end_trim - start_trim
+        ffmpeg.input(input_path, ss=start_trim, to=end_trim).output(
+            ffmpeg_output_path, r=fps, vframes=int(duration_seconds * fps)
+        ).overwrite_output().run()
 
         if should_overwrite_input:
             shutil.copy(ffmpeg_output_path, input_path)
     except ffmpeg._run.Error as e:
         logging.error("Failed trimming video {}".format(input_path))
         logging.error(e)
 
         # Cleanup
         if tmp_file is None and os.path.exists(ffmpeg_output_path):
             try:
                 os.remove(ffmpeg_output_path)
             except:
-                logger.error(f"Unable to cleanup {ffmpeg_output_path} after exception trimming video")
+                logger.error(
+                    f"Unable to cleanup {ffmpeg_output_path} after exception trimming video"
+                )
 
         return False
 
     return True
 
+
 def generate_video_mosaic(
-        video_inputs:List[str],
-        output_directory: Optional[str] = None,
-        output_path: Optional[str] = None
+    video_inputs: List[str],
+    output_directory: Optional[str] = None,
+    output_path: Optional[str] = None,
 ):
-    width=None
-    height=None
+    width = None
+    height = None
 
     if output_directory is None and output_path is None:
         raise ValueError("output_directory and output_path cannot both be None")
 
     if len(video_inputs) <= 1:
         raise ValueError("Number of video inputs must be two or greater")
 
@@ -197,54 +221,51 @@
 
     os.makedirs(_output_directory, exist_ok=True)
     ffmpeg_inputs = []
     for f in video_inputs:
         if not os.path.exists(f):
             err = f"'{f}' does not exist, unable to trim video. Raising FileNotFoundError exception."
             logger.error(err)
-            raise(FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), err))
+            raise (FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), err))
         ffmpeg_inputs.append(ffmpeg.input(f))
 
         if width is None or height is None:
             v = VideoReader(f)
             width = int(v.width())
             height = int(v.height())
 
     def get_grid(n):
         if n <= 0:
             return []
 
         row_width = math.ceil(math.sqrt(n))
         shape = []
-        for ii in range(row_width, n+1, row_width):
+        for ii in range(row_width, n + 1, row_width):
             shape.append(row_width)
 
         if n > sum(shape):
             shape.append(n - sum(shape))
 
         return shape
 
     grid = get_grid(len(video_inputs))
 
-    layout=[]
+    layout = []
     ideal_shape = max(grid)
     for row, num_cols in enumerate(grid):
         for col in range(num_cols):
             offset = int((ideal_shape - num_cols) * width * 0.5)
             layout.append(f"{offset + (col * width)}_{row * height}")
 
     vout = ffmpeg.filter(
         list(map(lambda v: v.video, ffmpeg_inputs)),
         "xstack",
         inputs=len(ffmpeg_inputs),
         layout="|".join(layout),
         # fill="black[out]"
     )
 
-    ffmpeg.output(vout,
-                  _output_path,
-                  pix_fmt='yuv420p',
-                  vcodec='libx264') \
-        .overwrite_output() \
-        .run()
+    ffmpeg.output(
+        vout, _output_path, pix_fmt="yuv420p", vcodec="libx264"
+    ).overwrite_output().run()
 
-    return _output_path
+    return _output_path
```

### Comparing `wf-video-io-3.2.2/video_io/video_reader.py` & `wf_video_io-3.2.3/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf-video-io-3.2.2/setup.py` & `wf_video_io-3.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,27 +12,28 @@
  'jmespath>=1.0.1,<2.0.0',
  'opencv-python>=4.6.0',
  'pyyaml>=6.0,<7.0',
  'tenacity>=8.1.0,<9.0.0',
  'urllib3>=1.26.12,<2.0.0',
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
+ 'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.2.2',
+    'version': '3.2.3',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `wf-video-io-3.2.2/PKG-INFO` & `wf_video_io-3.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.2.2
+Version: 3.2.3
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: opencv-python (>=4.6.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Requires-Dist: wf-cv-utils (>=3.4.0)
 Requires-Dist: wf-fastapi-auth0 (>=1.0)
+Requires-Dist: wf-gqlpycgen (>=0.7.4,<0.8.0)
 Requires-Dist: wf-honeycomb-io (>=2.0.0)
 Description-Content-Type: text/markdown
 
 # video_io
 
 Tools for accessing Wildflower video data
```

