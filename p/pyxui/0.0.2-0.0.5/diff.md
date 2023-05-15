# Comparing `tmp/pyxui-0.0.2.tar.gz` & `tmp/pyxui-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxui-0.0.2.tar", last modified: Thu May  4 20:29:29 2023, max compression
+gzip compressed data, was "pyxui-0.0.5.tar", last modified: Mon May 15 17:06:23 2023, max compression
```

## Comparing `pyxui-0.0.2.tar` & `pyxui-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.298730 pyxui-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-05-03 15:10:37.000000 pyxui-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5047 2023-05-04 20:29:29.296734 pyxui-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4632 2023-05-03 15:10:37.000000 pyxui-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.277782 pyxui-0.0.2/pyxui/
--rw-rw-rw-   0        0        0       26 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.287758 pyxui-0.0.2/pyxui/config_gen/
--rw-rw-rw-   0        0        0      452 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/config_gen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.288756 pyxui-0.0.2/pyxui/errors/
--rw-rw-rw-   0        0        0      917 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.295737 pyxui-0.0.2/pyxui/methods/
--rw-rw-rw-   0        0        0      247 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/methods/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/methods/base.py
--rw-rw-rw-   0        0        0     4913 2023-05-04 08:36:49.000000 pyxui-0.0.2/pyxui/methods/clients.py
--rw-rw-rw-   0        0        0     1415 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/methods/inbounds.py
--rw-rw-rw-   0        0        0     1123 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/methods/login.py
--rw-rw-rw-   0        0        0      482 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/xui.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.286764 pyxui-0.0.2/pyxui.egg-info/
--rw-rw-rw-   0        0        0     5047 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 20:29:29.298730 pyxui-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-05-04 20:28:51.000000 pyxui-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.275118 pyxui-0.0.5/
+-rw-rw-rw-   0        0        0     1070 2023-05-15 16:46:45.000000 pyxui-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5047 2023-05-15 17:06:23.274108 pyxui-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4464 2023-05-15 16:46:45.000000 pyxui-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.249366 pyxui-0.0.5/pyxui/
+-rw-rw-rw-   0        0        0       26 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.266687 pyxui-0.0.5/pyxui/config_gen/
+-rw-rw-rw-   0        0        0      441 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/config_gen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.267688 pyxui-0.0.5/pyxui/errors/
+-rw-rw-rw-   0        0        0      884 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.273110 pyxui-0.0.5/pyxui/methods/
+-rw-rw-rw-   0        0        0      235 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/__init__.py
+-rw-rw-rw-   0        0        0     1411 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/base.py
+-rw-rw-rw-   0        0        0     4746 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/clients.py
+-rw-rw-rw-   0        0        0     1367 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/inbounds.py
+-rw-rw-rw-   0        0        0     1077 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/methods/login.py
+-rw-rw-rw-   0        0        0      464 2023-05-15 16:46:45.000000 pyxui-0.0.5/pyxui/xui.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:06:23.265372 pyxui-0.0.5/pyxui.egg-info/
+-rw-rw-rw-   0        0        0     5047 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-15 17:06:23.000000 pyxui-0.0.5/pyxui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 17:06:23.275118 pyxui-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-15 16:46:45.000000 pyxui-0.0.5/setup.py
```

### Comparing `pyxui-0.0.2/PKG-INFO` & `pyxui-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxui
-Version: 0.0.2
+Version: 0.0.5
 Summary: An application with python that allows you to modify your xui panel
 Home-page: https://github.com/staliox/pyxui
 Author: Staliox
 License: MIT
 Keywords: pyxui,xui,xui python,xui panel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxui-0.0.2/README.md` & `pyxui-0.0.5/pyxui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pyxui
