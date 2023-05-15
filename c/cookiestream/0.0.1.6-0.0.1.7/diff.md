# Comparing `tmp/cookiestream-0.0.1.6.tar.gz` & `tmp/cookiestream-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiestream-0.0.1.6.tar", last modified: Mon May 15 00:32:45 2023, max compression
+gzip compressed data, was "cookiestream-0.0.1.7.tar", last modified: Mon May 15 00:36:31 2023, max compression
```

## Comparing `cookiestream-0.0.1.6.tar` & `cookiestream-0.0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:32:45.248209 cookiestream-0.0.1.6/
--rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-10 23:11:22.000000 cookiestream-0.0.1.6/LICENCE
--rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-15 00:32:45.248209 cookiestream-0.0.1.6/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-10 23:11:22.000000 cookiestream-0.0.1.6/README.md
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:32:45.248209 cookiestream-0.0.1.6/configs/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.6/configs/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      234 2023-05-11 21:21:05.000000 cookiestream-0.0.1.6/configs/base_config.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:32:45.248209 cookiestream-0.0.1.6/cookiestream/
--rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-15 00:06:49.000000 cookiestream-0.0.1.6/cookiestream/__init__.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:32:45.248209 cookiestream-0.0.1.6/cookiestream/src/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.6/cookiestream/src/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      432 2023-05-11 22:08:24.000000 cookiestream-0.0.1.6/cookiestream/src/clone_template.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1978 2023-05-11 22:46:42.000000 cookiestream-0.0.1.6/cookiestream/src/make_rename.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     2906 2023-05-14 17:49:27.000000 cookiestream-0.0.1.6/cookiestream/src/modify_yaml_content.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     3781 2023-05-14 20:22:06.000000 cookiestream-0.0.1.6/cookiestream/src/stream.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:32:45.248209 cookiestream-0.0.1.6/cookiestream.egg-info/
--rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-15 00:32:45.000000 cookiestream-0.0.1.6/cookiestream.egg-info/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)      546 2023-05-15 00:32:45.000000 cookiestream-0.0.1.6/cookiestream.egg-info/SOURCES.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-15 00:32:45.000000 cookiestream-0.0.1.6/cookiestream.egg-info/dependency_links.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       56 2023-05-15 00:32:45.000000 cookiestream-0.0.1.6/cookiestream.egg-info/entry_points.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       29 2023-05-15 00:32:45.000000 cookiestream-0.0.1.6/cookiestream.egg-info/requires.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       71 2023-05-15 00:32:45.000000 cookiestream-0.0.1.6/cookiestream.egg-info/top_level.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)      327 2023-05-15 00:28:23.000000 cookiestream-0.0.1.6/main_cookiestream.py
--rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-15 00:32:45.252209 cookiestream-0.0.1.6/setup.cfg
--rw-rw-r--   0 zied      (1000) zied      (1000)     2187 2023-05-15 00:32:33.000000 cookiestream-0.0.1.6/setup.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:32:45.248209 cookiestream-0.0.1.6/utils/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.6/utils/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-10 23:11:22.000000 cookiestream-0.0.1.6/utils/util.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:36:31.103502 cookiestream-0.0.1.7/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-10 23:11:22.000000 cookiestream-0.0.1.7/LICENCE
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-15 00:36:31.103502 cookiestream-0.0.1.7/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-10 23:11:22.000000 cookiestream-0.0.1.7/README.md
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:36:31.099502 cookiestream-0.0.1.7/configs/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.7/configs/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      234 2023-05-11 21:21:05.000000 cookiestream-0.0.1.7/configs/base_config.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:36:31.099502 cookiestream-0.0.1.7/cookiestream/
+-rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-15 00:06:49.000000 cookiestream-0.0.1.7/cookiestream/__init__.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:36:31.103502 cookiestream-0.0.1.7/cookiestream/src/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.7/cookiestream/src/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      432 2023-05-11 22:08:24.000000 cookiestream-0.0.1.7/cookiestream/src/clone_template.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1978 2023-05-11 22:46:42.000000 cookiestream-0.0.1.7/cookiestream/src/make_rename.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2906 2023-05-14 17:49:27.000000 cookiestream-0.0.1.7/cookiestream/src/modify_yaml_content.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3781 2023-05-14 20:22:06.000000 cookiestream-0.0.1.7/cookiestream/src/stream.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:36:31.103502 cookiestream-0.0.1.7/cookiestream.egg-info/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-15 00:36:30.000000 cookiestream-0.0.1.7/cookiestream.egg-info/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)      546 2023-05-15 00:36:31.000000 cookiestream-0.0.1.7/cookiestream.egg-info/SOURCES.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-15 00:36:30.000000 cookiestream-0.0.1.7/cookiestream.egg-info/dependency_links.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       56 2023-05-15 00:36:30.000000 cookiestream-0.0.1.7/cookiestream.egg-info/entry_points.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       29 2023-05-15 00:36:30.000000 cookiestream-0.0.1.7/cookiestream.egg-info/requires.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       71 2023-05-15 00:36:30.000000 cookiestream-0.0.1.7/cookiestream.egg-info/top_level.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)      327 2023-05-15 00:35:38.000000 cookiestream-0.0.1.7/main_cookiestream.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-15 00:36:31.103502 cookiestream-0.0.1.7/setup.cfg
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2187 2023-05-15 00:32:33.000000 cookiestream-0.0.1.7/setup.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:36:31.099502 cookiestream-0.0.1.7/utils/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.7/utils/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-10 23:11:22.000000 cookiestream-0.0.1.7/utils/util.py
```

### Comparing `cookiestream-0.0.1.6/LICENCE` & `cookiestream-0.0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.6/PKG-INFO` & `cookiestream-0.0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiestream
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: Generate template based on template_vierge project
 Home-page: https://github.com/Proxia-ai/cookiestream
 Author: BEN OTHMANE Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/Proxia-ai/cookiestream/issues
 Keywords: Python pypi template,python
```

### Comparing `cookiestream-0.0.1.6/README.md` & `cookiestream-0.0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.6/cookiestream/src/make_rename.py` & `cookiestream-0.0.1.7/cookiestream/src/make_rename.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.6/cookiestream/src/modify_yaml_content.py` & `cookiestream-0.0.1.7/cookiestream/src/modify_yaml_content.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.6/cookiestream/src/stream.py` & `cookiestream-0.0.1.7/cookiestream/src/stream.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.6/cookiestream.egg-info/PKG-INFO` & `cookiestream-0.0.1.7/cookiestream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiestream
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: Generate template based on template_vierge project
 Home-page: https://github.com/Proxia-ai/cookiestream
 Author: BEN OTHMANE Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/Proxia-ai/cookiestream/issues
 Keywords: Python pypi template,python
```

### Comparing `cookiestream-0.0.1.6/cookiestream.egg-info/SOURCES.txt` & `cookiestream-0.0.1.7/cookiestream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.6/setup.py` & `cookiestream-0.0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.6/utils/util.py` & `cookiestream-0.0.1.7/utils/util.py`

 * *Files identical despite different names*

