# Comparing `tmp/FreeTVG-karjakak-3.2.0rc2.tar.gz` & `tmp/FreeTVG-karjakak-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.2.0rc2.tar", last modified: Mon May 15 01:16:41 2023, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.2.1.tar", last modified: Mon May 15 12:31:28 2023, max compression
```

## Comparing `FreeTVG-karjakak-3.2.0rc2.tar` & `FreeTVG-karjakak-3.2.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.223241 FreeTVG-karjakak-3.2.0rc2/
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.218464 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      483 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-r--r--   0 karja      (501) staff       (20)      118 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.0rc2/LICENSE.txt
--rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-15 01:16:41.223346 FreeTVG-karjakak-3.2.0rc2/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.0rc2/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.220230 FreeTVG-karjakak-3.2.0rc2/TVG/
--rw-r--r--   0 karja      (501) staff       (20)   144548 2023-05-15 01:09:49.000000 FreeTVG-karjakak-3.2.0rc2/TVG/FreeTVG.py
--rw-r--r--   0 karja      (501) staff       (20)   359943 2023-01-16 15:03:13.000000 FreeTVG-karjakak-3.2.0rc2/TVG/Tutorial TVG.pdf
--rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.0rc2/TVG/__init__.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.221588 FreeTVG-karjakak-3.2.0rc2/TVG/structure/
--rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.0rc2/TVG/structure/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)    14809 2023-05-14 14:20:14.000000 FreeTVG-karjakak-3.2.0rc2/TVG/structure/frame_layouts.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.222992 FreeTVG-karjakak-3.2.0rc2/TVG/utility/
--rw-r--r--   0 karja      (501) staff       (20)     1091 2022-12-04 14:36:50.000000 FreeTVG-karjakak-3.2.0rc2/TVG/utility/RegMail.py
--rw-r--r--   0 karja      (501) staff       (20)      110 2022-11-22 15:56:19.000000 FreeTVG-karjakak-3.2.0rc2/TVG/utility/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     5639 2023-01-12 09:34:49.000000 FreeTVG-karjakak-3.2.0rc2/TVG/utility/mdh.py
--rw-r--r--   0 karja      (501) staff       (20)     1174 2022-11-23 15:06:38.000000 FreeTVG-karjakak-3.2.0rc2/TVG/utility/term.py
--rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.0rc2/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      944 2023-05-15 01:16:41.223645 FreeTVG-karjakak-3.2.0rc2/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 12:31:28.041970 FreeTVG-karjakak-3.2.1/
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 12:31:28.037802 FreeTVG-karjakak-3.2.1/FreeTVG_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-15 12:31:28.000000 FreeTVG-karjakak-3.2.1/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-15 12:31:28.000000 FreeTVG-karjakak-3.2.1/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-15 12:31:28.000000 FreeTVG-karjakak-3.2.1/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-15 12:31:28.000000 FreeTVG-karjakak-3.2.1/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-r--r--   0 karja      (501) staff       (20)      136 2023-05-15 12:31:28.000000 FreeTVG-karjakak-3.2.1/FreeTVG_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-15 12:31:28.000000 FreeTVG-karjakak-3.2.1/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.1/LICENSE.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-15 12:31:28.042063 FreeTVG-karjakak-3.2.1/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.1/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 12:31:28.040346 FreeTVG-karjakak-3.2.1/TVG/
+-rw-r--r--   0 karja      (501) staff       (20)   145553 2023-05-15 12:25:33.000000 FreeTVG-karjakak-3.2.1/TVG/FreeTVG.py
+-rw-r--r--   0 karja      (501) staff       (20)   359943 2023-01-16 15:03:13.000000 FreeTVG-karjakak-3.2.1/TVG/Tutorial TVG.pdf
+-rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.1/TVG/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 12:31:28.040854 FreeTVG-karjakak-3.2.1/TVG/structure/
+-rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.1/TVG/structure/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)    15881 2023-05-15 09:34:19.000000 FreeTVG-karjakak-3.2.1/TVG/structure/frame_layouts.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 12:31:28.041690 FreeTVG-karjakak-3.2.1/TVG/utility/
+-rw-r--r--   0 karja      (501) staff       (20)     1091 2022-12-04 14:36:50.000000 FreeTVG-karjakak-3.2.1/TVG/utility/RegMail.py
+-rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.1/TVG/utility/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     5639 2023-01-12 09:34:49.000000 FreeTVG-karjakak-3.2.1/TVG/utility/mdh.py
+-rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.1/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      960 2023-05-15 12:31:28.042348 FreeTVG-karjakak-3.2.1/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.2.1/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.0rc2
+Version: 3.2.1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.0rc2/LICENSE.txt` & `FreeTVG-karjakak-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc2/PKG-INFO` & `FreeTVG-karjakak-3.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.0rc2
+Version: 3.2.1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.0rc2/README.md` & `FreeTVG-karjakak-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc2/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.2.1/TVG/FreeTVG.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import ast
 import importlib
 import json
 import os
 import re
 import string
