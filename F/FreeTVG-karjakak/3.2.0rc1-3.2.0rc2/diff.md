# Comparing `tmp/FreeTVG-karjakak-3.2.0rc1.tar.gz` & `tmp/FreeTVG-karjakak-3.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.2.0rc1.tar", last modified: Sun May 14 10:01:54 2023, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.2.0rc2.tar", last modified: Mon May 15 01:16:41 2023, max compression
```

## Comparing `FreeTVG-karjakak-3.2.0rc1.tar` & `FreeTVG-karjakak-3.2.0rc2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.151575 FreeTVG-karjakak-3.2.0rc1/
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.147400 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      483 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-r--r--   0 karja      (501) staff       (20)      118 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-14 10:01:54.000000 FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.0rc1/LICENSE.txt
--rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-14 10:01:54.151651 FreeTVG-karjakak-3.2.0rc1/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.0rc1/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.149397 FreeTVG-karjakak-3.2.0rc1/TVG/
--rw-r--r--   0 karja      (501) staff       (20)   144471 2023-05-14 09:35:11.000000 FreeTVG-karjakak-3.2.0rc1/TVG/FreeTVG.py
--rw-r--r--   0 karja      (501) staff       (20)   359943 2023-01-16 15:03:13.000000 FreeTVG-karjakak-3.2.0rc1/TVG/Tutorial TVG.pdf
--rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.0rc1/TVG/__init__.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.150027 FreeTVG-karjakak-3.2.0rc1/TVG/structure/
--rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.0rc1/TVG/structure/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)    14763 2023-05-14 09:14:42.000000 FreeTVG-karjakak-3.2.0rc1/TVG/structure/frame_layouts.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-14 10:01:54.151347 FreeTVG-karjakak-3.2.0rc1/TVG/utility/
--rw-r--r--   0 karja      (501) staff       (20)     1091 2022-12-04 14:36:50.000000 FreeTVG-karjakak-3.2.0rc1/TVG/utility/RegMail.py
--rw-r--r--   0 karja      (501) staff       (20)      110 2022-11-22 15:56:19.000000 FreeTVG-karjakak-3.2.0rc1/TVG/utility/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     5639 2023-01-12 09:34:49.000000 FreeTVG-karjakak-3.2.0rc1/TVG/utility/mdh.py
--rw-r--r--   0 karja      (501) staff       (20)     1174 2022-11-23 15:06:38.000000 FreeTVG-karjakak-3.2.0rc1/TVG/utility/term.py
--rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.0rc1/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      944 2023-05-14 10:01:54.151941 FreeTVG-karjakak-3.2.0rc1/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.223241 FreeTVG-karjakak-3.2.0rc2/
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.218464 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      483 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-r--r--   0 karja      (501) staff       (20)      118 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-15 01:16:41.000000 FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.0rc2/LICENSE.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-15 01:16:41.223346 FreeTVG-karjakak-3.2.0rc2/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.0rc2/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.220230 FreeTVG-karjakak-3.2.0rc2/TVG/
+-rw-r--r--   0 karja      (501) staff       (20)   144548 2023-05-15 01:09:49.000000 FreeTVG-karjakak-3.2.0rc2/TVG/FreeTVG.py
+-rw-r--r--   0 karja      (501) staff       (20)   359943 2023-01-16 15:03:13.000000 FreeTVG-karjakak-3.2.0rc2/TVG/Tutorial TVG.pdf
+-rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.0rc2/TVG/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.221588 FreeTVG-karjakak-3.2.0rc2/TVG/structure/
+-rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.0rc2/TVG/structure/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)    14809 2023-05-14 14:20:14.000000 FreeTVG-karjakak-3.2.0rc2/TVG/structure/frame_layouts.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 01:16:41.222992 FreeTVG-karjakak-3.2.0rc2/TVG/utility/
+-rw-r--r--   0 karja      (501) staff       (20)     1091 2022-12-04 14:36:50.000000 FreeTVG-karjakak-3.2.0rc2/TVG/utility/RegMail.py
+-rw-r--r--   0 karja      (501) staff       (20)      110 2022-11-22 15:56:19.000000 FreeTVG-karjakak-3.2.0rc2/TVG/utility/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     5639 2023-01-12 09:34:49.000000 FreeTVG-karjakak-3.2.0rc2/TVG/utility/mdh.py
+-rw-r--r--   0 karja      (501) staff       (20)     1174 2022-11-23 15:06:38.000000 FreeTVG-karjakak-3.2.0rc2/TVG/utility/term.py
+-rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.0rc2/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      944 2023-05-15 01:16:41.223645 FreeTVG-karjakak-3.2.0rc2/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.2.0rc1/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.2.0rc2/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.0rc1/LICENSE.txt` & `FreeTVG-karjakak-3.2.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc1/PKG-INFO` & `FreeTVG-karjakak-3.2.0rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.0rc1/README.md` & `FreeTVG-karjakak-3.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc1/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.2.0rc2/TVG/FreeTVG.py`

 * *Files 0% similar despite different names*

```diff
@@ -2735,33 +2735,35 @@
         del ckf, fl, f
 
     def reblist(self, fon: str):
         """Destroy Listbox and rebuild it again,
         for font in listbox to be appear correctly
         """
 
