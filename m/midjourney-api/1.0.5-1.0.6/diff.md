# Comparing `tmp/midjourney_api-1.0.5.tar.gz` & `tmp/midjourney_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midjourney_api-1.0.5.tar", last modified: Sat May 13 21:48:59 2023, max compression
+gzip compressed data, was "midjourney_api-1.0.6.tar", last modified: Mon May 15 05:19:23 2023, max compression
```

## Comparing `midjourney_api-1.0.5.tar` & `midjourney_api-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 21:48:59.217827 midjourney_api-1.0.5/
--rw-rw-rw-   0        0        0     7388 2023-05-13 21:48:59.216846 midjourney_api-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6002 2023-05-13 21:22:12.000000 midjourney_api-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 21:48:59.206271 midjourney_api-1.0.5/midjourney_api/
--rw-rw-rw-   0        0        0     5916 2023-05-13 18:17:05.000000 midjourney_api-1.0.5/midjourney_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 21:48:59.214830 midjourney_api-1.0.5/midjourney_api.egg-info/
--rw-rw-rw-   0        0        0     7388 2023-05-13 21:48:59.000000 midjourney_api-1.0.5/midjourney_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-13 21:48:59.000000 midjourney_api-1.0.5/midjourney_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 21:48:59.000000 midjourney_api-1.0.5/midjourney_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-13 21:48:59.000000 midjourney_api-1.0.5/midjourney_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 21:48:59.217827 midjourney_api-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1798 2023-05-13 21:48:43.000000 midjourney_api-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:19:23.100782 midjourney_api-1.0.6/
+-rw-rw-rw-   0        0        0     7408 2023-05-15 05:19:23.100782 midjourney_api-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6576 2023-05-15 05:12:35.000000 midjourney_api-1.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-15 05:19:23.084771 midjourney_api-1.0.6/midjourney_api/
+-rw-rw-rw-   0        0        0     6002 2023-05-15 05:18:58.000000 midjourney_api-1.0.6/midjourney_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:19:23.092768 midjourney_api-1.0.6/midjourney_api.egg-info/
+-rw-rw-rw-   0        0        0     7408 2023-05-15 05:19:22.000000 midjourney_api-1.0.6/midjourney_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-05-15 05:19:22.000000 midjourney_api-1.0.6/midjourney_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 05:19:22.000000 midjourney_api-1.0.6/midjourney_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-15 05:19:22.000000 midjourney_api-1.0.6/midjourney_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 05:19:23.100782 midjourney_api-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1747 2023-05-15 05:09:01.000000 midjourney_api-1.0.6/setup.py
```

### Comparing `midjourney_api-1.0.5/PKG-INFO` & `midjourney_api-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midjourney_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Midjourney API wrapper by The Next Leg
 Home-page: https://github.com/midjourney-api-the-next-leg/python-midjourney-api
 Download-URL: https://github.com/midjourney-api-the-next-leg/python-midjourney-api/archive/refs/tags/v1.0.0.tar.gz
 Author: The Next leg
 Author-email: support@thenextleg.io
 License: MIT
 Keywords: MIDJOURNEY,API,THE_NEXT_LEG
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.6
 
 The Next Leg
 ============
 
 The Next Leg is a module that provides functionality for creating
 AI-generated images with Midjourney. It provides a simple interface for
-interacting with Midjourney’s API and performing various actions such as
+interacting with Midjourneyï¿½s API and performing various actions such as
 creating images from prompts or URLs, describing images, using buttons
 or slash commands, and getting/setting account settings.
 
 Installation
 ------------
 
 To use this package, you need to have Python installed on your machine.
@@ -40,15 +40,15 @@
 -----
 
 Here is an example of how to use the TNL package to create an image from
 a prompt:
 
 ::
 
-   from tnl import TNL
+   from midjourney_api import TNL
 
    TNL_API_KEY = 'your_api_key_here'
    tnl = TNL(TNL_API_KEY)
 
    prompt = 'a cat playing the piano'
    response = tnl.imagine(prompt)
 
@@ -81,15 +81,15 @@
 ``tnl.get_message_and_progress(message_id: str, expire_mins: Optional[int] = None)``
 
 Gets the progress and response of a message.
 
 -  ``message_id`` - The message ID of the message you want to get the
    progress and response for.
 -  ``expire_mins`` (optional) - A timeout for the request in minutes. If
