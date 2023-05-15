# Comparing `tmp/kien-0.7.0.tar.gz` & `tmp/kien-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kien-0.7.0.tar", last modified: Tue Aug  7 14:10:04 2018, max compression
+gzip compressed data, was "dist/kien-0.9.1.tar", last modified: Mon Aug 13 12:36:17 2018, max compression
```

## Comparing `kien-0.7.0.tar` & `kien-0.9.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-07 14:10:04.000000 kien-0.7.0/
--rw-r--r--   0 konrad    (1000) konrad    (1000)      151 2018-08-07 14:08:20.000000 kien-0.7.0/.bumpversion.cfg
--rw-r--r--   0 konrad    (1000) konrad    (1000)      188 2018-04-27 16:45:52.000000 kien-0.7.0/.gitignore
--rw-r--r--   0 konrad    (1000) konrad    (1000)     1313 2018-06-18 08:58:28.000000 kien-0.7.0/CHANGELOG.md
--rw-r--r--   0 konrad    (1000) konrad    (1000)    35149 2017-09-30 07:16:26.000000 kien-0.7.0/LICENSE
--rw-r--r--   0 konrad    (1000) konrad    (1000)      386 2018-06-20 11:58:04.000000 kien-0.7.0/Makefile
--rw-r--r--   0 konrad    (1000) konrad    (1000)     3158 2018-08-07 14:10:04.000000 kien-0.7.0/PKG-INFO
--rw-r--r--   0 konrad    (1000) konrad    (1000)      188 2018-04-27 16:56:18.000000 kien-0.7.0/Pipfile
--rw-r--r--   0 konrad    (1000) konrad    (1000)     1047 2018-04-27 16:56:21.000000 kien-0.7.0/Pipfile.lock
--rw-r--r--   0 konrad    (1000) konrad    (1000)     2102 2018-06-17 17:09:44.000000 kien-0.7.0/README.md
--rw-r--r--   0 konrad    (1000) konrad    (1000)        6 2018-08-07 14:08:20.000000 kien-0.7.0/VERSION
-drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-07 14:10:04.000000 kien-0.7.0/debian/
--rw-r--r--   0 konrad    (1000) konrad    (1000)     1233 2018-08-07 14:08:20.000000 kien-0.7.0/debian/changelog
--rw-r--r--   0 konrad    (1000) konrad    (1000)        2 2018-04-24 14:30:41.000000 kien-0.7.0/debian/compat
--rw-r--r--   0 konrad    (1000) konrad    (1000)      407 2018-04-24 14:30:41.000000 kien-0.7.0/debian/control
--rw-r--r--   0 konrad    (1000) konrad    (1000)      166 2018-04-24 14:30:41.000000 kien-0.7.0/debian/copyright
--rwxr-xr-x   0 konrad    (1000) konrad    (1000)       94 2018-04-24 14:30:41.000000 kien-0.7.0/debian/rules
-drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-07 14:10:04.000000 kien-0.7.0/debian/source/
--rw-r--r--   0 konrad    (1000) konrad    (1000)       10 2018-04-24 14:30:41.000000 kien-0.7.0/debian/source/format
-drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-07 14:10:04.000000 kien-0.7.0/docs/
--rw-r--r--   0 konrad    (1000) konrad    (1000)     4177 2018-04-24 14:43:52.000000 kien-0.7.0/docs/logo.png
--rw-r--r--   0 konrad    (1000) konrad    (1000)    65604 2018-04-27 13:48:02.000000 kien-0.7.0/docs/say-some-name-example.png
-drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-07 14:10:04.000000 kien-0.7.0/examples/
--rwxr-xr-x   0 konrad    (1000) konrad    (1000)       84 2018-04-27 13:38:58.000000 kien-0.7.0/examples/.executor.sh
--rwxr-xr-x   0 konrad    (1000) konrad    (1000)      727 2018-04-27 13:35:43.000000 kien-0.7.0/examples/say-my-name.py
--rwxr-xr-x   0 konrad    (1000) konrad    (1000)     1481 2018-04-27 13:40:57.000000 kien-0.7.0/examples/say-some-name.py
-drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-07 14:10:04.000000 kien-0.7.0/kien/
--rw-r--r--   0 konrad    (1000) konrad    (1000)      266 2018-06-17 17:05:43.000000 kien-0.7.0/kien/__init__.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)       22 2018-08-07 14:08:20.000000 kien-0.7.0/kien/__version__.py
-drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-07 14:10:04.000000 kien-0.7.0/kien/command/
--rw-r--r--   0 konrad    (1000) konrad    (1000)        0 2018-04-12 12:53:20.000000 kien-0.7.0/kien/command/__init__.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)     5042 2018-06-17 17:05:43.000000 kien-0.7.0/kien/command/help.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)      292 2018-04-12 12:53:20.000000 kien-0.7.0/kien/command/quit.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)     1004 2018-08-07 12:43:57.000000 kien-0.7.0/kien/command/set.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)    22911 2018-08-06 14:45:53.000000 kien-0.7.0/kien/commands.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)     4879 2018-08-01 00:46:13.000000 kien-0.7.0/kien/console.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)      663 2018-06-18 08:15:27.000000 kien-0.7.0/kien/error.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)      406 2018-06-17 17:05:50.000000 kien-0.7.0/kien/events.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)     5105 2018-08-01 00:46:13.000000 kien-0.7.0/kien/runner.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)     4341 2018-08-06 14:45:53.000000 kien-0.7.0/kien/transformation.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)     9624 2018-08-06 14:45:53.000000 kien-0.7.0/kien/utils.py
--rw-r--r--   0 konrad    (1000) konrad    (1000)     5584 2018-08-06 14:45:59.000000 kien-0.7.0/kien/validation.py
-drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-07 14:10:04.000000 kien-0.7.0/kien.egg-info/
--rw-r--r--   0 konrad    (1000) konrad    (1000)     3158 2018-08-07 14:10:04.000000 kien-0.7.0/kien.egg-info/PKG-INFO
--rw-r--r--   0 konrad    (1000) konrad    (1000)      780 2018-08-07 14:10:04.000000 kien-0.7.0/kien.egg-info/SOURCES.txt
--rw-r--r--   0 konrad    (1000) konrad    (1000)        1 2018-08-07 14:10:04.000000 kien-0.7.0/kien.egg-info/dependency_links.txt
--rw-r--r--   0 konrad    (1000) konrad    (1000)       18 2018-08-07 14:10:04.000000 kien-0.7.0/kien.egg-info/requires.txt
--rw-r--r--   0 konrad    (1000) konrad    (1000)        5 2018-08-07 14:10:04.000000 kien-0.7.0/kien.egg-info/top_level.txt
-drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-07 14:10:04.000000 kien-0.7.0/make.d/
--rw-r--r--   0 konrad    (1000) konrad    (1000)     1392 2018-05-29 09:48:24.000000 kien-0.7.0/make.d/makefilet-download-ondemand.mk
--rw-r--r--   0 konrad    (1000) konrad    (1000)       18 2018-04-27 16:56:33.000000 kien-0.7.0/requirements.txt
--rw-r--r--   0 konrad    (1000) konrad    (1000)      109 2018-08-07 14:10:04.000000 kien-0.7.0/setup.cfg
--rw-r--r--   0 konrad    (1000) konrad    (1000)     1112 2018-06-18 08:37:54.000000 kien-0.7.0/setup.py
+drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-13 12:36:17.000000 kien-0.9.1/
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      151 2018-08-13 12:25:36.000000 kien-0.9.1/.bumpversion.cfg
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      188 2018-04-27 16:45:52.000000 kien-0.9.1/.gitignore
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     3001 2018-08-13 12:24:57.000000 kien-0.9.1/CHANGELOG.md
+-rw-r--r--   0 konrad    (1000) konrad    (1000)    35149 2017-09-30 07:16:26.000000 kien-0.9.1/LICENSE
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      386 2018-06-20 11:58:04.000000 kien-0.9.1/Makefile
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     3182 2018-08-13 12:36:17.000000 kien-0.9.1/PKG-INFO
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      188 2018-04-27 16:56:18.000000 kien-0.9.1/Pipfile
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     1047 2018-04-27 16:56:21.000000 kien-0.9.1/Pipfile.lock
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     2118 2018-08-13 10:50:34.000000 kien-0.9.1/README.md
+-rw-r--r--   0 konrad    (1000) konrad    (1000)        6 2018-08-13 12:25:36.000000 kien-0.9.1/VERSION
+drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-13 12:36:17.000000 kien-0.9.1/debian/
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     1695 2018-08-13 12:25:36.000000 kien-0.9.1/debian/changelog
+-rw-r--r--   0 konrad    (1000) konrad    (1000)        2 2018-04-24 14:30:41.000000 kien-0.9.1/debian/compat
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      407 2018-04-24 14:30:41.000000 kien-0.9.1/debian/control
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      166 2018-04-24 14:30:41.000000 kien-0.9.1/debian/copyright
+-rwxr-xr-x   0 konrad    (1000) konrad    (1000)       94 2018-04-24 14:30:41.000000 kien-0.9.1/debian/rules
+drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-13 12:36:17.000000 kien-0.9.1/debian/source/
+-rw-r--r--   0 konrad    (1000) konrad    (1000)       10 2018-04-24 14:30:41.000000 kien-0.9.1/debian/source/format
+drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-13 12:36:17.000000 kien-0.9.1/docs/
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     7185 2018-08-13 11:08:41.000000 kien-0.9.1/docs/logo.png
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     9341 2018-08-13 11:08:43.000000 kien-0.9.1/docs/logo.svg
+-rw-r--r--   0 konrad    (1000) konrad    (1000)    65604 2018-04-27 13:48:02.000000 kien-0.9.1/docs/say-some-name-example.png
+drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-13 12:36:17.000000 kien-0.9.1/examples/
+-rwxr-xr-x   0 konrad    (1000) konrad    (1000)       84 2018-04-27 13:38:58.000000 kien-0.9.1/examples/.executor.sh
+-rwxr-xr-x   0 konrad    (1000) konrad    (1000)      727 2018-04-27 13:35:43.000000 kien-0.9.1/examples/say-my-name.py
+-rwxr-xr-x   0 konrad    (1000) konrad    (1000)     1481 2018-04-27 13:40:57.000000 kien-0.9.1/examples/say-some-name.py
+drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-13 12:36:17.000000 kien-0.9.1/kien/
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      275 2018-08-09 16:32:55.000000 kien-0.9.1/kien/__init__.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)       22 2018-08-13 12:25:36.000000 kien-0.9.1/kien/__version__.py
+drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-13 12:36:17.000000 kien-0.9.1/kien/command/
+-rw-r--r--   0 konrad    (1000) konrad    (1000)        0 2018-04-12 12:53:20.000000 kien-0.9.1/kien/command/__init__.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     5042 2018-06-17 17:05:43.000000 kien-0.9.1/kien/command/help.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      292 2018-04-12 12:53:20.000000 kien-0.9.1/kien/command/quit.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     1004 2018-08-07 12:43:57.000000 kien-0.9.1/kien/command/set.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)    23093 2018-08-09 16:30:17.000000 kien-0.9.1/kien/commands.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     6371 2018-08-13 10:19:42.000000 kien-0.9.1/kien/console.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      663 2018-06-18 08:15:27.000000 kien-0.9.1/kien/error.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      406 2018-06-17 17:05:50.000000 kien-0.9.1/kien/events.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     5836 2018-08-13 10:19:42.000000 kien-0.9.1/kien/runner.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     5069 2018-08-09 13:31:24.000000 kien-0.9.1/kien/transformation.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     9624 2018-08-06 14:45:53.000000 kien-0.9.1/kien/utils.py
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     5584 2018-08-06 14:45:59.000000 kien-0.9.1/kien/validation.py
+drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-13 12:36:17.000000 kien-0.9.1/kien.egg-info/
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     3182 2018-08-13 12:36:16.000000 kien-0.9.1/kien.egg-info/PKG-INFO
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      794 2018-08-13 12:36:17.000000 kien-0.9.1/kien.egg-info/SOURCES.txt
+-rw-r--r--   0 konrad    (1000) konrad    (1000)        1 2018-08-13 12:36:16.000000 kien-0.9.1/kien.egg-info/dependency_links.txt
+-rw-r--r--   0 konrad    (1000) konrad    (1000)       18 2018-08-13 12:36:16.000000 kien-0.9.1/kien.egg-info/requires.txt
+-rw-r--r--   0 konrad    (1000) konrad    (1000)        5 2018-08-13 12:36:16.000000 kien-0.9.1/kien.egg-info/top_level.txt
+drwxr-xr-x   0 konrad    (1000) konrad    (1000)        0 2018-08-13 12:36:17.000000 kien-0.9.1/make.d/
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     1392 2018-05-29 09:48:24.000000 kien-0.9.1/make.d/makefilet-download-ondemand.mk
+-rw-r--r--   0 konrad    (1000) konrad    (1000)       18 2018-04-27 16:56:33.000000 kien-0.9.1/requirements.txt
+-rw-r--r--   0 konrad    (1000) konrad    (1000)      109 2018-08-13 12:36:17.000000 kien-0.9.1/setup.cfg
+-rw-r--r--   0 konrad    (1000) konrad    (1000)     1211 2018-08-13 12:22:54.000000 kien-0.9.1/setup.py
```

### Comparing `kien-0.7.0/LICENSE` & `kien-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/PKG-INFO` & `kien-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kien
-Version: 0.7.0
+Version: 0.9.1
 Summary: kien is a line-based command parser for creating shell-like interfaces
 Home-page: https://github.com/silicann/kien
 Author: Konrad Mohrfeldt
 Author-email: mohrfeldt@silicann.com
 License: GPLv3+
 Description: 
         # ![kien logo](./docs/logo.png)
