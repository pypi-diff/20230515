# Comparing `tmp/qget-0.1.5.tar.gz` & `tmp/qget-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qget-0.1.5.tar", last modified: Wed Jan 25 19:34:42 2023, max compression
+gzip compressed data, was "qget-0.1.6.tar", last modified: Mon May 15 17:02:02 2023, max compression
```

## Comparing `qget-0.1.5.tar` & `qget-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 19:34:42.148364 qget-0.1.5/
--rw-rw-rw-   0        0        0    11514 2023-01-25 19:16:00.000000 qget-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       35 2022-05-30 17:16:20.000000 qget-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0    13212 2023-01-25 19:34:42.148364 qget-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    12352 2023-01-25 19:16:06.000000 qget-0.1.5/README.rst
--rw-rw-rw-   0        0        0       90 2022-05-31 12:54:59.000000 qget-0.1.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-01-25 19:34:42.132363 qget-0.1.5/qget/
--rw-rw-rw-   0        0        0      311 2023-01-25 19:06:43.000000 qget-0.1.5/qget/__init__.py
--rw-rw-rw-   0        0        0     7820 2023-01-25 19:15:45.000000 qget-0.1.5/qget/__main__.py
--rw-rw-rw-   0        0        0    33154 2023-01-25 19:14:34.000000 qget-0.1.5/qget/qget_aio.py
-drwxrwxrwx   0        0        0        0 2023-01-25 19:34:42.147363 qget-0.1.5/qget.egg-info/
--rw-rw-rw-   0        0        0    13212 2023-01-25 19:34:42.000000 qget-0.1.5/qget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-01-25 19:34:42.000000 qget-0.1.5/qget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 19:34:42.000000 qget-0.1.5/qget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-01-25 19:34:42.000000 qget-0.1.5/qget.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-01-25 19:34:42.000000 qget-0.1.5/qget.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1061 2023-01-25 19:34:42.152363 qget-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 17:02:02.889627 qget-0.1.6/
+-rw-rw-rw-   0        0        0    11514 2023-01-25 19:16:00.000000 qget-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       35 2022-05-30 17:16:20.000000 qget-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    13762 2023-05-15 17:02:02.889627 qget-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12902 2023-05-15 16:45:51.000000 qget-0.1.6/README.rst
+-rw-rw-rw-   0        0        0       90 2022-05-31 12:54:59.000000 qget-0.1.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-15 17:02:02.873625 qget-0.1.6/qget/
+-rw-rw-rw-   0        0        0      311 2023-05-15 16:41:30.000000 qget-0.1.6/qget/__init__.py
+-rw-rw-rw-   0        0        0     8234 2023-05-15 16:45:48.000000 qget-0.1.6/qget/__main__.py
+-rw-rw-rw-   0        0        0    35176 2023-05-15 16:43:22.000000 qget-0.1.6/qget/qget_aio.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:02:02.889627 qget-0.1.6/qget.egg-info/
+-rw-rw-rw-   0        0        0    13762 2023-05-15 17:02:02.000000 qget-0.1.6/qget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-15 17:02:02.000000 qget-0.1.6/qget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 17:02:02.000000 qget-0.1.6/qget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-15 17:02:02.000000 qget-0.1.6/qget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-15 17:02:02.000000 qget-0.1.6/qget.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1061 2023-05-15 17:02:02.894626 qget-0.1.6/setup.cfg
```

### Comparing `qget-0.1.5/LICENSE` & `qget-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qget-0.1.5/PKG-INFO` & `qget-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qget
-Version: 0.1.5
+Version: 0.1.6
 Summary: Async http(s) downloader
 Home-page: https://github.com/dwojtasik/qget
 Author: Dominik Wojtasik
 Author-email: d.b.wojtasik@gmail.com
 License: Apache 2
 Project-URL: Bug Tracker, https://github.com/dwojtasik/qget/issues
 Classifier: Environment :: Console
@@ -49,14 +49,15 @@
 ========
 
 - an executable script to download file via command line
 - support for HTTPS connection with basic auth and SSL verification skip
 - support for custom headers
 - automatic measurement of simultaneous connections limit
 - support for limiting download rate
