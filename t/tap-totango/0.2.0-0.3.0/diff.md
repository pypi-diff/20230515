# Comparing `tmp/tap_totango-0.2.0.tar.gz` & `tmp/tap_totango-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_totango-0.2.0.tar", max compression
+gzip compressed data, was "tap_totango-0.3.0.tar", max compression
```

## Comparing `tap_totango-0.2.0.tar` & `tap_totango-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2944 2023-05-13 19:27:45.024895 tap_totango-0.2.0/README.md
--rw-r--r--   0        0        0     1133 2023-05-14 01:50:14.081654 tap_totango-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-13 00:04:24.083057 tap_totango-0.2.0/tap_totango/__init__.py
--rw-r--r--   0        0        0     4583 2023-05-13 16:21:54.720246 tap_totango-0.2.0/tap_totango/client.py
--rw-r--r--   0        0        0      431 2023-05-13 22:00:37.289103 tap_totango-0.2.0/tap_totango/schemas/accounts.json
--rw-r--r--   0        0        0     1878 2023-05-13 16:35:50.832342 tap_totango-0.2.0/tap_totango/schemas/events.json
--rw-r--r--   0        0        0      918 2023-05-14 01:35:34.115672 tap_totango-0.2.0/tap_totango/schemas/users.json
--rw-r--r--   0        0        0     4764 2023-05-14 01:28:57.199660 tap_totango-0.2.0/tap_totango/streams.py
--rw-r--r--   0        0        0     6528 2023-05-14 01:22:13.452744 tap_totango-0.2.0/tap_totango/tap.py
--rw-r--r--   0        0        0     3685 1970-01-01 00:00:00.000000 tap_totango-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     9247 2023-05-14 23:55:50.616372 tap_totango-0.3.0/README.md
+-rw-r--r--   0        0        0     1141 2023-05-15 00:56:24.204530 tap_totango-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-13 00:04:24.083057 tap_totango-0.3.0/tap_totango/__init__.py
+-rw-r--r--   0        0        0     4583 2023-05-13 16:21:54.720246 tap_totango-0.3.0/tap_totango/client.py
+-rw-r--r--   0        0        0      431 2023-05-13 22:00:37.289103 tap_totango-0.3.0/tap_totango/schemas/accounts.json
+-rw-r--r--   0        0        0     1878 2023-05-13 16:35:50.832342 tap_totango-0.3.0/tap_totango/schemas/events.json
+-rw-r--r--   0        0        0      918 2023-05-14 01:35:34.115672 tap_totango-0.3.0/tap_totango/schemas/users.json
+-rw-r--r--   0        0        0     4764 2023-05-14 01:28:57.199660 tap_totango-0.3.0/tap_totango/streams.py
+-rw-r--r--   0        0        0    10271 2023-05-15 00:40:19.613886 tap_totango-0.3.0/tap_totango/tap.py
+-rw-r--r--   0        0        0     9996 1970-01-01 00:00:00.000000 tap_totango-0.3.0/PKG-INFO
```

### Comparing `tap_totango-0.2.0/pyproject.toml` & `tap_totango-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tap-totango"
-version = "0.2.0"
-description = "`tap-totango` is a Singer tap for totango, built with the Meltano Singer SDK."
+version = "0.3.0"
+description = "`tap-totango` is a Singer tap for the Totango API, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Edson Nogueira"]
 keywords = [
     "ELT",
     "totango",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_totango-0.2.0/tap_totango/client.py` & `tap_totango-0.3.0/tap_totango/client.py`

 * *Files identical despite different names*

### Comparing `tap_totango-0.2.0/tap_totango/schemas/events.json` & `tap_totango-0.3.0/tap_totango/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap_totango-0.2.0/tap_totango/schemas/users.json` & `tap_totango-0.3.0/tap_totango/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap_totango-0.2.0/tap_totango/streams.py` & `tap_totango-0.3.0/tap_totango/streams.py`

 * *Files identical despite different names*

