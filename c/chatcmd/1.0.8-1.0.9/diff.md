# Comparing `tmp/chatcmd-1.0.8.tar.gz` & `tmp/chatcmd-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.8.tar", last modified: Mon May 15 17:08:04 2023, max compression
+gzip compressed data, was "chatcmd-1.0.9.tar", last modified: Mon May 15 17:22:10 2023, max compression
```

## Comparing `chatcmd-1.0.8.tar` & `chatcmd-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 17:08:04.733611 chatcmd-1.0.8/
--rw-r--r--   0 user       (501) staff       (20)     4571 2023-05-15 17:08:04.733361 chatcmd-1.0.8/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3936 2023-05-15 16:55:31.000000 chatcmd-1.0.8/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 17:08:04.730866 chatcmd-1.0.8/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.8/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.8/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3517 2023-05-15 16:55:31.000000 chatcmd-1.0.8/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3772 2023-05-14 00:09:25.000000 chatcmd-1.0.8/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2203 2023-05-15 15:59:49.000000 chatcmd-1.0.8/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2616 2023-05-15 15:45:22.000000 chatcmd-1.0.8/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 17:08:04.732876 chatcmd-1.0.8/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     4571 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      302 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-15 17:08:04.000000 chatcmd-1.0.8/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1846 2023-05-15 16:55:31.000000 chatcmd-1.0.8/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-15 17:08:04.733714 chatcmd-1.0.8/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      535 2023-05-15 17:07:34.000000 chatcmd-1.0.8/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 17:22:10.733036 chatcmd-1.0.9/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     4743 2023-05-15 17:22:10.732692 chatcmd-1.0.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     4086 2023-05-15 17:19:19.000000 chatcmd-1.0.9/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 17:22:10.729979 chatcmd-1.0.9/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.9/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.9/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3517 2023-05-15 17:19:19.000000 chatcmd-1.0.9/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3772 2023-05-14 00:09:25.000000 chatcmd-1.0.9/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     2203 2023-05-15 15:59:49.000000 chatcmd-1.0.9/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2616 2023-05-15 15:45:22.000000 chatcmd-1.0.9/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 17:22:10.732161 chatcmd-1.0.9/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     4743 2023-05-15 17:22:10.000000 chatcmd-1.0.9/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      310 2023-05-15 17:22:10.000000 chatcmd-1.0.9/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 17:22:10.000000 chatcmd-1.0.9/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-15 17:22:10.000000 chatcmd-1.0.9/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-15 17:22:10.000000 chatcmd-1.0.9/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1846 2023-05-15 17:19:19.000000 chatcmd-1.0.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-15 17:22:10.733140 chatcmd-1.0.9/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      535 2023-05-15 17:19:19.000000 chatcmd-1.0.9/setup.py
```

### Comparing `chatcmd-1.0.8/PKG-INFO` & `chatcmd-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.8
+Version: 1.0.9
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
 Project-URL: Repository, https://github.com/naifalshaye/chatcmd.git
 Project-URL: Bug Tracker, https://github.com/naifalshaye/chatcmd/issues
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ChatCMD #
 #### **ChatCMD** is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input. ####
 
 #### Boost Your Productivity, ***Say Goodbye*** to Manual Searches ####
 
 ## Features
@@ -40,17 +41,17 @@
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
     python3 -m pip install chatcmd
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.8-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.9-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.8
+    Successfully installed chatcmd-1.0.9
 
 ### Uninstall ###
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
@@ -71,21 +72,21 @@
   -v, --version                     display ChatCMD version.
   -i, --library-info                display library information.
 
 ```
 
 ## Screenshots
 ### Help screen: ###
-<img src="chatcmd/images/help.png" alt="Help Screen" style="width:550px;"/>
+<img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/help.png" alt="Help Screen" style="width:550px;"/>
 
 ### Library Info: ###
-<img src="chatcmd/images/library-info.png" alt="Lookup Screen" style="width:500px;"/>
+<img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/library-info.png" alt="Lookup Screen" style="width:500px;"/>
 
 ### Command Lookup screen: ###
-<img src="chatcmd/images/lookup.png" alt="Lookup Screen" style="width:500px;"/>
+<img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/lookup.png" alt="Lookup Screen" style="width:500px;"/>
 
 ## Error Codes
 Include an exception message for each error if occurs.
 
 | Code |                     Description                     |
 |------|:---------------------------------------------------:|
 | 1001 |                  General exception                  |
```