+- support for retries during part downloading
 - support for downloading / rewriting progress with callbacks (by default using ``tqdm``)
 - support for limiting RAM usage with settings ``chunk_bytes`` and ``max_part_mb``
 - support for using own event loop in ``asyncio`` by ``qget_coro`` coroutine
 - support for SOCKS4(a), SOCKS5(h), HTTP (tunneling) proxy
 
 Motivation: ``wget`` vs ``qget``
 ================================
@@ -166,14 +167,16 @@
   connection_test_sec (int, optional): Maximum time in seconds assigned to test
       how much asynchronous connections can be achieved to URL.
       If set to 0 test will be omitted. Defaults to 5.
   chunk_bytes (int, optional): Chunk of data read in iteration from url and save to part file in bytes.
       Will be used also when rewriting parts to output file. If limit is supplied this can be override for
       stream iteration. Defaults to 2621440.
   max_part_mb (float, optional): Desirable (if possible) max part size in megabytes. Defaults to 5.
+  retries (int, optional): Retries number for part download. Defaults to 10.
+  retry_sec (int, optional): Time to wait between retries of part download in seconds. Defaults to 1.
   limit (str, optional): Download rate limit in MBps. Can be supplied with unit as "Nunit", eg. "5M".
       Valid units (case insensitive): b, k, m, g, kb, mb, gb. 0 bytes will be treat as no limit.
       Defaults to None.
   tmp_dir (str, optional): Temporary directory path. If not set it points to OS tmp directory.
       Defaults to None.
   debug (bool, optional): Debug flag. Defaults to False.
 
@@ -267,14 +270,16 @@
                           Maximum amount of asynchronous HTTP connections.
     --test CONNECTION_TEST_SEC
                           Maximum time in seconds assigned to test how much asynchronous
                           connections can be achieved to URL. Use 0 to skip.
     --bytes CHUNK_BYTES   Chunk of data read in iteration from url and save to part file in
                           bytes. Will be used also when rewriting parts to output file.
     --part MAX_PART_MB    Desirable (if possible) max part size in megabytes.
+    --retries RETRIES     Retries number for part download.
+    --retry_sec RETRY_SEC Time to wait between retries of part download in seconds.
     --limit LIMIT         Download rate limit in MBps. Can be supplied with unit as 'Nunit',
                           eg. '5M'. Valid units (case insensitive): b, k, m, g, kb, mb, gb.
                           0 bytes will be treat as no limit.
     --tmp TMP_DIR         Temporary directory path. If not set it points to OS tmp
                           directory.
     --debug               Debug flag.
     -v, --version         Displays actual version of qget.
@@ -311,14 +316,19 @@
 
 .. code-block:: text
 
    part_bytes = min(resource_bytes/connections, max_part_bytes)
 
 History
 =======
+0.1.6 (2023-05-15)
+------------------
+- Fixed multiple logging handlers created with multiple qget calls.
+- Added retries for connection errors during async downloading.
+
 0.1.5 (2023-01-25)
 ------------------
 - Updated copyright note.
 
 0.1.4 (2022-08-25)
 ------------------
 - Added support for SOCKS4(a), SOCKS5(h), HTTP (tunneling) proxy.
@@ -344,8 +354,8 @@
 - Fixed fallback to GET request on failed HEAD Content-Length read.
 - Fixed binary build scripts.
 
 0.0.1 (2022-05-31)
 ------------------
 - Initial version.
 
-.. |latest_version| replace:: 0.1.5
+.. |latest_version| replace:: 0.1.6
```

### Comparing `qget-0.1.5/README.rst` & `qget-0.1.6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ========
 
 - an executable script to download file via command line
 - support for HTTPS connection with basic auth and SSL verification skip
 - support for custom headers
 - automatic measurement of simultaneous connections limit
 - support for limiting download rate
+- support for retries during part downloading
 - support for downloading / rewriting progress with callbacks (by default using ``tqdm``)
 - support for limiting RAM usage with settings ``chunk_bytes`` and ``max_part_mb``
 - support for using own event loop in ``asyncio`` by ``qget_coro`` coroutine
 - support for SOCKS4(a), SOCKS5(h), HTTP (tunneling) proxy
 
 Motivation: ``wget`` vs ``qget``
 ================================
