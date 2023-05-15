# Comparing `tmp/pyapns_client3-3.0.5.tar.gz` & `tmp/pyapns_client3-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapns_client3-3.0.5.tar", last modified: Wed Jan  4 02:26:47 2023, max compression
+gzip compressed data, was "pyapns_client3-3.0.6.tar", last modified: Mon May 15 02:51:32 2023, max compression
```

## Comparing `pyapns_client3-3.0.5.tar` & `pyapns_client3-3.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 02:26:47.738897 pyapns_client3-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-01-04 02:26:47.738897 pyapns_client3-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 02:26:47.738897 pyapns_client3-3.0.5/pyapns_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/pyapns_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/pyapns_client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/pyapns_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/pyapns_client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/pyapns_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/pyapns_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/pyapns_client/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-01-04 02:26:36.000000 pyapns_client3-3.0.5/pyapns_client/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 02:26:47.738897 pyapns_client3-3.0.5/pyapns_client3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-01-04 02:26:47.000000 pyapns_client3-3.0.5/pyapns_client3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-04 02:26:47.000000 pyapns_client3-3.0.5/pyapns_client3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 02:26:47.000000 pyapns_client3-3.0.5/pyapns_client3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-04 02:26:47.000000 pyapns_client3-3.0.5/pyapns_client3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-04 02:26:47.000000 pyapns_client3-3.0.5/pyapns_client3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-04 02:26:47.738897 pyapns_client3-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-01-04 02:26:39.000000 pyapns_client3-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:51:32.784166 pyapns_client3-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-15 02:51:32.784166 pyapns_client3-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:51:32.780166 pyapns_client3-3.0.6/pyapns_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/pyapns_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/pyapns_client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/pyapns_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/pyapns_client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/pyapns_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/pyapns_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/pyapns_client/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-05-15 02:51:20.000000 pyapns_client3-3.0.6/pyapns_client/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:51:32.784166 pyapns_client3-3.0.6/pyapns_client3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-15 02:51:32.000000 pyapns_client3-3.0.6/pyapns_client3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-15 02:51:32.000000 pyapns_client3-3.0.6/pyapns_client3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 02:51:32.000000 pyapns_client3-3.0.6/pyapns_client3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 02:51:32.000000 pyapns_client3-3.0.6/pyapns_client3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 02:51:32.000000 pyapns_client3-3.0.6/pyapns_client3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 02:51:32.784166 pyapns_client3-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-15 02:51:26.000000 pyapns_client3-3.0.6/setup.py
```

### Comparing `pyapns_client3-3.0.5/LICENSE.rst` & `pyapns_client3-3.0.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyapns_client3-3.0.5/PKG-INFO` & `pyapns_client3-3.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyapns_client3
-Version: 3.0.5
+Version: 3.0.6
 Summary: Simple, flexible and fast Apple Push Notifications on iOS, OSX and Safari using the HTTP/2 Push provider API with async support.
 Home-page: https://github.com/capcom6/pyapns_client
 Author: Jakub Kleň
 Author-email: kukosk@gmail.com
 Maintainer: Aleksandr Soloshenko
 Maintainer-email: capcom2me@gmail.com
 License: MIT License
@@ -21,14 +21,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: dev
 License-File: LICENSE.rst
 
 **************
 pyapns_client3
 **************
 
 |version| |license|
@@ -151,14 +153,34 @@
 
 .. |license| image:: https://img.shields.io/pypi/l/pyapns_client3.svg?style=flat-square
     :target: https://pypi.python.org/pypi/pyapns_client3/
 
 
 3.0
 ===
+3.0.6
+-----
+Changed
+^^^^^^^
+- allow to use `str` as alert for notification payload (by @tartansandal)
+
+Added
+^^^^^
+- some tests with Python version 3.6-3.11
+- some payload serialization tests (by @tartansandal)
+- some type annotations
+- some docstrings
+
+3.0.5
+-----
+
+Fixed
+^^^^^
+- have `auth.py` use the `Dict` type hint from the typing module by @tinycogio
+
 3.0.0
 -----
 
 Refactored
 ^^^^^^^^^^
 - extract authentication classes
