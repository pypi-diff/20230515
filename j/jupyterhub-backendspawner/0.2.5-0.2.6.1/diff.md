# Comparing `tmp/jupyterhub-backendspawner-0.2.5.tar.gz` & `tmp/jupyterhub-backendspawner-0.2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.2.5.tar", last modified: Mon May 15 14:46:49 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.2.6.1.tar", last modified: Mon May 15 14:54:58 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.2.5.tar` & `jupyterhub-backendspawner-0.2.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 14:46:49.580796 jupyterhub-backendspawner-0.2.5/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.2.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-15 14:46:49.570796 jupyterhub-backendspawner-0.2.5/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.2.5/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 14:46:49.570796 jupyterhub-backendspawner-0.2.5/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.2.5/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.2.5/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17325 2023-05-15 14:44:20.000000 jupyterhub-backendspawner-0.2.5/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10709 2023-05-15 14:45:56.000000 jupyterhub-backendspawner-0.2.5/backendspawner/eventspawner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 14:46:49.570796 jupyterhub-backendspawner-0.2.5/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-15 14:46:49.000000 jupyterhub-backendspawner-0.2.5/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-15 14:46:49.000000 jupyterhub-backendspawner-0.2.5/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-15 14:46:49.000000 jupyterhub-backendspawner-0.2.5/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-15 14:46:49.000000 jupyterhub-backendspawner-0.2.5/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-15 14:46:49.000000 jupyterhub-backendspawner-0.2.5/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-15 14:46:49.580796 jupyterhub-backendspawner-0.2.5/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-15 14:46:38.000000 jupyterhub-backendspawner-0.2.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 14:54:58.870738 jupyterhub-backendspawner-0.2.6.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.2.6.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      456 2023-05-15 14:54:58.870738 jupyterhub-backendspawner-0.2.6.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.2.6.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 14:54:58.870738 jupyterhub-backendspawner-0.2.6.1/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.2.6.1/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.2.6.1/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17351 2023-05-15 14:54:00.000000 jupyterhub-backendspawner-0.2.6.1/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10721 2023-05-15 14:54:18.000000 jupyterhub-backendspawner-0.2.6.1/backendspawner/eventspawner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 14:54:58.870738 jupyterhub-backendspawner-0.2.6.1/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      456 2023-05-15 14:54:58.000000 jupyterhub-backendspawner-0.2.6.1/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-15 14:54:58.000000 jupyterhub-backendspawner-0.2.6.1/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-15 14:54:58.000000 jupyterhub-backendspawner-0.2.6.1/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-15 14:54:58.000000 jupyterhub-backendspawner-0.2.6.1/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-15 14:54:58.000000 jupyterhub-backendspawner-0.2.6.1/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-15 14:54:58.870738 jupyterhub-backendspawner-0.2.6.1/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      568 2023-05-15 14:54:45.000000 jupyterhub-backendspawner-0.2.6.1/setup.py
```

### Comparing `jupyterhub-backendspawner-0.2.5/LICENSE` & `jupyterhub-backendspawner-0.2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.5/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.2.6.1/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.5/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.2.6.1/backendspawner/backendspawner.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,16 +181,16 @@
     @default("failed_spawn_request_hook")
     def _failed_spawn_request_hook(self):
         return self._default_failed_spawn_request_hook
 
     def _default_failed_spawn_request_hook(self, spawner, exception):
         return
 
-    def run_failed_spawn_request_hook(self, exception):
-        self.failed_spawn_request_hook(self, exception)
+    async def run_failed_spawn_request_hook(self, exception):
+        await maybe_future(self.failed_spawn_request_hook(self, exception))
 
     post_spawn_request_hook = Callable(
         help="""
         If a start of a single-user server was successful, you can run additional commands here.
         This allows you to handle a successful start attempt properly, according to
         your specific backend API.
```

### Comparing `jupyterhub-backendspawner-0.2.5/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.2.6.1/backendspawner/eventspawner.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     async def get_stop_event(self):
         if callable(self.stop_event):
             stop_event = await maybe_future(self.stop_event(self))
         else:
             stop_event = self.stop_event
         return stop_event
 
-    def run_failed_spawn_request_hook(self, exception):
+    async def run_failed_spawn_request_hook(self, exception):
         now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
         event = {
             "progress": 99,
             "failed": False,
             "html_message": f"<details><summary>{now}: JupyterLab start failed. Deleting related resources...</summary>This may take a few seconds.</details>",
         }
         self.latest_events.append(event)
@@ -211,15 +211,15 @@
                 "progress": 100,
                 "failed": True,
                 "html_message": f"<details><summary>{now}: {summary}</summary>{details}</details>",
             }
             return event
 
         self.stop_event = _get_stop_event
-        super().run_failed_spawn_request_hook(exception)
+        await super().run_failed_spawn_request_hook(exception)
 
     def run_pre_spawn_hook(self):
         """Some commands are required."""
         if self.already_stopped:
             raise Exception("Server is in the process of stopping, please wait.")
 
         self.start_id = uuid.uuid4().hex[:8]
```

### Comparing `jupyterhub-backendspawner-0.2.5/setup.py` & `jupyterhub-backendspawner-0.2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.2.5",
+    version="0.2.6.1",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