@@ -26,14 +26,15 @@
          * (optional) keywords 
          * variables
          * validation
          * transformation
          * auto-generated help and documentation
          * dependency-injection
          * human-readable and json output
+         * tty handling
          
         ![Prompt example showing how the say-some-name example works in action](./docs/say-some-name-example.png)
         
         ## Examples
         
         kien mostly works by annotating functions with decorators. See the examples folder 😊
```

### Comparing `kien-0.7.0/Pipfile.lock` & `kien-0.9.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/README.md` & `kien-0.9.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
  * (optional) keywords 
  * variables
  * validation
  * transformation
  * auto-generated help and documentation
  * dependency-injection
  * human-readable and json output
+ * tty handling
  
 ![Prompt example showing how the say-some-name example works in action](./docs/say-some-name-example.png)
 
 ## Examples
 
 kien mostly works by annotating functions with decorators. See the examples folder 😊
```

### Comparing `kien-0.7.0/debian/changelog` & `kien-0.9.1/debian/changelog`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+python-kien (0.9.1-1) unstable; urgency=medium
+
+  * New upstream release
+
+ -- Konrad Mohrfeldt <mohrfeldt@silicann.com>  Mon, 13 Aug 2018 14:25:36 +0200
+
+python-kien (0.9.0-1) unstable; urgency=medium
+
+  * New upstream release
+
+ -- Konrad Mohrfeldt <mohrfeldt@silicann.com>  Mon, 13 Aug 2018 13:13:10 +0200
+
+python-kien (0.8.0-1) unstable; urgency=medium
+
+  * New upstream release
+
+ -- Konrad Mohrfeldt <mohrfeldt@silicann.com>  Thu, 09 Aug 2018 18:41:36 +0200
+
 python-kien (0.7.0-1) unstable; urgency=medium
 
   * New upstream release
 
  -- Konrad Mohrfeldt <mohrfeldt@silicann.com>  Tue, 07 Aug 2018 16:08:20 +0200
 
 python-kien (0.6.0-1) unstable; urgency=medium
```

