# Comparing `tmp/cookiestream-0.0.1.4.tar.gz` & `tmp/cookiestream-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiestream-0.0.1.4.tar", last modified: Mon May 15 00:07:23 2023, max compression
+gzip compressed data, was "cookiestream-0.0.1.5.tar", last modified: Mon May 15 00:18:44 2023, max compression
```

## Comparing `cookiestream-0.0.1.4.tar` & `cookiestream-0.0.1.5.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:07:23.821963 cookiestream-0.0.1.4/
--rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-10 23:11:22.000000 cookiestream-0.0.1.4/LICENCE
--rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-15 00:07:23.821963 cookiestream-0.0.1.4/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-10 23:11:22.000000 cookiestream-0.0.1.4/README.md
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:07:23.817963 cookiestream-0.0.1.4/configs/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.4/configs/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      234 2023-05-11 21:21:05.000000 cookiestream-0.0.1.4/configs/base_config.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:07:23.817963 cookiestream-0.0.1.4/cookiestream/
--rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-15 00:06:49.000000 cookiestream-0.0.1.4/cookiestream/__init__.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:07:23.821963 cookiestream-0.0.1.4/cookiestream/src/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.4/cookiestream/src/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      432 2023-05-11 22:08:24.000000 cookiestream-0.0.1.4/cookiestream/src/clone_template.py
--rw-rw-r--   0 zied      (1000) zied      (1000)       43 2023-05-15 00:07:15.000000 cookiestream-0.0.1.4/cookiestream/src/hello.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1978 2023-05-11 22:46:42.000000 cookiestream-0.0.1.4/cookiestream/src/make_rename.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     2906 2023-05-14 17:49:27.000000 cookiestream-0.0.1.4/cookiestream/src/modify_yaml_content.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     3781 2023-05-14 20:22:06.000000 cookiestream-0.0.1.4/cookiestream/src/stream.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:07:23.821963 cookiestream-0.0.1.4/cookiestream.egg-info/
--rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-15 00:07:23.000000 cookiestream-0.0.1.4/cookiestream.egg-info/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)      551 2023-05-15 00:07:23.000000 cookiestream-0.0.1.4/cookiestream.egg-info/SOURCES.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-15 00:07:23.000000 cookiestream-0.0.1.4/cookiestream.egg-info/dependency_links.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       68 2023-05-15 00:07:23.000000 cookiestream-0.0.1.4/cookiestream.egg-info/entry_points.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       29 2023-05-15 00:07:23.000000 cookiestream-0.0.1.4/cookiestream.egg-info/requires.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       70 2023-05-15 00:07:23.000000 cookiestream-0.0.1.4/cookiestream.egg-info/top_level.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-15 00:07:23.821963 cookiestream-0.0.1.4/setup.cfg
--rw-rw-r--   0 zied      (1000) zied      (1000)     2160 2023-05-15 00:07:15.000000 cookiestream-0.0.1.4/setup.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:07:23.817963 cookiestream-0.0.1.4/utils/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.4/utils/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-10 23:11:22.000000 cookiestream-0.0.1.4/utils/util.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:18:44.451937 cookiestream-0.0.1.5/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-10 23:11:22.000000 cookiestream-0.0.1.5/LICENCE
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-15 00:18:44.451937 cookiestream-0.0.1.5/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-10 23:11:22.000000 cookiestream-0.0.1.5/README.md
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:18:44.447937 cookiestream-0.0.1.5/configs/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.5/configs/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      234 2023-05-11 21:21:05.000000 cookiestream-0.0.1.5/configs/base_config.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:18:44.447937 cookiestream-0.0.1.5/cookiestream/
+-rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-15 00:06:49.000000 cookiestream-0.0.1.5/cookiestream/__init__.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:18:44.451937 cookiestream-0.0.1.5/cookiestream/src/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.5/cookiestream/src/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      432 2023-05-11 22:08:24.000000 cookiestream-0.0.1.5/cookiestream/src/clone_template.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1978 2023-05-11 22:46:42.000000 cookiestream-0.0.1.5/cookiestream/src/make_rename.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2906 2023-05-14 17:49:27.000000 cookiestream-0.0.1.5/cookiestream/src/modify_yaml_content.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3781 2023-05-14 20:22:06.000000 cookiestream-0.0.1.5/cookiestream/src/stream.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:18:44.447937 cookiestream-0.0.1.5/cookiestream.egg-info/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-15 00:18:44.000000 cookiestream-0.0.1.5/cookiestream.egg-info/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)      525 2023-05-15 00:18:44.000000 cookiestream-0.0.1.5/cookiestream.egg-info/SOURCES.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-15 00:18:44.000000 cookiestream-0.0.1.5/cookiestream.egg-info/dependency_links.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       56 2023-05-15 00:18:44.000000 cookiestream-0.0.1.5/cookiestream.egg-info/entry_points.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       29 2023-05-15 00:18:44.000000 cookiestream-0.0.1.5/cookiestream.egg-info/requires.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       70 2023-05-15 00:18:44.000000 cookiestream-0.0.1.5/cookiestream.egg-info/top_level.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-15 00:18:44.451937 cookiestream-0.0.1.5/setup.cfg
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2184 2023-05-15 00:18:43.000000 cookiestream-0.0.1.5/setup.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-15 00:18:44.447937 cookiestream-0.0.1.5/utils/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.5/utils/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-10 23:11:22.000000 cookiestream-0.0.1.5/utils/util.py
```

### Comparing `cookiestream-0.0.1.4/LICENCE` & `cookiestream-0.0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.4/PKG-INFO` & `cookiestream-0.0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiestream
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: Generate template based on template_vierge project
 Home-page: https://github.com/Proxia-ai/cookiestream
 Author: BEN OTHMANE Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/Proxia-ai/cookiestream/issues
 Keywords: Python pypi template,python
