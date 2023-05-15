# Comparing `tmp/screens.py-0.4.5.tar.gz` & `tmp/screens_py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screens.py-0.4.5.tar", last modified: Sun Dec 18 10:02:27 2022, max compression
+gzip compressed data, was "screens_py-0.5.0.tar", max compression
```

## Comparing `screens.py-0.4.5.tar` & `screens_py-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,9 @@
-drwxrwxrwx   0        0        0        0 2022-12-18 10:02:27.615176 screens.py-0.4.5/
--rw-rw-rw-   0        0        0    35807 2022-12-17 21:47:37.000000 screens.py-0.4.5/LICENSE
--rw-rw-rw-   0        0        0     1189 2022-12-18 10:02:27.614177 screens.py-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      807 2022-12-17 21:47:37.000000 screens.py-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2022-12-18 10:02:27.610178 screens.py-0.4.5/screens/
--rw-rw-rw-   0        0        0       48 2022-12-17 21:47:37.000000 screens.py-0.4.5/screens/__init__.py
--rw-rw-rw-   0        0        0      780 2022-12-18 09:58:19.000000 screens.py-0.4.5/screens/command.py
--rw-rw-rw-   0        0        0     1941 2022-12-18 09:57:57.000000 screens.py-0.4.5/screens/session.py
-drwxrwxrwx   0        0        0        0 2022-12-18 10:02:27.613176 screens.py-0.4.5/screens.py.egg-info/
--rw-rw-rw-   0        0        0     1189 2022-12-18 10:02:27.000000 screens.py-0.4.5/screens.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2022-12-18 10:02:27.000000 screens.py-0.4.5/screens.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-18 10:02:27.000000 screens.py-0.4.5/screens.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-12-18 10:02:27.000000 screens.py-0.4.5/screens.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-18 10:02:27.615176 screens.py-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      453 2022-12-18 09:58:34.000000 screens.py-0.4.5/setup.py
+-rw-r--r--   0        0        0    35807 2022-12-17 21:47:37.637448 screens_py-0.5.0/LICENSE
+-rw-r--r--   0        0        0      459 2023-05-15 19:56:22.323680 screens_py-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      801 2023-05-15 19:42:51.915676 screens_py-0.5.0/README.md
+-rw-r--r--   0        0        0      141 2023-05-15 19:52:14.870956 screens_py-0.5.0/screens/__init__.py
+-rw-r--r--   0        0        0      728 2023-05-15 19:09:00.708938 screens_py-0.5.0/screens/exceptions.py
+-rw-r--r--   0        0        0      487 2023-05-15 19:53:05.714235 screens_py-0.5.0/screens/req.py
+-rw-r--r--   0        0        0     1966 2023-05-15 19:54:06.554838 screens_py-0.5.0/screens/screens.py
+-rw-r--r--   0        0        0      101 2023-01-11 01:50:00.949549 screens_py-0.5.0/screens/units.py
+-rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 screens_py-0.5.0/PKG-INFO
```

### Comparing `screens.py-0.4.5/LICENSE` & `screens_py-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screens.py-0.4.5/PKG-INFO` & `screens_py-0.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,24 @@
-Metadata-Version: 2.1
-Name: screens.py
-Version: 0.4.5
-Summary: A light-weight library for easy interaction between Python and GNU screen.
-Home-page: https://github.com/romanin-rf/pyscreen
-Author: Romanin
-Author-email: semina054@gmail.com
-License: UNKNOWN
-Keywords: GNU screen,screens
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # screen.py
 ## Description
 A light-weight library for easy interaction between Python and GNU screen.
 
 This library allows you create, find and kill screen sessions programmatically from Python, as well as send (string) commands to these sessions. You can use this to start other software inside a screen session from a Python script, like this:
 ```python
 import screens
 
 # Start a new session and give it something to do    
-session = screens.ScreenSession('myName')
+session = screens.Session('myName')
 session.send_command('echo hello')
 
 # Kill a screen session with a particular name
 session = screens.get_session_with_name('testSession')
 session.kill()
 
 # Print all the id of all sessions
 for session in screens.get_all_sessions():
     print(session.id)
 ```
 ## Installation
 ```
 pip install --upgrade screens.py
 ```
-
-
```

