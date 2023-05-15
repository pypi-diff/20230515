# Comparing `tmp/smartgpt-0.1.1.tar.gz` & `tmp/smartgpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartgpt-0.1.1.tar", last modified: Mon May 15 03:56:23 2023, max compression
+gzip compressed data, was "smartgpt-0.1.2.tar", last modified: Mon May 15 04:08:50 2023, max compression
```

## Comparing `smartgpt-0.1.1.tar` & `smartgpt-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.638495 smartgpt-0.1.1/
--rw-r--r--   0 evan       (501) staff       (20)     1067 2023-05-11 06:26:43.000000 smartgpt-0.1.1/LICENSE
--rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-15 03:56:23.638737 smartgpt-0.1.1/PKG-INFO
--rw-r--r--   0 evan       (501) staff       (20)     2273 2023-05-14 20:48:56.000000 smartgpt-0.1.1/README.md
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.631620 smartgpt-0.1.1/bin/
--rwxrwxrwx   0 evan       (501) staff       (20)     5058 2023-05-15 03:51:22.000000 smartgpt-0.1.1/bin/smartgpt
--rw-r--r--   0 evan       (501) staff       (20)       62 2023-05-11 06:10:56.000000 smartgpt-0.1.1/pyproject.toml
--rw-r--r--   0 evan       (501) staff       (20)      103 2023-05-15 03:56:23.639641 smartgpt-0.1.1/setup.cfg
--rw-r--r--   0 evan       (501) staff       (20)      470 2023-05-15 03:55:56.000000 smartgpt-0.1.1/setup.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.634983 smartgpt-0.1.1/smartgpt/
--rw-r--r--   0 evan       (501) staff       (20)      237 2023-05-15 03:44:52.000000 smartgpt-0.1.1/smartgpt/__init__.py
--rw-r--r--   0 evan       (501) staff       (20)    10063 2023-05-15 03:44:52.000000 smartgpt-0.1.1/smartgpt/chat.py
--rw-r--r--   0 evan       (501) staff       (20)     5538 2023-05-15 03:50:20.000000 smartgpt-0.1.1/smartgpt/datatypes.py
--rw-r--r--   0 evan       (501) staff       (20)     1130 2023-05-15 03:44:52.000000 smartgpt-0.1.1/smartgpt/error.py
--rw-r--r--   0 evan       (501) staff       (20)     1510 2023-05-15 01:46:46.000000 smartgpt-0.1.1/smartgpt/logger.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.638017 smartgpt-0.1.1/smartgpt/prompts/
--rw-r--r--   0 evan       (501) staff       (20)      995 2023-05-14 20:45:10.000000 smartgpt-0.1.1/smartgpt/prompts/__init__.py
--rw-r--r--   0 evan       (501) staff       (20)     2113 2023-05-15 03:31:58.000000 smartgpt-0.1.1/smartgpt/repl.py
--rw-r--r--   0 evan       (501) staff       (20)     1379 2023-05-11 06:10:56.000000 smartgpt-0.1.1/smartgpt/strenum.py
--rw-r--r--   0 evan       (501) staff       (20)      808 2023-05-15 00:52:53.000000 smartgpt-0.1.1/smartgpt/user_profile.py
--rw-r--r--   0 evan       (501) staff       (20)      900 2023-05-15 03:44:53.000000 smartgpt-0.1.1/smartgpt/util.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.637299 smartgpt-0.1.1/smartgpt.egg-info/
--rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/PKG-INFO
--rw-r--r--   0 evan       (501) staff       (20)      459 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/SOURCES.txt
--rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/dependency_links.txt
--rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 00:27:20.000000 smartgpt-0.1.1/smartgpt.egg-info/not-zip-safe
--rw-r--r--   0 evan       (501) staff       (20)       42 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/requires.txt
--rw-r--r--   0 evan       (501) staff       (20)        9 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/top_level.txt
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:08:50.577889 smartgpt-0.1.2/
+-rw-r--r--   0 evan       (501) staff       (20)     1067 2023-05-11 06:26:43.000000 smartgpt-0.1.2/LICENSE
+-rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-15 04:08:50.578105 smartgpt-0.1.2/PKG-INFO
+-rw-r--r--   0 evan       (501) staff       (20)     2273 2023-05-14 20:48:56.000000 smartgpt-0.1.2/README.md
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:08:50.568493 smartgpt-0.1.2/bin/
+-rwxrwxrwx   0 evan       (501) staff       (20)     5058 2023-05-15 03:51:22.000000 smartgpt-0.1.2/bin/smartgpt
+-rw-r--r--   0 evan       (501) staff       (20)       62 2023-05-11 06:10:56.000000 smartgpt-0.1.2/pyproject.toml
+-rw-r--r--   0 evan       (501) staff       (20)      103 2023-05-15 04:08:50.579180 smartgpt-0.1.2/setup.cfg
+-rw-r--r--   0 evan       (501) staff       (20)      588 2023-05-15 04:08:10.000000 smartgpt-0.1.2/setup.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:08:50.572741 smartgpt-0.1.2/smartgpt/
+-rw-r--r--   0 evan       (501) staff       (20)      237 2023-05-15 03:44:52.000000 smartgpt-0.1.2/smartgpt/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)    10063 2023-05-15 03:44:52.000000 smartgpt-0.1.2/smartgpt/chat.py
+-rw-r--r--   0 evan       (501) staff       (20)     5538 2023-05-15 03:50:20.000000 smartgpt-0.1.2/smartgpt/datatypes.py
+-rw-r--r--   0 evan       (501) staff       (20)     1130 2023-05-15 03:44:52.000000 smartgpt-0.1.2/smartgpt/error.py
+-rw-r--r--   0 evan       (501) staff       (20)     1510 2023-05-15 01:46:46.000000 smartgpt-0.1.2/smartgpt/logger.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:08:50.577341 smartgpt-0.1.2/smartgpt/prompts/
+-rw-r--r--   0 evan       (501) staff       (20)      995 2023-05-14 20:45:10.000000 smartgpt-0.1.2/smartgpt/prompts/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)     2113 2023-05-15 03:31:58.000000 smartgpt-0.1.2/smartgpt/repl.py
+-rw-r--r--   0 evan       (501) staff       (20)     1379 2023-05-11 06:10:56.000000 smartgpt-0.1.2/smartgpt/strenum.py
+-rw-r--r--   0 evan       (501) staff       (20)      808 2023-05-15 00:52:53.000000 smartgpt-0.1.2/smartgpt/user_profile.py
+-rw-r--r--   0 evan       (501) staff       (20)      900 2023-05-15 03:44:53.000000 smartgpt-0.1.2/smartgpt/util.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 04:08:50.576681 smartgpt-0.1.2/smartgpt.egg-info/
+-rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-15 04:08:50.000000 smartgpt-0.1.2/smartgpt.egg-info/PKG-INFO
+-rw-r--r--   0 evan       (501) staff       (20)      459 2023-05-15 04:08:50.000000 smartgpt-0.1.2/smartgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 04:08:50.000000 smartgpt-0.1.2/smartgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 00:27:20.000000 smartgpt-0.1.2/smartgpt.egg-info/not-zip-safe
+-rw-r--r--   0 evan       (501) staff       (20)       42 2023-05-15 04:08:50.000000 smartgpt-0.1.2/smartgpt.egg-info/requires.txt
+-rw-r--r--   0 evan       (501) staff       (20)        9 2023-05-15 04:08:50.000000 smartgpt-0.1.2/smartgpt.egg-info/top_level.txt
```

### Comparing `smartgpt-0.1.1/LICENSE` & `smartgpt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/README.md` & `smartgpt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/bin/smartgpt` & `smartgpt-0.1.2/bin/smartgpt`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/smartgpt/chat.py` & `smartgpt-0.1.2/smartgpt/chat.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/smartgpt/datatypes.py` & `smartgpt-0.1.2/smartgpt/datatypes.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/smartgpt/error.py` & `smartgpt-0.1.2/smartgpt/error.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/smartgpt/logger.py` & `smartgpt-0.1.2/smartgpt/logger.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/smartgpt/prompts/__init__.py` & `smartgpt-0.1.2/smartgpt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/smartgpt/repl.py` & `smartgpt-0.1.2/smartgpt/repl.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/smartgpt/strenum.py` & `smartgpt-0.1.2/smartgpt/strenum.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/smartgpt/user_profile.py` & `smartgpt-0.1.2/smartgpt/user_profile.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.1/smartgpt/util.py` & `smartgpt-0.1.2/smartgpt/util.py`

 * *Files identical despite different names*

