# Comparing `tmp/kmlb-0.0.93.tar.gz` & `tmp/kmlb-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmlb-0.0.93.tar", last modified: Fri May  5 03:52:41 2023, max compression
+gzip compressed data, was "kmlb-0.0.94.tar", last modified: Mon May 15 19:55:46 2023, max compression
```

## Comparing `kmlb-0.0.93.tar` & `kmlb-0.0.94.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 03:52:41.290742 kmlb-0.0.93/
--rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.93/LICENSE.md
--rw-rw-rw-   0        0        0    38527 2023-05-05 03:52:41.290742 kmlb-0.0.93/PKG-INFO
--rw-rw-rw-   0        0        0    38044 2023-04-25 14:31:02.000000 kmlb-0.0.93/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 03:52:41.270417 kmlb-0.0.93/kmlb/
--rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.93/kmlb/__init__.py
--rw-rw-rw-   0        0        0    43400 2023-05-05 03:51:08.000000 kmlb-0.0.93/kmlb/base.py
--rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.93/kmlb/gis_basics.py
--rw-rw-rw-   0        0        0     6922 2023-04-26 16:09:29.000000 kmlb-0.0.93/kmlb/shapes.py
-drwxrwxrwx   0        0        0        0 2023-05-05 03:52:41.289736 kmlb-0.0.93/kmlb.egg-info/
--rw-rw-rw-   0        0        0    38527 2023-05-05 03:52:41.000000 kmlb-0.0.93/kmlb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-05-05 03:52:41.000000 kmlb-0.0.93/kmlb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 03:52:41.000000 kmlb-0.0.93/kmlb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-05 03:52:41.000000 kmlb-0.0.93/kmlb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 03:52:41.290742 kmlb-0.0.93/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-05-05 03:51:36.000000 kmlb-0.0.93/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:55:46.477979 kmlb-0.0.94/
+-rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.94/LICENSE.md
+-rw-rw-rw-   0        0        0    38527 2023-05-15 19:55:46.477979 kmlb-0.0.94/PKG-INFO
+-rw-rw-rw-   0        0        0    38044 2023-04-25 14:31:02.000000 kmlb-0.0.94/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 19:55:46.447138 kmlb-0.0.94/kmlb/
+-rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.94/kmlb/__init__.py
+-rw-rw-rw-   0        0        0    43468 2023-05-15 19:54:30.000000 kmlb-0.0.94/kmlb/base.py
+-rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.94/kmlb/gis_basics.py
+-rw-rw-rw-   0        0        0     6922 2023-04-26 16:09:29.000000 kmlb-0.0.94/kmlb/shapes.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:55:46.475977 kmlb-0.0.94/kmlb.egg-info/
+-rw-rw-rw-   0        0        0    38527 2023-05-15 19:55:46.000000 kmlb-0.0.94/kmlb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-05-15 19:55:46.000000 kmlb-0.0.94/kmlb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 19:55:46.000000 kmlb-0.0.94/kmlb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-15 19:55:46.000000 kmlb-0.0.94/kmlb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 19:55:46.477979 kmlb-0.0.94/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-05-15 19:55:12.000000 kmlb-0.0.94/setup.py
```

### Comparing `kmlb-0.0.93/LICENSE.md` & `kmlb-0.0.94/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.93/PKG-INFO` & `kmlb-0.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.93
+Version: 0.0.94
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kmlb-0.0.93/README.md` & `kmlb-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.93/kmlb/base.py` & `kmlb-0.0.94/kmlb/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1053,18 +1053,18 @@
                The name of the Network Link element
            link_path (String):
                 Path to file
            description (String) [Optional]:
                 A small body of descriptive text for the NetworkLink element.
            refresh_interval (Int) [Optional]:
                 Number of seconds between file refreshes. (Default = None)
-            folder_type (Integer):
+           folder_type (Integer):
                 Can be any of the following values:
                 1 = check, 2 = radioFolder, 3 = checkOffOnly, 4 = checkHideChildren
-            hidden (Bool) [Optional]:
+           hidden (Bool) [Optional]:
                 A value of 'True' or 'False' where 'False' means the network link will be visible (Default = 'False').
            collapsed (Bool) [Optional]:
                 True = Root folder is collapsed.
                 False = Root folder is open/expanded.
             camera (Element) [Optional]:
                 A KML 'LookAt' element that defines the default camera angle to the kml.
 
