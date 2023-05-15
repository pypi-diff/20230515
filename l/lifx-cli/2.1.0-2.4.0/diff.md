# Comparing `tmp/lifx_cli-2.1.0.tar.gz` & `tmp/lifx_cli-2.4.0.tar.gz`

## Comparing `lifx_cli-2.1.0.tar` & `lifx_cli-2.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/src/lifx/__init__.py
--rwxr-xr-x   0        0        0     1847 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/src/lifx/auth.py
--rwxr-xr-x   0        0        0     1782 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/src/lifx/colors.py
--rwxr-xr-x   0        0        0     1035 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/src/lifx/devices.py
--rwxr-xr-x   0        0        0    10079 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/src/lifx/lifx.py
--rwxr-xr-x   0        0        0     3508 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/src/lifx/lights.py
--rwxr-xr-x   0        0        0      955 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/src/lifx/scenes.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/LICENSE
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 lifx_cli-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/requirements.txt
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/src/lifx/__init__.py
+-rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/src/lifx/auth.py
+-rwxr-xr-x   0        0        0     1762 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/src/lifx/colors.py
+-rwxr-xr-x   0        0        0    10649 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/src/lifx/lifx.py
+-rwxr-xr-x   0        0        0     4407 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/src/lifx/lights.py
+-rwxr-xr-x   0        0        0     1002 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/src/lifx/scenes.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/LICENSE
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 lifx_cli-2.4.0/PKG-INFO
```

### Comparing `lifx_cli-2.1.0/src/lifx/auth.py` & `lifx_cli-2.4.0/src/lifx/auth.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 #!/usr/bin/env python3
+"""Configure and set authentication headers."""
+
+import sys
+import configparser
+from os import path, environ, getenv
 
 class Auth:
+    """Configure and set authentication headers."""
 
     def __init__(self):
-        from os import path
 
         self.auth_file = f'{path.expanduser("~")}/.keys'
         self.auth_file_section = 'lifx'
         self.auth_file_key = 'token'
         self.auth_env_var = 'LIFX'
 
     def configure(self):
         """Configure/update the ini file for API authentication."""
-        import configparser
-        from os import path
 
         config = configparser.RawConfigParser()
         api_key = input('What is your API token?: ')
 
         if path.exists(self.auth_file):
             config.read(self.auth_file)
 
         if not config.has_section(self.auth_file_section):
             config = configparser.RawConfigParser()
             config.add_section(self.auth_file_section)
             config.set(self.auth_file_section, self.auth_file_key, api_key)
 
-            with open(self.auth_file, 'a+') as f:
-                config.write(f)
+            with open(self.auth_file, 'a+', encoding='UTF-8') as file:
+                config.write(file)
         else:
-            overwrite = input('You already have an API key saved in ~/.keys. Do you want to overwrite this value? y/N ')
+            overwrite = input('You already have an API key saved in ~/.keys. '
+                              'Do you want to overwrite this value? y/N ')
             overwrite = overwrite.lower()
 
             if overwrite == 'y':
                 config.set(self.auth_file_section, self.auth_file_key, api_key)
 
-                with open(self.auth_file, 'w') as f:
-                    config.write(f)
+                with open(self.auth_file, 'w', encoding='UTF-8') as file:
+                    config.write(file)
 
-        return
+        sys.exit(0)
 
     def auth(self):
         """Returns the headers required to authenticate to the LIFX API."""
-        import configparser
-        from os import environ, getenv
 
         if environ.get(self.auth_env_var):
             token = getenv(self.auth_env_var)
         else:
             config = configparser.ConfigParser()
             config.read(self.auth_file)
```

### Comparing `lifx_cli-2.1.0/src/lifx/colors.py` & `lifx_cli-2.4.0/src/lifx/colors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 #!/usr/bin/env python3
+"""Learn about how the CLI accepts color encoding."""
 
