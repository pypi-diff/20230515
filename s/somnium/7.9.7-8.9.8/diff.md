# Comparing `tmp/somnium-7.9.7.tar.gz` & `tmp/somnium-8.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somnium-7.9.7.tar", last modified: Mon May 15 10:17:46 2023, max compression
+gzip compressed data, was "somnium-8.9.8.tar", last modified: Mon May 15 10:49:37 2023, max compression
```

## Comparing `somnium-7.9.7.tar` & `somnium-8.9.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:17:46.613902 somnium-7.9.7/
--rw-r--r--   0 kali      (1000) kali      (1000)       19 2022-07-25 10:16:20.000000 somnium-7.9.7/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-15 10:17:46.613902 somnium-7.9.7/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      412 2023-05-15 07:58:19.000000 somnium-7.9.7/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)      103 2022-07-25 10:16:08.000000 somnium-7.9.7/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)      687 2023-05-15 10:17:46.617902 somnium-7.9.7/setup.cfg
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:17:46.609902 somnium-7.9.7/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:17:46.609902 somnium-7.9.7/src/somnium/
--rw-r--r--   0 kali      (1000) kali      (1000)       30 2023-04-14 11:43:25.000000 somnium-7.9.7/src/somnium/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4972 2023-05-15 10:16:13.000000 somnium-7.9.7/src/somnium/__main__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:17:46.613902 somnium-7.9.7/src/somnium.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-15 10:17:46.000000 somnium-7.9.7/src/somnium.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      264 2023-05-15 10:17:46.000000 somnium-7.9.7/src/somnium.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-15 10:17:46.000000 somnium-7.9.7/src/somnium.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       22 2023-05-15 10:17:46.000000 somnium-7.9.7/src/somnium.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-05-15 10:17:46.000000 somnium-7.9.7/src/somnium.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:49:37.173350 somnium-8.9.8/
+-rw-r--r--   0 kali      (1000) kali      (1000)       19 2022-07-25 10:16:20.000000 somnium-8.9.8/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-15 10:49:37.173350 somnium-8.9.8/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      412 2023-05-15 07:58:19.000000 somnium-8.9.8/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      103 2022-07-25 10:16:08.000000 somnium-8.9.8/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)      687 2023-05-15 10:49:37.173350 somnium-8.9.8/setup.cfg
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:49:37.169350 somnium-8.9.8/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:49:37.173350 somnium-8.9.8/src/somnium/
+-rw-r--r--   0 kali      (1000) kali      (1000)       30 2023-04-14 11:43:25.000000 somnium-8.9.8/src/somnium/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4909 2023-05-15 10:48:07.000000 somnium-8.9.8/src/somnium/__main__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:49:37.173350 somnium-8.9.8/src/somnium.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      264 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       22 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/top_level.txt
```

### Comparing `somnium-7.9.7/PKG-INFO` & `somnium-8.9.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somnium
-Version: 7.9.7
+Version: 8.9.8
 Summary: Create beautiful artwork using the power of AI.
 Home-page: https://odium.us
 Author: odi
 Author-email: ivuxey@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://t.me/feelded
 Keywords: ai,stablediffusion,dream,somnium
```

### Comparing `somnium-7.9.7/setup.cfg` & `somnium-8.9.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = somnium
-version = 7.9.7
+version = 8.9.8
 author = odi
 author_email = ivuxey@gmail.com
 description = Create beautiful artwork using the power of AI.
 keywords = ai, stablediffusion, dream, somnium
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://odium.us
```

### Comparing `somnium-7.9.7/src/somnium/__main__.py` & `somnium-8.9.8/src/somnium/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,18 +113,18 @@
         gen_response = requests.post('https://paint.api.wombo.ai/api/v2/tasks', headers=headers, data=json.dumps(data))
 
         try:
             image_id = gen_response.json()["id"]
             for i in range(10):
                 response = requests.get(f'https://paint.api.wombo.ai/api/v2/tasks/{image_id}', headers=headers)
                 if response.json()['state'] == "failed":
-                    return 'https://i.ibb.co/S3dfVV1/nsfw.png'
+                    return None
                     break
                 time.sleep(3)
                 try:
                     img = response.json()["result"]["final"]
                     return img
                     break
                 except:
                     continue
         except Exception as e:
-            return 'https://i.ibb.co/SsTjP50/error.png'
+            return None
```

### Comparing `somnium-7.9.7/src/somnium.egg-info/PKG-INFO` & `somnium-8.9.8/src/somnium.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somnium
-Version: 7.9.7
+Version: 8.9.8
 Summary: Create beautiful artwork using the power of AI.
 Home-page: https://odium.us
 Author: odi
 Author-email: ivuxey@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://t.me/feelded
 Keywords: ai,stablediffusion,dream,somnium
```

