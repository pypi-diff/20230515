# Comparing `tmp/wireprobe-0.1.9.tar.gz` & `tmp/wireprobe-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireprobe-0.1.9.tar", last modified: Sun May 14 14:37:14 2023, max compression
+gzip compressed data, was "wireprobe-0.2.tar", last modified: Mon May 15 19:37:45 2023, max compression
```

## Comparing `wireprobe-0.1.9.tar` & `wireprobe-0.2.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 14:37:01.000000 wireprobe-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 14:37:14.249445 wireprobe-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-14 14:37:01.000000 wireprobe-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/fabfile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/fabfile/Config/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/Config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/HealthCheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/fabfile/Notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/Notifications/Telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/Notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:37:14.249445 wireprobe-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 14:37:01.000000 wireprobe-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/wireprobe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:45.447915 wireprobe-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 19:37:33.000000 wireprobe-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 19:37:45.447915 wireprobe-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-15 19:37:33.000000 wireprobe-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:37:45.447915 wireprobe-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 19:37:33.000000 wireprobe-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:45.443915 wireprobe-0.2/wireprobe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:33.000000 wireprobe-0.2/wireprobe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:45.447915 wireprobe-0.2/wireprobe/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:45.447915 wireprobe-0.2/wireprobe/app/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-15 19:37:33.000000 wireprobe-0.2/wireprobe/app/Config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:33.000000 wireprobe-0.2/wireprobe/app/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-15 19:37:33.000000 wireprobe-0.2/wireprobe/app/HealthCheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:45.447915 wireprobe-0.2/wireprobe/app/Notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-15 19:37:33.000000 wireprobe-0.2/wireprobe/app/Notifications/Telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:33.000000 wireprobe-0.2/wireprobe/app/Notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:33.000000 wireprobe-0.2/wireprobe/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-15 19:37:33.000000 wireprobe-0.2/wireprobe/fabfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-15 19:37:33.000000 wireprobe-0.2/wireprobe/settings.yml.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:37:45.447915 wireprobe-0.2/wireprobe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 19:37:45.000000 wireprobe-0.2/wireprobe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-15 19:37:45.000000 wireprobe-0.2/wireprobe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:37:45.000000 wireprobe-0.2/wireprobe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 19:37:45.000000 wireprobe-0.2/wireprobe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 19:37:45.000000 wireprobe-0.2/wireprobe.egg-info/top_level.txt
```

### Comparing `wireprobe-0.1.9/LICENSE` & `wireprobe-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wireprobe-0.1.9/README.md` & `wireprobe-0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,59 @@
 # wireprobe
 A Wireguard Probe
 
 ## Installation
 
+### Pypi
+
+```shell
+$ python3 -m pip install wireprobe
+```
+
+and upgrading
+
+```shell
+$ python3 -m pip install wireprobe -U
+```
+
 ### Debian
 
 ```shell
 $ sudo apt install python3-urllib3 python3-requests python3-decorator python3-fabric python3-invoke python3-pyyaml-env-tag
 ```
 
 ### Python pip
 ```shell
 python3 -m pip install -r requiremments
 ```
 
 ## Usage
 
 ```shell
-$ mv fabfile/settings.yml.example fabfile/settings.yml
+$ mv wireprobe/settings.yml.example wireprobe/settings.yml
 ```
 
-Set your configrations in `fabile/settings.yml`
+Set your configrations in `app/settings.yml`
 
 ```shell
+$ cd wireprobe
 $ fab run
 ```
 
+For INFO logs
+
+```shell
+$ cd wireprobe
+$ fab run -l 20
+```
+
 You can also set a different path for settings.yml
 
 ```shell
+$ cd wireprobe
 $ fab run -s /path/to/settings.yml
 ```
 
 ## Help
 
 ```shell
 $ fab --help run
```

### Comparing `wireprobe-0.1.9/fabfile/HealthCheck.py` & `wireprobe-0.2/wireprobe/app/HealthCheck.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,83 @@
 import datetime
+import logging
 import os
 import time
+
 from .Config.Config import Config
 from .Notifications.Telegram import Telegram
 
 
 class HealthCheck:
     """
     HealthCheck class
     """
     is_connected_client_list = {}
     client_list = {}
     interfaces = []
     timeout = 1
     frequency_check = 5
     telegram = None
+    logger = None
 
-    def __init__(self, settings_file=""):
+    def __init__(self, settings_file="", log_level=30):
         """
         Construct HealthCheck Object
         :param settings_file: Path to the setting file
+        :param log_level: verbosity log level
         :return:
         """
+        logging.basicConfig(format='[%(levelname)s] %(asctime)s: %(message)s', level=os.environ.get('VERBOSITY', log_level))
+        self.logger = logging.getLogger(__name__)
         if not settings_file:
