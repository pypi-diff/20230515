# Comparing `tmp/ox_ui-0.3.4.tar.gz` & `tmp/ox_ui-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_ui-0.3.4.tar", last modified: Mon May 15 18:13:17 2023, max compression
+gzip compressed data, was "ox_ui-0.3.5.tar", last modified: Mon May 15 19:12:33 2023, max compression
```

## Comparing `ox_ui-0.3.4.tar` & `ox_ui-0.3.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/
--rw-------   0 emin      (1000) emin      (1000)     1129 2019-07-23 18:08:30.000000 ox_ui-0.3.4/.gitignore
--rw-------   0 emin      (1000) emin      (1000)     1325 2019-07-23 18:03:49.000000 ox_ui-0.3.4/LICENSE.txt
--rw-------   0 emin      (1000) emin      (1000)       56 2019-07-24 15:29:34.000000 ox_ui-0.3.4/MANIFEST.in
--rw-rw-r--   0 emin      (1000) emin      (1000)      535 2023-05-15 18:13:17.113673 ox_ui-0.3.4/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)       82 2019-07-23 18:08:09.000000 ox_ui-0.3.4/README.org
--rw-rw-r--   0 emin      (1000) emin      (1000)       93 2022-04-19 15:06:12.000000 ox_ui-0.3.4/README.rst
--rw-------   0 emin      (1000) emin      (1000)       73 2019-07-23 18:03:49.000000 ox_ui-0.3.4/conftest.py
--rw-------   0 emin      (1000) emin      (1000)      459 2019-07-23 18:04:11.000000 ox_ui-0.3.4/makefile
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/
--rw-rw-r--   0 emin      (1000) emin      (1000)       67 2023-05-15 17:41:26.000000 ox_ui-0.3.4/ox_ui/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/assets/
--rw-------   0 emin      (1000) emin      (1000)       55 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/assets/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/assets/css/
--rw-------   0 emin      (1000) emin      (1000)       19 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/assets/css/__init__.py
--rw-------   0 emin      (1000) emin      (1000)    23563 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/assets/css/w3.css
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/core/
--rw-------   0 emin      (1000) emin      (1000)       31 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/core/__init__.py
--rw-rw-r--   0 emin      (1000) emin      (1000)    13909 2023-05-15 18:12:01.000000 ox_ui-0.3.4/ox_ui/core/c2f.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     7069 2022-05-09 17:50:36.000000 ox_ui-0.3.4/ox_ui/core/c2g.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     2556 2023-05-15 17:41:26.000000 ox_ui-0.3.4/ox_ui/core/decorators.py
--rw-------   0 emin      (1000) emin      (1000)     1405 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/core/sample_wtf.html
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/test_tools/
--rw-------   0 emin      (1000) emin      (1000)       39 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/test_tools/__init__.py
--rw-------   0 emin      (1000) emin      (1000)     2938 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/test_tools/server_tools.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui.egg-info/
--rw-------   0 emin      (1000) emin      (1000)      535 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)      629 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/SOURCES.txt
--rw-------   0 emin      (1000) emin      (1000)        1 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/dependency_links.txt
--rw-------   0 emin      (1000) emin      (1000)       40 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/entry_points.txt
--rw-------   0 emin      (1000) emin      (1000)        7 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/requires.txt
--rw-------   0 emin      (1000) emin      (1000)        6 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/top_level.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)      689 2023-05-15 18:12:44.000000 ox_ui-0.3.4/requirements.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-05-15 18:13:17.113673 ox_ui-0.3.4/setup.cfg
--rw-------   0 emin      (1000) emin      (1000)     1941 2019-07-23 18:05:48.000000 ox_ui-0.3.4/setup.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.109673 ox_ui-0.3.4/tests/
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/tests/flask/
--rw-rw-r--   0 emin      (1000) emin      (1000)     2490 2023-05-15 18:10:02.000000 ox_ui-0.3.4/tests/flask/c2f_app.py
--rw-------   0 emin      (1000) emin      (1000)      219 2019-07-23 18:01:55.000000 ox_ui-0.3.4/tests/flask/minimal_app.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     3655 2023-05-15 18:12:01.000000 ox_ui-0.3.4/tests/flask/test_simple_c2f.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/
+-rw-------   0 emin      (1000) emin      (1000)     1129 2019-07-23 18:08:30.000000 ox_ui-0.3.5/.gitignore
+-rw-------   0 emin      (1000) emin      (1000)     1325 2019-07-23 18:03:49.000000 ox_ui-0.3.5/LICENSE.txt
+-rw-------   0 emin      (1000) emin      (1000)       56 2019-07-24 15:29:34.000000 ox_ui-0.3.5/MANIFEST.in
+-rw-rw-r--   0 emin      (1000) emin      (1000)      535 2023-05-15 19:12:33.767293 ox_ui-0.3.5/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)       82 2019-07-23 18:08:09.000000 ox_ui-0.3.5/README.org
+-rw-rw-r--   0 emin      (1000) emin      (1000)       93 2022-04-19 15:06:12.000000 ox_ui-0.3.5/README.rst
+-rw-------   0 emin      (1000) emin      (1000)       73 2019-07-23 18:03:49.000000 ox_ui-0.3.5/conftest.py
+-rw-------   0 emin      (1000) emin      (1000)      459 2019-07-23 18:04:11.000000 ox_ui-0.3.5/makefile
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.763293 ox_ui-0.3.5/ox_ui/
+-rw-rw-r--   0 emin      (1000) emin      (1000)       67 2023-05-15 19:11:41.000000 ox_ui-0.3.5/ox_ui/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/ox_ui/assets/
+-rw-------   0 emin      (1000) emin      (1000)       55 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/assets/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/ox_ui/assets/css/
+-rw-------   0 emin      (1000) emin      (1000)       19 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/assets/css/__init__.py
+-rw-------   0 emin      (1000) emin      (1000)    23563 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/assets/css/w3.css
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/ox_ui/core/
+-rw-------   0 emin      (1000) emin      (1000)       31 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/core/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)    13909 2023-05-15 18:12:01.000000 ox_ui-0.3.5/ox_ui/core/c2f.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     7069 2022-05-09 17:50:36.000000 ox_ui-0.3.5/ox_ui/core/c2g.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     5914 2023-05-15 19:11:41.000000 ox_ui-0.3.5/ox_ui/core/decorators.py
+-rw-------   0 emin      (1000) emin      (1000)     1405 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/core/sample_wtf.html
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/ox_ui/test_tools/
+-rw-------   0 emin      (1000) emin      (1000)       39 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/test_tools/__init__.py
+-rw-------   0 emin      (1000) emin      (1000)     2938 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/test_tools/server_tools.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.763293 ox_ui-0.3.5/ox_ui.egg-info/
+-rw-------   0 emin      (1000) emin      (1000)      535 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)      629 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/SOURCES.txt
+-rw-------   0 emin      (1000) emin      (1000)        1 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/dependency_links.txt
+-rw-------   0 emin      (1000) emin      (1000)       40 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/entry_points.txt
+-rw-------   0 emin      (1000) emin      (1000)        7 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/requires.txt
+-rw-------   0 emin      (1000) emin      (1000)        6 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/top_level.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)      689 2023-05-15 18:12:44.000000 ox_ui-0.3.5/requirements.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-05-15 19:12:33.767293 ox_ui-0.3.5/setup.cfg
+-rw-------   0 emin      (1000) emin      (1000)     1941 2019-07-23 18:05:48.000000 ox_ui-0.3.5/setup.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.763293 ox_ui-0.3.5/tests/
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/tests/flask/
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2538 2023-05-15 19:11:41.000000 ox_ui-0.3.5/tests/flask/c2f_app.py
+-rw-------   0 emin      (1000) emin      (1000)      219 2019-07-23 18:01:55.000000 ox_ui-0.3.5/tests/flask/minimal_app.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     3655 2023-05-15 18:12:01.000000 ox_ui-0.3.5/tests/flask/test_simple_c2f.py
```

### Comparing `ox_ui-0.3.4/.gitignore` & `ox_ui-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/LICENSE.txt` & `ox_ui-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/PKG-INFO` & `ox_ui-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox_ui
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simple user interface tools for python
 Home-page: http://github.com/emin63/ox_ui
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_ui-0.3.4/ox_ui/assets/css/w3.css` & `ox_ui-0.3.5/ox_ui/assets/css/w3.css`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/ox_ui/core/c2f.py` & `ox_ui-0.3.5/ox_ui/core/c2f.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/ox_ui/core/c2g.py` & `ox_ui-0.3.5/ox_ui/core/c2g.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/ox_ui/core/sample_wtf.html` & `ox_ui-0.3.5/ox_ui/core/sample_wtf.html`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/ox_ui/test_tools/server_tools.py` & `ox_ui-0.3.5/ox_ui/test_tools/server_tools.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/ox_ui.egg-info/PKG-INFO` & `ox_ui-0.3.5/ox_ui.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox-ui
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simple user interface tools for python
 Home-page: http://github.com/emin63/ox_ui
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_ui-0.3.4/ox_ui.egg-info/SOURCES.txt` & `ox_ui-0.3.5/ox_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/requirements.txt` & `ox_ui-0.3.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/setup.py` & `ox_ui-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.4/tests/flask/c2f_app.py` & `ox_ui-0.3.5/tests/flask/c2f_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 """
 
 import datetime
 
 import click
 from flask import Flask, url_for
 
-from ox_ui.core import c2f
+from ox_ui.core import c2f, decorators
+
 
 APP = Flask(__name__)
 APP.config['WTF_CSRF_ENABLED'] = False
+decorators.setup_flask_watch(APP)
+
 
 @click.command()
 @click.option('--count', default=1, type=int, help='how many times to say it')
 @click.option('--text', default='hi', type=str, help='what to say')
 def hello_cmd(count, text):
     'say hello'
```

### Comparing `ox_ui-0.3.4/tests/flask/test_simple_c2f.py` & `ox_ui-0.3.5/tests/flask/test_simple_c2f.py`

 * *Files identical despite different names*

