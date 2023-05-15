# Comparing `tmp/mslex-0.2.0.tar.gz` & `tmp/mslex-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mslex-0.2.0.tar", last modified: Sun Oct  6 07:35:16 2019, max compression
+gzip compressed data, was "dist/mslex-0.3.0.tar", last modified: Sun Oct  6 21:56:48 2019, max compression
```

## Comparing `mslex-0.2.0.tar` & `mslex-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 07:35:16.000000 mslex-0.2.0/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     2921 2019-10-06 07:35:16.000000 mslex-0.2.0/PKG-INFO
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      587 2019-10-06 07:06:25.000000 mslex-0.2.0/LICENSE
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     3497 2019-10-06 07:06:25.000000 mslex-0.2.0/CONTRIBUTING.rst
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 07:35:16.000000 mslex-0.2.0/mslex.egg-info/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     2921 2019-10-06 07:35:15.000000 mslex-0.2.0/mslex.egg-info/PKG-INFO
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)        1 2019-10-03 04:23:25.000000 mslex-0.2.0/mslex.egg-info/not-zip-safe
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      581 2019-10-06 07:35:15.000000 mslex-0.2.0/mslex.egg-info/SOURCES.txt
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       49 2019-10-06 07:35:15.000000 mslex-0.2.0/mslex.egg-info/entry_points.txt
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)        6 2019-10-06 07:35:15.000000 mslex-0.2.0/mslex.egg-info/top_level.txt
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)        1 2019-10-06 07:35:15.000000 mslex-0.2.0/mslex.egg-info/dependency_links.txt
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 07:35:16.000000 mslex-0.2.0/tests/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       60 2019-10-06 07:06:25.000000 mslex-0.2.0/tests/__init__.py
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)    10752 2019-10-06 07:29:03.000000 mslex-0.2.0/tests/test_mslex.py
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      262 2019-10-06 07:06:25.000000 mslex-0.2.0/MANIFEST.in
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 07:35:16.000000 mslex-0.2.0/docs/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      302 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/index.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       33 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/contributing.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      607 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/Makefile
--rwxr-xr-x   0 lawrence_danna (941817330) admin       (80)     4793 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/conf.py
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       65 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/usage.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      767 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/make.bat
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 07:35:16.000000 mslex-0.2.0/docs/_build/
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 07:35:16.000000 mslex-0.2.0/docs/_build/html/
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 07:35:16.000000 mslex-0.2.0/docs/_build/html/_static/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       90 2019-10-03 05:23:34.000000 mslex-0.2.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      286 2019-10-03 05:23:34.000000 mslex-0.2.0/docs/_build/html/_static/file.png
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       90 2019-10-03 05:23:34.000000 mslex-0.2.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       28 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/history.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     1094 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/installation.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       28 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/authors.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       27 2019-10-06 07:06:25.000000 mslex-0.2.0/docs/readme.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     1411 2019-10-06 07:33:36.000000 mslex-0.2.0/setup.py
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       89 2019-10-06 07:06:25.000000 mslex-0.2.0/HISTORY.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      161 2019-10-06 07:06:25.000000 mslex-0.2.0/AUTHORS.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      379 2019-10-06 07:35:16.000000 mslex-0.2.0/setup.cfg
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     1678 2019-10-06 07:06:25.000000 mslex-0.2.0/README.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     4590 2019-10-06 07:33:36.000000 mslex-0.2.0/mslex.py
+drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)     2921 2019-10-06 21:56:48.000000 mslex-0.3.0/PKG-INFO
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)      587 2019-10-06 07:06:25.000000 mslex-0.3.0/LICENSE
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)     3497 2019-10-06 07:06:25.000000 mslex-0.3.0/CONTRIBUTING.rst
+drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/mslex.egg-info/
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)     2921 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/PKG-INFO
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)        1 2019-10-03 04:23:25.000000 mslex-0.3.0/mslex.egg-info/not-zip-safe
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)      581 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/SOURCES.txt
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       49 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/entry_points.txt
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)        6 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/top_level.txt
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)        1 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/dependency_links.txt
+drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/tests/
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       60 2019-10-06 07:06:25.000000 mslex-0.3.0/tests/__init__.py
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)    12030 2019-10-06 21:52:52.000000 mslex-0.3.0/tests/test_mslex.py
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)      262 2019-10-06 07:06:25.000000 mslex-0.3.0/MANIFEST.in
+drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/docs/
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)      302 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/index.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       33 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/contributing.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)      607 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/Makefile
+-rwxr-xr-x   0 lawrence_danna (941817330) admin       (80)     4793 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/conf.py
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       65 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/usage.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)      767 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/make.bat
+drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/docs/_build/
+drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/docs/_build/html/
+drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/docs/_build/html/_static/
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       90 2019-10-03 05:23:34.000000 mslex-0.3.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)      286 2019-10-03 05:23:34.000000 mslex-0.3.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       90 2019-10-03 05:23:34.000000 mslex-0.3.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       28 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/history.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)     1094 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/installation.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       28 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/authors.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       27 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/readme.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)     1411 2019-10-06 21:54:49.000000 mslex-0.3.0/setup.py
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)       89 2019-10-06 07:06:25.000000 mslex-0.3.0/HISTORY.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)      161 2019-10-06 07:06:25.000000 mslex-0.3.0/AUTHORS.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)      379 2019-10-06 21:56:48.000000 mslex-0.3.0/setup.cfg
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)     1678 2019-10-06 07:06:25.000000 mslex-0.3.0/README.rst
+-rw-r--r--   0 lawrence_danna (941817330) admin       (80)     5089 2019-10-06 21:54:49.000000 mslex-0.3.0/mslex.py
```

### Comparing `mslex-0.2.0/PKG-INFO` & `mslex-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mslex
-Version: 0.2.0
+Version: 0.3.0
 Summary: shlex for windows
 Home-page: https://github.com/smoofra/mslex
 Author: Lawrence D'Anna
 Author-email: larry@elder-gods.org
 License: Apache Software License 2.0
 Description: =====
         mslex