-   the request takes longer than this, it will return as ‘incomplete’
+   the request takes longer than this, it will return as ï¿½incompleteï¿½
 
 Img 2 Img
 ~~~~~~~~~
 
 ``tnl.img2img(prompt: str, img_url: str, ref: str = '', webhook_override: str = '')``
 
 Creates an image from a prompt and an image.
```

### Comparing `midjourney_api-1.0.5/README.md` & `midjourney_api-1.0.6/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,170 +1,233 @@
-# The Next Leg
+The Next Leg
+============
 
-The Next Leg is a module that provides functionality for creating AI-generated images with Midjourney. It provides a simple interface for interacting with Midjourney's API and performing various actions such as creating images from prompts or URLs, describing images, using buttons or slash commands, and getting/setting account settings.
+The Next Leg is a module that provides functionality for creating
+AI-generated images with Midjourney. It provides a simple interface for
+interacting with Midjourney�s API and performing various actions such as
+creating images from prompts or URLs, describing images, using buttons
+or slash commands, and getting/setting account settings.
 
-## Installation
+Installation
+------------
 
-To use this package, you need to have Python installed on your machine. You can install TNL using pip:
+To use this package, you need to have Python installed on your machine.
+You can install TNL using pip:
 
-```sh
-pip install midjourney-api
-```
+.. code:: sh
 
-## Usage
+   pip install midjourney-api
 
-Here is an example of how to use the TNL package to create an image from a prompt:
+Usage
+-----
 
-```
-from tnl import TNL
+Here is an example of how to use the TNL package to create an image from
+a prompt:
 
-TNL_API_KEY = 'your_api_key_here'
-tnl = TNL(TNL_API_KEY)
+::
 
-prompt = 'a cat playing the piano'
-response = tnl.imagine(prompt)
+   from midjourney_api import TNL
 
-print(response)
-```
+   TNL_API_KEY = 'your_api_key_here'
+   tnl = TNL(TNL_API_KEY)
 
-## API
+   prompt = 'a cat playing the piano'
+   response = tnl.imagine(prompt)
 
-### `TNL(api_key: str)
+   print(response)
 
-Creates a new instance of `TNL` with the provided `apiKey`.
+API
+---
 
