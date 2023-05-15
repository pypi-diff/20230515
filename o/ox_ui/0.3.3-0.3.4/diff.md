# Comparing `tmp/ox_ui-0.3.3.tar.gz` & `tmp/ox_ui-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_ui-0.3.3.tar", last modified: Tue Jul  5 21:16:56 2022, max compression
+gzip compressed data, was "ox_ui-0.3.4.tar", last modified: Mon May 15 18:13:17 2023, max compression
```

## Comparing `ox_ui-0.3.3.tar` & `ox_ui-0.3.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2022-07-05 21:16:56.314553 ox_ui-0.3.3/
--rw-------   0 emin      (1000) emin      (1000)     1129 2019-07-23 18:08:30.000000 ox_ui-0.3.3/.gitignore
--rw-------   0 emin      (1000) emin      (1000)     1325 2019-07-23 18:03:49.000000 ox_ui-0.3.3/LICENSE.txt
--rw-------   0 emin      (1000) emin      (1000)       56 2019-07-24 15:29:34.000000 ox_ui-0.3.3/MANIFEST.in
--rw-rw-r--   0 emin      (1000) emin      (1000)      535 2022-07-05 21:16:56.314553 ox_ui-0.3.3/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)       82 2019-07-23 18:08:09.000000 ox_ui-0.3.3/README.org
--rw-rw-r--   0 emin      (1000) emin      (1000)       93 2022-04-19 15:06:12.000000 ox_ui-0.3.3/README.rst
--rw-------   0 emin      (1000) emin      (1000)       73 2019-07-23 18:03:49.000000 ox_ui-0.3.3/conftest.py
--rw-------   0 emin      (1000) emin      (1000)      459 2019-07-23 18:04:11.000000 ox_ui-0.3.3/makefile
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2022-07-05 21:16:56.310553 ox_ui-0.3.3/ox_ui/
--rw-rw-r--   0 emin      (1000) emin      (1000)       67 2022-07-05 21:16:46.000000 ox_ui-0.3.3/ox_ui/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2022-07-05 21:16:56.310553 ox_ui-0.3.3/ox_ui/assets/
--rw-------   0 emin      (1000) emin      (1000)       55 2019-07-23 18:01:55.000000 ox_ui-0.3.3/ox_ui/assets/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2022-07-05 21:16:56.310553 ox_ui-0.3.3/ox_ui/assets/css/
--rw-------   0 emin      (1000) emin      (1000)       19 2019-07-23 18:01:55.000000 ox_ui-0.3.3/ox_ui/assets/css/__init__.py
--rw-------   0 emin      (1000) emin      (1000)    23563 2019-07-23 18:01:55.000000 ox_ui-0.3.3/ox_ui/assets/css/w3.css
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2022-07-05 21:16:56.310553 ox_ui-0.3.3/ox_ui/core/
--rw-------   0 emin      (1000) emin      (1000)       31 2019-07-23 18:01:55.000000 ox_ui-0.3.3/ox_ui/core/__init__.py
--rw-rw-r--   0 emin      (1000) emin      (1000)    13588 2022-07-05 21:16:46.000000 ox_ui-0.3.3/ox_ui/core/c2f.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     7069 2022-05-09 17:50:36.000000 ox_ui-0.3.3/ox_ui/core/c2g.py
--rw-------   0 emin      (1000) emin      (1000)     1405 2019-07-23 18:01:55.000000 ox_ui-0.3.3/ox_ui/core/sample_wtf.html
--rw-rw-r--   0 emin      (1000) emin      (1000)       67 2022-05-26 18:03:01.000000 ox_ui-0.3.3/ox_ui/flycheck___init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2022-07-05 21:16:56.314553 ox_ui-0.3.3/ox_ui/test_tools/
--rw-------   0 emin      (1000) emin      (1000)       39 2019-07-23 18:01:55.000000 ox_ui-0.3.3/ox_ui/test_tools/__init__.py
--rw-------   0 emin      (1000) emin      (1000)     2938 2019-07-23 18:01:55.000000 ox_ui-0.3.3/ox_ui/test_tools/server_tools.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2022-07-05 21:16:56.310553 ox_ui-0.3.3/ox_ui.egg-info/
--rw-------   0 emin      (1000) emin      (1000)      535 2022-07-05 21:16:56.000000 ox_ui-0.3.3/ox_ui.egg-info/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)      631 2022-07-05 21:16:56.000000 ox_ui-0.3.3/ox_ui.egg-info/SOURCES.txt
--rw-------   0 emin      (1000) emin      (1000)        1 2022-07-05 21:16:56.000000 ox_ui-0.3.3/ox_ui.egg-info/dependency_links.txt
--rw-------   0 emin      (1000) emin      (1000)       40 2022-07-05 21:16:56.000000 ox_ui-0.3.3/ox_ui.egg-info/entry_points.txt
--rw-------   0 emin      (1000) emin      (1000)        7 2022-07-05 21:16:56.000000 ox_ui-0.3.3/ox_ui.egg-info/requires.txt
--rw-------   0 emin      (1000) emin      (1000)        6 2022-07-05 21:16:56.000000 ox_ui-0.3.3/ox_ui.egg-info/top_level.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)      689 2022-05-26 18:04:04.000000 ox_ui-0.3.3/requirements.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)       38 2022-07-05 21:16:56.314553 ox_ui-0.3.3/setup.cfg
--rw-------   0 emin      (1000) emin      (1000)     1941 2019-07-23 18:05:48.000000 ox_ui-0.3.3/setup.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2022-07-05 21:16:56.310553 ox_ui-0.3.3/tests/
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2022-07-05 21:16:56.314553 ox_ui-0.3.3/tests/flask/
--rw-rw-r--   0 emin      (1000) emin      (1000)     2490 2022-04-19 15:06:33.000000 ox_ui-0.3.3/tests/flask/c2f_app.py
--rw-------   0 emin      (1000) emin      (1000)      219 2019-07-23 18:01:55.000000 ox_ui-0.3.3/tests/flask/minimal_app.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     3004 2022-04-19 15:06:33.000000 ox_ui-0.3.3/tests/flask/test_simple_c2f.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/
+-rw-------   0 emin      (1000) emin      (1000)     1129 2019-07-23 18:08:30.000000 ox_ui-0.3.4/.gitignore
+-rw-------   0 emin      (1000) emin      (1000)     1325 2019-07-23 18:03:49.000000 ox_ui-0.3.4/LICENSE.txt
+-rw-------   0 emin      (1000) emin      (1000)       56 2019-07-24 15:29:34.000000 ox_ui-0.3.4/MANIFEST.in
+-rw-rw-r--   0 emin      (1000) emin      (1000)      535 2023-05-15 18:13:17.113673 ox_ui-0.3.4/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)       82 2019-07-23 18:08:09.000000 ox_ui-0.3.4/README.org
+-rw-rw-r--   0 emin      (1000) emin      (1000)       93 2022-04-19 15:06:12.000000 ox_ui-0.3.4/README.rst
+-rw-------   0 emin      (1000) emin      (1000)       73 2019-07-23 18:03:49.000000 ox_ui-0.3.4/conftest.py
+-rw-------   0 emin      (1000) emin      (1000)      459 2019-07-23 18:04:11.000000 ox_ui-0.3.4/makefile
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/
+-rw-rw-r--   0 emin      (1000) emin      (1000)       67 2023-05-15 17:41:26.000000 ox_ui-0.3.4/ox_ui/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/assets/
+-rw-------   0 emin      (1000) emin      (1000)       55 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/assets/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/assets/css/
+-rw-------   0 emin      (1000) emin      (1000)       19 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/assets/css/__init__.py
+-rw-------   0 emin      (1000) emin      (1000)    23563 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/assets/css/w3.css
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/core/
+-rw-------   0 emin      (1000) emin      (1000)       31 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/core/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)    13909 2023-05-15 18:12:01.000000 ox_ui-0.3.4/ox_ui/core/c2f.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     7069 2022-05-09 17:50:36.000000 ox_ui-0.3.4/ox_ui/core/c2g.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2556 2023-05-15 17:41:26.000000 ox_ui-0.3.4/ox_ui/core/decorators.py
+-rw-------   0 emin      (1000) emin      (1000)     1405 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/core/sample_wtf.html
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui/test_tools/
+-rw-------   0 emin      (1000) emin      (1000)       39 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/test_tools/__init__.py
+-rw-------   0 emin      (1000) emin      (1000)     2938 2019-07-23 18:01:55.000000 ox_ui-0.3.4/ox_ui/test_tools/server_tools.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/ox_ui.egg-info/
+-rw-------   0 emin      (1000) emin      (1000)      535 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)      629 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/SOURCES.txt
+-rw-------   0 emin      (1000) emin      (1000)        1 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/dependency_links.txt
+-rw-------   0 emin      (1000) emin      (1000)       40 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/entry_points.txt
+-rw-------   0 emin      (1000) emin      (1000)        7 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/requires.txt
+-rw-------   0 emin      (1000) emin      (1000)        6 2023-05-15 18:13:17.000000 ox_ui-0.3.4/ox_ui.egg-info/top_level.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)      689 2023-05-15 18:12:44.000000 ox_ui-0.3.4/requirements.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-05-15 18:13:17.113673 ox_ui-0.3.4/setup.cfg
+-rw-------   0 emin      (1000) emin      (1000)     1941 2019-07-23 18:05:48.000000 ox_ui-0.3.4/setup.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.109673 ox_ui-0.3.4/tests/
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 18:13:17.113673 ox_ui-0.3.4/tests/flask/
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2490 2023-05-15 18:10:02.000000 ox_ui-0.3.4/tests/flask/c2f_app.py
+-rw-------   0 emin      (1000) emin      (1000)      219 2019-07-23 18:01:55.000000 ox_ui-0.3.4/tests/flask/minimal_app.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     3655 2023-05-15 18:12:01.000000 ox_ui-0.3.4/tests/flask/test_simple_c2f.py
```

### Comparing `ox_ui-0.3.3/.gitignore` & `ox_ui-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.3/LICENSE.txt` & `ox_ui-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.3/PKG-INFO` & `ox_ui-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox_ui
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple user interface tools for python
 Home-page: http://github.com/emin63/ox_ui
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_ui-0.3.3/ox_ui/assets/css/w3.css` & `ox_ui-0.3.4/ox_ui/assets/css/w3.css`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.3/ox_ui/core/c2f.py` & `ox_ui-0.3.4/ox_ui/core/c2f.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,25 +170,25 @@
 
 
 class ClickToWTF:
 
     def __init__(self, clickCmd, skip_opt_re=None, tweaks: list = None,
                  fill_get_from_url: bool = False):
         """Initializer.
-        
+
         :param clickCmd:   A click command to turn into a form.
-        
+
         :param skip_opt_re=None:  Regexp for options to skip in form.
-        
+
         :param tweaks:  List of 'tweaks' to add (e.g., FileResponseTweak).
-        
+
         :param fill_get_from_url:  If True, then when doing a GET request
                                    to fill out arguments we look in the
                                    URL params to override standard defaults.
-        
+
         """
         self.clickCmd = clickCmd
         self.rawTemplate = None
         self.skip_opt_re = skip_opt_re if not skip_opt_re else re.compile(
             skip_opt_re)
         self.tweaks = tweaks if tweaks else []
         self.fill_get_from_url = fill_get_from_url
@@ -214,15 +214,15 @@
 
         for opt in self.click_cmd_params():
             field = self.click_opt_to_wtf_field(opt)
             setattr(ClickForm, opt.name, field)
 
         if request.method == 'GET' and self.fill_get_from_url:
             self.populate_form_from_url(ClickForm)
-            
+
         return ClickForm
 
     def populate_form_from_url(self, ClickForm):
         """Populate a form from URL parameters.
 
         :param ClickForm:  Class form click form as produced by `form_cls`.
 
@@ -256,15 +256,23 @@
         return None
 
     def pad_kwargs(self, kwargs):
         for tweak in self.tweaks:
             tweak.pad_kwargs(self, kwargs)
 
     def form(self):
-        cls = self.form_cls()
+        try:
+            cls = self.form_cls()
+        except Exception as prob:  # pylint: disable=broad-except
+            #  Sometimes if you do a POST and do not provide all the
+            #  values expected by a form, newer versions of Flask will
+            #  have problems.
+            logging.exception(
+                'Unable to make form. If doing a POST; verify data provided.')
+            raise
         return cls()
 
     @classmethod
     def click_opt_to_wtf_field(cls, opt):
         validators = []
         if opt.required:
             validators.append(
@@ -349,15 +357,15 @@
         def get_form_data(self):
             data = super().get_form_data()
             data['my_custom_data'] = SOMETHING
             return data
 
         """
         return {'intro': self.clickCmd.help}
-        
+
     def show_form(self, form=None, template=None):
         if form is None:
             form = self.form()
         data = self.get_form_data()
         if template:
             result = render_template(template, form=form, **data)
         else:
```

