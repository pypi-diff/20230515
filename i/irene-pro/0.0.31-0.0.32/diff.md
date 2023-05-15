# Comparing `tmp/irene_pro-0.0.31.tar.gz` & `tmp/irene_pro-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.31.tar", last modified: Mon May 15 06:53:32 2023, max compression
+gzip compressed data, was "irene_pro-0.0.32.tar", last modified: Mon May 15 07:05:59 2023, max compression
```

## Comparing `irene_pro-0.0.31.tar` & `irene_pro-0.0.32.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 06:53:32.178219 irene_pro-0.0.31/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.31/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.31/MANIFEST.in
--rw-rw-rw-   0        0        0     1280 2023-05-15 06:53:32.177220 irene_pro-0.0.31/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-05-11 07:56:46.000000 irene_pro-0.0.31/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 06:53:32.126356 irene_pro-0.0.31/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.31/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.31/irene_pro/logic.py
--rw-rw-rw-   0        0        0    24996 2023-05-15 06:50:42.000000 irene_pro-0.0.31/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-15 06:53:32.173232 irene_pro-0.0.31/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1280 2023-05-15 06:53:32.000000 irene_pro-0.0.31/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-15 06:53:32.000000 irene_pro-0.0.31/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 06:53:32.000000 irene_pro-0.0.31/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-15 06:53:32.000000 irene_pro-0.0.31/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 06:53:32.000000 irene_pro-0.0.31/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 06:53:32.179215 irene_pro-0.0.31/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-15 06:52:15.000000 irene_pro-0.0.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:05:59.644385 irene_pro-0.0.32/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.32/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.32/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-05-15 07:05:59.643387 irene_pro-0.0.32/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-05-11 07:56:46.000000 irene_pro-0.0.32/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 07:05:59.623449 irene_pro-0.0.32/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.32/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.32/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    25476 2023-05-15 07:02:25.000000 irene_pro-0.0.32/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:05:59.639398 irene_pro-0.0.32/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-05-15 07:05:59.000000 irene_pro-0.0.32/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-15 07:05:59.000000 irene_pro-0.0.32/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 07:05:59.000000 irene_pro-0.0.32/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-15 07:05:59.000000 irene_pro-0.0.32/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 07:05:59.000000 irene_pro-0.0.32/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 07:05:59.645383 irene_pro-0.0.32/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-15 07:04:42.000000 irene_pro-0.0.32/setup.py
```

### Comparing `irene_pro-0.0.31/PKG-INFO` & `irene_pro-0.0.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.31
+Version: 0.0.32
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.31/README.md` & `irene_pro-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.31/irene_pro/logic.py` & `irene_pro-0.0.32/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.31/irene_pro/widgets.py` & `irene_pro-0.0.32/irene_pro/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,52 +116,67 @@
     def __init__(self, master,image = None, **kwargs):
         super().__init__(master=master, compound = "left", bd = 0,font = w(12),image = image, **kwargs)
         if image:
             image = PhotoImage(file = image)
         # configure save button
         if 'save' in str(self['text']).lower():
             self.config(bg = "#9400D3", fg = "#fff", image = image)
+            self.image = image
         
         elif 'edit' in str(self['text']).lower():
             self.config(bg = "#0b4", fg = "#fff", image = image)
+            self.image = image
 
         elif 'date' in str(self['text']).lower():
             self.config(bg = "#00BFFF", fg = "#000", image = image)
+            self.image = image
         
         elif "add" in str(self['text']).lower():
             self.config(bg = "#008000", fg = "#fff", image = image)
+            self.image = image
         elif "delete" in str(self['text']).lower():
             self.config(bg = "#600", fg = "#fff", image=image)
+            self.image = image
         elif 'set' in str(self['text']).lower():
             self.config(bg = "#DAA520", fg = "#fff", image=image)
+            self.image = image
         elif 'close' in str(self['text']).lower():
             self.config(image = image, bg = "maroon", fg = "#fff")
+            self.image = image
         elif 'display' in str(self['text']).lower() or 'show' in str(self['text']).lower(): 
             self.config(bg = "#008080", fg = "#fff", image=image)
+            self.image = image
 
         elif "cancel" in str(self['text']).lower():
             self.config(image = image, bg = "gray50")
+            self.image = image
         
         elif "attach" in str(self["text"]).lower() or "browse" in str(self["text"]).lower():
             self.config(image = image, bg = "#b04", fg = "#fff")
+            self.image = image
         
         elif "send" in str(self['text']).lower():
             self.config(image = image, bg = "#FF6E00", fg = "#fff")
+            self.image = image
         
         elif "print" in str(self['text']).lower():
             self.config(bg = "#FEE3B8", image = image)
+            self.image = image
         
         elif "plan" in str(self['text']).lower():
             self.config(bg = "#600", fg = "#fff", image = image)
+            self.image = image
 
         if " all" in str(self['text']).lower():
             self.config(image = image)
+            self.image = image
         
         if " id" in str(self['text']).lower():
             self.config(image = image)
+            self.image = image
 
 class Display:
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
     
     def image(self, img:str):
         try:
```

### Comparing `irene_pro-0.0.31/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.32/irene_pro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.31
+Version: 0.0.32
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.31/setup.py` & `irene_pro-0.0.32/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3331 270d 0a44 4553 4352   '0.0.31'..DESCR
+00000100: 2027 302e 302e 3332 270d 0a44 4553 4352   '0.0.32'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

