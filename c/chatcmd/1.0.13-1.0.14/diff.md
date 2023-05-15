# Comparing `tmp/chatcmd-1.0.13.tar.gz` & `tmp/chatcmd-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.13.tar", last modified: Mon May 15 19:16:02 2023, max compression
+gzip compressed data, was "chatcmd-1.0.14.tar", last modified: Mon May 15 21:22:23 2023, max compression
```

## Comparing `chatcmd-1.0.13.tar` & `chatcmd-1.0.14.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 19:16:02.347171 chatcmd-1.0.13/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.13/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     4489 2023-05-15 19:16:02.346663 chatcmd-1.0.13/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3831 2023-05-15 19:12:25.000000 chatcmd-1.0.13/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 19:16:02.341853 chatcmd-1.0.13/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.13/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.13/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3518 2023-05-15 19:15:47.000000 chatcmd-1.0.13/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3772 2023-05-14 00:09:25.000000 chatcmd-1.0.13/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2783 2023-05-15 19:10:56.000000 chatcmd-1.0.13/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2602 2023-05-15 19:07:09.000000 chatcmd-1.0.13/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 19:16:02.345823 chatcmd-1.0.13/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     4489 2023-05-15 19:16:02.000000 chatcmd-1.0.13/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-15 19:16:02.000000 chatcmd-1.0.13/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 19:16:02.000000 chatcmd-1.0.13/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-15 19:16:02.000000 chatcmd-1.0.13/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       14 2023-05-15 19:16:02.000000 chatcmd-1.0.13/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-15 19:16:02.000000 chatcmd-1.0.13/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1823 2023-05-15 19:14:53.000000 chatcmd-1.0.13/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-15 19:16:02.347325 chatcmd-1.0.13/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-15 19:12:25.000000 chatcmd-1.0.13/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 21:22:23.794811 chatcmd-1.0.14/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.14/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     4489 2023-05-15 21:22:23.794550 chatcmd-1.0.14/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3831 2023-05-15 21:21:19.000000 chatcmd-1.0.14/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 21:22:23.791537 chatcmd-1.0.14/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.14/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.14/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3525 2023-05-15 21:21:19.000000 chatcmd-1.0.14/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3770 2023-05-15 21:19:30.000000 chatcmd-1.0.14/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     2783 2023-05-15 19:10:56.000000 chatcmd-1.0.14/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2602 2023-05-15 19:07:09.000000 chatcmd-1.0.14/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 21:22:23.794175 chatcmd-1.0.14/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     4489 2023-05-15 21:22:23.000000 chatcmd-1.0.14/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-15 21:22:23.000000 chatcmd-1.0.14/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 21:22:23.000000 chatcmd-1.0.14/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-15 21:22:23.000000 chatcmd-1.0.14/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2023-05-15 21:22:23.000000 chatcmd-1.0.14/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-15 21:22:23.000000 chatcmd-1.0.14/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1823 2023-05-15 21:21:19.000000 chatcmd-1.0.14/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-15 21:22:23.794894 chatcmd-1.0.14/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-15 21:21:19.000000 chatcmd-1.0.14/setup.py
```

### Comparing `chatcmd-1.0.13/LICENSE` & `chatcmd-1.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.13/PKG-INFO` & `chatcmd-1.0.14/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.13
+Version: 1.0.14
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
-    Using cached chatcmd-1.0.13-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.14-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.13
+    Successfully installed chatcmd-1.0.14
 
 ### Uninstall ###
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
```

### Comparing `chatcmd-1.0.13/README.md` & `chatcmd-1.0.14/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
     python3 -m pip install chatcmd
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.13-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.14-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.13
+    Successfully installed chatcmd-1.0.14
 
 ### Uninstall ###
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
```

### Comparing `chatcmd-1.0.13/chatcmd/api.py` & `chatcmd-1.0.14/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.13/chatcmd/chatcmd.py` & `chatcmd-1.0.14/chatcmd/chatcmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD \033[32m1.0.13\033[0m')
+            print('ChatCMD \033[32m1.0.14\033[0m')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
@@ -71,15 +71,15 @@
         elif args['--delete-cmd']:
             delete_cmd(conn, cursor)
         elif args['--delete-last-cmd']:
             delete_last_num_cmd(conn, cursor, args['--delete-last-cmd'])
         elif args['--clear-history']:
             clear_history(conn, cursor)
         elif args['--db-size']:
-            get_db_size()
+            get_db_size(db_path)
         elif args['--library-info']:
             library_info()
         else:
             prompt(conn, cursor, api_key)
 
         cursor.close()
         conn.close()
```

### Comparing `chatcmd-1.0.13/chatcmd/commands.py` & `chatcmd-1.0.14/chatcmd/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,16 @@
         conn.commit()
         print(color_text(f"\nAll command lookup has been cleared.",'green'))
         return True
     except sqlite3.Error as e:
         error_msg(f"Error 1017: Failed clearing history: {e}")
     return False
 
-def get_db_size():
-    file_size_bytes = os.path.getsize('data/db.sqlite')
+def get_db_size(db_path):
+    file_size_bytes = os.path.getsize(db_path)
     units = ['bytes', 'KB', 'MB', 'GB']
     size = file_size_bytes
     unit_index = 0
 
     while size >= 1024 and unit_index < len(units)-1:
         size /= 1024
         unit_index += 1
```

### Comparing `chatcmd-1.0.13/chatcmd/helpers.py` & `chatcmd-1.0.14/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.13/chatcmd/lookup.py` & `chatcmd-1.0.14/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.13/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.14/chatcmd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.13
+Version: 1.0.14
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
-    Using cached chatcmd-1.0.13-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.14-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.13
+    Successfully installed chatcmd-1.0.14
 
 ### Uninstall ###
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
```

### Comparing `chatcmd-1.0.13/pyproject.toml` & `chatcmd-1.0.14/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 65",
     "wheel >= 0.38",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.13"
+version = "1.0.14"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 [project.license]
 text = "MIT"
 readme = "README.md"
```

### Comparing `chatcmd-1.0.13/setup.py` & `chatcmd-1.0.14/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.13",
+    version="1.0.14",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     license="MIT",
     url="https://github.com/naifalshaye/chatcmd",
```