### Comparing `ox_ui-0.3.3/ox_ui/core/c2g.py` & `ox_ui-0.3.4/ox_ui/core/c2g.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.3/ox_ui/core/sample_wtf.html` & `ox_ui-0.3.4/ox_ui/core/sample_wtf.html`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.3/ox_ui/test_tools/server_tools.py` & `ox_ui-0.3.4/ox_ui/test_tools/server_tools.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.3/ox_ui.egg-info/PKG-INFO` & `ox_ui-0.3.4/ox_ui.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox-ui
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple user interface tools for python
 Home-page: http://github.com/emin63/ox_ui
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_ui-0.3.3/ox_ui.egg-info/SOURCES.txt` & `ox_ui-0.3.4/ox_ui.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 README.org
 README.rst
 conftest.py
 makefile
 requirements.txt
 setup.py
 ox_ui/__init__.py
-ox_ui/flycheck___init__.py
 ox_ui.egg-info/PKG-INFO
 ox_ui.egg-info/SOURCES.txt
 ox_ui.egg-info/dependency_links.txt
 ox_ui.egg-info/entry_points.txt
 ox_ui.egg-info/requires.txt
 ox_ui.egg-info/top_level.txt
 ox_ui/assets/__init__.py
 ox_ui/assets/css/__init__.py
 ox_ui/assets/css/w3.css
 ox_ui/core/__init__.py
 ox_ui/core/c2f.py
 ox_ui/core/c2g.py
