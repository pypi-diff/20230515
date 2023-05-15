# Comparing `tmp/selfcord.py-0.1.6.tar.gz` & `tmp/selfcord.py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.1.6.tar", last modified: Fri May 12 18:58:24 2023, max compression
+gzip compressed data, was "selfcord.py-0.1.7.tar", last modified: Mon May 15 14:34:36 2023, max compression
```

## Comparing `selfcord.py-0.1.6.tar` & `selfcord.py-0.1.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.253287 selfcord.py-0.1.6/selfcord/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.253287 selfcord.py-0.1.6/selfcord/api/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.253287 selfcord.py-0.1.6/selfcord/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/voice/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/selfcord/models/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/selfcord/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/utils/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.253287 selfcord.py-0.1.6/selfcord.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.896771 selfcord.py-0.1.7/selfcord/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.896771 selfcord.py-0.1.7/selfcord/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20670 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.896771 selfcord.py-0.1.7/selfcord/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/voice/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/selfcord/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/selfcord/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.896771 selfcord.py-0.1.7/selfcord.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/tests/test_commands.py
```

### Comparing `selfcord.py-0.1.6/PKG-INFO` & `selfcord.py-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
-Author: Shell of OMEGA
+Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
+Provides-Extra: voice
 
 <div align="center">
 <img src="./logo.png" widht="180" height="180" style="border-radius: 100%;">
 <h1 align="center">SELFCORD</h1>
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.1.6-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.1.7-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
@@ -31,15 +32,15 @@
  - Easy to use with an object oriented design
  - Optimised for both speed and memory
  - Prevents detection of user account automation
  - Clean Documentation
  - Community Support
 
 ## Installation
-Python 3.10 or higher is required
+Python 3.10 or higher is required.
 ```
 pip install selfcord.py
 ```
 
 ## Wiki
 
 Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in regards to documentation and getting started.
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.6 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.7 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
-Author: Shell of OMEGA License: MIT Keywords:
-selfbot,discord,discordapi,discordwrapper Description-Content-Type: text/
-markdown
+Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
+Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.1.6-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.1.7-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
-## Installation Python 3.10 or higher is required ``` pip install selfcord.py
+## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
 responds to a message ("ping!") with another message ("pong"). ```py import
 selfcord token = "insert token" bot = selfcord.Bot() @bot.on("ready") async def
 ready(time): print(f"Connected To {bot.user.name}\n Startup took {time:0.2f}
 seconds") @bot.on("message") async def responder(message): if message.content
 == "ping!": await message.channel.send("pong!") bot.run(token) ``` ## Examples/
```

### Comparing `selfcord.py-0.1.6/README.md` & `selfcord.py-0.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.1.6-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.1.7-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
@@ -21,15 +21,15 @@
  - Easy to use with an object oriented design
  - Optimised for both speed and memory
  - Prevents detection of user account automation
  - Clean Documentation
  - Community Support
 
 ## Installation
-Python 3.10 or higher is required
+Python 3.10 or higher is required.
 ```
 pip install selfcord.py
 ```
 
 ## Wiki
 
 Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in regards to documentation and getting started.
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.1.6-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.1.7-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
-## Installation Python 3.10 or higher is required ``` pip install selfcord.py
+## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
 responds to a message ("ping!") with another message ("pong"). ```py import
 selfcord token = "insert token" bot = selfcord.Bot() @bot.on("ready") async def
 ready(time): print(f"Connected To {bot.user.name}\n Startup took {time:0.2f}
 seconds") @bot.on("message") async def responder(message): if message.content
 == "ping!": await message.channel.send("pong!") bot.run(token) ``` ## Examples/
```

### Comparing `selfcord.py-0.1.6/selfcord/api/errors.py` & `selfcord.py-0.1.7/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/api/events.py` & `selfcord.py-0.1.7/selfcord/api/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from __future__ import annotations
 from time import perf_counter
 from ..models.role import Role
 from ..models import User, Client, Guild, TextChannel, VoiceChannel, DMChannel, GroupChannel, Message
 from aioconsole import aprint
 import asyncio
 from .voice import Voice
+from ..utils import logging
+
+log = logging.getLogger("Event")
 
 class EventHandler:
     '''
     Used to handle discord events
     '''
-    def __init__(self, bot, http):
+    def __init__(self, bot, http, debug=False):
         self._events = {}
         self.http    = http
         self.bot     = bot
