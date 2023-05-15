# Comparing `tmp/amps-py-0.1.5.tar.gz` & `tmp/amps-py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amps-py-0.1.5.tar", last modified: Wed May  3 22:31:17 2023, max compression
+gzip compressed data, was "amps-py-0.1.6.tar", last modified: Mon May 15 08:05:49 2023, max compression
```

## Comparing `amps-py-0.1.5.tar` & `amps-py-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-03 22:31:17.643022 amps-py-0.1.5/
--rw-r--r--   0 abhayram   (501) staff       (20)     1074 2023-04-13 22:49:51.000000 amps-py-0.1.5/LICENSE
--rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-05-03 22:31:17.643118 amps-py-0.1.5/PKG-INFO
--rw-r--r--   0 abhayram   (501) staff       (20)      314 2023-04-13 22:49:51.000000 amps-py-0.1.5/README.md
--rw-r--r--   0 abhayram   (501) staff       (20)       84 2023-04-13 22:49:51.000000 amps-py-0.1.5/pyproject.toml
--rw-r--r--   0 abhayram   (501) staff       (20)      638 2023-05-03 22:31:17.644017 amps-py-0.1.5/setup.cfg
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-03 22:31:17.640282 amps-py-0.1.5/src/
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-03 22:31:17.641381 amps-py-0.1.5/src/amps/
--rw-r--r--   0 abhayram   (501) staff       (20)    35519 2023-05-03 22:23:35.000000 amps-py-0.1.5/src/amps/__init__.py
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-03 22:31:17.642889 amps-py-0.1.5/src/amps_py.egg-info/
--rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-05-03 22:31:17.000000 amps-py-0.1.5/src/amps_py.egg-info/PKG-INFO
--rw-r--r--   0 abhayram   (501) staff       (20)      203 2023-05-03 22:31:17.000000 amps-py-0.1.5/src/amps_py.egg-info/SOURCES.txt
--rw-r--r--   0 abhayram   (501) staff       (20)        1 2023-05-03 22:31:17.000000 amps-py-0.1.5/src/amps_py.egg-info/dependency_links.txt
--rw-r--r--   0 abhayram   (501) staff       (20)        5 2023-05-03 22:31:17.000000 amps-py-0.1.5/src/amps_py.egg-info/top_level.txt
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-15 08:05:49.894472 amps-py-0.1.6/
+-rw-r--r--   0 abhayram   (501) staff       (20)     1074 2023-04-13 22:49:51.000000 amps-py-0.1.6/LICENSE
+-rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-05-15 08:05:49.894609 amps-py-0.1.6/PKG-INFO
+-rw-r--r--   0 abhayram   (501) staff       (20)      314 2023-04-13 22:49:51.000000 amps-py-0.1.6/README.md
+-rw-r--r--   0 abhayram   (501) staff       (20)       84 2023-04-13 22:49:51.000000 amps-py-0.1.6/pyproject.toml
+-rw-r--r--   0 abhayram   (501) staff       (20)      638 2023-05-15 08:05:49.895391 amps-py-0.1.6/setup.cfg
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-15 08:05:49.892028 amps-py-0.1.6/src/
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-15 08:05:49.893113 amps-py-0.1.6/src/amps/
+-rw-r--r--   0 abhayram   (501) staff       (20)    38060 2023-05-15 07:28:29.000000 amps-py-0.1.6/src/amps/__init__.py
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-15 08:05:49.894330 amps-py-0.1.6/src/amps_py.egg-info/
+-rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-05-15 08:05:49.000000 amps-py-0.1.6/src/amps_py.egg-info/PKG-INFO
+-rw-r--r--   0 abhayram   (501) staff       (20)      203 2023-05-15 08:05:49.000000 amps-py-0.1.6/src/amps_py.egg-info/SOURCES.txt
+-rw-r--r--   0 abhayram   (501) staff       (20)        1 2023-05-15 08:05:49.000000 amps-py-0.1.6/src/amps_py.egg-info/dependency_links.txt
+-rw-r--r--   0 abhayram   (501) staff       (20)        5 2023-05-15 08:05:49.000000 amps-py-0.1.6/src/amps_py.egg-info/top_level.txt
```

### Comparing `amps-py-0.1.5/LICENSE` & `amps-py-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `amps-py-0.1.5/PKG-INFO` & `amps-py-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amps-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package for Interfacing with AMPS from Agile Data Inc.
 Home-page: https://mftlabs.github.io/amps-py
 Author: Abhay Ram
 Author-email: abhayram@hub4edi.com
 Project-URL: Bug Tracker, https://github.com/mftlabs/amps-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `amps-py-0.1.5/setup.cfg` & `amps-py-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amps-py