-### Imagine
+\`TNL(api_key: str)
+~~~~~~~~~~~~~~~~~~~
 
-`tnl.imagine(prompt: str, ref: str = '', webhook_override: str = '')`
+Creates a new instance of ``TNL`` with the provided ``apiKey``.
+
+Imagine
+~~~~~~~
+
+``tnl.imagine(prompt: str, ref: str = '', webhook_override: str = '')``
 
 Creates a new image from a prompt.
 
-- `prompt` - The prompt you want to use to generate the image.
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+-  ``prompt`` - The prompt you want to use to generate the image.
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
 
-### Get Progress and Message Result
+Get Progress and Message Result
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-`tnl.get_message_and_progress(message_id: str, expire_mins: Optional[int] = None)`
+``tnl.get_message_and_progress(message_id: str, expire_mins: Optional[int] = None)``
 
 Gets the progress and response of a message.
 
-- `message_id` - The message ID of the message you want to get the progress and response for.
-- `expire_mins` (optional) - A timeout for the request in minutes. If the request takes longer than this, it will return as 'incomplete'
+-  ``message_id`` - The message ID of the message you want to get the
+   progress and response for.
+-  ``expire_mins`` (optional) - A timeout for the request in minutes. If
+   the request takes longer than this, it will return as �incomplete�
 
-### Img 2 Img
+Img 2 Img
+~~~~~~~~~
 
-`tnl.img2img(prompt: str, img_url: str, ref: str = '', webhook_override: str = '')`
+``tnl.img2img(prompt: str, img_url: str, ref: str = '', webhook_override: str = '')``
 
 Creates an image from a prompt and an image.
 
-- `prompt` - The prompt you want to use to generate the image.
-- `img_url` - The URL of the image you want to use as the base image.
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+-  ``prompt`` - The prompt you want to use to generate the image.
+-  ``img_url`` - The URL of the image you want to use as the base image.
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
 
-### Describe
+Describe
+~~~~~~~~
 
-`tnl.describe(img_url: str, ref: str = '', webhook_override: str = '')`
+``tnl.describe(img_url: str, ref: str = '', webhook_override: str = '')``
 
 Describes an image.
 
-- `img_url` - The URL of the image you want to describe.
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+-  ``img_url`` - The URL of the image you want to describe.
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
 
-### Button
+Button
+~~~~~~
 
-`tnl.button(button: TNLTypes.ButtonTypes, button_message_id: str, ref: str = '', webhook_override: str = '')`
+``tnl.button(button: TNLTypes.ButtonTypes, button_message_id: str, ref: str = '', webhook_override: str = '')``
 
 Uses a button on an image.
 
-- `button` - A button type.
-- `button_message_id` - The button_message_id of the message that contains the button.
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+-  ``button`` - A button type.
+-  ``button_message_id`` - The button_message_id of the message that
+   contains the button.
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
 
-### Get Seed
+Get Seed
+~~~~~~~~
 
-`tnl.getSeed(message_id: string): Promise<TNLTypes.Response.Seed>`
+``tnl.getSeed(message_id: string): Promise<TNLTypes.Response.Seed>``
 
 Gets a seed of a message.
 
-- `message_id` - The message ID of the message you want to get the seed for.
+-  ``message_id`` - The message ID of the message you want to get the
+   seed for.
 
-### Slash Command
+Slash Command
+~~~~~~~~~~~~~
 
-`tnl.slashCommand(slashCommand: TNLTypes.SlashCommands, ref?: string, webhook_override?: string)`
+``tnl.slashCommand(slashCommand: TNLTypes.SlashCommands, ref?: string, webhook_override?: string)``
 
 Uses a slash command such as relax, fast, private, or stealth.
 
-- `slashCommand` - A slash command type.
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+-  ``slashCommand`` - A slash command type.
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
 
-### Get Settings
+Get Settings
+~~~~~~~~~~~~
 
-`tnl.getSettings(): Promise<TNLTypes.Response.Message>`
+``tnl.getSettings(): Promise<TNLTypes.Response.Message>``
 
 Gets the settings available for your account.
 
-### Set Settings
+Set Settings
+~~~~~~~~~~~~
 
-`tnl.setSettings(settings: TNLTypes.Settings, ref?: string, webhook_override?: string)`
+``tnl.setSettings(settings: TNLTypes.Settings, ref?: string, webhook_override?: string)``
 
 Sets the settings for your account.
 
-- `settings` - The settings you want to set.
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+-  ``settings`` - The settings you want to set.
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
 
-### Get Info
+Get Info
+~~~~~~~~
 
-`tnl.getInfo(ref?: string, webhook_override?: string)`
+``tnl.getInfo(ref?: string, webhook_override?: string)``
 
-Gets information about your account including Fast Time Remaining, Job Mode, Queued Jobs and more.
+Gets information about your account including Fast Time Remaining, Job
+Mode, Queued Jobs and more.
 
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
 
-### Get Seed
+.. _get-seed-1:
 
-`tnl.getSeed(message_id: str)`
+Get Seed
+~~~~~~~~
 
-Gets a seed of a message.
+``tnl.getSeed(message_id: str)``
 
-- `message_id` - The message ID of the message you want to get the seed for.
+Gets a seed of a message.
 
-### Slash Command
+-  ``message_id`` - The message ID of the message you want to get the
+   seed for.
 
-`tnl.slashCommand(slash_command: TNLTypes.SlashCommands, ref: str = '', webhook_override: str = '')`
+.. _slash-command-1:
 
-Uses a slash command such as relax, fast, private, or stealth.
+Slash Command
+~~~~~~~~~~~~~
 
-- `slash_command` - A slash command type.
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+``tnl.slashCommand(slash_command: TNLTypes.SlashCommands, ref: str = '', webhook_override: str = '')``
 
-### Get Settings
+Uses a slash command such as relax, fast, private, or stealth.
 
-`tnl.getSettings()`
+-  ``slash_command`` - A slash command type.
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
 
-Gets the settings available for your account.
+.. _get-settings-1:
 
-### Set Settings
+Get Settings
+~~~~~~~~~~~~
 
-`tnl.setSettings(settings: TNLTypes.Settings, ref: str = '', webhook_override: str = '')`
+``tnl.getSettings()``
 
-Sets the settings for your account.
+Gets the settings available for your account.
 
-- `settings` - The settings you want to set.
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+.. _set-settings-1:
 
-### Get Info
+Set Settings
+~~~~~~~~~~~~
 
-`tnl.getInfo(ref: str = '', webhook_override: str = '')`
+``tnl.setSettings(settings: TNLTypes.Settings, ref: str = '', webhook_override: str = '')``
 
-Gets information about your account including Fast Time Remaining, Job Mode, Queued Jobs and more.
+Sets the settings for your account.
 
-- `ref` (optional) - A reference string that will be returned in the webhook response.
-- `webhook_override` (optional) - A webhook URL that will be used instead of the one set in the dashboard.
+-  ``settings`` - The settings you want to set.
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
+
+.. _get-info-1:
+
+Get Info
+~~~~~~~~
+
+``tnl.getInfo(ref: str = '', webhook_override: str = '')``
+
+Gets information about your account including Fast Time Remaining, Job
+Mode, Queued Jobs and more.
+
+-  ``ref`` (optional) - A reference string that will be returned in the
+   webhook response.
+-  ``webhook_override`` (optional) - A webhook URL that will be used
+   instead of the one set in the dashboard.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `midjourney_api-1.0.5/midjourney_api/__init__.py` & `midjourney_api-1.0.6/midjourney_api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,167 +1,186 @@
 import requests
 
