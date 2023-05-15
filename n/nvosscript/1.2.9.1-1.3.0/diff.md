# Comparing `tmp/nvosscript-1.2.9.1.tar.gz` & `tmp/nvosscript-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.2.9.1.tar", last modified: Thu May 11 02:24:08 2023, max compression
+gzip compressed data, was "nvosscript-1.3.0.tar", last modified: Mon May 15 02:50:32 2023, max compression
```

## Comparing `nvosscript-1.2.9.1.tar` & `nvosscript-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.809830 nvosscript-1.2.9.1/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.2.9.1/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-11 02:24:08.809695 nvosscript-1.2.9.1/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.2.9.1/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.807087 nvosscript-1.2.9.1/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.2.9.1/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    13051 2023-05-10 10:01:20.000000 nvosscript-1.2.9.1/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.2.9.1/nvos/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-10 10:01:27.000000 nvosscript-1.2.9.1/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4796 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/nvos/run.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/nvos/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.808077 nvosscript-1.2.9.1/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-11 02:24:08.809865 nvosscript-1.2.9.1/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      808 2023-05-11 02:23:52.000000 nvosscript-1.2.9.1/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.808651 nvosscript-1.2.9.1/skyeye/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/skyeye/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/skyeye/datahandler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/skyeye/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/skyeye/skyeyecommand.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.809031 nvosscript-1.2.9.1/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.2.9.1/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/start/commonUtil.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4532 2023-05-11 02:23:52.000000 nvosscript-1.2.9.1/start/main.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.805051 nvosscript-1.2.9.1/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.809256 nvosscript-1.2.9.1/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.2.9.1/venv/bin/activate_this.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.809499 nvosscript-1.2.9.1/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1273 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.761165 nvosscript-1.3.0/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.0/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-05-15 02:50:32.760947 nvosscript-1.3.0/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.0/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.757087 nvosscript-1.3.0/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.0/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    13051 2023-05-12 07:47:19.000000 nvosscript-1.3.0/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.3.0/nvos/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-12 07:47:19.000000 nvosscript-1.3.0/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     6172 2023-05-11 08:47:40.000000 nvosscript-1.3.0/nvos/run.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.3.0/nvos/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.758389 nvosscript-1.3.0/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-15 02:50:32.761226 nvosscript-1.3.0/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-05-12 07:47:19.000000 nvosscript-1.3.0/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.759223 nvosscript-1.3.0/skyeye/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.0/skyeye/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.3.0/skyeye/datahandler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.3.0/skyeye/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.3.0/skyeye/skyeyecommand.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.759947 nvosscript-1.3.0/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.0/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.3.0/start/commonUtil.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4525 2023-05-12 07:47:19.000000 nvosscript-1.3.0/start/main.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.752771 nvosscript-1.3.0/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.760269 nvosscript-1.3.0/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.0/venv/bin/activate_this.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.760612 nvosscript-1.3.0/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.0/win/win_auto_script.py
```

### Comparing `nvosscript-1.2.9.1/LICENSE` & `nvosscript-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.9.1/nvos/file.py` & `nvosscript-1.3.0/nvos/file.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.9.1/nvos/login.py` & `nvosscript-1.3.0/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.9.1/nvos/remote.py` & `nvosscript-1.3.0/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.9.1/nvos/utils.py` & `nvosscript-1.3.0/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.9.1/setup.py` & `nvosscript-1.3.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.2.9.01',
+    version='1.3.0',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.2.9.1/skyeye/datahandler.py` & `nvosscript-1.3.0/skyeye/datahandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.9.1/skyeye/remote.py` & `nvosscript-1.3.0/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.9.1/start/main.py` & `nvosscript-1.3.0/start/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     subparsers = parser.add_subparsers(title="NDTC Script Command", dest='subcommand')
     subparsers.add_parser('login', help='[NVOS]The login command is the first command that must be executed.')
 
     subparsers.add_parser('init', help='[NVOS]The Init command is used to initialize the workspace. Please execute the '
                                        'command in your workspace directory')
     asyncparse = subparsers.add_parser('async',
                                        help='[NVOS]The async command automatically synchronizes the data you modify from the cloud and to push addtion file to cloud')
-    asyncparse.add_argument('-t', '--type', choices=['pull', 'push', 'all'],
+    asyncparse.add_argument('-m', '--model', choices=['start', 'stop'],
                             help='switch you want async model,The currently owned modes are pull and push.')
     subparsers.add_parser('pull', help='[NVOS]The pull command pulls the data you modify from the cloud')
     subparsers.add_parser('push', help='[NVOS]The push command is used upload local new files or folders to the cloud')
     subparsers.add_parser('version', help='[NVOS]The version command will tell you this script really version')
     subparsers.add_parser('path',
                           help='[NVOS]The path command will return windows service register script path, so you can '
                                'install this script for windows like async command.You need execute "pythonw '
@@ -48,21 +48,21 @@
         username = input("email：")
         password = getpass.getpass("password：")
         status = login.login_user_check(username, password)
         print(status)
     elif args.subcommand == "init":
         run.command_init()
     elif args.subcommand == "async":
-        run.command_async(args.type)
+        run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.2.9.01")
+        print("1.3.0")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.2.9.1/venv/bin/activate_this.py` & `nvosscript-1.3.0/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.9.1/win/win_auto_script.py` & `nvosscript-1.3.0/win/win_auto_script.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 if __name__ == '__main__':
     logger.info("service start success......")
     with concurrent.futures.ThreadPoolExecutor(max_workers=5) as executor:
         while True:
             logger.info("start execute next task........")
             try:
-                if os.path.exists(os.path.expanduser(os.path.join("~", "workspace"))):
-                    with open(os.path.expanduser(os.path.join("~", "workspace")), "r") as f:
+                if os.path.exists(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace"))):
+                    with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace")), "r") as f:
                         all_workspace_path = json.loads(f.readline().strip())
                     for temp in all_workspace_path.keys():
                         logger.info("command_async current run workspace is " + temp)
                         executor.submit(execute_async, temp)
             except Exception as e:
                 logger.exception("An exception occurred")
             time.sleep(10)
```

