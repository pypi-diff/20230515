# Comparing `tmp/glaceon-1.1.0.tar.gz` & `tmp/glaceon-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glaceon-1.1.0.tar", last modified: Sun May 14 11:45:20 2023, max compression
+gzip compressed data, was "glaceon-1.2.0.tar", last modified: Sun May 14 11:53:19 2023, max compression
```

## Comparing `glaceon-1.1.0.tar` & `glaceon-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 11:45:20.957569 glaceon-1.1.0/
--rw-rw-rw-   0        0        0      230 2023-05-14 11:45:20.957569 glaceon-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 11:45:20.953579 glaceon-1.1.0/glaceon/
--rw-rw-rw-   0        0        0     2524 2023-05-14 11:38:55.000000 glaceon-1.1.0/glaceon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:45:20.956571 glaceon-1.1.0/glaceon.egg-info/
--rw-rw-rw-   0        0        0      230 2023-05-14 11:45:20.000000 glaceon-1.1.0/glaceon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-14 11:45:20.000000 glaceon-1.1.0/glaceon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 11:45:20.000000 glaceon-1.1.0/glaceon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 11:45:20.000000 glaceon-1.1.0/glaceon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 11:45:20.957569 glaceon-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      223 2023-05-14 11:44:51.000000 glaceon-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:53:19.359317 glaceon-1.2.0/
+-rw-rw-rw-   0        0        0      230 2023-05-14 11:53:19.358317 glaceon-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 11:53:19.341364 glaceon-1.2.0/glaceon/
+-rw-rw-rw-   0        0        0     2194 2023-05-14 11:52:50.000000 glaceon-1.2.0/glaceon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:53:19.357353 glaceon-1.2.0/glaceon.egg-info/
+-rw-rw-rw-   0        0        0      230 2023-05-14 11:53:19.000000 glaceon-1.2.0/glaceon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-14 11:53:19.000000 glaceon-1.2.0/glaceon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 11:53:19.000000 glaceon-1.2.0/glaceon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-14 11:53:19.000000 glaceon-1.2.0/glaceon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 11:53:19.359317 glaceon-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      223 2023-05-14 11:52:59.000000 glaceon-1.2.0/setup.py
```

### Comparing `glaceon-1.1.0/glaceon/__init__.py` & `glaceon-1.2.0/glaceon/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 import time
 
 
-class glaceon:
+class cli:
     def __init__(self, speed=1, debug=False):
         self.speed = speed
         self.last_timestamp = time.time()
         self.debug = debug
         self.initialized = True
 
     def getTimestamp(self):
@@ -57,22 +57,7 @@
 
         # delay the output based on the specified speed
         time.sleep(max(1 / self.speed - time_elapsed, 0))
 
         # print the timestamp, tag, and message
         timestamp = self.getTimestamp()
         print(f"{timestamp} [{tag_text}] {message_text}")
-
-
-
-
-
-
-
-
-glaceon = glaceon(debug=True)
-
-# use the print method to output logs with different tags
-glaceon.print("SUCCESS", "This is an informational message")
-glaceon.print("WARNING", "This is a warning message")
-glaceon.print("ERROR", "This is an error message")
-glaceon.print("DEBUG", "This is a debug message")
```