@@ -143,14 +144,16 @@
   connection_test_sec (int, optional): Maximum time in seconds assigned to test
       how much asynchronous connections can be achieved to URL.
       If set to 0 test will be omitted. Defaults to 5.
   chunk_bytes (int, optional): Chunk of data read in iteration from url and save to part file in bytes.
       Will be used also when rewriting parts to output file. If limit is supplied this can be override for
       stream iteration. Defaults to 2621440.
   max_part_mb (float, optional): Desirable (if possible) max part size in megabytes. Defaults to 5.
+  retries (int, optional): Retries number for part download. Defaults to 10.
+  retry_sec (int, optional): Time to wait between retries of part download in seconds. Defaults to 1.
   limit (str, optional): Download rate limit in MBps. Can be supplied with unit as "Nunit", eg. "5M".
       Valid units (case insensitive): b, k, m, g, kb, mb, gb. 0 bytes will be treat as no limit.
       Defaults to None.
   tmp_dir (str, optional): Temporary directory path. If not set it points to OS tmp directory.
       Defaults to None.
   debug (bool, optional): Debug flag. Defaults to False.
 
@@ -244,14 +247,16 @@
                           Maximum amount of asynchronous HTTP connections.
     --test CONNECTION_TEST_SEC
                           Maximum time in seconds assigned to test how much asynchronous
                           connections can be achieved to URL. Use 0 to skip.
     --bytes CHUNK_BYTES   Chunk of data read in iteration from url and save to part file in
                           bytes. Will be used also when rewriting parts to output file.
     --part MAX_PART_MB    Desirable (if possible) max part size in megabytes.
+    --retries RETRIES     Retries number for part download.
+    --retry_sec RETRY_SEC Time to wait between retries of part download in seconds.
     --limit LIMIT         Download rate limit in MBps. Can be supplied with unit as 'Nunit',
                           eg. '5M'. Valid units (case insensitive): b, k, m, g, kb, mb, gb.
                           0 bytes will be treat as no limit.
     --tmp TMP_DIR         Temporary directory path. If not set it points to OS tmp
                           directory.
     --debug               Debug flag.
     -v, --version         Displays actual version of qget.
@@ -288,14 +293,19 @@
 
 .. code-block:: text
 
    part_bytes = min(resource_bytes/connections, max_part_bytes)
 
 History
 =======
+0.1.6 (2023-05-15)
+------------------
+- Fixed multiple logging handlers created with multiple qget calls.
+- Added retries for connection errors during async downloading.
+
 0.1.5 (2023-01-25)
 ------------------
 - Updated copyright note.
 
 0.1.4 (2022-08-25)
 ------------------
 - Added support for SOCKS4(a), SOCKS5(h), HTTP (tunneling) proxy.
@@ -321,8 +331,8 @@
 - Fixed fallback to GET request on failed HEAD Content-Length read.
 - Fixed binary build scripts.
 
 0.0.1 (2022-05-31)
 ------------------
 - Initial version.
 
-.. |latest_version| replace:: 0.1.5
+.. |latest_version| replace:: 0.1.6
```

### Comparing `qget-0.1.5/qget/__main__.py` & `qget-0.1.6/qget/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,14 +134,28 @@
         "--part",
         type=float,
         dest="max_part_mb",
         default=default_args["max_part_mb"],
         help="Desirable (if possible) max part size in megabytes.",
     )
     parser.add_argument(
+        "--retries",
+        type=int,
+        dest="retries",
+        default=default_args["retries"],
+        help="Retries number for part download.",
+    )
+    parser.add_argument(
+        "--retry_sec",
+        type=int,
+        dest="retry_sec",
+        default=default_args["retry_sec"],
+        help="Time to wait between retries of part download in seconds.",
+    )
+    parser.add_argument(
         "--limit",
         type=str,
         dest="limit",
         default=default_args["limit"],
         help="Download rate limit in MBps. Can be supplied with unit as 'Nunit', eg. '5M'. "
         + "Valid units (case insensitive): b, k, m, g, kb, mb, gb. 0 bytes will be treat as no limit.",
     )
```

### Comparing `qget-0.1.5/qget/qget_aio.py` & `qget-0.1.6/qget/qget_aio.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import logging
 import math
 import os
 import sys
 import tempfile
 import time
 from dataclasses import dataclass
-from typing import Callable, Dict
+from typing import Awaitable, Callable, Dict
 from urllib.parse import unquote, urlparse
 from python_socks import parse_proxy_url
 
 import aiofiles
 import aiohttp
 from aiohttp_socks import ProxyConnector
 
