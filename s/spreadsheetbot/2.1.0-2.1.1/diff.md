# Comparing `tmp/spreadsheetbot-2.1.0.tar.gz` & `tmp/spreadsheetbot-2.1.1.tar.gz`

## Comparing `spreadsheetbot-2.1.0.tar` & `spreadsheetbot-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/Makefile
--rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/basic/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/basic/drive.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/basic/errors.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/basic/handlers.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/basic/log.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/__init__.py
--rw-r--r--   0        0        0     9520 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/abstract.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/groups.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/i18n.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/keyboard.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/log.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/notifications.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/registration.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/report.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/settings.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/switch.py
--rw-r--r--   0        0        0    20960 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/users.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/Makefile
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/drive.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/errors.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/handlers.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/log.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/__init__.py
+-rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/abstract.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/groups.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/i18n.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/keyboard.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/log.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/notifications.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/registration.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/report.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/settings.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/switch.py
+-rw-r--r--   0        0        0    20944 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/users.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/PKG-INFO
```

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/__init__.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Settings,
     Groups,
     Users,
     Registration,
     Report,
     Keyboard,
     Notifications,
-    PerfomNotifications
+    PerformAndScheldueNotifications
 )
 
 from spreadsheetbot.basic import Log, INFO, DEBUG
 from spreadsheetbot.basic.handlers import ErrorHandlerFun, ChatMemberHandlerFun
 
 UPDATE_GROUP_USER_REQUEST  = 0
 UPDATE_GROUP_GROUP_REQUEST = 2
@@ -57,23 +57,23 @@
         await Notifications.async_init(self.sheets_secret, self.sheets_link)
 
         bot: Bot = app.bot
         await bot.set_my_commands([(HELP_COMMAND, Settings.help_command_description)])
 
         await LogSheet.write(None, "Started an application")
 
-        Switch.update(app)
-        Settings.update(app)
-        Groups.update(app)
-        Users.update(app)
-        Registration.update(app)
-        Report.update(app)
-        Keyboard.update(app)
-        Notifications.update(app)
-        PerfomNotifications(app)
+        Switch.scheldue_update(app)
+        Settings.scheldue_update(app)
+        Groups.scheldue_update(app)
+        Users.scheldue_update(app)
+        Registration.scheldue_update(app)
+        Report.scheldue_update(app)
+        Keyboard.scheldue_update(app)
+        Notifications.scheldue_update(app)
+        PerformAndScheldueNotifications(app)
 
     async def post_shutdown(self, app: Application) -> None:
         await LogSheet.write(None, "Stopped an application")
 
     def run_polling(self):
         Log.info("Starting...")
         app = ApplicationBuilder() \
```

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/basic/drive.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/basic/drive.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/basic/handlers.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/basic/handlers.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/basic/log.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/basic/log.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/__init__.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,36 +11,48 @@
 
 import asyncio
 from telegram.ext import Application
 from telegram.constants import ParseMode
 
 from spreadsheetbot.basic.log import Log
 
-def PerfomNotifications(app: Application):
+def PerformAndScheldueNotifications(app: Application):
     app.create_task(
-        _perform_notification(app),
+        _perform_notifications(app),
         {
-            'action': 'Perform notification'
+            'action': 'Perform first notifications'
         }
     )
+    ScheldueNotifications(app)
 
-async def _perform_notification(app: Application):
+def ScheldueNotifications(app: Application) -> None:
+    app.create_task(
+        _scheldue_and_perform_notification(app),
+        {
+            'action': 'Perform scheldued notifications'
+        }
+    )
+
+async def _scheldue_and_perform_notification(app: Application) -> None:
+    await asyncio.sleep(Settings.notifications_update_time)
+    ScheldueNotifications(app)
+    await _perform_notifications(app)
+
+async def _perform_notifications(app: Application) -> None:
     Log.info("Start performing notification")
     for idx,row in Notifications.as_df.loc[Notifications.selector_to_notify()].iterrows():
