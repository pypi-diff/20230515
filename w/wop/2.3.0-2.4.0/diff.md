# Comparing `tmp/wop-2.3.0.tar.gz` & `tmp/wop-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wop-2.3.0.tar", last modified: Fri Apr 14 19:20:23 2023, max compression
+gzip compressed data, was "D:\rlafage\workspace\WhatsOpt-CLI\dist\.tmp-wijuiq1d\wop-2.4.0.tar", last modified: Mon May 15 13:06:20 2023, max compression
```

## Comparing `wop-2.3.0.tar` & `wop-2.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 19:20:23.101657 wop-2.3.0/
--rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.3.0/LICENSE
--rw-rw-rw-   0        0        0      851 2023-04-14 19:20:23.101657 wop-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 19:20:23.101657 wop-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1481 2023-04-14 19:05:22.000000 wop-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 19:20:23.039125 wop-2.3.0/tests/
--rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_convert_utils.py
--rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.3.0/tests/test_mooptimization.py
--rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_push_command.py
--rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_push_utils.py
--rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_upload_utils.py
--rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_utils.py
--rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.3.0/tests/test_whatsopt_client.py
--rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_wop.py
-drwxrwxrwx   0        0        0        0 2023-04-14 19:20:23.086006 wop-2.3.0/whatsopt/
--rw-rw-rw-   0        0        0       23 2023-04-12 16:39:47.000000 wop-2.3.0/whatsopt/__init__.py
--rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.3.0/whatsopt/convert_utils.py
--rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.3.0/whatsopt/logging.py
--rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.3.0/whatsopt/mooptimization.py
--rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.3.0/whatsopt/optimization.py
--rw-rw-rw-   0        0        0      232 2023-04-12 16:39:47.000000 wop-2.3.0/whatsopt/publish_utils.py
--rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.3.0/whatsopt/push_command.py
--rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.3.0/whatsopt/push_utils.py
--rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.3.0/whatsopt/show_utils.py
--rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.3.0/whatsopt/upload_utils.py
--rw-rw-rw-   0        0        0     5616 2023-04-07 15:50:56.000000 wop-2.3.0/whatsopt/utils.py
--rw-rw-rw-   0        0        0    36682 2023-04-14 19:05:22.000000 wop-2.3.0/whatsopt/whatsopt_client.py
--rw-rw-rw-   0        0        0    11955 2023-04-14 19:05:22.000000 wop-2.3.0/whatsopt/wop.py
-drwxrwxrwx   0        0        0        0 2023-04-14 19:20:23.101657 wop-2.3.0/wop.egg-info/
--rw-rw-rw-   0        0        0      851 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2019-12-02 13:07:07.000000 wop-2.3.0/wop.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-15 13:06:20.503549 wop-2.4.0/
+-rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0      851 2023-05-15 13:06:20.503549 wop-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 13:06:20.503549 wop-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1481 2023-04-14 19:05:22.000000 wop-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 13:06:20.472293 wop-2.4.0/tests/
+-rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_convert_utils.py
+-rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.4.0/tests/test_mooptimization.py
+-rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_push_command.py
+-rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_push_utils.py
+-rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_upload_utils.py
+-rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.4.0/tests/test_whatsopt_client.py
+-rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.4.0/tests/test_wop.py
+drwxrwxrwx   0        0        0        0 2023-05-15 13:06:20.487925 wop-2.4.0/whatsopt/
+-rw-rw-rw-   0        0        0       23 2023-05-15 12:58:25.000000 wop-2.4.0/whatsopt/__init__.py
+-rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.4.0/whatsopt/convert_utils.py
+-rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.4.0/whatsopt/logging.py
+-rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.4.0/whatsopt/mooptimization.py
+-rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.4.0/whatsopt/optimization.py
+-rw-rw-rw-   0        0        0      232 2023-04-12 16:39:47.000000 wop-2.4.0/whatsopt/publish_utils.py
+-rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.4.0/whatsopt/push_command.py
+-rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.4.0/whatsopt/push_utils.py
+-rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.4.0/whatsopt/show_utils.py
+-rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.4.0/whatsopt/upload_utils.py
+-rw-rw-rw-   0        0        0     6025 2023-05-15 12:58:25.000000 wop-2.4.0/whatsopt/utils.py
+-rw-rw-rw-   0        0        0    40369 2023-05-15 12:58:25.000000 wop-2.4.0/whatsopt/whatsopt_client.py
+-rw-rw-rw-   0        0        0    13166 2023-05-15 12:58:25.000000 wop-2.4.0/whatsopt/wop.py
+drwxrwxrwx   0        0        0        0 2023-05-15 13:06:20.503549 wop-2.4.0/wop.egg-info/
+-rw-rw-rw-   0        0        0      851 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 13:06:20.000000 wop-2.4.0/wop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2019-12-02 13:07:07.000000 wop-2.4.0/wop.egg-info/zip-safe
```

### Comparing `wop-2.3.0/LICENSE` & `wop-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/PKG-INFO` & `wop-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wop
-Version: 2.3.0
+Version: 2.4.0
 Summary: WhatsOpt web application command line client
 Home-page: https://github.com/OneraHub/WhatsOpt-CLI
 Download-URL: https://github.com/OneraHub/WhatsOpt-CLI/releases
 Author: Rémi Lafage
 Author-email: remi.lafage@onera.fr
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wop-2.3.0/README.md` & `wop-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/setup.py` & `wop-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/tests/test_convert_utils.py` & `wop-2.4.0/tests/test_convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/tests/test_push_command.py` & `wop-2.4.0/tests/test_push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/tests/test_push_utils.py` & `wop-2.4.0/tests/test_push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/tests/test_upload_utils.py` & `wop-2.4.0/tests/test_upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/tests/test_utils.py` & `wop-2.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/tests/test_wop.py` & `wop-2.4.0/tests/test_wop.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/whatsopt/convert_utils.py` & `wop-2.4.0/whatsopt/convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/whatsopt/mooptimization.py` & `wop-2.4.0/whatsopt/mooptimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/whatsopt/optimization.py` & `wop-2.4.0/whatsopt/optimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/whatsopt/push_command.py` & `wop-2.4.0/whatsopt/push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/whatsopt/push_utils.py` & `wop-2.4.0/whatsopt/push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/whatsopt/show_utils.py` & `wop-2.4.0/whatsopt/show_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/whatsopt/upload_utils.py` & `wop-2.4.0/whatsopt/upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.3.0/whatsopt/utils.py` & `wop-2.4.0/whatsopt/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os, re
 import sys
 import tomli_w
 from whatsopt.logging import error