```

### Comparing `pyapns_client3-3.0.5/README.rst` & `pyapns_client3-3.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `pyapns_client3-3.0.5/pyapns_client/__init__.py` & `pyapns_client3-3.0.6/pyapns_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,54 @@
-from .client import (
-    APNSClient,
-)
-
-from .async_client import (
-    AsyncAPNSClient,
-)
-
+from .async_client import AsyncAPNSClient
+from .auth import CertificateBasedAuth, TokenBasedAuth
+from .client import APNSClient
 from .exceptions import (
-    APNSException,
+    APNSConnectionException,
     APNSDeviceException,
-    APNSServerException,
+    APNSException,
     APNSProgrammingException,
-    APNSConnectionException,
+    APNSServerException,
+    BadCertificateEnvironmentException,
+    BadCertificateException,
     BadCollapseIdException,
     BadDeviceTokenException,
     BadExpirationDateException,
     BadMessageIdException,
+    BadPathException,
     BadPriorityException,
     BadTopicException,
     DeviceTokenNotForTopicException,
     DuplicateHeadersException,
-    IdleTimeoutException,
-    MissingDeviceTokenException,
-    MissingTopicException,
-    PayloadEmptyException,
-    TopicDisallowedException,
-    BadCertificateException,
-    BadCertificateEnvironmentException,
     ExpiredProviderTokenException,
     ForbiddenException,
+    IdleTimeoutException,
+    InternalServerErrorException,
     InvalidProviderTokenException,
-    MissingProviderTokenException,
-    BadPathException,
     MethodNotAllowedException,
-    UnregisteredException,
+    MissingDeviceTokenException,
+    MissingProviderTokenException,
+    MissingTopicException,
+    PayloadEmptyException,
     PayloadTooLargeException,
-    TooManyProviderTokenUpdatesException,
-    TooManyRequestsException,
-    InternalServerErrorException,
     ServiceUnavailableException,
     ShutdownException,
+    TooManyProviderTokenUpdatesException,
+    TooManyRequestsException,
+    TopicDisallowedException,
+    UnregisteredException,
 )
-
-from .logging import (
-    logger,
-)
-
+from .logging import logger
 from .notification import (
     IOSNotification,
-    SafariNotification,
     IOSPayload,
-    SafariPayload,
     IOSPayloadAlert,
-    SafariPayloadAlert,
     PasskitPayload,
-)
-
-from .auth import (
-    TokenBasedAuth,
-    CertificateBasedAuth,
+    SafariNotification,
+    SafariPayload,
+    SafariPayloadAlert,
 )
 
 __all__ = [
     "APNSClient",
     "APNSConnectionException",
     "APNSDeviceException",
     "APNSException",
```

### Comparing `pyapns_client3-3.0.5/pyapns_client/async_client.py` & `pyapns_client3-3.0.6/pyapns_client/async_client.py`

 * *Files identical despite different names*

### Comparing `pyapns_client3-3.0.5/pyapns_client/auth.py` & `pyapns_client3-3.0.6/pyapns_client/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         raise NotImplementedError
 
     def __call__(self) -> Dict[str, Any]:
         raise NotImplementedError
 
 
 class TokenBasedAuth(Auth):
