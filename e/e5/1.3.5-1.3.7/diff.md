# Comparing `tmp/e5-1.3.5.tar.gz` & `tmp/e5-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\mcpherro\Local\Source\Python3\e5py\dist\tmpa_n008au\e5-1.3.5.tar", last modified: Wed Jul 13 12:16:12 2022, max compression
+gzip compressed data, was "C:\Users\mcpherro\Local\Source\Python3\e5py\dist\tmpdi9c9q6h\e5-1.3.7.tar", last modified: Wed Jul 20 18:08:49 2022, max compression
```

## Comparing `e5-1.3.5.tar` & `e5-1.3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-07-13 12:16:12.466351 e5-1.3.5/
--rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 e5-1.3.5/LICENSE
--rw-rw-rw-   0        0        0    15906 2022-07-13 12:16:12.467330 e5-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    15007 2022-06-17 13:53:30.000000 e5-1.3.5/README.md
--rw-rw-rw-   0        0        0      521 2022-06-17 13:03:27.000000 e5-1.3.5/pyproject.toml
--rw-rw-rw-   0        0        0     1206 2022-07-13 12:16:12.477093 e5-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 e5-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-13 12:16:12.369677 e5-1.3.5/src/
-drwxrwxrwx   0        0        0        0 2022-07-13 12:16:12.433150 e5-1.3.5/src/e5.egg-info/
--rw-rw-rw-   0        0        0    15906 2022-07-13 12:16:12.000000 e5-1.3.5/src/e5.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2022-07-13 12:16:12.000000 e5-1.3.5/src/e5.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-13 12:16:12.000000 e5-1.3.5/src/e5.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-17 13:08:38.000000 e5-1.3.5/src/e5.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      117 2022-07-13 12:16:12.000000 e5-1.3.5/src/e5.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-07-13 12:16:12.000000 e5-1.3.5/src/e5.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-13 12:16:12.448775 e5-1.3.5/src/e5py/
--rw-rw-rw-   0        0        0        0 2022-06-13 13:41:36.000000 e5-1.3.5/src/e5py/__init__.py
--rw-rw-rw-   0        0        0      171 2022-06-17 13:36:22.000000 e5-1.3.5/src/e5py/__main__.py
--rw-rw-rw-   0        0        0     9555 2022-06-14 12:57:16.000000 e5-1.3.5/src/e5py/e5.kv
--rw-rw-rw-   0        0        0    70976 2022-07-13 12:12:19.000000 e5-1.3.5/src/e5py/e5.py
-drwxrwxrwx   0        0        0        0 2022-07-13 12:16:12.465376 e5-1.3.5/src/e5py/lib/
--rw-rw-rw-   0        0        0     4208 2022-06-17 13:12:45.000000 e5-1.3.5/src/e5py/lib/blockdata.py
--rw-rw-rw-   0        0        0     4284 2022-06-17 13:15:05.000000 e5-1.3.5/src/e5py/lib/colorscheme.py
--rw-rw-rw-   0        0        0     1437 2022-06-17 13:12:24.000000 e5-1.3.5/src/e5py/lib/constants.py
--rw-rw-rw-   0        0        0     3454 2022-06-14 13:13:15.000000 e5-1.3.5/src/e5py/lib/dbs.py
--rw-rw-rw-   0        0        0   102862 2022-06-17 13:13:48.000000 e5-1.3.5/src/e5py/lib/e5_widgets.py
--rw-rw-rw-   0        0        0     1772 2022-06-08 15:04:53.000000 e5-1.3.5/src/e5py/lib/misc.py
+drwxrwxrwx   0        0        0        0 2022-07-20 18:08:49.025666 e5-1.3.7/
+-rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 e5-1.3.7/LICENSE
+-rw-rw-rw-   0        0        0    15906 2022-07-20 18:08:49.026666 e5-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    15007 2022-06-17 13:53:30.000000 e5-1.3.7/README.md
+-rw-rw-rw-   0        0        0      521 2022-06-17 13:03:27.000000 e5-1.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1206 2022-07-20 18:08:49.029668 e5-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 e5-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-20 18:08:48.926666 e5-1.3.7/src/
+drwxrwxrwx   0        0        0        0 2022-07-20 18:08:48.978665 e5-1.3.7/src/e5.egg-info/
+-rw-rw-rw-   0        0        0    15906 2022-07-20 18:08:48.000000 e5-1.3.7/src/e5.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2022-07-20 18:08:48.000000 e5-1.3.7/src/e5.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-20 18:08:48.000000 e5-1.3.7/src/e5.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-17 13:08:38.000000 e5-1.3.7/src/e5.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      117 2022-07-20 18:08:48.000000 e5-1.3.7/src/e5.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-07-20 18:08:48.000000 e5-1.3.7/src/e5.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-20 18:08:48.987666 e5-1.3.7/src/e5py/
+-rw-rw-rw-   0        0        0        0 2022-06-13 13:41:36.000000 e5-1.3.7/src/e5py/__init__.py
+-rw-rw-rw-   0        0        0      171 2022-06-17 13:36:22.000000 e5-1.3.7/src/e5py/__main__.py
+-rw-rw-rw-   0        0        0     9555 2022-06-14 12:57:16.000000 e5-1.3.7/src/e5py/e5.kv
+-rw-rw-rw-   0        0        0    72012 2022-07-20 18:06:29.000000 e5-1.3.7/src/e5py/e5.py
+drwxrwxrwx   0        0        0        0 2022-07-20 18:08:49.024665 e5-1.3.7/src/e5py/lib/
+-rw-rw-rw-   0        0        0     4208 2022-06-17 13:12:45.000000 e5-1.3.7/src/e5py/lib/blockdata.py
+-rw-rw-rw-   0        0        0     4284 2022-06-17 13:15:05.000000 e5-1.3.7/src/e5py/lib/colorscheme.py
+-rw-rw-rw-   0        0        0     1437 2022-06-17 13:12:24.000000 e5-1.3.7/src/e5py/lib/constants.py
+-rw-rw-rw-   0        0        0     3454 2022-06-14 13:13:15.000000 e5-1.3.7/src/e5py/lib/dbs.py
+-rw-rw-rw-   0        0        0   102862 2022-06-17 13:13:48.000000 e5-1.3.7/src/e5py/lib/e5_widgets.py
+-rw-rw-rw-   0        0        0     1772 2022-06-08 15:04:53.000000 e5-1.3.7/src/e5py/lib/misc.py
```

### Comparing `e5-1.3.5/LICENSE` & `e5-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `e5-1.3.5/PKG-INFO` & `e5-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e5
-Version: 1.3.5
+Version: 1.3.7
 Summary: Configurable data entry program for archaeology
 Home-page: https://github.com/surf3s/E5
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/E5/issues
 Platform: unix
```

