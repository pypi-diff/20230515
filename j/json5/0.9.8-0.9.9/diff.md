# Comparing `tmp/json5-0.9.8.tar.gz` & `tmp/json5-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json5-0.9.8.tar", last modified: Mon May  9 01:48:59 2022, max compression
+gzip compressed data, was "json5-0.9.9.tar", last modified: Mon Aug  1 22:28:38 2022, max compression
```

## Comparing `json5-0.9.8.tar` & `json5-0.9.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 dpranke    (501) staff       (20)        0 2022-05-09 01:48:59.073501 json5-0.9.8/
--rw-r--r--   0 dpranke    (501) staff       (20)    11325 2017-08-13 03:11:11.000000 json5-0.9.8/LICENSE
--rw-r--r--   0 dpranke    (501) staff       (20)       29 2020-01-30 23:15:02.000000 json5-0.9.8/MANIFEST.in
--rw-rw-r--   0 dpranke    (501) staff       (20)     8724 2022-05-09 01:48:59.073647 json5-0.9.8/PKG-INFO
--rw-rw-r--   0 dpranke    (501) staff       (20)     8009 2022-05-09 01:48:26.000000 json5-0.9.8/README.md
-drwxrwxr-x   0 dpranke    (501) staff       (20)        0 2022-05-09 01:48:59.071953 json5-0.9.8/json5/
--rw-r--r--   0 dpranke    (501) staff       (20)      821 2019-06-12 01:09:07.000000 json5-0.9.8/json5/__init__.py
--rw-r--r--   0 dpranke    (501) staff       (20)      741 2017-11-23 21:45:54.000000 json5-0.9.8/json5/__main__.py
--rw-r--r--   0 dpranke    (501) staff       (20)     2130 2019-06-12 01:09:07.000000 json5-0.9.8/json5/arg_parser.py
--rw-r--r--   0 dpranke    (501) staff       (20)     1635 2019-06-12 01:09:07.000000 json5-0.9.8/json5/host.py
--rw-rw-r--   0 dpranke    (501) staff       (20)    19248 2022-05-06 21:20:57.000000 json5-0.9.8/json5/lib.py
--rw-rw-r--   0 dpranke    (501) staff       (20)    29770 2022-05-09 01:48:26.000000 json5-0.9.8/json5/parser.py
--rw-rw-r--   0 dpranke    (501) staff       (20)     3690 2022-05-08 20:02:40.000000 json5-0.9.8/json5/tool.py
--rw-rw-r--   0 dpranke    (501) staff       (20)      614 2022-05-09 01:48:26.000000 json5-0.9.8/json5/version.py
-drwxrwxr-x   0 dpranke    (501) staff       (20)        0 2022-05-09 01:48:59.073299 json5-0.9.8/json5.egg-info/
--rw-rw-r--   0 dpranke    (501) staff       (20)     8724 2022-05-09 01:48:59.000000 json5-0.9.8/json5.egg-info/PKG-INFO
--rw-rw-r--   0 dpranke    (501) staff       (20)      354 2022-05-09 01:48:59.000000 json5-0.9.8/json5.egg-info/SOURCES.txt
--rw-rw-r--   0 dpranke    (501) staff       (20)        1 2022-05-09 01:48:59.000000 json5-0.9.8/json5.egg-info/dependency_links.txt
--rw-rw-r--   0 dpranke    (501) staff       (20)       45 2022-05-09 01:48:59.000000 json5-0.9.8/json5.egg-info/entry_points.txt
--rw-rw-r--   0 dpranke    (501) staff       (20)       18 2022-05-09 01:48:59.000000 json5-0.9.8/json5.egg-info/requires.txt
--rw-rw-r--   0 dpranke    (501) staff       (20)        6 2022-05-09 01:48:59.000000 json5-0.9.8/json5.egg-info/top_level.txt
--rw-r--r--   0 dpranke    (501) staff       (20)      107 2022-05-09 01:48:59.074172 json5-0.9.8/setup.cfg
--rw-rw-r--   0 dpranke    (501) staff       (20)     1883 2022-05-06 21:46:49.000000 json5-0.9.8/setup.py
+drwxr-xr-x   0 dpranke    (501) staff       (20)        0 2022-08-01 22:28:38.511002 json5-0.9.9/
+-rw-r--r--   0 dpranke    (501) staff       (20)    11325 2017-08-13 03:11:11.000000 json5-0.9.9/LICENSE
+-rw-r--r--   0 dpranke    (501) staff       (20)       29 2020-01-30 23:15:02.000000 json5-0.9.9/MANIFEST.in
+-rw-r--r--   0 dpranke    (501) staff       (20)     9314 2022-08-01 22:28:38.511136 json5-0.9.9/PKG-INFO
+-rw-rw-r--   0 dpranke    (501) staff       (20)     8619 2022-08-01 22:20:44.000000 json5-0.9.9/README.md
+drwxr-xr-x   0 dpranke    (501) staff       (20)        0 2022-08-01 22:28:38.509153 json5-0.9.9/json5/
+-rw-r--r--   0 dpranke    (501) staff       (20)      821 2019-06-12 01:09:07.000000 json5-0.9.9/json5/__init__.py
+-rw-r--r--   0 dpranke    (501) staff       (20)      741 2017-11-23 21:45:54.000000 json5-0.9.9/json5/__main__.py
+-rw-r--r--   0 dpranke    (501) staff       (20)     2130 2019-06-12 01:09:07.000000 json5-0.9.9/json5/arg_parser.py
+-rw-r--r--   0 dpranke    (501) staff       (20)     1635 2019-06-12 01:09:07.000000 json5-0.9.9/json5/host.py
+-rw-rw-r--   0 dpranke    (501) staff       (20)    19567 2022-08-01 22:13:09.000000 json5-0.9.9/json5/lib.py
+-rw-rw-r--   0 dpranke    (501) staff       (20)    29770 2022-07-21 03:36:57.000000 json5-0.9.9/json5/parser.py
+-rw-rw-r--   0 dpranke    (501) staff       (20)     3690 2022-05-08 20:02:40.000000 json5-0.9.9/json5/tool.py
+-rw-rw-r--   0 dpranke    (501) staff       (20)      614 2022-08-01 22:14:18.000000 json5-0.9.9/json5/version.py
+drwxr-xr-x   0 dpranke    (501) staff       (20)        0 2022-08-01 22:28:38.510784 json5-0.9.9/json5.egg-info/
+-rw-r--r--   0 dpranke    (501) staff       (20)     9314 2022-08-01 22:28:38.000000 json5-0.9.9/json5.egg-info/PKG-INFO
+-rw-r--r--   0 dpranke    (501) staff       (20)      354 2022-08-01 22:28:38.000000 json5-0.9.9/json5.egg-info/SOURCES.txt
+-rw-r--r--   0 dpranke    (501) staff       (20)        1 2022-08-01 22:28:38.000000 json5-0.9.9/json5.egg-info/dependency_links.txt
+-rw-r--r--   0 dpranke    (501) staff       (20)       44 2022-08-01 22:28:38.000000 json5-0.9.9/json5.egg-info/entry_points.txt
+-rw-r--r--   0 dpranke    (501) staff       (20)       18 2022-08-01 22:28:38.000000 json5-0.9.9/json5.egg-info/requires.txt
+-rw-r--r--   0 dpranke    (501) staff       (20)        6 2022-08-01 22:28:38.000000 json5-0.9.9/json5.egg-info/top_level.txt
+-rw-r--r--   0 dpranke    (501) staff       (20)      107 2022-08-01 22:28:38.511610 json5-0.9.9/setup.cfg
+-rw-rw-r--   0 dpranke    (501) staff       (20)     1883 2022-07-21 03:36:57.000000 json5-0.9.9/setup.py
```

### Comparing `json5-0.9.8/LICENSE` & `json5-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `json5-0.9.8/PKG-INFO` & `json5-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: json5
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Python implementation of the JSON5 data format.
 Home-page: https://github.com/dpranke/pyjson5
 Author: Dirk Pranke
 Author-email: dpranke@chromium.org
 License: Apache
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -73,14 +72,24 @@
 ## Running the tests
 To run the tests, setup a venv and install the required dependencies with
 `pip install -e '.[dev]'`, then run the tests with `python setup.py test`.
 
 
 ## Version History / Release Notes
 
+* v0.9.9 (2022-08-01)
+    * [GitHub issue #57](https://github.com/dpranke/pyjson5/issues/57)
+      Fixed serialization for objects that subclass `int` or `float`:
+      Previously we would use the objects __str__ implementation, but
+      that might result in an illegal JSON5 value if the object had
+      customized __str__ to return something illegal. Instead,
+      we follow the lead of the `JSON` module and call `int.__repr__`
+      or `float.__repr__` directly.
+    * While I was at it, I added tests for dumps(-inf) and dumps(nan)
+      when those were supposed to be disallowed by `allow_nan=False`.
 * v0.9.8 (2022-05-08)
     * [GitHub issue #47](https://github.com/dpranke/pyjson5/issues/47)
       Fixed error reporting in some cases due to how parsing was handling
       nested rules in the grammar - previously the reported location for
       the error could be far away from the point where it actually happened.
 
 * v0.9.7 (2022-05-06)
@@ -195,9 +204,7 @@
 
 * v0.6.0 (2017-11-28)
     * First implementation that attempted to implement 100% of the spec.
 
 * v0.5.0 (2017-09-04)
     * First implementation that supported the full set of kwargs that
       the `json` module supports.
-
-
```