-COLOR_TABLE = [['[name]', 'white, red, orange, yellow, cyan, green, blue, purple, or pink', 'Sets hue and '
-                                                                                            'saturation only.'],
+import json
+from requests import get
+from tabulate import tabulate
+from src.lifx.auth import Auth
+
+COLOR_TABLE = [['[name]', 'white, red, orange, yellow, cyan, green, blue, purple, or pink',
+                'Sets hue and saturation only.'],
                ['hue:[0-360]', 'hue:120', 'Sets hue.'],
                ['saturation:[0.0-1.0]', 'saturation:0.5', 'Sets saturation.'],
                ['brightness:[0.0-1.0]', 'brightness:0.5', 'Sets brightness.'],
                ['kelvin:[1500-9000]', 'kelvin:5000', 'Sets kelvin to -c and saturation to 0.0.'],
                ['#RRGGBB', '#ff0000', 'Converts to HSBK.'],
                ['rgb:[0-255],[0-255],[0-255]', 'rgb:255,255,0', '	Converts to HSBK.']]
 
 
 class Colors:
+    """Learn about how the CLI accepts color encoding."""
     def __init__(self):
-        from src.lifx.auth import Auth
 
         self.auth = Auth()
         self.auth_headers = self.auth.auth()
 
     @staticmethod
     def color_information():
         """Print color formatting information."""
-        from tabulate import tabulate
 
         print(tabulate(COLOR_TABLE, headers=["Format", "Example", "Notes"]))
 
     def validate_color(self, color):
         """Validate the provided color with the LIFX API."""
-        import json
-        from requests import get
-        from tabulate import tabulate
 
-        response = get(f'https://api.lifx.com/v1/color?string={color}', headers=self.auth_headers)
+        url = f'https://api.lifx.com/v1/color?string={color}'
+        response = get(url, headers=self.auth_headers, timeout=5)
         response = json.loads(response.content)
 
         hue = response['hue'] or 'None'
         saturation = response['saturation'] or 'None'
         brightness = response['brightness'] or 'None'
         kelvin = response['kelvin'] or 'None'
 
         validated_colors = [[hue, saturation, brightness, kelvin]]
 
         print(tabulate(validated_colors, headers=["Hue", "Saturation", "Brightness", "Kelvin"]))
-        pass
```

### Comparing `lifx_cli-2.1.0/src/lifx/lifx.py` & `lifx_cli-2.4.0/src/lifx/lifx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 #!/usr/bin/env python3
-
+"""
+Author: Wes Henderson
+Control your lights with the unofficial LIFX CLI. This CLI uses the
+LIFX HTTP endpoints to configure your lights.
+https://api.developer.lifx.com/reference/introduction
+"""
 import argparse
 from src.lifx.auth import Auth
 from src.lifx.colors import Colors
-from src.lifx.devices import Devices
 from src.lifx.lights import Lights
 from src.lifx.scenes import Scenes
 
 auth = Auth()
 colors = Colors()
-device = Devices()
 light = Lights()
 scene = Scenes()
 
-logo = """
+LOGO = """
 ██      ██ ███████ ██   ██      ██████ ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ██      ██ █████     ███       ██      ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ███████ ██ ██      ██   ██      ██████ ███████ ██
 
 """
 
 
 def lights_sub_command(args):
+    """Control the actions for the 'lights' sub-command."""
     devices = args.list_devices
     light_id = args.light_id
     toggle = args.toggle
     group = args.group
     state = args.state
     color = args.color
     power = args.power
     brightness = args.brightness
     infrared = args.infrared
     duration = args.duration
 
     if devices:
-        device.get()
+        light.get()
 
     if toggle:
         light.toggle(light_id, group)
 
     if state:
-        light.set_state(light_id, group, color, power, brightness, duration, infrared)
+        state_attributes = {'power': power,
+                            'brightness': brightness,
+                            'duration': duration,
+                            'infrared': infrared}
+        light.set_state(light_id, group, color, state_attributes)
 
 
 def scenes_sub_command(args):
+    """Control the actions for the 'scenes' sub-command."""
     scenes = args.list_scenes
     scene_id = args.scene_id
 
     if scenes:
         scene.get()
 
     if scene_id:
         scene.activate(scene_id)
 
 
 def effects_sub_command(args):
+    """Control the actions for the 'effects' sub-command."""
     list_effects = args.list_effects
     light_id = args.light_id
     group = args.group
     color = args.color
     breathe = args.breathe
     pulse = args.pulse
     stop = args.stop
@@ -72,26 +82,28 @@
     elif pulse:
         light.pulse_effect(light_id, group, color)
     elif stop:
         light.stop_effect(light_id, group)
 
 
 def colors_sub_command(args):
+    """Control the actions for the 'colors' sub-command."""
     list_colors = args.list_colors
     provided_color = args.colors
 
     if list_colors:
         colors.color_information()
 
     if provided_color:
         colors.validate_color(provided_color)
 
 
 def main():
-    print(logo)
+    """Main entrypoint for the LIFX CLI."""
+    print(LOGO)
     # Create the parser
     description = 'Control LIFX devices via the CLI!'
     epilog = 'Run `lifx --configure` to setup authentication.'
     job_options = argparse.ArgumentParser(description=description, epilog=epilog)
 
     # Add the arguments
     job_options.add_argument('-c',
@@ -153,15 +165,15 @@
                                default=0.5,
                                action='store',
                                help='State: 0.0 to 1.0 [Default: 1.0]')
     light_command.add_argument('-u',
                                '--duration',
                                default=1,
                                action='store',
-                               help='State: How long the action will take (in seconds). [Default: 1]')
+                               help='State: How many seconds should the action take. [Default: 1]')
 
     # Add the 'scenes' sub-command.
     scene_command = light_job_options.add_parser('scenes', help='Scene specific functions.')
     scene_command.add_argument('-l',
                                '--list',
                                default=False,
                                dest='list_scenes',
@@ -199,15 +211,15 @@
                                 default=False,
                                 action='store_true',
                                 help='Specify whether or not the target is a group.')
     effect_command.add_argument('-c',
                                 '--color',
                                 default=[],
                                 action='append',
-                                help='Use the specified color. Use multiple -c options to alternate colors.')
+                                help='Specify the color; multiple -c options alternate colors.')
     effect_command.add_argument('--breathe',
                                 default=False,
                                 action='store_true',
                                 help='Effects: Breathe')
     effect_command.add_argument('--pulse',
                                 default=False,
                                 action='store_true',
@@ -237,15 +249,14 @@
 
     args = job_options.parse_args()
     configure = args.configure
 
     # Configure authentication.
     if configure:
         auth.configure()
-        exit(0)
 
     # The 'lights' sub-command.
     if args.command == 'lights':
         lights_sub_command(args)
 
     # The 'scenes' sub-command.
     if args.command == 'scenes':
```

### Comparing `lifx_cli-2.1.0/src/lifx/lights.py` & `lifx_cli-2.4.0/src/lifx/lights.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,84 @@
 #!/usr/bin/env python3
+"""Control LIFX lights and effects."""
+
+import json
+from requests import get, post, put
+from tabulate import tabulate
+from src.lifx.auth import Auth
+
 
 class Lights:
+    """Control LIFX lights and effects."""
 
     def __init__(self):
-        from src.lifx.auth import Auth
-
         self.auth = Auth()
         self.auth_headers = self.auth.auth()
 
+    def get(self):
+        """Print a list of all LIFX devices on this account."""
+
+        url = 'https://api.lifx.com/v1/lights/all'
+        response = get(url, headers=self.auth_headers, timeout=5)
+        response = json.loads(response.content)
+
+        devices = []
+
+        for key in range(0, len(response)):
+            label = response[key]["label"]
+            ident = response[key]["id"]
+            power = response[key]["power"]
+            connected = response[key]["connected"]
+            group = response[key]["group"]["name"]
+            group_id = response[key]["group"]["id"]
+
+            devices += [[label, ident, power, connected, group, group_id]]
+
+        devices.sort()
+        print(tabulate(devices, headers=["Name", "ID", "State", "Connected", "Group", "Group ID"]))
+
     def toggle(self, light_id, group):
         """Toggles the power for the specified light. Requires the device ID."""
-        from requests import post
 
         if group:
             light_id = f'group_id:{light_id}'
 
-        post(f"https://api.lifx.com/v1/lights/{light_id}/toggle", headers=self.auth_headers)
+        url = f"https://api.lifx.com/v1/lights/{light_id}/toggle"
+        post(url, headers=self.auth_headers, timeout=5)
 
-    def set_state(self, light_id, group, color, power, brightness, duration, infrared):
-        """Changes the state for the specified light. Requires the device ID as well as optional changes."""
-        from requests import put
+    def set_state(self, light_id, group, color, state_attributes):
+        """Changes the state for the specified light. Requires the device ID."""
 
         payload = {
-            "power": f"{power}",
+            "power": f"{state_attributes['power']}",
             "color": f"{color}",
-            "brightness": f"{brightness}",
-            "duration": f"{duration}",
-            "infrared": f"{infrared}",
+            "brightness": f"{state_attributes['brightness']}",
+            "duration": f"{state_attributes['duration']}",
+            "infrared": f"{state_attributes['infrared']}",
         }
 
         if group:
             light_id = f'group_id:{light_id}'
 
-        put(f"https://api.lifx.com/v1/lights/{light_id}/state", data=payload, headers=self.auth_headers)
+        url = f"https://api.lifx.com/v1/lights/{light_id}/state"
+        put(url, data=payload, headers=self.auth_headers, timeout=5)
 
     def list_effects(self):
         """List effects currently supported by the CLI."""
-        from tabulate import tabulate
-
-        effects = [['Breathe', 'Performs a breathe effect by slowly fading between the given colors.'],
-                   ['Pulse', 'Performs a pulse effect by quickly flashing between the given colors. ']]
+        effects = [['Breathe',
+                    'Performs a breathe effect by slowly fading between the given colors.'],
+                   ['Pulse',
+                    'Performs a pulse effect by quickly flashing between the given colors. ']]
 
         print(tabulate(effects, headers=["Name", "Description"]))
         print("\nNote: The CLI can only control effects stored on your light's firmware.")
-        pass
 
     def breathe_effect(self, light_id, group, color):
-        """Activates the breath effect on the specified light (period: 2; cycles: 10). Requires the device ID and
-        color."""
-        from requests import post
+        """Activates the breath effect (period: 2; cycles: 10).
+        Requires the device ID and color."""
 
         if len(color) == 1:
             data = {
                 "period": 2,
                 "cycles": 10,
                 "color": f"{color[0]}",
             }
@@ -63,20 +89,20 @@
                 "from_color": f"{color[0]}",
                 "color": f"{color[1]}",
             }
 
         if group:
             light_id = f'group_id:{light_id}'
 
-        post(f"https://api.lifx.com/v1/lights/{light_id}/effects/breathe", data=data, headers=self.auth_headers)
+        url = f"https://api.lifx.com/v1/lights/{light_id}/effects/breathe"
+        post(url, data=data, headers=self.auth_headers, timeout=5)
 
     def pulse_effect(self, light_id, group, color):
-        """Activates the pulse effect on the specified light (period: 2; cycles: 10). Requires the device ID and
-        color."""
-        from requests import post
+        """Activates the pulse effect (period: 2; cycles: 10).
+        Requires the device ID and color."""
 
         if len(color) == 1:
             data = {
                 "period": 2,
                 "cycles": 10,
                 "color": f"{color[0]}",
             }
@@ -87,21 +113,22 @@
                 "from_color": f"{color[0]}",
                 "color": f"{color[1]}",
             }
 
         if group:
             light_id = f'group_id:{light_id}'
 
-        post(f"https://api.lifx.com/v1/lights/{light_id}/effects/pulse", data=data, headers=self.auth_headers)
+        url = f"https://api.lifx.com/v1/lights/{light_id}/effects/pulse"
+        post(url, data=data, headers=self.auth_headers, timeout=5)
 
     def stop_effect(self, light_id, group):
         """Stop all effects on the specified light. Requires Light ID."""
-        from requests import post
 
         data = {
             "power_off": True
         }
 
         if group:
             light_id = f'group_id:{light_id}'
 
-        post(f"https://api.lifx.com/v1/lights/{light_id}/effects/off", data=data, headers=self.auth_headers)
+        url = f"https://api.lifx.com/v1/lights/{light_id}/effects/off"
+        post(url, data=data, headers=self.auth_headers, timeout=5)
```

### Comparing `lifx_cli-2.1.0/src/lifx/scenes.py` & `lifx_cli-2.4.0/src/lifx/scenes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 #!/usr/bin/env python3
+"""List and control LIFX scenes."""
+
+import json
+from requests import get, put
+from tabulate import tabulate
+from src.lifx.auth import Auth
+
 
 class Scenes:
+    """List and control LIFX scenes."""
 
     def __init__(self):
-        from src.lifx.auth import Auth
-
         self.auth = Auth()
         self.auth_headers = self.auth.auth()
 
     def get(self):
         """Print a list of all scenes on this account."""
-        import json
-        from requests import get
-        from tabulate import tabulate
 
-        response = get('https://api.lifx.com/v1/scenes', headers=self.auth_headers)
+        url = 'https://api.lifx.com/v1/scenes'
+        response = get(url, headers=self.auth_headers, timeout=5)
         response = json.loads(response.content)
-        
+
         scenes = []
-        
-        for key in range(0, len(response)):
+
+        for key in enumerate(response):
             scenes += [[response[key]["name"], response[key]["uuid"]]]
-        
+
         scenes.sort()
         print(tabulate(scenes, headers=["Name", "ID"]))
 
     def activate(self, scene_id):
         """Activates the specified scene. Requires scene UUID."""
-        from requests import put
 
-        put(f'https://api.lifx.com/v1/scenes/scene_id:{scene_id}/activate', headers=self.auth_headers)
+        url = f'https://api.lifx.com/v1/scenes/scene_id:{scene_id}/activate'
+        put(url, headers=self.auth_headers, timeout=5)
```

### Comparing `lifx_cli-2.1.0/.gitignore` & `lifx_cli-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.1.0/LICENSE` & `lifx_cli-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.1.0/README.md` & `lifx_cli-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.1.0/pyproject.toml` & `lifx_cli-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifx-cli"
-version = "2.1.0"
+version = "2.4.0"
 authors = [{name="Wes Henderson", email="info@necrux.com"}]
 description = "The Unofficial LIFX CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'requests',
   'tabulate',
```

### Comparing `lifx_cli-2.1.0/PKG-INFO` & `lifx_cli-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifx-cli
-Version: 2.1.0
+Version: 2.4.0
 Summary: The Unofficial LIFX CLI
 Project-URL: Homepage, https://github.com/necrux/lifx-cli
 Project-URL: Bug Tracker, https://github.com/necrux/lifx-cli/issues
 Author-email: Wes Henderson <info@necrux.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