+ox_ui/core/decorators.py
 ox_ui/core/sample_wtf.html
 ox_ui/test_tools/__init__.py
 ox_ui/test_tools/server_tools.py
 tests/flask/c2f_app.py
 tests/flask/minimal_app.py
 tests/flask/test_simple_c2f.py
```

### Comparing `ox_ui-0.3.3/requirements.txt` & `ox_ui-0.3.4/requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 astroid==2.11.1
 attrs==21.4.0
-certifi==2021.10.8
+certifi==2022.12.7
 charset-normalizer==2.0.12
 click==8.0.4
 dill==0.3.4
 execnet==1.9.0
 eyap==0.9.3
 flake8==4.0.1
 Flask==2.0.3
@@ -32,11 +32,11 @@
 pytest-xdist==2.5.0
 python-dateutil==2.8.2
 requests==2.27.1
 six==1.16.0
 tomli==2.0.1
 typing-extensions==4.1.1
 urllib3==1.26.9
-Werkzeug==2.0.3
+Werkzeug==2.2.3
 wrapt==1.14.0
 WTForms==3.0.1
 xmltodict==0.13.0
```

### Comparing `ox_ui-0.3.3/setup.py` & `ox_ui-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.3/tests/flask/c2f_app.py` & `ox_ui-0.3.4/tests/flask/c2f_app.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.3/tests/flask/test_simple_c2f.py` & `ox_ui-0.3.4/tests/flask/test_simple_c2f.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+"""Test using flask server.
+"""
 