-BASE_URL = 'https://api.thenextleg.io/v2'
+BASE_URL = "https://api.thenextleg.io/v2"
+
 
 class TNL:
     def __init__(self, token):
         self.token = token
 
     def create_headers(self):
         return {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {self.token}',
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.token}",
         }
 
-    async def imagine(self, prompt, ref='', webhook_override=''):
+    def imagine(self, prompt, ref="", webhook_override=""):
         """
         Imagine an image based on a prompt.
-        ARGS:   
+        ARGS:
             prompt: str - The prompt to use.
             ref: str - A reference string passed back in the webhook
             webhook_override: str - A webhook to override the default webhook.
         """
         request = {
-            'msg': prompt,
-            'ref': ref,
-            'webhookOverride': webhook_override,
+            "msg": prompt,
+            "ref": ref,
+            "webhookOverride": webhook_override,
         }
 
-        res = await requests.post(f'{BASE_URL}/imagine', json=request, headers=self.create_headers())
+        res = requests.post(
+            f"{BASE_URL}/imagine", json=request, headers=self.create_headers()
+        )
+
         return res.json()
 
-    async def img2img(self, prompt, img_url, ref='', webhook_override=''):
+    def img2img(self, prompt, img_url, ref="", webhook_override=""):
         """
         Perform an image to image operation.
         ARGS:
             prompt: str - The prompt to use.
             img_url: str - The image to use.
             ref: str - A reference string passed back in the webhook
             webhook_override: str - A webhook to override the default webhook.
         """
         request = {
-            'msg': f'{img_url} {prompt}',
-            'ref': ref,
-            'webhookOverride': webhook_override,
+            "msg": f"{img_url} {prompt}",
+            "ref": ref,
+            "webhookOverride": webhook_override,
         }
 
-        res = await requests.post(f'{BASE_URL}/imagine', json=request, headers=self.create_headers())
+        res = requests.post(
+            f"{BASE_URL}/imagine", json=request, headers=self.create_headers()
+        )
         return res.json()
 
-    async def describe(self, img_url, ref='', webhook_override=''):
+    def describe(self, img_url, ref="", webhook_override=""):
         """
         Describe an image.
         ARGS:
             img_url: str - The image to describe.
             ref: str - A reference string passed back in the webhook
             webhook_override: str - A webhook to override the default webhook.
         """
         request = {
-            'url': img_url,
-            'ref': ref,
-            'webhookOverride': webhook_override,
+            "url": img_url,
+            "ref": ref,
+            "webhookOverride": webhook_override,
         }
 