-            settings_file = config_path=os.path.join(os.path.dirname(__file__), "settings.yml")
+            settings_file = config_path=os.path.join(os.path.dirname(__file__), "../settings.yml")
         settings = Config.load_yaml_config(config_path=settings_file)
         self.timeout = settings['settings']["timeout"]
         self.frequency_check = settings["settings"]["frequency_check"]
         self.client_list = {v: k for k, v in settings["settings"]["clients"].items()}
         for client in self.client_list:
             self.is_connected_client_list[self.client_list[client]] = False
-        self.telegram = Telegram(settings_file)
+        self.telegram = Telegram(settings_file, self.logger)
         self.interfaces = settings['settings']['interfaces']
-        print(self.client_list)
-        print(self.is_connected_client_list)
+        # Debug content vars
+        self.logger.debug("client_list = {client_list}\n"
+                          "id_connected_client_list = {is_connected_client_list}\n"
+                          "interface_list = {interface_list}\n"
+                          "timeout = {timeout}\n"
+                          "frequency_check = {frequency_check}".format(
+                            client_list=self.client_list,
+                            is_connected_client_list=self.is_connected_client_list,
+                            interface_list=self.interfaces,
+                            timeout=self.timeout,
+                            frequency_check=self.frequency_check))
 
     def check(self):
         """
         Check method
         :return:
         """
 
         while True:
             time.sleep(self.frequency_check)
             for current_interface in self.interfaces:
-                result = os.popen("wg show {} dump | tail -n +2".format(current_interface)).readlines()
+                result = os.popen("wg show {interface} dump | tail -n +2".format(interface=current_interface)).readlines()
 
                 for line in result:
                     result_line_list = line.split("\t")
-                    print(result_line_list[5])
                     if result_line_list[3] not in self.client_list:
                         continue
                     current_client_name = self.client_list[result_line_list[3]]
-                    print("current client : " + current_client_name)
+                    self.logger.info("current client check : {current_client_name}".format(
+                        current_client_name=current_client_name)
+                    )
                     now = datetime.datetime.now()
                     last_seen = datetime.datetime.fromtimestamp(int(result_line_list[4]))
                     d1_ts = time.mktime(now.timetuple())
                     d2_ts = time.mktime(last_seen.timetuple())
                     minutes_diff = (d1_ts - d2_ts) / 60
-                    print(now, last_seen, now - last_seen, minutes_diff)
+                    self.logger.info("Last refreshed handshake : {last_seen}\nLong ago : {diff}".format(last_seen=last_seen, diff=minutes_diff))
                     if minutes_diff > self.timeout and self.is_connected_client_list[current_client_name]:
                         self.is_connected_client_list[current_client_name] = False
                         self.telegram.notify_disconnected(client_name=current_client_name)
                     elif minutes_diff < self.timeout and not self.is_connected_client_list[current_client_name]:
                         self.is_connected_client_list[current_client_name] = True
                         self.telegram.notify_connected(client_name=current_client_name)
```

### Comparing `wireprobe-0.1.9/fabfile/Notifications/Telegram.py` & `wireprobe-0.2/wireprobe/app/Notifications/Telegram.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,52 @@
+import logging
+import os
 import urllib.request
 import urllib.parse
-import os
+
 from ..Config.Config import Config
 
 
 class Telegram:
     """
     Telegram notification class
     """
     connect_alert = "🐉 Wireguard: {client_name} tunnel is up"
     disconnect_alert = "🐉 Wireguard: {client_name} tunnel potentially seems down"
     parse_mode = "MarkdownV2"
     bot_token = ""
     chat_id = ""
     url_notify_telegram = "https://api.telegram.org/bot{bot_token}/sendMessage"
+    logger = None
 
-    def __init__(self, settings_file):
+    def __init__(self, settings_file, logger=None):
         """
         Constructor Telegram
         :param bot_token: The token of the bot
         :param chat_id: The chan telegram id
         """
+        self.logger = logger
         if not settings_file:
             settings = Config.load_yaml_config(config_path=os.path.join(os.path.dirname(__file__), "settings.yml"))
         else:
             settings = Config.load_yaml_config(config_path=settings_file)
         self.bot_token = settings['settings']['telegram']['bot_token']
         self.chat_id = settings['settings']['telegram']['chat_id']
-        print(self.bot_token, self.chat_id)
+        self.logger.debug("bot_token = {bot_token}\n"
+                          "chat_id = {chat_id}".format(bot_token=self.bot_token, chat_id=self.chat_id))
 
     def send_notification(self, message):
         """
         Notify method
         :param message: Message to send to telegram
         :return:
         """
         data = urllib.parse.urlencode({'chat_id': self.chat_id, 'text': message, 'parse_mode': self.parse_mode}).encode('ascii')
         with urllib.request.urlopen(self.url_notify_telegram.format(bot_token=self.bot_token), data) as f:
-            print(f.read().decode('utf-8'))
+            self.logger.info(f.read().decode('utf-8'))
 
     def notify_connected(self, client_name):
         """
         Notify connected method to send message connection to telegram
         :param client_name: Name of the client ti display
         :return:
         """
```