+        self.debug = debug
 
     async def handle_ready(self, data: dict, user: Client, http):
         """Handles what happens when the ready event is fired, when the bot first connects
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
@@ -270,14 +274,54 @@
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         if data['channel_id'] != None:
             self.session_id = data['session_id']
 
+    async def handle_presence_update(self, data: dict, user: Client, http):
+        """Handles the presence updating
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
+        PLAYING = 0
+        STREAMING = 1
+        LISTENING = 2
+        WATCHING = 3
+        CUSTOM = 4
+
+        last_modified = data.get("last_modified")
+        status = data.get("status")
+        check = data.get("user").get("username")
+        if check != None:
+            user = User(data.get("user"), self.bot, self.http)
+        else:
+            user = data.get("user").get("id")
+
+        client_status = data.get("client_status")
+        activity = data.get("activities")
+        activities = []
+        if activity != None:
+            for activity in activity:
+                type = activity.get("type")
+                if type == PLAYING:
+                    type = "PLAYING"
+                elif type == STREAMING:
+                    type = "STREAMING"
+                elif type == WATCHING:
+                    type == "WATCHING"
+                elif type == 4:
+                    type = "CUSTOM"
+                activities.append({"Type": type, "Name": activity.get("name")})
+
+        await self.bot.emit('presence_update', user, status, last_modified, client_status, activities)
+
     async def handle_voice_server_update(self, data: dict, user: Client, http):
         """Handles the voice server updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
@@ -285,20 +329,23 @@
         self.token = data['token']
         self.endpoint = data['endpoint']
         if data['guild_id'] != None:
             self.server_id = data['guild_id']
         else:
             self.server_id = data['channel_id']
         await asyncio.sleep(1)
-        self.voice = Voice(self.session_id, self.token, self.endpoint, self.server_id, self.bot)
+        self.voice = Voice(self.session_id, self.token, self.endpoint, self.server_id, self.bot, debug=self.debug)
         await self.voice_start(self.voice)
 
     async def voice_start(self, voice: Voice):
         asyncio.create_task(voice.start())
         setattr(self.bot, "voice", self.voice)
+        if self.debug:
+            log.debug("Voice attribute created")
+            log.info(f"Created voice attribute with Session ID: {self.session_id} Endpoint: {self.endpoint}")
```

### Comparing `selfcord.py-0.1.6/selfcord/api/gateway.py` & `selfcord.py-0.1.7/selfcord/api/gateway.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 import asyncio
 import websockets
-from aioconsole import aprint
 import json
+import os
 import time
 import zlib
 from .events import EventHandler
 from .errors import ReconnectWebsocket
 from selfcord.models.client import Client
 import requests
 from traceback import format_exception
+from ..utils import logging
 
-class Activity:
+log = logging.getLogger("Gateway")
 
+class Activity:
     @staticmethod
     def Game(name: str, details: str, state: str, buttons: dict, application_id: str, key: str) -> dict[str, int]:
         """Method to generate activity dict for the "Playing ..." payload
 
         Args:
             name (str): Name of the activity
             details (str): Details of the activity
@@ -262,16 +264,16 @@
     RECONNECT          = 7
     REQUEST_MEMBERS    = 8
     INVALIDATE_SESSION = 9
     HELLO              = 10
     HEARTBEAT_ACK      = 11
     GUILD_SYNC         = 12
 
-    def __init__(self, http, show_heartbeat=False):
-        self.show_heartbeat = show_heartbeat
+    def __init__(self, http, debug=False):
+        self.debug = debug
         self.http = http
         self.zlib = zlib.decompressobj()
         self.zlib_suffix = b'\x00\x00\xff\xff'
         self.last_ack = time.perf_counter()
         self.last_send = time.perf_counter()
         self.latency = float('inf')
         self.alive = False
@@ -292,20 +294,20 @@
             op      = item.get('op') # Op code
             data    = item.get('d') # Data
             event   = item.get('t') # The event
 
 
             if  op == self.RECONNECT:
                 await self.close()
-                raise ReconnectWebsocket('Connection was closed.')
+                log.error("Reconnect websocket")
 
             elif op == self.INVALIDATE_SESSION:
                 if data:
                     await self.close()
-                    raise ReconnectWebsocket('Connection was closed.')
+                    log.error("Session Invalidated")
 
             elif op == self.HELLO:
                 # Begins heartbeat and sends identify if this op is received
                 interval = data['heartbeat_interval'] / 1000.0
                 await self.identify()
                 asyncio.create_task(self.heartbeat(interval))
 
@@ -358,14 +360,17 @@
                 "activities": [activity],
                 "status": status.lower(),
                 "afk": afk
             },
         }
 
         await self.send_json(payload)