+        tlframe = self.tframe.tlframe
         self.listb.destroy()
         self.listb = Listbox(
-            self.tlframe,
+            tlframe,
             background=self.text["background"],
             foreground=self.text["foreground"],
             font=fon,
+            exportselection=False,
         )
         self.listb.pack(side=LEFT, fill="both", expand=1)
         self.listb.pack_propagate(0)
         self.bt["listb"] = self.listb
         self.listb.config(yscrollcommand=self.scrollbar2.set)
         self.scrollbar2.config(command=self.listb.yview)
         self.listb.bind("<<ListboxSelect>>", self.infobar)
         self.listb.bind("<MouseWheel>", self.mscrl)
         self.listb.bind("<Up>", self.mscrl)
         self.listb.bind("<Down>", self.mscrl)
         self.listb.bind("<FocusIn>", self.flb)
         self.listb.update()
-        del fon
+        del fon, tlframe
 
     def ft(self, event=None, path=None):
         """Initial starting fonts chooser"""
 
         if path:
             with open(path) as rd:
                 self.clb(rd.read(), wr=False)
```

### Comparing `FreeTVG-karjakak-3.2.0rc1/TVG/Tutorial TVG.pdf` & `FreeTVG-karjakak-3.2.0rc2/TVG/Tutorial TVG.pdf`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc1/TVG/structure/frame_layouts.py` & `FreeTVG-karjakak-3.2.0rc2/TVG/structure/frame_layouts.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     StringVar,
     X,
     ttk,
     Text,
     Listbox,
     CENTER,
 )
-from excptr import DEFAULTDIR, DEFAULTFILE, DIRPATH, excp, excpcls
+from excptr import DEFAULTDIR, DEFAULTFILE, DIRPATH, excpcls
 
 DEFAULTDIR = os.path.join(DIRPATH, "FreeTVG_TRACE")
 if not os.path.exists(DEFAULTDIR):
     os.mkdir(DEFAULTDIR)
 DEFAULTFILE = os.path.join(DEFAULTDIR, Path(DEFAULTFILE).name)
 
 
@@ -276,14 +276,15 @@
         self.sc2frame = ttk.Frame(self, width=scw)
         self.sc2frame.pack(anchor="w", side=LEFT, fill="y", pady=1)
         self.sc2frame.pack_propagate(0)
         self.scrollbar2 = ttk.Scrollbar(self.sc2frame, orient="vertical")
         self.scrollbar2.config(command=self.listb.yview)
         self.scrollbar2.pack(side="left", fill="y")
         self.listb.config(yscrollcommand=self.scrollbar2.set)
+        del frw, lbw, scw
 
 
 @excpcls(m=2, filenm=DEFAULTFILE)
 class Lay8(ttk.Frame):
     def __init__(self, root):
         super().__init__()
         frw = int(round(root.winfo_screenwidth() * 0.9224011713030746))
@@ -306,14 +307,15 @@
             anchor=CENTER,
             textvariable=self.info,
             font="consolas 10 bold",
             justify=CENTER,
         )
         self.labcor.pack(side=LEFT, fill="x", expand=1)
         self.labcor.propagate(0)
+        del frw, lbw, scw
 
 
 @excpcls(m=2, filenm=DEFAULTFILE)
 class Scribe:
     def scribe(self):
         return {
             "Insert": "Insert word in outline on selected row",
```

### Comparing `FreeTVG-karjakak-3.2.0rc1/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.2.0rc2/TVG/utility/RegMail.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc1/TVG/utility/mdh.py` & `FreeTVG-karjakak-3.2.0rc2/TVG/utility/mdh.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc1/TVG/utility/term.py` & `FreeTVG-karjakak-3.2.0rc2/TVG/utility/term.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.0rc1/setup.cfg` & `FreeTVG-karjakak-3.2.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FreeTVG-karjakak
-version = 3.2.0rc1
+version = 3.2.0rc2
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Tree View Gui for outline treeview note.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG#latest-notice
 license = MIT License
```

