# Comparing `tmp/chatcmd-1.0.7.tar.gz` & `tmp/chatcmd-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.7.tar", last modified: Mon May 15 16:03:13 2023, max compression
+gzip compressed data, was "chatcmd-1.0.8.tar", last modified: Mon May 15 17:08:04 2023, max compression
```

## Comparing `chatcmd-1.0.7.tar` & `chatcmd-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 16:03:13.493197 chatcmd-1.0.7/
--rw-r--r--   0 user       (501) staff       (20)      593 2023-05-15 16:03:13.492775 chatcmd-1.0.7/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3840 2023-05-13 22:50:37.000000 chatcmd-1.0.7/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 16:03:13.490285 chatcmd-1.0.7/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.7/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.7/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3517 2023-05-15 16:02:52.000000 chatcmd-1.0.7/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3772 2023-05-14 00:09:25.000000 chatcmd-1.0.7/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2203 2023-05-15 15:59:49.000000 chatcmd-1.0.7/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2616 2023-05-15 15:45:22.000000 chatcmd-1.0.7/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 16:03:13.492280 chatcmd-1.0.7/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      593 2023-05-15 16:03:13.000000 chatcmd-1.0.7/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      302 2023-05-15 16:03:13.000000 chatcmd-1.0.7/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 16:03:13.000000 chatcmd-1.0.7/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-15 16:03:13.000000 chatcmd-1.0.7/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-15 16:03:13.000000 chatcmd-1.0.7/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1846 2023-05-15 16:02:52.000000 chatcmd-1.0.7/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-15 16:03:13.493280 chatcmd-1.0.7/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      383 2023-05-15 16:02:52.000000 chatcmd-1.0.7/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 17:08:04.733611 chatcmd-1.0.8/
+-rw-r--r--   0 user       (501) staff       (20)     4571 2023-05-15 17:08:04.733361 chatcmd-1.0.8/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3936 2023-05-15 16:55:31.000000 chatcmd-1.0.8/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 17:08:04.730866 chatcmd-1.0.8/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.8/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.8/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3517 2023-05-15 16:55:31.000000 chatcmd-1.0.8/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3772 2023-05-14 00:09:25.000000 chatcmd-1.0.8/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     2203 2023-05-15 15:59:49.000000 chatcmd-1.0.8/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2616 2023-05-15 15:45:22.000000 chatcmd-1.0.8/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 17:08:04.732876 chatcmd-1.0.8/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     4571 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      302 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1846 2023-05-15 16:55:31.000000 chatcmd-1.0.8/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-15 17:08:04.733714 chatcmd-1.0.8/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      535 2023-05-15 17:07:34.000000 chatcmd-1.0.8/setup.py
```

### Comparing `chatcmd-1.0.7/README.md` & `chatcmd-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 - Display library information.
 
 ## Requirements
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
-### Using PIP ###
-    pip3 install chatcmd
-    
-### From Source ###
-    git clone https://github.com/naifalshaye/chatcmd.git
-    sudo python3 setup.py install
+    python3 -m pip install chatcmd
 
+    Collecting chatcmd
+    Using cached chatcmd-1.0.8-py3-none-any.whl (6.8 kB)
+    Installing collected packages: chatcmd
+    Successfully installed chatcmd-1.0.8
+
+### Uninstall ###
+    python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
 
 chatcmd [options]
```

### Comparing `chatcmd-1.0.7/chatcmd/api.py` & `chatcmd-1.0.8/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.7/chatcmd/chatcmd.py` & `chatcmd-1.0.8/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD \033[32m1.0.7\033[0m')
+            print('ChatCMD \033[32m1.0.8\033[0m')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.7/chatcmd/commands.py` & `chatcmd-1.0.8/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.7/chatcmd/helpers.py` & `chatcmd-1.0.8/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.7/chatcmd/lookup.py` & `chatcmd-1.0.8/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.7/pyproject.toml` & `chatcmd-1.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 65",
     "wheel >= 0.38"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.7"
+version = "1.0.8"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 [project.license]
 text = "MIT"
 readme = "README.md"
```

