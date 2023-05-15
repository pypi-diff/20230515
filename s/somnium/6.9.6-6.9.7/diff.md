# Comparing `tmp/somnium-6.9.6.tar.gz` & `tmp/somnium-6.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somnium-6.9.6.tar", last modified: Fri Apr 14 13:19:35 2023, max compression
+gzip compressed data, was "somnium-6.9.7.tar", last modified: Mon May 15 08:54:30 2023, max compression
```

## Comparing `somnium-6.9.6.tar` & `somnium-6.9.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-14 13:19:35.066928 somnium-6.9.6/
--rw-r--r--   0 kali      (1000) kali      (1000)       19 2022-07-25 10:16:20.000000 somnium-6.9.6/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)      879 2023-04-14 13:19:35.066928 somnium-6.9.6/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      358 2023-04-14 12:54:55.000000 somnium-6.9.6/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)      103 2022-07-25 10:16:08.000000 somnium-6.9.6/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)      651 2023-04-14 13:19:35.066928 somnium-6.9.6/setup.cfg
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-14 13:19:35.062928 somnium-6.9.6/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-14 13:19:35.066928 somnium-6.9.6/src/somnium/
--rw-r--r--   0 kali      (1000) kali      (1000)       30 2023-04-14 11:43:25.000000 somnium-6.9.6/src/somnium/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3062 2023-04-14 12:54:31.000000 somnium-6.9.6/src/somnium/__main__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-14 13:19:35.066928 somnium-6.9.6/src/somnium.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      879 2023-04-14 13:19:35.000000 somnium-6.9.6/src/somnium.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      230 2023-04-14 13:19:35.000000 somnium-6.9.6/src/somnium.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-14 13:19:35.000000 somnium-6.9.6/src/somnium.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-04-14 13:19:35.000000 somnium-6.9.6/src/somnium.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 08:54:30.234442 somnium-6.9.7/
+-rw-r--r--   0 kali      (1000) kali      (1000)       19 2022-07-25 10:16:20.000000 somnium-6.9.7/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-15 08:54:30.234442 somnium-6.9.7/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      412 2023-05-15 07:58:19.000000 somnium-6.9.7/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      103 2022-07-25 10:16:08.000000 somnium-6.9.7/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)      644 2023-05-15 08:54:30.234442 somnium-6.9.7/setup.cfg
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 08:54:30.206442 somnium-6.9.7/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 08:54:30.230442 somnium-6.9.7/src/somnium/
+-rw-r--r--   0 kali      (1000) kali      (1000)       30 2023-04-14 11:43:25.000000 somnium-6.9.7/src/somnium/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4826 2023-05-15 08:52:40.000000 somnium-6.9.7/src/somnium/__main__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 08:54:30.234442 somnium-6.9.7/src/somnium.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-15 08:54:30.000000 somnium-6.9.7/src/somnium.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      230 2023-05-15 08:54:30.000000 somnium-6.9.7/src/somnium.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-15 08:54:30.000000 somnium-6.9.7/src/somnium.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-05-15 08:54:30.000000 somnium-6.9.7/src/somnium.egg-info/top_level.txt
```

### Comparing `somnium-6.9.6/PKG-INFO` & `somnium-6.9.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: somnium
-Version: 6.9.6
+Version: 6.9.7
 Summary: Create beautiful artwork using the power of AI.
 Home-page: https://odium.us
 Author: odi
 Author-email: ivuxey@gmail.com
 License: MIT
-Project-URL: Bug Tracker, https://github.com/llawllet
+Project-URL: Bug Tracker, https://t.me/feelded
 Keywords: ai,stablediffusion,dream,somnium
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h1>Somnium</h1>
 Create beautiful artwork using the power of AI
 </div>
@@ -29,13 +29,16 @@
 ```
 
 <h2>Examples:</h2>
 
 ```python
 >>> from somnium import Somnium
 
+>>> # Get Styles UI
+>>> print(Somnium.StylesGraph())
+
 >>> # Get Styles
 >>> s = Somnium.Styles()
 
 >>> # Generate Artwork
 >>> print(Somnium.Generate('Girl', s[list(s.keys())[0]]))
 ```
```

### Comparing `somnium-6.9.6/setup.cfg` & `somnium-6.9.7/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [metadata]
 name = somnium
-version = 6.9.6
+version = 6.9.7
 author = odi
 author_email = ivuxey@gmail.com
 description = Create beautiful artwork using the power of AI.
 keywords = ai, stablediffusion, dream, somnium
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://odium.us
 license = MIT
 project_urls = 
-	Bug Tracker = https://github.com/llawllet
+	Bug Tracker = https://t.me/feelded
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.3
+python_requires = >=3.5
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `somnium-6.9.6/src/somnium.egg-info/PKG-INFO` & `somnium-6.9.7/src/somnium.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: somnium
-Version: 6.9.6
+Version: 6.9.7
 Summary: Create beautiful artwork using the power of AI.
 Home-page: https://odium.us
 Author: odi
 Author-email: ivuxey@gmail.com
 License: MIT
-Project-URL: Bug Tracker, https://github.com/llawllet
+Project-URL: Bug Tracker, https://t.me/feelded
 Keywords: ai,stablediffusion,dream,somnium
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h1>Somnium</h1>
 Create beautiful artwork using the power of AI
 </div>
@@ -29,13 +29,16 @@
 ```
 
 <h2>Examples:</h2>
 
 ```python
 >>> from somnium import Somnium
 
+>>> # Get Styles UI
+>>> print(Somnium.StylesGraph())
+
 >>> # Get Styles
 >>> s = Somnium.Styles()
 
 >>> # Generate Artwork
 >>> print(Somnium.Generate('Girl', s[list(s.keys())[0]]))
 ```
```

