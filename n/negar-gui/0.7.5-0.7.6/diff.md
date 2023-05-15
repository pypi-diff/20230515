# Comparing `tmp/negar-gui-0.7.5.tar.gz` & `tmp/negar-gui-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negar-gui-0.7.5.tar", last modified: Wed Apr 19 22:18:20 2023, max compression
+gzip compressed data, was "negar-gui-0.7.6.tar", last modified: Mon May 15 16:20:31 2023, max compression
```

## Comparing `negar-gui-0.7.5.tar` & `negar-gui-0.7.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-04-19 22:18:20.322585 negar-gui-0.7.5/
--rw-r--r--   0 javad     (1000) javad     (1000)    35149 2023-04-01 17:16:18.000000 negar-gui-0.7.5/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1000)      121 2023-04-01 17:16:18.000000 negar-gui-0.7.5/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-04-19 22:18:20.322585 negar-gui-0.7.5/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)     2399 2023-04-01 17:16:18.000000 negar-gui-0.7.5/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-04-19 22:18:20.322585 negar-gui-0.7.5/negar_gui/
--rw-r--r--   0 javad     (1000) javad     (1000)     2280 2023-04-01 17:16:18.000000 negar-gui-0.7.5/negar_gui/Ui_hwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)    35703 2023-04-07 20:19:39.000000 negar-gui-0.7.5/negar_gui/Ui_mwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)     2960 2023-04-07 20:19:39.000000 negar-gui-0.7.5/negar_gui/Ui_uwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)        0 2023-04-01 17:16:18.000000 negar-gui-0.7.5/negar_gui/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)      257 2023-04-19 21:30:07.000000 negar-gui-0.7.5/negar_gui/constants.py
--rw-r--r--   0 javad     (1000) javad     (1000)    16208 2023-04-01 17:16:18.000000 negar-gui-0.7.5/negar_gui/gui.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-04-19 22:18:20.322585 negar-gui-0.7.5/negar_gui/icons/
--rw-r--r--   0 javad     (1000) javad     (1000)     1551 2023-04-01 17:20:04.000000 negar-gui-0.7.5/negar_gui/icons/logo.png
--rw-r--r--   0 javad     (1000) javad     (1000)    25042 2023-04-19 21:25:19.000000 negar-gui-0.7.5/negar_gui/main.py
--rw-r--r--   0 javad     (1000) javad     (1000)   301781 2023-04-19 21:10:47.000000 negar-gui-0.7.5/negar_gui/resource_rc.py
--rw-r--r--   0 javad     (1000) javad     (1000)     4938 2023-04-01 17:16:18.000000 negar-gui-0.7.5/negar_gui/style.qss
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-04-19 22:18:20.322585 negar-gui-0.7.5/negar_gui/ts/
--rw-r--r--   0 javad     (1000) javad     (1000)     5234 2023-04-01 17:20:04.000000 negar-gui-0.7.5/negar_gui/ts/fa.qm
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-04-19 22:18:20.322585 negar-gui-0.7.5/negar_gui.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-04-19 22:18:20.000000 negar-gui-0.7.5/negar_gui.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)      470 2023-04-19 22:18:20.000000 negar-gui-0.7.5/negar_gui.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-04-19 22:18:20.000000 negar-gui-0.7.5/negar_gui.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       85 2023-04-19 22:18:20.000000 negar-gui-0.7.5/negar_gui.egg-info/entry_points.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       84 2023-04-19 22:18:20.000000 negar-gui-0.7.5/negar_gui.egg-info/requires.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       10 2023-04-19 22:18:20.000000 negar-gui-0.7.5/negar_gui.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-04-19 22:18:20.322585 negar-gui-0.7.5/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1000)     1153 2023-04-01 17:20:04.000000 negar-gui-0.7.5/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/
+-rw-r--r--   0 javad     (1000) javad     (1000)    35149 2023-04-01 17:16:18.000000 negar-gui-0.7.6/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1000)      121 2023-04-01 17:16:18.000000 negar-gui-0.7.6/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-05-15 16:20:31.819549 negar-gui-0.7.6/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)     2399 2023-04-01 17:16:18.000000 negar-gui-0.7.6/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/negar_gui/
+-rw-r--r--   0 javad     (1000) javad     (1000)     2280 2023-04-01 17:16:18.000000 negar-gui-0.7.6/negar_gui/Ui_hwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    35703 2023-04-07 20:19:39.000000 negar-gui-0.7.6/negar_gui/Ui_mwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     2960 2023-04-07 20:19:39.000000 negar-gui-0.7.6/negar_gui/Ui_uwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)        0 2023-04-01 17:16:18.000000 negar-gui-0.7.6/negar_gui/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)      257 2023-05-15 13:26:58.000000 negar-gui-0.7.6/negar_gui/constants.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    16208 2023-04-01 17:16:18.000000 negar-gui-0.7.6/negar_gui/gui.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/negar_gui/icons/
+-rw-r--r--   0 javad     (1000) javad     (1000)     1551 2023-04-01 17:20:04.000000 negar-gui-0.7.6/negar_gui/icons/logo.png
+-rw-r--r--   0 javad     (1000) javad     (1000)    25360 2023-05-15 13:26:27.000000 negar-gui-0.7.6/negar_gui/main.py
+-rw-r--r--   0 javad     (1000) javad     (1000)   301781 2023-05-15 13:23:51.000000 negar-gui-0.7.6/negar_gui/resource_rc.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     4938 2023-04-01 17:16:18.000000 negar-gui-0.7.6/negar_gui/style.qss
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/negar_gui/ts/
+-rw-r--r--   0 javad     (1000) javad     (1000)     5234 2023-04-01 17:20:04.000000 negar-gui-0.7.6/negar_gui/ts/fa.qm
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/negar_gui.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)      470 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       85 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/entry_points.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       84 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/requires.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       10 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-05-15 16:20:31.819549 negar-gui-0.7.6/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1000)     1153 2023-04-01 17:20:04.000000 negar-gui-0.7.6/setup.py
```

### Comparing `negar-gui-0.7.5/LICENSE` & `negar-gui-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/PKG-INFO` & `negar-gui-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negar-gui
-Version: 0.7.5
+Version: 0.7.6
 Summary: Graphical User Interface for Negar -- Persian Text Editor
 Home-page: http://github.com/javadr/negar-gui
 Author: Javad Razavian
 Author-email: javadr@gmail.com
 License: GPLv3
 Keywords: Spellcheck Persian Text-Editor
 Platform: UNKNOWN
