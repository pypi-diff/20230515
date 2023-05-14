# Comparing `tmp/testcell-0.0.4.tar.gz` & `tmp/testcell-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcell-0.0.4.tar", last modified: Sat May 13 16:05:12 2023, max compression
+gzip compressed data, was "testcell-0.0.5.tar", last modified: Sun May 14 22:08:32 2023, max compression
```

## Comparing `testcell-0.0.4.tar` & `testcell-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-13 16:05:12.915533 testcell-0.0.4/
--rw-rw-r--   0 dldev     (1000) dldev     (1000)    11357 2023-05-01 12:51:46.000000 testcell-0.0.4/LICENSE
--rw-rw-r--   0 dldev     (1000) dldev     (1000)      111 2023-04-27 10:12:58.000000 testcell-0.0.4/MANIFEST.in
--rw-r--r--   0 dldev     (1000) dldev     (1000)     6222 2023-05-13 16:05:12.911533 testcell-0.0.4/PKG-INFO
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     5400 2023-05-13 16:03:22.000000 testcell-0.0.4/README.md
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     1018 2023-05-13 16:03:22.000000 testcell-0.0.4/settings.ini
--rw-r--r--   0 dldev     (1000) dldev     (1000)       38 2023-05-13 16:05:12.915533 testcell-0.0.4/setup.cfg
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     2596 2023-04-27 10:12:58.000000 testcell-0.0.4/setup.py
-drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-13 16:05:12.911533 testcell-0.0.4/testcell/
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     1289 2023-05-13 16:03:22.000000 testcell-0.0.4/testcell/__init__.py
--rw-r--r--   0 dldev     (1000) dldev     (1000)     1506 2023-05-13 16:01:07.000000 testcell-0.0.4/testcell/_modidx.py
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     2746 2023-05-13 16:03:22.000000 testcell-0.0.4/testcell/core.py
-drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-13 16:05:12.911533 testcell-0.0.4/testcell.egg-info/
--rw-r--r--   0 dldev     (1000) dldev     (1000)     6222 2023-05-13 16:05:12.000000 testcell-0.0.4/testcell.egg-info/PKG-INFO
--rw-r--r--   0 dldev     (1000) dldev     (1000)      334 2023-05-13 16:05:12.000000 testcell-0.0.4/testcell.egg-info/SOURCES.txt
--rw-r--r--   0 dldev     (1000) dldev     (1000)        1 2023-05-13 16:05:12.000000 testcell-0.0.4/testcell.egg-info/dependency_links.txt
--rw-r--r--   0 dldev     (1000) dldev     (1000)       38 2023-05-13 16:05:12.000000 testcell-0.0.4/testcell.egg-info/entry_points.txt
--rw-r--r--   0 dldev     (1000) dldev     (1000)        1 2023-05-01 13:54:05.000000 testcell-0.0.4/testcell.egg-info/not-zip-safe
--rw-r--r--   0 dldev     (1000) dldev     (1000)       25 2023-05-13 16:05:12.000000 testcell-0.0.4/testcell.egg-info/requires.txt
--rw-r--r--   0 dldev     (1000) dldev     (1000)        9 2023-05-13 16:05:12.000000 testcell-0.0.4/testcell.egg-info/top_level.txt
+drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-14 22:08:32.995519 testcell-0.0.5/
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)    11357 2023-05-01 12:51:46.000000 testcell-0.0.5/LICENSE
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)      111 2023-04-27 10:12:58.000000 testcell-0.0.5/MANIFEST.in
+-rw-r--r--   0 dldev     (1000) dldev     (1000)     6222 2023-05-14 22:08:32.995519 testcell-0.0.5/PKG-INFO
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     5400 2023-05-13 16:03:22.000000 testcell-0.0.5/README.md
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     1018 2023-05-14 22:04:21.000000 testcell-0.0.5/settings.ini
+-rw-r--r--   0 dldev     (1000) dldev     (1000)       38 2023-05-14 22:08:32.995519 testcell-0.0.5/setup.cfg
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     2596 2023-04-27 10:12:58.000000 testcell-0.0.5/setup.py
+drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-14 22:08:32.991518 testcell-0.0.5/testcell/
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     1289 2023-05-14 22:04:21.000000 testcell-0.0.5/testcell/__init__.py
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     1612 2023-05-14 22:04:21.000000 testcell-0.0.5/testcell/_modidx.py
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     3175 2023-05-14 22:04:21.000000 testcell-0.0.5/testcell/core.py
+drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-14 22:08:32.995519 testcell-0.0.5/testcell.egg-info/
+-rw-r--r--   0 dldev     (1000) dldev     (1000)     6222 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/PKG-INFO
+-rw-r--r--   0 dldev     (1000) dldev     (1000)      334 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/SOURCES.txt
+-rw-r--r--   0 dldev     (1000) dldev     (1000)        1 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/dependency_links.txt
+-rw-r--r--   0 dldev     (1000) dldev     (1000)       38 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/entry_points.txt
+-rw-r--r--   0 dldev     (1000) dldev     (1000)        1 2023-05-01 13:54:05.000000 testcell-0.0.5/testcell.egg-info/not-zip-safe
+-rw-r--r--   0 dldev     (1000) dldev     (1000)       25 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/requires.txt
+-rw-r--r--   0 dldev     (1000) dldev     (1000)        9 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/top_level.txt
```

### Comparing `testcell-0.0.4/LICENSE` & `testcell-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `testcell-0.0.4/PKG-INFO` & `testcell-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcell
-Version: 0.0.4
+Version: 0.0.5
 Summary: testcell prevents your testing cells from affecting the global namespace
 Home-page: https://github.com/artste/testcell
 Author: Stefano Giomo
 Author-email: artste@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `testcell-0.0.4/README.md` & `testcell-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `testcell-0.0.4/settings.ini` & `testcell-0.0.5/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = testcell
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = testcell
```

