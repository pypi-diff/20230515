# Comparing `tmp/hoyo-daily-logins-helper-2.2.1.tar.gz` & `tmp/hoyo-daily-logins-helper-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.2.1.tar", last modified: Sun May 14 01:48:02 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.3.0.tar", last modified: Mon May 15 03:55:52 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.2.1.tar` & `hoyo-daily-logins-helper-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.475201 hoyo-daily-logins-helper-2.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.297960 hoyo-daily-logins-helper-2.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 03:55:52.305960 hoyo-daily-logins-helper-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:52.301960 hoyo-daily-logins-helper-2.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 03:55:52.000000 hoyo-daily-logins-helper-2.3.0/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 03:55:30.000000 hoyo-daily-logins-helper-2.3.0/src/utils.py
```

### Comparing `hoyo-daily-logins-helper-2.2.1/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-2.3.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.1/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.1/.gitignore` & `hoyo-daily-logins-helper-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.1/LICENSE` & `hoyo-daily-logins-helper-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.1/PKG-INFO` & `hoyo-daily-logins-helper-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.2.1
+Version: 2.3.0
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
+![](https://i.imgur.com/LiWb3EG.png)
+
 ## Usage
 
 1. Get your cookie string, open the daily check in page
    * [Daily Check-in page for Genshin Impact](https://act.hoyolab.com/ys/event/signin-sea-v3/index.html?act_id=e202102251931481)
    * [Daily Check-in page for Honkai: Star Rail](https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html?act_id=e202303301540311)
    * [Daily Check-in page for Honkai Impact 3rd](https://act.hoyolab.com/bbs/event/signin-bh3/index.html?act_id=e202110291205111)
    * [Daily Check-in page for Tears of Themis](https://act.hoyolab.com/bbs/event/signin/nxx/index.html?act_id=e202202281857121)
@@ -173,12 +175,24 @@
 cookie = "My Starrail Cookie..."
 # this account is in a different region so you have to explicitly overwrite this
 region = "Asia"
 ```
 
 If you are not setting the regions properly the scheduler will run at the wrong time.
 
+### Discord notifications
+
+If you want to ping a Discord channel create a webhook and add it to the configuration:
+
+```toml
+[config]
+# ...
+notifications = [
+    {type = "discord", webhook_url = "https://...."}
+]
+```
+
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.2.1/README.md` & `hoyo-daily-logins-helper-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
+![](https://i.imgur.com/LiWb3EG.png)
+
 ## Usage
 
 1. Get your cookie string, open the daily check in page
    * [Daily Check-in page for Genshin Impact](https://act.hoyolab.com/ys/event/signin-sea-v3/index.html?act_id=e202102251931481)
    * [Daily Check-in page for Honkai: Star Rail](https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html?act_id=e202303301540311)
    * [Daily Check-in page for Honkai Impact 3rd](https://act.hoyolab.com/bbs/event/signin-bh3/index.html?act_id=e202110291205111)
    * [Daily Check-in page for Tears of Themis](https://act.hoyolab.com/bbs/event/signin/nxx/index.html?act_id=e202202281857121)
@@ -162,12 +164,24 @@
 cookie = "My Starrail Cookie..."
 # this account is in a different region so you have to explicitly overwrite this
 region = "Asia"
 ```
 
 If you are not setting the regions properly the scheduler will run at the wrong time.
 
+### Discord notifications
+
+If you want to ping a Discord channel create a webhook and add it to the configuration:
+
+```toml
+[config]
+# ...
+notifications = [
+    {type = "discord", webhook_url = "https://...."}
+]
+```
+
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.2.1/hoyo-daily-logins-helper.toml.template` & `hoyo-daily-logins-helper-2.3.0/hoyo-daily-logins-helper.toml.template`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 [config]
 language = "en-us"
+notifications = [
+    # {type = "discord", webhook_url = "..."}
+]
 
 [[accounts]]
 identifier = "My Genshin Account Name" # this serves no purpose beyond identification for you in the logs
 game = "genshin"
 cookie = "My Genshin Cookie..."
 
 [[accounts]]
```

### Comparing `hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.2.1
+Version: 2.3.0
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
+![](https://i.imgur.com/LiWb3EG.png)
+
 ## Usage
 
 1. Get your cookie string, open the daily check in page
    * [Daily Check-in page for Genshin Impact](https://act.hoyolab.com/ys/event/signin-sea-v3/index.html?act_id=e202102251931481)
    * [Daily Check-in page for Honkai: Star Rail](https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html?act_id=e202303301540311)
    * [Daily Check-in page for Honkai Impact 3rd](https://act.hoyolab.com/bbs/event/signin-bh3/index.html?act_id=e202110291205111)
    * [Daily Check-in page for Tears of Themis](https://act.hoyolab.com/bbs/event/signin/nxx/index.html?act_id=e202202281857121)
@@ -173,12 +175,24 @@
 cookie = "My Starrail Cookie..."
 # this account is in a different region so you have to explicitly overwrite this
 region = "Asia"
 ```
 
 If you are not setting the regions properly the scheduler will run at the wrong time.
 
+### Discord notifications
+
+If you want to ping a Discord channel create a webhook and add it to the configuration:
+
+```toml
+[config]
+# ...
+notifications = [
+    {type = "discord", webhook_url = "https://...."}
+]
+```
+
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.3.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 src/__init__.py
 src/__main__.py
 src/_version.py
 src/consts.py
 src/games.py
 src/http.py
 src/main.py
-src/scheduler.py
+src/notifications.py
+src/scheduler.py
+src/utils.py
```

### Comparing `hoyo-daily-logins-helper-2.2.1/pyproject.toml` & `hoyo-daily-logins-helper-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.1/requirements.txt` & `hoyo-daily-logins-helper-2.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.1/src/games.py` & `hoyo-daily-logins-helper-2.3.0/src/games.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
+import logging
 import random
 import time
-import logging
+from typing import Optional
 
 from src.http import http_get_json, http_post_json
-
+from src.notifications import NotificationManager, Notification
 
 RET_CODE_ALREADY_SIGNED_IN = -5003
 
 GAMES = {
     "genshin": {
         "name": "Genshin Impact",
         "event_base_url": "https://hk4e-api-os.mihoyo.com/event/sol",
@@ -29,18 +30,19 @@
         "event_base_url": "https://sg-public-api.hoyolab.com/event/luna/os",
         "act_id": "e202202281857121",
     }
 }
 
 
 def game_perform_checkin(
-    account_ident: str,
-    game: str,
-    cookie_str: str,
-    language: str,
+        account_ident: str,
+        game: str,
+        cookie_str: str,
+        language: str,
+        notification_manager: Optional[NotificationManager]
 ):
     if game not in GAMES:
         raise Exception(f"unknown game identifier found: {game}")
 
     game_name = GAMES[game]["name"]
     event_base_url = GAMES[game]["event_base_url"]
     act_id = GAMES[game]["act_id"]
@@ -102,15 +104,40 @@
     logging.debug(f"return code {code}")
 
     if code == RET_CODE_ALREADY_SIGNED_IN:
         logging.info("Already signed in for today...")
         return
     elif code != 0:
         logging.error(response['message'])
+        if notification_manager:
+            notification_manager.send(Notification(
+                success=False,
+                account_identifier=account_ident,
+                game_name=game_name,
+                message=response["message"],
+            ))
         return
 
     reward = awards[total_sign_in_day - 1]
 
     logging.info("Check-in complete!")
     logging.info(f"\tTotal Sign-in Days: {total_sign_in_day + 1}")
     logging.info(f"\tReward: {reward['cnt']}x {reward['name']}")
-    logging.info(f"\tMessage: {response['message']}")
+    logging.info(f"\tMessage: {response['message']}")
+
+    if notification_manager:
+        notification_manager.send(Notification(
+            success=True,
+            account_identifier=account_ident,
+            game_name=game_name,
+            message=response["message"],
+            custom_fields=[
+                {
+                    "key": "Total Sign-in days",
+                    "value": total_sign_in_day + 1
+                },
+                {
+                    "key": "Rewards",
+                    "value": f"{reward['cnt']}x {reward['name']}",
+                },
+            ],
+        ))
```

### Comparing `hoyo-daily-logins-helper-2.2.1/src/http.py` & `hoyo-daily-logins-helper-2.3.0/src/http.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import logging
 from typing import Dict
 
 import requests
 from requests import HTTPError, Response
 
+from src.utils import dict_prettify
+
 USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) " \
               "AppleWebKit/537.36 (KHTML, like Gecko) " \
               "Chrome/74.0.3729.169 Safari/537.36"
 _http_req_settings = {"user_agent": USER_AGENT}
 
 
 def http_set_user_agent(user_agent: str):
@@ -41,17 +43,21 @@
     max_retries: int = 2,
     **kwargs
 ) -> Response:
     for i in range(max_retries + 1):
         try:
             logging.debug(f"{method.upper()} {url}, REQ: {i+1}/{max_retries}")
             session = requests.Session()
-            session.headers["USER_AGENT"] = _http_req_settings["user_agent"]
+            session.headers["User-Agent"] = _http_req_settings["user_agent"]
             resp = session.request(method, url, **kwargs)
-            logging.debug(f"Response: {resp.status_code}\n\n{resp.text}\n")
+
+            text = resp.text
+            if resp.headers.get("Content-Type", "") == "application/json":
+                text = dict_prettify(json.loads(text))
+            logging.debug(f"Response: {resp.status_code}\n\n{text}\n")
         except HTTPError as e:
             logging.error(f"HTTP error: {e}, REQ: {i+1}/{max_retries}")
         except KeyError as e:
             logging.error(f"Wrong response: {e}, REQ: {i+1}/{max_retries}")
         except Exception as e:
             logging.error(f"Unknown error: {e}, REQ: {i+1}/{max_retries}")
         else:
```

### Comparing `hoyo-daily-logins-helper-2.2.1/src/main.py` & `hoyo-daily-logins-helper-2.3.0/src/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import logging
 import os
 import sys
 import tomllib
 from pathlib import Path
+from typing import Optional
 
 import comboparse
 
 from src._version import __version__
 from src.consts import DEFAULT_LANGUAGE
 from src.games import GAMES, game_perform_checkin
 from src.http import http_set_user_agent
+from src.notifications import NotificationManager
 from src.scheduler import run_scheduler
+from src.utils import dict_prettify
 
 
 def main():
     """ Main function for CLI """
     cli_args = list(sys.argv[1:])
     default_file = Path("hoyo-daily-logins-helper.toml")
 
@@ -127,20 +130,22 @@
         if "COOKIE" in os.environ:
             args.cookie = [os.environ["COOKIE"]]
         if "GAME" in os.environ:
             args.game = [os.environ["GAME"]]
 
     enable_scheduler = False
     account_identifiers = [None for _ in args.game]
+    notification_manager: Optional[NotificationManager] = None
 
     if args.config_file:
         logging.info(f"Found config file at: {args.config_file}")
 
         with open(args.config_file, "rb") as file:
             config_data = tomllib.load(file)
+            logging.debug(dict_prettify(config_data))
 
             # parse config from toml file
             language = config_data.get("config", {}).get("language", None)
 
             if language:
                 args.language = language
 
@@ -148,14 +153,18 @@
 
             if user_agent:
                 args.user_agent = user_agent
 
             enable_scheduler = config_data.get("config", {})\
                 .get("enable_scheduler", False)
 
+            notifications = config_data.get("config", {}).get("notifications", [])
+
+            notification_manager = NotificationManager(notifications)
+
             # parse accounts
             for index, account in enumerate(config_data.get("accounts", [])):
                 game = account.get("game", None)
                 cookie = account.get("cookie", None)
 
                 if not game:
                     logging.error(f"account #{index} has no game selected")
@@ -182,25 +191,31 @@
         )
         exit(1)
 
     if args.user_agent:
         http_set_user_agent(args.user_agent)
 
     if enable_scheduler:
-        run_scheduler(config_data, args.language)
+        run_scheduler(config_data, args.language, notification_manager)
         return
 
     for index, game in enumerate(args.game):
         identifier = f"Account #{index}"
         cookie = args.cookie[index]
 
         if account_identifiers[index]:
             identifier = account_identifiers[index]
 
-        game_perform_checkin(identifier, game, cookie, args.language)
+        game_perform_checkin(
+            identifier,
+            game,
+            cookie,
+            args.language,
+            notification_manager
+        )
 
 
 def has_legacy_environment_variable() -> bool:
     for env_var in ["LANGUAGE", "COOKIE", "GAME"]:
         if env_var in os.environ:
             return True
     return False
```

### Comparing `hoyo-daily-logins-helper-2.2.1/src/scheduler.py` & `hoyo-daily-logins-helper-2.3.0/src/scheduler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 import logging
 from datetime import datetime, timezone, time
 from time import sleep
+from typing import Optional
 
 import pytz
 from scheduler import Scheduler
 
 from src.games import game_perform_checkin
+from src.notifications import NotificationManager
 
 _RESET_TIME = {
     # running this one hour after reset to prevent potential fuckery with
     # timezones
     "hour": 5,
     "minute": 1,
 }
 
 _RESET_TIMES = {
-    "Asia": time(tzinfo=pytz.timezone("Etc/GMT+8"), **_RESET_TIME),
-    "EU": time(tzinfo=pytz.timezone("Etc/GMT+1"), **_RESET_TIME),
-    "NA": time(tzinfo=pytz.timezone("Etc/GMT-5"), **_RESET_TIME),
+    "Asia": time(tzinfo=pytz.timezone("Asia/Shanghai"), **_RESET_TIME),
+    "EU": time(tzinfo=pytz.timezone("CET"), **_RESET_TIME),
+    "NA": time(tzinfo=pytz.timezone("US/Pacific"), **_RESET_TIME),
 }
 
 
-def run_scheduler(config_data: dict, language: str):
+def run_scheduler(
+        config_data: dict,
+        language: str,
+        notifications_manager: Optional[NotificationManager]
+):
     logging.info("Run in scheduler mode")
 
     tz = datetime.now(timezone.utc).astimezone().tzinfo
 
     schedule = Scheduler(tzinfo=tz)
 
     accounts = config_data.get("accounts", [])
@@ -48,23 +54,24 @@
             identifier = f"Account #{index}"
 
         checkin_job = create_checkin_job(
             identifier,
             account.get("game"),
             account.get("cookie"),
             language,
+            notifications_manager,
         )
 
         job = schedule.daily(
             _RESET_TIMES[region],
             checkin_job
         )
 
         due_in_hours = round(
-            job.timedelta(datetime.now(tz=tz)).total_seconds() / 60 / 60,#
+            job.timedelta(datetime.now(tz=tz)).total_seconds() / 60 / 60,
             1
         )
 
         logging.info(
             f"Added account '{identifier}' to scheduler, region: '{region}', "
             f"next fire time in {due_in_hours} hours"
         )
@@ -81,14 +88,21 @@
         sleep(60)
 
 
 def create_checkin_job(
         account_ident: str,
         game: str,
         cookie_str: str,
-        language: str
+        language: str,
+        notification_manager: Optional[NotificationManager]
 ):
     def _checkin_job():
         logging.info(f"Running scheduler for '{account_ident}'...")
-        game_perform_checkin(account_ident, game, cookie_str, language)
+        game_perform_checkin(
+            account_ident,
+            game,
+            cookie_str,
+            language,
+            notification_manager
+        )
 
     return _checkin_job
```

