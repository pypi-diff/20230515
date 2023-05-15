# Comparing `tmp/vvault-0.0.3.tar.gz` & `tmp/vvault-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvault-0.0.3.tar", max compression
+gzip compressed data, was "vvault-0.0.4.tar", max compression
```

## Comparing `vvault-0.0.3.tar` & `vvault-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2023-04-28 12:54:50.063653 vvault-0.0.3/LICENSE
--rw-r--r--   0        0        0     1996 2023-04-28 12:54:50.063653 vvault-0.0.3/README.md
--rw-r--r--   0        0        0      750 2023-04-28 12:54:50.063653 vvault-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 12:54:50.063653 vvault-0.0.3/vvault/__init__.py
--rw-r--r--   0        0        0      157 2023-04-28 12:54:50.063653 vvault-0.0.3/vvault/logger.py
--rw-r--r--   0        0        0     9517 2023-04-28 12:54:50.063653 vvault-0.0.3/vvault/vault.py
--rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 vvault-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-15 14:53:28.907299 vvault-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1996 2023-05-15 14:53:28.907299 vvault-0.0.4/README.md
+-rw-r--r--   0        0        0      750 2023-05-15 14:53:28.907299 vvault-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 14:53:28.907299 vvault-0.0.4/vvault/__init__.py
+-rw-r--r--   0        0        0      157 2023-05-15 14:53:28.907299 vvault-0.0.4/vvault/logger.py
+-rw-r--r--   0        0        0     9550 2023-05-15 14:53:28.907299 vvault-0.0.4/vvault/vault.py
+-rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 vvault-0.0.4/PKG-INFO
```

### Comparing `vvault-0.0.3/LICENSE` & `vvault-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vvault-0.0.3/README.md` & `vvault-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vvault-0.0.3/pyproject.toml` & `vvault-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vvault"
-version = "0.0.3"
+version = "0.0.4"
 readme = "README.md"
 packages = [{include = "vvault"}]
 authors = ["StepanGavrilov <gavrilovstepan78@gmail.com>"]
 description = "Python Client for vault"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `vvault-0.0.3/vvault/vault.py` & `vvault-0.0.4/vvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,14 @@
         logger.info(
             f"Client authenticated (master token): {self.client.is_authenticated()}"
         )
 
         # enable auth methods
         self.enable_auth_methods(auth_methods=self._auth_methods)
 
-        self.__init_config()
-
     def start(
         self,
         config_file: Path,
         unseal_keys: tuple[str, ...] | None = None,
         root_token=None,
         update: bool = False,
     ) -> dict:
@@ -253,17 +251,19 @@
         except InvalidSchema:
             logger.error("No connection to vault!")
             raise ConnectionError(f"No connection to vault: {self.url}")
 
         # first start
         if not self.client.seal_status.get("initialized"):
             self.__init()
+            self.__unseal()
+            self.__init_config()
 
         # if init (need root token and unsealed keys from input)
-        if self.client.seal_status.get("sealed"):
+        elif self.client.seal_status.get("sealed"):
             self.__unseal()
 
         self.client = hvac.Client(url=self.url, token=self.__root_token)
 
         if update:
             logger.info(f"Updating config: {update}")
             self.__init_config()
```

### Comparing `vvault-0.0.3/PKG-INFO` & `vvault-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: vvault
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Client for vault
 Author: StepanGavrilov
 Author-email: gavrilovstepan78@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: hvac (>=1.1.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 VVault
 ==
```

