# Comparing `tmp/dissect.ntfs-3.5.dev1.tar.gz` & `tmp/dissect.ntfs-3.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ntfs-3.5.dev1.tar", last modified: Thu Apr  6 22:09:20 2023, max compression
+gzip compressed data, was "dissect.ntfs-3.5.dev2.tar", last modified: Mon May 15 12:48:22 2023, max compression
```

## Comparing `dissect.ntfs-3.5.dev1.tar` & `dissect.ntfs-3.5.dev2.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:09:20.383600 dissect.ntfs-3.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-06 22:09:20.383600 dissect.ntfs-3.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:09:20.375599 dissect.ntfs-3.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:09:20.379600 dissect.ntfs-3.5.dev1/dissect/ntfs/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/c_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/dissect/ntfs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:09:20.375599 dissect.ntfs-3.5.dev1/dissect.ntfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-06 22:09:20.000000 dissect.ntfs-3.5.dev1/dissect.ntfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-06 22:09:20.000000 dissect.ntfs-3.5.dev1/dissect.ntfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 22:09:20.000000 dissect.ntfs-3.5.dev1/dissect.ntfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-06 22:09:20.000000 dissect.ntfs-3.5.dev1/dissect.ntfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-06 22:09:20.000000 dissect.ntfs-3.5.dev1/dissect.ntfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-06 22:09:08.000000 dissect.ntfs-3.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 22:09:20.383600 dissect.ntfs-3.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:09:20.379600 dissect.ntfs-3.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:09:20.383600 dissect.ntfs-3.5.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/data/boot_2m.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/data/mft.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/data/ntfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/data/ntfs_fragmented_mft.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/data/sds.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/test_mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/test_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/test_secure.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/test_usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-06 22:09:03.000000 dissect.ntfs-3.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:22.262694 dissect.ntfs-3.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-15 12:48:22.262694 dissect.ntfs-3.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:22.238694 dissect.ntfs-3.5.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:22.250694 dissect.ntfs-3.5.dev2/dissect/ntfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/c_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/dissect/ntfs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:22.242694 dissect.ntfs-3.5.dev2/dissect.ntfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-15 12:48:22.000000 dissect.ntfs-3.5.dev2/dissect.ntfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-15 12:48:22.000000 dissect.ntfs-3.5.dev2/dissect.ntfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:22.000000 dissect.ntfs-3.5.dev2/dissect.ntfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:22.000000 dissect.ntfs-3.5.dev2/dissect.ntfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:22.000000 dissect.ntfs-3.5.dev2/dissect.ntfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-15 12:48:07.000000 dissect.ntfs-3.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:22.262694 dissect.ntfs-3.5.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:22.254694 dissect.ntfs-3.5.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:22.258694 dissect.ntfs-3.5.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/data/boot_2m.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/data/mft.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/data/ntfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/data/ntfs_fragmented_mft.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/data/sds.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:22.258694 dissect.ntfs-3.5.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/test_mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/test_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/test_secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/test_usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:59.000000 dissect.ntfs-3.5.dev2/tox.ini
```

### Comparing `dissect.ntfs-3.5.dev1/LICENSE` & `dissect.ntfs-3.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/PKG-INFO` & `dissect.ntfs-3.5.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.ntfs-3.5.dev1/README.md` & `dissect.ntfs-3.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/__init__.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/attr.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/c_ntfs.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/c_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/index.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/mft.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/mft.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/ntfs.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/secure.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/stream.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/usnjrnl.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect/ntfs/util.py` & `dissect.ntfs-3.5.dev2/dissect/ntfs/util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/dissect.ntfs.egg-info/PKG-INFO` & `dissect.ntfs-3.5.dev2/dissect.ntfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.ntfs-3.5.dev1/dissect.ntfs.egg-info/SOURCES.txt` & `dissect.ntfs-3.5.dev2/dissect.ntfs.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -29,8 +29,11 @@
 tests/test_secure.py
 tests/test_usnjrnl.py
 tests/test_util.py
 tests/data/boot_2m.bin.gz
 tests/data/mft.bin.gz
 tests/data/ntfs.bin.gz
 tests/data/ntfs_fragmented_mft.csv.gz
-tests/data/sds.bin.gz
+tests/data/sds.bin.gz
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.ntfs-3.5.dev1/pyproject.toml` & `dissect.ntfs-3.5.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/conftest.py` & `dissect.ntfs-3.5.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/data/boot_2m.bin.gz` & `dissect.ntfs-3.5.dev2/tests/data/boot_2m.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/data/mft.bin.gz` & `dissect.ntfs-3.5.dev2/tests/data/mft.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/data/ntfs.bin.gz` & `dissect.ntfs-3.5.dev2/tests/data/ntfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/data/ntfs_fragmented_mft.csv.gz` & `dissect.ntfs-3.5.dev2/tests/data/ntfs_fragmented_mft.csv.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/data/sds.bin.gz` & `dissect.ntfs-3.5.dev2/tests/data/sds.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/test_attr.py` & `dissect.ntfs-3.5.dev2/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/test_index.py` & `dissect.ntfs-3.5.dev2/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/test_mft.py` & `dissect.ntfs-3.5.dev2/tests/test_mft.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/test_ntfs.py` & `dissect.ntfs-3.5.dev2/tests/test_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/test_secure.py` & `dissect.ntfs-3.5.dev2/tests/test_secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/test_usnjrnl.py` & `dissect.ntfs-3.5.dev2/tests/test_usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tests/test_util.py` & `dissect.ntfs-3.5.dev2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.5.dev1/tox.ini` & `dissect.ntfs-3.5.dev2/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -51,7 +51,27 @@
 
 [flake8]
 max-line-length = 120
 extend-ignore =
     # See https://github.com/PyCQA/pycodestyle/issues/373
     E203,
 statistics = True
+
+[testenv:docs-build]
+allowlist_externals = make
+deps =
+    sphinx
+    sphinx-autoapi
+    sphinx_argparse_cli
+    sphinx-copybutton
+    sphinx-design
+    furo
+commands =
+    make -C tests/docs clean
+    make -C tests/docs html
+
+[testenv:docs-linkcheck]
+allowlist_externals = make
+deps = {[testenv:docs-build]deps}
+commands =
+    make -C tests/docs clean
+    make -C tests/docs linkcheck
```