### Comparing `testcell-0.0.4/setup.py` & `testcell-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `testcell-0.0.4/testcell/__init__.py` & `testcell-0.0.5/testcell/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_testcell.ipynb.
 
 # %% auto 0
 __all__ = ['testcell', 'testcelln']
 
 # %% ../nbs/02_testcell.ipynb 4
 import ast
```

### Comparing `testcell-0.0.4/testcell/_modidx.py` & `testcell-0.0.5/testcell/_modidx.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
                 'doc_host': 'https://artste.github.io',
                 'git_url': 'https://github.com/artste/testcell',
                 'lib_path': 'testcell'},
   'syms': { 'testcell.core': { 'testcell.core.auto_display': ('ast.html#auto_display', 'testcell/core.py'),
                                'testcell.core.code_till_node': ('ast.html#code_till_node', 'testcell/core.py'),
                                'testcell.core.extract_call': ('ast.html#extract_call', 'testcell/core.py'),
                                'testcell.core.is_assignment': ('ast.html#is_assignment', 'testcell/core.py'),
+                               'testcell.core.is_ast_node': ('ast.html#is_ast_node', 'testcell/core.py'),
                                'testcell.core.is_function_call': ('ast.html#is_function_call', 'testcell/core.py'),
                                'testcell.core.is_import_statement': ('ast.html#is_import_statement', 'testcell/core.py'),
                                'testcell.core.last_node': ('ast.html#last_node', 'testcell/core.py'),
                                'testcell.core.last_statement_has_semicolon': ('ast.html#last_statement_has_semicolon', 'testcell/core.py'),
                                'testcell.core.need_display': ('ast.html#need_display', 'testcell/core.py'),
                                'testcell.core.node_source': ('ast.html#node_source', 'testcell/core.py'),
                                'testcell.core.wrap_node': ('ast.html#wrap_node', 'testcell/core.py')}}}
```

### Comparing `testcell-0.0.4/testcell/core.py` & `testcell-0.0.5/testcell/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,87 +1,98 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_ast.ipynb.
 
 # %% auto 0