@@ -245,14 +245,16 @@
     Returns:
         logging.Logger: The configured logger.
     """
     logger = logging.getLogger("aio_download")
     logger.setLevel(logging.DEBUG if debug else logging.ERROR)
     handler = logging.StreamHandler(sys.stdout)
     handler.setLevel(logging.DEBUG if debug else logging.ERROR)
+    if logger.hasHandlers():
+        logger.handlers.clear()
     logger.addHandler(handler)
     return logger
 
 
 def _to_human_readable_unit(byte_count: int, out_format: str = "%.2f %s") -> str:
     """Returns byte count as human readable string.
 
@@ -492,59 +494,95 @@
     except ValueError as ex:
         raise ValueError(f"Parameter limit has invalid numeric value. Actual value: {limit}.") from ex
     if value < 0:
         raise ValueError(f"Parameter limit cannot be negative. Actual value: {limit}.")
     return value
 
 
+async def _with_retries(
+    code: Callable[[], Awaitable[None]], retries: int = 10, retry_sec: int = 1, exception: Exception = None
+) -> None:
+    """Retries code block execution.
+
+    Args:
+        code (Callable[[], Awaitable[None]]): Code to execute in form of async callback.
+        retries (int, optional): Retries number. Defaults to 10.
+        retry_sec (int, optional): Time to wait between retries in seconds. Defaults to 1.
+        exception (Exception, optional): Exception thrown meanwhile code execution. Defaults to None.
+
+    Raises:
+        exception: Exception thrown meanwhile execution. Thrown only when retries run out.
+    """
+    if retries < 0:
+        if exception is not None:
+            raise exception
+        return
+    try:
+        await code()
+    except Exception as ex:  # pylint: disable=broad-except
+        await asyncio.sleep(retry_sec)
+        await _with_retries(code, retries - 1, retry_sec, ex)
+
+
 async def _download_part(
     session: aiohttp.ClientSession,
     url: str,
     tmp_dir: str,
     part_data: PartData,
     chunk_bytes: int,
+    retries: int,
+    retry_sec: int,
     limiter: Limiter = None,
     progress_ref: ProgressState = None,
 ) -> None:
     """Downloads part of resource URL and stores it in temporary file.
 
     Args:
         session (aiohttp.ClientSession): Session that is used to create requests.
         url (str): The resource URL.
         tmp_dir (str): Temporary directory path to save part file.
         part_data (PartData): Basic informations about part.
         chunk_bytes (int): Chunk of data read in iteration from url and save to part file in bytes.
+        retries (int): Retries number.
+        retry_sec (int): Time to wait between retries in seconds.
         limiter (Limiter, optional): Limiter for download rate. If supplied FileBuffer will be used and chunk_bytes
             for stream iteration will be overridden with new calculated value. Defaults to None.
         progress_ref (ProgressState, optional): Reference to progress state.
             If passed part bytes will be updated in it. Defaults to None.
     """
     has_limit = limiter is not None
     iter_size = limiter.chunk_bytes if has_limit else chunk_bytes
-    async with session.get(
-        url,
-        headers={
-            "range": f"bytes={part_data.begin}-{part_data.end}",
-        },
-        timeout=None,
-    ) as response:
-        async with aiofiles.open(f"{tmp_dir}/part-{part_data.part_id}.cr", "wb") as part_file:
-            if has_limit:
-                file_buffer = FileBuffer(part_file, chunk_bytes)
-            async for chunk in response.content.iter_chunked(iter_size):
-                byte_count = len(chunk)
-                if progress_ref:
-                    progress_ref.update_part_progress(part_data.part_id, byte_count)
+
+    async def _download_call():
+        """Download callable code block used for retries"""
+        async with session.get(
+            url,
+            headers={
+                "range": f"bytes={part_data.begin}-{part_data.end}",
+            },
+            timeout=None,
+        ) as response:
+            if progress_ref:
+                progress_ref.parts_bytes[part_data.part_id] = 0
+            async with aiofiles.open(f"{tmp_dir}/part-{part_data.part_id}.cr", "wb") as part_file:
+                if has_limit:
+                    file_buffer = FileBuffer(part_file, chunk_bytes)
+                async for chunk in response.content.iter_chunked(iter_size):
+                    byte_count = len(chunk)
+                    if progress_ref:
+                        progress_ref.update_part_progress(part_data.part_id, byte_count)
+                    if has_limit:
+                        await limiter.throttle(byte_count)
+                        await file_buffer.write(chunk)
+                    else:
+                        await part_file.write(chunk)
                 if has_limit:
