# Comparing `tmp/pyirbrain-1.1.tar.gz` & `tmp/pyirbrain-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyirbrain-1.1.tar", last modified: Wed May  3 14:34:15 2023, max compression
+gzip compressed data, was "pyirbrain-1.2.tar", last modified: Mon May 15 11:11:58 2023, max compression
```

## Comparing `pyirbrain-1.1.tar` & `pyirbrain-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 14:34:15.700000 pyirbrain-1.1/
--rw-rw-rw-   0        0        0      180 2023-05-03 14:34:16.000000 pyirbrain-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      147 2022-12-08 11:00:02.000000 pyirbrain-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 14:34:15.710000 pyirbrain-1.1/pyirbrain/
--rw-rw-rw-   0        0        0        0 2021-04-07 00:56:32.000000 pyirbrain-1.1/pyirbrain/__init__.py
--rw-rw-rw-   0        0        0      737 2022-12-08 10:44:08.000000 pyirbrain-1.1/pyirbrain/deflib.py
--rw-rw-rw-   0        0        0     1858 2022-12-08 10:44:40.000000 pyirbrain-1.1/pyirbrain/ikeyevent.py
--rw-rw-rw-   0        0        0      819 2023-05-03 13:37:30.000000 pyirbrain-1.1/pyirbrain/packet.py
--rw-rw-rw-   0        0        0     1367 2022-12-08 10:56:30.000000 pyirbrain-1.1/pyirbrain/parse.py
--rw-rw-rw-   0        0        0     4568 2022-12-08 10:56:34.000000 pyirbrain-1.1/pyirbrain/zeroDrone.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:34:15.730000 pyirbrain-1.1/pyirbrain.egg-info/
--rw-rw-rw-   0        0        0      180 2023-05-03 14:34:16.000000 pyirbrain-1.1/pyirbrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-05-03 14:34:16.000000 pyirbrain-1.1/pyirbrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:34:16.000000 pyirbrain-1.1/pyirbrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-03 14:34:16.000000 pyirbrain-1.1/pyirbrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 14:34:16.000000 pyirbrain-1.1/pyirbrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-03 14:34:16.000000 pyirbrain-1.1/setup.cfg
--rw-rw-rw-   0        0        0      395 2023-05-03 14:28:14.000000 pyirbrain-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:11:57.960000 pyirbrain-1.2/
+-rw-rw-rw-   0        0        0      239 2023-05-15 11:12:00.000000 pyirbrain-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2022-12-08 11:00:02.000000 pyirbrain-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 11:11:57.970000 pyirbrain-1.2/pyirbrain/
+-rw-rw-rw-   0        0        0        0 2021-04-07 00:56:32.000000 pyirbrain-1.2/pyirbrain/__init__.py
+-rw-rw-rw-   0        0        0      737 2022-12-08 10:44:08.000000 pyirbrain-1.2/pyirbrain/deflib.py
+-rw-rw-rw-   0        0        0     2882 2023-05-15 10:30:18.000000 pyirbrain-1.2/pyirbrain/ikeyevent.py
+-rw-rw-rw-   0        0        0      819 2023-05-03 13:37:30.000000 pyirbrain-1.2/pyirbrain/packet.py
+-rw-rw-rw-   0        0        0     1367 2022-12-08 10:56:30.000000 pyirbrain-1.2/pyirbrain/parse.py
+-rw-rw-rw-   0        0        0     4568 2022-12-08 10:56:34.000000 pyirbrain-1.2/pyirbrain/zeroDrone.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-15 11:12:00.000000 pyirbrain-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      395 2023-05-15 10:42:54.000000 pyirbrain-1.2/setup.py
```

### Comparing `pyirbrain-1.1/pyirbrain/deflib.py` & `pyirbrain-1.2/pyirbrain/deflib.py`

 * *Files identical despite different names*

### Comparing `pyirbrain-1.1/pyirbrain/ikeyevent.py` & `pyirbrain-1.2/pyirbrain/ikeyevent.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,23 @@
         if key == keyboard.Key.up:
             self.keyUp = True
         if key == keyboard.Key.down:
             self.keyDown = True
         if key == keyboard.Key.right:
             self.keyRight = True
         if key == keyboard.Key.left:
-           self.keyLeft = True
+            self.keyLeft = True
+        if key == keyboard.KeyCode(char="w"):
+            self.keyGoUp = True
+        if key == keyboard.KeyCode(char="x"):
+            self.keyGoDown = True
+        if key == keyboard.KeyCode(char="a"):
+            self.keyLTurn = True
+        if key == keyboard.KeyCode(char="d"):
+            self.keyRTurn = True
         if key == keyboard.Key.esc:
            self.keyEsc = True
 
     def on_release(self, key):
         if key == keyboard.Key.enter:
             self.keyEnter = False
         if key == keyboard.Key.space:
@@ -26,24 +34,36 @@
             self.keyUp = False
         if key == keyboard.Key.down:
             self.keyDown = False
         if key == keyboard.Key.right:
             self.keyRight = False
         if key == keyboard.Key.left:
             self.keyLeft = False
+        if key == keyboard.KeyCode(char="w"):
+            self.keyGoUp = False
+        if key == keyboard.KeyCode(char="x"):
+            self.keyGoDown = False
+        if key == keyboard.KeyCode(char="a"):
+            self.keyLTurn = False
+        if key == keyboard.KeyCode(char="d"):
+            self.keyRTurn = False
         if key == keyboard.Key.esc:
            self.keyEsc = False
 
     def __init__(self):
         self.keyEnter = False
         self.keySpace = False   
         self.keyUp = False
         self.keyDown = False
         self.keyLeft = False
         self.keyRight = False
+        self.keyGoUp = False
+        self.keyGoDown = False
+        self.keyLTurn= False
+        self.keyRTurn = False
         self.keyEsc = False
 
         listener = keyboard.Listener(on_press=self.on_press, on_release=self.on_release)
         listener.start()
 
     def isKeyEnterPressed(self):
         return self.keyEnter
@@ -58,10 +78,22 @@
         return self.keyDown
 
     def isKeyLeftPressed(self):
         return self.keyLeft
 
     def isKeyRightPressed(self):
         return self.keyRight
+    
+    def isKeyRightPressed(self):
+        return self.keyGoUp
+    
+    def isKeyRightPressed(self):
+        return self.keyGoDown
+    
+    def isKeyRightPressed(self):
+        return self.keyLTurn
+    
+    def isKeyRightPressed(self):
+        return self.keyRTurn
 
     def isKeyEscPressed(self):
         return self.keyEsc
```

### Comparing `pyirbrain-1.1/pyirbrain/packet.py` & `pyirbrain-1.2/pyirbrain/packet.py`

 * *Files identical despite different names*

### Comparing `pyirbrain-1.1/pyirbrain/parse.py` & `pyirbrain-1.2/pyirbrain/parse.py`

 * *Files identical despite different names*

### Comparing `pyirbrain-1.1/pyirbrain/zeroDrone.py` & `pyirbrain-1.2/pyirbrain/zeroDrone.py`

 * *Files identical despite different names*

