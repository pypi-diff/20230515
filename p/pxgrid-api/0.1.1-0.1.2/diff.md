# Comparing `tmp/pxgrid-api-0.1.1.tar.gz` & `tmp/pxgrid-api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxgrid-api-0.1.1.tar", last modified: Sat May 13 02:09:28 2023, max compression
+gzip compressed data, was "pxgrid-api-0.1.2.tar", last modified: Mon May 15 19:49:05 2023, max compression
```

## Comparing `pxgrid-api-0.1.1.tar` & `pxgrid-api-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-13 02:09:28.159716 pxgrid-api-0.1.1/
--rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.1.1/LICENSE
--rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.1.1/MANIFEST.in
--rw-r--r--   0 vibobrov   (503) staff       (20)    28907 2023-05-13 02:09:28.158959 pxgrid-api-0.1.1/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)    15464 2023-05-13 01:57:49.000000 pxgrid-api-0.1.1/README.md
--rw-r--r--   0 vibobrov   (503) staff       (20)      712 2023-05-13 02:07:51.000000 pxgrid-api-0.1.1/pyproject.toml
--rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-13 02:09:28.159924 pxgrid-api-0.1.1/setup.cfg
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-13 02:09:28.145964 pxgrid-api-0.1.1/src/
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-13 02:09:28.151667 pxgrid-api-0.1.1/src/pxapi/
--rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-13 02:08:19.000000 pxgrid-api-0.1.1/src/pxapi/__init__.py
--rwx------   0 vibobrov   (503) staff       (20)    20359 2023-05-13 01:27:59.000000 pxgrid-api-0.1.1/src/pxapi/__main__.py
--rw-r--r--   0 vibobrov   (503) staff       (20)    30241 2023-05-13 01:24:16.000000 pxgrid-api-0.1.1/src/pxapi/pxapi.py
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-13 02:09:28.157721 pxgrid-api-0.1.1/src/pxgrid_api.egg-info/
--rw-r--r--   0 vibobrov   (503) staff       (20)    28907 2023-05-13 02:09:28.000000 pxgrid-api-0.1.1/src/pxgrid_api.egg-info/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)      337 2023-05-13 02:09:28.000000 pxgrid-api-0.1.1/src/pxgrid_api.egg-info/SOURCES.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-13 02:09:28.000000 pxgrid-api-0.1.1/src/pxgrid_api.egg-info/dependency_links.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-13 02:09:28.000000 pxgrid-api-0.1.1/src/pxgrid_api.egg-info/entry_points.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-13 02:09:28.000000 pxgrid-api-0.1.1/src/pxgrid_api.egg-info/requires.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)        6 2023-05-13 02:09:28.000000 pxgrid-api-0.1.1/src/pxgrid_api.egg-info/top_level.txt
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-15 19:49:05.142566 pxgrid-api-0.1.2/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.1.2/LICENSE
+-rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.1.2/MANIFEST.in
+-rw-r--r--   0 vibobrov   (503) staff       (20)    28994 2023-05-15 19:49:05.142141 pxgrid-api-0.1.2/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)    15551 2023-05-15 19:47:44.000000 pxgrid-api-0.1.2/README.md
+-rw-r--r--   0 vibobrov   (503) staff       (20)      712 2023-05-15 19:47:31.000000 pxgrid-api-0.1.2/pyproject.toml
+-rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-15 19:49:05.142699 pxgrid-api-0.1.2/setup.cfg
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-15 19:49:05.131290 pxgrid-api-0.1.2/src/
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-15 19:49:05.136026 pxgrid-api-0.1.2/src/pxapi/
+-rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-15 19:47:35.000000 pxgrid-api-0.1.2/src/pxapi/__init__.py
+-rwx------   0 vibobrov   (503) staff       (20)    20359 2023-05-13 01:27:59.000000 pxgrid-api-0.1.2/src/pxapi/__main__.py
+-rw-r--r--   0 vibobrov   (503) staff       (20)    30241 2023-05-13 01:24:16.000000 pxgrid-api-0.1.2/src/pxapi/pxapi.py
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-15 19:49:05.141173 pxgrid-api-0.1.2/src/pxgrid_api.egg-info/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    28994 2023-05-15 19:49:05.000000 pxgrid-api-0.1.2/src/pxgrid_api.egg-info/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)      337 2023-05-15 19:49:05.000000 pxgrid-api-0.1.2/src/pxgrid_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-15 19:49:05.000000 pxgrid-api-0.1.2/src/pxgrid_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-15 19:49:05.000000 pxgrid-api-0.1.2/src/pxgrid_api.egg-info/entry_points.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-15 19:49:05.000000 pxgrid-api-0.1.2/src/pxgrid_api.egg-info/requires.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)        6 2023-05-15 19:49:05.000000 pxgrid-api-0.1.2/src/pxgrid_api.egg-info/top_level.txt
```

### Comparing `pxgrid-api-0.1.1/LICENSE` & `pxgrid-api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.1.1/PKG-INFO` & `pxgrid-api-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: pxGrid API library and command line tool
 Author-email: Viktor Bobrov <vibobrov@cisco.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -237,25 +237,22 @@
 
 ## Additonal reference material:
 * https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki
 * https://developer.cisco.com/docs/pxgrid/
 * https://developer.cisco.com/codeexchange/github/repo/cisco-pxgrid/python-advanced-examples
 
 
