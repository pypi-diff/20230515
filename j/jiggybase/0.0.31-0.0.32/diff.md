# Comparing `tmp/jiggybase-0.0.31.tar.gz` & `tmp/jiggybase-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.31.tar", last modified: Mon May 15 04:11:54 2023, max compression
+gzip compressed data, was "jiggybase-0.0.32.tar", last modified: Mon May 15 16:43:48 2023, max compression
```

## Comparing `jiggybase-0.0.31.tar` & `jiggybase-0.0.32.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 04:11:54.603532 jiggybase-0.0.31/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.31/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-15 04:11:54.603102 jiggybase-0.0.31/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.0.31/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 04:11:54.594959 jiggybase-0.0.31/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.31/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     2403 2023-05-14 15:03:38.000000 jiggybase-0.0.31/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     9510 2023-05-15 04:07:01.000000 jiggybase-0.0.31/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 04:11:54.597702 jiggybase-0.0.31/jiggybase/examples/
--rw-r--r--   0 wsk        (501) staff       (20)      214 2023-05-15 03:26:25.000000 jiggybase-0.0.31/jiggybase/examples/chat_completion.py
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.31/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.31/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     5670 2023-05-15 03:33:57.000000 jiggybase-0.0.31/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.31/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 04:11:54.602170 jiggybase-0.0.31/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.31/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.31/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     2426 2023-05-15 03:38:10.000000 jiggybase-0.0.31/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.0.31/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.31/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.31/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.31/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.31/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.31/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     3166 2023-05-14 15:04:22.000000 jiggybase-0.0.31/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.31/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.31/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.31/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.31/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.31/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 04:11:54.596783 jiggybase-0.0.31/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-15 04:11:54.000000 jiggybase-0.0.31/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      890 2023-05-15 04:11:54.000000 jiggybase-0.0.31/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-15 04:11:54.000000 jiggybase-0.0.31/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-15 04:11:54.000000 jiggybase-0.0.31/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-15 04:11:54.000000 jiggybase-0.0.31/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-15 04:11:54.000000 jiggybase-0.0.31/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-15 03:28:45.000000 jiggybase-0.0.31/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-15 04:11:54.603673 jiggybase-0.0.31/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 04:11:54.602596 jiggybase-0.0.31/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.31/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:43:48.436671 jiggybase-0.0.32/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.32/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-15 16:43:48.436087 jiggybase-0.0.32/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.0.32/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:43:48.427367 jiggybase-0.0.32/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.32/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.0.32/jiggybase/chat_stream.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2403 2023-05-15 15:21:13.000000 jiggybase-0.0.32/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)    10620 2023-05-15 16:06:05.000000 jiggybase-0.0.32/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:43:48.430645 jiggybase-0.0.32/jiggybase/examples/
+-rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.0.32/jiggybase/examples/chat_completion.py
+-rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-15 15:35:06.000000 jiggybase-0.0.32/jiggybase/examples/chat_completion_stream.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.32/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.32/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     5705 2023-05-15 15:27:23.000000 jiggybase-0.0.32/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.32/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:43:48.435052 jiggybase-0.0.32/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.32/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.32/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2767 2023-05-15 16:07:13.000000 jiggybase-0.0.32/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.0.32/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.32/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.32/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.32/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.32/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.32/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3166 2023-05-14 15:04:22.000000 jiggybase-0.0.32/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.32/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.32/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.32/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.32/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.32/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:43:48.429059 jiggybase-0.0.32/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-15 16:43:48.000000 jiggybase-0.0.32/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      960 2023-05-15 16:43:48.000000 jiggybase-0.0.32/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-15 16:43:48.000000 jiggybase-0.0.32/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-15 16:43:48.000000 jiggybase-0.0.32/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-15 16:43:48.000000 jiggybase-0.0.32/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-15 16:43:48.000000 jiggybase-0.0.32/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-15 15:19:55.000000 jiggybase-0.0.32/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-15 16:43:48.436788 jiggybase-0.0.32/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:43:48.435470 jiggybase-0.0.32/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.32/test/test.py
```

### Comparing `jiggybase-0.0.31/LICENSE` & `jiggybase-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/PKG-INFO` & `jiggybase-0.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.31
+Version: 0.0.32
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.31/README.md` & `jiggybase-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/client.py` & `jiggybase-0.0.32/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/collection.py` & `jiggybase-0.0.32/jiggybase/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Optional, Tuple, List
+import os
+from typing import Optional, List, Iterator
 from pydantic import BaseModel, Field, BaseConfig, HttpUrl
 from enum import Enum
 from .models import collection, CollectionChatConfig, PatchCollectionChatConfig
 from .jiggybase_session import JiggyBaseSession
 from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter, DocChunksResponse
