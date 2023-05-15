# Comparing `tmp/chatcmd-1.0.11.tar.gz` & `tmp/chatcmd-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.11.tar", last modified: Mon May 15 18:15:52 2023, max compression
+gzip compressed data, was "chatcmd-1.0.12.tar", last modified: Mon May 15 18:50:29 2023, max compression
```

## Comparing `chatcmd-1.0.11.tar` & `chatcmd-1.0.12.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 18:15:52.121472 chatcmd-1.0.11/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.11/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     4746 2023-05-15 18:15:52.121155 chatcmd-1.0.11/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     4088 2023-05-15 18:09:12.000000 chatcmd-1.0.11/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 18:15:52.117231 chatcmd-1.0.11/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.11/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.11/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3518 2023-05-15 18:09:12.000000 chatcmd-1.0.11/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3772 2023-05-14 00:09:25.000000 chatcmd-1.0.11/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2203 2023-05-15 15:59:49.000000 chatcmd-1.0.11/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2616 2023-05-15 15:45:22.000000 chatcmd-1.0.11/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 18:15:52.120712 chatcmd-1.0.11/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     4746 2023-05-15 18:15:52.000000 chatcmd-1.0.11/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-15 18:15:52.000000 chatcmd-1.0.11/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 18:15:52.000000 chatcmd-1.0.11/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-15 18:15:52.000000 chatcmd-1.0.11/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       24 2023-05-15 18:15:52.000000 chatcmd-1.0.11/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-15 18:15:52.000000 chatcmd-1.0.11/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1848 2023-05-15 18:09:12.000000 chatcmd-1.0.11/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-15 18:15:52.121569 chatcmd-1.0.11/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      577 2023-05-15 18:15:39.000000 chatcmd-1.0.11/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 18:50:29.828331 chatcmd-1.0.12/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.12/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     4746 2023-05-15 18:50:29.827992 chatcmd-1.0.12/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     4088 2023-05-15 18:49:59.000000 chatcmd-1.0.12/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 18:50:29.825332 chatcmd-1.0.12/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.12/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.12/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3518 2023-05-15 18:49:59.000000 chatcmd-1.0.12/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3772 2023-05-14 00:09:25.000000 chatcmd-1.0.12/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     2726 2023-05-15 18:47:46.000000 chatcmd-1.0.12/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2594 2023-05-15 18:49:02.000000 chatcmd-1.0.12/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 18:50:29.827626 chatcmd-1.0.12/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     4746 2023-05-15 18:50:29.000000 chatcmd-1.0.12/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-15 18:50:29.000000 chatcmd-1.0.12/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 18:50:29.000000 chatcmd-1.0.12/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-15 18:50:29.000000 chatcmd-1.0.12/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2023-05-15 18:50:29.000000 chatcmd-1.0.12/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-15 18:50:29.000000 chatcmd-1.0.12/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1823 2023-05-15 18:49:59.000000 chatcmd-1.0.12/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-15 18:50:29.828416 chatcmd-1.0.12/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-15 18:49:59.000000 chatcmd-1.0.12/setup.py
```

### Comparing `chatcmd-1.0.11/LICENSE` & `chatcmd-1.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.11/PKG-INFO` & `chatcmd-1.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.11
+Version: 1.0.12
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -41,17 +41,17 @@
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
     python3 -m pip install chatcmd
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.11-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.12-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.11
+    Successfully installed chatcmd-1.0.12
 
 ### Uninstall ###
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
```

### Comparing `chatcmd-1.0.11/README.md` & `chatcmd-1.0.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
     python3 -m pip install chatcmd
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.11-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.12-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.11
+    Successfully installed chatcmd-1.0.12
 
 ### Uninstall ###
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
```

### Comparing `chatcmd-1.0.11/chatcmd/api.py` & `chatcmd-1.0.12/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.11/chatcmd/chatcmd.py` & `chatcmd-1.0.12/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD \033[32m1.0.11\033[0m')
+            print('ChatCMD \033[32m1.0.12\033[0m')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.11/chatcmd/commands.py` & `chatcmd-1.0.12/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.11/chatcmd/helpers.py` & `chatcmd-1.0.12/chatcmd/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import re
 import inspect
+import subprocess
+import sys
 
 RESET = '\033[0m'
 
 def library_info():
     print(
     "----------------------------------------------------------------\n"
     "  \033[32mLibrary Name:\033[0m \033[33mChatCMD\033[0m\n"
@@ -65,10 +67,21 @@
         return False
     if len(api_key) != 51:
         return False
     if not re.match("^[a-zA-Z0-9-]+$", api_key):
         return False
     return True
 
+def copy_text(text):
+    try:
+        if sys.platform.startswith('win'):
+            subprocess.run(['clip'], input=text.strip().encode('utf-8'), check=True)
+        elif sys.platform.startswith('linux') or sys.platform.startswith('darwin'):
+            subprocess.run(['pbcopy'], input=text.strip().encode('utf-8'), check=True)
+        else:
+            raise error_msg('Unsupported operating system')
+    except subprocess.CalledProcessError as e:
+        print(f"Failed to copy text: {e}")
+
 def get_line_number():
     frame = inspect.currentframe().f_back
     return frame.f_lineno
```

### Comparing `chatcmd-1.0.11/chatcmd/lookup.py` & `chatcmd-1.0.12/chatcmd/lookup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .commands import *
-import pyperclip
 import openai
 
 def prompt(conn, cursor, api_key):
     print("""
 
      ######  ##     ##    ###    ########  ######  ##     ## ########
     ##    ## ##     ##   ## ##      ##    ##    ## ###   ### ##     ##
@@ -22,15 +21,15 @@
         prompt(conn, cursor, api_key)
     if prompt == 'exit':
         print(color_text('bye...', 'green'))
         exit()
     elif validateInput(prompt):
         command = lookup(prompt, api_key)
         if command is not None:
-            pyperclip.copy(command)
+            copy_text(command)
             command = clear_input(command)
 
             if command.find('there is no command') is True and command.find('There is no specific command') is True:
                 warning_msg('there is no command for this!')
             else:
                 history = add_cmd(conn, cursor, prompt, command.strip())
                 if history is False:
```

### Comparing `chatcmd-1.0.11/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.12/chatcmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.11
+Version: 1.0.12
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -41,17 +41,17 @@
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
     python3 -m pip install chatcmd
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.11-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.12-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.11
+    Successfully installed chatcmd-1.0.12
 
 ### Uninstall ###
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
```

### Comparing `chatcmd-1.0.11/pyproject.toml` & `chatcmd-1.0.12/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 65",
     "wheel >= 0.38",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.11"
+version = "1.0.12"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 [project.license]
 text = "MIT"
 readme = "README.md"
@@ -30,15 +30,14 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation",
 ]
 keywords = [
     "cli", "command", "command-line", "commandline", "terminal", "development","linux", "ai", "artificial-intelligence", "chatgpt", "lookup","open source","MIT"
 ]
 dependencies = [
-    "pyperclip >=1.8.2",
     "docopt >=0.6.2",
     "openai >=0.6.4",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/naifalshaye/chatcmd"
 "Documentation" = "https://github.com/naifalshaye/chatcmd/blob/master/README.md"
```

### Comparing `chatcmd-1.0.11/setup.py` & `chatcmd-1.0.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.11",
+    version="1.0.12",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     license="MIT",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
-        "pyperclip",
         "docopt",
         "openai",
     ],
 )
```