-import sys
 from datetime import datetime as dt
 from functools import partial
 from itertools import islice
 from pathlib import Path
 from sys import platform
 from tkinter import (
     BROWSE,
@@ -42,24 +41,24 @@
     colorchooser,
     font,
     messagebox,
     simpledialog,
     ttk,
 )
 
+import darkdetect
 import tomlkit
 from treeview import TreeView as tv
 from treeview.dbase import Datab as db
 
 from excptr import DEFAULTDIR, DEFAULTFILE, DIRPATH, excp, excpcls
 
 from .structure import Lay1, Lay2, Lay3, Lay4, Lay5, Lay6, Lay7, Lay8, Scribe
 from .utility.mdh import convhtml
 from .utility.RegMail import composemail, wrwords
-from .utility.term import ctlight
 
 __all__ = ["main"]
 
 
 DEFAULTDIR = os.path.join(DIRPATH, "FreeTVG_TRACE")
 if not os.path.exists(DEFAULTDIR):
     os.mkdir(DEFAULTDIR)
@@ -72,15 +71,15 @@
             print("Add-On for TVG is ready!")
             from addon_tvg import Charts, EvalExp, SumAll
         else:
             print("Add-On for TVG is missing!")
     case _:
         print("Add-On for TVG is missing!")
 
-THEME_MODE = ctlight()
+THEME_MODE = darkdetect.theme().lower()
 
 SELECT_MODE = "extended"
 
 HIDDEN_OPT = False
 
 WRAPPING = "none"
 
@@ -133,14 +132,15 @@
         self.lock = False
         self.unlock = True
         self.store = None
         self.editorsel = None
         self.tpl = None
         self.ai = None
         self.ew = None
+        self.cycle = None
 
         # Creating style "clam" style for TVG
         self.stl = ttk.Style(self.root)
         self.stl.theme_use("clam")
 
         # All root bindings
         self.root.bind_all("<Control-f>", self.fcsent)
@@ -396,14 +396,23 @@
             self.root.register(self.clb),
             "-parent",
             self.root,
         )
 
         # Checking theme mode!
         self.ldmode()
+        self.cycle_theme()
+
+    def cycle_theme(self):
+        """Detecting system theme cycle and apply it to TVG"""
+
+        if darkdetect.theme().lower() != self.tmode:
+            self.tmode = darkdetect.theme().lower()
+            self.ldmode()
+        self.cycle = self.root.after(1000, self.cycle_theme)
 
     def ldmode(self):
         """Dark mode for easing the eye"""
 
         oribg = "#dcdad5"
         chbg = "grey30"
         orifg = "black"
@@ -444,17 +453,48 @@
                 with open(
                     self.glop.joinpath(self.glop.parent, "theme.tvg"), "w"
                 ) as thm:
                     thm.write("#4d4d4d")
                 self.txtcol(
                     path=self.glop.joinpath(self.glop.parent, "theme.tvg"), wr=False
                 )
-            del oribg, chbg, orifg, chfg
         elif self.tmode == "light":