-
     AUTH_TOKEN_LIFETIME = 45 * 60  # seconds
     AUTH_TOKEN_ENCRYPTION = "ES256"
 
     def __init__(
         self,
         auth_key_path: str,
         auth_key_id: str,
@@ -59,15 +58,27 @@
     @property
     def _is_auth_token_expired(self):
         if self._auth_token_time is None:
             return True
         return time.time() >= self._auth_token_time + self.AUTH_TOKEN_LIFETIME
 
     @staticmethod
-    def _get_auth_key(auth_key_path):
+    def _get_auth_key(auth_key_path) -> str:
+        """
+        Returns the authentication key as a string from either a file path or a file object.
+
+        Parameters:
+            auth_key_path (str or file object): The path to the file containing the authentication key,
+                or a file object containing the authentication key.
+
+        Returns:
+            str: The authentication key as a string.
+        """
+        if hasattr(auth_key_path, "read"):
+            return auth_key_path.read()
         with open(auth_key_path) as f:
             return f.read()
 
     @property
     def _auth_token(self):
         if self._auth_token_storage is None or self._is_auth_token_expired:
             logger.debug("Creating a new authentication token.")
```

### Comparing `pyapns_client3-3.0.5/pyapns_client/base.py` & `pyapns_client3-3.0.6/pyapns_client/base.py`

 * *Files identical despite different names*

### Comparing `pyapns_client3-3.0.5/pyapns_client/client.py` & `pyapns_client3-3.0.6/pyapns_client/client.py`

 * *Files identical despite different names*

### Comparing `pyapns_client3-3.0.5/pyapns_client/exceptions.py` & `pyapns_client3-3.0.6/pyapns_client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import pytz
 from datetime import datetime
 
+import pytz
 
 # BASE
 
+
 class APNSException(Exception):
     """
     The base class for all exceptions.
     """
 
     def __init__(self, status_code, apns_id):
         super().__init__()
@@ -45,25 +46,27 @@
     """
 
     pass
 
 
 # CONNECTION
 
+
 class APNSConnectionException(APNSServerException):
     """
     Used when a connectinon to APNS servers fails.
     """
 
     def __init__(self):
         super().__init__(status_code=None, apns_id=None)
 
 
 # APNS REASONS
 
+
 class BadCollapseIdException(APNSProgrammingException):
     """
     The collapse identifier exceeds the maximum allowed size.
     """
 
     pass
```

### Comparing `pyapns_client3-3.0.5/pyapns_client3.egg-info/PKG-INFO` & `pyapns_client3-3.0.6/pyapns_client3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyapns-client3
-Version: 3.0.5
+Version: 3.0.6
 Summary: Simple, flexible and fast Apple Push Notifications on iOS, OSX and Safari using the HTTP/2 Push provider API with async support.
 Home-page: https://github.com/capcom6/pyapns_client
 Author: Jakub Kleň
 Author-email: kukosk@gmail.com
 Maintainer: Aleksandr Soloshenko
 Maintainer-email: capcom2me@gmail.com
 License: MIT License
@@ -21,14 +21,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: dev
 License-File: LICENSE.rst
 
 **************
 pyapns_client3
 **************
 
 |version| |license|
@@ -151,14 +153,34 @@
 
 .. |license| image:: https://img.shields.io/pypi/l/pyapns_client3.svg?style=flat-square
     :target: https://pypi.python.org/pypi/pyapns_client3/
 
 
 3.0
 ===
+3.0.6
+-----
+Changed
+^^^^^^^
+- allow to use `str` as alert for notification payload (by @tartansandal)
+
+Added
+^^^^^
+- some tests with Python version 3.6-3.11
+- some payload serialization tests (by @tartansandal)
+- some type annotations
+- some docstrings
+
+3.0.5
+-----
+
+Fixed
+^^^^^
+- have `auth.py` use the `Dict` type hint from the typing module by @tinycogio
+
 3.0.0
 -----
 
 Refactored
 ^^^^^^^^^^
 - extract authentication classes
```

### Comparing `pyapns_client3-3.0.5/setup.py` & `pyapns_client3-3.0.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 import os
-from setuptools import setup, Command
+from distutils.command.clean import clean as _clean
 
+from setuptools import setup
 
-class CleanCommand(Command):
-    """Custom clean command to tidy up the project root."""
 
-    user_options = []
+class CleanCommand(_clean):
+    """
+    A custom clean command to remove build artifacts.
+    """
 
-    def initialize_options(self):
-        pass
+    def run(self):
+        import os
+        import shutil
 
-    def finalize_options(self):
-        pass
+        # remove the build directory
+        build_dir = os.path.join(os.path.dirname(__file__), "build")
+        shutil.rmtree(build_dir, ignore_errors=True)
+
+        # remove any compiled Python files
+        for root, dirs, files in os.walk(os.path.dirname(__file__)):
+            for file in files:
+                if file.endswith(".pyc") or file.endswith(".pyo") or file.endswith("~"):
+                    os.remove(os.path.join(root, file))
 
-    def run(self):
-        os.system("rm -vrf ./build ./dist ./*.pyc ./*.tgz ./*.egg-info")
+        # call the base class's run method
+        _clean.run(self)
 
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 README = open(os.path.join(os.path.dirname(__file__), "README.rst")).read()
 CHANGELOG = open(os.path.join(os.path.dirname(__file__), "CHANGELOG.rst")).read()
 
 
 setup(
     name="pyapns_client3",
-    version="3.0.5",
+    version="3.0.6",
     packages=["pyapns_client"],
     include_package_data=True,
     license="MIT License",
     description="Simple, flexible and fast Apple Push Notifications on iOS, OSX and Safari using the HTTP/2 Push provider API with async support.",
     long_description="\n\n".join([README, CHANGELOG]),
     keywords="apns apple ios osx safari push notifications",
     url="https://github.com/capcom6/pyapns_client",
@@ -52,18 +62,27 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     cmdclass={
         "clean": CleanCommand,
     },
     install_requires=[
         "httpx[http2]",
         "PyJWT>=2",
-        "cryptography",
+        "cryptography>=40.0.2",
         "pytz",
     ],
+    extras_require={
+        "dev": [
+            "pytest",
+            "black",
+            "flake8",
+            "wheel",
+        ]
+    },
 )
```