+import logging
 import os
+import socket
+import time
 import pathlib
 import unittest
 import tempfile
 
 import requests
 
 import ox_ui
@@ -18,14 +23,26 @@
     def setUpClass(cls):
         cmd = ['flask', 'run']
         cwd = pathlib.Path(ox_ui.__file__).parents[1].joinpath(
             'tests', 'flask')
         env = os.environ.copy()
         env['FLASK_APP'] = str(cwd.joinpath('c2f_app.py'))
         cls.server_info = server_tools.start_server(cmd=cmd, cwd=cwd, env=env)
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        for attempt in range(10):
+            result = sock.connect_ex(('127.0.0.1', cls.server_info.s_port))
+            if result == 0:
+                logging.info('Succesfully started server at port %s',
+                             cls.server_info.s_port)
+                break
+            else:
+                logging.warning('Sleeping 2**%i to wait for server', attempt)
+                time.sleep(2**i)
+        else:
+            raise ValueError('Could not start flask server.')
 
     @classmethod
     def tearDownClass(cls):
         s_proc = cls.server_info.s_proc
         if s_proc:
             s_proc.kill()
             s_proc.wait(timeout=10)
@@ -44,15 +61,15 @@
                 self.assertEqual(req.text, str(len(data)))
 
     def test_choice(self):
         "Test if the choice mapping works right."
 
         url = 'http://127.0.0.1:%s/favorite_color' % (
             self.server_info.s_port)
-        post_req = requests.post(url)  # default
+        post_req = requests.post(url, data={'color': 'green'})  # default
         self.assertEqual(post_req.status_code, 200)
         self.assertEqual(post_req.text, 'I like green as well.')
         post_req = requests.post(url, data={'color': 'red'})  # choose red
         self.assertEqual(post_req.status_code, 200)
         self.assertEqual(post_req.text, 'I like red as well.')
 
     def test_good_c2f(self):
```