### Comparing `chatcmd-1.0.8/README.md` & `chatcmd-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
     python3 -m pip install chatcmd
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.8-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.9-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.8
+    Successfully installed chatcmd-1.0.9
 
 ### Uninstall ###
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
@@ -57,21 +57,21 @@
   -v, --version                     display ChatCMD version.
   -i, --library-info                display library information.
 
 ```
 
 ## Screenshots
 ### Help screen: ###
-<img src="chatcmd/images/help.png" alt="Help Screen" style="width:550px;"/>
+<img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/help.png" alt="Help Screen" style="width:550px;"/>
 
 ### Library Info: ###
-<img src="chatcmd/images/library-info.png" alt="Lookup Screen" style="width:500px;"/>
+<img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/library-info.png" alt="Lookup Screen" style="width:500px;"/>
 
 ### Command Lookup screen: ###
-<img src="chatcmd/images/lookup.png" alt="Lookup Screen" style="width:500px;"/>
+<img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/lookup.png" alt="Lookup Screen" style="width:500px;"/>
 
 ## Error Codes
 Include an exception message for each error if occurs.
 
 | Code |                     Description                     |
 |------|:---------------------------------------------------:|
 | 1001 |                  General exception                  |
```

### Comparing `chatcmd-1.0.8/chatcmd/api.py` & `chatcmd-1.0.9/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.8/chatcmd/chatcmd.py` & `chatcmd-1.0.9/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD \033[32m1.0.8\033[0m')
+            print('ChatCMD \033[32m1.0.9\033[0m')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.8/chatcmd/commands.py` & `chatcmd-1.0.9/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.8/chatcmd/helpers.py` & `chatcmd-1.0.9/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.8/chatcmd/lookup.py` & `chatcmd-1.0.9/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.8/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.9/chatcmd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.8
+Version: 1.0.9
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
 Project-URL: Repository, https://github.com/naifalshaye/chatcmd.git
 Project-URL: Bug Tracker, https://github.com/naifalshaye/chatcmd/issues
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ChatCMD #
 #### **ChatCMD** is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input. ####
 
 #### Boost Your Productivity, ***Say Goodbye*** to Manual Searches ####
 
 ## Features
@@ -40,17 +41,17 @@
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
     python3 -m pip install chatcmd
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.8-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.9-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.8
+    Successfully installed chatcmd-1.0.9
 
 ### Uninstall ###
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
@@ -71,21 +72,21 @@
   -v, --version                     display ChatCMD version.
   -i, --library-info                display library information.
 
 ```
 
 ## Screenshots
 ### Help screen: ###
-<img src="chatcmd/images/help.png" alt="Help Screen" style="width:550px;"/>
+<img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/help.png" alt="Help Screen" style="width:550px;"/>
 
 ### Library Info: ###
-<img src="chatcmd/images/library-info.png" alt="Lookup Screen" style="width:500px;"/>
+<img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/library-info.png" alt="Lookup Screen" style="width:500px;"/>
 
 ### Command Lookup screen: ###
-<img src="chatcmd/images/lookup.png" alt="Lookup Screen" style="width:500px;"/>
+<img src="https://github.com/naifalshaye/chatcmd/raw/master/chatcmd/images/lookup.png" alt="Lookup Screen" style="width:500px;"/>
 
 ## Error Codes
 Include an exception message for each error if occurs.
 
 | Code |                     Description                     |
 |------|:---------------------------------------------------:|
 | 1001 |                  General exception                  |
```

### Comparing `chatcmd-1.0.8/pyproject.toml` & `chatcmd-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 65",
     "wheel >= 0.38"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.8"
+version = "1.0.9"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 [project.license]
 text = "MIT"
 readme = "README.md"
```

### Comparing `chatcmd-1.0.8/setup.py` & `chatcmd-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.8",
+    version="1.0.9",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     license="MIT",
     url="https://github.com/naifalshaye/chatcmd",
```