```

### Comparing `mslex-0.2.0/LICENSE` & `mslex-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mslex-0.2.0/CONTRIBUTING.rst` & `mslex-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mslex-0.2.0/mslex.egg-info/PKG-INFO` & `mslex-0.3.0/mslex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mslex
-Version: 0.2.0
+Version: 0.3.0
 Summary: shlex for windows
 Home-page: https://github.com/smoofra/mslex
 Author: Lawrence D'Anna
 Author-email: larry@elder-gods.org
 License: Apache Software License 2.0
 Description: =====
         mslex
```

### Comparing `mslex-0.2.0/mslex.egg-info/SOURCES.txt` & `mslex-0.3.0/mslex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mslex-0.2.0/tests/test_mslex.py` & `mslex-0.3.0/tests/test_mslex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """Tests for `mslex` package."""
 
 import sys
 import itertools
+import functools
 import unittest
 import subprocess
 
 from mslex import split, quote
 
 if sys.platform == 'win32':
     import ctypes
@@ -187,35 +188,52 @@
     ('\\\\\\\\""""""""""" x', ['\\\\"""', 'x']),
     ('\\\\\\\\"""""""""""" x', ['\\\\""""', 'x'])]
 
 
 cmd_examples = [
     (r'"foo &whoami bar"', ['foo &whoami bar']),
     (r'^^', ['^']),
+    (r'"^"', ['^']),
     (r'"^^"', ['^^']),
     (r'foo^bar', ['foobar']),
     (r'foo^^bar', ['foo^bar']),
     (r'"foo^bar"', ['foo^bar']),
     (r'"foo^^bar"', ['foo^^bar']),
     ]
 
 
+pretty_examples = [
+    (r'c:\Program Files\FooBar', r'"c:\Program Files\FooBar"'),
+    (r'c:\Program Files (x86)\FooBar', r'"c:\Program Files (x86)\FooBar"'),
+    (r'^', '"^"'),
+    (r' ^', '" ^"'),
+    (r'&', '"&"'),
+    (r'!', '^!'),
+    (r'!foo!', '^!foo^!'),
+    ("foo\\bar\\baz\\", 'foo\\bar\\baz\\'),
+    ("foo bar\\baz\\", '"foo bar\\baz\\\\"'),
+    ("foo () bar\\baz\\", '"foo () bar\\baz\\\\"'),
+    ("foo () bar\\baz\\\\", '"foo () bar\\baz\\\\\\\\"'),
+    ("foo () bar\\baz\\\\\\", '"foo () bar\\baz\\\\\\\\\\\\"'),
+    ("foo () bar\\baz\\\\\\\\", '"foo () bar\\baz\\\\\\\\\\\\\\\\"'),
+]
+
 class TestMslex(unittest.TestCase):
     """Tests for `mslex` package."""
 
     def case(self, s, ans, cmd):
         try:
             if ans is not None:
