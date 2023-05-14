# Comparing `tmp/kynaylibs-7.1.2.tar.gz` & `tmp/kynaylibs-7.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-7.1.2.tar", last modified: Sun May 14 21:46:29 2023, max compression
+gzip compressed data, was "kynaylibs-7.1.3.tar", last modified: Sun May 14 21:57:01 2023, max compression
```

## Comparing `kynaylibs-7.1.2.tar` & `kynaylibs-7.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.949216 kynaylibs-7.1.2/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     2047 2023-05-14 21:46:05.000000 kynaylibs-7.1.2/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)      704 2023-05-14 21:32:06.000000 kynaylibs-7.1.2/kynaylibs/nan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 20:20:56.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-14 21:32:06.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)     8093 2023-05-14 21:32:06.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-14 21:04:54.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17782 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 20:20:56.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 21:46:05.000000 kynaylibs-7.1.2/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      838 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:57:01.236613 kynaylibs-7.1.3/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:57:01.236613 kynaylibs-7.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:57:01.232613 kynaylibs-7.1.3/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-05-14 21:56:39.000000 kynaylibs-7.1.3/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:57:01.232613 kynaylibs-7.1.3/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)      704 2023-05-14 21:32:06.000000 kynaylibs-7.1.3/kynaylibs/nan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:57:01.232613 kynaylibs-7.1.3/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 20:20:56.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-14 21:32:06.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:57:01.232613 kynaylibs-7.1.3/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)     8093 2023-05-14 21:56:39.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-14 21:04:54.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17782 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 20:20:56.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 21:56:39.000000 kynaylibs-7.1.3/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:57:01.232613 kynaylibs-7.1.3/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:57:01.000000 kynaylibs-7.1.3/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      838 2023-05-14 21:57:01.000000 kynaylibs-7.1.3/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 21:57:01.000000 kynaylibs-7.1.3/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-14 21:57:01.000000 kynaylibs-7.1.3/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 21:57:01.000000 kynaylibs-7.1.3/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 21:57:01.236613 kynaylibs-7.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-14 19:46:25.000000 kynaylibs-7.1.3/setup.py
```

### Comparing `kynaylibs-7.1.2/LICENSE` & `kynaylibs-7.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/PKG-INFO` & `kynaylibs-7.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.1.2
+Version: 7.1.3
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.1.2/README.md` & `kynaylibs-7.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/__init__.py` & `kynaylibs-7.1.3/kynaylibs/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,14 @@
 import sys
 from importlib import import_module
 
 import pyrogram
-from naya import *
-from naya.modules import loadModule
 from pyrogram import *
 from pyrogram import Client, filters
 
-
-async def loadPlugins():
-    modules = loadModule()
-    for mod in modules:
-        imported_module = import_module(f"naya.modules.{mod}")
-        if hasattr(imported_module, "__MODULE__") and imported_module.__MODULE__:
-            imported_module.__MODULE__ = imported_module.__MODULE__
-            if hasattr(imported_module, "__HELP__") and imported_module.__HELP__:
-                CMD_HELP[
-                    imported_module.__MODULE__.replace(" ", "_").lower()
-                ] = imported_module
-
-
 BL_GCAST = [
     -1001599474353,
     -1001692751821,
     -1001473548283,
     -1001459812644,
     -1001433238829,
     -1001476936696,
```

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/__init__.py` & `kynaylibs-7.1.3/kynaylibs/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/ai.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/basic.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/constants.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/db/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         group_description = "Jangan Hapus Atau Keluar Dari Grup Ini\n\nCreated By @KynanSupport .\nJika menemukan kendala atau ingin menanyakan sesuatu\nHubungi : @kenapanan, @rizzvbss atau bisa ke @KynanSupport."
         group = await bot.create_supergroup(group_name, group_description)
         botlog_chat_id = group.id
         message_text = "Grup Log Berhasil Dibuat,\nKetik `setlog` untuk menentapkan grup log ini sebagai tempat log bot\n"
         await bot.send_message(botlog_chat_id, message_text)
         await asyncio.sleep(1)
 
-        await usersdb.users.insert_one(
+        await usersdb.users.update_one(
             {"user_id": user_id},
             {"$set": {"bot_log_group_id": botlog_chat_id}},
             upsert=True,
         )
 
     if botlog_chat_id is None:
         return None
```

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/db/permit.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/function.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/inline.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/interval.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/misc.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/parser.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/pilter.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/tools.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/unpack.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs/nan/utils/utility.py` & `kynaylibs-7.1.3/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-7.1.3/kynaylibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.1.2
+Version: 7.1.3
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.1.2/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-7.1.3/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.2/setup.py` & `kynaylibs-7.1.3/setup.py`

 * *Files identical despite different names*

