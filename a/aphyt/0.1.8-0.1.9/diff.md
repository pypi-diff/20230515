# Comparing `tmp/aphyt-0.1.8.tar.gz` & `tmp/aphyt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aphyt-0.1.8.tar", last modified: Fri Feb  3 21:43:48 2023, max compression
+gzip compressed data, was "dist\aphyt-0.1.9.tar", last modified: Tue Mar  7 17:45:52 2023, max compression
```

## Comparing `aphyt-0.1.8.tar` & `aphyt-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 21:43:48.561628 aphyt-0.1.8/
--rw-rw-rw-   0        0        0    12309 2023-02-03 21:43:48.558717 aphyt-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    10291 2023-02-03 21:26:12.000000 aphyt-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-03 21:43:48.380181 aphyt-0.1.8/aphyt/
--rw-rw-rw-   0        0        0      111 2021-11-01 13:36:11.000000 aphyt-0.1.8/aphyt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-03 21:43:48.444590 aphyt-0.1.8/aphyt/cip/
--rw-rw-rw-   0        0        0      223 2022-04-12 18:05:35.000000 aphyt-0.1.8/aphyt/cip/__init__.py
--rw-rw-rw-   0        0        0     9363 2022-04-12 18:05:35.000000 aphyt-0.1.8/aphyt/cip/cip.py
--rw-rw-rw-   0        0        0     1023 2022-04-12 18:05:35.000000 aphyt-0.1.8/aphyt/cip/cip_attributes.py
--rw-rw-rw-   0        0        0    28413 2023-02-03 21:26:12.000000 aphyt-0.1.8/aphyt/cip/cip_datatypes.py
--rw-rw-rw-   0        0        0     4520 2022-04-12 18:05:35.000000 aphyt-0.1.8/aphyt/cip/cip_services.py
-drwxrwxrwx   0        0        0        0 2023-02-03 21:43:48.462899 aphyt-0.1.8/aphyt/eip/
--rw-rw-rw-   0        0        0      175 2022-04-12 18:05:35.000000 aphyt-0.1.8/aphyt/eip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-03 21:43:48.478511 aphyt-0.1.8/aphyt/eip/cip_objects/
--rw-rw-rw-   0        0        0      111 2022-04-12 18:05:35.000000 aphyt-0.1.8/aphyt/eip/cip_objects/__init__.py
--rw-rw-rw-   0        0        0     3698 2022-04-12 18:05:35.000000 aphyt-0.1.8/aphyt/eip/cip_objects/tcp_interface.py
--rw-rw-rw-   0        0        0    13592 2023-02-03 21:26:12.000000 aphyt-0.1.8/aphyt/eip/eip.py
-drwxrwxrwx   0        0        0        0 2023-02-03 21:43:48.506826 aphyt-0.1.8/aphyt/omron/
--rw-rw-rw-   0        0        0      170 2021-11-01 13:36:11.000000 aphyt-0.1.8/aphyt/omron/__init__.py
--rw-rw-rw-   0        0        0    10495 2022-04-12 18:05:35.000000 aphyt-0.1.8/aphyt/omron/k6pm_th.py
--rw-rw-rw-   0        0        0    39159 2023-02-03 21:26:12.000000 aphyt-0.1.8/aphyt/omron/n_series.py
--rw-rw-rw-   0        0        0     2831 2021-11-01 13:36:12.000000 aphyt-0.1.8/aphyt/omron/omron_datatypes.py
-drwxrwxrwx   0        0        0        0 2023-02-03 21:43:48.551770 aphyt-0.1.8/aphyt/tkmi/
--rw-rw-rw-   0        0        0      111 2021-11-01 13:36:12.000000 aphyt-0.1.8/aphyt/tkmi/__init__.py
--rw-rw-rw-   0        0        0     2755 2021-11-01 13:36:12.000000 aphyt-0.1.8/aphyt/tkmi/helper.py
--rw-rw-rw-   0        0        0    10271 2023-02-03 21:26:12.000000 aphyt-0.1.8/aphyt/tkmi/tkmi_main.py
--rw-rw-rw-   0        0        0    23244 2023-02-03 21:26:12.000000 aphyt-0.1.8/aphyt/tkmi/widgets.py
-drwxrwxrwx   0        0        0        0 2023-02-03 21:43:48.410170 aphyt-0.1.8/aphyt.egg-info/
--rw-rw-rw-   0        0        0    12309 2023-02-03 21:43:47.000000 aphyt-0.1.8/aphyt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-02-03 21:43:47.000000 aphyt-0.1.8/aphyt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 21:43:47.000000 aphyt-0.1.8/aphyt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-02-03 21:43:47.000000 aphyt-0.1.8/aphyt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-03 21:43:48.562618 aphyt-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      799 2023-02-03 21:26:12.000000 aphyt-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-07 17:45:52.682972 aphyt-0.1.9/
+-rw-rw-rw-   0        0        0    12309 2023-03-07 17:45:52.681019 aphyt-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10291 2023-02-03 21:26:12.000000 aphyt-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-07 17:45:52.601919 aphyt-0.1.9/aphyt/
+-rw-rw-rw-   0        0        0      111 2021-11-01 13:36:11.000000 aphyt-0.1.9/aphyt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 17:45:52.632198 aphyt-0.1.9/aphyt/cip/
+-rw-rw-rw-   0        0        0      223 2022-04-12 18:05:35.000000 aphyt-0.1.9/aphyt/cip/__init__.py
+-rw-rw-rw-   0        0        0     9363 2022-04-12 18:05:35.000000 aphyt-0.1.9/aphyt/cip/cip.py
+-rw-rw-rw-   0        0        0     1023 2022-04-12 18:05:35.000000 aphyt-0.1.9/aphyt/cip/cip_attributes.py
+-rw-rw-rw-   0        0        0    28413 2023-02-03 21:26:12.000000 aphyt-0.1.9/aphyt/cip/cip_datatypes.py
+-rw-rw-rw-   0        0        0     4520 2022-04-12 18:05:35.000000 aphyt-0.1.9/aphyt/cip/cip_services.py
+drwxrwxrwx   0        0        0        0 2023-03-07 17:45:52.639028 aphyt-0.1.9/aphyt/eip/
+-rw-rw-rw-   0        0        0      175 2022-04-12 18:05:35.000000 aphyt-0.1.9/aphyt/eip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 17:45:52.644882 aphyt-0.1.9/aphyt/eip/cip_objects/
+-rw-rw-rw-   0        0        0      111 2022-04-12 18:05:35.000000 aphyt-0.1.9/aphyt/eip/cip_objects/__init__.py
+-rw-rw-rw-   0        0        0     3698 2022-04-12 18:05:35.000000 aphyt-0.1.9/aphyt/eip/cip_objects/tcp_interface.py
+-rw-rw-rw-   0        0        0    13592 2023-02-03 21:26:12.000000 aphyt-0.1.9/aphyt/eip/eip.py
+drwxrwxrwx   0        0        0        0 2023-03-07 17:45:52.656610 aphyt-0.1.9/aphyt/omron/
+-rw-rw-rw-   0        0        0      170 2021-11-01 13:36:11.000000 aphyt-0.1.9/aphyt/omron/__init__.py
+-rw-rw-rw-   0        0        0    10495 2022-04-12 18:05:35.000000 aphyt-0.1.9/aphyt/omron/k6pm_th.py
+-rw-rw-rw-   0        0        0    39159 2023-02-03 21:26:12.000000 aphyt-0.1.9/aphyt/omron/n_series.py
+-rw-rw-rw-   0        0        0     2831 2021-11-01 13:36:12.000000 aphyt-0.1.9/aphyt/omron/omron_datatypes.py
+drwxrwxrwx   0        0        0        0 2023-03-07 17:45:52.676133 aphyt-0.1.9/aphyt/tkmi/
+-rw-rw-rw-   0        0        0      546 2023-02-03 21:26:12.000000 aphyt-0.1.9/aphyt/tkmi/Transparent_Pixel.png
+-rw-rw-rw-   0        0        0      111 2021-11-01 13:36:12.000000 aphyt-0.1.9/aphyt/tkmi/__init__.py
+-rw-rw-rw-   0        0        0     2755 2021-11-01 13:36:12.000000 aphyt-0.1.9/aphyt/tkmi/helper.py
+-rw-rw-rw-   0        0        0    10271 2023-02-03 21:26:12.000000 aphyt-0.1.9/aphyt/tkmi/tkmi_main.py
+-rw-rw-rw-   0        0        0     4286 2023-03-07 00:39:42.000000 aphyt-0.1.9/aphyt/tkmi/transparent_icon.ico
+-rw-rw-rw-   0        0        0    23327 2023-03-07 00:39:42.000000 aphyt-0.1.9/aphyt/tkmi/widgets.py
+drwxrwxrwx   0        0        0        0 2023-03-07 17:45:52.614619 aphyt-0.1.9/aphyt.egg-info/
+-rw-rw-rw-   0        0        0    12309 2023-03-07 17:45:52.000000 aphyt-0.1.9/aphyt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-03-07 17:45:52.000000 aphyt-0.1.9/aphyt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-07 17:45:52.000000 aphyt-0.1.9/aphyt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-03-07 17:45:52.000000 aphyt-0.1.9/aphyt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-07 17:45:52.682972 aphyt-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-03-07 17:43:25.000000 aphyt-0.1.9/setup.py
```

### Comparing `aphyt-0.1.8/PKG-INFO` & `aphyt-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aphyt
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library to communicate with Omron NX and NJ PLC and motion controllers
 Home-page: https://bitbucket.org/jryan/aphytcomm/src/master/
 Author: Joseph Ryan
 Author-email: jr@aphyt.com
 License: UNKNOWN
 Description: # aphyt
         This is a library for communicating with industrial devices using Python.
