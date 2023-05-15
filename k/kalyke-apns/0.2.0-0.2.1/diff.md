# Comparing `tmp/kalyke_apns-0.2.0.tar.gz` & `tmp/kalyke_apns-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalyke_apns-0.2.0.tar", max compression
+gzip compressed data, was "kalyke_apns-0.2.1.tar", max compression
```

## Comparing `kalyke_apns-0.2.0.tar` & `kalyke_apns-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/LICENSE
--rw-r--r--   0        0        0     2429 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/README.md
--rw-r--r--   0        0        0      609 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/__init__.py
--rw-r--r--   0        0        0     1334 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/clients/__init__.py
--rw-r--r--   0        0        0     2263 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/clients/apns.py
--rw-r--r--   0        0        0     1602 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/clients/voip.py
--rw-r--r--   0        0        0     5594 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/internal/__init__.py
--rw-r--r--   0        0        0     1419 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/internal/status_code.py
--rw-r--r--   0        0        0      432 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/models/__init__.py
--rw-r--r--   0        0        0     1825 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/models/apns_config.py
--rw-r--r--   0        0        0      161 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/models/apns_priority.py
--rw-r--r--   0        0        0      264 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/models/apns_push_type.py
--rw-r--r--   0        0        0      872 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/models/critical_sound.py
--rw-r--r--   0        0        0      185 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/models/interruption_level.py
--rw-r--r--   0        0        0     3247 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/models/payload.py
--rw-r--r--   0        0        0     2183 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/kalyke/models/payload_alert.py
--rw-r--r--   0        0        0     1313 2023-01-02 11:17:58.636046 kalyke_apns-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 kalyke_apns-0.2.0/setup.py
--rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 kalyke_apns-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2579 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/README.md
+-rw-r--r--   0        0        0      609 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/__init__.py
+-rw-r--r--   0        0        0     2005 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/clients/__init__.py
+-rw-r--r--   0        0        0     1481 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/clients/apns.py
+-rw-r--r--   0        0        0      845 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/clients/voip.py
+-rw-r--r--   0        0        0     5594 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/exceptions.py
+-rw-r--r--   0        0        0        0 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/internal/__init__.py
+-rw-r--r--   0        0        0     1419 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/internal/status_code.py
+-rw-r--r--   0        0        0      432 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/models/__init__.py
+-rw-r--r--   0        0        0     1825 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/models/apns_config.py
+-rw-r--r--   0        0        0      161 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/models/apns_priority.py
+-rw-r--r--   0        0        0      264 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/models/apns_push_type.py
+-rw-r--r--   0        0        0      872 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/models/critical_sound.py
+-rw-r--r--   0        0        0      185 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/models/interruption_level.py
+-rw-r--r--   0        0        0     3247 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/models/payload.py
+-rw-r--r--   0        0        0     2183 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/kalyke/models/payload_alert.py
+-rw-r--r--   0        0        0     1365 2023-01-11 13:21:06.722496 kalyke_apns-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 kalyke_apns-0.2.1/setup.py
+-rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 kalyke_apns-0.2.1/PKG-INFO
```

### Comparing `kalyke_apns-0.2.0/LICENSE` & `kalyke_apns-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kalyke_apns-0.2.0/README.md` & `kalyke_apns-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # kalyke
 
 ![Test](https://github.com/nnsnodnb/kalyke/workflows/Test/badge.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/fb85bcf746e1f4025afa/maintainability)](https://codeclimate.com/github/nnsnodnb/kalyke/maintainability)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Coverage Status](https://coveralls.io/repos/github/nnsnodnb/kalyke/badge.svg?branch=main)](https://coveralls.io/github/nnsnodnb/kalyke?branch=main)
 
 [![PyPI Package version](https://badge.fury.io/py/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![Python Supported versions](https://img.shields.io/pypi/pyversions/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![wheel](https://img.shields.io/pypi/wheel/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![format](https://img.shields.io/pypi/format/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![implementation](https://img.shields.io/pypi/implementation/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![LICENSE](https://img.shields.io/pypi/l/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
@@ -52,15 +53,15 @@
 import asyncio
 from pathlib import Path
 
 from kalyke import ApnsConfig, ApnsPushType, VoIPClient
 
 client = VoIPClient(
     use_sandbox=True,
-    auth_key_file_path=Path("/") / "path" / "to" / "YOUR_VOIP_CERTIFICATE.pem",
+    auth_key_filepath=Path("/") / "path" / "to" / "YOUR_VOIP_CERTIFICATE.pem",
 )
 
 registration_id = "a8a799ba6c21e0795b07b577b562b8537418570c0fb8f7a64dca5a86a5a3b500"
 
 payload = {"key": "value"}
 config = ApnsConfig(topic="com.example.App.voip", push_type=ApnsPushType.VOIP)
```

### Comparing `kalyke_apns-0.2.0/kalyke/__init__.py` & `kalyke_apns-0.2.1/kalyke/__init__.py`

 * *Files identical despite different names*

### Comparing `kalyke_apns-0.2.0/kalyke/clients/voip.py` & `kalyke_apns-0.2.1/kalyke/clients/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,59 @@
-from pathlib import Path
+import importlib
+import urllib.parse
 from typing import Any, Dict, Union
 
-import httpx
-from httpx import AsyncClient
+from httpx import AsyncClient, Response
 
+from ..exceptions import ApnsProviderException
 from ..internal.status_code import StatusCode
 from ..models import ApnsConfig, Payload
-from . import __Client as BaseClient
 
 
-class VoIPClient(BaseClient):
-    _auth_key_filepath: Path
-
-    def __init__(self, use_sandbox: bool, auth_key_file_path: Union[str, Path]) -> None:
-        self.use_sandbox = use_sandbox
-        if isinstance(auth_key_file_path, Path):
-            self._auth_key_filepath = auth_key_file_path
-        else:
-            self._auth_key_filepath = Path(auth_key_file_path)
+class __Client(object):
+    use_sandbox: bool
 
     async def send_message(
         self,
         device_token: str,
         payload: Union[Payload, Dict[str, Any]],
         apns_config: ApnsConfig,
     ) -> str:
         if isinstance(payload, Payload):
             data = payload.dict()
-        else:
+        elif isinstance(payload, Dict):
             data = payload
+        else:
+            raise ValueError("Type of 'payload' must be specified by Payload or Dict[str, Any].")
 
         async with self._init_client(apns_config=apns_config) as client:
             request_url = self._make_url(device_token=device_token)
             res = await self._send(client=client, url=request_url, data=data)
 
         status_code = StatusCode(res.status_code)
         if status_code.is_success:
             return res.headers["apns-id"]
 
         raise self._handle_error(error_json=res.json())
 
+    @property
+    def _base_url(self) -> str:
+        if self.use_sandbox:
+            return "https://api.sandbox.push.apple.com"
+        else:
+            return "https://api.push.apple.com"
+
     def _init_client(self, apns_config: ApnsConfig) -> AsyncClient:
-        headers = apns_config.make_headers()
-        context = httpx.create_ssl_context()
-        context.load_cert_chain(self._auth_key_filepath)
-        client = AsyncClient(headers=headers, verify=context, http2=True)
-        return client
+        raise NotImplementedError
+
+    def _make_url(self, device_token: str) -> str:
+        return f"{self._base_url}/3/device/{urllib.parse.quote(device_token)}"
+
+    async def _send(self, client: AsyncClient, url: str, data: Dict[str, Any]) -> Response:
+        return await client.post(url=url, json=data)
+
+    def _handle_error(self, error_json: Dict[str, Any]) -> ApnsProviderException:
+        reason = error_json.pop("reason")
+        exceptions_module = importlib.import_module("kalyke.exceptions")
+        exception_class = getattr(exceptions_module, reason)
+
+        return exception_class(error=error_json)
```

### Comparing `kalyke_apns-0.2.0/kalyke/exceptions.py` & `kalyke_apns-0.2.1/kalyke/exceptions.py`

 * *Files identical despite different names*

### Comparing `kalyke_apns-0.2.0/kalyke/internal/status_code.py` & `kalyke_apns-0.2.1/kalyke/internal/status_code.py`

 * *Files identical despite different names*

### Comparing `kalyke_apns-0.2.0/kalyke/models/apns_config.py` & `kalyke_apns-0.2.1/kalyke/models/apns_config.py`

 * *Files identical despite different names*

### Comparing `kalyke_apns-0.2.0/kalyke/models/critical_sound.py` & `kalyke_apns-0.2.1/kalyke/models/critical_sound.py`

 * *Files identical despite different names*

### Comparing `kalyke_apns-0.2.0/kalyke/models/payload.py` & `kalyke_apns-0.2.1/kalyke/models/payload.py`

 * *Files identical despite different names*

### Comparing `kalyke_apns-0.2.0/kalyke/models/payload_alert.py` & `kalyke_apns-0.2.1/kalyke/models/payload_alert.py`

 * *Files identical despite different names*

### Comparing `kalyke_apns-0.2.0/pyproject.toml` & `kalyke_apns-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalyke-apns"
-version = "0.2.0"
+version = "0.2.1"
 description = "A library for interacting with APNs and VoIP using HTTP/2."
 authors = ["Yuya Oka <nnsnodnb@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/nnsnodnb/kalyke"
 keywords = ["apns", "voip", "apns provider api", "apple push notifications"]
 classifiers = [
@@ -29,14 +29,16 @@
 pytest = "^7.1.1"
 black = "^22.8.0"
 isort = "^5.10.1"
 flake8 = "^5.0.4"
 mypy = "^0.971"
 pytest-cov = "^4.0.0"
 coveralls = "^3.3.1"
+pytest-httpx = "^0.21.2"
+pytest-asyncio = "^0.20.3"
 
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -51,8 +53,8 @@
     )/
 )
 '''
 
 [tool.isort]
 include_trailing_comma = true
 line_length = 120
-multi_line_output = 5
+multi_line_output = 3
```

### Comparing `kalyke_apns-0.2.0/setup.py` & `kalyke_apns-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 install_requires = \
 ['PyJWT>=2.6.0,<3.0.0',
  'cryptography>=39.0.0,<40.0.0',
  'httpx[http2]>=0.23.1,<0.24.0']
 
 setup_kwargs = {
     'name': 'kalyke-apns',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'A library for interacting with APNs and VoIP using HTTP/2.',
-    'long_description': '# kalyke\n\n![Test](https://github.com/nnsnodnb/kalyke/workflows/Test/badge.svg)\n[![Maintainability](https://api.codeclimate.com/v1/badges/fb85bcf746e1f4025afa/maintainability)](https://codeclimate.com/github/nnsnodnb/kalyke/maintainability)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n[![PyPI Package version](https://badge.fury.io/py/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![Python Supported versions](https://img.shields.io/pypi/pyversions/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![wheel](https://img.shields.io/pypi/wheel/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![format](https://img.shields.io/pypi/format/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![implementation](https://img.shields.io/pypi/implementation/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![LICENSE](https://img.shields.io/pypi/l/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n\nA library for interacting with APNs and VoIP using HTTP/2.\n\n## Installation\n\nkalyke requires python 3.7 or later.\n\n```bash\n$ pip install kalyke-apns\n```\n\n## Usage\n\n### APNs\n\n```python\nimport asyncio\n\nfrom kalyke import ApnsClient, ApnsConfig, Payload, PayloadAlert\n\nclient = ApnsClient(\n    use_sandbox=True,\n    team_id="YOUR_TEAM_ID",\n    auth_key_id="AUTH_KEY_ID",\n    auth_key_filepath="/path/to/AuthKey_AUTH_KEY_ID.p8",\n)\n\nregistration_id = "a8a799ba6c21e0795b07b577b562b8537418570c0fb8f7a64dca5a86a5a3b500"\n\npayload_alert = PayloadAlert(title="YOUR TITLE", body="YOUR BODY")\npayload = Payload(alert=payload_alert, badge=1, sound="default")\nconfig = ApnsConfig(topic="com.example.App")\n\nasyncio.run(client.send_message(device_token=registration_id, payload=payload, apns_config=config))\n```\n\n### VoIP\n\n```python\nimport asyncio\nfrom pathlib import Path\n\nfrom kalyke import ApnsConfig, ApnsPushType, VoIPClient\n\nclient = VoIPClient(\n    use_sandbox=True,\n    auth_key_file_path=Path("/") / "path" / "to" / "YOUR_VOIP_CERTIFICATE.pem",\n)\n\nregistration_id = "a8a799ba6c21e0795b07b577b562b8537418570c0fb8f7a64dca5a86a5a3b500"\n\npayload = {"key": "value"}\nconfig = ApnsConfig(topic="com.example.App.voip", push_type=ApnsPushType.VOIP)\n\nasyncio.run(client.send_message(device_token=registration_id, payload=payload, apns_config=config))\n```\n\n## License\n\nThis software is licensed under the MIT License (See [LICENSE](LICENSE)).\n',
+    'long_description': '# kalyke\n\n![Test](https://github.com/nnsnodnb/kalyke/workflows/Test/badge.svg)\n[![Maintainability](https://api.codeclimate.com/v1/badges/fb85bcf746e1f4025afa/maintainability)](https://codeclimate.com/github/nnsnodnb/kalyke/maintainability)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Coverage Status](https://coveralls.io/repos/github/nnsnodnb/kalyke/badge.svg?branch=main)](https://coveralls.io/github/nnsnodnb/kalyke?branch=main)\n\n[![PyPI Package version](https://badge.fury.io/py/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![Python Supported versions](https://img.shields.io/pypi/pyversions/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![wheel](https://img.shields.io/pypi/wheel/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![format](https://img.shields.io/pypi/format/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![implementation](https://img.shields.io/pypi/implementation/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n[![LICENSE](https://img.shields.io/pypi/l/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)\n\nA library for interacting with APNs and VoIP using HTTP/2.\n\n## Installation\n\nkalyke requires python 3.7 or later.\n\n```bash\n$ pip install kalyke-apns\n```\n\n## Usage\n\n### APNs\n\n```python\nimport asyncio\n\nfrom kalyke import ApnsClient, ApnsConfig, Payload, PayloadAlert\n\nclient = ApnsClient(\n    use_sandbox=True,\n    team_id="YOUR_TEAM_ID",\n    auth_key_id="AUTH_KEY_ID",\n    auth_key_filepath="/path/to/AuthKey_AUTH_KEY_ID.p8",\n)\n\nregistration_id = "a8a799ba6c21e0795b07b577b562b8537418570c0fb8f7a64dca5a86a5a3b500"\n\npayload_alert = PayloadAlert(title="YOUR TITLE", body="YOUR BODY")\npayload = Payload(alert=payload_alert, badge=1, sound="default")\nconfig = ApnsConfig(topic="com.example.App")\n\nasyncio.run(client.send_message(device_token=registration_id, payload=payload, apns_config=config))\n```\n\n### VoIP\n\n```python\nimport asyncio\nfrom pathlib import Path\n\nfrom kalyke import ApnsConfig, ApnsPushType, VoIPClient\n\nclient = VoIPClient(\n    use_sandbox=True,\n    auth_key_filepath=Path("/") / "path" / "to" / "YOUR_VOIP_CERTIFICATE.pem",\n)\n\nregistration_id = "a8a799ba6c21e0795b07b577b562b8537418570c0fb8f7a64dca5a86a5a3b500"\n\npayload = {"key": "value"}\nconfig = ApnsConfig(topic="com.example.App.voip", push_type=ApnsPushType.VOIP)\n\nasyncio.run(client.send_message(device_token=registration_id, payload=payload, apns_config=config))\n```\n\n## License\n\nThis software is licensed under the MIT License (See [LICENSE](LICENSE)).\n',
     'author': 'Yuya Oka',
     'author_email': 'nnsnodnb@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nnsnodnb/kalyke',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `kalyke_apns-0.2.0/PKG-INFO` & `kalyke_apns-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalyke-apns
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for interacting with APNs and VoIP using HTTP/2.
 Home-page: https://github.com/nnsnodnb/kalyke
 License: MIT
 Keywords: apns,voip,apns provider api,apple push notifications
 Author: Yuya Oka
 Author-email: nnsnodnb@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -28,14 +28,15 @@
 Description-Content-Type: text/markdown
 
 # kalyke
 
 ![Test](https://github.com/nnsnodnb/kalyke/workflows/Test/badge.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/fb85bcf746e1f4025afa/maintainability)](https://codeclimate.com/github/nnsnodnb/kalyke/maintainability)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Coverage Status](https://coveralls.io/repos/github/nnsnodnb/kalyke/badge.svg?branch=main)](https://coveralls.io/github/nnsnodnb/kalyke?branch=main)
 
 [![PyPI Package version](https://badge.fury.io/py/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![Python Supported versions](https://img.shields.io/pypi/pyversions/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![wheel](https://img.shields.io/pypi/wheel/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![format](https://img.shields.io/pypi/format/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![implementation](https://img.shields.io/pypi/implementation/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
 [![LICENSE](https://img.shields.io/pypi/l/kalyke-apns.svg)](https://pypi.org/project/kalyke-apns)
@@ -81,15 +82,15 @@
 import asyncio
 from pathlib import Path
 
 from kalyke import ApnsConfig, ApnsPushType, VoIPClient
 
 client = VoIPClient(
     use_sandbox=True,
-    auth_key_file_path=Path("/") / "path" / "to" / "YOUR_VOIP_CERTIFICATE.pem",
+    auth_key_filepath=Path("/") / "path" / "to" / "YOUR_VOIP_CERTIFICATE.pem",
 )
 
 registration_id = "a8a799ba6c21e0795b07b577b562b8537418570c0fb8f7a64dca5a86a5a3b500"
 
 payload = {"key": "value"}
 config = ApnsConfig(topic="com.example.App.voip", push_type=ApnsPushType.VOIP)
```

