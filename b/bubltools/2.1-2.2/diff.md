# Comparing `tmp/bubltools-2.1.tar.gz` & `tmp/bubltools-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bubltools-2.1.tar", last modified: Thu Mar  9 17:21:47 2023, max compression
+gzip compressed data, was "bubltools-2.2.tar", last modified: Mon May 15 19:40:44 2023, max compression
```

## Comparing `bubltools-2.1.tar` & `bubltools-2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-09 17:21:47.861271 bubltools-2.1/
--rw-r--r--   0 runner    (1000) runner    (1000)      885 2023-03-09 17:21:47.857271 bubltools-2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-09 17:21:47.857271 bubltools-2.1/bubltools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      885 2023-03-09 17:21:47.000000 bubltools-2.1/bubltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      131 2023-03-09 17:21:47.000000 bubltools-2.1/bubltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-03-09 17:21:47.000000 bubltools-2.1/bubltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-03-09 17:21:47.000000 bubltools-2.1/bubltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-03-09 17:21:47.861271 bubltools-2.1/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-15 19:40:44.882195 bubltools-2.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      897 2023-05-15 19:40:44.882195 bubltools-2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-15 19:40:44.878195 bubltools-2.2/bubltools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      897 2023-05-15 19:40:44.000000 bubltools-2.2/bubltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      131 2023-05-15 19:40:44.000000 bubltools-2.2/bubltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-15 19:40:44.000000 bubltools-2.2/bubltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-15 19:40:44.000000 bubltools-2.2/bubltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-15 19:40:44.882195 bubltools-2.2/setup.cfg
```

### Comparing `bubltools-2.1/PKG-INFO` & `bubltools-2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bubltools
-Version: 2.1
+Version: 2.2
 Summary: Some tools I coded
 Home-page: https://github.com/BubblePlayzTHEREAL/BubbleTools
 Author: BubblePlayz#3098
 Author-email: bubblelind@gmail.com
 License: UNKNOWN
 Description: # About
         ---
         
-        Here are some little tools I have come up with. I dont have much right now but you could add an "issue" on the github and suggest a tool or inclusion I could try to add.
+        Here are some little tools I have come up with. I dont have much right now but you could add an "issue" on the github or email me and suggest a tool or inclusion I could try to add.
         # Tools
         ## linebreak
         Creates an empty line in the console/terminal
         ### Usage
         `bubltools.linebreak(lines)`
         
         lines is the amount of lines to get rid of (default is 1)
```

### Comparing `bubltools-2.1/bubltools.egg-info/PKG-INFO` & `bubltools-2.2/bubltools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bubltools
-Version: 2.1
+Version: 2.2
 Summary: Some tools I coded
 Home-page: https://github.com/BubblePlayzTHEREAL/BubbleTools
 Author: BubblePlayz#3098
 Author-email: bubblelind@gmail.com
 License: UNKNOWN
 Description: # About
         ---
         
-        Here are some little tools I have come up with. I dont have much right now but you could add an "issue" on the github and suggest a tool or inclusion I could try to add.
+        Here are some little tools I have come up with. I dont have much right now but you could add an "issue" on the github or email me and suggest a tool or inclusion I could try to add.
         # Tools
         ## linebreak
         Creates an empty line in the console/terminal
         ### Usage
         `bubltools.linebreak(lines)`
         
         lines is the amount of lines to get rid of (default is 1)
```

