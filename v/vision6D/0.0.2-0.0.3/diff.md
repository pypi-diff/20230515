# Comparing `tmp/vision6D-0.0.2.tar.gz` & `tmp/vision6D-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.0.2.tar", last modified: Sun May 14 22:26:06 2023, max compression
+gzip compressed data, was "dist\vision6D-0.0.3.tar", last modified: Mon May 15 19:06:14 2023, max compression
```

## Comparing `vision6D-0.0.2.tar` & `vision6D-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:06.185261 vision6D-0.0.2/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      793 2023-05-14 22:26:06.186261 vision6D-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      106 2023-05-11 21:10:38.000000 vision6D-0.0.2/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1918 2023-05-14 22:26:06.207264 vision6D-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       65 2023-01-03 15:55:08.000000 vision6D-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:06.142265 vision6D-0.0.2/test/
--rw-rw-rw-   0        0        0    21974 2023-05-11 22:16:59.000000 vision6D-0.0.2/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-04-21 21:41:53.000000 vision6D-0.0.2/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:06.162264 vision6D-0.0.2/vision6D/
--rw-rw-rw-   0        0        0    45348 2023-05-14 22:21:14.000000 vision6D-0.0.2/vision6D/GUI.py
--rw-rw-rw-   0        0        0      935 2023-05-09 15:00:33.000000 vision6D-0.0.2/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-05 15:04:28.000000 vision6D-0.0.2/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-11 22:14:53.000000 vision6D-0.0.2/vision6D/config.py
--rw-rw-rw-   0        0        0    22897 2023-05-08 19:47:11.000000 vision6D-0.0.2/vision6D/interface.py
--rw-rw-rw-   0        0        0    28492 2023-05-14 22:15:55.000000 vision6D-0.0.2/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-08 19:54:14.000000 vision6D-0.0.2/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14911 2023-05-08 18:27:06.000000 vision6D-0.0.2/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:06.182261 vision6D-0.0.2/vision6D.egg-info/
--rw-rw-rw-   0        0        0      793 2023-05-14 22:26:05.000000 vision6D-0.0.2/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-05-14 22:26:06.000000 vision6D-0.0.2/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 22:26:05.000000 vision6D-0.0.2/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-05-14 22:26:05.000000 vision6D-0.0.2/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 22:26:05.000000 vision6D-0.0.2/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 19:06:14.473451 vision6D-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1603 2023-05-15 19:06:14.473451 vision6D-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-15 16:36:59.000000 vision6D-0.0.3/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1918 2023-05-15 19:06:14.490448 vision6D-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-01-03 15:55:08.000000 vision6D-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:06:14.325445 vision6D-0.0.3/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-14 22:36:01.000000 vision6D-0.0.3/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.0.3/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:06:14.399447 vision6D-0.0.3/vision6D/
+-rw-rw-rw-   0        0        0    45496 2023-05-15 16:26:28.000000 vision6D-0.0.3/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      961 2023-05-14 22:53:44.000000 vision6D-0.0.3/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.0.3/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-14 22:36:01.000000 vision6D-0.0.3/vision6D/config.py
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.0.3/vision6D/interface.py
+-rw-rw-rw-   0        0        0    28492 2023-05-14 22:36:02.000000 vision6D-0.0.3/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.0.3/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0      509 2023-05-14 22:53:44.000000 vision6D-0.0.3/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.0.3/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.0.3/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:06:14.471448 vision6D-0.0.3/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-15 19:06:14.000000 vision6D-0.0.3/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-05-15 19:06:14.000000 vision6D-0.0.3/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 19:06:14.000000 vision6D-0.0.3/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-05-15 19:06:14.000000 vision6D-0.0.3/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 19:06:14.000000 vision6D-0.0.3/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.0.2/LICENSE` & `vision6D-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.2/setup.cfg` & `vision6D-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 7572  sion = 0.0.2..ur
+00000020: 7369 6f6e 203d 2030 2e30 2e33 0d0a 7572  sion = 0.0.3..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.0.2/test/test_create_dataset.py` & `vision6D-0.0.3/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.2/test/test_projection.py` & `vision6D-0.0.3/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.2/vision6D/GUI.py` & `vision6D-0.0.3/vision6D/GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,41 +310,44 @@
     def add_image_file(self, prompt=True):
         if prompt:
             if self.image_path == None or self.image_path == '':
                 self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg)")
             else:
                 self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.image_path).parent), "Files (*.png *.jpg)")
 
-        if self.image_path != '': 
+        if self.image_path != '':
+            self.hintLabel.hide()
             image_source = np.array(PIL.Image.open(self.image_path), dtype='uint8')
             if len(image_source.shape) == 2: image_source = image_source[..., None]
             self.add_image(image_source)
             
     def add_mask_file(self, prompt=True):
         if prompt:
             if self.mask_path == None or self.mask_path == '':
                 self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg)")
             else:
                 self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.mask_path).parent), "Files (*.png *.jpg)")
         
         if self.mask_path != '':
+            self.hintLabel.hide()
             mask_source = np.array(PIL.Image.open(self.mask_path), dtype='uint8')
             if len(mask_source.shape) == 2: mask_source = mask_source[..., None]
             self.add_mask(mask_source)
 
     def add_mesh_file(self, mesh_name=None, prompt=True):
         if prompt:
             if self.mesh_path == None or self.mesh_path == '':
                 self.mesh_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.mesh *.ply *.stl *.obj *.off *.dae *.fbx *.3ds *.x3d)")
             else:
                 self.mesh_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.mesh_path).parent), "Files (*.mesh *.ply)")
-
+        
         if self.mesh_path != '':
+            self.hintLabel.hide()
             if mesh_name is None:
-                mesh_name, ok = self.input_dialog.getText(self, 'Input', 'Specify the object Class name', text='ossicles')
+                mesh_name, ok = self.input_dialog.getText(self, 'Input', 'Specify the object Class name')#, text='ossicles')
                 if not ok: return 0
 
             self.meshdict[mesh_name] = self.mesh_path
             self.mesh_opacity[mesh_name] = self.surface_opacity
             transformation_matrix = self.transformation_matrix
             if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix                   
@@ -353,15 +356,16 @@
     def add_pose_file(self, prompt=True):
         if prompt:
             if self.pose_path == None or self.pose_path == '':
                 self.pose_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.npy)")
             else:
                 self.pose_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.pose_path).parent), "Files (*.npy)")
         
-        if self.pose_path != '': 
+        if self.pose_path != '':
+            self.hintLabel.hide()
             transformation_matrix = np.load(self.pose_path)
             self.transformation_matrix = transformation_matrix
             if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             self.add_pose(matrix=transformation_matrix)
     
     def mirror_actors(self, direction):
```

### Comparing `vision6D-0.0.2/vision6D/__init__.py` & `vision6D-0.0.3/vision6D/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 # Setup the logging configuration
 logging.config.dictConfig(LOGGING_CONFIG)
 
 from .app import App
 from .interface import Interface
 from .interface_gui import Interface_GUI
 from . import utils
-from . import config
+from . import config
+from .run_gui import exe
```

### Comparing `vision6D-0.0.2/vision6D/app.py` & `vision6D-0.0.3/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.2/vision6D/config.py` & `vision6D-0.0.3/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.2/vision6D/interface.py` & `vision6D-0.0.3/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.2/vision6D/interface_gui.py` & `vision6D-0.0.3/vision6D/interface_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.2/vision6D/mainwindow.py` & `vision6D-0.0.3/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.2/vision6D/utils.py` & `vision6D-0.0.3/vision6D/utils.py`

 * *Files identical despite different names*