### Comparing `kien-0.7.0/docs/say-some-name-example.png` & `kien-0.9.1/docs/say-some-name-example.png`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/examples/say-my-name.py` & `kien-0.9.1/examples/say-my-name.py`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/examples/say-some-name.py` & `kien-0.9.1/examples/say-some-name.py`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/kien/command/help.py` & `kien-0.9.1/kien/command/help.py`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/kien/command/set.py` & `kien-0.9.1/kien/command/set.py`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/kien/commands.py` & `kien-0.9.1/kien/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,36 +35,38 @@
 
 
 class _Token:
     is_variable = False
     is_placeholder = False
 
     def __init__(self, value=_Undefined, name=None, is_optional=False,
-                 greedy=False, transform=None, choices=None, description=None):
+                 greedy=False, transform=None, choices=None, description=None,
+                 aliases=None):
         """ specify possible value of a command string token
 
         @param choices: may be None, an enum or an iterable
         """
         # TODO: greedy should accept integers
         self.value = value
         self.name = name
         self.is_optional = is_optional
         self.greedy = greedy
         self.transform = transform
         self.description = description
+        self.aliases = frozenset(aliases or [])
         if choices is None:
             self.choices = set()
         elif _is_enum(choices):
             self.choices = {item.value for item in choices}
         else:
             self.choices = set(choices)
 
     def matches(self, value):
         if self.value is not _Undefined:
