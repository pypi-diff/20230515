# Comparing `tmp/hydrogibs-0.3.1.tar.gz` & `tmp/hydrogibs-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.3.1.tar", last modified: Sun May 14 17:16:03 2023, max compression
+gzip compressed data, was "hydrogibs-0.3.2.tar", last modified: Mon May 15 06:35:27 2023, max compression
```

## Comparing `hydrogibs-0.3.1.tar` & `hydrogibs-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-14 17:16:03.007904 hydrogibs-0.3.1/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.1/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-14 17:16:03.007904 hydrogibs-0.3.1/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.3.1/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-14 17:16:03.003904 hydrogibs-0.3.1/hydrogibs/
--rwxrwxr-x   0 axel      (1000) axel      (1000)    12664 2023-05-14 16:53:37.000000 hydrogibs-0.3.1/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     5149 2023-05-14 16:38:39.000000 hydrogibs-0.3.1/hydrogibs/ModelApp.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.1/hydrogibs/ModelTemplate.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     8243 2023-05-14 16:42:20.000000 hydrogibs-0.3.1/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.1/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.3.1/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.3.1/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.1/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-14 17:16:03.007904 hydrogibs-0.3.1/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-14 17:16:02.000000 hydrogibs-0.3.1/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-05-14 17:16:02.000000 hydrogibs-0.3.1/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-05-14 17:16:02.000000 hydrogibs-0.3.1/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-05-14 17:16:02.000000 hydrogibs-0.3.1/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-05-14 17:15:52.000000 hydrogibs-0.3.1/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-05-14 17:16:03.007904 hydrogibs-0.3.1/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-15 06:35:27.352188 hydrogibs-0.3.2/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.2/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-15 06:35:27.352188 hydrogibs-0.3.2/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.3.2/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-15 06:35:27.352188 hydrogibs-0.3.2/hydrogibs/
+-rwxrwxr-x   0 axel      (1000) axel      (1000)    12664 2023-05-14 16:53:37.000000 hydrogibs-0.3.2/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     5162 2023-05-15 06:33:21.000000 hydrogibs-0.3.2/hydrogibs/ModelApp.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.2/hydrogibs/ModelTemplate.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     8243 2023-05-14 16:42:20.000000 hydrogibs-0.3.2/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.2/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.3.2/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.3.2/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.2/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-15 06:35:27.352188 hydrogibs-0.3.2/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-05-15 06:35:27.000000 hydrogibs-0.3.2/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-05-15 06:35:27.000000 hydrogibs-0.3.2/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-05-15 06:35:27.000000 hydrogibs-0.3.2/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-05-15 06:35:27.000000 hydrogibs-0.3.2/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-05-15 06:35:15.000000 hydrogibs-0.3.2/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-05-15 06:35:27.352188 hydrogibs-0.3.2/setup.cfg
```

### Comparing `hydrogibs-0.3.1/LICENSE` & `hydrogibs-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.1/PKG-INFO` & `hydrogibs-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.1
+Version: 0.3.2
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.3.1/hydrogibs/GR4.py` & `hydrogibs-0.3.2/hydrogibs/GR4.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.1/hydrogibs/ModelApp.py` & `hydrogibs-0.3.2/hydrogibs/ModelApp.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             close()
 
     def init_diagram(self, *args, **kwargs):
 
         diagram = self.event.diagram(*args, **kwargs)
 
         self.canvas = FigureCanvasTkAgg(diagram.figure, master=self.dframe)
-        toolbar = NavigationToolbar2Tk(self.canvas)
+        toolbar = NavigationToolbar2Tk(self.canvas, self.dframe)
         toolbar.update()
         self.canvas._tkcanvas.pack()
         self.canvas.draw()
         self.canvas.get_tk_widget().pack()
         self.canvas.mpl_connect('key_press_event',
                                 lambda arg: key_press_handler(
                                     arg, self.canvas, toolbar
```

### Comparing `hydrogibs-0.3.1/hydrogibs/ModelTemplate.py` & `hydrogibs-0.3.2/hydrogibs/ModelTemplate.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.1/hydrogibs/QDF.py` & `hydrogibs-0.3.2/hydrogibs/QDF.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.1/hydrogibs/RationalMethod.py` & `hydrogibs-0.3.2/hydrogibs/RationalMethod.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.1/hydrogibs/SoCoSe.py` & `hydrogibs-0.3.2/hydrogibs/SoCoSe.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.1/hydrogibs/misc.py` & `hydrogibs-0.3.2/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.1/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.3.2/hydrogibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.1
+Version: 0.3.2
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

