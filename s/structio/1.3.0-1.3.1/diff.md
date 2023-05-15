# Comparing `tmp/structio-1.3.0.tar.gz` & `tmp/structio-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.3.0.tar", last modified: Sat Apr 29 05:49:12 2023, max compression
+gzip compressed data, was "structio-1.3.1.tar", last modified: Mon May 15 16:12:43 2023, max compression
```

## Comparing `structio-1.3.0.tar` & `structio-1.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:49:12.972128 structio-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-04-29 05:49:12.972128 structio-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-04-29 05:48:52.000000 structio-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-29 05:48:52.000000 structio-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 05:49:12.972128 structio-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:49:12.972128 structio-1.3.0/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-04-29 05:49:12.000000 structio-1.3.0/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-29 05:49:12.000000 structio-1.3.0/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 05:49:12.000000 structio-1.3.0/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 05:49:12.000000 structio-1.3.0/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-04-29 05:48:52.000000 structio-1.3.0/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:12:43.464842 structio-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-05-15 16:12:43.464842 structio-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-05-15 16:12:26.000000 structio-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-15 16:12:26.000000 structio-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:12:43.464842 structio-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:12:43.464842 structio-1.3.1/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-05-15 16:12:43.000000 structio-1.3.1/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-15 16:12:43.000000 structio-1.3.1/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:12:43.000000 structio-1.3.1/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 16:12:43.000000 structio-1.3.1/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-05-15 16:12:26.000000 structio-1.3.1/structio.py
```

### Comparing `structio-1.3.0/PKG-INFO` & `structio-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -21,15 +21,15 @@
 Writing to a stream:
 
 ```python
 >>> from structio import StructIO
 >>> stream = StructIO()
 >>> stream.write_int(10, 2)
 2
->>> stream.write_float(3.14)
+>>> stream.write_float(3.14, 4)
 4
 >>> stream.write_cstr('Hello')
 6
 >>> stream.write_pstr('World!', 1)
 7
 >>> stream.seek(0)
 0
@@ -40,15 +40,15 @@
 Reading from the same stream:
 
 ```python
 >>> stream.seek(0)
 0
 >>> stream.read_int(2)
 10
->>> stream.read_float()
+>>> stream.read_float(4)
 3.140000104904175
 >>> stream.read_cstr()
 'Hello'
 >>> stream.read_pstr(1)
 'World!'
 ```
```

### Comparing `structio-1.3.0/README.md` & `structio-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Writing to a stream:
 
 ```python
 >>> from structio import StructIO
 >>> stream = StructIO()
 >>> stream.write_int(10, 2)
 2
->>> stream.write_float(3.14)
+>>> stream.write_float(3.14, 4)
 4
 >>> stream.write_cstr('Hello')
 6
 >>> stream.write_pstr('World!', 1)
 7
 >>> stream.seek(0)
 0
@@ -32,15 +32,15 @@
 Reading from the same stream:
 
 ```python
 >>> stream.seek(0)
 0
 >>> stream.read_int(2)
 10
->>> stream.read_float()
+>>> stream.read_float(4)
 3.140000104904175
 >>> stream.read_cstr()
 'Hello'
 >>> stream.read_pstr(1)
 'World!'
 ```
```

### Comparing `structio-1.3.0/structio.egg-info/PKG-INFO` & `structio-1.3.1/structio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -21,15 +21,15 @@
 Writing to a stream:
 
 ```python
 >>> from structio import StructIO
 >>> stream = StructIO()
 >>> stream.write_int(10, 2)
 2
->>> stream.write_float(3.14)
+>>> stream.write_float(3.14, 4)
 4
 >>> stream.write_cstr('Hello')
 6
 >>> stream.write_pstr('World!', 1)
 7
 >>> stream.seek(0)
 0
@@ -40,15 +40,15 @@
 Reading from the same stream:
 
 ```python
 >>> stream.seek(0)
 0
 >>> stream.read_int(2)
 10
->>> stream.read_float()
+>>> stream.read_float(4)
 3.140000104904175
 >>> stream.read_cstr()
 'Hello'
 >>> stream.read_pstr(1)
 'World!'
 ```
```

### Comparing `structio-1.3.0/structio.py` & `structio-1.3.1/structio.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,14 @@
         
     def unpack_float(self, b, numbytes, endian=None):
         return struct.unpack(self._get_format(numbytes, self._get_endian(endian)), b)[0]
         
     def pack_float(self, number, numbytes, endian=None):
         return struct.pack(self._get_format(numbytes, self._get_endian(endian)), number)
         
-    def _get_str_len(self, b, length, start=0):
-        return length
-        
     def unpack_str(self, b):
         return b.decode(self.encoding, errors=self.errors)
         
     def pack_str(self, string):
         return string.encode(self.encoding, errors=self.errors)
         
     def _get_cstr_len(self, b, start=0):
@@ -301,15 +298,16 @@
     def write_str(self, string):
         return self.write(self._struct.pack_str(string))
         
     def append_str(self, string):
         return self.append(self._struct.pack_str(string))
         
     def overwrite_str(self, string, length):
-        return self._overwrite(self._struct._get_str_len, (length,), self._struct.pack_str, (string,))
+        start = self.tell()
+        return self.overwrite(start, start + length, self._struct.pack_str(string))
         
     def read_cstr(self):
         return self._read(self._struct.unpack_cstr, ())
         
     def write_cstr(self, string):
         return self.write(self._struct.pack_cstr(string))
```