-            return self.value == value
+            return self.value == value or value in self.aliases
         if self.name and self.transform:
             # we trigger the token validation here to handle args that
             # have been misspelled and to provide command suggestions
             getattr(self.transform, 'validate', noop)(value)
         if self.name and self.choices:
             # if choices were defined we must validate that the provided
             # value actually is one of those choices
@@ -121,14 +123,18 @@
     return _Variable(value, name, is_optional, greedy, transform, choices, description)
 
 
 def optional(value):
     return _Placeholder(value, is_optional=True)
 
 
+def keyword(value, aliases=None):
+    return _Token(value, aliases=aliases)
+
+
 def group(name, description=None):
     return _Group(name, description)
 
 
 def _find_token(tokens, index):
     if len(tokens) > index:
         return tokens[index]
```

### Comparing `kien-0.7.0/kien/console.py` & `kien-0.9.1/kien/console.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import curses
+import fcntl
+import io
 import json
+import os
 # merely importing readline enable command history via "input"
 # noinspection PyUnresolvedReferences
 import readline  # noqa: F401
 import sys
 import termios
 
 import blessings
@@ -117,7 +120,46 @@
                     format_begin=format_begin, text=text, format_end=format_end
                 )
             if self._last_status > 0:
                 prompt = _format(self.terminal.red, prompt)
             else:
                 prompt = _format(self.terminal.blue, prompt)
         return prompt
