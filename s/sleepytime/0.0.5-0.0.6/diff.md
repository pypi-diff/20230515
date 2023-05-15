# Comparing `tmp/sleepytime-0.0.5.tar.gz` & `tmp/sleepytime-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepytime-0.0.5.tar", last modified: Thu Jan 12 23:47:56 2023, max compression
+gzip compressed data, was "sleepytime-0.0.6.tar", last modified: Mon May 15 04:49:42 2023, max compression
```

## Comparing `sleepytime-0.0.5.tar` & `sleepytime-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-12 23:47:56.363845 sleepytime-0.0.5/
--rw-rw-rw-   0        0        0     1094 2023-01-12 23:47:24.000000 sleepytime-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1166 2023-01-12 23:47:56.363845 sleepytime-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-01-12 23:47:24.000000 sleepytime-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-01-12 23:47:56.363845 sleepytime-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1028 2023-01-12 23:47:24.000000 sleepytime-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-12 23:47:56.363845 sleepytime-0.0.5/sleepytime/
--rw-rw-rw-   0        0        0        0 2023-01-12 23:47:24.000000 sleepytime-0.0.5/sleepytime/__init__.py
--rw-rw-rw-   0        0        0      484 2023-01-12 23:47:24.000000 sleepytime-0.0.5/sleepytime/__main__.py
--rw-rw-rw-   0        0        0       23 2023-01-12 23:47:24.000000 sleepytime-0.0.5/sleepytime/__version__.py
--rw-rw-rw-   0        0        0     3396 2023-01-12 23:47:24.000000 sleepytime-0.0.5/sleepytime/gui.py
-drwxrwxrwx   0        0        0        0 2023-01-12 23:47:56.363845 sleepytime-0.0.5/sleepytime.egg-info/
--rw-rw-rw-   0        0        0     1166 2023-01-12 23:47:56.000000 sleepytime-0.0.5/sleepytime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-01-12 23:47:56.000000 sleepytime-0.0.5/sleepytime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-12 23:47:56.000000 sleepytime-0.0.5/sleepytime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-01-12 23:47:56.000000 sleepytime-0.0.5/sleepytime.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-12 23:47:56.000000 sleepytime-0.0.5/sleepytime.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 04:49:42.966699 sleepytime-0.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-05-15 04:49:13.000000 sleepytime-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1166 2023-05-15 04:49:42.966699 sleepytime-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-05-15 04:49:13.000000 sleepytime-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 04:49:42.966699 sleepytime-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2023-05-15 04:49:13.000000 sleepytime-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 04:49:42.966699 sleepytime-0.0.6/sleepytime/
+-rw-rw-rw-   0        0        0        0 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/__init__.py
+-rw-rw-rw-   0        0        0      484 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/__version__.py
+-rw-rw-rw-   0        0        0     3510 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/gui.py
+-rw-rw-rw-   0        0        0     2628 2023-05-15 04:49:13.000000 sleepytime-0.0.6/sleepytime/resume_watcher.py
+drwxrwxrwx   0        0        0        0 2023-05-15 04:49:42.966699 sleepytime-0.0.6/sleepytime.egg-info/
+-rw-rw-rw-   0        0        0     1166 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 04:49:42.000000 sleepytime-0.0.6/sleepytime.egg-info/top_level.txt
```

### Comparing `sleepytime-0.0.5/LICENSE` & `sleepytime-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepytime-0.0.5/PKG-INFO` & `sleepytime-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepytime
-Version: 0.0.5
+Version: 0.0.6
 Home-page: http://github.com/csm10495/sleepytime
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `sleepytime-0.0.5/README.md` & `sleepytime-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sleepytime-0.0.5/setup.py` & `sleepytime-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `sleepytime-0.0.5/sleepytime/gui.py` & `sleepytime-0.0.6/sleepytime/gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import sys
 import time
 
 import PySimpleGUI as sg
 from psgtray import SystemTray
 
 from .__version__ import __version__
+from .resume_watcher import ResumeWatcher
 
 DELAY_TEXT = "Delay"
 HIBERNATE_TEXT = "Hibernate"
 DELAY_TIMEDELTA = datetime.timedelta(hours=1)
 
 if os.name != "nt":
     raise NotImplementedError(
@@ -76,14 +77,15 @@
         menu=["", ["Exit"]],
         tooltip=f"SleepTime {__version__} is running...",
         window=window,
     )
 
     death_time = time.time() + countdown
     unhide_time = None
+    resume_watcher = ResumeWatcher()
 
     try:
         while time.time() < death_time:
             event, values = window.read(timeout=500)
             # print(event, values)
 
             window["countdown"].update(
@@ -103,16 +105,16 @@
                 sys_tray.set_tooltip(f"Sleeping until: {unhide_time}")
                 death_time = 999999999999999999999
 
             elif event == HIBERNATE_TEXT:
                 hibernate_and_exit()
             elif (
                 event in (sg.WIN_CLOSED, "Exit")
-                or event == SystemTray.DEFAULT_KEY
-                and values[sys_tray.key] == "Exit"
+                or (event == SystemTray.DEFAULT_KEY and values[sys_tray.key] == "Exit")
+                or resume_watcher.is_resumed()
             ):
                 break
             elif event == sg.EVENT_TIMEOUT:
                 continue
         else:
             hibernate_and_exit()
     finally:
```

### Comparing `sleepytime-0.0.5/sleepytime.egg-info/PKG-INFO` & `sleepytime-0.0.6/sleepytime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepytime
-Version: 0.0.5
+Version: 0.0.6
 Home-page: http://github.com/csm10495/sleepytime
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
```

