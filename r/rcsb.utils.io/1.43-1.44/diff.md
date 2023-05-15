# Comparing `tmp/rcsb.utils.io-1.43.tar.gz` & `tmp/rcsb.utils.io-1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.io-1.43.tar", last modified: Mon May  8 14:04:43 2023, max compression
+gzip compressed data, was "rcsb.utils.io-1.44.tar", last modified: Mon May 15 18:06:41 2023, max compression
```

## Comparing `rcsb.utils.io-1.43.tar` & `rcsb.utils.io-1.44.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.085972 rcsb.utils.io-1.43/
--rw-r--r--   0 vsts      (1001) docker     (122)     9456 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1740 2023-05-08 14:04:43.085972 rcsb.utils.io-1.43/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1024 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.081972 rcsb.utils.io-1.43/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.081972 rcsb.utils.io-1.43/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.085972 rcsb.utils.io-1.43/rcsb/utils/io/
--rw-r--r--   0 vsts      (1001) docker     (122)     1828 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/CacheUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6185 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/CryptUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4635 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/ExecUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12022 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/FastaUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5604 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/FileLock.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25377 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/FileUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12683 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/FtpUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6281 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/GitUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1198 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/HashableDict.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6761 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/IndexUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    32305 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/IoUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/LogUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6341 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/MarshalUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5113 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/ProcessStatusUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6260 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/SftpUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)      796 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/SingletonClass.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1716 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/SplitJoin.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12245 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/StashUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11807 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/StashableBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3145 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14760 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/UrlRequestUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4495 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/rcsb/utils/io/decorators.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 14:04:43.081972 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1740 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      975 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-08 13:59:52.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      423 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-08 14:04:43.000000 rcsb.utils.io-1.43/rcsb.utils.io.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      389 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-08 14:04:43.085972 rcsb.utils.io-1.43/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2271 2023-05-08 13:58:21.000000 rcsb.utils.io-1.43/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 18:06:41.605157 rcsb.utils.io-1.44/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1740 2023-05-15 18:06:41.605157 rcsb.utils.io-1.44/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1024 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 18:06:41.597156 rcsb.utils.io-1.44/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 18:06:41.597156 rcsb.utils.io-1.44/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 18:06:41.605157 rcsb.utils.io-1.44/rcsb/utils/io/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1828 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/CacheUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6185 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/CryptUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4635 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/ExecUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12022 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/FastaUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5604 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/FileLock.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25377 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/FileUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12683 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/FtpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6281 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/GitUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1198 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/HashableDict.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6761 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/IndexUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    32305 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/IoUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/LogUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6341 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/MarshalUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5113 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/ProcessStatusUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6260 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/SftpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      796 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/SingletonClass.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1716 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/SplitJoin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12245 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/StashUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11807 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/StashableBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3145 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14760 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/UrlRequestUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4495 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/rcsb/utils/io/decorators.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 18:06:41.597156 rcsb.utils.io-1.44/rcsb.utils.io.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1740 2023-05-15 18:06:41.000000 rcsb.utils.io-1.44/rcsb.utils.io.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      975 2023-05-15 18:06:41.000000 rcsb.utils.io-1.44/rcsb.utils.io.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-15 18:06:41.000000 rcsb.utils.io-1.44/rcsb.utils.io.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-15 18:01:20.000000 rcsb.utils.io-1.44/rcsb.utils.io.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-05-15 18:06:41.000000 rcsb.utils.io-1.44/rcsb.utils.io.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-15 18:06:41.000000 rcsb.utils.io-1.44/rcsb.utils.io.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      408 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-15 18:06:41.609156 rcsb.utils.io-1.44/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2271 2023-05-15 17:59:51.000000 rcsb.utils.io-1.44/setup.py
```

### Comparing `rcsb.utils.io-1.43/HISTORY.txt` & `rcsb.utils.io-1.44/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -127,8 +127,9 @@
  8-Sep-2022  - V1.36 Resolve pylint issues
  3-Oct-2022  - V1.37 Add options to UrlRequestUtil
  5-Dec-2022  - V1.38 Update UniProt fetching tests
 23-Dec-2022  - V1.39 Configuration changes to support tox 4
 13-Feb-2023  - V1.40 Resolve pylint issues
 14-Mar-2023  - V1.41 Make 'timeout' parameter a keyword argument for instantiating FileUtil object
 15-Mar-2023  - V1.42 Fix checking for remote branches by name in GitUtil()
- 8-May-2023  - V1.43 Use allowed_methods instead of deprecated param in UrlRequestUtil()
+ 8-May-2023  - V1.43 Use allowed_methods instead of deprecated param in UrlRequestUtil()
+15-May-2023  - V1.44 Update urllib3 requirements
```

### Comparing `rcsb.utils.io-1.43/LICENSE` & `rcsb.utils.io-1.44/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/PKG-INFO` & `rcsb.utils.io-1.44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.io
-Version: 1.43
+Version: 1.44
 Summary: RCSB Python I/O Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_io
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.io-1.43/README.md` & `rcsb.utils.io-1.44/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/CacheUtils.py` & `rcsb.utils.io-1.44/rcsb/utils/io/CacheUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/CryptUtils.py` & `rcsb.utils.io-1.44/rcsb/utils/io/CryptUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/ExecUtils.py` & `rcsb.utils.io-1.44/rcsb/utils/io/ExecUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/FastaUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/FastaUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/FileLock.py` & `rcsb.utils.io-1.44/rcsb/utils/io/FileLock.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/FileUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/FileUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/FtpUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/FtpUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/GitUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/GitUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/HashableDict.py` & `rcsb.utils.io-1.44/rcsb/utils/io/HashableDict.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/IndexUtils.py` & `rcsb.utils.io-1.44/rcsb/utils/io/IndexUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/IoUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/IoUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/LogUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/LogUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/MarshalUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/MarshalUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/ProcessStatusUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/ProcessStatusUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/SftpUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/SftpUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/SingletonClass.py` & `rcsb.utils.io-1.44/rcsb/utils/io/SingletonClass.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/SplitJoin.py` & `rcsb.utils.io-1.44/rcsb/utils/io/SplitJoin.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/StashUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/StashUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/StashableBase.py` & `rcsb.utils.io-1.44/rcsb/utils/io/StashableBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/TimeUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/UrlRequestUtil.py` & `rcsb.utils.io-1.44/rcsb/utils/io/UrlRequestUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb/utils/io/decorators.py` & `rcsb.utils.io-1.44/rcsb/utils/io/decorators.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/rcsb.utils.io.egg-info/PKG-INFO` & `rcsb.utils.io-1.44/rcsb.utils.io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.io
-Version: 1.43
+Version: 1.44
 Summary: RCSB Python I/O Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_io
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.io-1.43/rcsb.utils.io.egg-info/SOURCES.txt` & `rcsb.utils.io-1.44/rcsb.utils.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.43/setup.py` & `rcsb.utils.io-1.44/setup.py`

 * *Files identical despite different names*