-        res = await requests.post(f'{BASE_URL}/imagine', json=request, headers=self.create_headers())
+        res = requests.post(
+            f"{BASE_URL}/imagine", json=request, headers=self.create_headers()
+        )
         return res.json()
 
-    async def button(self, button, button_message_id, ref='', webhook_override=''):
+    def button(self, button, button_message_id, ref="", webhook_override=""):
         """
         Press a button.
         ARGS:
             button: str - The button to press.
             button_message_id: str - The message id of the button.
             ref: str - A reference string passed back in the webhook
             webhook_override: str - A webhook to override the default webhook.
         """
         request = {
-            'cmd': button,
-            'buttonMessageId': button_message_id,
-            'ref': ref,
-            'webhookOverride': webhook_override,
+            "cmd": button,
+            "buttonMessageId": button_message_id,
+            "ref": ref,
+            "webhookOverride": webhook_override,
         }
 
-        res = await requests.post(f'{BASE_URL}/button', json=request, headers=self.create_headers())
+        res = requests.post(
+            f"{BASE_URL}/button", json=request, headers=self.create_headers()
+        )
         return res.json()
 
-    async def get_seed(self, message_id):
+    def get_seed(self, message_id):
         """
         Get the seed of a message.
         ARGS:
             message_id: str - The message id of the message.
         """
         request = {
-            'messageId': message_id,
+            "messageId": message_id,
         }
 
-        res = await requests.post(f'{BASE_URL}/seed', json=request, headers=self.create_headers())
+        res = requests.post(
+            f"{BASE_URL}/seed", json=request, headers=self.create_headers()
+        )
         return res.json()
 
-    async def slash_command(self, slash_command, ref='', webhook_override=''):
-        """ 
+    def slash_command(self, slash_command, ref="", webhook_override=""):
+        """
         Perform a slash command.
-        ARGS: 
+        ARGS:
             slash_command: str - The slash command to perform.
             ref: str - A reference string passed back in the webhook
             webhook_override: str - A webhook to override the default webhook.
-        """ 
+        """
         request = {
-            'cmd': slash_command,
-            'ref': ref,
-            'webhookOverride': webhook_override,
+            "cmd": slash_command,
+            "ref": ref,
+            "webhookOverride": webhook_override,
         }
 
-        res = await requests.post(f'{BASE_URL}/slash-commands', json=request, headers=self.create_headers())
+        res = requests.post(
+            f"{BASE_URL}/slash-commands", json=request, headers=self.create_headers()
+        )
         return res.json()
 
-    async def get_settings(self):
+    def get_settings(self):
         """
-        Get an account setting.   
+        Get an account setting.
         """
-        res = await requests.get(f'{BASE_URL}/settings', headers=self.create_headers())
+        res = requests.get(f"{BASE_URL}/settings", headers=self.create_headers())
         return res.json()
 
-    async def set_settings(self, setting, ref='', webhook_override=''):
+    def set_settings(self, setting, ref="", webhook_override=""):
         """
         Set an account settings.
         ARGS:
             setting: str - The setting to set.
             ref: str - A reference string passed back in the webhook
             webhook_override: str - A webhook to override the default webhook.
         """
         request = {
-            'settingsToggle': setting,
-            'ref': ref,
-            'webhookOverride': webhook_override,
+            "settingsToggle": setting,
+            "ref": ref,
+            "webhookOverride": webhook_override,
         }
 
-        res = await requests.post(f'{BASE_URL}/settings', json=request, headers=self.create_headers())
+        res = requests.post(
+            f"{BASE_URL}/settings", json=request, headers=self.create_headers()
+        )
         return res.json()
 
-    async def get_info(self, ref='', webhook_override=''):
+    def get_info(self, ref="", webhook_override=""):
         """
         Get the info of the account.
         ARGS:
             ref: str - A reference string passed back in the webhook
             webhook_override: str - A webhook to override the default webhook.
         """
         request = {
-            'ref': ref,
-            'webhookOverride': webhook_override,
+            "ref": ref,
+            "webhookOverride": webhook_override,
         }
 