@@ -1085,56 +1085,56 @@
 
        Returns
        -------
        network_link : element
 
        """
 
-    network_link = ET.Element("NetworkLink")
-    ET.SubElement(network_link, "name").text = str(name)
-    ET.SubElement(network_link, "description").text = str(description)
+    net_link = ET.Element("NetworkLink")
+    ET.SubElement(net_link, "name").text = str(name)
+    ET.SubElement(net_link, "description").text = str(description)
     collapsed = 0 if collapsed is True else 1
-    ET.SubElement(network_link, "open").text = str(collapsed)
+    ET.SubElement(net_link, "open").text = str(collapsed)
 
     # Set 'visibility' value
     visibility = 0
     if hidden is False:
         visibility = 1
 
-    ET.SubElement(network_link, 'visibility').text = str(visibility)
+    ET.SubElement(net_link, 'visibility').text = str(visibility)
 
-    style = ET.SubElement(network_link, "Style")
+    style = ET.SubElement(net_link, "Style")
     list_style = ET.SubElement(style, "ListStyle")
     if folder_type == 1:
         folder_type = 'check'
     elif folder_type == 2:
         folder_type = 'radioFolder'
     elif folder_type == 3:
         folder_type = 'checkOffOnly'
     elif folder_type == 4:
         folder_type = 'checkHideChildren'
     else:
         folder_type = 'check'
 
     ET.SubElement(list_style, "listItemType").text = folder_type
 
-    link = ET.SubElement(network_link, "Link")
+    link = ET.SubElement(net_link, "Link")
     ET.SubElement(link, "href").text = link_path
 
     if refresh_interval is not None:
         ET.SubElement(link, "refreshMode").text = 'onInterval'
         ET.SubElement(link, "refreshInterval").text = str(refresh_interval)
     else:
         pass
 
     # Network Link Camera Angle
     if camera is not None:
-        network_link.append(camera)
+        net_link.append(camera)
 
-    return network_link
+    return net_link
 
 
 def ground_overlay(name, img_path, bounds, description='', opacity=100, refresh_interval=None, altitude=0, altitude_mode='CTG', hidden=False, camera=None):
     """
     INPUTS:
     name (String):
         The name to be given to the overlay.
@@ -1218,15 +1218,16 @@
        OVERVIEW:
            Creates a KMZ file that can contain KMLs and files such as images.
 
        INPUTS:
             kmz_name (String):
                 The name of the KMZ
             kmls (Tuples):
-                 (Layer Name, KML as XML str, folder_type)
+                 (Layer Name, KML as XML str, folder_type, hidden)
+                 hidden: 1 = True, 0 = false
             path (String) [Optional]:
                 The path where the kmz file will be written to. The KMz's file name is defined within the path.
                 Necessary folders will be created if they do not exist.
                 Note: The file path should end '.kmz'
             files_as_bytes (Tuple) [Optional]:
                  (desitnation path of file within KMZ root, data as bytes)
             kwargs
@@ -1254,17 +1255,18 @@
     kmz_buffer = io.BytesIO()
 
     with zipfile.ZipFile(kmz_buffer, 'w') as zf:
         for count, doc in enumerate(kmls):
             name = doc[0]
             data = doc[1].encode()
             folder_type = doc[2]
+            visibility = doc[3]
             doc_path = f"kmls/doc_{count}.kml"
             zf.writestr(doc_path, data)
-            nl = network_link(name, doc_path, folder_type=folder_type)
+            nl = network_link(name, doc_path, folder_type=folder_type, hidden=visibility)
             network_link_elements.append(nl)
 
         if files_as_bytes is not None:
             for fb in files_as_bytes:
                 file_path = fb[0]
                 data = fb[1]
                 zf.writestr(file_path, data)
```

### Comparing `kmlb-0.0.93/kmlb/gis_basics.py` & `kmlb-0.0.94/kmlb/gis_basics.py`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.93/kmlb/shapes.py` & `kmlb-0.0.94/kmlb/shapes.py`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.93/kmlb.egg-info/PKG-INFO` & `kmlb-0.0.94/kmlb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.93
+Version: 0.0.94
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kmlb-0.0.93/setup.py` & `kmlb-0.0.94/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kmlb",
-    version="0.0.93",
+    version="0.0.94",
     author="HFM3",
     description="A Straightforward Google Earth KML Builder",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HFM3/kmlb",
     packages=setuptools.find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "images", "art"]),
     classifiers=[
```

