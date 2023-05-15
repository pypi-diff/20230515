# Comparing `tmp/pyassorted-0.5.0.tar.gz` & `tmp/pyassorted-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassorted-0.5.0.tar", max compression
+gzip compressed data, was "pyassorted-0.6.0.tar", max compression
```

## Comparing `pyassorted-0.5.0.tar` & `pyassorted-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.5.0/LICENSE
--rw-r--r--   0        0        0     1799 2023-04-01 13:44:09.331817 pyassorted-0.5.0/README.md
--rw-r--r--   0        0        0       53 2023-04-01 13:44:09.334164 pyassorted-0.5.0/pyassorted/__init__.py
--rw-r--r--   0        0        0      116 2023-02-17 09:28:12.934937 pyassorted-0.5.0/pyassorted/asyncio/__init__.py
--rw-r--r--   0        0        0     1349 2023-04-01 13:44:09.334680 pyassorted-0.5.0/pyassorted/asyncio/executor.py
--rw-r--r--   0        0        0     1017 2023-02-15 09:50:56.450314 pyassorted-0.5.0/pyassorted/asyncio/utils.py
--rw-r--r--   0        0        0       61 2023-03-27 15:28:16.228462 pyassorted-0.5.0/pyassorted/cache/__init__.py
--rw-r--r--   0        0        0     8109 2023-03-27 15:28:16.228823 pyassorted-0.5.0/pyassorted/cache/cache.py
--rw-r--r--   0        0        0      148 2023-04-26 07:11:33.288957 pyassorted-0.5.0/pyassorted/datetime/__init__.py
--rw-r--r--   0        0        0     1052 2023-04-26 03:26:51.215458 pyassorted-0.5.0/pyassorted/datetime/datetime.py
--rw-r--r--   0        0        0     1001 2023-04-26 09:05:15.499398 pyassorted-0.5.0/pyassorted/datetime/timer.py
--rw-r--r--   0        0        0       56 2023-04-01 13:44:09.335149 pyassorted-0.5.0/pyassorted/lock/__init__.py
--rw-r--r--   0        0        0     4191 2023-04-01 13:44:09.335570 pyassorted-0.5.0/pyassorted/lock/filelock.py
--rw-r--r--   0        0        0       18 2023-04-01 13:44:09.335865 pyassorted-0.5.0/pyassorted/version.py
--rw-r--r--   0        0        0      495 2023-04-27 07:53:32.556778 pyassorted-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 pyassorted-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3072 2023-05-15 11:42:43.730031 pyassorted-0.6.0/README.md
+-rw-r--r--   0        0        0       53 2023-04-01 13:44:09.334164 pyassorted-0.6.0/pyassorted/__init__.py
+-rw-r--r--   0        0        0      116 2023-02-17 09:28:12.934937 pyassorted-0.6.0/pyassorted/asyncio/__init__.py
+-rw-r--r--   0        0        0     1349 2023-04-01 13:44:09.334680 pyassorted-0.6.0/pyassorted/asyncio/executor.py
+-rw-r--r--   0        0        0     2943 2023-05-15 11:04:24.691896 pyassorted-0.6.0/pyassorted/asyncio/io.py
+-rw-r--r--   0        0        0     1017 2023-02-15 09:50:56.450314 pyassorted-0.6.0/pyassorted/asyncio/utils.py
+-rw-r--r--   0        0        0       61 2023-03-27 15:28:16.228462 pyassorted-0.6.0/pyassorted/cache/__init__.py
+-rw-r--r--   0        0        0     8109 2023-03-27 15:28:16.228823 pyassorted-0.6.0/pyassorted/cache/cache.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:33:14.706799 pyassorted-0.6.0/pyassorted/collections/__init__.py
+-rw-r--r--   0        0        0     2853 2023-05-15 11:13:46.316476 pyassorted-0.6.0/pyassorted/collections/sqlitedict.py
+-rw-r--r--   0        0        0      148 2023-05-15 10:33:14.707589 pyassorted-0.6.0/pyassorted/datetime/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-15 10:33:14.707963 pyassorted-0.6.0/pyassorted/datetime/datetime.py
+-rw-r--r--   0        0        0     2013 2023-05-15 11:48:14.665776 pyassorted-0.6.0/pyassorted/datetime/timer.py
+-rw-r--r--   0        0        0     2527 2023-05-15 10:33:14.708765 pyassorted-0.6.0/pyassorted/io/__init__.py
+-rw-r--r--   0        0        0       56 2023-04-01 13:44:09.335149 pyassorted-0.6.0/pyassorted/lock/__init__.py
+-rw-r--r--   0        0        0     4191 2023-04-01 13:44:09.335570 pyassorted-0.6.0/pyassorted/lock/filelock.py
+-rw-r--r--   0        0        0       18 2023-05-15 11:51:11.076029 pyassorted-0.6.0/pyassorted/version.py
+-rw-r--r--   0        0        0      546 2023-05-15 11:51:03.756162 pyassorted-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 pyassorted-0.6.0/PKG-INFO
```

### Comparing `pyassorted-0.5.0/LICENSE` & `pyassorted-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassorted-0.5.0/pyassorted/asyncio/executor.py` & `pyassorted-0.6.0/pyassorted/asyncio/executor.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.5.0/pyassorted/asyncio/utils.py` & `pyassorted-0.6.0/pyassorted/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.5.0/pyassorted/cache/cache.py` & `pyassorted-0.6.0/pyassorted/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.5.0/pyassorted/datetime/datetime.py` & `pyassorted-0.6.0/pyassorted/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.5.0/pyassorted/lock/filelock.py` & `pyassorted-0.6.0/pyassorted/lock/filelock.py`

 * *Files identical despite different names*