-        res = await requests.post(f'{BASE_URL}/info', json=request, headers=self.create_headers())
+        res = requests.post(
+            f"{BASE_URL}/info", json=request, headers=self.create_headers()
+        )
         return res.json()
-    
-    async def get_message_and_progress(self,message_id, expire_mins):
+
+    def get_message_and_progress(self, message_id, expire_mins):
         """
         Get the message and progress of a message.
         ARGS:
             message_id: str - The message id of the message.
             expire_mins: int - The time to live for the message.
         """
-        url = f'{BASE_URL}/message/{message_id}'
+        url = f"{BASE_URL}/message/{message_id}"
         if expire_mins:
-            url += f'?expireMins={expire_mins}'
-        res = await requests.get(f'{BASE_URL}/message/{message_id}', headers=self.create_headers())
+            url += f"?expireMins={expire_mins}"
+        res = requests.get(
+            f"{BASE_URL}/message/{message_id}", headers=self.create_headers()
+        )
         return res.json()
-
```

### Comparing `midjourney_api-1.0.5/midjourney_api.egg-info/PKG-INFO` & `midjourney_api-1.0.6/midjourney_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midjourney-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Midjourney API wrapper by The Next Leg
 Home-page: https://github.com/midjourney-api-the-next-leg/python-midjourney-api
 Download-URL: https://github.com/midjourney-api-the-next-leg/python-midjourney-api/archive/refs/tags/v1.0.0.tar.gz
 Author: The Next leg
 Author-email: support@thenextleg.io
 License: MIT
 Keywords: MIDJOURNEY,API,THE_NEXT_LEG
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.6
 
 The Next Leg
 ============
 
 The Next Leg is a module that provides functionality for creating
 AI-generated images with Midjourney. It provides a simple interface for
-interacting with Midjourney’s API and performing various actions such as
+interacting with Midjourneyï¿½s API and performing various actions such as
 creating images from prompts or URLs, describing images, using buttons
 or slash commands, and getting/setting account settings.
 
 Installation
 ------------
 
 To use this package, you need to have Python installed on your machine.
@@ -40,15 +40,15 @@
 -----
 
 Here is an example of how to use the TNL package to create an image from
 a prompt:
 
 ::
 
-   from tnl import TNL
+   from midjourney_api import TNL
 
    TNL_API_KEY = 'your_api_key_here'
    tnl = TNL(TNL_API_KEY)
 
    prompt = 'a cat playing the piano'
    response = tnl.imagine(prompt)
 
@@ -81,15 +81,15 @@
 ``tnl.get_message_and_progress(message_id: str, expire_mins: Optional[int] = None)``
 
 Gets the progress and response of a message.
 
 -  ``message_id`` - The message ID of the message you want to get the
    progress and response for.
 -  ``expire_mins`` (optional) - A timeout for the request in minutes. If
-   the request takes longer than this, it will return as ‘incomplete’
+   the request takes longer than this, it will return as ï¿½incompleteï¿½
 
 Img 2 Img
 ~~~~~~~~~
 
 ``tnl.img2img(prompt: str, img_url: str, ref: str = '', webhook_override: str = '')``
 
 Creates an image from a prompt and an image.
```

### Comparing `midjourney_api-1.0.5/setup.py` & `midjourney_api-1.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import pypandoc
 import setuptools
 
 setuptools.setup(
     name="midjourney_api",  # How you named your package folder (MyLib)
     packages=["midjourney_api"],  # Chose the same as "name"
-    version="1.0.5",  # Start with a small number and increase it with every change you make
+    version="1.0.6",  # Start with a small number and increase it with every change you make
     license="MIT",  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-    long_description=pypandoc.convert_file("README.md", "rst").replace("\r", ""),
+    long_description=open("README.rst").read(),
     description="Midjourney API wrapper by The Next Leg",  # Give a short description about your library
     author="The Next leg",  # Type in your name
     author_email="support@thenextleg.io",  # Type in your E-Mail
     url="https://github.com/midjourney-api-the-next-leg/python-midjourney-api",  # Provide either the link to your github or to your website
     download_url="https://github.com/midjourney-api-the-next-leg/python-midjourney-api/archive/refs/tags/v1.0.0.tar.gz",  # I explain this later on
     keywords=[
         "MIDJOURNEY",
```