```

### Comparing `aphyt-0.1.8/README.md` & `aphyt-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/cip/cip.py` & `aphyt-0.1.9/aphyt/cip/cip.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/cip/cip_attributes.py` & `aphyt-0.1.9/aphyt/cip/cip_attributes.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/cip/cip_datatypes.py` & `aphyt-0.1.9/aphyt/cip/cip_datatypes.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/cip/cip_services.py` & `aphyt-0.1.9/aphyt/cip/cip_services.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/eip/cip_objects/tcp_interface.py` & `aphyt-0.1.9/aphyt/eip/cip_objects/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/eip/eip.py` & `aphyt-0.1.9/aphyt/eip/eip.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/omron/k6pm_th.py` & `aphyt-0.1.9/aphyt/omron/k6pm_th.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/omron/n_series.py` & `aphyt-0.1.9/aphyt/omron/n_series.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/omron/omron_datatypes.py` & `aphyt-0.1.9/aphyt/omron/omron_datatypes.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/tkmi/helper.py` & `aphyt-0.1.9/aphyt/tkmi/helper.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/tkmi/tkmi_main.py` & `aphyt-0.1.9/aphyt/tkmi/tkmi_main.py`

 * *Files identical despite different names*

### Comparing `aphyt-0.1.8/aphyt/tkmi/widgets.py` & `aphyt-0.1.9/aphyt/tkmi/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,17 @@
                  background=None,
                  screen_change_variable=None,
                  **kwargs):
         super().__init__(**kwargs)
         self.initial_page = initial_page
         self.pages = {}
         self.withdraw()
-        self.iconbitmap('transparent_icon.ico')
+        path = os.path.dirname(__file__)
+        path = os.path.join(path, 'transparent_icon.ico')
+        self.iconbitmap(path)
         self.title(window_title)
         self.screen_change_variable = screen_change_variable
         if geometry is not None:
             self.geometry(geometry)
         if background is not None:
             self.config(background=background)
         self.rowconfigure(0, weight=1)
```

### Comparing `aphyt-0.1.8/aphyt.egg-info/PKG-INFO` & `aphyt-0.1.9/aphyt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aphyt
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library to communicate with Omron NX and NJ PLC and motion controllers
 Home-page: https://bitbucket.org/jryan/aphytcomm/src/master/
 Author: Joseph Ryan
 Author-email: jr@aphyt.com
 License: UNKNOWN
 Description: # aphyt
         This is a library for communicating with industrial devices using Python.
```