+
+
+def _become_session_leader():
+    """ replicate the effect of the helper program 'setsid ...' """
+    if os.getpid() == os.getsid(0):
+        # we are already the session leader
+        pass
+    else:
+        # We need to fork in order to be able to create our own session group.
+        if os.fork() != 0:
+            # the parent process may die
+            sys.exit()
+        else:
+            os.setsid()
+
+
+def acquire_controlling_terminal(terminal_dev_path):
+    """ fork the process in order to become session leader and replace stdin/stdout/stderr 
+
+    The result should be comparable with running the program via "setsid -w agetty ...".
+    """
+    _become_session_leader()
+    # TODO: the flags are just copied from agetty's behaviour
+    dev = os.open(terminal_dev_path, os.O_RDWR | os.O_NOCTTY | os.O_NONBLOCK | os.O_LARGEFILE)
+    sys.stdin.close()
+    sys.stdout.close()
+    fcntl.ioctl(dev, termios.TIOCSCTTY, 0)
+    # duplicate the open handle to stdin and stdout
+    os.dup2(dev, 0)
+    os.dup2(dev, 1)
+    # replace the text-based stdin/stdout handles
+    sys.stdin = open(0, "rt", buffering=1)
+    sys.stdout = open(1, "wt", buffering=1)
+    # apply some useful settings for an interactive terminal
+    term_settings = termios.tcgetattr(dev)
+    # output: new line should also include a carriage return
+    term_settings[3] = term_settings[3] | termios.ONLCR
+    termios.tcsetattr(dev, termios.TCSADRAIN, term_settings)
+    os.close(dev)
```

### Comparing `kien-0.7.0/kien/error.py` & `kien-0.9.1/kien/error.py`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/kien/runner.py` & `kien-0.9.1/kien/runner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import argparse
+import functools
 import logging
 import readline
+import signal
 import sys
 from typing import Sequence
-from blinker import signal
-from .console import Console
+
+import blinker
+
+from .console import Console, acquire_controlling_terminal
 from .events import ConsoleExitEvent, StopProcessingEvent
 from .utils import autoload, failsafe
 from .error import CommandError
 
 logger = logging.getLogger('eliza-runner')
 
-on_result = signal('result')
-on_dispatch = signal('dispatch')
-on_error = signal('error')
+on_result = blinker.signal('result')
+on_dispatch = blinker.signal('dispatch')
+on_error = blinker.signal('error')
 
 
 class ConsoleRunner:
     def __init__(self) -> None:
         self.cli_args = None
         self.console = None
         self.commander = None
@@ -30,14 +34,19 @@
         parser = argparse.ArgumentParser()
         parser.add_argument('--disable-style', dest='disable_style', action='store_true',
                             help='Disable terminal styling (colors).')
         parser.add_argument('--autoload', dest='modules', action='append',
                             help='autoload a module for the interpreter')
         parser.add_argument('--history', default=None,
                             help='Read history from and write it to the specified file')
+        parser.add_argument('--tty', dest='tty',
+                            help='Acquire the specified TTY and use it for input and output')
+        parser.add_argument('--reconnect-on-hangup', dest='reconnect_on_hangup',
+                            action='store_true',
+                            help='Reconnect to the tty after receiving a SIGHUP signal.')
         parser.add_argument('--ignore-eof', dest='ignore_eof', action='store_true',
                             help='Ignore the EOF control character (commonly: CTRL-D)')
         parser.add_argument('--failsafe', action='store_true',
                             help='keep the application running no matter what '
                                  'runtime exceptions are thrown')
         parser.add_argument('--failsafe-errors', action='store_true',
                             help='in case failsafe is enabled this option will log any unhandled '
@@ -49,14 +58,19 @@
 
     def parse_args(self, args: Sequence[str] = None) -> argparse.Namespace:
         args = sys.argv[1:] if args is None else args
         return self.get_arg_parser().parse_args(args)
 
     def configure(self) -> None:
         self.cli_args = self.parse_args()
+        if self.cli_args.tty:
+            acquire_tty_func = functools.partial(acquire_controlling_terminal, self.cli_args.tty)
+            if self.cli_args.reconnect_on_hangup:
+                signal.signal(signal.SIGHUP, lambda sig, frame: acquire_tty_func())
+            acquire_tty_func()
 
     def run(self) -> None:
         self.configure()
 
         with Console(sys.stdout, prompt=self.prompt) as console:
             console.configure_auto(force_disable_style=self.cli_args.disable_style)
             if self.commander is None:
```