### Comparing `e5-1.3.5/README.md` & `e5-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `e5-1.3.5/pyproject.toml` & `e5-1.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `e5-1.3.5/setup.cfg` & `e5-1.3.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 350d 0a64 6573 6372 6970 7469   = e5..descripti
 00000020: 6f6e 203d 2043 6f6e 6669 6775 7261 626c  on = Configurabl
 00000030: 6520 6461 7461 2065 6e74 7279 2070 726f  e data entry pro
 00000040: 6772 616d 2066 6f72 2061 7263 6861 656f  gram for archaeo
 00000050: 6c6f 6779 0d0a 7665 7273 696f 6e20 3d20  logy..version = 
-00000060: 312e 332e 350d 0a61 7574 686f 7220 3d20  1.3.5..author = 
+00000060: 312e 332e 370d 0a61 7574 686f 7220 3d20  1.3.7..author = 
 00000070: 5368 616e 6e6f 6e20 502e 204d 6350 6865  Shannon P. McPhe
 00000080: 7272 6f6e 0d0a 6175 7468 6f72 5f65 6d61  rron..author_ema
 00000090: 696c 203d 206d 6370 6865 7272 6f6e 4065  il = mcpherron@e
 000000a0: 7661 2e6d 7067 2e64 650d 0a6c 6f6e 675f  va.mpg.de..long_
 000000b0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 000000c0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 000000d0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
