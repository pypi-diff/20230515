# Comparing `tmp/odoo_xmlrpc_wrapper-1.0.1.tar.gz` & `tmp/odoo_xmlrpc_wrapper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\cagat\OneDrive\Belgeler\kodlar\odoo_xmlrpc_wrapper\dist\.tmp-cnfld15d\odoo_xmlrpc_wrapper-1.0.1.tar", last modified: Thu Mar 23 23:22:35 2023, max compression
+gzip compressed data, was "dist\odoo_xmlrpc_wrapper-1.1.1.tar", last modified: Mon May 15 06:41:49 2023, max compression
```

## Comparing `odoo_xmlrpc_wrapper-1.0.1.tar` & `odoo_xmlrpc_wrapper-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/
--rw-rw-rw-   0        0        0     1092 2023-03-19 23:13:15.000000 odoo_xmlrpc_wrapper-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     7602 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4914 2023-03-23 23:22:28.000000 odoo_xmlrpc_wrapper-1.0.1/README.md
--rw-rw-rw-   0        0        0     1431 2023-03-23 23:16:43.000000 odoo_xmlrpc_wrapper-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1194 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-03-23 23:16:43.000000 odoo_xmlrpc_wrapper-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper/
--rw-rw-rw-   0        0        0      134 2023-03-17 11:20:36.000000 odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper/__init__.py
--rw-rw-rw-   0        0        0     8673 2023-03-23 20:08:45.000000 odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper/odoo_xmlrpc_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper.egg-info/
--rw-rw-rw-   0        0        0     7602 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-23 23:22:35.000000 odoo_xmlrpc_wrapper-1.0.1/tests/
--rw-rw-rw-   0        0        0     1543 2023-03-23 19:43:33.000000 odoo_xmlrpc_wrapper-1.0.1/tests/test_odoo_xmlrpc_wapper.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-10 10:42:01.000000 odoo_xmlrpc_wrapper-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7602 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4914 2023-05-10 10:42:01.000000 odoo_xmlrpc_wrapper-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1431 2023-05-10 10:56:42.000000 odoo_xmlrpc_wrapper-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1194 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-05-10 10:57:14.000000 odoo_xmlrpc_wrapper-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper/
+-rw-rw-rw-   0        0        0      134 2023-05-10 10:42:01.000000 odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     9226 2023-05-10 10:53:28.000000 odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper/odoo_xmlrpc_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     7602 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 06:41:49.000000 odoo_xmlrpc_wrapper-1.1.1/tests/
+-rw-rw-rw-   0        0        0     1543 2023-05-10 10:42:01.000000 odoo_xmlrpc_wrapper-1.1.1/tests/test_odoo_xmlrpc_wapper.py
```

### Comparing `odoo_xmlrpc_wrapper-1.0.1/LICENSE` & `odoo_xmlrpc_wrapper-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odoo_xmlrpc_wrapper-1.0.1/PKG-INFO` & `odoo_xmlrpc_wrapper-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_xmlrpc_wrapper
-Version: 1.0.1
+Version: 1.1.1
 Summary: A simple Python library to make CRUD process easier
 Home-page: https://github.com/cagatayuresin/odoo-xmlrpc-wrapper
 Author: Cagatay URESIN
 Author-email: Cagatay URESIN <cagatayuresin@gmail.com>
 Maintainer-email: Cagatay URESIN <cagatayuresin@gmail.com>
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: odoo_xmlrpc_wrapper Version: 1.0.1 Summary: A
+Metadata-Version: 2.1 Name: odoo_xmlrpc_wrapper Version: 1.1.1 Summary: A
 simple Python library to make CRUD process easier Home-page: https://
 github.com/cagatayuresin/odoo-xmlrpc-wrapper Author: Cagatay URESIN Author-
 email: Cagatay URESIN
 gmail.com> Maintainer-email: Cagatay URESIN
 gmail.com> License: MIT License Copyright 2023 Cagatay URESIN Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the âSoftwareâ), to deal in the
```

### Comparing `odoo_xmlrpc_wrapper-1.0.1/README.md` & `odoo_xmlrpc_wrapper-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `odoo_xmlrpc_wrapper-1.0.1/pyproject.toml` & `odoo_xmlrpc_wrapper-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "odoo_xmlrpc_wrapper"
-version = "1.0.1"
+version = "1.1.1"
 description = "A simple Python library to make CRUD process easier"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["odoo", "external", "api", "xmlrpc", "rpc", "wrapper"]
 authors = [
   {name = "Cagatay URESIN", email = "cagatayuresin@gmail.com"}
```