-            self.stl.theme_use("clam")
+            self.stl.configure(
+                ".",
+                background=oribg,
+                foreground=orifg,
+                fieldbackground=oribg,
+                insertcolor=orifg,
+                troughcolor="#bab5ab",
+                arrowcolor=orifg,
+                bordercolor="#9e9a91",
+            )
+            self.stl.map(
+                ".",
+                background=[("background", oribg)],
+            )
+            self.stl.map(
+                "TCombobox",
+                fieldbackground=[("readonly", oribg)],
+                background=[("active", "#eeebe7")],
+                arrowcolor=[("active", "black")],
+            )
+            self.stl.map(
+                "Horizontal.TScrollbar",
+                background=[("active", "#eeebe7")],
+                arrowcolor=[("active", "black")],
+            )
+            self.stl.map(
+                "Vertical.TScrollbar",
+                background=[("active", "#eeebe7")],
+                arrowcolor=[("active", "black")],
+            )
+            self.stl.configure("TEntry", fieldbackground=chfg)
+        del oribg, chbg, orifg, chfg
+        self.root.update()
 
     def ttip(self, event=None):
         """Tooltip for TVG buttons"""
 
         if tx := self.scribe.get(event.widget["text"], None):
 
             def exit():
@@ -634,16 +674,18 @@
         if self.listb.yview()[1] < 1.0:
             self.text.yview_moveto(self.listb.yview()[0])
         else:
             self.text.yview_moveto(self.listb.yview()[1])
 
     def fcsent(self, event=None):
         """Key Bindings to keyboards"""
-
-        fcom = str(self.root.focus_get())
+        try:
+            fcom = str(self.root.focus_get())
+        except:
+            fcom = ""
         if self.FREEZE is False:
             if event.keysym == "f":
                 self.bt["entry"].focus()
             elif event.keysym == "r":
                 self.bt["entry3"].focus()
             elif event.keysym == "t":
                 st = self.listb.curselection()
@@ -2646,14 +2688,19 @@
                     else:
                         with open(
                             os.path.join(self.glop.parent, "geo.tvg"), "wb"
                         ) as geo:
                             geo.write(str({"geo": self.GEO}).encode())
                     del ask
                 self.addonchk()
+            if self.cycle:
+                self.root.after_cancel(self.cycle)
+            self.__delattr__("bt")
+            self.__delattr__("scribe")
+            self.__delattr__("addonb")
             self.root.quit()
         else:
             messagebox.showerror(
                 "TreeViewGui", "Do not exit before a function end!!!", parent=self.root
             )
 
     def txtcol(self, event=None, path=None, wr=True):
@@ -3428,42 +3475,14 @@
         HIDDEN_OPT = cfg["Configure"]["HIDDEN_OPT"]
         WRAPPING = cfg["Configure"]["WRAPPING"]
         CHECKED_BOX = cfg["Configure"]["CHECKED_BOX"]
         del cfg
 
 
 @excp(m=2, filenm=DEFAULTFILE)
-def configuring(args: list):
-    """configuring TVG"""
-
-    match ment := len(args):
-        case ment if ment == 2:
-            _mode(args[1])
-        case _:
-            pass
-    del args, ment
-
-
-@excp(m=2, filenm=DEFAULTFILE)
-def _mode(mode: str):
-    global THEME_MODE
-
-    match mode := mode:
-        case mode if mode.lower() == "dark":
-            if THEME_MODE is True:
-                THEME_MODE = "dark"
-        case mode if mode.lower() == "light":
-            if THEME_MODE is False:
-                THEME_MODE = "light"
-        case _:
-            pass
-    del mode
-
-
-@excp(m=2, filenm=DEFAULTFILE)
 def titlemode(sent: str):
     try:
         cks = string.printable.partition("!")[0] + "_ "
         j = []
         for st in set(sent):
             if st not in cks:
                 return f"Temporer{int(dt.timestamp(dt.today()))}"
@@ -3485,15 +3504,14 @@
     global _addon
     if _addon and _addon.name == "addon_tvg":
         _addon = True
     else:
         _addon = False
 
     findpath()
-    configuring(sys.argv)
     _load_config()
 
     root = Tk()
     root.withdraw()
     # case fontchooser dialog still reacted toward the application sudden exit and cause it to show
     # when application started.
     if root.tk.call("tk", "fontchooser", "configure", "-visible"):
