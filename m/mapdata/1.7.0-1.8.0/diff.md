# Comparing `tmp/mapdata-1.7.0.tar.gz` & `tmp/mapdata-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-1.7.0.tar", last modified: Sat May 13 16:49:05 2023, max compression
+gzip compressed data, was "mapdata-1.8.0.tar", last modified: Mon May 15 01:29:58 2023, max compression
```

## Comparing `mapdata-1.7.0.tar` & `mapdata-1.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-13 16:49:05.014003 mapdata-1.7.0/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-1.7.0/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-1.7.0/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     2695 2023-05-13 16:49:05.014003 mapdata-1.7.0/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     1568 2023-05-13 16:28:26.000000 mapdata-1.7.0/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-13 16:49:05.014003 mapdata-1.7.0/mapdata/
--rwxr-xr-x   0 dreas     (1000) dreas     (1000)    84192 2023-05-13 16:18:06.000000 mapdata-1.7.0/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-13 16:49:05.014003 mapdata-1.7.0/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     2695 2023-05-13 16:49:04.000000 mapdata-1.7.0/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-05-13 16:49:04.000000 mapdata-1.7.0/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-13 16:49:04.000000 mapdata-1.7.0/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-13 16:49:04.000000 mapdata-1.7.0/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-05-13 16:49:05.014003 mapdata-1.7.0/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1270 2023-05-13 16:48:57.000000 mapdata-1.7.0/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-15 01:29:58.169349 mapdata-1.8.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-1.8.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-1.8.0/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-15 01:29:58.169349 mapdata-1.8.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     1866 2023-05-15 01:02:57.000000 mapdata-1.8.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-15 01:29:58.169349 mapdata-1.8.0/mapdata/
+-rwxr-xr-x   0 dreas     (1000) dreas     (1000)    84596 2023-05-15 00:27:28.000000 mapdata-1.8.0/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-15 01:29:58.169349 mapdata-1.8.0/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-15 01:29:58.000000 mapdata-1.8.0/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-05-15 01:29:58.000000 mapdata-1.8.0/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-15 01:29:58.000000 mapdata-1.8.0/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-15 01:29:58.000000 mapdata-1.8.0/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-05-15 01:29:58.169349 mapdata-1.8.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1279 2023-05-15 00:34:38.000000 mapdata-1.8.0/setup.py
```

### Comparing `mapdata-1.7.0/LICENSE.txt` & `mapdata-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-1.7.0/PKG-INFO` & `mapdata-1.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 1.7.0
+Version: 1.8.0
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
@@ -20,14 +20,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Scientific/Engineering
 Requires: tkintermapview
 Requires: pyproj
+Requires: odfpy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
@@ -55,9 +56,15 @@
 The map can be exported to a Postscript, PNG, or JPEG file.  Using command-line options,
 *mapdata* can be directed to load a data file and display location markers and then to
 export the map to an image file, and quit.
 
 Selected rows in the data table can be exported to a CSV file.
 
 
+Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
+
+A configuration file template, application icons for Linux and Windows, a .desktop
+file for Linux, and additional bitmap symbols, are available for download from
+[OSDN](https://osdn.net/projects/mapdata/releases/).
+
```

### Comparing `mapdata-1.7.0/mapdata/mapdata.py` & `mapdata-1.8.0/mapdata/mapdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,21 @@
 #				settings for the location symbol, color, font, font size,
 #				font color, and font location, and allowed all of those to
 #				be changed via the configuration file.  RDN.
 #	2023-05-08	Added conversion of other coordinate reference systems to 4326.  RDN.
 #	2023-05-09	Added ability to switch CRSs for the same data.  RDN.
 #	2023-05-11	Fixed map controls when resizing.  Added command-line arguments
 #				to export the map and quit.  RDN.
-#	2020-05-12	Added export of configuration settings.  Cleaned up help
+#	2023-05-12	Added export of configuration settings.  Cleaned up help
 #				dialogs.  RDN.
+#	2023-05-14	Put the map and table in a PanedWindow.  RDN.
 # ==================================================================
 
-version = "1.7.0"
-vdate = "2023-05-12"
+version = "1.8.0"
+vdate = "2023-05-14"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -81,14 +82,15 @@
 import datetime
 import time
 import tkinter as tk
 import tkinter.ttk as ttk
 import tkinter.font as tkfont
 import tkinter.filedialog as tkfiledialog
 import tkintermapview as tkmv
+from PIL import ImageGrab
 
 
 # Default name of configuration file.  Files with other names may be read.
 config_file_name = "mapdata.conf"
 
 # Configuration files read on startup
 config_files = []
@@ -385,14 +387,22 @@
 # List of imported symbol names and paths
 imported_symbols = []
 
 # Keys for custom symbols are made up of the color name and the icon name, separated with a space.
 custom_icons = {}
 
 
+# X11 bitmap for the application window icon
+win_icon_xbm = """#define window_icon_width 16
+#define window_icon_height 16
+static unsigned char window_icon_bits[] = {
+   0xff, 0xff, 0x01, 0x80, 0x01, 0x84, 0x01, 0x8e, 0x01, 0x9f, 0x81, 0xbf,
+   0x21, 0x80, 0x71, 0x80, 0xf9, 0x80, 0xfd, 0x81, 0x01, 0x84, 0x01, 0x8e,
+   0x01, 0x9f, 0x81, 0xbf, 0x01, 0x80, 0xff, 0xff};"""
+
 def warning(message):
 	tk.messagebox.showerror("Warning", message)
 
 def fatal_error(message):
 	tk.messagebox.showerror("Fatal error", message)
 	sys.exit()
 
@@ -513,14 +523,17 @@
 			self.win._root().deiconify()
 		self.full_fn = os.path.abspath(fn)
 		base_fn = os.path.basename(fn)
 		self.win.title("Map of %s" % base_fn)
 		headers, rows = file_data(fn)
 		self.headers = headers
 		self.rows = rows
+		# Set the application window icon
+		#win_icon = tk.BitmapImage(data=win_icon_xbm, foreground="black", background="tan")
+		#self.win.iconbitmap(win_icon)
 		# Source and possibly un-projected crs
 		self.src_crs = crs
 		self.crs = crs
 		# Created column names for un-projected coordinates
 		self.lat_4326_col = None
 		self.lon_4326_col = None
 		# The markers for all the locations in the data table
@@ -539,36 +552,40 @@
 		# Initializes selection marker to the global settings
 		self.set_sel_marker(select_symbol, select_color)
 		# Create icons for the buttonbar
 		expand_icon = tk.BitmapImage(data=expand_xbm, foreground="black")
 		focus_icon = tk.BitmapImage(data=wedge_sm_xbm, foreground="red")
 		zoom_sel_icon = tk.BitmapImage(data=wedges_3_xbm, foreground="red")
 		unselect_icon = tk.BitmapImage(data=cancel_xbm, foreground="black")
-		# Use stacked frames for the main application window components
+		# Use stacked frames for the main application window components.  Map and table in a PanedWindow.
 		msgframe = ttk.Frame(self.win, padding="3 2")
 		ctrlframe = ttk.Frame(self.win, padding="3 2")
-		mapframe = ttk.Frame(self.win, borderwidth=2, relief=tk.RIDGE)
-		self.tblframe = ttk.Frame(self.win, padding="3 2")
+		datapanes = ttk.PanedWindow(self.win, orient=tk.VERTICAL)
+		mapframe = ttk.Frame(datapanes, borderwidth=2, relief=tk.RIDGE)
+		self.tblframe = ttk.Frame(datapanes, padding="3 2")
+		datapanes.add(mapframe, weight=1)
+		datapanes.add(self.tblframe, weight=1)
 		# Allow vertical resizing of map and table frames, not of message and control frames
 		self.win.columnconfigure(0, weight=1)
-		self.win.rowconfigure(0, weight=0)
-		self.win.rowconfigure(1, weight=0)
-		self.win.rowconfigure(2, weight=1)
-		self.win.rowconfigure(3, weight=1)
+		self.win.rowconfigure(0, weight=0)		# msgframe
+		self.win.rowconfigure(1, weight=0)		# ctrlframe
+		self.win.rowconfigure(2, weight=1)		# datapanes
+		# Grid all the main frames
+		msgframe.grid(row=0, column=0, sticky=tk.NSEW)
+		ctrlframe.grid(row=1, column=0, sticky=tk.W)
+		datapanes.grid(row=2, column=0, sticky=tk.NSEW)
 		# Populate the message frame
 		self.msg_label = ttk.Label(msgframe, text=message)
 		def wrap_msg(event):
 			self.msg_label.configure(wraplength=event.width - 5)
 		self.msg_label.bind("<Configure>", wrap_msg)
 		self.msg_label.grid(column=0, row=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		msgframe.columnconfigure(0, weight=1)
 		msgframe.rowconfigure(0, weight=1)
-		msgframe.grid(row=0, column=0, sticky=tk.NSEW)
 		# Populate the map control frame
-		ctrlframe.grid(row=1, column=0, sticky=tk.W)
 		ctrlframe.rowconfigure(0, weight=0)
 		ctrlframe.columnconfigure(0, weight=0)
 		# Basemap controls and buttons
 		self.basemap_label = ttk.Label(ctrlframe, text="Basemap:", anchor="w")
 		self.basemap_label.grid(row=0, column=0, padx=(5, 5), pady=(2, 5), sticky=tk.W)
 		global initial_basemap
 		bm_name = initial_basemap
@@ -591,42 +608,36 @@
 			self.set_status()
 		# Set by global variable
 		self.multiselect_var = tk.StringVar(self.win, multiselect)
 		ck_multiselect = ttk.Checkbutton(ctrlframe, text="Multi-select", variable=self.multiselect_var, command=ck_changed)
 		ck_multiselect.grid(row=0, column=2, sticky=tk.W, padx=(0, 20))
 		# Map control buttons
 		zoomsel_btn = ttk.Button(ctrlframe, text="Zoom selected", image=zoom_sel_icon, compound=tk.LEFT, command=self.zoom_selected)
-		#zoomsel_btn = ttk.Button(ctrlframe, text="Zoom selected", command=self.zoom_selected)
 		zoomsel_btn.image = zoom_sel_icon
 		zoomsel_btn.grid(row=0, column=3, sticky=tk.W)
 		expand_btn = ttk.Button(ctrlframe, text="Zoom full", image=expand_icon, compound=tk.LEFT, command=self.zoom_full)
-		#expand_btn = ttk.Button(ctrlframe, text="Zoom full", command=self.zoom_full)
 		expand_btn.image = expand_icon
 		expand_btn.grid(row=0, column=4, sticky=tk.W)
 		focus_btn = ttk.Button(ctrlframe, text="Center", image=focus_icon, compound=tk.LEFT, command=self.focus_map)
-		#focus_btn = ttk.Button(ctrlframe, text="Center", command=self.focus_map)
 		focus_btn.image = focus_icon
 		focus_btn.grid(row=0, column=5, sticky=tk.W)
 		unselect_btn = ttk.Button(ctrlframe, text="Un-select", image=unselect_icon, compound=tk.LEFT, command=self.unselect_map)
-		#unselect_btn = ttk.Button(ctrlframe, text="Un-select", command=self.unselect_map)
 		unselect_btn.image = unselect_icon
 		unselect_btn.grid(row=0, column=6, sticky=tk.W)
 		# Map widget
 		mapframe.rowconfigure(0, weight=1)
 		mapframe.columnconfigure(0, weight=1)
 		self.map_widget = tkmv.TkinterMapView(mapframe, height=600, width=600, corner_radius=0)
 		if initial_basemap != "OpenMapServer":
 			tileserver = self.tile_url(initial_basemap)
 			self.map_widget.set_tile_server(tileserver)
 		self.map_widget.grid(row=0, column=0, sticky=tk.NSEW)
-		mapframe.grid(row=2, column=0, sticky=tk.NSEW)
 		# Populate the table frame
 		self.tblframe.rowconfigure(0, weight=1)
 		self.tblframe.columnconfigure(0, weight=1)
-		self.tblframe.grid(row=3, column=0, sticky=tk.NSEW)
 		self.tableframe, self.tbl = self.add_data(rows, headers, lat_col, lon_col, label_col,
 				symbol_col, color_col)
 		self.tableframe.grid(column=0, row=0, sticky=tk.NSEW)
 		self.set_tbl_selectmode()
 		self.set_status()
 		# Add menu
 		self.add_menu(table_object = self.tbl, column_headers=headers)
@@ -1015,15 +1026,14 @@
 			self.map_widget.update_idletasks()
 			#self.win.after(200, self.save_imageoutputfile)
 			self.save_imageoutputfile()
 		self.win.destroy()
 	def export_map_to_ps(self, outfile):
 		self.map_widget.canvas.postscript(file=outfile, colormode='color')
 	def save_imageoutputfile(self):
-		from PIL import ImageGrab
 		obj = self.map_widget.canvas
 		bounds = (obj.winfo_rootx(), obj.winfo_rooty(), 
 				obj.winfo_rootx() + obj.winfo_width(), obj.winfo_rooty() + obj.winfo_height())
 		ImageGrab.grab(bbox=bounds).save(self.imageoutputfile)
 	def export_map_to_img(self, outfile):
 		# Allow map to recover from blocking by the file dialog box before grabbing and exporting the canvas
 		self.map_widget.update_idletasks()
```

### Comparing `mapdata-1.7.0/mapdata.egg-info/PKG-INFO` & `mapdata-1.8.0/mapdata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 1.7.0
+Version: 1.8.0
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
@@ -20,14 +20,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Scientific/Engineering
 Requires: tkintermapview
 Requires: pyproj
+Requires: odfpy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
@@ -55,9 +56,15 @@
 The map can be exported to a Postscript, PNG, or JPEG file.  Using command-line options,
 *mapdata* can be directed to load a data file and display location markers and then to
 export the map to an image file, and quit.
 
 Selected rows in the data table can be exported to a CSV file.
 
 
+Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
+
+A configuration file template, application icons for Linux and Windows, a .desktop
+file for Linux, and additional bitmap symbols, are available for download from
+[OSDN](https://osdn.net/projects/mapdata/releases/).
+
```

### Comparing `mapdata-1.7.0/setup.py` & `mapdata-1.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='1.7.0',
+	version='1.8.0',
 	description="An interactive map and table explorer for geographic coordinates in a CSV file",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
-	requires=['tkintermapview', 'pyproj'],
+	requires=['tkintermapview', 'pyproj', 'odfpy'],
 	python_requires = '>=3.8',
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Environment :: Console',
 		'Environment :: X11 Applications',
 		'Environment :: Win32 (MS Windows)',
 		'Intended Audience :: End Users/Desktop',
```