-from .models import Message, CompletionRequest, ChatCompletion
-import os
-
+from .models import Message, CompletionRequest, ChatCompletion, ChatUsage
+from .chat_stream import extract_content_from_sse_bytes
 
 from typing import Union, List
 class PluginAuthType(Enum):
     bearer :str = "bearer"
     none   :str = "none"
     oauth  :str = "oauth"
 
@@ -57,15 +57,15 @@
     class Config(BaseConfig):
         extra = "allow"
 
     def __init__(self, session, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.session = session
         self.plugin_session = JiggyBaseSession(host=f'https://{kwargs["fqdn"]}', api='')
-        self.chat_session = JiggyBaseSession(api='v1')
+        self.chat_session = JiggyBaseSession(host=session.host, api='v1')
         
     def set_description(self, description:str) -> "Collection":
         """
         Update an existing collection using its ID and the provided description.
         """
         patch_request = CollectionPatchRequest(description=description)
         rsp = self.session.patch(f"/orgs/{self.org_id}/collections/{self.id}", model=patch_request)
@@ -164,15 +164,14 @@
         reverse - Reverse the order of the items returned
         """
         params = {"start": start, "limit": limit, "reverse": reverse}
         rsp = self.plugin_session.get("/chunks", params=params)
         return [DocumentChunk.parse_obj(chunk) for chunk in rsp.json()]
 
 
-
     def delete_docs(self, 
                     ids                      : Optional[List[str]] = None, 
                     document_metadata_filter : Optional[DocumentMetadataFilter] = None, 
                     delete_all               : Optional[bool] = False) -> DeleteResponse:
         """
         Delete items in the collection by document id's or document metadata filter.
         A delete_all option is also provided to delete all documents in the collection.
@@ -192,11 +191,32 @@
         The input here mirrors openai chat completion parameters, while the output is different
         """
         cr = CompletionRequest(model       = f'{self.name}_{model}', 
                                messages    = messages,
                                max_tokens  = max_tokens,
                                temperature = temperature,
                                stream      = False)
-        rsp = self.chat_session.post("/chat/completions", model=cr)                      
-        return ChatCompletion.parse_obj(rsp.json())
+        rsp = self.chat_session.post("/chat/completions", model=cr)          
+        try:            
+            return ChatCompletion.parse_obj(rsp.json())
+        except:
+            return ChatUsage.parse_obj(rsp.json())  # transitional hack
 
-                        
+    def _chat_completion_stream_str(self, 
+                         messages: List[Message],
+                         model = 'gpt-3.5-turbo',
+                         max_tokens = None,
+                         temperature = .1) -> Iterator[str]:
+        """
+        low level interface for chat completion with streaming
+        yields the model output as an iteration of strings
+        """
+        cr = CompletionRequest(model       = f'{self.name}_{model}', 
+                               messages    = messages,
+                               max_tokens  = max_tokens,
+                               temperature = temperature,
+                               stream      = True)
+        rsp = self.chat_session.post("/chat/completions", model=cr, stream=True)
+        for line in rsp.iter_lines():
+            if line:  # filter out keep-alive newlines        
+                yield extract_content_from_sse_bytes(line)
+
```

### Comparing `jiggybase-0.0.31/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.32/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.32/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/jiggybase_session.py` & `jiggybase-0.0.32/jiggybase/jiggybase_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from requests.auth import HTTPBasicAuth
 from requests.packages.urllib3 import Retry
 from requests.adapters import HTTPAdapter
 import requests
 from time import sleep
 from .login import window_open
 
-JIGGYBASE_HOST     = 'https://api.gpt-gateway.com'   # transition to jiggy.ai in progress
+JIGGYBASE_HOST     = os.environ.get('JIGGYBASE_HOST', 'https://api.gpt-gateway.com')   # transition to jiggy.ai in progress
 
 JB_KEY_FILE = os.path.expanduser('~') + '/.jiggybase'   # local file to store user entered apikey 
 
 """
 Retry the following status codes:
 500 Internal Server Error: The server encountered an error while processing the request.
 502 Bad Gateway: The server, while acting as a gateway, received an invalid response from the upstream server.
@@ -38,15 +38,15 @@
 
         host: The url host prefix of the form "https:/api.gpt-gateway.com"
               if host arg is not set, will use 
                     JIGGYBASE_HOST environment variable or "api.gpt-gateway.com" as final default.
 
         api:  The api & version to use. defaults to 'gpt-gateway-v1'
                 
-        final url prefix are of the form "https:/{host}/{api}"
+        final url prefix are of the form "https://{host}/{api}"
         """
         super(JiggyBaseSession, self).__init__(*args, **kwargs)
         if not host.startswith('http'):
             host = f"https://{host}" if not host.startswith('localhost') else f'http://{host}'
         self.host = host
         if api:
             self.prefix_url = f"{host}/{api}"
```

### Comparing `jiggybase-0.0.31/jiggybase/login.py` & `jiggybase-0.0.32/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/auth.py` & `jiggybase-0.0.32/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/chat.py` & `jiggybase-0.0.32/jiggybase/models/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Config for chat-related functionality
 """
 
 from pydantic import BaseModel, Field
 from .chatmodel import ChatModelName
-from typing import Optional
+from typing import Optional, List
 
 
 class CollectionChatConfig(BaseModel):
     """Config for Collection chat-related functionality"""    
     model_name          : str           = Field(description="The model associated with this configuration")
     rate_limit_messages : int           = Field(description="The total number of messages allowed in the rate limit time period across all collection users")
     rate_limit_hours    : int           = Field(description="The number of hours in the rate limit time period")
@@ -32,18 +32,43 @@
     model: str
     messages: list[Message]
     max_tokens: Optional[int] = None
     temperature: float
     stream: bool
 
 
-# Response returned from JiggyBase Chat Completion api endpoint
-# While the inputs to our chat completion api are similar to OpenAI, the output response model is quite different:
+
+
+class Choice(BaseModel):
+    finish_reason: str
+    index: int
+    message: Message
+
+class Usage(BaseModel):
+    completion_tokens: int
+    prompt_tokens: int
+    total_tokens: int
 
 class ChatCompletion(BaseModel):
+    id: str
+    choices: List[Choice]
+    created: int
+    model: str
+    object: str
+    usage: Usage
+
+    def __str__(self):
+        return self.choices[0].message.content
+    
+
+
+class ChatUsage(BaseModel):
+    """
+    JiggyBase chat completion that was temporarily used before transitioning to the OpenAI ChatCompletion
+    """
     collection_id:   int           = Field(description="The collection ID used to inform the completion")
     model:           str           = Field(description="The name of the model used to generate the completion")
     user_message:    str           = Field(description="The user's input message")
     input_tokens:    int           = Field(description="The number of input tokens sent to the model")
     output_tokens:   int           = Field(description="The number of output tokens generated by the model")
     messages_json:   Optional[str] = Field(description="JSON representation of the input messages sent to model endpoint")    
     completion:      Optional[str] = Field(description="The completion text returned by the model")
```

### Comparing `jiggybase-0.0.31/jiggybase/models/chunk.py` & `jiggybase-0.0.32/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/collection.py` & `jiggybase-0.0.32/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/metadata.py` & `jiggybase-0.0.32/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/org.py` & `jiggybase-0.0.32/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/plugin.py` & `jiggybase-0.0.32/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/plugin_config.py` & `jiggybase-0.0.32/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/prompt.py` & `jiggybase-0.0.32/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/providers.py` & `jiggybase-0.0.32/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/models/user.py` & `jiggybase-0.0.32/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase/org.py` & `jiggybase-0.0.32/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.31/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.32/jiggybase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.31
+Version: 0.0.32
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.31/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.32/jiggybase.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
 jiggybase/__init__.py
+jiggybase/chat_stream.py
 jiggybase/client.py
 jiggybase/collection.py
 jiggybase/jiggybase_session.py
 jiggybase/login.py
 jiggybase/org.py
 jiggybase.egg-info/PKG-INFO
 jiggybase.egg-info/SOURCES.txt
 jiggybase.egg-info/dependency_links.txt
 jiggybase.egg-info/entry_points.txt
 jiggybase.egg-info/requires.txt
 jiggybase.egg-info/top_level.txt
 jiggybase/examples/chat_completion.py
+jiggybase/examples/chat_completion_stream.py
 jiggybase/examples/jiggybase_upload.py
 jiggybase/examples/upload_email_example.py
 jiggybase/models/__init__.py
 jiggybase/models/auth.py
 jiggybase/models/chat.py
 jiggybase/models/chatmodel.py
 jiggybase/models/chunk.py
```

### Comparing `jiggybase-0.0.31/pyproject.toml` & `jiggybase-0.0.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.31"
+version = "0.0.32"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.31/test/test.py` & `jiggybase-0.0.32/test/test.py`

 * *Files identical despite different names*

