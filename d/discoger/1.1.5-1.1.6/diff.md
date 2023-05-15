# Comparing `tmp/discoger-1.1.5.tar.gz` & `tmp/discoger-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.1.5.tar", last modified: Mon May  8 22:04:39 2023, max compression
+gzip compressed data, was "discoger-1.1.6.tar", last modified: Mon May 15 10:51:00 2023, max compression
```

## Comparing `discoger-1.1.5.tar` & `discoger-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:04:39.417441 discoger-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 22:04:22.000000 discoger-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-08 22:04:39.417441 discoger-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-08 22:04:22.000000 discoger-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:04:39.417441 discoger-1.1.5/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:04:22.000000 discoger-1.1.5/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 22:04:22.000000 discoger-1.1.5/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-08 22:04:22.000000 discoger-1.1.5/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:04:39.417441 discoger-1.1.5/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 22:04:39.417441 discoger-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-08 22:04:22.000000 discoger-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:51:00.371171 discoger-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 10:50:47.000000 discoger-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-15 10:51:00.371171 discoger-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-15 10:50:47.000000 discoger-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:51:00.371171 discoger-1.1.6/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:50:47.000000 discoger-1.1.6/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-15 10:50:47.000000 discoger-1.1.6/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-05-15 10:50:47.000000 discoger-1.1.6/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:51:00.371171 discoger-1.1.6/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 10:51:00.371171 discoger-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-15 10:50:47.000000 discoger-1.1.6/setup.py
```

### Comparing `discoger-1.1.5/LICENSE` & `discoger-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.1.5/PKG-INFO` & `discoger-1.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.5
+Version: 1.1.6
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.5.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.6.tar.gz
 Description: # Discoger
         
-        Telegram bot for checking if there are new sell in one specific list on Discogs
+        Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
+        
+        ## Usage
+        
+        1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
         
         ## How to use it
         
         ### Installation
         
         Installation is in three steps, the first is getting credentials from Discogs and Telegram.
         You need to create a [Token](https://www.discogs.com/fr/settings/developers).
```

### Comparing `discoger-1.1.5/README.md` & `discoger-1.1.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Discoger
 
-Telegram bot for checking if there are new sell in one specific list on Discogs
+Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
+
+## Usage
+
+1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
 
 ## How to use it
 
 ### Installation
 
 Installation is in three steps, the first is getting credentials from Discogs and Telegram.
 You need to create a [Token](https://www.discogs.com/fr/settings/developers).
```

### Comparing `discoger-1.1.5/discoger/discoger.py` & `discoger-1.1.6/discoger/discoger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python3
 
 import configparser
 import discogs_client
-from yamldb.YamlDB import YamlDB
+import logging
 import feedparser
-import re
-from pathlib import Path
-
 import threading
 import schedule
+import telebot
 import time
-from time import sleep
+import re
 
-import telebot
+from yamldb.YamlDB import YamlDB
+from pathlib import Path
+from time import sleep
 from telebot import types, util
 
-import logging
 logging.basicConfig(format='%(asctime)s %(levelname)s - %(message)s', level=logging.INFO)
 
 home = str(Path.home())
 config_file = Path(home + "/.config/discoger/config.ini")
 database_dir = Path(home + "/.config/discoger/databases")
 discogs_url = 'https://www.discogs.com'
 
@@ -30,15 +29,16 @@
     logging.error("No config file, please create a config file follwing example")
     raise SystemExit()
 
 if not database_dir.exists():
     database_dir.mkdir(parents=True, exist_ok=True)
 
 token = config["telegram"]["token"]
-secret = secret = config["discogs"]["secret"]
+secret = config["discogs"]["secret"]
+disable_unofficial = config["DEFAULT"].getboolean('disable_unofficial', fallback=True)
 bot = telebot.TeleBot(token)
 
 commands = {  # command description used in the "help" command
     '/start': 'Get used to the bot',
     '/help': 'Gives you information about the available commands',
     '/list': 'Show all items in your following list',
     '/delete': 'Delete item from the following list',
@@ -154,28 +154,31 @@
     id_item = message.text
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     db["release_list"].pop(int(id_item))
     db.save()
     bot.send_message(chat_id, "%s is deleted in following list" % (id_item))
 
 
-def get_info(release_id, type_sell):
+def check_sales(release_id, type_sell):
     data_last_sell = dict()
     if type_sell == 'master':
         url = f"{discogs_url}/sell/mplistrss?output=rss&master_id={release_id}&ev=mb&format=Vinyl"
     else:
         url = f"{discogs_url}/sell/mplistrss?output=rss&release_id={release_id}"
     feed = feedparser.parse(url)
     try:
         entry = feed.entries[-1]
         data_last_sell["id"] = re.findall(r'\d+', entry["link"])[0]
         data_last_sell["date"] = entry["updated"]
         data_last_sell["url"] = entry["link"]
         data_last_sell["price"] = re.findall(r'... \d?\d?\d\d.\d\d', entry["summary_detail"]["value"])[0]
-        return data_last_sell
+        if disable_unofficial and len(re.findall('Unofficial', entry["title"])) > 0:
+            return None
+        else:
+            return data_last_sell
     except Exception as e:
         logging.debug("%s: for %s item" % (e, release_id))
         return None
 
 
 def check_discogs(chat_id=None):
     if chat_id:
@@ -193,15 +196,15 @@
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     chat_id = db.get("chat_id")
     for i in range(len(db["release_list"])):
         item = db.search("release_list[%s]" % (str(i)))
         sell_type = item.get("type")
         if sell_type is None:
             sell_type = "release"
-        data_last_sell = get_info(item["release_id"], sell_type)
+        data_last_sell = check_sales(item["release_id"], sell_type)
         if data_last_sell:
             if not item["last_sell"] or (item["last_sell"]["id"] != data_last_sell["id"] and item["last_sell"]["date"] < data_last_sell["date"]):
                 logging.info("New item for %s - %s" % (item["artist"], item["title"]))
                 text = "New release for:\n%s - %s\ndate: %s\nprice: %s\n%s" % (item["artist"], item["title"], data_last_sell["date"], data_last_sell["price"], data_last_sell["url"])
                 bot.send_message(chat_id, text, disable_web_page_preview=False)
                 db["release_list"][i]["last_sell"] = data_last_sell
             else:
```

### Comparing `discoger-1.1.5/discoger.egg-info/PKG-INFO` & `discoger-1.1.6/discoger.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.5
+Version: 1.1.6
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.5.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.6.tar.gz
 Description: # Discoger
         
-        Telegram bot for checking if there are new sell in one specific list on Discogs
+        Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
+        
+        ## Usage
+        
+        1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
         
         ## How to use it
         
         ### Installation
         
         Installation is in three steps, the first is getting credentials from Discogs and Telegram.
         You need to create a [Token](https://www.discogs.com/fr/settings/developers).
```

### Comparing `discoger-1.1.5/setup.py` & `discoger-1.1.6/setup.py`

 * *Files identical despite different names*