```

### Comparing `cookiestream-0.0.1.4/README.md` & `cookiestream-0.0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.4/cookiestream/src/make_rename.py` & `cookiestream-0.0.1.5/cookiestream/src/make_rename.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.4/cookiestream/src/modify_yaml_content.py` & `cookiestream-0.0.1.5/cookiestream/src/modify_yaml_content.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.4/cookiestream/src/stream.py` & `cookiestream-0.0.1.5/cookiestream/src/stream.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.4/cookiestream.egg-info/PKG-INFO` & `cookiestream-0.0.1.5/cookiestream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiestream
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: Generate template based on template_vierge project
 Home-page: https://github.com/Proxia-ai/cookiestream
 Author: BEN OTHMANE Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/Proxia-ai/cookiestream/issues
 Keywords: Python pypi template,python
```

### Comparing `cookiestream-0.0.1.4/cookiestream.egg-info/SOURCES.txt` & `cookiestream-0.0.1.5/cookiestream.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,11 +11,10 @@
 cookiestream.egg-info/SOURCES.txt
 cookiestream.egg-info/dependency_links.txt
 cookiestream.egg-info/entry_points.txt
 cookiestream.egg-info/requires.txt
 cookiestream.egg-info/top_level.txt
 cookiestream/src/__init__.py
 cookiestream/src/clone_template.py
-cookiestream/src/hello.py
 cookiestream/src/make_rename.py
 cookiestream/src/modify_yaml_content.py
 cookiestream/src/stream.py
```

### Comparing `cookiestream-0.0.1.4/setup.py` & `cookiestream-0.0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,26 +28,27 @@
     project_urls=yaml_asset_config[0]["asset_meta_information"]["project_urls"][0],
     install_requires=requirements,
     classifiers=yaml_asset_config[0]["asset_meta_information"]["classifiers"],
     license='BSD',
     package_data={
         "configs": ["config.ini", "{}_config.yaml".format(asset_name)],
         "{}".format(asset_name): ["__init__.py"],
+        "": ["main_cookiestream.py"]
     },
     packages=['{}/src'.format(asset_name), '{}/utils'.format(asset_name), '{}/configs'.format(asset_name),
               '{}'.format(asset_name)],
     package_dir={
         '{}/src'.format(asset_name): '{}/src'.format(asset_name),
         '{}/utils'.format(asset_name): './utils',
         '{}/configs'.format(asset_name): './configs',
-        '{}'.format(asset_name): '{}'.format(asset_name),
+        '{}'.format(asset_name): '{}'.format(asset_name)
     },
     # scripts=['cookiestream.sh'],
     entry_points={
         'console_scripts': [
-            'cookiestream = cookiestream.src.hello:hello_world',
+            'cookiestream = main_cookiestream:main',
         ]
     },
     # entry_points={'console_scripts': ['{} = main:main'.format(asset_name)]},
     # include_package_data=True,
     python_requires=yaml_asset_config[0]["asset_meta_information"]["python_required"]
 )
```

### Comparing `cookiestream-0.0.1.4/utils/util.py` & `cookiestream-0.0.1.5/utils/util.py`

 * *Files identical despite different names*