-                    await limiter.throttle(byte_count)
-                    await file_buffer.write(chunk)
-                else:
-                    await part_file.write(chunk)
-            if has_limit:
-                await file_buffer.close()
+                    await file_buffer.close()
+
+    await _with_retries(_download_call, retries, retry_sec)
 
 
 async def _rewrite_parts(filepath: str, tmp_dir: str, chunk_bytes: int, progress_ref: ProgressState = None) -> None:
     """Joins and removes all part files into output file.
 
     Args:
         filepath (str): Output path for joined file.
@@ -579,14 +617,16 @@
     proxy_url: str = None,
     headers: Dict[str, str] = None,
     progress_ref: ProgressState = None,
     max_connections: int = 50,
     connection_test_sec: int = 5,
     chunk_bytes: int = 2621440,
     max_part_mb: float = 5.0,
+    retries: int = 10,
+    retry_sec: int = 1,
     limit: str = None,
     tmp_dir: str = None,
     debug: bool = False,
 ) -> None:
     """Download resource from given URL in buffered parts using asynchronous HTTP(S) connections with aiohttp session.
 
     Args:
@@ -608,14 +648,16 @@
         max_connections (int, optional): Maximum amount of asynchronous HTTP connections. Defaults to 50.
         connection_test_sec (int, optional): Maximum time in seconds assigned to test
             how much asynchronous connections can be achieved to URL. If set to 0 test will be omitted. Defaults to 5.
         chunk_bytes (int, optional): Chunk of data read in iteration from url and save to part file in bytes.
             Will be used also when rewriting parts to output file. If limit is supplied this can be override for
             stream iteration. Defaults to 2621440.
         max_part_mb (float, optional): Desirable (if possible) max part size in megabytes. Defaults to 5.
+        retries (int, optional): Retries number for part download. Defaults to 10.
+        retry_sec (int, optional): Time to wait between retries of part download in seconds. Defaults to 1.
         limit (str, optional): Download rate limit in MBps. Can be supplied with unit as "Nunit", eg. "5M".
             Valid units (case insensitive): b, k, m, g, kb, mb, gb. 0 bytes will be treat as no limit.
             Defaults to None.
         tmp_dir (str, optional): Temporary directory path. If not set it points to OS tmp directory. Defaults to None.
         debug (bool, optional): Debug flag. Defaults to False.
 
     Raises:
@@ -702,14 +744,16 @@
                     tmp_dir,
                     PartData(
                         str(part).zfill(part_zfill),
                         begin,
                         resource_bytes if part == part_count - 1 else begin + part_bytes - 1,
                     ),
                     chunk_bytes,
+                    retries,
+                    retry_sec,
                     limiter,
                     progress_ref,
                 )
             )
             for part, begin in enumerate(range(0, resource_bytes, part_bytes))
         ]
 
@@ -759,14 +803,16 @@
             If passed all parts bytes and rewrite status will be updated in it. Defaults to None.
         max_connections (int, optional): Maximum amount of asynchronous HTTP connections. Defaults to 50.
         connection_test_sec (int, optional): Maximum time in seconds assigned to test
             how much asynchronous connections can be achieved to URL. If set to 0 test will be omitted. Defaults to 5.
         chunk_bytes (int, optional): Chunk of data read in iteration from url and save to part file in bytes.
             Will be used also when rewriting parts to output file. Defaults to 2621440.
         max_part_mb (float, optional): Desirable (if possible) max part size in megabytes. Defaults to 5.