-__all__ = ['last_node', 'node_source', 'is_assignment', 'extract_call', 'is_function_call', 'is_import_statement', 'need_display',
-           'wrap_node', 'last_statement_has_semicolon', 'code_till_node', 'auto_display']
+__all__ = ['last_node', 'node_source', 'is_assignment', 'extract_call', 'is_function_call', 'is_import_statement', 'is_ast_node',
+           'need_display', 'wrap_node', 'last_statement_has_semicolon', 'code_till_node', 'auto_display']
 
 # %% ../nbs/01_ast.ipynb 3
 import ast
 
 # %% ../nbs/01_ast.ipynb 5
 def last_node(code):
     tree = ast.parse(code)
     if len(tree.body)==0: return None
     src = tree.body[-1]
     last_node = None
+    parent_node = None
     for node in ast.walk(src):
         if isinstance(node, ast.stmt):
+            parent_node = last_node
             last_node = node
+    if parent_node is not None: return None # deal with nested statements like "for loop".
     return last_node
 
 # %% ../nbs/01_ast.ipynb 7
 def node_source(node,code):
     return ast.get_source_segment(code,node)
 
-# %% ../nbs/01_ast.ipynb 10
+# %% ../nbs/01_ast.ipynb 13
 def is_assignment(node):
     return isinstance(node, ast.Assign)
 
-# %% ../nbs/01_ast.ipynb 12
+# %% ../nbs/01_ast.ipynb 15
 def extract_call(node):
     if not isinstance(node, ast.Expr): return None
     node = node.value # step in
     if isinstance(node, ast.Name): return None # "fn"
     if isinstance(node, ast.Call):
         n = node.func # step in
         if isinstance(n, ast.Name): return n.id # "fn()"
         if isinstance(n, ast.Attribute): return n.attr
     return None # all the rest is not supported
 
-# %% ../nbs/01_ast.ipynb 14
+# %% ../nbs/01_ast.ipynb 17
 def is_function_call(node,names):
     function_name = extract_call(node)
     if function_name is None: return False # this is not a function call
     return function_name in names
 
-# %% ../nbs/01_ast.ipynb 16
+# %% ../nbs/01_ast.ipynb 19
 def is_import_statement(node):
     return isinstance(node, (ast.Import, ast.ImportFrom))
 
-# %% ../nbs/01_ast.ipynb 18
+# %% ../nbs/01_ast.ipynb 21
+def is_ast_node(x,ref):
+    for t in ref:
+        if isinstance(x,t): return True
+    return False
+
+# %% ../nbs/01_ast.ipynb 24
 def need_display(node):
     if node is None: return False
+    if is_assignment(node): return False
     if is_function_call(node,names=['print','display']): return False
+    if is_ast_node(node,ref=[ast.Delete, ast.Assert, ast.Global, ast.Nonlocal]): return False
     if is_import_statement(node): return False
     return True
 
-# %% ../nbs/01_ast.ipynb 20
+# %% ../nbs/01_ast.ipynb 26
 def wrap_node(node,function_name):
     return ast.Expr(
         value=ast.Call(
             func=ast.Name(id=function_name, ctx=ast.Load()),
             args=[node],
             keywords=[])
         )
 
-# %% ../nbs/01_ast.ipynb 23
+# %% ../nbs/01_ast.ipynb 29
 def last_statement_has_semicolon(code):
     t = [x.strip() for x in code.splitlines()]
     t = [x for x in t if not x.startswith('#')]
     return t[-1].endswith(';')
 
-# %% ../nbs/01_ast.ipynb 25
+# %% ../nbs/01_ast.ipynb 31
 def code_till_node(code:str,node):
     t = code.splitlines()
     t = t[:node.lineno]
     t[-1] = t[-1][:node.col_offset]
     if len(t[-1])==0: t = t[:-1]
     return '\n'.join(t)
 
-# %% ../nbs/01_ast.ipynb 28
+# %% ../nbs/01_ast.ipynb 34
 def auto_display(code):
     if last_statement_has_semicolon(code): return code
     
     n = last_node(code)
     if not need_display(n): return code
     
     ns = node_source(n,code)
```

### Comparing `testcell-0.0.4/testcell.egg-info/PKG-INFO` & `testcell-0.0.5/testcell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcell
-Version: 0.0.4
+Version: 0.0.5
 Summary: testcell prevents your testing cells from affecting the global namespace
 Home-page: https://github.com/artste/testcell
 Author: Stefano Giomo
 Author-email: artste@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