-                self.assertEqual(split(s), ans)
+                self.assertEqual(split(s, like_cmd=cmd), ans)
             if sys.platform == 'win32' and not cmd:
                 self.assertEqual(split(s), ctypes_split(s))
         except AssertionError:
             print(f"in: «{s}»")
             print()
-            for x in split(s):
+            for x in split(s, like_cmd=cmd):
                 print(f"out: «{x}»")
             print()
             if ans is not None:
                 for x in ans:
                     print(f"ans: «{x}»")
                 print()
             if sys.platform == 'win32':
@@ -256,47 +274,53 @@
                     self.case(s, None, False)
 
     def test_examples(self):
         for s, ans in examples:
             self.case(s, ans, cmd=False)
 
     def test_examples_for_cmd(self):
-        for s, ans in examples:
+        for s, ans in cmd_examples:
             self.case(s, ans, cmd=True)
 
     def test_quote_examples(self):
-        for s, ans in examples:
+        qu = functools.partial(quote, for_cmd=False)
+        sp = functools.partial(split, like_cmd=False)
+        for s, ans in itertools.chain(examples, cmd_examples):
+            self.assertEqual(ans, sp(' '.join(map(qu, ans))))
+
+    def test_quote_examples_cmd(self):
+        for s, ans in itertools.chain(examples, cmd_examples):
             self.assertEqual(ans, split(' '.join(map(quote, ans))))
 
-    def test_requote_examples(self):
+    def test_requote_examples_cmd(self):
         for s, ans in examples:
             self.assertEqual([s], split(quote(s)))
 
-    def test_requote_examples_nocmd(self):
+    def test_requote_examples(self):
         for s, ans in examples:
             self.assertEqual([s], split(quote(s, for_cmd=False), like_cmd=False))
 
     def test_quote_every_string(self):
 
         def every_string():
             chars = [' ', 'x', '"', '\\']
             prod = itertools.product(*itertools.repeat(chars, 8))
             for x in prod:
                 yield ''.join(x)
 
         for s in every_string():
-            q = quote(s)
-            self.assertEqual([s], split(q))
-            self.assertEqual([s, s], split(f'{q} {q}'))
+            q = quote(s, for_cmd=False)
+            self.assertEqual([s], split(q, like_cmd=False))
+            self.assertEqual([s, s], split(f'{q} {q}', like_cmd=False))
 
 
     def test_quote_every_string_for_cmd(self):
 
         def every_string():
-            chars = [' ', 'x', '"', '\\', '^', '&']
+            chars = [' ', 'x', '"', '\\', '^', '&', '!']
             prod = itertools.product(*itertools.repeat(chars, 6))
             for x in prod:
                 yield ''.join(x)
 
         for s in every_string():
             q = quote(s)
             self.assertEqual([s], split(q))
@@ -311,7 +335,13 @@
             for x in prod:
                 yield ''.join(x)
         for s in every_string():
             q = quote(s)
             if sys.platform == "win32":
                 proc = subprocess.run('python -c "import sys; print(sys.argv[1])" ' + q, shell=True, stdout=subprocess.PIPE)
                 self.assertEqual(proc.stdout.decode('ascii').rstrip(), s.rstrip())
+
+    def test_pretty_examples(self):
+        for s, ans in pretty_examples:
+            self.assertEqual(quote(s), ans)
+            self.assertEqual(split(ans), [s])
+            self.assertEqual(split(ans + ' ' + ans + " foo bar"), [s, s, 'foo', 'bar'])
```

### Comparing `mslex-0.2.0/docs/Makefile` & `mslex-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mslex-0.2.0/docs/conf.py` & `mslex-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mslex-0.2.0/docs/make.bat` & `mslex-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mslex-0.2.0/docs/installation.rst` & `mslex-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mslex-0.2.0/setup.py` & `mslex-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords='mslex',
     name='mslex',
     py_modules=['mslex'],
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/smoofra/mslex',
-    version='0.2.0',
+    version='0.3.0',
     zip_safe=False,
 )
