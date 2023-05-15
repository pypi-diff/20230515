# Comparing `tmp/botsh-0.1.6.tar.gz` & `tmp/botsh-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botsh-0.1.6.tar", last modified: Tue Apr 18 16:38:16 2023, max compression
+gzip compressed data, was "botsh-0.1.7.tar", last modified: Mon May 15 14:39:55 2023, max compression
```

## Comparing `botsh-0.1.6.tar` & `botsh-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.532794 botsh-0.1.6/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2023-04-18 14:41:00.000000 botsh-0.1.6/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-04-18 14:41:00.000000 botsh-0.1.6/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4562 2023-04-18 16:38:16.532794 botsh-0.1.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      234 2023-04-18 16:17:51.000000 botsh-0.1.6/Pipfile
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    64876 2023-04-18 14:41:00.000000 botsh-0.1.6/Pipfile.lock
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3901 2023-04-18 14:41:00.000000 botsh-0.1.6/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-18 16:38:16.532794 botsh-0.1.6/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1597 2023-04-18 16:37:45.000000 botsh-0.1.6/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.528794 botsh-0.1.6/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.528794 botsh-0.1.6/src/botsh/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-18 14:41:00.000000 botsh-0.1.6/src/botsh/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3601 2023-04-18 15:21:53.000000 botsh-0.1.6/src/botsh/docker_exec.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      317 2023-04-18 14:41:00.000000 botsh-0.1.6/src/botsh/history.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1581 2023-04-18 16:30:29.000000 botsh-0.1.6/src/botsh/llm.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2023-04-18 14:41:00.000000 botsh-0.1.6/src/botsh/logging.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2718 2023-04-18 14:41:00.000000 botsh-0.1.6/src/botsh/main.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1204 2023-04-18 16:28:51.000000 botsh-0.1.6/src/botsh/prompt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2189 2023-04-18 16:37:34.000000 botsh-0.1.6/src/botsh/task_driver.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.532794 botsh-0.1.6/src/botsh/templates/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1099 2023-04-18 16:29:47.000000 botsh-0.1.6/src/botsh/templates/prompt.jinja2
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.532794 botsh-0.1.6/src/botsh.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4562 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      462 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      881 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/top_level.txt
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-05-15 14:39:55.787879 botsh-0.1.7/
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1074 2023-04-10 17:14:36.000000 botsh-0.1.7/LICENSE
+-rw-r--r--   0 paulbutler   (501) staff       (20)       54 2023-04-10 14:28:50.000000 botsh-0.1.7/MANIFEST.in
+-rw-r--r--   0 paulbutler   (501) staff       (20)     4962 2023-05-15 14:39:55.787743 botsh-0.1.7/PKG-INFO
+-rw-r--r--   0 paulbutler   (501) staff       (20)      234 2023-04-10 14:12:58.000000 botsh-0.1.7/Pipfile
+-rw-r--r--   0 paulbutler   (501) staff       (20)    64876 2023-04-10 14:13:02.000000 botsh-0.1.7/Pipfile.lock
+-rw-r--r--   0 paulbutler   (501) staff       (20)     4301 2023-05-15 14:36:42.000000 botsh-0.1.7/README.md
+-rw-r--r--   0 paulbutler   (501) staff       (20)       38 2023-05-15 14:39:55.787932 botsh-0.1.7/setup.cfg
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1597 2023-05-15 14:39:40.000000 botsh-0.1.7/setup.py
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-05-15 14:39:55.783268 botsh-0.1.7/src/
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-05-15 14:39:55.786652 botsh-0.1.7/src/botsh/
+-rw-r--r--   0 paulbutler   (501) staff       (20)        0 2023-04-10 09:30:05.000000 botsh-0.1.7/src/botsh/__init__.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3663 2023-05-15 14:38:22.000000 botsh-0.1.7/src/botsh/docker_exec.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)      317 2023-04-10 11:28:56.000000 botsh-0.1.7/src/botsh/history.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1581 2023-05-15 14:36:42.000000 botsh-0.1.7/src/botsh/llm.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)       46 2023-04-10 12:14:03.000000 botsh-0.1.7/src/botsh/logging.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2718 2023-04-10 14:39:56.000000 botsh-0.1.7/src/botsh/main.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1204 2023-05-15 14:36:42.000000 botsh-0.1.7/src/botsh/prompt.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2189 2023-05-15 14:36:42.000000 botsh-0.1.7/src/botsh/task_driver.py
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-05-15 14:39:55.787533 botsh-0.1.7/src/botsh/templates/
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1099 2023-05-15 14:36:42.000000 botsh-0.1.7/src/botsh/templates/prompt.jinja2
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-05-15 14:39:55.787426 botsh-0.1.7/src/botsh.egg-info/
+-rw-r--r--   0 paulbutler   (501) staff       (20)     4962 2023-05-15 14:39:55.000000 botsh-0.1.7/src/botsh.egg-info/PKG-INFO
+-rw-r--r--   0 paulbutler   (501) staff       (20)      462 2023-05-15 14:39:55.000000 botsh-0.1.7/src/botsh.egg-info/SOURCES.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)        1 2023-05-15 14:39:55.000000 botsh-0.1.7/src/botsh.egg-info/dependency_links.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)       42 2023-05-15 14:39:55.000000 botsh-0.1.7/src/botsh.egg-info/entry_points.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)      881 2023-05-15 14:39:55.000000 botsh-0.1.7/src/botsh.egg-info/requires.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)        6 2023-05-15 14:39:55.000000 botsh-0.1.7/src/botsh.egg-info/top_level.txt
```

### Comparing `botsh-0.1.6/LICENSE` & `botsh-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `botsh-0.1.6/PKG-INFO` & `botsh-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.6
+Version: 0.1.7
 Summary: A task runner powered by OpenAI and Docker.
 Home-page: https://github.com/drifting-in-space/botsh
 Author: Paul Butler
 Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,21 +19,31 @@
 
 # `botsh`
 
 [![PyPI version](https://badge.fury.io/py/botsh.svg)](https://badge.fury.io/py/botsh)
 
 `botsh` attaches a chat agent to a Docker container running Ubuntu.
 
-This effectively gives the agent access to the entire [Apt](https://wiki.debian.org/Apt)
-universe, while limiting its blast radius to the current directory.
+This effectively gives the agent access to the entire [APT](https://wiki.debian.org/Apt)
+universe, while limiting its blast radius to the current directory (which gets mounted into the container).
 
 ## Demo
 
 This demo uses the prompt `create a sequence of 100 200x200 images which each contain a different number, and turn them into a 30fps video with ffmpeg`.
 
+`botsh`:
+
+- tries to run `imagemagick` and fails (because it is a fresh Ubuntu install)
+- installs `imagemagick`
+- attempts to run `ffmpeg` and fails
+- installs `ffmpeg`
+- attempts to turn frames into a video and fails (because it has not created them)
+- writes a bash for-loop to generate 100 frames with `imagemagick`
+- uses `ffmpeg` to convert them into a video
+
 https://user-images.githubusercontent.com/46173/230953506-c8545345-c0a1-46b1-b937-458191fc2456.mp4
 
 ## Setup
 
 Install with:
 
     pip install botsh
@@ -41,19 +51,19 @@
 `botsh` expects an OpenAI API key to be provided as the `OPENAI_API_KEY`
 environment variable.
 
 `botsh` also requires Docker to be running on the system.
 
 ## Examples
 
-    # botsh "convert cat.jpg into a png file"
+    botsh "convert cat.jpg into a png file"
 
-    # botsh "use a remote service to find my public ip and base64 encode it"
+    botsh "use a remote service to find my public ip and base64 encode it"
 
-    # botsh "run pylint on the codebase in src/"
+    botsh "run pylint on the codebase in src/"
 
 ## Additional details
 
 `botsh` will create a bare Ubuntu Docker container associated with
 the current directory, or create one if one does not exist. botsh
 will then attach the OpenAI API to a shell running in the container
 to attempt to complete the given task.
```