+from shutil import move
+
 
 WOP_CONF_FILENAME = ".wop"
 
 WOP_FORMAT_VERSION_KEY = "wop_format_version"
 WHATSOPT_URL_KEY = "whatsopt_url"
 ANALYSIS_ID_KEY = "analysis_id"
 FRAMEWORK_KEY = "framework"
@@ -189,7 +191,20 @@
                 break
     return detected
 
 
 def is_package_mode():
     state = load_state()
     return state and state[PULL_MODE_KEY] == MODE_PACKAGE
+
+
+def move_files(file_to_move, tempdir):
+    for f in file_to_move.keys():
+        file_from = os.path.join(tempdir, f)
+        file_to = f
+        dir_to = os.path.dirname(f)
+        if dir_to == "":
+            dir_to = "."
+        elif not os.path.exists(dir_to):
+            os.makedirs(dir_to)
+        if file_to_move[file_to]:
+            move(file_from, dir_to)
```

### Comparing `wop-2.3.0/whatsopt/whatsopt_client.py` & `wop-2.4.0/whatsopt/whatsopt_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from http import HTTPStatus
-from shutil import move
 import os
 import sys
 import json
 import getpass
 import requests
 import copy
 import re
 import zipfile
 import tempfile
 import numpy as np
 import time
+from datetime import datetime
 import tomli
 import tomli_w
 from tabulate import tabulate
 from urllib.parse import urlparse
 from packaging.version import Version
 
 # push