```

### Comparing `mslex-0.2.0/README.rst` & `mslex-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `mslex-0.2.0/mslex.py` & `mslex-0.3.0/mslex.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import re
 import itertools
 
 __all__ = ('split', 'quote')
 
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 
 def iter_arg(peek, i):
     quote_mode = False
     for m in itertools.chain([peek], i):
         space, slashes, quotes, text = m.groups()
         if space:
             if quote_mode:
@@ -29,16 +29,20 @@
             yield text
 
 def iter_args(s):
     i = re.finditer(r'(\s+)|(\\*)(\"+)|(.[^\s\\\"]*)', s.lstrip())
     for m in i:
         yield ''.join(iter_arg(m, i))
 
+cmd_meta = r'([\"\^\&\|\<\>\(\)\%\!])'
+cmd_meta_or_space = r'[\s\"\^\&\|\<\>\(\)\%\!]'
 
-def split(s, like_cmd=True):
+cmd_meta_inside_quotes = r'([\"\%\!])'
+
+def split(s, like_cmd=True, check=True):
     """
     Split a string of command line arguments like DOS and Windows do.
 
     On windows, before a command line argument becomes a char* in a
     program's argv, it must be parsed by both cmd.exe, and by
     CommandLineToArgvW.
 
@@ -46,46 +50,44 @@
     CommandLineToArgvW.   Since cmd.exe is a shell, and can run
     external programs, this function obviously cannot emulate
     everything it does.   However if the string passed in would
     be parsed by cmd as a quoted literal, without command
     invocations like `&whoami`, and without string substitutions like
     `%PATH%`, then this function will split it accurately.
 
-    if like_cmd is false, then this will split the string like
+    If check is true, split will raise a ValueError if cmd metacharacters
+    occur in the string without being quoted.
+
+    f like_cmd is false, then this will split the string like
     CommandLineToArgvW does.
     """
-    if like_cmd and re.search(r'[\%\!\^]', s):
+    if like_cmd and re.search(cmd_meta, s):
         def i():
             quote_mode = False
             for m in re.finditer(r'(\^.)|(\")|([^\^\"]+)', s):
                 escaped, quote, text = m.groups()
                 if escaped:
                     if quote_mode:
                         yield escaped
+                        if escaped[1] == '"':
+                            quote_mode = False
                     else:
                         yield escaped[1]
                 elif quote:
                     yield '"'
                     quote_mode = not quote_mode
                 else:
                     yield text
+                    if check:
+                        meta = cmd_meta_inside_quotes if quote_mode else cmd_meta
+                        if re.search(meta, text):
+                            raise ValueError(f"unquoted cmd metacharacters in string: {repr(s)}")
         s = ''.join(i())
-        # def i(parts):
-        #     quote_mode = False
-        #     for part in parts:
-        #         if quote_mode:
-        #             yield re.sub(r'\^(.)', r'\1', part)
-        #         else:
-        #             yield part
-        #         quote_mode = not quote_mode
-        #s = '"'.join(i(s.split('"')))
     return list(iter_args(s))
 
-cmd_meta = r'([\"\^\&\|\<\>\(\)\%\!])'
-cmd_meta_or_space = r'[\s\"\^\&\|\<\>\(\)\%\!]'
 
 
 def quote(s, for_cmd=True):
     """
     Quote a string for use as a command line argument in DOS or Windows.
 
     On windows, before a command line argument becomes a char* in a
@@ -102,14 +104,22 @@
     parse correctly in both situations.
     """
     if not s:
         return '""'
     if not re.search(cmd_meta_or_space, s):
         return s
     if for_cmd and re.search(cmd_meta, s):
+        if not re.search(cmd_meta_inside_quotes, s):
+            m = re.search(r'\\+$', s)
+            if m:
+                return '"' + s + m.group() + '"'
+            else:
+                return '"' + s + '"'
+        if not re.search(r'[\s\"]', s):
+            return re.sub(cmd_meta, r'^\1', s)
         return re.sub(cmd_meta, r'^\1', quote(s, for_cmd=False))
     i = re.finditer(r'(\\*)(\"+)|(\\+)|([^\\\"]+)', s)
     def parts():
         yield '"'
         for m in i:
             pos,end = m.span()
             slashes, quotes, onlyslashes, text = m.groups()
```