-        await Users.send_notification_to_all_users(
+        Users.send_notification_to_all_users(
             app, row.text_markdown, ParseMode.MARKDOWN, row.send_picture, row.state, row.condition
         )
         if row.state == "":
-            await Groups.send_to_all_normal_groups(app, row.text_markdown, ParseMode.MARKDOWN, row.send_picture)
+            Groups.send_to_all_normal_groups(app, row.text_markdown, ParseMode.MARKDOWN, row.send_picture)
         admin_group_text = \
             Settings.notification_admin_groups_template.format(message=row.text_markdown) if row.condition == None \
             else Settings.notification_admin_groups_condition_template.format(message=row.text_markdown, condition=row.condition)
-        await Groups.send_to_all_admin_groups(
+        Groups.send_to_all_admin_groups(
             app, 
             admin_group_text,
             ParseMode.MARKDOWN,
             row.send_picture
         )
         await Notifications.set_done(idx)
-    Log.info("Done performing notification")
-    await asyncio.sleep(Settings.notifications_update_time)
-    PerfomNotifications(app)
+    Log.info("Done performing notification")
```

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/abstract.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,26 +81,26 @@
 
     def _create_update_context(self, action, **kwargs) -> dict:
         return {
             'action': action,
             'name': self.name,
         } | kwargs
     
-    def update(self, app: Application) -> None:
+    def scheldue_update(self, app: Application) -> None:
         app.create_task(self._update(app), self._create_update_context('Whole df update'))
     
     async def _update(self, app: Application) -> None:
         await self._pre_update()
         await asyncio.sleep(self.update_sleep_time)
         
         Log.info(f"Prepared to update whole df {self.name}")
         while len(self.mutex) > 0:
             Log.info(f"Halted whole df update at {self.name} with mutex {self.mutex}")
             await asyncio.sleep(self.retry_sleep_time)
-        self.update(app)
+        self.scheldue_update(app)
         self.whole_mutex = True
         
         await self._connect()
         self.as_df = await self._get_df()
         self.whole_mutex = False
 
         Log.info(f"Updated whole df {self.name}")
```

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/groups.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/groups.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/i18n.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/i18n.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/keyboard.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/keyboard.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/log.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/log.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/notifications.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/notifications.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/registration.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/registration.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/report.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/report.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/settings.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/settings.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/switch.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/switch.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/src/spreadsheetbot/sheets/users.py` & `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,17 +132,17 @@
             return(message.text, None)
         elif len(message.photo) != 0:
             return(message.photo, document_link)
         elif message.document != None:
             return(message.document, document_link)
         return (None, None)
     
-    async def send_notification_to_all_users(self, app: Application, message: str, parse_mode: str,
-                                             send_photo: str = None, state: str = None,
-                                             condition: str = None):
+    def send_notification_to_all_users(self, app: Application, message: str, parse_mode: str,
+                                        send_photo: str = None, state: str = None,
+                                        condition: str = None):
         condition_column = 'is_active' if condition in [None, ''] else condition
         self._send_to_all_uids(
             self.selector_condition(condition_column),
             app, message, parse_mode,
             send_photo,
             reply_markup=Notifications.get_keyboard(state)
         )
```

### Comparing `spreadsheetbot-2.1.0/.gitignore` & `spreadsheetbot-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/LICENSE.txt` & `spreadsheetbot-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/README.md` & `spreadsheetbot-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.0/pyproject.toml` & `spreadsheetbot-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spreadsheetbot"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Google Spreadsheet-based Telegram Bot Package"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `spreadsheetbot-2.1.0/PKG-INFO` & `spreadsheetbot-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spreadsheetbot
-Version: 2.1.0
+Version: 2.1.1
 Summary: Google Spreadsheet-based Telegram Bot Package
 Project-URL: Homepage, https://github.com/twobrowin-study/spreadsheetbot-lib
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/spreadsheetbot-lib/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

