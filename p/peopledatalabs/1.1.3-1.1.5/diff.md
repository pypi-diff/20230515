# Comparing `tmp/peopledatalabs-1.1.3.tar.gz` & `tmp/peopledatalabs-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peopledatalabs-1.1.3.tar", max compression
+gzip compressed data, was "peopledatalabs-1.1.5.tar", max compression
```

## Comparing `peopledatalabs-1.1.3.tar` & `peopledatalabs-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-05-01 23:34:09.985973 peopledatalabs-1.1.3/LICENSE
--rw-r--r--   0        0        0    12222 2023-05-01 23:34:09.985973 peopledatalabs-1.1.3/README.md
--rw-r--r--   0        0        0     1639 2023-05-01 23:34:09.985973 peopledatalabs-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/__init__.py
--rw-r--r--   0        0        0     5612 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/__init__.py
--rw-r--r--   0        0        0     1635 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/company.py
--rw-r--r--   0        0        0      762 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/location.py
--rw-r--r--   0        0        0     2812 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/person.py
--rw-r--r--   0        0        0      744 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/school.py
--rw-r--r--   0        0        0      314 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/errors.py
--rw-r--r--   0        0        0      984 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/logger.py
--rw-r--r--   0        0        0     5069 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/main.py
--rw-r--r--   0        0        0     2445 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/__init__.py
--rw-r--r--   0        0        0     2198 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/company.py
--rw-r--r--   0        0        0      215 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/location.py
--rw-r--r--   0        0        0     4188 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/person.py
--rw-r--r--   0        0        0      783 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/school.py
--rw-r--r--   0        0        0     2434 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/requests.py
--rw-r--r--   0        0        0     1156 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/settings.py
--rw-r--r--   0        0        0      670 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/utils.py
--rw-r--r--   0        0        0    13629 1970-01-01 00:00:00.000000 peopledatalabs-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-15 14:09:06.649279 peopledatalabs-1.1.5/LICENSE
+-rw-r--r--   0        0        0    12222 2023-05-15 14:09:06.649279 peopledatalabs-1.1.5/README.md
+-rw-r--r--   0        0        0     1639 2023-05-15 14:09:06.649279 peopledatalabs-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/__init__.py
+-rw-r--r--   0        0        0     5591 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/endpoints/__init__.py
+-rw-r--r--   0        0        0     1635 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/endpoints/company.py
+-rw-r--r--   0        0        0      762 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/endpoints/location.py
+-rw-r--r--   0        0        0     2812 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/endpoints/person.py
+-rw-r--r--   0        0        0      744 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/endpoints/school.py
+-rw-r--r--   0        0        0      314 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/errors.py
+-rw-r--r--   0        0        0      984 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/logger.py
+-rw-r--r--   0        0        0     5048 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/main.py
+-rw-r--r--   0        0        0     2445 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/models/__init__.py
+-rw-r--r--   0        0        0     2198 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/models/company.py
+-rw-r--r--   0        0        0      215 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/models/location.py
+-rw-r--r--   0        0        0     4349 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/models/person.py
+-rw-r--r--   0        0        0      783 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/models/school.py
+-rw-r--r--   0        0        0     2241 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/requests.py
+-rw-r--r--   0        0        0     1139 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/settings.py
+-rw-r--r--   0        0        0      460 2023-05-15 14:09:06.653279 peopledatalabs-1.1.5/src/peopledatalabs/utils.py
+-rw-r--r--   0        0        0    13629 1970-01-01 00:00:00.000000 peopledatalabs-1.1.5/PKG-INFO
```

### Comparing `peopledatalabs-1.1.3/LICENSE` & `peopledatalabs-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/README.md` & `peopledatalabs-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/pyproject.toml` & `peopledatalabs-1.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peopledatalabs"
-version = "1.1.3"
+version = "1.1.5"
 description = "Official Python client for the People Data Labs API"
 homepage = "https://www.peopledatalabs.com"
 repository = "https://github.com/peopledatalabs/peopledatalabs-python"
 documentation = "https://docs.peopledatalabs.com"
 keywords = [
   "data enrichment",
   "people data labs",
@@ -34,17 +34,17 @@
 python-dotenv = "^0"
 requests = "^2"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^1.4"
 black = "^22.3.0"
 coverage = "^6.3.2"
-docformatter = "^1.4"
+docformatter = "^1.7"
 flake8 = "^4.0.1"
-pylint = "^2.13.5"
+pylint = "^2.17.4"
 pytest = "^7.1.1"
 pyupgrade = "^2.32.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/__init__.py` & `peopledatalabs-1.1.5/src/peopledatalabs/endpoints/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 from typing import Type
 
 from pydantic import (
     BaseModel,
     HttpUrl,
-    SecretStr,
     StrictStr,
 )
 from pydantic.dataclasses import dataclass
 
 from ..errors import InvalidEndpointError
 from ..requests import Request
 from ..utils import check_empty_parameters
@@ -32,15 +31,15 @@
     Args:
         api_key (str): The authentication API key for API calls.
         base_path (str): PeopleDataLabs' API base URL.
         section: (:obj:`str`, optional): The section to prepend to the
             API endpoint.
     """
 
-    api_key: SecretStr
+    api_key: str
     base_path: HttpUrl
     section: str = None
 
     def get_url(self, endpoint: str):
         """
         Forms the URL for the API call.
```

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/company.py` & `peopledatalabs-1.1.5/src/peopledatalabs/endpoints/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/location.py` & `peopledatalabs-1.1.5/src/peopledatalabs/endpoints/location.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/person.py` & `peopledatalabs-1.1.5/src/peopledatalabs/endpoints/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/school.py` & `peopledatalabs-1.1.5/src/peopledatalabs/endpoints/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/logger.py` & `peopledatalabs-1.1.5/src/peopledatalabs/logger.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/main.py` & `peopledatalabs-1.1.5/src/peopledatalabs/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Client's main module.
 """
 
 
 from pydantic import (
     HttpUrl,
-    SecretStr,
     constr,
     validator,
 )
 from pydantic.dataclasses import dataclass
 
 
 from .endpoints import Endpoint
@@ -38,15 +37,15 @@
             API key for API calls.
         base_path (:obj:`str`, optional): PeopleDataLabs' API base URL.
         version (:obj:`str`, optional): PeopleDataLabs' API version.
             Will be used only if base_path has no value.
         log_level (:obj:`str`, optional): The logger level.
     """
 
-    api_key: SecretStr = settings.api_key
+    api_key: str = settings.api_key
     base_path: HttpUrl = None
     version: constr(regex=settings.version_re) = settings.version
     log_level: str = None
     sandbox: bool = False
 
     @validator("api_key", pre=True, always=True)
     def api_key_not_none(cls, v):
```

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/models/__init__.py` & `peopledatalabs-1.1.5/src/peopledatalabs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/models/company.py` & `peopledatalabs-1.1.5/src/peopledatalabs/models/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/models/person.py` & `peopledatalabs-1.1.5/src/peopledatalabs/models/person.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from enum import Enum
 from typing import List, Optional, Union
 
 from pydantic import (
     BaseModel,
     EmailStr,
     root_validator,
+    conint,
     validator,
 )
 
 from . import (
     AdditionalParametersModel,
     BaseRequestModel,
     BaseSearchModel,
@@ -40,14 +41,18 @@
     phone: Optional[Union[List[str], str]]
     postal_code: Optional[Union[List[str], str]]
     profile: Optional[Union[List[str], str]]
     region: Optional[str]
     school: Optional[Union[List[str], str]]
     street_address: Optional[str]
     pdl_id: Optional[str]
+    min_likelihood: Optional[conint(ge=1, le=10)]
+    required: Optional[str]
+    data_include: Optional[str]
+    include_if_matched: Optional[bool]
 
     @root_validator(pre=True)
     def at_least_one(cls, value):
         """
         Checks that at least one parameter is valued.
         """
         if not any(value.values()):
```

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/models/school.py` & `peopledatalabs-1.1.5/src/peopledatalabs/models/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/requests.py` & `peopledatalabs-1.1.5/src/peopledatalabs/requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,18 @@
 
 import json
 from typing import Dict, Type
 
 from pydantic import (
     BaseModel,
     HttpUrl,
-    SecretStr,
 )
 from pydantic.dataclasses import dataclass
 import requests
 
-from . import utils
 from .logger import get_logger
 
 
 logger = get_logger("requests")
 
 
 @dataclass
@@ -32,15 +30,15 @@
         api_key (str): The authentication API key for API calls.
         url (str): URL of the API to call.
         headers (dict of str: str): The request headers.
         params (dict): The parameters to use in the API call.
         validator: The validator to use to validate params.
     """
 
-    api_key: SecretStr
+    api_key: str
     url: HttpUrl
     headers: Dict[str, str]
     params: dict
     validator: Type[BaseModel]
 
     def __post_init__(self):
         """
@@ -59,32 +57,31 @@
         Returns:
             A requests.Response object with the result of the HTTP call.
         """
         self.params["api_key"] = self.api_key
         logger.info(
             "Calling %s with params: %s",
             self.url,
-            json.dumps(self.params, indent=2, default=utils.json_defaults),
+            json.dumps(self.params, indent=2),
         )
-        self.params["api_key"] = self.params["api_key"].get_secret_value()
         return requests.get(
             self.url, params=self.params, headers=self.headers, timeout=None
         )
 
     def post(self):
         """
         Executes a POST request to the specified API.
 
         User's PDL_API_KEY is sent as a 'X-api-key' header.
 
         Returns:
             A requests.Response object with the result of the HTTP call.
         """
-        self.headers["X-api-key"] = self.api_key.get_secret_value()
+        self.headers["X-api-key"] = self.api_key
         logger.info(
             "Calling %s with params: %s",
             self.url,
-            json.dumps(self.params, indent=2, default=utils.json_defaults),
+            json.dumps(self.params, indent=2),
         )
         return requests.post(
             self.url, json=self.params, headers=self.headers, timeout=None
         )
```

### Comparing `peopledatalabs-1.1.3/src/peopledatalabs/settings.py` & `peopledatalabs-1.1.5/src/peopledatalabs/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 Settings also loads environment variables eventually declared in an .env
 file.
 """
 
 import os
 
 from dotenv import find_dotenv, load_dotenv
-from pydantic import HttpUrl, SecretStr
+from pydantic import HttpUrl
 from pydantic.dataclasses import dataclass
 
 
 @dataclass
 class Settings:
     """
     Singleton holding app's settings.
 
     Settings are eventually overridden if a .env file is provided, or
     environment variables are defined.
 
     All env variables should be in the form of PDL_<setting name>
     """
 
-    api_key: SecretStr = None
+    api_key: str = None
     base_path: HttpUrl = "https://api.peopledatalabs.com/"
     log_level: str = None
     log_format: str = "{asctime} [{levelname}] - {name}.{funcName}: {message}"
     version: str = "v5"
     version_re: str = r"^v[0-9]$"
     sandbox_base_path: HttpUrl = "https://sandbox.api.peopledatalabs.com/"
```

### Comparing `peopledatalabs-1.1.3/PKG-INFO` & `peopledatalabs-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peopledatalabs
-Version: 1.1.3
+Version: 1.1.5
 Summary: Official Python client for the People Data Labs API
 Home-page: https://www.peopledatalabs.com
 License: MIT
 Keywords: data enrichment,people data labs,person enrichment,company enrichment,search
 Author: People Data Labs
 Author-email: hello@peopledatalabs.com
 Requires-Python: >=3.7.2,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: peopledatalabs Version: 1.1.3 Summary: Official
+Metadata-Version: 2.1 Name: peopledatalabs Version: 1.1.5 Summary: Official
 Python client for the People Data Labs API Home-page: https://
 www.peopledatalabs.com License: MIT Keywords: data enrichment,people data
 labs,person enrichment,company enrichment,search Author: People Data Labs
 Author-email: hello@peopledatalabs.com Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