@@ -38,14 +38,15 @@
     is_framework_switch,
     is_package_mode,
     is_run_script_file,
     is_test_file,
     is_user_file,
     get_analysis_id,
     get_whatsopt_url,
+    move_files,
     save_state,
 )
 from whatsopt.upload_utils import (
     load_from_csv,
     load_from_sqlite,
     load_from_hdf5,
     print_cases,
@@ -446,15 +447,15 @@
             key = "Analysis"
         params = {}
         params[key.lower()] = attrs
         resp = self.session.post(url, headers=self.headers, json=params)
         resp.raise_for_status()
         log("{} {} pushed".format(key, attrs["name"]))
 
-    def pull_mda(self, mda_id, options={}, msg=None):
+    def pull_mda(self, mda_id, options={}, msg=None, info_keep_run_ops=True):
         if not msg:
             msg = "Analysis %s pulled" % mda_id
 
         framework = FRAMEWORK_OPENMDAO
         if options.get("--gemseo"):
             framework = FRAMEWORK_GEMSEO
 
@@ -504,17 +505,17 @@
         zipf.close()
         file_to_move = {}
         if options.get("--dry-run"):
             cmd = "Pull"
             if options.get("--update"):
                 cmd = "Update"
             info(
-                "*******************************************************************\n"
-                f"* {cmd} is run in DRY RUN mode (actions are listed but not done) *\n"
-                "*******************************************************************"
+                "***************************************************\n"
+                f"* DRY RUN mode (actions are listed but not done) *\n"
+                "***************************************************"
             )
 
         # Special case: When framework switch we have to update
         # user analysis main file which name depends on package name
         framework_switch = is_framework_switch(framework)
         if framework_switch:
             url = self.endpoint(f"/api/v1/analyses/{mda_id}/openmdao_impl")
@@ -532,15 +533,16 @@
                     log(f"Update {file_to}")
                     if options.get("--dry-run"):
                         file_to_move[file_to] = False
                     else:
                         os.remove(file_to)
                 elif options.get("--update"):
                     if is_run_script_file(f) and not options.get("--run-ops"):
-                        info(f"Keep existing {file_to} (use -r to override)")
+                        if info_keep_run_ops:
+                            info(f"Keep existing {file_to} (use -r to override)")
                         file_to_move[file_to] = False
                         continue
                     if is_test_file(f) and not options.get("--test-units"):
                         file_to_move[file_to] = False
                         continue
                     if is_user_file(f):
                         file_to_move[file_to] = False
@@ -568,24 +570,15 @@
                     or is_user_file(f)
                 ):
                     file_to_move[file_to] = False
                 else:
                     log(f"Pull {file_to}")
 
         if not options.get("--dry-run"):
-            for f in file_to_move.keys():
-                file_from = os.path.join(tempdir, f)
-                file_to = f
-                dir_to = os.path.dirname(f)
-                if dir_to == "":
-                    dir_to = "."
-                elif not os.path.exists(dir_to):
-                    os.makedirs(dir_to)
-                if file_to_move[file_to]:
-                    move(file_from, dir_to)
+            move_files(file_to_move, tempdir)
             state = {
                 "whatsopt_url": self._url,
                 "analysis_id": mda_id,
                 "framework": framework,
                 "pull_mode": MODE_PACKAGE if options.get("--package") else MODE_PLAIN,
             }
             save_state(state)
@@ -599,15 +592,15 @@
 
     def pull_project_json(self, project_id):
         url = self.endpoint(f"/api/v1/design_projects/{project_id}.wopjson")
         resp = self.session.get(url, headers=self.headers, stream=True)
         resp.raise_for_status()
         print(json.dumps(resp.json()))
 
-    def update_mda(self, analysis_id=None, options={}):
+    def update_mda(self, analysis_id=None, options={}, info_keep_run_ops=True):
         mda_id = analysis_id or get_analysis_id()
         if mda_id and not analysis_id:
             url = get_whatsopt_url()
             if url != self.url:
                 warn(
                     f"You want to update code pulled from {url} while you are logged in {self.url}."
                 )