-# pxAPI Library
+# PXAPI Library
 
 This library simplifies interaction with ISE pxGrid
 
 
 ## Installation
 
 ```
-# Optionally create virtual env
-python3 -m venv env
-
 # Install the module
 pip install pxgrid-api
 ```
 
 ## Usage
 
 pxapi.py file has comments throughout describing all functions.  
@@ -346,15 +343,23 @@
 api=PXAPI('pxgridnode.example.com','client-name','client.cer','client.key','root.cer')
 api.topic_subscribe("com.cisco.ise.session","sessionTopic",on_message)
 
 ```
 
 # pxshell
 
-This utility is an interactive wrapper for pxAPI library. It allows interaction with pxGrid using simple CLI interface.
+This utility is an interactive wrapper for PXAPI library. It allows interaction with pxGrid using simple CLI interface.
+
+## Installation
+This cli utility is installed along with PXAPI with the same command.
+
+```
+# Install the module
+pip install pxgrid-api
+```
 
 ## Usage
 
 All commands are document and help can be retrived using help &lt;command&gt;
 ```
 $ pxshell
 pxshell> help
```

### Comparing `pxgrid-api-0.1.1/README.md` & `pxgrid-api-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,22 @@
 
 ## Additonal reference material:
 * https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki
 * https://developer.cisco.com/docs/pxgrid/
 * https://developer.cisco.com/codeexchange/github/repo/cisco-pxgrid/python-advanced-examples
 
 
-# pxAPI Library
+# PXAPI Library
 
 This library simplifies interaction with ISE pxGrid
 
 
 ## Installation
 
 ```
-# Optionally create virtual env
-python3 -m venv env
-
 # Install the module
 pip install pxgrid-api
 ```
 
 ## Usage
 
 pxapi.py file has comments throughout describing all functions.  
@@ -130,15 +127,23 @@
 api=PXAPI('pxgridnode.example.com','client-name','client.cer','client.key','root.cer')
 api.topic_subscribe("com.cisco.ise.session","sessionTopic",on_message)
 
 ```
 
 # pxshell
 
-This utility is an interactive wrapper for pxAPI library. It allows interaction with pxGrid using simple CLI interface.
+This utility is an interactive wrapper for PXAPI library. It allows interaction with pxGrid using simple CLI interface.
+
+## Installation
+This cli utility is installed along with PXAPI with the same command.
+
+```
+# Install the module
+pip install pxgrid-api
+```
 
 ## Usage
 
 All commands are document and help can be retrived using help &lt;command&gt;
 ```
 $ pxshell
 pxshell> help
```

### Comparing `pxgrid-api-0.1.1/pyproject.toml` & `pxgrid-api-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["setuptools","wheel"]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pxgrid-api"
-version = "0.1.1"
+version = "0.1.2"
 description = "pxGrid API library and command line tool"
 readme = "README.md"
 authors = [{ name = "Viktor Bobrov", email = "vibobrov@cisco.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `pxgrid-api-0.1.1/src/pxapi/__main__.py` & `pxgrid-api-0.1.2/src/pxapi/__main__.py`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.1.1/src/pxapi/pxapi.py` & `pxgrid-api-0.1.2/src/pxapi/pxapi.py`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.1.1/src/pxgrid_api.egg-info/PKG-INFO` & `pxgrid-api-0.1.2/src/pxgrid_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: pxGrid API library and command line tool
 Author-email: Viktor Bobrov <vibobrov@cisco.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -237,25 +237,22 @@
 
 ## Additonal reference material:
 * https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki
 * https://developer.cisco.com/docs/pxgrid/
 * https://developer.cisco.com/codeexchange/github/repo/cisco-pxgrid/python-advanced-examples
 
 
-# pxAPI Library
+# PXAPI Library
 
 This library simplifies interaction with ISE pxGrid
 
 
 ## Installation
 
 ```
-# Optionally create virtual env
-python3 -m venv env
-
 # Install the module
 pip install pxgrid-api
 ```
 
 ## Usage
 
 pxapi.py file has comments throughout describing all functions.  
@@ -346,15 +343,23 @@
 api=PXAPI('pxgridnode.example.com','client-name','client.cer','client.key','root.cer')
 api.topic_subscribe("com.cisco.ise.session","sessionTopic",on_message)
 
 ```
 
 # pxshell
 
-This utility is an interactive wrapper for pxAPI library. It allows interaction with pxGrid using simple CLI interface.
+This utility is an interactive wrapper for PXAPI library. It allows interaction with pxGrid using simple CLI interface.
+
+## Installation
+This cli utility is installed along with PXAPI with the same command.
+
+```
+# Install the module
+pip install pxgrid-api
+```
 
 ## Usage
 
 All commands are document and help can be retrived using help &lt;command&gt;
 ```
 $ pxshell
 pxshell> help
```

