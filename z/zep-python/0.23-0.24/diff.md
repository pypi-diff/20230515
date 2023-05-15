# Comparing `tmp/zep_python-0.23.tar.gz` & `tmp/zep_python-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.23.tar", max compression
+gzip compressed data, was "zep_python-0.24.tar", max compression
```

## Comparing `zep_python-0.23.tar` & `zep_python-0.24.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-10 23:55:26.241521 zep_python-0.23/LICENSE
--rw-r--r--   0        0        0    11193 2023-05-10 23:55:26.241521 zep_python-0.23/README.md
--rw-r--r--   0        0        0      630 2023-05-10 23:55:26.245521 zep_python-0.23/pyproject.toml
--rw-r--r--   0        0        0      339 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/exceptions.py
--rw-r--r--   0        0        0     6840 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/models.py
--rw-r--r--   0        0        0        0 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/py.typed
--rw-r--r--   0        0        0      670 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/utils.py
--rw-r--r--   0        0        0    11069 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/zep_client.py
--rw-r--r--   0        0        0    11830 1970-01-01 00:00:00.000000 zep_python-0.23/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 20:33:14.641595 zep_python-0.24/LICENSE
+-rw-r--r--   0        0        0    11572 2023-05-15 20:33:14.641595 zep_python-0.24/README.md
+-rw-r--r--   0        0        0      775 2023-05-15 20:33:14.641595 zep_python-0.24/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/exceptions.py
+-rw-r--r--   0        0        0     4861 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/models.py
+-rw-r--r--   0        0        0        0 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/py.typed
+-rw-r--r--   0        0        0      670 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/utils.py
+-rw-r--r--   0        0        0    12664 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/zep_client.py
+-rw-r--r--   0        0        0    12251 1970-01-01 00:00:00.000000 zep_python-0.24/PKG-INFO
```

### Comparing `zep_python-0.23/LICENSE` & `zep_python-0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.23/README.md` & `zep_python-0.24/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml)
+[![Tests](https://github.com/getzep/zep-python/actions/workflows/test.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/test.yml) [![lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-python?color=blue)
 
 # Zep: A long-term memory store for conversational AI applications
 
 This is the Python client package for the Zep service. For more information about Zep, see https://github.com/getzep/zep.
 
 ### Installation
```

### Comparing `zep_python-0.23/pyproject.toml` & `zep_python-0.24/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.23"
+version = "0.24"
 description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.0"
+pydantic = "^1.10.7"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3.1"
+pytest-httpx = "^0.22.0"
+pytest-asyncio = "^0.21.0"
+ruff = "^0.0.265"
+mypy = "^1.2.0"
+pytest-mock = "^3.10.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.265"
 mypy = "^1.2.0"
 pre-commit = "^3.3.1"
 sphinxawesome-theme = "^4.0.3"
-pytest = "^7.3.1"
-pytest-httpx = "^0.22.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zep_python-0.23/zep_python/exceptions.py` & `zep_python-0.24/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.23/zep_python/utils.py` & `zep_python-0.24/zep_python/utils.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.23/zep_python/zep_client.py` & `zep_python-0.24/zep_python/zep_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
+import asyncio
 from types import TracebackType
 from typing import List, Optional, Type
 
 import httpx
 
 from zep_python.exceptions import APIError, NotFoundError
-from zep_python.models import Memory, SearchPayload, SearchResult
+from zep_python.models import Memory, Message, SearchPayload, SearchResult, Summary
 from zep_python.utils import sync
 
 API_BASEURL = "/api/v1"
 
 
 class ZepClient:
     """
@@ -50,27 +51,38 @@
         self.base_url = base_url
         self.client = httpx.AsyncClient()
 
     # Asynchronous context manager entry point
     async def __aenter__(self) -> "ZepClient":
         return self
 
-    # Asynchronous context manager exit point
+    # Sync context manager exit point
     async def __aexit__(
         self,
         exc_type: Type[Exception],
         exc_val: Exception,
         exc_tb: TracebackType,
     ) -> None:
-        await self.close()
+        await self.aclose()
+
+    # Asynchronous context manager entry point
+    def __enter__(self) -> "ZepClient":
+        return self
+
+    # Sync context manager exit point
+    def __exit__(
+        self,
+        exc_type: Type[Exception],
+        exc_val: Exception,
+        exc_tb: TracebackType,
+    ) -> None:
+        self.close()
 
     @sync
-    def get_memory(
-        self, session_id: str, lastn: Optional[int] = None
-    ) -> List[Memory]:
+    def get_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]:
         """
         Retrieve memory for the specified session. This method is a synchronous wrapper
         for the asynchronous method `aget_memory`.
 
         Parameters
         ----------
         session_id : str
@@ -87,14 +99,17 @@
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
         # we've wrapped the function in a decorator that will run it synchronously.
         # ignore the type error.
+        if session_id is None or session_id == "":
+            raise ValueError("session_id must be provided")
+
         return self.aget_memory(session_id, lastn)  # type: ignore
 
     async def aget_memory(
         self, session_id: str, lastn: Optional[int] = None
     ) -> List[Memory]:
         """
         Asynchronously retrieve memory for the specified session.
@@ -113,44 +128,52 @@
             A list of Memory objects representing the retrieved memory entries.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
+        if session_id is None or session_id == "":
+            raise ValueError("session_id must be provided")
+
         url = f"{self.base_url}{API_BASEURL}/sessions/{session_id}/memory"
         params = (
             {"lastn": lastn} if lastn is not None else {}
         )  # Include 'lastn' as a query parameter if provided
         response = await self.client.get(url, params=params)
 
         if response.status_code == 404:
             raise NotFoundError(f"No memory found for session {session_id}")
 
         if response.status_code != 200:
             raise APIError(f"Unexpected status code: {response.status_code}")
 
         response_data = response.json()
-
-        # Check if the response contains the expected field 'messages'.
-        if "messages" in response_data:
-            # If 'messages' is None, return an empty list.
-            if response_data["messages"] is None:
-                return []
-            # Create a Memory instance using the 'messages' field from the response.
-            memory = Memory(
-                messages=response_data["messages"],
-                # Add the 'summary' field if it is present in the response.
-                summary=response_data.get("summary", None),
-                # Add any other fields from the response that are relevant to the
-                # Memory class.
-            )
-            return [memory]
-        else:
-            raise APIError("Unexpected response format from the API")
+        messages: List[Message]
+        try:
+            messages = [
+                Message.parse_obj(m) for m in response_data.get("messages", None)
+            ]
+            if len(messages) == 0:
+                raise ValueError("Messages can't be empty")
+        except (TypeError, ValueError) as e:
+            raise APIError("Unexpected response format from the API") from e
+
+        summary: Optional[Summary] = None
+        if response_data.get("summary", None) is not None:
+            summary = Summary.parse_obj(response_data["summary"])
+
+        memory = Memory(
+            messages=messages,
+            # Add the 'summary' field if it is present in the response.
+            summary=summary,
+            # Add any other fields from the response that are relevant to the
+            # Memory class.
+        )
+        return [memory]
 
     @sync
     def add_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
         Add memory to the specified session. This method is a synchronous wrapper for
         the asynchronous method `aadd_memory`.
 
@@ -169,19 +192,20 @@
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
         # we've wrapped the function in a decorator that will run it synchronously.
         # ignore the type error.
+        if session_id is None or session_id == "":
+            raise ValueError("session_id must be provided")
+
         return self.aadd_memory(session_id, memory_messages)  # type: ignore
 
-    async def aadd_memory(
-        self, session_id: str, memory_messages: Memory
-    ) -> str:
+    async def aadd_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
         Asynchronously add memory to the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session to which memory should be added.
@@ -194,17 +218,20 @@
             The response text from the API.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
+        if session_id is None or session_id == "":
+            raise ValueError("session_id must be provided")
+
         response = await self.client.post(
             f"{self.base_url}{API_BASEURL}/sessions/{session_id}/memory",
-            json=memory_messages.to_dict(),
+            json=memory_messages.dict(exclude_none=True),
         )
         if response.status_code != 200:
             raise APIError(f"Unexpected status code: {response.status_code}")
 
         return response.text
 
     @sync
@@ -226,14 +253,17 @@
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
         # we've wrapped the function in a decorator that will run it synchronously.
         # ignore the type error.
+        if session_id is None or session_id == "":
+            raise ValueError("session_id must be provided")
+
         return self.adelete_memory(session_id)  # type: ignore
 
     async def adelete_memory(self, session_id: str) -> str:
         """
         Asynchronously delete memory for the specified session.
 
         Parameters
@@ -247,14 +277,17 @@
             The response text from the API.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
+        if session_id is None or session_id == "":
+            raise ValueError("session_id must be provided")
+
         response = await self.client.delete(
             f"{self.base_url}{API_BASEURL}/sessions/{session_id}/memory"
         )
         if response.status_code == 404:
             raise NotFoundError(f"No session found for session {session_id}")
 
         if response.status_code != 200:
@@ -289,14 +322,17 @@
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
         # we've wrapped the function in a decorator that will run it synchronously.
         # ignore the type error.
+        if session_id is None or session_id == "":
+            raise ValueError("session_id must be provided")
+
         return self.asearch_memory(session_id, search_payload, limit)  # type: ignore
 
     async def asearch_memory(
         self,
         session_id: str,
         search_payload: SearchPayload,
         limit: Optional[int] = None,
@@ -319,29 +355,42 @@
             A list of SearchResult objects representing the search results.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
+        if session_id is None or session_id == "":
+            raise ValueError("session_id must be provided")
+
+        if search_payload is None:
+            raise ValueError("search_payload must be provided")
+
         params = {"limit": limit} if limit is not None else {}
         response = await self.client.post(
             f"{self.base_url}{API_BASEURL}/sessions/{session_id}/search",
-            json=search_payload.__dict__,
+            json=search_payload.dict(),
             params=params,
         )
         if response.status_code == 404:
             raise NotFoundError("No query results found")
         if response.status_code != 200:
             raise APIError(f"Unexpected status code: {response.status_code}")
-        return [
-            SearchResult(**search_result) for search_result in response.json()
-        ]
+        return [SearchResult(**search_result) for search_result in response.json()]
 
-    async def close(self) -> None:
+    async def aclose(self) -> None:
         """
         Asynchronously close the HTTP client.
 
         [Optional] This method may be called when the ZepClient is no longer needed to
         release resources.
         """
         await self.client.aclose()
+
+    def close(self) -> None:
+        """
+        Close the HTTP client.
+
+        [Optional] This method may be called when the ZepClient is no longer needed to
+        release resources.
+        """
+        asyncio.run(self.client.aclose())
```

### Comparing `zep_python-0.23/PKG-INFO` & `zep_python-0.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 0.23
+Version: 0.24
 Summary: Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
 
-[![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml)
+[![Tests](https://github.com/getzep/zep-python/actions/workflows/test.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/test.yml) [![lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-python?color=blue)
 
 # Zep: A long-term memory store for conversational AI applications
 
 This is the Python client package for the Zep service. For more information about Zep, see https://github.com/getzep/zep.
 
 ### Installation
```

