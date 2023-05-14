# Comparing `tmp/yokkaichi-1.4.2.tar.gz` & `tmp/yokkaichi-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.4.2.tar", last modified: Sun May 14 19:42:33 2023, max compression
+gzip compressed data, was "yokkaichi-1.4.3.tar", last modified: Sun May 14 22:03:19 2023, max compression
```

## Comparing `yokkaichi-1.4.2.tar` & `yokkaichi-1.4.3.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.4.2/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2252 2023-05-12 19:27:27.000000 yokkaichi-1.4.2/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1503 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2921 2023-05-12 18:51:44.000000 yokkaichi-1.4.2/yokkaichi/MasscanScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     6039 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     8322 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1261 2023-05-12 18:51:44.000000 yokkaichi-1.4.2/yokkaichi/args_to_cfg.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2068 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/yokkaichi/config_loader.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1160 2023-05-12 18:51:44.000000 yokkaichi-1.4.2/yokkaichi/port_parser.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      364 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       63 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:03:19.686141 yokkaichi-1.4.3/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.4.3/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-14 22:03:19.686141 yokkaichi-1.4.3/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2252 2023-05-12 19:27:27.000000 yokkaichi-1.4.3/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-05-14 22:03:19.686141 yokkaichi-1.4.3/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1547 2023-05-14 22:01:12.000000 yokkaichi-1.4.3/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:03:19.682808 yokkaichi-1.4.3/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2921 2023-05-12 18:51:44.000000 yokkaichi-1.4.3/yokkaichi/MasscanScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     6039 2023-05-14 19:38:14.000000 yokkaichi-1.4.3/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-05-14 22:01:12.000000 yokkaichi-1.4.3/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     8322 2023-05-14 21:45:54.000000 yokkaichi-1.4.3/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1261 2023-05-12 18:51:44.000000 yokkaichi-1.4.3/yokkaichi/args_to_cfg.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3800 2023-05-14 22:01:12.000000 yokkaichi-1.4.3/yokkaichi/config_loader.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:03:19.686141 yokkaichi-1.4.3/yokkaichi/constants/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.4.3/yokkaichi/constants/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-05-14 19:38:14.000000 yokkaichi-1.4.3/yokkaichi/constants/rich_console.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1160 2023-05-12 18:51:44.000000 yokkaichi-1.4.3/yokkaichi/port_parser.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:03:19.686141 yokkaichi-1.4.3/yokkaichi/structs/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1053 2023-05-14 22:01:12.000000 yokkaichi-1.4.3/yokkaichi/structs/CFG.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.4.3/yokkaichi/structs/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:03:19.686141 yokkaichi-1.4.3/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-14 22:03:19.000000 yokkaichi-1.4.3/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      487 2023-05-14 22:03:19.000000 yokkaichi-1.4.3/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-05-14 22:03:19.000000 yokkaichi-1.4.3/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       63 2023-05-14 22:03:19.000000 yokkaichi-1.4.3/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-05-14 22:03:19.000000 yokkaichi-1.4.3/yokkaichi.egg-info/top_level.txt
```

### Comparing `yokkaichi-1.4.2/LICENSE.txt` & `yokkaichi-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.2/PKG-INFO` & `yokkaichi-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.4.2
+Version: 1.4.3
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `yokkaichi-1.4.2/README.md` & `yokkaichi-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.2/setup.py` & `yokkaichi-1.4.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,9 +38,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
-    packages=["yokkaichi"],
+    packages=["yokkaichi", "yokkaichi.constants", "yokkaichi.structs"],
 )
```

### Comparing `yokkaichi-1.4.2/yokkaichi/MasscanScan.py` & `yokkaichi-1.4.3/yokkaichi/MasscanScan.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.2/yokkaichi/ServerScan.py` & `yokkaichi-1.4.3/yokkaichi/ServerScan.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.2/yokkaichi/__main__.py` & `yokkaichi-1.4.3/yokkaichi/__main__.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.2/yokkaichi/args_to_cfg.py` & `yokkaichi-1.4.3/yokkaichi/args_to_cfg.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.2/yokkaichi/port_parser.py` & `yokkaichi-1.4.3/yokkaichi/port_parser.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.2/yokkaichi.egg-info/PKG-INFO` & `yokkaichi-1.4.3/yokkaichi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.4.2
+Version: 1.4.3
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

