# Comparing `tmp/atmoswing-vigicrues-1.1.0.tar.gz` & `tmp/atmoswing-vigicrues-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-1.1.0.tar", last modified: Fri May 12 15:15:38 2023, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.1.1.tar", last modified: Mon May 15 16:16:39 2023, max compression
```

## Comparing `atmoswing-vigicrues-1.1.0.tar` & `atmoswing-vigicrues-1.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.500329 atmoswing-vigicrues-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-12 15:15:38.500329 atmoswing-vigicrues-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-12 15:15:38.500329 atmoswing-vigicrues-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.492329 atmoswing-vigicrues-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.500329 atmoswing-vigicrues-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:39.935382 atmoswing-vigicrues-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-15 16:16:39.935382 atmoswing-vigicrues-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 16:16:39.935382 atmoswing-vigicrues-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:39.931382 atmoswing-vigicrues-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:39.931382 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:39.931382 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:39.931382 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:39.935382 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:39.931382 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-15 16:16:39.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-15 16:16:39.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:16:39.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 16:16:39.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 16:16:39.000000 atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:39.935382 atmoswing-vigicrues-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-15 16:16:21.000000 atmoswing-vigicrues-1.1.1/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.1.0/LICENSE` & `atmoswing-vigicrues-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/pyproject.toml` & `atmoswing-vigicrues-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/__init__.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/__init__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/__main__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime
 import glob
 import importlib
 import subprocess