```

### Comparing `e5-1.3.5/src/e5.egg-info/PKG-INFO` & `e5-1.3.7/src/e5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e5
-Version: 1.3.5
+Version: 1.3.7
 Summary: Configurable data entry program for archaeology
 Home-page: https://github.com/surf3s/E5
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/E5/issues
 Platform: unix
```

### Comparing `e5-1.3.5/src/e5py/e5.kv` & `e5-1.3.7/src/e5py/e5.kv`

 * *Files identical despite different names*

### Comparing `e5-1.3.5/src/e5py/e5.py` & `e5-1.3.7/src/e5py/e5.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,20 @@
 
 # Long term
 #   Consider putting a dropdown menu into the grid view for sorting and maybe searching
 #   Think about whether to allow editing of CFG in the program
 
 # TODO Need to fix ASAP conditions in e4 not comma delimited
 
-__version__ = '1.3.5'
+__version__ = '1.3.7'
 __date__ = 'July, 2022'
 __program__ = 'E5'
 
 # region Imports
+from kivy.config import Config
 from kivy import resources
 from kivy.clock import Clock, mainthread
 from kivy.app import App
 from kivy.uix.switch import Switch
 from kivy.factory import Factory
 from kivy.uix.popup import Popup
 from kivy.uix.screenmanager import ScreenManager, Screen
@@ -615,34 +616,46 @@
         return(self.has_errors)
 
     # Pull the conditions appart into a list of objects
     # that make it easier to evaluate.
     def format_conditions(self, conditions):
         formatted_conditions = []
         for condition in conditions:
-            condition_parsed = condition.split(' ')
-            condition_parsed = self.clean_menu(condition_parsed)
-            formatted_condition = a_condition()
-            if len(condition_parsed) > 1:
-                formatted_condition.match_field = condition_parsed[0].upper()
-                if condition_parsed[1].upper() == 'NOT':
-                    formatted_condition.negate_it = True
-                    if len(condition_parsed) > 2:
-                        formatted_condition.match_list = condition_parsed[2].upper().split(',')
+            condition_parsed = []
+            if ' ' in condition:
+                condition_parsed.append(condition[:condition.find(' ')])
+                condition = condition[condition.find(' '):].strip()
+                if condition[:3].upper() == 'NOT':
+                    condition_parsed.append('NOT')
+                    condition = condition[3:]
+                if condition.upper().endswith(' OR'):
+                    condition = condition[:-3]
+                    condition_parsed.append(condition.strip())
+                    condition_parsed.append('OR')
                 else:
