# Comparing `tmp/tradernet_sdk-0.3.4.tar.gz` & `tmp/tradernet_sdk-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradernet_sdk-0.3.4.tar", max compression
+gzip compressed data, was "tradernet_sdk-0.3.7.tar", max compression
```

## Comparing `tradernet_sdk-0.3.4.tar` & `tradernet_sdk-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1131 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/LICENSE
--rw-r--r--   0        0        0     4024 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/README.md
--rw-r--r--   0        0        0      978 2023-04-17 12:07:06.989999 tradernet_sdk-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1305 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/PublicApiClient.py
--rw-r--r--   0        0        0      583 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/__init__.py
--rw-r--r--   0        0        0    32929 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/client.py
--rw-r--r--   0        0        0    11656 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/core.py
--rw-r--r--   0        0        0     2231 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/netutils.py
--rw-r--r--   0        0        0     7877 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/string_utils.py
--rw-r--r--   0        0        0        0 2023-04-17 12:12:02.327268 tradernet_sdk-0.3.4/tradernet/symbols/__init__.py
--rw-r--r--   0        0        0     6329 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/base_market_symbol.py
--rw-r--r--   0        0        0     4151 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/base_option_symbol.py
--rw-r--r--   0        0        0     2836 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/das_option.py
--rw-r--r--   0        0        0      290 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/option_properties.py
--rw-r--r--   0        0        0     2132 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/tradernet_option.py
--rw-r--r--   0        0        0     2336 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/tradernet_symbol.py
--rw-r--r--   0        0        0     3052 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/tradernet_wsapi.py
--rw-r--r--   0        0        0     6996 2023-04-14 16:56:52.678694 tradernet_sdk-0.3.4/tradernet/trading.py
--rw-r--r--   0        0        0     2858 2023-04-12 18:30:40.754961 tradernet_sdk-0.3.4/tradernet/ws_utils.py
--rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 tradernet_sdk-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/LICENSE
+-rw-r--r--   0        0        0     4024 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/README.md
+-rw-r--r--   0        0        0     1012 2023-05-15 10:59:31.178578 tradernet_sdk-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1305 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/PublicApiClient.py
+-rw-r--r--   0        0        0      583 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/__init__.py
+-rw-r--r--   0        0        0    32923 2023-05-04 19:07:13.429662 tradernet_sdk-0.3.7/tradernet/client.py
+-rw-r--r--   0        0        0      283 2023-05-04 19:07:13.429662 tradernet_sdk-0.3.7/tradernet/common/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-04 19:08:23.526279 tradernet_sdk-0.3.7/tradernet/common/file_utils.py
+-rw-r--r--   0        0        0     2238 2023-05-04 19:02:07.994968 tradernet_sdk-0.3.7/tradernet/common/netutils.py
+-rw-r--r--   0        0        0     7327 2023-05-04 19:07:13.429662 tradernet_sdk-0.3.7/tradernet/common/string_utils.py
+-rw-r--r--   0        0        0     2858 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/common/ws_utils.py
+-rw-r--r--   0        0        0    11653 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/core.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:59:04.366109 tradernet_sdk-0.3.7/tradernet/symbols/__init__.py
+-rw-r--r--   0        0        0     6329 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/symbols/base_market_symbol.py
+-rw-r--r--   0        0        0     4151 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/symbols/base_option_symbol.py
+-rw-r--r--   0        0        0     2836 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/symbols/das_option.py
+-rw-r--r--   0        0        0      290 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/symbols/option_properties.py
+-rw-r--r--   0        0        0     2132 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/symbols/tradernet_option.py
+-rw-r--r--   0        0        0     2336 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/symbols/tradernet_symbol.py
+-rw-r--r--   0        0        0     3016 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/tradernet_wsapi.py
+-rw-r--r--   0        0        0     6996 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.7/tradernet/trading.py
+-rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 tradernet_sdk-0.3.7/PKG-INFO
```

### Comparing `tradernet_sdk-0.3.4/LICENSE` & `tradernet_sdk-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/README.md` & `tradernet_sdk-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/pyproject.toml` & `tradernet_sdk-0.3.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "tradernet-sdk"
-version = "0.3.4"
+version = "0.3.7"
 description = "Public API for TraderNet"
 authors = ["Anton Kudelin <a.kudelin@freedomfinance.eu>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://tradernet.com/tradernet-api/"
+homepage = "https://dev.tradernet.ru/tradernet-api/python-sdk"
 packages = [
     {include = "tradernet"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 lxml = "^4.9.2"
 pandas = "^2.0.0"
-requests = "^2.28.2"
+requests = "^2.29.0"
 aiohttp = "^3.8.4"
 mypy-extensions = "^1.0.0"
 certifi = "^2022.12.7"
 tabulate = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.2.0"
 pylint = "^2.17.2"
 types-requests = "^2.28.11.17"
+requests = "~2.29.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 strict = true
```

### Comparing `tradernet_sdk-0.3.4/tradernet/PublicApiClient.py` & `tradernet_sdk-0.3.7/tradernet/PublicApiClient.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/tradernet/__init__.py` & `tradernet_sdk-0.3.7/tradernet/__init__.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/tradernet/client.py` & `tradernet_sdk-0.3.7/tradernet/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from io import BytesIO
 from typing import Any
 from urllib.parse import quote
 
 from lxml.html import parse
 
 from tradernet.core import TraderNetCore
-from tradernet.string_utils import extract_zip
+from tradernet.common import extract_zip
 
 
 class TraderNetAPI(TraderNetCore):
     """
     Client methods to interact TraderNet API.
     """
     def new_user(
```

### Comparing `tradernet_sdk-0.3.4/tradernet/core.py` & `tradernet_sdk-0.3.7/tradernet/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from configparser import ConfigParser
 from copy import deepcopy
 from datetime import datetime
 from json import dumps as json_dumps
 from logging import getLogger
 from typing import Any, ClassVar, Type, TypeVar
 
-from tradernet.netutils import NetUtils
+from tradernet.common import NetUtils
 
 
 Self = TypeVar('Self', bound='TraderNetCore')
 
 
 class TraderNetCore(NetUtils):
     """
@@ -40,15 +40,15 @@
     }
     CHUNK_SIZE: ClassVar[int] = 7000         # Instruments per request
 
     __slots__ = (
         'public',
         '_private',
         'login',
-        '__password',
+        '_password',
         '_session_id',
         '_session_time'
     )
 
     def __init__(
         self,
         public: str | None = None,
@@ -269,17 +269,17 @@
         elif version == 1:
             message['sig'] = self.sign(self._private)
             query = {'q': json_dumps(message)}
 
         elif version == 2:
             url = f'{self.url}/api/v2/cmd/{cmd}'
             message['apiKey'] = self.public
-            # Signing the body of the request
             message_string = self.str_from_dict(message)
 
+            # Signing the body of the request
             headers = deepcopy(self.HEADERS)
             headers['X-NtApi-Sig'] = self.sign(self._private, message_string)
             query = self.http_build_query(message).encode('utf-8')
             self.logger.debug('Message string: %s', message_string)
 
         else:
             raise ValueError('Unknown API version')
```

### Comparing `tradernet_sdk-0.3.4/tradernet/netutils.py` & `tradernet_sdk-0.3.7/tradernet/common/netutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import OrderedDict
 from logging import getLogger
 from typing import Any
 from urllib.parse import quote
 
 from requests import Response, Session as HTTPSession
 
-from tradernet.string_utils import StringUtils
+from tradernet.common.string_utils import StringUtils
 
 
 class NetUtils(StringUtils):
     __slots__ = ('session', 'timeout', 'logger')
 
     def __init__(self) -> None:
         self.session: HTTPSession | None = None
```

### Comparing `tradernet_sdk-0.3.4/tradernet/string_utils.py` & `tradernet_sdk-0.3.7/tradernet/common/string_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,20 @@
 from __future__ import annotations
 
 from collections.abc import Callable, MutableMapping
 from hmac import new as hmac_new
 from json import dumps as json_dumps
-from io import BytesIO
 from typing import Any, Union
-from zipfile import ZipFile
 
 from mypy_extensions import trait
 
 
 JSON_VALUE_TYPE = Union[str, int, float, bool, None]
 
 
-def extract_zip(content: bytes) -> dict[str, str]:
-    """
-    Extracting a zipped file into a dictionary having the structure
-    "name->content".
-    Parameters
-    ----------
-    content : bytes
-        Byte-representation of an archive.
-    Returns
-    -------
-    dict[str, str]
-        Resulting dictionary.
-    """
-    with ZipFile(BytesIO(content)) as zip_file:
-        return {
-            name: zip_file.read(name).decode() for name in zip_file.namelist()
-        }
-
-
 @trait
 class StringUtils:
     """
     A collection of methods for strings composition.
     """
     @staticmethod
     def simple_list(raw_list: list[Any]) -> str:
```

### Comparing `tradernet_sdk-0.3.4/tradernet/symbols/base_market_symbol.py` & `tradernet_sdk-0.3.7/tradernet/symbols/base_market_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/tradernet/symbols/base_option_symbol.py` & `tradernet_sdk-0.3.7/tradernet/symbols/base_option_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/tradernet/symbols/das_option.py` & `tradernet_sdk-0.3.7/tradernet/symbols/das_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/tradernet/symbols/tradernet_option.py` & `tradernet_sdk-0.3.7/tradernet/symbols/tradernet_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/tradernet/symbols/tradernet_symbol.py` & `tradernet_sdk-0.3.7/tradernet/symbols/tradernet_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/tradernet/tradernet_wsapi.py` & `tradernet_sdk-0.3.7/tradernet/tradernet_wsapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from collections.abc import AsyncIterator, Sequence
 from json import loads as json_loads
 from typing import Any
 
-from tradernet.ws_utils import WSUtils
-from tradernet.string_utils import StringUtils
+from tradernet.common import WSUtils, StringUtils
 from tradernet.core import TraderNetCore
 
 
 class TraderNetWSAPI(WSUtils, StringUtils):
     __slots__ = ('url',)
 
     def __init__(self, api: TraderNetCore) -> None:
```

### Comparing `tradernet_sdk-0.3.4/tradernet/trading.py` & `tradernet_sdk-0.3.7/tradernet/trading.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/tradernet/ws_utils.py` & `tradernet_sdk-0.3.7/tradernet/common/ws_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.4/PKG-INFO` & `tradernet_sdk-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tradernet-sdk
-Version: 0.3.4
+Version: 0.3.7
 Summary: Public API for TraderNet
-Home-page: https://tradernet.com/tradernet-api/
+Home-page: https://dev.tradernet.ru/tradernet-api/python-sdk
 License: MIT
 Author: Anton Kudelin
 Author-email: a.kudelin@freedomfinance.eu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: mypy-extensions (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # tradernet-sdk
 
 Public Python API for TraderNet
```

