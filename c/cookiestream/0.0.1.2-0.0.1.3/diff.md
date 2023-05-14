# Comparing `tmp/cookiestream-0.0.1.2.tar.gz` & `tmp/cookiestream-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiestream-0.0.1.2.tar", last modified: Sun May 14 21:37:23 2023, max compression
+gzip compressed data, was "cookiestream-0.0.1.3.tar", last modified: Sun May 14 23:44:05 2023, max compression
```

## Comparing `cookiestream-0.0.1.2.tar` & `cookiestream-0.0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/
--rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/LICENCE
--rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/README.md
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.602713 cookiestream-0.0.1.2/configs/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/configs/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      234 2023-05-11 21:21:05.000000 cookiestream-0.0.1.2/configs/base_config.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.602713 cookiestream-0.0.1.2/cookiestream/
--rw-rw-r--   0 zied      (1000) zied      (1000)       48 2023-05-11 21:26:51.000000 cookiestream-0.0.1.2/cookiestream/__init__.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/cookiestream/src/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/cookiestream/src/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      432 2023-05-11 22:08:24.000000 cookiestream-0.0.1.2/cookiestream/src/clone_template.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1978 2023-05-11 22:46:42.000000 cookiestream-0.0.1.2/cookiestream/src/make_rename.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     2906 2023-05-14 17:49:27.000000 cookiestream-0.0.1.2/cookiestream/src/modify_yaml_content.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     3781 2023-05-14 20:22:06.000000 cookiestream-0.0.1.2/cookiestream/src/stream.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/cookiestream.egg-info/
--rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)      494 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/SOURCES.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/dependency_links.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       29 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/requires.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       70 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/top_level.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       85 2023-05-14 21:35:49.000000 cookiestream-0.0.1.2/main.sh
--rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/setup.cfg
--rw-rw-r--   0 zied      (1000) zied      (1000)     2018 2023-05-14 21:35:49.000000 cookiestream-0.0.1.2/setup.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.602713 cookiestream-0.0.1.2/utils/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/utils/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/utils/util.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 23:44:05.093466 cookiestream-0.0.1.3/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-10 23:11:22.000000 cookiestream-0.0.1.3/LICENCE
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-14 23:44:05.093466 cookiestream-0.0.1.3/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-10 23:11:22.000000 cookiestream-0.0.1.3/README.md
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 23:44:05.089465 cookiestream-0.0.1.3/configs/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.3/configs/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      234 2023-05-11 21:21:05.000000 cookiestream-0.0.1.3/configs/base_config.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 23:44:05.093466 cookiestream-0.0.1.3/cookiestream/
+-rw-rw-r--   0 zied      (1000) zied      (1000)       92 2023-05-14 23:41:28.000000 cookiestream-0.0.1.3/cookiestream/__init__.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 23:44:05.093466 cookiestream-0.0.1.3/cookiestream/src/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.3/cookiestream/src/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      432 2023-05-11 22:08:24.000000 cookiestream-0.0.1.3/cookiestream/src/clone_template.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1978 2023-05-11 22:46:42.000000 cookiestream-0.0.1.3/cookiestream/src/make_rename.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2906 2023-05-14 17:49:27.000000 cookiestream-0.0.1.3/cookiestream/src/modify_yaml_content.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3781 2023-05-14 20:22:06.000000 cookiestream-0.0.1.3/cookiestream/src/stream.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 23:44:05.093466 cookiestream-0.0.1.3/cookiestream.egg-info/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-14 23:44:04.000000 cookiestream-0.0.1.3/cookiestream.egg-info/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)      525 2023-05-14 23:44:05.000000 cookiestream-0.0.1.3/cookiestream.egg-info/SOURCES.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-14 23:44:04.000000 cookiestream-0.0.1.3/cookiestream.egg-info/dependency_links.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       48 2023-05-14 23:44:04.000000 cookiestream-0.0.1.3/cookiestream.egg-info/entry_points.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       29 2023-05-14 23:44:04.000000 cookiestream-0.0.1.3/cookiestream.egg-info/requires.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       70 2023-05-14 23:44:04.000000 cookiestream-0.0.1.3/cookiestream.egg-info/top_level.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-14 23:44:05.093466 cookiestream-0.0.1.3/setup.cfg
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2140 2023-05-14 23:43:23.000000 cookiestream-0.0.1.3/setup.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 23:44:05.089465 cookiestream-0.0.1.3/utils/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.3/utils/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-10 23:11:22.000000 cookiestream-0.0.1.3/utils/util.py
```

### Comparing `cookiestream-0.0.1.2/LICENCE` & `cookiestream-0.0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.2/PKG-INFO` & `cookiestream-0.0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiestream
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Generate template based on template_vierge project
 Home-page: https://github.com/Proxia-ai/cookiestream
 Author: BEN OTHMANE Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/Proxia-ai/cookiestream/issues
 Keywords: Python pypi template,python
```

### Comparing `cookiestream-0.0.1.2/README.md` & `cookiestream-0.0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.2/cookiestream/src/make_rename.py` & `cookiestream-0.0.1.3/cookiestream/src/make_rename.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.2/cookiestream/src/modify_yaml_content.py` & `cookiestream-0.0.1.3/cookiestream/src/modify_yaml_content.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.2/cookiestream/src/stream.py` & `cookiestream-0.0.1.3/cookiestream/src/stream.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.2/cookiestream.egg-info/PKG-INFO` & `cookiestream-0.0.1.3/cookiestream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiestream
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Generate template based on template_vierge project
 Home-page: https://github.com/Proxia-ai/cookiestream
 Author: BEN OTHMANE Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/Proxia-ai/cookiestream/issues
 Keywords: Python pypi template,python
```

### Comparing `cookiestream-0.0.1.2/setup.py` & `cookiestream-0.0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,22 +27,27 @@
     keywords=yaml_asset_config[0]["asset_meta_information"]["keywords"],
     project_urls=yaml_asset_config[0]["asset_meta_information"]["project_urls"][0],
     install_requires=requirements,
     classifiers=yaml_asset_config[0]["asset_meta_information"]["classifiers"],
     license='BSD',
     package_data={
         "configs": ["config.ini", "{}_config.yaml".format(asset_name)],
-        "{}".format(asset_name): ["__init__.py"]
+        "{}".format(asset_name): ["__init__.py"],
     },
     packages=['{}/src'.format(asset_name), '{}/utils'.format(asset_name), '{}/configs'.format(asset_name),
               '{}'.format(asset_name)],
     package_dir={
         '{}/src'.format(asset_name): '{}/src'.format(asset_name),
         '{}/utils'.format(asset_name): './utils',
         '{}/configs'.format(asset_name): './configs',
-        '{}'.format(asset_name): '{}'.format(asset_name)
+        '{}'.format(asset_name): '{}'.format(asset_name),
+    },
+    # scripts=['cookiestream.sh'],
+    entry_points={
+        'console_scripts': [
+            'hello-world = src:hello_world',
+        ]
     },
-    scripts=['main.sh'],
     # entry_points={'console_scripts': ['{} = main:main'.format(asset_name)]},
     # include_package_data=True,
     python_requires=yaml_asset_config[0]["asset_meta_information"]["python_required"]
 )
```

### Comparing `cookiestream-0.0.1.2/utils/util.py` & `cookiestream-0.0.1.3/utils/util.py`

 * *Files identical despite different names*

