# Comparing `tmp/acquire-3.6.dev7.tar.gz` & `tmp/acquire-3.6.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.6.dev7.tar", last modified: Tue May  2 12:42:54 2023, max compression
+gzip compressed data, was "acquire-3.6.dev8.tar", last modified: Mon May 15 12:44:54 2023, max compression
```

## Comparing `acquire-3.6.dev7.tar` & `acquire-3.6.dev8.tar`

### file list

```diff
@@ -1,59 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.400156 acquire-3.6.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 12:42:39.000000 acquire-3.6.dev7/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-02 12:42:39.000000 acquire-3.6.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 12:42:39.000000 acquire-3.6.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-02 12:42:54.400156 acquire-3.6.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-02 12:42:39.000000 acquire-3.6.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.392156 acquire-3.6.dev7/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75961 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.400156 acquire-3.6.dev7/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-02 12:42:44.000000 acquire-3.6.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:42:54.400156 acquire-3.6.dev7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.400156 acquire-3.6.dev7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.021101 acquire-3.6.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-15 12:44:40.000000 acquire-3.6.dev8/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:44:40.000000 acquire-3.6.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:44:40.000000 acquire-3.6.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-15 12:44:54.021101 acquire-3.6.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-15 12:44:40.000000 acquire-3.6.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75961 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.021101 acquire-3.6.dev8/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-15 12:44:54.000000 acquire-3.6.dev8/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-15 12:44:44.000000 acquire-3.6.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:44:54.021101 acquire-3.6.dev8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.021101 acquire-3.6.dev8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.021101 acquire-3.6.dev8/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tox.ini
```

### Comparing `acquire-3.6.dev7/LICENSE` & `acquire-3.6.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/PKG-INFO` & `acquire-3.6.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev7
+Version: 3.6.dev8
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev7/README.md` & `acquire-3.6.dev8/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/acquire.py` & `acquire-3.6.dev8/acquire/acquire.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/collector.py` & `acquire-3.6.dev8/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/crypt.py` & `acquire-3.6.dev8/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/dynamic/windows/collect.py` & `acquire-3.6.dev8/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/dynamic/windows/handles.py` & `acquire-3.6.dev8/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/dynamic/windows/named_objects.py` & `acquire-3.6.dev8/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/dynamic/windows/ntdll.py` & `acquire-3.6.dev8/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/dynamic/windows/types.py` & `acquire-3.6.dev8/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/esxi.py` & `acquire-3.6.dev8/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/hashes.py` & `acquire-3.6.dev8/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/log.py` & `acquire-3.6.dev8/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/outputs/base.py` & `acquire-3.6.dev8/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/outputs/dir.py` & `acquire-3.6.dev8/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/outputs/tar.py` & `acquire-3.6.dev8/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/tools/decrypter.py` & `acquire-3.6.dev8/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/uploaders/minio.py` & `acquire-3.6.dev8/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/uploaders/plugin.py` & `acquire-3.6.dev8/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/uploaders/plugin_registry.py` & `acquire-3.6.dev8/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire/utils.py` & `acquire-3.6.dev8/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/acquire.egg-info/PKG-INFO` & `acquire-3.6.dev8/acquire.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev7
+Version: 3.6.dev8
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev7/acquire.egg-info/SOURCES.txt` & `acquire-3.6.dev8/acquire.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -41,8 +41,11 @@
 tests/conftest.py
 tests/test_acquire_command.py
 tests/test_collector.py
 tests/test_esxi_memory.py
 tests/test_file_sorting.py
 tests/test_minio_uploader.py
 tests/test_plugin.py
-tests/test_utils.py
+tests/test_utils.py
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `acquire-3.6.dev7/pyproject.toml` & `acquire-3.6.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/tests/conftest.py` & `acquire-3.6.dev8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/tests/test_acquire_command.py` & `acquire-3.6.dev8/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/tests/test_collector.py` & `acquire-3.6.dev8/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/tests/test_esxi_memory.py` & `acquire-3.6.dev8/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/tests/test_file_sorting.py` & `acquire-3.6.dev8/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/tests/test_minio_uploader.py` & `acquire-3.6.dev8/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/tests/test_plugin.py` & `acquire-3.6.dev8/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev7/tests/test_utils.py` & `acquire-3.6.dev8/tests/test_utils.py`

 * *Files identical despite different names*