### Comparing `odoo_xmlrpc_wrapper-1.0.1/setup.cfg` & `odoo_xmlrpc_wrapper-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 646f 6f5f 786d 6c72 7063 5f77   = odoo_xmlrpc_w
 00000020: 7261 7070 6572 0d0a 7665 7273 696f 6e20  rapper..version 
-00000030: 3d20 312e 302e 310d 0a61 7574 686f 7220  = 1.0.1..author 
+00000030: 3d20 312e 312e 310d 0a61 7574 686f 7220  = 1.1.1..author 
 00000040: 3d20 4361 6761 7461 7920 5552 4553 494e  = Cagatay URESIN
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2063 6167 6174 6179 7572 6573 696e 4067   cagatayuresin@g
 00000070: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000080: 7074 696f 6e20 3d20 4120 7369 6d70 6c65  ption = A simple
 00000090: 2050 7974 686f 6e20 6c69 6272 6172 7920   Python library 
 000000a0: 746f 206d 616b 6520 4352 5544 2070 726f  to make CRUD pro
```

### Comparing `odoo_xmlrpc_wrapper-1.0.1/setup.py` & `odoo_xmlrpc_wrapper-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="odoo_xmlrpc_wrapper",
-    version="1.0.1",
+    version="1.1.1",
     description="A simple Python library to make CRUD process easier.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cagatayuresin/odoo-xmlrpc-wrapper",
     author="Cagatay URESIN",
     author_email="cagatayuresin@gmail.com",
     license="MIT",
```

### Comparing `odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper/odoo_xmlrpc_wrapper.py` & `odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper/odoo_xmlrpc_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,21 +50,19 @@
             raise Exception(
                 f"Wrong one ({self.HOST}, {self.DB}, {self.USERLOGIN}, PASSWORD)"
             )
         self.__orm = xmlrpc.client.ServerProxy(f"{self.URL}/object")
         self.profile = self.read("res.users", ids=self.uid, fields=["name"])[0]
         self.name = self.profile["name"]
         self.successful = True
-        print(
-            f"Successfully Logged\n"
-            f"Name: {self.name}\n"
-            f"DB: {self.DB}\n"
-            f"HOST: {self.HOST}\n"
-            f"VERSION: {self.version['server_version']}"
-        )
+        if self.successful:
+            print(self.status)
+
+    def satus(self) -> str:
+        return f"Successfully Logged\nName: {self.name}\nDB: {self.DB}\nHOST: {self.HOST}\nVERSION: {self.version['server_version']}"
 
     def search_read(
         self,
         model: str = None,
         constraints: list = None,
         fields: list = None,
         limit: int = None,
@@ -258,7 +256,25 @@
             self.uid,
             self.__PASSWORD,
             self.model,
             "fields_get",
             [],
             {"attributes": attributes} if attributes else {},
         )
+
+    def custom(self, model: str = None, command: str = None, att=[[]]):
+        """
+        Triggering a method remotely.
+
+        Args:
+            model (str): Model name.
+            command (str): Your custom command's name.
+            att (list, optional): Sends attributes your custom method.
+
+        Returns:
+            Your method's return.
+        """
+        if model:
+            self.model = model
+        return self.__orm.execute_kw(
+            self.DB, self.uid, self.__PASSWORD, self.model, command, att
+        )
```

### Comparing `odoo_xmlrpc_wrapper-1.0.1/src/odoo_xmlrpc_wrapper.egg-info/PKG-INFO` & `odoo_xmlrpc_wrapper-1.1.1/src/odoo_xmlrpc_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-xmlrpc-wrapper
-Version: 1.0.1
+Version: 1.1.1
 Summary: A simple Python library to make CRUD process easier
 Home-page: https://github.com/cagatayuresin/odoo-xmlrpc-wrapper
 Author: Cagatay URESIN
 Author-email: Cagatay URESIN <cagatayuresin@gmail.com>
 Maintainer-email: Cagatay URESIN <cagatayuresin@gmail.com>
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: odoo-xmlrpc-wrapper Version: 1.0.1 Summary: A
+Metadata-Version: 2.1 Name: odoo-xmlrpc-wrapper Version: 1.1.1 Summary: A
 simple Python library to make CRUD process easier Home-page: https://
 github.com/cagatayuresin/odoo-xmlrpc-wrapper Author: Cagatay URESIN Author-
 email: Cagatay URESIN
 gmail.com> Maintainer-email: Cagatay URESIN
 gmail.com> License: MIT License Copyright 2023 Cagatay URESIN Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the âSoftwareâ), to deal in the
```

### Comparing `odoo_xmlrpc_wrapper-1.0.1/tests/test_odoo_xmlrpc_wapper.py` & `odoo_xmlrpc_wrapper-1.1.1/tests/test_odoo_xmlrpc_wapper.py`

 * *Files identical despite different names*