### Comparing `json5-0.9.8/README.md` & `json5-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,24 @@
 ## Running the tests
 To run the tests, setup a venv and install the required dependencies with
 `pip install -e '.[dev]'`, then run the tests with `python setup.py test`.
 
 
 ## Version History / Release Notes
 
+* v0.9.9 (2022-08-01)
+    * [GitHub issue #57](https://github.com/dpranke/pyjson5/issues/57)
+      Fixed serialization for objects that subclass `int` or `float`:
+      Previously we would use the objects __str__ implementation, but
+      that might result in an illegal JSON5 value if the object had
+      customized __str__ to return something illegal. Instead,
+      we follow the lead of the `JSON` module and call `int.__repr__`
+      or `float.__repr__` directly.
+    * While I was at it, I added tests for dumps(-inf) and dumps(nan)
+      when those were supposed to be disallowed by `allow_nan=False`.
 * v0.9.8 (2022-05-08)
     * [GitHub issue #47](https://github.com/dpranke/pyjson5/issues/47)
       Fixed error reporting in some cases due to how parsing was handling
       nested rules in the grammar - previously the reported location for
       the error could be far away from the point where it actually happened.
 
 * v0.9.7 (2022-05-06)
```

### Comparing `json5-0.9.8/json5/__init__.py` & `json5-0.9.9/json5/__init__.py`

 * *Files identical despite different names*

### Comparing `json5-0.9.8/json5/__main__.py` & `json5-0.9.9/json5/__main__.py`

 * *Files identical despite different names*

### Comparing `json5-0.9.8/json5/arg_parser.py` & `json5-0.9.9/json5/arg_parser.py`

 * *Files identical despite different names*

### Comparing `json5-0.9.8/json5/host.py` & `json5-0.9.9/json5/host.py`

 * *Files identical despite different names*

### Comparing `json5-0.9.8/json5/lib.py` & `json5-0.9.9/json5/lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -260,23 +260,44 @@
            seen, level, is_key):
     if obj is True:
         s = u'true'
     elif obj is False:
         s = u'false'
     elif obj is None:
         s = u'null'
+    elif obj == math.inf:
+        if allow_nan:
+            s = u'Infinity'
+        else:
+            raise ValueError()
+    elif obj == -math.inf:
+        if allow_nan:
+            s = u'-Infinity'
+        else:
+            raise ValueError()
+    elif isinstance(obj, float) and math.isnan(obj):
+        if allow_nan:
+            s = u'NaN'
+        else:
+            raise ValueError()
     elif isinstance(obj, str_types):
         if (is_key and _is_ident(obj) and not quote_keys
             and not _is_reserved_word(obj)):
             return True, obj
         return True, _dump_str(obj, ensure_ascii)
-    elif isinstance(obj, float):
-        s = _dump_float(obj,allow_nan)
     elif isinstance(obj, int):
-        s = str(obj)
+        # Subclasses of `int` and `float` may have custom
+        # __repr__ or __str__ methods, but the `JSON` library
+        # ignores them in order to ensure that the representation
+        # are just bare numbers. In order to match JSON's behavior
+        # we call the methods of the `float` and `int` class directly.
+        s = int.__repr__(obj)
+    elif isinstance(obj, float):
+        # See comment above for int
+        s = float.__repr__(obj)
     else:
         s = None
 
     if is_key:
         if s is not None:
             return True, '"%s"' % s
         if skipkeys:
@@ -399,28 +420,14 @@
                                   allow_nan, indent, separators, default,
                                   sort_keys, quote_keys, trailing_commas,
                                   allow_duplicate_keys,
                                   seen, level, False)[1] for el in obj]) +
             end_str + u']')
 
 
