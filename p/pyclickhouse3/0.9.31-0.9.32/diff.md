# Comparing `tmp/pyclickhouse3-0.9.31.tar.gz` & `tmp/pyclickhouse3-0.9.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclickhouse3-0.9.31.tar", last modified: Thu Jan 26 12:28:02 2023, max compression
+gzip compressed data, was "pyclickhouse3-0.9.32.tar", last modified: Mon May 15 07:49:44 2023, max compression
```

## Comparing `pyclickhouse3-0.9.31.tar` & `pyclickhouse3-0.9.32.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-01-26 12:28:02.099707 pyclickhouse3-0.9.31/
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    11357 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.31/LICENSE
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-01-26 12:28:02.099707 pyclickhouse3-0.9.31/PKG-INFO
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1779 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.31/README.md
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-01-26 12:28:02.099707 pyclickhouse3-0.9.31/pyclickhouse/
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     8887 2022-05-20 10:07:52.000000 pyclickhouse3-0.9.31/pyclickhouse/Connection.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    25465 2023-01-23 16:34:27.000000 pyclickhouse3-0.9.31/pyclickhouse/Cursor.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     3702 2021-09-29 15:05:05.000000 pyclickhouse3-0.9.31/pyclickhouse/FilterableCache.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       61 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.31/pyclickhouse/__init__.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    23708 2023-01-26 12:27:25.000000 pyclickhouse3-0.9.31/pyclickhouse/formatter.py
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-01-26 12:28:02.099707 pyclickhouse3-0.9.31/pyclickhouse3.egg-info/
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-01-26 12:28:02.000000 pyclickhouse3-0.9.31/pyclickhouse3.egg-info/PKG-INFO
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      485 2023-01-26 12:28:02.000000 pyclickhouse3-0.9.31/pyclickhouse3.egg-info/SOURCES.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2023-01-26 12:28:02.000000 pyclickhouse3-0.9.31/pyclickhouse3.egg-info/dependency_links.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2021-02-10 13:40:28.000000 pyclickhouse3-0.9.31/pyclickhouse3.egg-info/not-zip-safe
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)       30 2023-01-26 12:28:02.000000 pyclickhouse3-0.9.31/pyclickhouse3.egg-info/requires.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)       13 2023-01-26 12:28:02.000000 pyclickhouse3-0.9.31/pyclickhouse3.egg-info/top_level.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      103 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.31/pyproject.toml
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       79 2023-01-26 12:28:02.099707 pyclickhouse3-0.9.31/setup.cfg
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)      691 2023-01-26 12:27:25.000000 pyclickhouse3-0.9.31/setup.py
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-01-26 12:28:02.099707 pyclickhouse3-0.9.31/test/
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1560 2023-01-23 10:37:59.000000 pyclickhouse3-0.9.31/test/test_compatibility.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     2613 2023-01-23 14:27:59.000000 pyclickhouse3-0.9.31/test/test_map.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    10330 2023-01-26 12:08:31.000000 pyclickhouse3-0.9.31/test/test_new.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     4759 2023-01-23 10:49:05.000000 pyclickhouse3-0.9.31/test/test_simple.py
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    11357 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.32/LICENSE
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/PKG-INFO
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1779 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.32/README.md
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/pyclickhouse/
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     8887 2022-05-20 10:07:52.000000 pyclickhouse3-0.9.32/pyclickhouse/Connection.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    25465 2023-01-23 16:34:27.000000 pyclickhouse3-0.9.32/pyclickhouse/Cursor.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     3702 2021-09-29 15:05:05.000000 pyclickhouse3-0.9.32/pyclickhouse/FilterableCache.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       61 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.32/pyclickhouse/__init__.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    23715 2023-05-15 07:48:35.000000 pyclickhouse3-0.9.32/pyclickhouse/formatter.py
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/PKG-INFO
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      485 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/SOURCES.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/dependency_links.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2021-02-10 13:40:28.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/not-zip-safe
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)       25 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/requires.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)       13 2023-05-15 07:49:44.000000 pyclickhouse3-0.9.32/pyclickhouse3.egg-info/top_level.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      103 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.32/pyproject.toml
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       79 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/setup.cfg
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)      683 2023-05-15 07:49:32.000000 pyclickhouse3-0.9.32/setup.py
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 07:49:44.490765 pyclickhouse3-0.9.32/test/
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1560 2023-01-23 10:37:59.000000 pyclickhouse3-0.9.32/test/test_compatibility.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     2613 2023-01-23 14:27:59.000000 pyclickhouse3-0.9.32/test/test_map.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    10330 2023-01-26 12:08:31.000000 pyclickhouse3-0.9.32/test/test_new.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     4759 2023-01-23 10:49:05.000000 pyclickhouse3-0.9.32/test/test_simple.py
```

### Comparing `pyclickhouse3-0.9.31/LICENSE` & `pyclickhouse3-0.9.32/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.31/README.md` & `pyclickhouse3-0.9.32/README.md`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.31/pyclickhouse/Connection.py` & `pyclickhouse3-0.9.32/pyclickhouse/Connection.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.31/pyclickhouse/Cursor.py` & `pyclickhouse3-0.9.32/pyclickhouse/Cursor.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.31/pyclickhouse/FilterableCache.py` & `pyclickhouse3-0.9.32/pyclickhouse/FilterableCache.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.31/pyclickhouse/formatter.py` & `pyclickhouse3-0.9.32/pyclickhouse/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import numpy as np
-import pytz
+from dateutil import tz
 import ast
 
 import ujson
 
 import sys
 import datetime as dt
 from decimal import Decimal
@@ -386,15 +386,15 @@
                 value = value[1:]
             if value.endswith("'"):
                 value = value[:-1]
             if value == '0000-00-00 00:00:00' or value == '1970-01-01 86:28:16':
                 return None
             tmp = dt.datetime.strptime(value, '%Y-%m-%d %H:%M:%S')
             if type.startswith('DateTime('):
-                tmp = tmp.replace(tzinfo=pytz.timezone(type.split('(')[1][2:-3]))
+                tmp = tmp.replace(tzinfo=tz.gettz(type.split('(')[1][2:-3]))
             return tmp
         if type.startswith('Array('):
             value = value.replace(',,', ",'',") # workaround empty string clickhouse bug
             parts = ast.literal_eval(value)
 
             def handle_dates(val, typ):
                 if typ.startswith('Date'):
@@ -440,23 +440,23 @@
         types = split[1].split('\t')
 
         dtypes = dict()
         converters = dict()
 
         def make_to_datetime(type):
             if type.startswith('('):
-                tz = pytz.timezone(type.split('(')[1][2:-3])
+                tzinfo = tz.gettz(type.split('(')[1][2:-3])
                 def to_datetime(value):
                     if value.startswith("'"):
                         value = value[1:]
                     if value.endswith("'"):
                         value = value[:-1]
                     if value == '0000-00-00 00:00:00' or value == '1970-01-01 86:28:16':
                         return None
-                    return dt.datetime.strptime(value, '%Y-%m-%d %H:%M:%S').replace(tzinfo=tz)
+                    return dt.datetime.strptime(value, '%Y-%m-%d %H:%M:%S').replace(tzinfo=tzinfo)
             else:
                 def to_datetime(value):
                     if value.startswith("'"):
                         value = value[1:]
                     if value.endswith("'"):
                         value = value[:-1]
                     if value == '0000-00-00 00:00:00' or value == '1970-01-01 86:28:16':
@@ -481,15 +481,15 @@
                 type = type[len('Nullable('):-1]
 
             if 'Array' in type or 'Map' in type:
                 dtypes[field] = np.object
             elif type in ['UInt8', 'UInt16', 'UInt32', 'UInt64', 'Int8', 'Int16', 'Int32', 'Int64']:
                 dtypes[field] = np.float # np.int does not support NANs
             elif type in ['String', 'IPv6']:
-                dtypes[field] = np.str
+                dtypes[field] = str
             elif type in ['Float32', 'Float64']:
                 dtypes[field] = np.float
             elif type == 'Date':
                 converters[field] = to_date
             elif type == 'DateTime' or type.startswith('DateTime('):
                 converters[field] = make_to_datetime(type)
             else:
```

### Comparing `pyclickhouse3-0.9.31/test/test_compatibility.py` & `pyclickhouse3-0.9.32/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.31/test/test_map.py` & `pyclickhouse3-0.9.32/test/test_map.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.31/test/test_new.py` & `pyclickhouse3-0.9.32/test/test_new.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.31/test/test_simple.py` & `pyclickhouse3-0.9.32/test/test_simple.py`

 * *Files identical despite different names*