+import tempfile
+from pathlib import Path
 
 import atmoswing_vigicrues as asv
 
 
 class Controller:
     """
     Classe principale pour la gestion des prévisions AtmoSwing pour le réseau Vigicrues.
@@ -171,23 +173,25 @@
         options = run['with']
         cmd = self._build_atmoswing_cmd(options)
         print(f"Exécution de : '{name}'")
         print(f"Prévision pour la date : {self.date.strftime('%Y-%m-%d %H')}")
         print("Commande: " + ' '.join(cmd))
 
         try:
-            ret = subprocess.run(cmd, capture_output=True, check=True)
+            ret = subprocess.run(cmd, capture_output=True)
 
             if ret.returncode != 0:
                 print("  -> Échec de l'exécution.")
+                self._parse_log_file()
                 raise asv.Error("Erreur de AtmoSwing Forecaster.")
             else:
                 print("  -> Exécution correcte.")
         except Exception as e:
             print("  -> Échec de l'exécution.")
+            self._parse_log_file()
             raise asv.Error(f"Exception de AtmoSwing Forecaster: {e}")
 
     def _build_atmoswing_cmd(self, options):
         now_str = self.date.strftime("%Y%m%d%H")
         cmd = []
 
         if 'atmoswing_path' not in options or not options['atmoswing_path']:
@@ -226,21 +230,19 @@
     def _run_post_actions(self):
         """
         Exécute les opérations postérieures à la prévision par AtmoSwing.
         """
         if not self.post_actions or len(self.post_actions) == 0:
             return
 
-        files = self._get_files_for_post_actions()
+        files = self._list_atmoswing_output_files()
         if len(files) == 0:
             print("  -> Aucun nouveau fichier à traiter en post-action.")
             return
 
-        print(f"  -> {len(files)} nouveaux fichier à traiter en post-action.")
-
         for action in self.post_actions:
             print(f"Exécution de : '{action.type_name}' [{action.name}]")
             action.feed(files, {'forecast_date': self.date})
             if action.run():
                 print("  -> Exécution correcte.")
             else:
                 print("  -> Échec de l'exécution.")
@@ -284,7 +286,18 @@
         return files
 
     def _list_files(self, local_dir, ext, pattern='%Y-%m-%d_%H'):
         local_dir = asv.utils.build_date_dir_structure(local_dir, self.date)
         pattern = f"{str(local_dir)}/{self.date.strftime(pattern)}{f'.*{ext}'}"
         files = glob.glob(pattern)
         return files
+
+    @staticmethod
+    def _parse_log_file():
+        tmp_dir = Path(tempfile.gettempdir())
+        log_file = tmp_dir / "AtmoSwingForecaster.log"
+        if not log_file.exists():
+            print(f"  -> Le journal des logs n'a pas été trouvé ({str(log_file)}).")
+        with open(str(log_file)) as file:
+            for item in file:
+                content = item.replace("\r\n", "").replace("\n", "")
+                print(f"     | {content}")
```

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,23 @@
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
         if not self._file_paths:
             print("  -> Aucun fichier à traiter")
             return False
 
+        files_count = 0
         for file in self._file_paths:
             file = Path(file)
+
+            # Nom du fichier
+            file_path = self._build_file_path(file)
+            if file_path.exists():
+                continue
+
             self._reset_status()
             nc_file = None
 
             if not asv.file_exists(file):
                 self.status = 100
                 self.message = "Absence du fichier netcdf."
             else:
@@ -120,26 +127,27 @@
                     'only_relevant_stations': self.only_relevant_stations
                 },
                 'metadata': metadata,
                 'data': data,
                 'statistics': statistics,
             }
 
-            # Nom du fichier
-            file_path = self._build_file_path(file)
-
             with open(file_path, "w", encoding="utf-8", newline='\r\n') as outfile:
                 if self.use_indentation:
                     json.dump(data, outfile, indent=4, ensure_ascii=False)
                 else:
                     json.dump(data, outfile, ensure_ascii=False)
 
             if nc_file:
                 nc_file.close()
 
+            files_count += 1
+
+        print(f"  -> Nombre de fichiers exportés : {files_count}.")
+
         return True
 
     def _create_metadata_block(self, nc_file):
         block = {
             'atmoswing': {
                 'creation_date': nc_file.creation_date,
                 'origin': nc_file.origin
```

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,43 +64,50 @@
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
         if not self._file_paths:
             print("  -> Aucun fichier à traiter")
             return False
 
+        files_count = 0
         for file in self._file_paths:
             nc_file = asv.Dataset(file, 'r', format='NETCDF4')
             station_ids = self._extract_station_ids(nc_file)
             header_comments = self._create_header_comments(nc_file)
             if self.combine_stations_in_one_file:
+                file_path = self._build_file_path(file)
+                if file_path.exists():
+                    continue
+
                 header_data = self._create_header_data(nc_file, station_ids)
                 content = self._create_content(nc_file, station_ids)
                 full_content = f"{header_comments}{header_data}{content}"
 
-                # File name
-                file_path = self._build_file_path(file)
-
                 with open(file_path, 'w', encoding="utf-8", newline='\r\n') as outfile:
                     outfile.write(full_content)
             else:
                 for station_id in station_ids:
+                    file_path = self._build_file_path(file, station_id)
+                    if file_path.exists():
+                        continue
+
                     header_data = self._create_header_data(nc_file, station_id)
                     content = self._create_content(nc_file, station_id)
                     full_content = f"{header_comments}{header_data}{content}"
 
-                    # File name
-                    file_path = self._build_file_path(file, station_id)
-
                     with open(file_path, 'w', encoding="utf-8", newline='\r\n') \
                             as outfile:
                         outfile.write(full_content)
 
             nc_file.close()
 
+            files_count += 1
+
+        print(f"  -> Nombre de fichiers exportés : {files_count}.")
+
         return True
 
     def _create_header_comments(self, nc_file):
         list_frequencies = [str(int(100 * i)) for i in self.frequencies]
 
         header = \
             f"# Sortie du module ExportPrv de AtmoSwing-Vigicrues\n" \
```

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/postaction.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/postactions/postaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/preaction.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/preaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 
             # Change the directory to the desired remote directory
             sftp.chdir(self.remote_dir)
 
             # Download files
             local_path = Path(self._get_local_path(date))
             forecast_date = date.strftime("%Y%m%d")
+            files_count = 0
             for remote_file in sftp.listdir('.'):
                 pattern = f'{self.prefix.lower()}*_{forecast_date}*.*'
                 if self.variables is not None:
                     for variable in self.variables:
                         pattern = f'{self.prefix.lower()}_{variable.lower()}' \
                                   f'_{forecast_date}*.*'
                         if fnmatch.fnmatch(remote_file.lower(), pattern):
@@ -128,19 +129,22 @@
 
                 if fnmatch.fnmatch(remote_file.lower(), pattern):
                     local_file = local_path / remote_file
                     if local_file.exists():
                         continue
                     sftp.get(remote_file, str(local_file), prefetch=False)
                     self._unpack_if_needed(local_file, local_path)
+                    files_count += 1
 
             # Close the SFTP client and transport objects
             sftp.close()
             transport.close()
 
+            print(f"  -> Nombre de fichiers récupérés : {files_count}.")
+
         except paramiko.ssh_exception.PasswordRequiredException as e:
             print(f"SFTP PasswordRequiredException {e}")
             return False
         except paramiko.ssh_exception.BadAuthenticationType as e:
             print(f"SFTP BadAuthenticationType {e}")
             return False
         except paramiko.ssh_exception.AuthenticationException as e:
```

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/utils.py` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues/utils.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/SOURCES.txt` & `atmoswing-vigicrues-1.1.1/src/atmoswing_vigicrues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_controller.py` & `atmoswing-vigicrues-1.1.1/tests/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,23 +195,7 @@
         config_file=DIR_PATH + '/files/config_atmoswing_now_failing_preaction.yaml',
         batch_file=tmp_dir + '/batch_file_fail.xml'
     )
     controller = get_controller_with_fixed_paths_preaction(options, tmp_dir)
     if RUN_ATMOSWING:
         controller.run()
     shutil.rmtree(tmp_dir)
-
-
-def test_list_only_new_forecaster_files(tmp_dir, capsys):
-    options = types.SimpleNamespace(
-        config_file=DIR_PATH + '/files/config_atmoswing_now_full.yaml',
-        batch_file=tmp_dir + '/batch_file.xml'
-    )
-    controller = get_controller_with_fixed_paths_full(options, tmp_dir)
-    if RUN_ATMOSWING:
-        controller.run()
-        controller.run()
-        captured = capsys.readouterr()
-        assert captured.out.endswith("  -> Aucun nouveau fichier à traiter "
-                                     "en post-action.\n")
-
-    shutil.rmtree(tmp_dir)
```

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_download_gfs.py` & `atmoswing-vigicrues-1.1.1/tests/test_download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_exceptions.py` & `atmoswing-vigicrues-1.1.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_export_bdapbp.py` & `atmoswing-vigicrues-1.1.1/tests/test_export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_export_prv.py` & `atmoswing-vigicrues-1.1.1/tests/test_export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_options.py` & `atmoswing-vigicrues-1.1.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.1/tests/test_transfer_sftp_in.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.1/tests/test_transfer_sftp_out.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,7 @@
 
 def test_upload_nc_succeeds(options, forecast_files):
     action = asv.TransferSftpOut('Upload nc files over SFTP', options)
     action.feed(forecast_files)
     date = datetime(2022, 12, 16, 00)
     if RUN_SFTP:
         assert action.run(date)
-
```

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_transform_gfs.py` & `atmoswing-vigicrues-1.1.1/tests/test_transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.0/tests/test_utils.py` & `atmoswing-vigicrues-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

