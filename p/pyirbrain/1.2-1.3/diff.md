# Comparing `tmp/pyirbrain-1.2.tar.gz` & `tmp/pyirbrain-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyirbrain-1.2.tar", last modified: Mon May 15 11:11:58 2023, max compression
+gzip compressed data, was "pyirbrain-1.3.tar", last modified: Mon May 15 11:34:13 2023, max compression
```

## Comparing `pyirbrain-1.2.tar` & `pyirbrain-1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:11:57.960000 pyirbrain-1.2/
--rw-rw-rw-   0        0        0      239 2023-05-15 11:12:00.000000 pyirbrain-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      147 2022-12-08 11:00:02.000000 pyirbrain-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 11:11:57.970000 pyirbrain-1.2/pyirbrain/
--rw-rw-rw-   0        0        0        0 2021-04-07 00:56:32.000000 pyirbrain-1.2/pyirbrain/__init__.py
--rw-rw-rw-   0        0        0      737 2022-12-08 10:44:08.000000 pyirbrain-1.2/pyirbrain/deflib.py
--rw-rw-rw-   0        0        0     2882 2023-05-15 10:30:18.000000 pyirbrain-1.2/pyirbrain/ikeyevent.py
--rw-rw-rw-   0        0        0      819 2023-05-03 13:37:30.000000 pyirbrain-1.2/pyirbrain/packet.py
--rw-rw-rw-   0        0        0     1367 2022-12-08 10:56:30.000000 pyirbrain-1.2/pyirbrain/parse.py
--rw-rw-rw-   0        0        0     4568 2022-12-08 10:56:34.000000 pyirbrain-1.2/pyirbrain/zeroDrone.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/
--rw-rw-rw-   0        0        0      239 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 11:11:58.000000 pyirbrain-1.2/pyirbrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-15 11:12:00.000000 pyirbrain-1.2/setup.cfg
--rw-rw-rw-   0        0        0      395 2023-05-15 10:42:54.000000 pyirbrain-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:34:13.840000 pyirbrain-1.3/
+-rw-rw-rw-   0        0        0      239 2023-05-15 11:34:14.000000 pyirbrain-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2022-12-08 11:00:02.000000 pyirbrain-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 11:34:13.850000 pyirbrain-1.3/pyirbrain/
+-rw-rw-rw-   0        0        0        0 2021-04-07 00:56:32.000000 pyirbrain-1.3/pyirbrain/__init__.py
+-rw-rw-rw-   0        0        0      737 2022-12-08 10:44:08.000000 pyirbrain-1.3/pyirbrain/deflib.py
+-rw-rw-rw-   0        0        0     2866 2023-05-15 11:30:56.000000 pyirbrain-1.3/pyirbrain/ikeyevent.py
+-rw-rw-rw-   0        0        0      819 2023-05-03 13:37:30.000000 pyirbrain-1.3/pyirbrain/packet.py
+-rw-rw-rw-   0        0        0     1367 2022-12-08 10:56:30.000000 pyirbrain-1.3/pyirbrain/parse.py
+-rw-rw-rw-   0        0        0     4568 2022-12-08 10:56:34.000000 pyirbrain-1.3/pyirbrain/zeroDrone.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:34:13.860000 pyirbrain-1.3/pyirbrain.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-05-15 11:34:14.000000 pyirbrain-1.3/pyirbrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-05-15 11:34:14.000000 pyirbrain-1.3/pyirbrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:34:14.000000 pyirbrain-1.3/pyirbrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-15 11:34:14.000000 pyirbrain-1.3/pyirbrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 11:34:14.000000 pyirbrain-1.3/pyirbrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-15 11:34:14.000000 pyirbrain-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      395 2023-05-15 11:33:20.000000 pyirbrain-1.3/setup.py
```

### Comparing `pyirbrain-1.2/pyirbrain/deflib.py` & `pyirbrain-1.3/pyirbrain/deflib.py`

 * *Files identical despite different names*

### Comparing `pyirbrain-1.2/pyirbrain/ikeyevent.py` & `pyirbrain-1.3/pyirbrain/ikeyevent.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,21 +79,21 @@
 
     def isKeyLeftPressed(self):
         return self.keyLeft
 
     def isKeyRightPressed(self):
         return self.keyRight
     
-    def isKeyRightPressed(self):
+    def isKeyWPressed(self):
         return self.keyGoUp
     
-    def isKeyRightPressed(self):
+    def isKeyXPressed(self):
         return self.keyGoDown
     
-    def isKeyRightPressed(self):
+    def isKeyAPressed(self):
         return self.keyLTurn
     
-    def isKeyRightPressed(self):
+    def isKeyDPressed(self):
         return self.keyRTurn
 
     def isKeyEscPressed(self):
         return self.keyEsc
```

### Comparing `pyirbrain-1.2/pyirbrain/packet.py` & `pyirbrain-1.3/pyirbrain/packet.py`

 * *Files identical despite different names*

### Comparing `pyirbrain-1.2/pyirbrain/parse.py` & `pyirbrain-1.3/pyirbrain/parse.py`

 * *Files identical despite different names*

### Comparing `pyirbrain-1.2/pyirbrain/zeroDrone.py` & `pyirbrain-1.3/pyirbrain/zeroDrone.py`

 * *Files identical despite different names*