+Version: 0.0.5
+Summary: An application with python that allows you to modify your xui panel
+Home-page: https://github.com/staliox/pyxui
+Author: Staliox
+License: MIT
+Keywords: pyxui,xui,xui python,xui panel
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyXUI 
 An application with python that allows you to modify your xui panel ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) ([alireza0 x-ui](https://github.com/alireza0/x-ui))
 
 ## How To Install
 ```
 pip install pyxui
 ```
```

### Comparing `pyxui-0.0.2/pyxui/methods/base.py` & `pyxui-0.0.5/pyxui/methods/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import requests
-
-import pyxui
-
-class Base:
-    @property
-    def _panel_address(self: "pyxui.XUI") -> str:
-        return f"{self.https}://{self.address}:{self.port}{self.path}/"
-
-    def request(
-        self: "pyxui.XUI",
-        path: str,
-        method: str,
-        params: dict = None
-    ) -> requests.Response:
-        """Request to xui panel.
-
-        Parameters:
-            path (``str``):
-                Your request path, you can see all of them in https://github.com/alireza0/x-ui#api-routes
-                
-            method (``str``):
-                Your request method, GET or POST
-                
-            params (``dict``, optional):
-                Your request parameters, None is set for default but it's necessary for some POST methods
-
-        Returns:
-            `~requests.Response`: On success, the response is returned.
-        """
-        
-        if path == "login":
-            url = self._panel_address + path
-        else:
-            url = self._panel_address + "xui/API/inbounds/" + path
-
-        if self.session_string:
-            cookie = {'session': self.session_string}
-        else:
-            cookie = None
-
-        if method == "GET":
-            response = requests.get(url, cookies=cookie, verify=False)
-        elif method == "POST":
-            response = requests.post(url, cookies=cookie, data=params, verify=False)
-
-        return response
+import requests
+
+import pyxui
+
+class Base:
+    @property
+    def _panel_address(self: "pyxui.XUI") -> str:
+        return f"{self.https}://{self.address}:{self.port}{self.path}/"
+
+    def request(
+        self: "pyxui.XUI",
+        path: str,
+        method: str,
+        params: dict = None
+    ) -> requests.Response:
+        """Request to xui panel.
+
+        Parameters:
+            path (``str``):
+                Your request path, you can see all of them in https://github.com/alireza0/x-ui#api-routes
+                
+            method (``str``):
+                Your request method, GET or POST
+                
+            params (``dict``, optional):
+                Your request parameters, None is set for default but it's necessary for some POST methods
+
+        Returns:
+            `~requests.Response`: On success, the response is returned.
+        """
+        
+        if path == "login":
+            url = self._panel_address + path
+        else:
+            url = self._panel_address + "xui/API/inbounds/" + path
+
+        if self.session_string:
+            cookie = {'session': self.session_string}
+        else:
+            cookie = None
+
+        if method == "GET":
+            response = requests.get(url, cookies=cookie, verify=self.https)
+        elif method == "POST":
+            response = requests.post(url, cookies=cookie, data=params, verify=self.https)
+
+        return response
```

### Comparing `pyxui-0.0.2/pyxui/methods/clients.py` & `pyxui-0.0.5/pyxui/methods/clients.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-import json
-from typing import Union
-
-import pyxui
-from pyxui import errors
-
-class Clients:
-    def get_client(
-        self: "pyxui.XUI",
-        inbound_id: int,
-        email: str = False,
-        uuid: str = False
-    ) -> Union[dict, errors.NotFound]:
-        """Get client from exist inbound.
-
-        Parameters:
-            inbound_id (``int``):
-                Inbound id
-                
-            email (``str``, optional):
-               Email of client
-                
-            uuid (``str``, optional):
-               UUID of client
-            
-        Returns:
-            `~Dict`: On success, a dict is returned else 404 error will be raised
-        """
-        
-        get_inbounds = self.get_inbounds()
-        
-        if not email and not uuid:
-            raise ValueError()
-        
-        for inbound in get_inbounds['obj']:
-            if inbound['id'] != inbound_id:
-                continue
-            
-            settings = json.loads(inbound['settings'])
-            
-            for client in settings['clients']:
-                if client['email'] != email and client['id'] != uuid:
-                    continue
-                
-                return client
-
-        raise errors.NotFound()
-
-    def add_client(
-        self: "pyxui.XUI",
-        inbound_id: int,
-        email: str,
-        uuid: str,
-        enable: bool = True,
-        flow: str = "",
-        limit_ip: int = 0,
-        total_gb: int = 0,
-        expire_time: int = 0,
-        telegram_id: str = "",
-        subscription_id: str = "",
-    ) -> Union[dict, errors.NotFound]:
-        """Add client to exist inbound.
-
-        Parameters:
-            inbound_id (``int``):
-                Inbound id
-                
-            email (``str``):
-               Email of client
-                
-            enable (``bool``, optional):
-               Status of client
-                
-            flow (``str``, optional):
-               Flow of client
-                
-            uuid (``str``, optional):
-               UUID of client
-                
-            limit_ip (``str``, optional):
-               IP Limit of client
-                
-            total_gb (``str``, optional):
-                Download and uploader limition of client and it's in bytes
-                
-            expire_time (``str``, optional):
-                Client expiration date and it's in timestamp (epoch)
-                
-            telegram_id (``str``, optional):
-               Telegram id of client
-                
-            subscription_id (``str``, optional):
-               Subscription id of client
-            
-        Returns:
-            `~Dict`: On success, a dict is returned else 404 error will be raised
-        """
-        
-        settings = {
-            "clients": [
-                {
-                    "id": uuid,
-                    "email": email,
-                    "enable": enable,
-                    "flow": flow,
-                    "limitIp": limit_ip,
-                    "totalGB": total_gb,
-                    "expiryTime": expire_time,
-                    "tgId": telegram_id,
-                    "subId": subscription_id
-                }
-            ]
-        }
-        
-        params = {
-            "id": inbound_id,
-            "settings": json.dumps(settings)
-        }
-
-        send_request = self.request(
-            path="addClient",
-            method="POST",
-            params=params
-        )
-
-        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
-            return send_request.json()
-        else:
-            raise errors.NotFound()
-
-    def delete_client(
-        self: "pyxui.XUI",
-        inbound_id: int,
-        email: str = False,
-        uuid: str = False
-    ) -> Union[dict, errors.NotFound]:
-        """Delete client from exist inbound.
-
-        Parameters:
-            inbound_id (``int``):
-                Inbound id
-                
-            email (``str``, optional):
-               Email of client
-                
-            uuid (``str``, optional):
-               UUID of client
-            
-        Returns:
-            `~Dict`: On success, a dict is returned else 404 error will be raised
-        """
-        
-        find_client = self.get_client(
-            inbound_id=inbound_id,
-            email=email,
-            uuid=uuid
-        )
-        
-        send_request = self.request(
-            path=f"{inbound_id}/delClient/{find_client['id']}",
-            method="POST"
-        )
-
-        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
-            return send_request.json()
-        else:
-            raise errors.NotFound()
+import json
+from typing import Union
+
+import pyxui
+from pyxui import errors
+
+class Clients:
+    def get_client(
+        self: "pyxui.XUI",
+        inbound_id: int,
+        email: str = False,
+        uuid: str = False
+    ) -> Union[dict, errors.NotFound]:
+        """Get client from exist inbound.
+
+        Parameters:
+            inbound_id (``int``):
+                Inbound id
+                
+            email (``str``, optional):
+               Email of client
+                
+            uuid (``str``, optional):
+               UUID of client
+            
+        Returns:
+            `~Dict`: On success, a dict is returned else 404 error will be raised
+        """
+        
+        get_inbounds = self.get_inbounds()
+        
+        if not email and not uuid:
+            raise ValueError()
+        
+        for inbound in get_inbounds['obj']:
+            if inbound['id'] != inbound_id:
+                continue
+            
+            settings = json.loads(inbound['settings'])
+            
+            for client in settings['clients']:
+                if client['email'] != email and client['id'] != uuid:
+                    continue
+                
+                return client
+
+        raise errors.NotFound()
+
+    def add_client(
+        self: "pyxui.XUI",
+        inbound_id: int,
+        email: str,
+        uuid: str,
+        enable: bool = True,
+        flow: str = "",
+        limit_ip: int = 0,
+        total_gb: int = 0,
+        expire_time: int = 0,
+        telegram_id: str = "",
+        subscription_id: str = "",
+    ) -> Union[dict, errors.NotFound]:
+        """Add client to exist inbound.
+
+        Parameters:
+            inbound_id (``int``):
+                Inbound id
+                
+            email (``str``):
+               Email of client
+                
+            enable (``bool``, optional):
+               Status of client
+                
+            flow (``str``, optional):
+               Flow of client
+                
+            uuid (``str``, optional):
+               UUID of client
+                
+            limit_ip (``str``, optional):
+               IP Limit of client
+                
+            total_gb (``str``, optional):
+                Download and uploader limition of client and it's in bytes
+                
+            expire_time (``str``, optional):
+                Client expiration date and it's in timestamp (epoch)
+                
+            telegram_id (``str``, optional):
+               Telegram id of client
+                
+            subscription_id (``str``, optional):
+               Subscription id of client
+            
+        Returns:
+            `~Dict`: On success, a dict is returned else 404 error will be raised
+        """
+        
+        settings = {
+            "clients": [
+                {
+                    "id": uuid,
+                    "email": email,
+                    "enable": enable,
+                    "flow": flow,
+                    "limitIp": limit_ip,
+                    "totalGB": total_gb,
+                    "expiryTime": expire_time,
+                    "tgId": telegram_id,
+                    "subId": subscription_id
+                }
+            ]
+        }
+        
+        params = {
+            "id": inbound_id,
+            "settings": json.dumps(settings)
+        }
+
+        send_request = self.request(
+            path="addClient",
+            method="POST",
+            params=params
+        )
+
+        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
+            return send_request.json()
+        else:
+            raise errors.NotFound()
+
+    def delete_client(
+        self: "pyxui.XUI",
+        inbound_id: int,
+        email: str = False,
+        uuid: str = False
+    ) -> Union[dict, errors.NotFound]:
+        """Delete client from exist inbound.
+
+        Parameters:
+            inbound_id (``int``):
+                Inbound id
+                
+            email (``str``, optional):
+               Email of client
+                
+            uuid (``str``, optional):
+               UUID of client
+            
+        Returns:
+            `~Dict`: On success, a dict is returned else 404 error will be raised
+        """
+        
+        find_client = self.get_client(
+            inbound_id=inbound_id,
+            email=email,
+            uuid=uuid
+        )
+        
+        send_request = self.request(
+            path=f"{inbound_id}/delClient/{find_client['id']}",
+            method="POST"
+        )
+
+        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
+            return send_request.json()
+        else:
+            raise errors.NotFound()
```

### Comparing `pyxui-0.0.2/pyxui/methods/inbounds.py` & `pyxui-0.0.5/pyxui/methods/inbounds.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Union
-
-import pyxui
-from pyxui import errors
-
-class Inbounds:
-    def get_inbounds(
-        self: "pyxui.XUI"
-    ) -> Union[dict, errors.NotFound]:
-        """Get inbounds of xui panel.
-        
-        Returns:
-            `~Dict | errors.NotFound`: On success, a dict is returned else 404 error will be raised
-        """
-        
-        send_request = self.request(
-            path="list",
-            method="GET"
-        )
-
-        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
-            return send_request.json()
-        else:
-            raise errors.NotFound()
-        
-    def get_inbound(
-        self: "pyxui.XUI",
-        inbound_id: int
-    ) -> Union[dict, errors.NotFound]:
-        """Get inbounds of xui panel.
-
-        Parameters:
-            inbound_id (``int``):
-                Inbound id
-        
-        Returns:
-            `~Dict | errors.NotFound`: On success, a dict is returned else 404 error will be raised
-        """
-        
-        send_request = self.request(
-            path=f"get/{inbound_id}",
-            method="GET"
-        )
-
-        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
-            return send_request.json()
-        else:
-            raise errors.NotFound()
+from typing import Union
+
+import pyxui
+from pyxui import errors
+
+class Inbounds:
+    def get_inbounds(
+        self: "pyxui.XUI"
+    ) -> Union[dict, errors.NotFound]:
+        """Get inbounds of xui panel.
+        
+        Returns:
+            `~Dict | errors.NotFound`: On success, a dict is returned else 404 error will be raised
+        """
+        
+        send_request = self.request(
+            path="list",
+            method="GET"
+        )
+
+        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
+            return send_request.json()
+        else:
+            raise errors.NotFound()
+        
+    def get_inbound(
+        self: "pyxui.XUI",
+        inbound_id: int
+    ) -> Union[dict, errors.NotFound]:
+        """Get inbounds of xui panel.
+
+        Parameters:
+            inbound_id (``int``):
+                Inbound id
+        
+        Returns:
+            `~Dict | errors.NotFound`: On success, a dict is returned else 404 error will be raised
+        """
+        
+        send_request = self.request(
+            path=f"get/{inbound_id}",
+            method="GET"
+        )
+
+        if send_request.status_code != 404 and send_request.headers.get('Content-Type').startswith('application/json'):
+            return send_request.json()
+        else:
+            raise errors.NotFound()
```

### Comparing `pyxui-0.0.2/setup.py` & `pyxui-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
     
-VERSION = "0.0.2"
+VERSION = "0.0.5"
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="pyxui",
     version=VERSION,
```