```

### Comparing `negar-gui-0.7.5/README.md` & `negar-gui-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/negar_gui/Ui_hwin.py` & `negar-gui-0.7.6/negar_gui/Ui_hwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/negar_gui/Ui_mwin.py` & `negar-gui-0.7.6/negar_gui/Ui_mwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/negar_gui/Ui_uwin.py` & `negar-gui-0.7.6/negar_gui/Ui_uwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/negar_gui/gui.py` & `negar-gui-0.7.6/negar_gui/gui.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/negar_gui/icons/logo.png` & `negar-gui-0.7.6/negar_gui/icons/logo.png`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/negar_gui/main.py` & `negar-gui-0.7.6/negar_gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 #!/usr/bin/env python
 
+'''
+negar-gui
+
+Usage:
+    negar-gui -h
+    negar-gui -v
+    negar-gui
+
+Options:
+    -h, --help          Show this screen.
+    -v, --version       Show version and exit
+'''
+
 import re
 import sys
+from docopt import docopt
 import asyncio
 import requests
 from threading import Thread
 from pathlib import Path
 import tempfile
 from pyuca import Collator
 from pyperclip import copy as pyclipcopy
@@ -536,15 +550,20 @@
 def statusBar_Timeout(self, notification, timeout=5000): # Timeout in milliseconds
     self.statusBar.showMessage(notification, timeout)
     timer = QTimer()
     timer.setSingleShot( True )
     timer.timeout.connect( self.statusBar.clearMessage )
     timer.start(timeout)
 
-def main():
+def main(args=docopt(__doc__)):
+
+    if args['--version']:
+        print (f"negar-gui, Version {__version__}")
+        sys.exit()
+
     global MainWindow
     qdarktheme.enable_hi_dpi()
     app = QApplication(sys.argv)
     qdarktheme.setup_theme("dark")
     MainWindow = MyWindow()
     MainWindow.show()
     sys.exit(app.exec_())
```

### Comparing `negar-gui-0.7.5/negar_gui/resource_rc.py` & `negar-gui-0.7.6/negar_gui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/negar_gui/style.qss` & `negar-gui-0.7.6/negar_gui/style.qss`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/negar_gui/ts/fa.qm` & `negar-gui-0.7.6/negar_gui/ts/fa.qm`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.5/negar_gui.egg-info/PKG-INFO` & `negar-gui-0.7.6/negar_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negar-gui
-Version: 0.7.5
+Version: 0.7.6
 Summary: Graphical User Interface for Negar -- Persian Text Editor
 Home-page: http://github.com/javadr/negar-gui
 Author: Javad Razavian
 Author-email: javadr@gmail.com
 License: GPLv3
 Keywords: Spellcheck Persian Text-Editor
 Platform: UNKNOWN
```

### Comparing `negar-gui-0.7.5/setup.py` & `negar-gui-0.7.6/setup.py`

 * *Files identical despite different names*

