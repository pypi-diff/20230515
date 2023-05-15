# Comparing `tmp/py3Dmol-2.0.1.post1.tar.gz` & `tmp/py3Dmol-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3Dmol-2.0.1.post1.tar", last modified: Fri Feb 10 19:43:31 2023, max compression
+gzip compressed data, was "py3Dmol-2.0.3.tar", last modified: Mon May 15 12:40:14 2023, max compression
```

## Comparing `py3Dmol-2.0.1.post1.tar` & `py3Dmol-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dkoes     (1000) dkoes     (1000)        0 2023-02-10 19:43:31.099433 py3Dmol-2.0.1.post1/
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     1023 2023-01-02 16:10:55.000000 py3Dmol-2.0.1.post1/LICENSE.txt
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)       38 2023-01-02 16:10:55.000000 py3Dmol-2.0.1.post1/MANIFEST.in
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     2016 2023-02-10 19:43:31.099433 py3Dmol-2.0.1.post1/PKG-INFO
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     1219 2023-01-04 19:01:38.000000 py3Dmol-2.0.1.post1/README.md
-drwxrwxr-x   0 dkoes     (1000) dkoes     (1000)        0 2023-02-10 19:43:31.099433 py3Dmol-2.0.1.post1/py3Dmol/
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)    14002 2023-02-10 19:34:14.000000 py3Dmol-2.0.1.post1/py3Dmol/__init__.py
-drwxrwxr-x   0 dkoes     (1000) dkoes     (1000)        0 2023-02-10 19:43:31.099433 py3Dmol-2.0.1.post1/py3Dmol.egg-info/
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     2016 2023-02-10 19:43:30.000000 py3Dmol-2.0.1.post1/py3Dmol.egg-info/PKG-INFO
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)      226 2023-02-10 19:43:31.000000 py3Dmol-2.0.1.post1/py3Dmol.egg-info/SOURCES.txt
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)        1 2023-02-10 19:43:31.000000 py3Dmol-2.0.1.post1/py3Dmol.egg-info/dependency_links.txt
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)       19 2023-02-10 19:43:31.000000 py3Dmol-2.0.1.post1/py3Dmol.egg-info/requires.txt
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)        8 2023-02-10 19:43:31.000000 py3Dmol-2.0.1.post1/py3Dmol.egg-info/top_level.txt
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)      108 2023-02-10 19:43:31.099433 py3Dmol-2.0.1.post1/setup.cfg
--rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     2768 2023-02-10 19:43:05.000000 py3Dmol-2.0.1.post1/setup.py
+drwxrwxr-x   0 dkoes     (1000) dkoes     (1000)        0 2023-05-15 12:40:14.911244 py3Dmol-2.0.3/
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     1023 2023-01-02 16:10:55.000000 py3Dmol-2.0.3/LICENSE.txt
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)       38 2023-01-02 16:10:55.000000 py3Dmol-2.0.3/MANIFEST.in
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     2010 2023-05-15 12:40:14.911244 py3Dmol-2.0.3/PKG-INFO
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     1219 2023-01-04 19:01:38.000000 py3Dmol-2.0.3/README.md
+drwxrwxr-x   0 dkoes     (1000) dkoes     (1000)        0 2023-05-15 12:40:14.911244 py3Dmol-2.0.3/py3Dmol/
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)    14756 2023-05-13 22:18:54.000000 py3Dmol-2.0.3/py3Dmol/__init__.py
+drwxrwxr-x   0 dkoes     (1000) dkoes     (1000)        0 2023-05-15 12:40:14.911244 py3Dmol-2.0.3/py3Dmol.egg-info/
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     2010 2023-05-15 12:40:14.000000 py3Dmol-2.0.3/py3Dmol.egg-info/PKG-INFO
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)      226 2023-05-15 12:40:14.000000 py3Dmol-2.0.3/py3Dmol.egg-info/SOURCES.txt
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)        1 2023-05-15 12:40:14.000000 py3Dmol-2.0.3/py3Dmol.egg-info/dependency_links.txt
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)       19 2023-05-15 12:40:14.000000 py3Dmol-2.0.3/py3Dmol.egg-info/requires.txt
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)        8 2023-05-15 12:40:14.000000 py3Dmol-2.0.3/py3Dmol.egg-info/top_level.txt
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)      108 2023-05-15 12:40:14.911244 py3Dmol-2.0.3/setup.cfg
+-rw-rw-r--   0 dkoes     (1000) dkoes     (1000)     2843 2023-05-15 12:39:58.000000 py3Dmol-2.0.3/setup.py
```

### Comparing `py3Dmol-2.0.1.post1/LICENSE.txt` & `py3Dmol-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py3Dmol-2.0.1.post1/PKG-INFO` & `py3Dmol-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3Dmol
-Version: 2.0.1.post1
+Version: 2.0.3
 Summary: An IPython interface for embedding 3Dmol.js views in Jupyter notebooks
 Home-page: https://3dmol.org
 Author: David Koes
 Author-email: dkoes@pitt.edu
 License: MIT
 Keywords: molecule protein visualization
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py3Dmol-2.0.1.post1/README.md` & `py3Dmol-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `py3Dmol-2.0.1.post1/py3Dmol/__init__.py` & `py3Dmol-2.0.3/py3Dmol/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 import json
 import sys
+import re
 
 try:
     import IPython.display
     _has_IPython = True
 except ImportError:
     _has_IPython = False
 
@@ -49,15 +50,15 @@
        specify which viewer they apply to (with viewer=(r,c)) or will apply to all
        viewers in the grid.
 
        The API for the created object is exactly that for $3Dmol.GLViewer, with
        the exception that the functions all return None.
        http://3dmol.org/doc/GLViewer.html
     '''
-    def __init__(self,query='',width=640,height=480,viewergrid=None,data=None,style=None,linked=True,options=dict(),js='https://cdnjs.cloudflare.com/ajax/libs/3Dmol/2.0.1/3Dmol-min.js'):
+    def __init__(self,query='',width=640,height=480,viewergrid=None,data=None,style=None,linked=True,options=dict(),js='https://cdnjs.cloudflare.com/ajax/libs/3Dmol/2.0.3/3Dmol-min.js'):
         '''Create a 3Dmol.js view.
             width -- width in pixels of container
             height -- height in pixels of container
             query -- optional argument to provide to $3Dmol.download
             viewergrid -- optional tuple (rows,columns) to define grid
             data -- molecular data to provide to addModel, wit viewer grid can be indexed (r,c)
             style -- style to apply, with viewer grid can be indexed (r,c)
@@ -67,15 +68,15 @@
         warnid = "3dmolwarning_UNIQUEID"
         self.uniqueid = None
         #convert numerical width/height to pixels
         if type(width) == int:
             width = '%dpx'%width
         if type(height) == int:
             height = '%dpx'%height
-        self.startjs = '''<div id="%s"  style="position: relative; width: %s; height: %s">
+        self.startjs = '''<div id="%s"  style="position: relative; width: %s; height: %s;">
         <p id="%s" style="background-color:#ffcccc;color:black">You appear to be running in JupyterLab (or JavaScript failed to load for some other reason).  You need to install the 3dmol extension: <br>
         <tt>jupyter labextension install jupyterlab_3dmol</tt></p>
         </div>\n''' % (divid,width,height,warnid)
         self.startjs += '<script>\n'
         self.endjs = '</script>'
 
         self.updatejs = '' # code added since last show
@@ -204,14 +205,39 @@
                 %s
                 viewer_%s.render();
             });
             </script>''' % (self.updatejs.replace('UNIQUEID',self.uniqueid),self.uniqueid)
         self.updatejs = ''
         return IPython.display.publish_display_data({'application/3dmoljs_load.v0':script, 'text/html': script},metadata={})
 
+
+    def write_html(self, f=None, fullpage=False):
+      '''Write html to reproduce viewer in a web page to a file.
+      f -- file name (str) or writeable file object; if unspecified html string is returned
+      fullpage -- instead of specified width/height make viewer fill the web page
+      '''
+      
+      if f == None:
+        return self._make_html()
+        
+      if type(f) == str:
+        f = open(f,'wt')
+      html = self._make_html()
+      html = f'''<html>
+<body style="margin: 0; padding: 0; display: block;">
+{html}
+</body>
+</html>'''
+      if fullpage:
+        html = re.sub(r'width: (\S+);', 'width: 100%;', html)
+        html = re.sub(r'height: (\S+);', 'height: 100vh;', html)
+        
+      f.write(html)
+      
+      
     @using_ipython
     def png(self):
         '''output png image of viewer, which must already be instantiated'''
         if not self.uniqueid:
             raise AssertionError('Must instantiate viewer before generating image.')
         script = '''<img id="img_{0}">
             <script>
```

### Comparing `py3Dmol-2.0.1.post1/py3Dmol.egg-info/PKG-INFO` & `py3Dmol-2.0.3/py3Dmol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3Dmol
-Version: 2.0.1.post1
+Version: 2.0.3
 Summary: An IPython interface for embedding 3Dmol.js views in Jupyter notebooks
 Home-page: https://3dmol.org
 Author: David Koes
 Author-email: dkoes@pitt.edu
 License: MIT
 Keywords: molecule protein visualization
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py3Dmol-2.0.1.post1/setup.py` & `py3Dmol-2.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 setup(
     name='py3Dmol',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.0.1.post1',
+    # Keep version in synce with 3Dmol.js version.  Use "postX" suffix if needed
+    version='2.0.3',
 
     description='An IPython interface for embedding 3Dmol.js views in Jupyter notebooks',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://3dmol.org',
```