### Comparing `kien-0.7.0/kien/transformation.py` & `kien-0.9.1/kien/transformation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import collections
 from functools import update_wrapper, wraps
 import itertools
 import re
+from typing import Hashable, Iterable, Mapping
 
 from .validation import validate_value, one_of
 
 TRUE_CHOICES = ('true', '1', 'on', 'yes', 'enable')
 FALSE_CHOICES = ('false', '0', 'off', 'no', 'disable')
 
 
@@ -120,15 +121,30 @@
     for group, index in match.re.groupindex.items():
         kwargs[group] = match[index]
 
     return convert_to(*args, **kwargs)
 
 
 @simple_transformator
-def to_enum(enum, value):
+def to_enum(enum, value, static_map: Mapping[Hashable, Iterable[str]] = None):
+    """
+    Converts a literal value to a value from an enum.
+
+    :param enum: the enum the value should be converted to
+    :param value: a value that should be mapped to the provided enum
+    :param static_map: a static mapping for aliases that should be respected while
+                       converting to the enum. Expects an enum value mapped to a
+                       an Iterable of str.
+    :return: returns the enum value or None
+    """
+    if static_map is not None:
+        for enum_value, mappings in static_map.items():
+            if value in mappings:
+                value = enum_value
+                break
     if value is None:
         return None
     for item in tuple(enum):
         if value == item or value == item.value:
             return item
```

### Comparing `kien-0.7.0/kien/utils.py` & `kien-0.9.1/kien/utils.py`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/kien/validation.py` & `kien-0.9.1/kien/validation.py`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/kien.egg-info/PKG-INFO` & `kien-0.9.1/kien.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kien
-Version: 0.7.0
+Version: 0.9.1
 Summary: kien is a line-based command parser for creating shell-like interfaces
 Home-page: https://github.com/silicann/kien
 Author: Konrad Mohrfeldt
 Author-email: mohrfeldt@silicann.com
 License: GPLv3+
 Description: 
         # ![kien logo](./docs/logo.png)
@@ -26,14 +26,15 @@
          * (optional) keywords 
          * variables
          * validation
          * transformation
          * auto-generated help and documentation
          * dependency-injection
          * human-readable and json output
+         * tty handling
          
         ![Prompt example showing how the say-some-name example works in action](./docs/say-some-name-example.png)
         
         ## Examples
         
         kien mostly works by annotating functions with decorators. See the examples folder 😊
```

### Comparing `kien-0.7.0/kien.egg-info/SOURCES.txt` & `kien-0.9.1/kien.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 debian/changelog
 debian/compat
 debian/control
 debian/copyright
 debian/rules
 debian/source/format
 docs/logo.png
+docs/logo.svg
 docs/say-some-name-example.png
 examples/.executor.sh
 examples/say-my-name.py
 examples/say-some-name.py
 kien/__init__.py
 kien/__version__.py
 kien/commands.py
```

### Comparing `kien-0.7.0/make.d/makefilet-download-ondemand.mk` & `kien-0.9.1/make.d/makefilet-download-ondemand.mk`

 * *Files identical despite different names*

### Comparing `kien-0.7.0/setup.py` & `kien-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     packages=find_packages(exclude=('examples', )),
     install_requires=[
         'blessings',
         'blinker'
     ],
     extras_require={},
     include_package_data=True,
+    package_data={
+        '': ['requirements.txt', 'README.md', 'LICENSE', 'CHANGELOG.md']
+    },
     license='GPLv3+',
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ]
```

