# Comparing `tmp/itkdb_gtk-0.0.5.tar.gz` & `tmp/itkdb_gtk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itkdb_gtk-0.0.5.tar", last modified: Thu May 11 14:24:10 2023, max compression
+gzip compressed data, was "itkdb_gtk-0.0.6.tar", last modified: Mon May 15 11:02:03 2023, max compression
```

## Comparing `itkdb_gtk-0.0.5.tar` & `itkdb_gtk-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-11 14:24:10.410026 itkdb_gtk-0.0.5/
--rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-05-11 14:24:10.409595 itkdb_gtk-0.0.5/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     1997 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.5/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-11 14:24:10.406049 itkdb_gtk-0.0.5/itkdb_gtk/
--rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.5/itkdb_gtk/GlueWeight.py
--rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.5/itkdb_gtk/ITkDB.desktop
--rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.5/itkdb_gtk/ITkDB.svg
--rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.5/itkdb_gtk/ITkDBlogin.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14208 2023-05-11 14:04:07.000000 itkdb_gtk-0.0.5/itkdb_gtk/ITkDButils.py
--rw-r--r--   0 lacasta    (503) staff       (20)      552 2023-04-11 16:04:01.000000 itkdb_gtk-0.0.5/itkdb_gtk/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3342 2023-04-13 14:46:29.000000 itkdb_gtk-0.0.5/itkdb_gtk/checkComponent.py
--rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.5/itkdb_gtk/checkJSon.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4375 2023-05-11 14:02:42.000000 itkdb_gtk-0.0.5/itkdb_gtk/dashBoard.py
--rw-r--r--   0 lacasta    (503) staff       (20)    20708 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.5/itkdb_gtk/dbGtkUtils.py
--rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.5/itkdb_gtk/getShipments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7140 2023-04-11 15:50:48.000000 itkdb_gtk-0.0.5/itkdb_gtk/groundingTest.py
--rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.5/itkdb_gtk/readAVSdata.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.5/itkdb_gtk/readGoogleSheet.py
--rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.5/itkdb_gtk/sendShipments.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    21093 2023-04-11 15:23:27.000000 itkdb_gtk-0.0.5/itkdb_gtk/uploadPetalInformation.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    13713 2023-05-11 14:22:11.000000 itkdb_gtk-0.0.5/itkdb_gtk/uploadTest.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-11 14:24:10.408900 itkdb_gtk-0.0.5/itkdb_gtk.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-05-11 14:24:10.000000 itkdb_gtk-0.0.5/itkdb_gtk.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      654 2023-05-11 14:24:10.000000 itkdb_gtk-0.0.5/itkdb_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-11 14:24:10.000000 itkdb_gtk-0.0.5/itkdb_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      239 2023-05-11 14:24:10.000000 itkdb_gtk-0.0.5/itkdb_gtk.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-05-11 14:24:10.000000 itkdb_gtk-0.0.5/itkdb_gtk.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-11 14:24:10.000000 itkdb_gtk-0.0.5/itkdb_gtk.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)     1087 2023-05-11 14:23:45.000000 itkdb_gtk-0.0.5/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-11 14:24:10.410133 itkdb_gtk-0.0.5/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-15 11:02:03.171526 itkdb_gtk-0.0.6/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-05-15 11:02:03.171124 itkdb_gtk-0.0.6/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     1997 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.6/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-15 11:02:03.164464 itkdb_gtk-0.0.6/itkdb_gtk/
+-rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.6/itkdb_gtk/GlueWeight.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.6/itkdb_gtk/ITkDB.desktop
+-rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.6/itkdb_gtk/ITkDB.svg
+-rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.6/itkdb_gtk/ITkDBlogin.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14208 2023-05-11 14:04:07.000000 itkdb_gtk-0.0.6/itkdb_gtk/ITkDButils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      552 2023-04-11 16:04:01.000000 itkdb_gtk-0.0.6/itkdb_gtk/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3342 2023-04-13 14:46:29.000000 itkdb_gtk-0.0.6/itkdb_gtk/checkComponent.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.6/itkdb_gtk/checkJSon.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4375 2023-05-11 14:02:42.000000 itkdb_gtk-0.0.6/itkdb_gtk/dashBoard.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    20708 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.6/itkdb_gtk/dbGtkUtils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.6/itkdb_gtk/getShipments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7140 2023-04-11 15:50:48.000000 itkdb_gtk-0.0.6/itkdb_gtk/groundingTest.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.6/itkdb_gtk/readAVSdata.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.6/itkdb_gtk/readGoogleSheet.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.6/itkdb_gtk/sendShipments.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    21093 2023-04-11 15:23:27.000000 itkdb_gtk-0.0.6/itkdb_gtk/uploadPetalInformation.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    13689 2023-05-15 10:52:22.000000 itkdb_gtk-0.0.6/itkdb_gtk/uploadTest.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-15 11:02:03.170466 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      654 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      239 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)     1087 2023-05-15 11:01:53.000000 itkdb_gtk-0.0.6/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-15 11:02:03.171638 itkdb_gtk-0.0.6/setup.cfg
```

### Comparing `itkdb_gtk-0.0.5/PKG-INFO` & `itkdb_gtk-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb_gtk
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.5/README.md` & `itkdb_gtk-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/GlueWeight.py` & `itkdb_gtk-0.0.6/itkdb_gtk/GlueWeight.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/ITkDB.svg` & `itkdb_gtk-0.0.6/itkdb_gtk/ITkDB.svg`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/ITkDBlogin.py` & `itkdb_gtk-0.0.6/itkdb_gtk/ITkDBlogin.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/ITkDButils.py` & `itkdb_gtk-0.0.6/itkdb_gtk/ITkDButils.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/__init__.py` & `itkdb_gtk-0.0.6/itkdb_gtk/__init__.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/checkComponent.py` & `itkdb_gtk-0.0.6/itkdb_gtk/checkComponent.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/checkJSon.py` & `itkdb_gtk-0.0.6/itkdb_gtk/checkJSon.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/dashBoard.py` & `itkdb_gtk-0.0.6/itkdb_gtk/dashBoard.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/dbGtkUtils.py` & `itkdb_gtk-0.0.6/itkdb_gtk/dbGtkUtils.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/getShipments.py` & `itkdb_gtk-0.0.6/itkdb_gtk/getShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/groundingTest.py` & `itkdb_gtk-0.0.6/itkdb_gtk/groundingTest.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/readAVSdata.py` & `itkdb_gtk-0.0.6/itkdb_gtk/readAVSdata.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/readGoogleSheet.py` & `itkdb_gtk-0.0.6/itkdb_gtk/readGoogleSheet.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/sendShipments.py` & `itkdb_gtk-0.0.6/itkdb_gtk/sendShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/uploadPetalInformation.py` & `itkdb_gtk-0.0.6/itkdb_gtk/uploadPetalInformation.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk/uploadTest.py` & `itkdb_gtk-0.0.6/itkdb_gtk/uploadTest.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,16 +244,14 @@
                     if site:
                         self.data["institution"] = site
                         self.write_message("Setting Institution to {}\n".format(self.data["institution"]))
 
                 else:
                     dbGtkUtils.complain("Invalid JSON file\n{}".format('\n'.join(errors)), fnam)
 
-                return
-
             self.entrySN.set_text(self.data["component"])
             self.entryTest.set_text(self.data["testType"])
 
         except Exception as E:
             self.data = None
             self.write_message("Cannot load file {}\n".format(fnam))
             self.write_message("{}\n".format(str(E)))
```

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk.egg-info/PKG-INFO` & `itkdb_gtk-0.0.6/itkdb_gtk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb-gtk
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.5/itkdb_gtk.egg-info/SOURCES.txt` & `itkdb_gtk-0.0.6/itkdb_gtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.5/pyproject.toml` & `itkdb_gtk-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itkdb_gtk"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of Gtk based GUI to access ITkDB."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