```

### Comparing `FreeTVG-karjakak-3.2.0rc2/TVG/Tutorial TVG.pdf` & `FreeTVG-karjakak-3.2.1/TVG/Tutorial TVG.pdf`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc2/TVG/structure/frame_layouts.py` & `FreeTVG-karjakak-3.2.1/TVG/structure/frame_layouts.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,42 +78,63 @@
                 return True
             else:
                 return False
 
     def radiobut(self, event=None):
         """These are the switches on radio buttons, to apply certain rule on child"""
 
-        case = {"": self.rb.get(), "child": "child", "parent": "parent"}
-        self.entry.config(state="normal")
-        if self.entry.get() in case:
-            if case[self.rb.get()] == "child":
+        match (self.rb.get(), str(self.entry.cget("state")), self.entry.get()):
+            case ("parent", "disable", _):
+                self.entry.config(state="normal")
+                self.entry.insert(0, "parent")
+            case ("child", "disable", _):
+                self.entry.config(state="normal")
+                self.entry.insert(0, "child")
+                self.entry3.config(state="normal")
                 self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
                 self.entry3.current(0)
-            elif case[self.rb.get()] != "child":
-                self.entry3.config(values="")
+                self.entry3.config(state="readonly")
+            case ("parent", _, "child"):
+                self.entry.delete(0, END)
+                self.entry.insert(0, "parent")
                 self.entry3.config(state="normal")
+                self.entry3.config(values="")
                 self.entry3.delete(0, END)
                 self.entry3.config(state="readonly")
-            self.entry.delete(0, END)
-            if len(str(self.entry.focus_get())) > 5:
-                if str(self.entry.focus_get())[-5:] != "entry":
-                    self.entry.insert(0, case[""])
-            else:
-                self.entry.insert(0, case[""])
-        else:
-            if case[self.rb.get()] == "child":
+            case ("child", _, "parent"):
+                self.entry.delete(0, END)
+                self.entry.insert(0, "child")
+                self.entry3.config(state="normal")
                 self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
                 self.entry3.current(0)
-            elif case[self.rb.get()] != "child":
+                self.entry3.config(state="readonly")
+            case ("parent", _, ""):
+                self.entry.insert(0, "parent")
+                self.entry3.config(state="normal")
                 self.entry3.config(values="")
+                self.entry3.delete(0, END)
+                self.entry3.config(state="readonly")
+            case ("child", _, ""):
+                self.entry.insert(0, "child")
                 self.entry3.config(state="normal")
+                self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
+                self.entry3.current(0)
+                self.entry3.config(state="readonly")
+            case ("parent", _, _):
+                self.entry3.config(state="normal")
+                self.entry3.config(values="")
                 self.entry3.delete(0, END)
                 self.entry3.config(state="readonly")
-            self.entry.selection_clear()
-        del case
+            case ("child", _, _):
+                self.entry3.config(state="normal")
+                self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
+                self.entry3.current(0)
+                self.entry3.config(state="readonly")
+
+        self.entry.configure(validate="focusin")
 
 
 @excpcls(m=2, filenm=DEFAULTFILE)
 class Lay2(ttk.Frame):
     def __init__(self, root):
         super().__init__()
         self.pack(side=TOP, fill="x")
```

### Comparing `FreeTVG-karjakak-3.2.0rc2/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.2.1/TVG/utility/RegMail.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc2/TVG/utility/mdh.py` & `FreeTVG-karjakak-3.2.1/TVG/utility/mdh.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc2/setup.cfg` & `FreeTVG-karjakak-3.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FreeTVG-karjakak
-version = 3.2.0rc2
+version = 3.2.1
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Tree View Gui for outline treeview note.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG#latest-notice
 license = MIT License
@@ -24,14 +24,15 @@
 install_requires = 
 	markdown>=3.3.4
 	pymdown-extensions>=9.0
 	treeview-karjakak>=1.8.1
 	excptr-karjakak>=0.1.0
 	demoji>=1.1.0
 	tomlkit>=0.11.6
+	darkdetect>=0.8.0
 
 [options.package_data]
 * = *.pdf
 
 [options.entry_points]
 gui_scripts = 
 	TVG = TVG:main
```