+        if self.debug:
+            log.debug("Began rich presence")
+            log.info(f"{activity}")
 
 
 
     async def lazy_chunk(self, guild_id: str, channel_id: str, amount: int):
         '''Sends lazy guild request to gather current online members
 
         Args:
@@ -386,34 +391,42 @@
                     'typing': True,
                     'channels': {channel_id:item}
                 }
             }
 
             await self.send_json(payload)
 
+        if self.debug:
+            log.debug("Finished guild lazy chunking")
+            log.info(f"Subscription to GUILD: {guild_id} with CHANNEL: {channel_id}")
+
 
     async def send_json(self, payload: dict):
         '''Send json to the gateway
 
         Args:
             payload (dict): Valid payload to send to the gateway
         '''
         await self.ws.send(json.dumps(payload))
 
     async def connect(self):
         '''Connect to discord gateway
         '''
         self.ws = await websockets.connect('wss://gateway.discord.gg/?encoding=json&v=9&compress=zlib-stream', origin='https://discord.com', max_size=None)
         self.alive = True
+        if self.debug:
+            log.debug("Established connection to Discord Gateway")
 
     async def close(self):
         '''Close the connection to discord gateway
         '''
         self.alive= False
         await self.ws.close()
+        if self.debug:
+            log.debug("Closed connection to discord gateway")
 
     async def identify(self):
         '''Identify to gateway, uses amazing mobile client spoof
         '''
         payload = {
             'op': 2,
             'd': {
@@ -424,34 +437,38 @@
                     '$device': 'Discord Android',
                     '$referrer': '',
                     '$referring_domain': ''
                 },
             }
         }
         await self.send_json(payload)
+        if self.debug:
+            log.debug("Sent identify payload")
+            log.info(f"Idenitified with {self.token} under Discord Android")
 
 
 
     async def heartbeat(self, interval):
         '''Heartbeat for gateway to maintain connection
 
         Args:
             interval (int): Interval between sends
         '''
-        await aprint(f'Hearbeat loop has began with the interval of {interval} seconds!')
+        log.info(f'Hearbeat loop has began with the interval of {interval} seconds!')
         heartbeatJSON = {
             'op': 1,
             'd': time.time()
         }
         while True:
             await asyncio.sleep(interval)
             await self.send_json(heartbeatJSON)
             self.last_send = time.perf_counter()
-            if self.show_heartbeat:
-                await aprint('Sent Beat')
+            if self.debug:
+                log.debug('Sent heartbeat')
+                log.info(f"Delay since last heartbeat {self.latency:0.2f}ms")
 
     async def heartbeat_ack(self):
         '''Whenever heartbeat ack is sent, logs the time between last send of heartbeat json and receive of the ack
         '''
         self.last_ack = time.perf_counter()
         self.latency = self.last_ack - self.last_send
 
@@ -459,31 +476,33 @@
         '''Start discord gateway connection
 
         Args:
             token (str): User token
             user (Client): User client
             bot (_type_): Bot class
         '''
-        self.handler = EventHandler(bot, self.http)
+        self.handler = EventHandler(bot, self.http, self.debug)
         self.bot = bot
 
         await self.bot.inbuilt_commands() # In built commands very cool
 
         self.user = user
         self.token = token
 
         await self.connect()
         while self.alive:
             try: await self.recv_msg()
             except KeyboardInterrupt:
-                await aprint('Shutting down...')
+                log.critical('Shutting down...')
                 await self.close()
             except Exception as e:
                 error = "".join(format_exception(e, e, e.__traceback__))
                 await self.bot.emit("error", error)
+                if self.debug:
+                    log.error(f"Websocket Unexpectedly closed\n{error}")
                 await self.close()
 
     async def video_call(self, channel: str, guild=None):
         """Initiates a discord video call
 
         Args:
             channel (str): Channel ID
@@ -497,16 +516,21 @@
                 "preferred_region": "rotterdam",
                 "self_mute": False,
                 "self_deaf": False,
                 "self_video": True,
             }
         }
         await self.send_json(payload)
+        if self.debug:
+            log.debug("Initiated video call")
+            log.info(f"Began video call to GUILD: {guild} and CHANNEL: {channel}")
         if guild == None:
             await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
+            if self.debug:
+                log.debug("Sent Ring")
 
 
     async def call(self, channel: str, guild=None):
         """Initiates a discord call
 
         Args:
             channel (str): Channel ID
@@ -520,16 +544,22 @@
                 "preferred_region": "rotterdam",
                 "self_mute": False,
                 "self_deaf": False,
                 "self_video": False,
             }
         }
         await self.send_json(payload)
+        if self.debug:
+            log.debug("Initiated call")
+            log.info(f"Began call to GUILD: {guild} and CHANNEL: {channel}")
         if guild == None:
             await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
+            if self.debug:
+                log.debug("Sent Ring")
+
 
 
     async def stream_call(self, channel: str, guild=None):
         """Initiates a discord stream call
 
         Args:
             channel (str): Channel ID
@@ -542,32 +572,42 @@
                 "guild_id": guild,
                 "channel_id": channel,
                 "preferred_region": "rotterdam",
                 "type": type
             }
         }
         await self.send_json(payload)
+        if self.debug:
+            log.debug("Initiated call")
+            log.info(f"Began call to GUILD: {guild} and CHANNEL: {channel}")
         if guild == None:
+
             await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
 
             payload = {
                 "op": 22,
                 "d": {
                     "stream_key": f"call:{channel}:{self.user.id}",
                     "paused": False
                 }
             }
+            if self.debug:
+                log.debug("Initiated streaming")
+                log.info(f"Began stream to CHANNEL: {channel}")
         else:
             payload = {
                 "op": 22,
                 "d": {
                     "stream_key": f"guild:{guild}:{channel}:{self.user.id}",
                     "paused": False
                 }
             }
+            if self.debug:
+                log.debug("Initiated streaming")
+                log.info(f"Began stream to GUILD: {guild} and CHANNEL: {channel}")
 
         await self.send_json(payload)
 
 
 
 
     async def leave_call(self):
@@ -580,14 +620,21 @@
                 "channel_id": None,
                 "self_mute": False,
                 "self_deaf": False,
                 "self_video": False,
             }
         }
         await self.send_json(payload)
+        if self.debug:
+            log.debug("Left Voice call")
+        if hasattr(self.bot, "voice"):
+            await self.bot.voice.close()
+            delattr(self.bot, "voice")
+        if self.debug:
+            log.info("Voice attribute for bot has been deleted")
```

### Comparing `selfcord.py-0.1.6/selfcord/bot.py` & `selfcord.py-0.1.7/selfcord/bot.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 import json
 from .api import gateway, http, Activity
 import inspect
 from .models import Client, TextChannel, GroupChannel, DMChannel, VoiceChannel, Guild, User
 from collections import defaultdict
 from aioconsole import aprint, aexec
 import time
-from .utils import Command, CommandCollection, Context, ExtensionCollection, Extension, Event
+from .utils import Command, CommandCollection, Context, ExtensionCollection, Extension, Event, logging
 import random
 import contextlib
 from traceback import format_exception
 import io
 from functools import partial
 import importlib
 import aiohttp
 
 
+log = logging.getLogger("Bot")
 class Bot:
-    def __init__(self, show_beat: bool = False, prefixes: list = ["s!"], inbuilt_help=True, userbot=False, eval=False) -> None:
+    def __init__(self, debug: bool = False, prefixes: list = ["s!"], inbuilt_help=True, userbot=False, eval=False) -> None:
         self.inbuilt_help= inbuilt_help
-        self.show_beat = show_beat
+        self.debug = debug
         self.token = None
-        self.http = http()
+        self.http = http(debug)
         self.t1 = time.perf_counter()
-        self.gateway = gateway(self.http, self.show_beat)
+        self.gateway = gateway(self.http, self.debug)
         self._events = defaultdict(list)
         self.commands = CommandCollection()
         self.prefixes = prefixes if isinstance(prefixes, list) else [prefixes]
         self.extensions = ExtensionCollection()
         self.user = None
         self.eval = eval
         self.userbot = userbot
@@ -42,14 +43,17 @@
         """
         self.token = token
 
         async def runner():
             data = await self.http.static_login(token)
             self.user = Client(data)
             await self.gateway.start(token, self.user, self)
+            if self.debug:
+                log.debug("Started Bot")
+                log.info(f"Logged in as {self.user}")
 
         try:
             asyncio.run(runner())
         except KeyboardInterrupt:
             pass
 
     @property
@@ -164,15 +168,15 @@
 
         Args:
             event (str): The event to check for
         """
 
         def decorator(coro):
             if not inspect.iscoroutinefunction(coro):
-                raise RuntimeWarning("Faulure")
+                log.error("Not a coroutine")
             else:
                 self._events[event].append(Event(name=event, coro=coro, ext=None))
 
                 def wrapper(*args, **kwargs):
 
                     result = self._events[event].append(Event(name=event, coro=coro, ext=None))
 
@@ -218,15 +222,15 @@
         """
         if isinstance(aliases, str):
             aliases = [aliases]
 
         def decorator(coro):
             name = coro.__name__
             if not inspect.iscoroutinefunction(coro):
-                raise RuntimeWarning("Not an async function!")
+                log.error("Not a coroutine")
             else:
                 cmd = Command(name=name, description=description, aliases=aliases, func=coro)
                 self.commands.add(cmd)
             return cmd
 
         return decorator
 
@@ -242,15 +246,15 @@
         Raises:
             RuntimeWarning: If you suck and don't use a coroutine
         """
         if isinstance(aliases, str):
             aliases = [aliases]
         name = coro.__name__
         if not inspect.iscoroutinefunction(coro):
-            raise RuntimeWarning("Not an async function!")
+            log.error("Not a coroutine")
         else:
             cmd = Command(name=name, description=description, aliases=aliases, func=coro)
             self.commands.add(cmd)
 
     async def process_commands(self, msg):
         """
         What is called in order to actually get command input and run commands
@@ -271,42 +275,46 @@
 
         Raises:
             ModuleNotFoundError: If you suck and don't know the name of what you want to load
         """
         try:
             name = importlib.util.resolve_name(name, None)
         except Exception as e:
-            raise ModuleNotFoundError(f"{name} does not exist")
+            error = "".join(format_exception(e, e, e.__traceback__))
+            log.error(f"Could not resolve extension name\n{error}")
 
         spec = importlib.util.find_spec(name)
 
         lib = importlib.util.module_from_spec(spec)
 
         try:
             spec.loader.exec_module(lib)
         except Exception as e:
-            raise ModuleNotFoundError(f"Spec could not be loaded {e}")
+            error = "".join(format_exception(e, e, e.__traceback__))
+            log.error(f"Spec could not be loaded\n{error}")
         try:
             ext = getattr(lib, 'Ext')
         except Exception as e:
-            raise ModuleNotFoundError(f"Extension does not exist {e}")
+            error = "".join(format_exception(e, e, e.__traceback__))
+            log.error(f"Extension does not exist\n{error}")
 
         # Creates an Extension - ext in this case refers to the Ext class used for initialisation
         ext = Extension(name=ext.name, description=ext.description, ext=ext(self), _events=ext._events)
         self.extensions.add(ext)
         try:
             for name, event in ext._events.items():
                 for ext_event in event:
                     self._events[name].append(Event(name=name, coro=ext_event.coro, ext=ext.ext))
-
-
+            if self.debug:
+                log.debug("Loaded Extension")
+                log.info(f"Loaded Extension {ext.name} to Bot")
 
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
-            print(error)
+            log.error(f"Failed to load extension events\n{error}")
 
 
 
 
 
 
 
@@ -364,14 +372,17 @@
         return user
 
     async def create_guild(self, name: str, icon_url: str = None, template: str = "2TffvPucqHkN"):
         """Creates a guild
         """
         image = await self.http.encode_image(icon_url)
         await self.http.request(method="post", endpoint=f"/guilds", headers={"origin": "https://discord.com", "referer": "https://discord.com/channels/@me"}, json={"name": name, "icon": image, "template": template })
+        if self.debug:
+            log.debug("Finished Creating Guild")
+            log.info(f"Created Guild NAME: {name} TEMPLATE: {template} ICON: {icon_url}")
 
 
     async def add_friend(self, user_id: str):
         """
         Function to add a specific user as a friend.
 
         Args:
@@ -381,24 +392,29 @@
             No return value.
         """
 
         await self.http.request(method="put", endpoint=f"/users/@me/relationships/{user_id}",
                                 headers={"origin": "https://discord.com",
                                          "referer": f"https://discord.com/channels/@me/{random.choice(self.user.private_channels).id}"},
                                 json={})
+        if self.debug:
+            log.debug("Sent Friend request")
+            log.info(f"Sent Friend request to {user_id}")
 
     async def edit_profile(self, bio: str = None, accent: int = None):
         """ Edits user profile
         """
         fields = {}
         if bio != None:
             fields['bio'] = bio
         if accent != None:
             fields['accent'] = accent
         await self.http.request(method="patch", endpoint=f"/users/@me/profile", json=fields)
+        if self.debug:
+            log.debug("Finished Edit profile")
 
     async def change_pfp(self, avatar_url=None):
         """Disclaimer: This may phone lock your account :(
 
         Args:
             avatar_url (str): URL of image
 
@@ -407,15 +423,17 @@
         """
         if avatar_url != None:
             image = await self.http.encode_image(avatar_url)
             await self.http.request(method="patch", endpoint="/users/@me", headers={"origin": "https://discord.com",
                                                                                     "referer": "https://discord.com/channels/@me"},
                                     json={'avatar': image})
         else:
-            raise TypeError("Avatar url not specified")
+            log.error("Avatar URL not specified")
+        if self.debug:
+            log.debug("Finished changing avatar")
 
     async def create_dm(self, recipient_id: int):
         """
         Function to create new DM Channel with other user. Can be used with bots too.
 
         Args:
             recipient_id (snowflake): ID of recipient - Has to be user or bot ID
@@ -425,28 +443,30 @@
 
         Returns:
             DMChannel object
         """
         if recipient_id is not None:
             data = await self.http.request(method="post", endpoint="/users/@me/channels",
                                            json={"recipient_id": recipient_id})
+            if self.debug:
+                log.debug("Created DM Channel")
             return DMChannel(data, bot=self, http=self.http)
         else:
-            raise TypeError("Recipient ID not specified")
+            log.error("Recipient ID not specified")
 
     async def redeem_nitro(self, code: str):
         """Helper function to redeem nitro
 
         Args:
             code (str): Nitro code
         """
         async with aiohttp.ClientSession() as session:
             async with session.post(f"https://canary.discord.com/api/v9/entitlements/gift-codes/{code}/redeem", headers={"authorization": f"{self.token}", "user-agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/112.0", "content-type":"application/json"}, json={}) as resp:
                 j = await resp.json()
-                await aprint(j, resp.status)
+                log.info(F"Status: {resp.status} Nitro Redeem response: {j}")
 
 
 
 
     async def change_hypesquad(self, house: "str"):
         """Helper function to change hypesquad
 
@@ -455,20 +475,26 @@
         """
         if house.lower() == "bravery":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 1})
         if house.lower() == "brilliance":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 2})
         if house.lower() == "balance":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 3})
+        if self.debug:
+            log.debug("Finished changing hypesquad")
+            log.info(f"Changed hypesquad to {house}")
 
     async def change_presence(self, status: str, afk: bool, activity: dict):
         """Change discord activity presence
 
         Args:
             status (str): Online, Offline, Dnd, Invisible
             afk (bool): True or False
             activity (dict): Selfcord.Activity method.
         """
         await self.gateway.change_presence(status, afk, activity=activity)
+        if self.debug:
+            log.debug("Finished changing presence")
+            log.info(f"Changed Status to {status}, AFK to {afk}")
```

### Comparing `selfcord.py-0.1.6/selfcord/models/channel.py` & `selfcord.py-0.1.7/selfcord/models/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 from .message import Message
 import time
 from .user import User
 from .webhook import Webhook
 import asyncio
-
+from ..utils import logging
 from selfcord.models import message
+from traceback import format_exception
 
+log = logging.getLogger("Channel")
 
 class Messageable:
     """Parent class specific for those classes that include a textchat for sending messages.
     """
     def __init__(self, http, bot) -> None:
         self.http = http
         self.bot = bot
@@ -298,17 +300,16 @@
             payload['position'] = position
         if topic is not None and topic != "":
             payload['topic'] = topic
 
         try:
             await self.http.request(method="patch", endpoint=f"/channels/{self.id}", json=payload)
         except Exception as e:
-            from traceback import format_exception
             error = "".join(format_exception(e, e, e.__traceback__))
-            return error
+            log.error(f"Could not edit channel \n{error}")
 
     async def create_webhook(self, name: str = None, avatar_url: str = None) -> Webhook:
         """
         Creates a webhook in the specified channel
 
         Args:
             name (str, optional): Name of the webhook. Defaults to None.
@@ -320,15 +321,15 @@
         Raises:
             NameError: Name is required
         """
         fields = {}
         if name != None:
             fields['name'] = name
         else:
-            raise TypeError("Name is required...")
+            log.error("Name is required")
         if avatar_url != None:
             data = await self.http.encode_image(avatar_url)
             fields['avatar'] = data
         data = await self.http.request(method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields)
         webhook = Webhook(data, self.bot, http=self.http)
         self.webhooks.append(webhook)
         return webhook
@@ -388,15 +389,15 @@
             NameError: Name is required
         """
 
         fields = {}
         if name != None:
             fields['name'] = name
         else:
-            raise TypeError("Name is required...")
+            log.error("Name is required...")
         if avatar_url != None:
             data = await self.http.encode_image(avatar_url)
             fields['avatar'] = data
         data = await self.http.request(method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields)
         webhook = Webhook(data, self.bot, self.http)
         self.webhooks.append(webhook)
         return webhook
```

### Comparing `selfcord.py-0.1.6/selfcord/models/client.py` & `selfcord.py-0.1.7/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/models/emoji.py` & `selfcord.py-0.1.7/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/models/guild.py` & `selfcord.py-0.1.7/selfcord/models/guild.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/models/member.py` & `selfcord.py-0.1.7/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/models/message.py` & `selfcord.py-0.1.7/selfcord/models/message.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/models/permission.py` & `selfcord.py-0.1.7/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/models/role.py` & `selfcord.py-0.1.7/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/models/user.py` & `selfcord.py-0.1.7/selfcord/models/user.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/models/webhook.py` & `selfcord.py-0.1.7/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.6/selfcord/utils/command.py` & `selfcord.py-0.1.7/selfcord/utils/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 import inspect
 import re
 from collections import defaultdict
+from .logging import logging
+from traceback import format_exception
 
+log = logging.getLogger("Commands")
 
 class Extension:
     """Extension object. Discord.py equivalent of cogs, a helper system to help manage and organise code into multiple files
     """
     def __init__(self, **kwargs):
         self.name: str | None = kwargs.get("name")
         self.description: str | None = kwargs.get('description')
@@ -60,33 +63,33 @@
             ext (Extension): Extension to add
 
         Raises:
             ValueError: Extension must be subclass of extension
             ValueError: A name or alias is already registered
         """
         if not isinstance(ext, Extension):
-            raise ValueError('ext must be a subclass of Extension')
+            log.error(f"ext is not an Extension or subclass of Extension")
         if self._is_already_registered(ext):
-            raise ValueError('A name or alias is already registered')
+            log.error("Name or Alias is already registered")
         # Add extension to the collection
         self.extensions[ext.name] = ext
 
     def get(self, alias: str) -> Extension:
         """Get an extension
 
         Args:
             alias (str): Name of the extension
 
         Returns:
             Extension: Extension obtained
         """
         try:
             return self.extensions[alias]
-        except KeyError:
-            pass
+        except KeyError as e:
+            log.error(f"{e}")
         for extension in self.extensions:
             if extension.name in extension.aliases:
                 return extension
 
 
 
 class Command:
@@ -139,15 +142,15 @@
         Args:
             collection (CommandCollection): Collection instance
 
         Raises:
             ValueError: Collection must be subclass of CommandCollection
         """
         if not isinstance(collection, CommandCollection):
-            raise ValueError('collection must be a subclass of CommandCollection')
+            log.error("collection is not a subclass of CommandCollection")
         for item in collection:
             self.commands[item.name] = item
             self.recent_commands[item.name] = item
 
     def add(self, cmd: Command):
         """Add a Command to the collection
 
@@ -155,17 +158,17 @@
             cmd (Command): Command to be added
 
         Raises:
             ValueError: cmd must be a subclass of Command
             ValueError: Name or Alias is already registered
         """
         if not isinstance(cmd, Command):
-            raise ValueError('cmd must be a subclass of Command')
+            log.error("cmd must be a subclass of Command")
         if self._is_already_registered(cmd):
-            raise ValueError('A name or alias is already registered')
+            log.error("Command Name or Alias is already registered")
         self.commands[cmd.name] = cmd
         self.recent_commands[cmd.name] = cmd
 
     def recents(self):
         """View commands recently acquired
 
         Yields:
@@ -192,16 +195,16 @@
             alias (str): Name of the command
 
         Returns:
             Command: Command obtained
         """
         try:
             return self.commands[alias]
-        except KeyError:
-            pass
+        except KeyError as e:
+            log.error(f"{e}")
         for command in self.commands:
             if alias in command.aliases:
                 return command
 class Event:
     """Event object
     """
     def __init__(self, name, coro, ext) -> None:
@@ -236,15 +239,15 @@
         """
         if isinstance(aliases, str):
             aliases = [aliases]
 
         def decorator(coro):
             name = coro.__name__
             if not inspect.iscoroutinefunction(coro):
-                raise RuntimeWarning("Not an async function!")
+                log.error("Not a coroutine")
             else:
                 cmd = Command(name=name, description=description, aliases=aliases, func=coro)
                 cls.commands.add(cmd)
 
             return cmd
 
         return decorator
@@ -255,15 +258,15 @@
 
         Args:
             event (str): The event to check for
         """
 
         def decorator(coro):
             if not inspect.iscoroutinefunction(coro):
-                raise RuntimeWarning("Faulure")
+                log.error("Not a coroutine")
             else:
                 eve = Event(name=event, coro=coro, ext=cls)
                 cls._events[event].append(eve)
 
                 def wrapper(*args, **kwargs):
                     result = cls._events[event].append(eve)
                     return result
@@ -285,15 +288,15 @@
         Raises:
             RuntimeWarning: If you suck and don't use a coroutine
         """
         if isinstance(aliases, str):
             aliases = [aliases]
         name = coro.__name__
         if not inspect.iscoroutinefunction(coro):
-            raise RuntimeWarning("Not an async function!")
+            log.error("Not a coroutine")
         else:
 
 
             cmd = Command(name=name, description=description, aliases=aliases, func=coro, ext=cls)
             cls.commands.add(cmd)
 
 
@@ -379,15 +382,15 @@
 
     def get_converter(self, param):
         if param.annotation is param.empty:
             return str
         if callable(param.annotation):
             return param.annotation
         else:
-            raise ValueError('Parameter annotation must be callable')
+            log.error("Parameter annotation must be callable")
 
     def convert(self, param, value):
         """Attempts to turn x value in y value, using get_converter func for the values
 
         Args:
             param (_type_): function parameter
             value (_type_): value in message
@@ -474,16 +477,20 @@
             if func.__code__.co_varnames[0] == "self":
 
                 args.insert(0, self.extension)
                 args.insert(1, self)
             else:
 
                 args.insert(0, self)
+        try:
+            await func(*args, **kwargs)
+        except Exception as e:
+            error = "".join(format_exception(e, e, e.__traceback__))
+            log.error(f"Could not run command \n{error}")
 
-        await func(*args, **kwargs)
 
 
 
     async def reply(self, content: str, tts=False):
         """Helper function to reply to your own message containing the command
 
         Args:
```

### Comparing `selfcord.py-0.1.6/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.1.7/selfcord.py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
-Author: Shell of OMEGA
+Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
+Provides-Extra: voice
 
 <div align="center">
 <img src="./logo.png" widht="180" height="180" style="border-radius: 100%;">
 <h1 align="center">SELFCORD</h1>
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.1.6-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.1.7-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
@@ -31,15 +32,15 @@
  - Easy to use with an object oriented design
  - Optimised for both speed and memory
  - Prevents detection of user account automation
  - Clean Documentation
  - Community Support
 
 ## Installation
-Python 3.10 or higher is required
+Python 3.10 or higher is required.
 ```
 pip install selfcord.py
 ```
 
 ## Wiki
 
 Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in regards to documentation and getting started.
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.6 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.7 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
-Author: Shell of OMEGA License: MIT Keywords:
-selfbot,discord,discordapi,discordwrapper Description-Content-Type: text/
-markdown
+Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
+Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.1.6-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.1.7-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
-## Installation Python 3.10 or higher is required ``` pip install selfcord.py
+## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
 responds to a message ("ping!") with another message ("pong"). ```py import
 selfcord token = "insert token" bot = selfcord.Bot() @bot.on("ready") async def
 ready(time): print(f"Connected To {bot.user.name}\n Startup took {time:0.2f}
 seconds") @bot.on("message") async def responder(message): if message.content
 == "ping!": await message.channel.send("pong!") bot.run(token) ``` ## Examples/
```

### Comparing `selfcord.py-0.1.6/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.1.7/selfcord.py.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 selfcord/models/message.py
 selfcord/models/permission.py
 selfcord/models/role.py
 selfcord/models/user.py
 selfcord/models/webhook.py
 selfcord/utils/__init__.py
 selfcord/utils/command.py
+selfcord/utils/logging.py
 tests/test_commands.py
```

### Comparing `selfcord.py-0.1.6/setup.py` & `selfcord.py-0.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 if __name__ == "__main__":
+
     this_directory = Path(__file__).parent
     long_description = ( this_directory /"README.md").read_text()
     setup(
         name="selfcord.py",
         packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models', 'selfcord.api.voice']),
-        version="0.1.6",
+        version="0.1.7",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
-        author="Shell of OMEGA",
+        author="Shell",
+        extras_require={"voice": ["pynacl==1.5.0","opuslib==3.0.1"]},
         license="MIT",
         install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "requests"],
         setup_requires=['pytest-runner'],
         tests_require=['pytest'],
         test_suite='tests',
         keywords=["selfbot", "discord", "discordapi", "discordwrapper"],
         long_description=long_description,
```