@@ -639,15 +632,17 @@
                 "--gemseo": opts["--gemseo"]
                 or (not opts["--openmdao"] and is_based_on(FRAMEWORK_GEMSEO)),
                 "--openmdao": opts["--openmdao"]
                 or (not opts["--gemseo"] and is_based_on(FRAMEWORK_OPENMDAO)),
                 "--package": is_package_mode(),
             }
         )
-        self.pull_mda(mda_id, opts, "Analysis #{} updated".format(mda_id))
+        self.pull_mda(
+            mda_id, opts, "Analysis #{} updated".format(mda_id), info_keep_run_ops
+        )
 
     def show_mda(self, analysis_id, pbfile, name, outfile, batch, depth):
         options = {
             "--xdsm": True,
             "--name": name,
             "--dry-run": False,
             "--depth": depth,
@@ -921,32 +916,124 @@
         elif resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
             error(resp.json()["message"])
             error("Duplicate detected! The package already exists on WopStore!")
             exit(-1)
         else:
             resp.raise_for_status()
 
-    def build(self, analysis_id=None):
+    def build(self):
         if not is_package_mode():
             error("Package mode is required!")
             exit(-1)
+        self._update_mda_base()
+        filename = build_package()
+        return filename
+
+    def fetch(self, target_id=None, options={}):
+        if not is_package_mode():
+            error("Package mode is required!")
+            exit(-1)
+        mda_id = get_analysis_id()
+        param = f"?src_id={target_id}"
+        format_query = "mda_pkg_content"
+        url = self.endpoint(
+            f"/api/v1/analyses/{mda_id}/exports/new.{format_query}{param}"
+        )
+        resp = self.session.get(url, headers=self.headers, stream=True)
+        if resp.ok:
+            name = None
+            with tempfile.NamedTemporaryFile(
+                suffix=".zip", mode="wb", delete=False
+            ) as fd:
+                for chunk in resp.iter_content(chunk_size=128):
+                    fd.write(chunk)
+                name = fd.name
+            zipf = zipfile.ZipFile(name, "r")
+            tempdir = tempfile.mkdtemp(suffix="wop", dir=tempfile.tempdir)
+            zipf.extractall(tempdir)
+            filenames = zipf.namelist()
+            zipf.close()
+
+            file_to_move = {}
+            for f in filenames:
+                file_to = f
+                file_to_move[file_to] = True
+                if os.path.exists(file_to):
+                    if options.get("--force"):
+                        log(f"Fetch {file_to}")
+                        if options.get("--dry-run"):
+                            file_to_move[file_to] = False
+                        else:
+                            os.remove(file_to)
+                    else:
+                        warn(
+                            f"File {file_to} in the way: remove it or use --force to override"
+                        )
+                        file_to_move[file_to] = False
+                else:
+                    log(f"Fetch {file_to}")
+            if not options.get("--dry-run"):
+                move_files(file_to_move, tempdir)
+                log(f"Analysis #{target_id} fetched")
+        else:
+            error(f"Error while fetching Analysis #{target_id}")
+            resp.raise_for_status()
+
+    def merge(self, target_id=None, options={}):
+        if not is_package_mode():
+            error("Package mode is required!")
+            exit(-1)
+        current_id = get_analysis_id()
+        url = self.endpoint(f"/api/v1/analyses/{current_id}")
+        params = {
+            "analysis": {
+                "import": {"analysis": target_id},
+            },
+            "requested_at": str(datetime.now()),
+        }
+        if options.get("--dry-run"):
+            self.get_status()
+            url = self.endpoint("/api/v1/analyses/{}".format(target_id))
+            resp = self.session.get(url, headers=self.headers)
+            log(f"Analysis #{target_id} #{resp.json()} is selected to be merged")
+        else:
+            resp = self.session.put(url, headers=self.headers, json=params)
+        if resp.ok:
+            self.fetch(target_id, options)
+            self._update_mda_base(options.get("--dry-run"), options.get("--force"))
+            if not options.get("--dry-run"):
+                info(f"Analysis #{target_id} successfully merged")
+        elif resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+            error(f"Error while merging Analysis #{target_id}.")
+            error(
+                f"    Check analyses, maybe they are not compatible (same variable produced by different disciplines)"
+            )
+        elif resp.status_code == HTTPStatus.FORBIDDEN:
+            error(f"Error while merging Analysis #{target_id}.")
+            error(
+                f"    You are not authorized to update the current analysis: either you do not own it or"
+                f" current analysis is already packaged or operated"
+            )
+        else:
+            error(f"Error while merging Analysis #{target_id}")
+            resp.raise_for_status()
+
+    def _update_mda_base(self, dry_run=False, force=False):
         update_options = {
-            "--dry-run": False,
-            "--force": False,
+            "--dry-run": dry_run,
+            "--force": force,
             "--server": False,
             "--egmdo": False,
             "--run-ops": False,
             "--test-units": False,
             "--gemseo": is_based_on(FRAMEWORK_GEMSEO),
             "--openmdao": is_based_on(FRAMEWORK_OPENMDAO),
         }
-        mda_id = analysis_id if analysis_id else get_analysis_id()
-        self.update_mda(mda_id, update_options)
-        filename = build_package()
-        return filename
+        mda_id = get_analysis_id()
+        self.update_mda(mda_id, update_options, info_keep_run_ops=False)
 
     def _test_connection(self):
         if self.api_key:
             self.headers = {
                 "Authorization": "Token token=" + self.api_key,
                 "User-Agent": "wop/{}".format(__version__),
             }
```

### Comparing `wop-2.3.0/whatsopt/wop.py` & `wop-2.4.0/whatsopt/wop.py`

 * *Files 5% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
 @wop.command()
 @click.option(
     "-n",
     "--dry-run",
     is_flag=True,
     default=False,
-    help="print analysis update infos without actually updating",
+    help="print analysis update info without actually updating",
 )
 @click.option(
     "-a",
     "--analysis-id",
     help="specify the analysis to update from (otherwise guessed from current files)",
 )
 @click.option(
@@ -463,9 +463,47 @@
 @wop.command()
 @click.pass_context
 def build(ctx):
     """Build current analysis package. Package mode is required."""
     WhatsOpt(**ctx.obj).login().build()
 
 
+@wop.command()
+@click.option(
+    "-n",
+    "--dry-run",
+    is_flag=True,
+    default=False,
+    help="print analysis fetch info without actually fetching",
+)
+@click.option(
+    "-f", "--force", is_flag=True, default=False, help="overwrite existing files"
+)
+@click.argument("target_id")
+@click.pass_context
+def fetch(ctx, target_id, dry_run, force):
+    """Fetch package content of the given analysis specified by its identifier"""
+    options = {"--dry-run": dry_run, "--force": force}
+    WhatsOpt(**ctx.obj).login().fetch(target_id, options)
+
+
+@wop.command()
+@click.argument("analysis_id")
+@click.pass_context
+@click.option(
+    "-n",
+    "--dry-run",
+    is_flag=True,
+    default=False,
+    help="print analysis merge info without actually merging",
+)
+def merge(ctx, analysis_id, dry_run):
+    """Merge the given analysis to the current one.
+    All the disciplines of the to-be-merged analysis are imported. The command may fail
+    if imported disciplines are not compatible (eg an output variable is already produced
+    by a discipline of the current analysis)."""
+    options = {"--dry-run": dry_run}
+    WhatsOpt(**ctx.obj).login().merge(analysis_id, options)
+
+
 if __name__ == "__main__":
     wop()
```

### Comparing `wop-2.3.0/wop.egg-info/PKG-INFO` & `wop-2.4.0/wop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wop
-Version: 2.3.0
+Version: 2.4.0
 Summary: WhatsOpt web application command line client
 Home-page: https://github.com/OneraHub/WhatsOpt-CLI
 Download-URL: https://github.com/OneraHub/WhatsOpt-CLI/releases
 Author: Rémi Lafage
 Author-email: remi.lafage@onera.fr
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wop-2.3.0/wop.egg-info/SOURCES.txt` & `wop-2.4.0/wop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