### Comparing `botsh-0.1.6/Pipfile.lock` & `botsh-0.1.7/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `botsh-0.1.6/README.md` & `botsh-0.1.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 # `botsh`
 
 [![PyPI version](https://badge.fury.io/py/botsh.svg)](https://badge.fury.io/py/botsh)
 
 `botsh` attaches a chat agent to a Docker container running Ubuntu.
 
-This effectively gives the agent access to the entire [Apt](https://wiki.debian.org/Apt)
-universe, while limiting its blast radius to the current directory.
+This effectively gives the agent access to the entire [APT](https://wiki.debian.org/Apt)
+universe, while limiting its blast radius to the current directory (which gets mounted into the container).
 
 ## Demo
 
 This demo uses the prompt `create a sequence of 100 200x200 images which each contain a different number, and turn them into a 30fps video with ffmpeg`.
 
+`botsh`:
+
+- tries to run `imagemagick` and fails (because it is a fresh Ubuntu install)
+- installs `imagemagick`
+- attempts to run `ffmpeg` and fails
+- installs `ffmpeg`
+- attempts to turn frames into a video and fails (because it has not created them)
+- writes a bash for-loop to generate 100 frames with `imagemagick`
+- uses `ffmpeg` to convert them into a video
+
 https://user-images.githubusercontent.com/46173/230953506-c8545345-c0a1-46b1-b937-458191fc2456.mp4
 
 ## Setup
 
 Install with:
 
     pip install botsh
@@ -22,19 +32,19 @@
 `botsh` expects an OpenAI API key to be provided as the `OPENAI_API_KEY`
 environment variable.
 
 `botsh` also requires Docker to be running on the system.
 
 ## Examples
 
-    # botsh "convert cat.jpg into a png file"
+    botsh "convert cat.jpg into a png file"
 
-    # botsh "use a remote service to find my public ip and base64 encode it"
+    botsh "use a remote service to find my public ip and base64 encode it"
 
-    # botsh "run pylint on the codebase in src/"
+    botsh "run pylint on the codebase in src/"
 
 ## Additional details
 
 `botsh` will create a bare Ubuntu Docker container associated with
 the current directory, or create one if one does not exist. botsh
 will then attach the OpenAI API to a shell running in the container
 to attempt to complete the given task.
```

### Comparing `botsh-0.1.6/setup.py` & `botsh-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         f"{pkg_name}{pkg_info['version']}"
         for pkg_name, pkg_info in pipfile_lock[mode].items()
     ]
 
 
 setup(
     name="botsh",
-    version="0.1.6",
+    version="0.1.7",
     description="A task runner powered by OpenAI and Docker.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Paul Butler",
     author_email="paul@driftingin.space",
     url="https://github.com/drifting-in-space/botsh",
     packages=find_packages("src"),
```

### Comparing `botsh-0.1.6/src/botsh/docker_exec.py` & `botsh-0.1.7/src/botsh/docker_exec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import hashlib
 import os
 import shlex
 
 import docker
 from docker.types import Mount
 from termcolor import colored
+import platform
 
 from botsh.logging import log
 
 
 class DockerContainer:
     current_directory: str
     shell_command: str
@@ -21,23 +22,23 @@
         self.current_directory = os.getcwd()
         self.shell_command = shell_command
         dir_hash = hashlib.sha256(self.current_directory.encode("utf-8")).hexdigest()
         container_name = f"botsh-{dir_hash}"
 
         log.info("Connecting to Docker...")
         try:
-           self.client = docker.from_env()
+            self.client = docker.from_env()
         except Exception as e:
-           log.error(
-                "Permission error connecting to Docker. "
-                "Is Docker running? "
-                "You may need to follow these instructions: "
-                "https://docs.docker.com/engine/install/linux-postinstall/.",
-           )
-           exit(1)
+            log.error("Error connecting to Docker. Is Docker running?", err=e)
+            if platform.system() == "Linux":
+                log.info(
+                    "You may need to follow these instructions: "
+                    "https://docs.docker.com/engine/install/linux-postinstall/."
+                )
+            exit(1)
 
         self._get_container(container_name, image, wipe)
 
     def _get_mounts(self) -> list[Mount]:
         mount = Mount(target="/work", source=self.current_directory, type="bind")
 
         return [mount]
```

### Comparing `botsh-0.1.6/src/botsh/llm.py` & `botsh-0.1.7/src/botsh/llm.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.6/src/botsh/main.py` & `botsh-0.1.7/src/botsh/main.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.6/src/botsh/prompt.py` & `botsh-0.1.7/src/botsh/prompt.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.6/src/botsh/task_driver.py` & `botsh-0.1.7/src/botsh/task_driver.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.6/src/botsh/templates/prompt.jinja2` & `botsh-0.1.7/src/botsh/templates/prompt.jinja2`

 * *Files identical despite different names*

### Comparing `botsh-0.1.6/src/botsh.egg-info/PKG-INFO` & `botsh-0.1.7/src/botsh.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.6
+Version: 0.1.7
 Summary: A task runner powered by OpenAI and Docker.
 Home-page: https://github.com/drifting-in-space/botsh
 Author: Paul Butler
 Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,21 +19,31 @@
 
 # `botsh`
 
 [![PyPI version](https://badge.fury.io/py/botsh.svg)](https://badge.fury.io/py/botsh)
 
 `botsh` attaches a chat agent to a Docker container running Ubuntu.
 
-This effectively gives the agent access to the entire [Apt](https://wiki.debian.org/Apt)
-universe, while limiting its blast radius to the current directory.
+This effectively gives the agent access to the entire [APT](https://wiki.debian.org/Apt)
+universe, while limiting its blast radius to the current directory (which gets mounted into the container).
 
 ## Demo
 
 This demo uses the prompt `create a sequence of 100 200x200 images which each contain a different number, and turn them into a 30fps video with ffmpeg`.
 
+`botsh`:
+
+- tries to run `imagemagick` and fails (because it is a fresh Ubuntu install)
+- installs `imagemagick`
+- attempts to run `ffmpeg` and fails
+- installs `ffmpeg`
+- attempts to turn frames into a video and fails (because it has not created them)
+- writes a bash for-loop to generate 100 frames with `imagemagick`
+- uses `ffmpeg` to convert them into a video
+
 https://user-images.githubusercontent.com/46173/230953506-c8545345-c0a1-46b1-b937-458191fc2456.mp4
 
 ## Setup
 
 Install with:
 
     pip install botsh
@@ -41,19 +51,19 @@
 `botsh` expects an OpenAI API key to be provided as the `OPENAI_API_KEY`
 environment variable.
 
 `botsh` also requires Docker to be running on the system.
 
 ## Examples
 
-    # botsh "convert cat.jpg into a png file"
+    botsh "convert cat.jpg into a png file"
 
-    # botsh "use a remote service to find my public ip and base64 encode it"
+    botsh "use a remote service to find my public ip and base64 encode it"
 
-    # botsh "run pylint on the codebase in src/"
+    botsh "run pylint on the codebase in src/"
 
 ## Additional details
 
 `botsh` will create a bare Ubuntu Docker container associated with
 the current directory, or create one if one does not exist. botsh
 will then attach the OpenAI API to a shell running in the container
 to attempt to complete the given task.
```

### Comparing `botsh-0.1.6/src/botsh.egg-info/requires.txt` & `botsh-0.1.7/src/botsh.egg-info/requires.txt`

 * *Files identical despite different names*