+        retries (int, optional): Retries number for part download. Defaults to 10.
+        retry_sec (int, optional): Time to wait between retries of part download in seconds. Defaults to 1.
         limit (str, optional): Download rate limit in MBps. Can be supplied with unit as "Nunit", eg. "5M".
             Valid units (case insensitive): b, k, m, g, kb, mb, gb. 0 bytes will be treat as no limit.
             Defaults to None.
         tmp_dir (str, optional): Temporary directory path. If not set it points to OS tmp directory. Defaults to None.
         debug (bool, optional): Debug flag. Defaults to False.
     """
```

### Comparing `qget-0.1.5/qget.egg-info/PKG-INFO` & `qget-0.1.6/qget.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qget
-Version: 0.1.5
+Version: 0.1.6
 Summary: Async http(s) downloader
 Home-page: https://github.com/dwojtasik/qget
 Author: Dominik Wojtasik
 Author-email: d.b.wojtasik@gmail.com
 License: Apache 2
 Project-URL: Bug Tracker, https://github.com/dwojtasik/qget/issues
 Classifier: Environment :: Console
@@ -49,14 +49,15 @@
 ========
 
 - an executable script to download file via command line
 - support for HTTPS connection with basic auth and SSL verification skip
 - support for custom headers
 - automatic measurement of simultaneous connections limit
 - support for limiting download rate
+- support for retries during part downloading
 - support for downloading / rewriting progress with callbacks (by default using ``tqdm``)
 - support for limiting RAM usage with settings ``chunk_bytes`` and ``max_part_mb``
 - support for using own event loop in ``asyncio`` by ``qget_coro`` coroutine
 - support for SOCKS4(a), SOCKS5(h), HTTP (tunneling) proxy
 
 Motivation: ``wget`` vs ``qget``
 ================================
@@ -166,14 +167,16 @@
   connection_test_sec (int, optional): Maximum time in seconds assigned to test
       how much asynchronous connections can be achieved to URL.
       If set to 0 test will be omitted. Defaults to 5.
   chunk_bytes (int, optional): Chunk of data read in iteration from url and save to part file in bytes.
       Will be used also when rewriting parts to output file. If limit is supplied this can be override for
       stream iteration. Defaults to 2621440.
   max_part_mb (float, optional): Desirable (if possible) max part size in megabytes. Defaults to 5.
+  retries (int, optional): Retries number for part download. Defaults to 10.
+  retry_sec (int, optional): Time to wait between retries of part download in seconds. Defaults to 1.
   limit (str, optional): Download rate limit in MBps. Can be supplied with unit as "Nunit", eg. "5M".
       Valid units (case insensitive): b, k, m, g, kb, mb, gb. 0 bytes will be treat as no limit.
       Defaults to None.
   tmp_dir (str, optional): Temporary directory path. If not set it points to OS tmp directory.
       Defaults to None.
   debug (bool, optional): Debug flag. Defaults to False.
 
@@ -267,14 +270,16 @@
                           Maximum amount of asynchronous HTTP connections.
     --test CONNECTION_TEST_SEC
                           Maximum time in seconds assigned to test how much asynchronous
                           connections can be achieved to URL. Use 0 to skip.
     --bytes CHUNK_BYTES   Chunk of data read in iteration from url and save to part file in
                           bytes. Will be used also when rewriting parts to output file.
     --part MAX_PART_MB    Desirable (if possible) max part size in megabytes.
+    --retries RETRIES     Retries number for part download.
+    --retry_sec RETRY_SEC Time to wait between retries of part download in seconds.
     --limit LIMIT         Download rate limit in MBps. Can be supplied with unit as 'Nunit',
                           eg. '5M'. Valid units (case insensitive): b, k, m, g, kb, mb, gb.
                           0 bytes will be treat as no limit.
     --tmp TMP_DIR         Temporary directory path. If not set it points to OS tmp
                           directory.
     --debug               Debug flag.
     -v, --version         Displays actual version of qget.
@@ -311,14 +316,19 @@
 
 .. code-block:: text
 
    part_bytes = min(resource_bytes/connections, max_part_bytes)
 
 History
 =======
+0.1.6 (2023-05-15)
+------------------
+- Fixed multiple logging handlers created with multiple qget calls.
+- Added retries for connection errors during async downloading.
+
 0.1.5 (2023-01-25)
 ------------------
 - Updated copyright note.
 
 0.1.4 (2022-08-25)
 ------------------
 - Added support for SOCKS4(a), SOCKS5(h), HTTP (tunneling) proxy.
@@ -344,8 +354,8 @@
 - Fixed fallback to GET request on failed HEAD Content-Length read.
 - Fixed binary build scripts.
 
 0.0.1 (2022-05-31)
 ------------------
 - Initial version.
 
-.. |latest_version| replace:: 0.1.5
+.. |latest_version| replace:: 0.1.6
```

### Comparing `qget-0.1.5/setup.cfg` & `qget-0.1.6/setup.cfg`

 * *Files identical despite different names*

