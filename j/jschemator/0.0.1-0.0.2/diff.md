# Comparing `tmp/jschemator-0.0.1.tar.gz` & `tmp/jschemator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jschemator-0.0.1.tar", last modified: Thu May 11 13:28:43 2023, max compression
+gzip compressed data, was "jschemator-0.0.2.tar", last modified: Mon May 15 06:40:38 2023, max compression
```

## Comparing `jschemator-0.0.1.tar` & `jschemator-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:28:43.915880 jschemator-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 13:28:29.000000 jschemator-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-11 13:28:43.915880 jschemator-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 13:28:29.000000 jschemator-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:28:43.915880 jschemator-0.0.1/jschemator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-11 13:28:43.000000 jschemator-0.0.1/jschemator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-11 13:28:43.000000 jschemator-0.0.1/jschemator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:28:43.000000 jschemator-0.0.1/jschemator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 13:28:43.000000 jschemator-0.0.1/jschemator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:28:43.915880 jschemator-0.0.1/schemator/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-11 13:28:29.000000 jschemator-0.0.1/schemator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:28:43.915880 jschemator-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-11 13:28:29.000000 jschemator-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:40:38.612392 jschemator-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 06:40:27.000000 jschemator-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 06:40:38.612392 jschemator-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 06:40:27.000000 jschemator-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:40:38.612392 jschemator-0.0.2/jschemator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 06:40:27.000000 jschemator-0.0.2/jschemator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-15 06:40:27.000000 jschemator-0.0.2/jschemator/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:40:38.612392 jschemator-0.0.2/jschemator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 06:40:38.612392 jschemator-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-15 06:40:27.000000 jschemator-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:40:38.612392 jschemator-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 06:40:27.000000 jschemator-0.0.2/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-15 06:40:27.000000 jschemator-0.0.2/tests/test_schema.py
```

### Comparing `jschemator-0.0.1/LICENSE` & `jschemator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jschemator-0.0.1/schemator/__init__.py` & `jschemator-0.0.2/jschemator/fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,67 @@
-class ComplexType:
-    def render(self):
+class BaseField:
+    def json_schema_render(self):
         raise NotImplementedError
 
+    def __get__(self, __instance__, __owner__):
+        return self.value
+
+    def __set__(self, __instance__, value):
+        self.value = value
+
     value = None
     contribute_to_class = True
 
 
-class BooleanField(ComplexType):
-    def render(self):
+class StringField(BaseField):
+    def json_schema_render(self):
+        return {"type": "string"}
+
+    def __set__(self, __instance__, value):
+        if not isinstance(value, str):
+            raise ValueError("Value must be a string")
+        self.value = value
+
+
+class BooleanField(BaseField):
+    def json_schema_render(self):
         return {"type": "boolean"}
 
 
-class IntegerField(ComplexType):
-    def render(self):
+class IntegerField(BaseField):
+    def json_schema_render(self):
         return {"type": "integer"}
 
 
-class DateTimeField(ComplexType):
-    def render(self):
+class DateTimeField(BaseField):
+    def json_schema_render(self):
         return {
             "type": "string",
             "pattern": "^([\\+-]?\\d{4}(?!\\d{2}\\b))((-?)((0[1-9]|1[0-2])(\\3([12]\\d|0[1-9]|3[01]))?|W([0-4]\\d|5[0-2])(-?[1-7])?|(00[1-9]|0[1-9]\\d|[12]\\d{2}|3([0-5]\\d|6[1-6])))([T\\s]((([01]\\d|2[0-3])((:?)[0-5]\\d)?|24\\:?00)([\\.,]\\d+(?!:))?)?(\\17[0-5]\\d([\\.,]\\d+)?)?([zZ]|([\\+-])([01]\\d|2[0-3]):?([0-5]\\d)?)?)?)?$",
         }
 
 
-class UrlField(ComplexType):
-    def render(self):
+class UrlField(BaseField):
+    def json_schema_render(self):
         return {
             "type": "string",
             "pattern": "^([a-zA-Z0-9]+(-[a-zA-Z0-9]+)*\\.)+[a-zA-Z]{2,}",
         }
 
 
-class ArrayField(ComplexType):
-    def __init__(self, type):
+class ArrayField(BaseField):
+    def __init__(self, type: BaseField):
         self.type = type
 
-    def render(self):
-        return {"type": "array", "items": self.type.render()}
+    def json_schema_render(self):
+        return {"type": "array", "items": self.type.json_schema_render()}
 
 
-class EnumField(ComplexType):
+class EnumField(BaseField):
     def __init__(self, enum):
         self.enum = enum
 
-    def render(self):
+    def json_schema_render(self):
         return {
             "type": "string",
             "enum": [e.value for e in self.enum],
         }
-
-
-class StringField(ComplexType):
-    def render(self):
-        return {"type": "string"}
-
-    def __get__(self, __instance__, __owner__):
-        return self.value
-
-    def __set__(self, __instance__, value):
-        self.value = value
-
-
-class JsonSchema:
-    def schema(self):
-        schema_fields = []
-        for attribute_name, attribute_description in type(self).__dict__.items():
-            if (
-                not "__" in attribute_name
-                and type(attribute_description).contribute_to_class
-            ):
-                schema_fields.append(attribute_name)
-        properties = {
-            schema_field: type(self).__dict__[schema_field].render()
-            for schema_field in schema_fields
-        }
-        return {
-            "$schema": "http://json-schema.org/draft-07/schema#",
-            "type": "object",
-            "properties": properties,
-        }
```