-                    formatted_condition.match_list = condition_parsed[1].upper().split(',')
-                if formatted_condition.negate_it and len(condition_parsed) == 4:
-                    if condition_parsed[3].upper() == 'OR':
-                        formatted_condition.or_it = True
-                elif not formatted_condition.negate_it and len(condition_parsed) == 3:
-                    if condition_parsed[2].upper() == 'OR':
-                        formatted_condition.or_it = True
-                if formatted_condition.match_list:
-                    formatted_condition.match_list = self.clean_menu(formatted_condition.match_list)
-            formatted_conditions.append(formatted_condition)
+                    condition_parsed.append(condition.strip())
+                condition_parsed = self.clean_menu(condition_parsed)
+                formatted_condition = a_condition()
+                if len(condition_parsed) > 1:
+                    formatted_condition.match_field = condition_parsed[0].upper()
+                    if condition_parsed[1].upper() == 'NOT':
+                        formatted_condition.negate_it = True
+                        if len(condition_parsed) > 2:
+                            formatted_condition.match_list = condition_parsed[2].upper().split(',')
+                    else:
+                        formatted_condition.match_list = condition_parsed[1].upper().split(',')
+                    if formatted_condition.negate_it and len(condition_parsed) == 4:
+                        if condition_parsed[3].upper() == 'OR':
+                            formatted_condition.or_it = True
+                    elif not formatted_condition.negate_it and len(condition_parsed) == 3:
+                        if condition_parsed[2].upper() == 'OR':
+                            formatted_condition.or_it = True
+                    if formatted_condition.match_list:
+                        formatted_condition.match_list = self.clean_menu(formatted_condition.match_list)
+                formatted_conditions.append(formatted_condition)
         return(formatted_conditions)
 
     def gps_location(self):
         logger = logging.getLogger(__name__)
         logger.info('Have location in cfg.is_valid')
 
     def save(self):
@@ -1322,14 +1335,16 @@
             pass
 
     def show_load_cfg(self):
         if self.cfg.filename and self.cfg.path:
             start_path = self.cfg.path
         else:
             start_path = self.ini.get_value(__program__, 'APP_PATH')
+        if not path.exists(start_path):
+            start_path = path.abspath(path.dirname(__file__))
         content = e5_LoadDialog(load = self.load,
                                 cancel = self.dismiss_popup,
                                 start_path = start_path,
                                 button_color = self.colors.button_color,
                                 button_background = self.colors.button_background)
         self.popup = Popup(title = "Load CFG file", content = content,
                             size_hint = (0.9, 0.9))
@@ -1544,18 +1559,21 @@
 
 
 class E5App(App):
 
     def __init__(self, **kwargs):
         super(E5App, self).__init__(**kwargs)
 
-        self.app_path = self.user_data_dir
+        if platform_name() != 'Android':
+            self.app_path = path.abspath(path.dirname(__file__))
+        else:
+            self.app_path = self.user_data_dir
 
     def build(self):
-        sm.add_widget(MainScreen(user_data_dir = self.user_data_dir, name = 'MainScreen'))
+        sm.add_widget(MainScreen(user_data_dir = self.app_path, name = 'MainScreen'))
         sm.current = 'MainScreen'
         self.title = __program__ + " " + __version__
         return(sm)
 
 
 Factory.register(__program__, cls=E5App)
 
@@ -1569,8 +1587,9 @@
 
     return path.join(path.abspath("."))
 
 
 if __name__ == '__main__':
     # This line goes with the function above
     resources.resource_add_path(resourcePath())  # add this line
+    Config.set('input', 'mouse', 'mouse,multitouch_on_demand')      # Removes red dot
     E5App().run()
```

### Comparing `e5-1.3.5/src/e5py/lib/blockdata.py` & `e5-1.3.7/src/e5py/lib/blockdata.py`

 * *Files identical despite different names*

### Comparing `e5-1.3.5/src/e5py/lib/colorscheme.py` & `e5-1.3.7/src/e5py/lib/colorscheme.py`

 * *Files identical despite different names*

### Comparing `e5-1.3.5/src/e5py/lib/constants.py` & `e5-1.3.7/src/e5py/lib/constants.py`

 * *Files identical despite different names*

### Comparing `e5-1.3.5/src/e5py/lib/dbs.py` & `e5-1.3.7/src/e5py/lib/dbs.py`

 * *Files identical despite different names*

### Comparing `e5-1.3.5/src/e5py/lib/e5_widgets.py` & `e5-1.3.7/src/e5py/lib/e5_widgets.py`

 * *Files identical despite different names*

### Comparing `e5-1.3.5/src/e5py/lib/misc.py` & `e5-1.3.7/src/e5py/lib/misc.py`

 * *Files identical despite different names*