-def _dump_float(obj, allow_nan):
-    if allow_nan:
-        if math.isnan(obj):
-            return 'NaN'
-        if obj == float('inf'):
-            return 'Infinity'
-        if obj == float('-inf'):
-            return '-Infinity'
-    elif math.isnan(obj) or obj == float('inf') or obj == float('-inf'):
-        raise ValueError('Out of range float values '
-                         'are not JSON compliant')
-    return str(obj)
-
-
 def _dump_str(obj, ensure_ascii):
     ret = ['"']
     for ch in obj:
         if ch == '\\':
             ret.append('\\\\')
         elif ch == '"':
             ret.append('\\"')
```

### Comparing `json5-0.9.8/json5/parser.py` & `json5-0.9.9/json5/parser.py`

 * *Files identical despite different names*

### Comparing `json5-0.9.8/json5/tool.py` & `json5-0.9.9/json5/tool.py`

 * *Files identical despite different names*

### Comparing `json5-0.9.8/json5/version.py` & `json5-0.9.9/json5/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = '0.9.8'
+VERSION = '0.9.9'
```

### Comparing `json5-0.9.8/json5.egg-info/PKG-INFO` & `json5-0.9.9/json5.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: json5
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Python implementation of the JSON5 data format.
 Home-page: https://github.com/dpranke/pyjson5
 Author: Dirk Pranke
 Author-email: dpranke@chromium.org
 License: Apache
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -73,14 +72,24 @@
 ## Running the tests
 To run the tests, setup a venv and install the required dependencies with
 `pip install -e '.[dev]'`, then run the tests with `python setup.py test`.
 
 
 ## Version History / Release Notes
 