-version = 0.1.5
+version = 0.1.6
 author = Abhay Ram
 author_email = abhayram@hub4edi.com
 description = Package for Interfacing with AMPS from Agile Data Inc.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mftlabs.github.io/amps-py
 project_urls =
```

### Comparing `amps-py-0.1.5/src/amps/__init__.py` & `amps-py-0.1.6/src/amps/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,14 +188,77 @@
         collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
             b'index'), [bytes(self.env, "utf-8"), coll])
         result = call(Atom(b'Elixir.Amps.PyService'),
                       Atom(b'delete'), [collection, id])
         return Util.unravel_erlport_object(result)
 
 
+class Users:
+    def __init__(self, env):
+        self.env = env
+
+    def find(self, env, clauses={}, opts={}):
+        coll = bytes(collection, "utf-8")
+        collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
+            b'index'), [bytes(self.env, "utf-8"), coll])
+        clauses = Map(clauses)
+        opts = Map(opts)
+        result = call(Atom(b'Elixir.Amps.PyService'),
+                      Atom(b'find'), [collection, clauses, opts])
+        return Util.unravel_erlport_object(result)
+
+    def find_one(self, env, clauses={}, opts={}):
+        coll = bytes(collection, "utf-8")
+        collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
+            b'index'), [bytes(self.env, "utf-8"), coll])
+        clauses = Map(clauses)
+        opts = Map(opts)
+        result = call(Atom(b'Elixir.Amps.PyService'),
+                      Atom(b'find_one'), [collection, clauses, opts])
+        return Util.unravel_erlport_object(result)
+
+    def create(self, user):
+        user = Map(user)
+        result = call(Atom(b'Elixir.Amps.PyService.Users'),
+                      Atom(b'create'), [user, self.env])
+        return Util.unravel_erlport_object(result)
+
+    def update(self, id, body):
+        user = Map(body)
+        result = call(Atom(b'Elixir.Amps.PyService.Users'),
+                      Atom(b'update'), [id, user, self.env])
+        return Util.unravel_erlport_object(result)
+
+    def delete(self, id):
+        result = call(Atom(b'Elixir.Amps.PyService.Users'),
+                      Atom(b'delete'), [id, self.env])
+        return Util.unravel_erlport_object(result)
+
+    def create_session(self, user):
+        user = Map(user)
+        result = call(Atom(b'Elixir.Amps.PyService.Users'),
+                      Atom(b'create_session'), [user, self.env])
+        return Util.unravel_erlport_object(result)
+
+    def authenticate(self, access_token):
+        result = call(Atom(b'Elixir.Amps.PyService.Users'),
+                      Atom(b'authenticate'), [access_token, self.env])
+        return Util.unravel_erlport_object(result)
+
+    def renew_session(self, renewal_token):
+        result = call(Atom(b'Elixir.Amps.PyService.Users'),
+                      Atom(b'renew_session'), [renewal_token, self.env])
+        return Util.unravel_erlport_object(result)
+
+    def delete_session(self, access_token):
+        result = call(Atom(b'Elixir.Amps.PyService.Users'),
+                      Atom(b'delete_session'), [access_token, self.env])
+        return Util.unravel_erlport_object(result)
+
+
 class Action:
     """The `Action` class from AMPS provides a base class for actions that must be extended in a custom action. Actions can be performed by overriding the `Action.action` callback exposed by the class.
 
     Attributes:
         msg (dict): The msg attribute contains a python of the dictionary and the message with all of its metadata. Message data can be accessed from the msg attribute, either using the "data" key for inline data, or the "fpath" key for a path to the file containing the data.
         parms (dict): The parms attribute contains all the parameters of the configured action including any extra parameters you may have specified under the "parms" key.
         sysparms (dict): The sysparms attribute contains all useful system configuration parameters for use in actions. Currently, sysparms only contains the AMPS temporary directory under the "tempdir" key.
@@ -224,14 +287,16 @@
         msgdata = json.loads(msgdata)
         self.msg = msgdata["msg"]
         self.parms = msgdata["parms"]
         self.sysparms = msgdata["sysparms"]
         self.extra = self.parms["parms"]
         self.env = self.parms["env"]
         self.db = DB(self.env)
+        self.users = Users(self.env)
+
         if self.parms["use_provider"]:
             self.provider = self.parms["provider"]
         if self.msg.get("sid"):
             self.logger = Logger(sid=self.msg["sid"])
         else:
             self.logger = Logger()
```

### Comparing `amps-py-0.1.5/src/amps_py.egg-info/PKG-INFO` & `amps-py-0.1.6/src/amps_py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amps-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package for Interfacing with AMPS from Agile Data Inc.
 Home-page: https://mftlabs.github.io/amps-py
 Author: Abhay Ram
 Author-email: abhayram@hub4edi.com
 Project-URL: Bug Tracker, https://github.com/mftlabs/amps-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

