# Comparing `tmp/scansegmentdecoding-2.0.2.tar.gz` & `tmp/scansegmentdecoding-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scansegmentdecoding-2.0.2.tar", max compression
+gzip compressed data, was "scansegmentdecoding-2.0.3.tar", max compression
```

## Comparing `scansegmentdecoding-2.0.2.tar` & `scansegmentdecoding-2.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1050 2023-04-27 09:24:01.695738 scansegmentdecoding-2.0.2/LICENSE
--rw-r--r--   0        0        0      440 2023-05-05 11:36:56.589158 scansegmentdecoding-2.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 09:24:01.720738 scansegmentdecoding-2.0.2/scansegmentdecoding/__init__.py
--rw-r--r--   0        0        0     2778 2023-04-27 09:24:01.721738 scansegmentdecoding-2.0.2/scansegmentdecoding/connectionHandler.py
--rw-r--r--   0        0        0     2376 2023-04-27 09:24:01.725737 scansegmentdecoding-2.0.2/scansegmentdecoding/decodeUtil.py
--rw-r--r--   0        0        0     3388 2023-04-27 09:24:01.729739 scansegmentdecoding-2.0.2/scansegmentdecoding/msgpackUtil.py
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 scansegmentdecoding-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1050 2023-05-08 06:17:28.854924 scansegmentdecoding-2.0.3/LICENSE
+-rw-r--r--   0        0        0      439 2023-05-15 08:55:21.845169 scansegmentdecoding-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 06:17:28.879919 scansegmentdecoding-2.0.3/scansegmentdecoding/__init__.py
+-rw-r--r--   0        0        0     2778 2023-05-08 06:17:28.880917 scansegmentdecoding-2.0.3/scansegmentdecoding/connectionHandler.py
+-rw-r--r--   0        0        0     2376 2023-05-08 06:17:28.892929 scansegmentdecoding-2.0.3/scansegmentdecoding/decodeUtil.py
+-rw-r--r--   0        0        0     3388 2023-05-08 06:17:28.898927 scansegmentdecoding-2.0.3/scansegmentdecoding/msgpackUtil.py
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 scansegmentdecoding-2.0.3/PKG-INFO
```

### Comparing `scansegmentdecoding-2.0.2/LICENSE` & `scansegmentdecoding-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scansegmentdecoding-2.0.2/scansegmentdecoding/connectionHandler.py` & `scansegmentdecoding-2.0.3/scansegmentdecoding/connectionHandler.py`

 * *Files identical despite different names*

### Comparing `scansegmentdecoding-2.0.2/scansegmentdecoding/decodeUtil.py` & `scansegmentdecoding-2.0.3/scansegmentdecoding/decodeUtil.py`

 * *Files identical despite different names*

### Comparing `scansegmentdecoding-2.0.2/scansegmentdecoding/msgpackUtil.py` & `scansegmentdecoding-2.0.3/scansegmentdecoding/msgpackUtil.py`

 * *Files identical despite different names*