+* v0.9.9 (2022-08-01)
+    * [GitHub issue #57](https://github.com/dpranke/pyjson5/issues/57)
+      Fixed serialization for objects that subclass `int` or `float`:
+      Previously we would use the objects __str__ implementation, but
+      that might result in an illegal JSON5 value if the object had
+      customized __str__ to return something illegal. Instead,
+      we follow the lead of the `JSON` module and call `int.__repr__`
+      or `float.__repr__` directly.
+    * While I was at it, I added tests for dumps(-inf) and dumps(nan)
+      when those were supposed to be disallowed by `allow_nan=False`.
 * v0.9.8 (2022-05-08)
     * [GitHub issue #47](https://github.com/dpranke/pyjson5/issues/47)
       Fixed error reporting in some cases due to how parsing was handling
       nested rules in the grammar - previously the reported location for
       the error could be far away from the point where it actually happened.
 
 * v0.9.7 (2022-05-06)
@@ -195,9 +204,7 @@
 
 * v0.6.0 (2017-11-28)
     * First implementation that attempted to implement 100% of the spec.
 
 * v0.5.0 (2017-09-04)
     * First implementation that supported the full set of kwargs that
       the `json` module supports.
-
-
```

### Comparing `json5-0.9.8/setup.py` & `json5-0.9.9/setup.py`

 * *Files identical despite different names*

