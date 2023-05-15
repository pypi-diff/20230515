# Comparing `tmp/opendatacrawler-1.0.8.tar.gz` & `tmp/opendatacrawler-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendatacrawler-1.0.8.tar", last modified: Thu Apr 20 15:31:34 2023, max compression
+gzip compressed data, was "opendatacrawler-1.0.9.tar", last modified: Thu Apr 20 15:35:15 2023, max compression
```

## Comparing `opendatacrawler-1.0.8.tar` & `opendatacrawler-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:31:34.167551 opendatacrawler-1.0.8/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1070 2023-02-03 16:41:45.000000 opendatacrawler-1.0.8/LICENSE
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:31:34.166943 opendatacrawler-1.0.8/PKG-INFO
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7205 2023-03-08 15:49:21.000000 opendatacrawler-1.0.8/README.md
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:31:34.144004 opendatacrawler-1.0.8/opendatacrawler/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4613 2023-04-20 15:15:12.000000 opendatacrawler-1.0.8/opendatacrawler/CkanCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3928 2023-04-20 15:19:24.000000 opendatacrawler-1.0.8/opendatacrawler/INECrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4644 2023-04-20 15:19:53.000000 opendatacrawler-1.0.8/opendatacrawler/OpenDataSoftCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1935 2023-04-20 15:14:34.000000 opendatacrawler-1.0.8/opendatacrawler/SocrataCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3164 2023-04-20 15:20:49.000000 opendatacrawler-1.0.8/opendatacrawler/ZenodoCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       95 2023-04-20 15:17:05.000000 opendatacrawler-1.0.8/opendatacrawler/__init__.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9194 2023-04-20 15:13:21.000000 opendatacrawler-1.0.8/opendatacrawler/__main__.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     6214 2023-04-20 15:18:49.000000 opendatacrawler-1.0.8/opendatacrawler/datosgobescrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3101 2023-04-20 15:18:33.000000 opendatacrawler-1.0.8/opendatacrawler/eurostatcrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      818 2023-02-03 16:41:45.000000 opendatacrawler-1.0.8/opendatacrawler/intro.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9669 2023-04-20 15:16:58.000000 opendatacrawler-1.0.8/opendatacrawler/odcrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1938 2023-03-16 09:49:44.000000 opendatacrawler-1.0.8/opendatacrawler/opendatacrawlerInterface.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      881 2023-02-03 16:41:45.000000 opendatacrawler-1.0.8/opendatacrawler/setup_logger.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     5119 2023-04-20 15:11:35.000000 opendatacrawler-1.0.8/opendatacrawler/utils.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     2480 2023-04-20 15:14:50.000000 opendatacrawler-1.0.8/opendatacrawler/worldbankcrawler.py
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:31:34.165810 opendatacrawler-1.0.8/opendatacrawler.egg-info/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/PKG-INFO
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      749 2023-04-20 15:31:34.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/SOURCES.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)        1 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/dependency_links.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       58 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/entry_points.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       12 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/requires.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       16 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/top_level.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       38 2023-04-20 15:31:34.167631 opendatacrawler-1.0.8/setup.cfg
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1041 2023-04-20 15:31:30.000000 opendatacrawler-1.0.8/setup.py
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:35:15.484024 opendatacrawler-1.0.9/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1070 2023-02-03 16:41:45.000000 opendatacrawler-1.0.9/LICENSE
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:35:15.482231 opendatacrawler-1.0.9/PKG-INFO
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7205 2023-03-08 15:49:21.000000 opendatacrawler-1.0.9/README.md
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:35:15.467929 opendatacrawler-1.0.9/opendatacrawler/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4595 2023-04-20 15:34:24.000000 opendatacrawler-1.0.9/opendatacrawler/CkanCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3928 2023-04-20 15:19:24.000000 opendatacrawler-1.0.9/opendatacrawler/INECrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4644 2023-04-20 15:19:53.000000 opendatacrawler-1.0.9/opendatacrawler/OpenDataSoftCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1935 2023-04-20 15:14:34.000000 opendatacrawler-1.0.9/opendatacrawler/SocrataCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3164 2023-04-20 15:20:49.000000 opendatacrawler-1.0.9/opendatacrawler/ZenodoCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       95 2023-04-20 15:17:05.000000 opendatacrawler-1.0.9/opendatacrawler/__init__.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9194 2023-04-20 15:13:21.000000 opendatacrawler-1.0.9/opendatacrawler/__main__.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     6214 2023-04-20 15:18:49.000000 opendatacrawler-1.0.9/opendatacrawler/datosgobescrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3101 2023-04-20 15:18:33.000000 opendatacrawler-1.0.9/opendatacrawler/eurostatcrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      818 2023-02-03 16:41:45.000000 opendatacrawler-1.0.9/opendatacrawler/intro.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9645 2023-04-20 15:33:49.000000 opendatacrawler-1.0.9/opendatacrawler/odcrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1938 2023-03-16 09:49:44.000000 opendatacrawler-1.0.9/opendatacrawler/opendatacrawlerInterface.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      881 2023-02-03 16:41:45.000000 opendatacrawler-1.0.9/opendatacrawler/setup_logger.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     5119 2023-04-20 15:11:35.000000 opendatacrawler-1.0.9/opendatacrawler/utils.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     2474 2023-04-20 15:34:46.000000 opendatacrawler-1.0.9/opendatacrawler/worldbankcrawler.py
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:35:15.481210 opendatacrawler-1.0.9/opendatacrawler.egg-info/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:35:15.000000 opendatacrawler-1.0.9/opendatacrawler.egg-info/PKG-INFO
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      749 2023-04-20 15:35:15.000000 opendatacrawler-1.0.9/opendatacrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)        1 2023-04-20 15:35:15.000000 opendatacrawler-1.0.9/opendatacrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       58 2023-04-20 15:35:15.000000 opendatacrawler-1.0.9/opendatacrawler.egg-info/entry_points.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       12 2023-04-20 15:35:15.000000 opendatacrawler-1.0.9/opendatacrawler.egg-info/requires.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       16 2023-04-20 15:35:15.000000 opendatacrawler-1.0.9/opendatacrawler.egg-info/top_level.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       38 2023-04-20 15:35:15.484156 opendatacrawler-1.0.9/setup.cfg
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1041 2023-04-20 15:35:08.000000 opendatacrawler-1.0.9/setup.py
```

### Comparing `opendatacrawler-1.0.8/LICENSE` & `opendatacrawler-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/PKG-INFO` & `opendatacrawler-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatacrawler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Crawler for open data portals
 Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor
 Author-email: alberto.berenguer@ua.es
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.8 Summary: Crawler for
+Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.9 Summary: Crawler for
 open data portals Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor Author-email: alberto.berenguer@ua.es License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
```

### Comparing `opendatacrawler-1.0.8/README.md` & `opendatacrawler-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/CkanCrawler.py` & `opendatacrawler-1.0.9/opendatacrawler/CkanCrawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,23 +67,23 @@
 
             if response.status_code == 200:
                 meta = response.json()['result']
 
                 metadata = dict()
 
                 metadata['id_portal'] = id
-                metadata['id_custom'] = utils.get_id_custom(metadata['id_portal']+self.domain)
+                metadata['id_custom'] = get_id_custom(metadata['id_portal']+self.domain)
                 metadata['title'] = meta.get('title', None)
                 metadata['img_portal'] = None
                 metadata['description'] = meta.get('notes', None)
                 metadata['language'] = meta.get('language', None)
                 metadata['theme'] = meta.get('category', None)
 
                 if metadata['theme'] is None:
-                    metadata['theme'] = utils.extract_tags(meta.get('tags', None))
+                    metadata['theme'] = extract_tags(meta.get('tags', None))
 
                 resource_list = []
                 for res in meta['resources']:
                     if (self.data_types is None or
                     res['format'].lower() in self.data_types):
                         resource = dict()
                         resource['name'] = res.get('name', None)
@@ -107,15 +107,15 @@
                         
                 metadata['temporal_coverage'] = [coverage]
                 metadata['spatial_coverage'] = None
                 
                 metadata['file_name'] = str(metadata['id_custom']) + '-' + str(self.domain.split('.')[1]) + '-' + str(metadata['id_portal'])
                 
                 # Saving all meta in a json file
-                utils.save_all_metadata(metadata['file_name'], meta, self.path)
+                save_all_metadata(metadata['file_name'], meta, self.path)
 
                 return metadata
             else:
                 return None
 
         except Exception as e:
             logger.error(e)
```

### Comparing `opendatacrawler-1.0.8/opendatacrawler/INECrawler.py` & `opendatacrawler-1.0.9/opendatacrawler/INECrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/OpenDataSoftCrawler.py` & `opendatacrawler-1.0.9/opendatacrawler/OpenDataSoftCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/SocrataCrawler.py` & `opendatacrawler-1.0.9/opendatacrawler/SocrataCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/ZenodoCrawler.py` & `opendatacrawler-1.0.9/opendatacrawler/ZenodoCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/__main__.py` & `opendatacrawler-1.0.9/opendatacrawler/__main__.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/datosgobescrawler.py` & `opendatacrawler-1.0.9/opendatacrawler/datosgobescrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/eurostatcrawler.py` & `opendatacrawler-1.0.9/opendatacrawler/eurostatcrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/intro.txt` & `opendatacrawler-1.0.9/opendatacrawler/intro.txt`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/odcrawler.py` & `opendatacrawler-1.0.9/opendatacrawler/odcrawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         self.domain = domain
         self.dms = None
         self.dms_instance = None
         self.max_sec = sec
         if not path:
             directory = os.getcwd()
             path = directory+"/data/"
-            utils.create_folder(path)
-        self.save_path = path + utils.clean_url(self.domain)
-        self.resume_path = path + "resume_"+utils.clean_url(self.domain)+".txt"
+            create_folder(path)
+        self.save_path = path + clean_url(self.domain)
+        self.resume_path = path + "resume_"+clean_url(self.domain)+".txt"
 
         if data_types:
             self.data_types = [x.lower() for x in list(data_types)]
         else:
             self.data_types = None
 
         print("Detecting DMS")
@@ -65,15 +65,15 @@
 
                 response = requests.get(self.domain+v, verify=False)
                 # If the content-type not is a webpage(we want a json api response) and the result code is 200
                 if response.status_code == 200 and response.headers['Content-Type']!="text/html":
                     self.dms = k
                     logger.info("DMS detected %s", k)
 
-                    if not utils.create_folder(self.save_path):
+                    if not create_folder(self.save_path):
                         logger.info("Can't create folder" + self.save_path)
                         exit()
                     break
             except Exception as e:
                 logger.info(e)
 
         # Create an instance of the corresponding dms
```

### Comparing `opendatacrawler-1.0.8/opendatacrawler/opendatacrawlerInterface.py` & `opendatacrawler-1.0.9/opendatacrawler/opendatacrawlerInterface.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/setup_logger.py` & `opendatacrawler-1.0.9/opendatacrawler/setup_logger.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/utils.py` & `opendatacrawler-1.0.9/opendatacrawler/utils.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/opendatacrawler/worldbankcrawler.py` & `opendatacrawler-1.0.9/opendatacrawler/worldbankcrawler.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             meta = response.json()
 
             metadata = dict()
 
             metadata['identifier'] = id
             metadata['title'] = meta.get('identification', None).get('title',None)
             metadata['description'] = meta.get('identification', None).get('description',None)
-            metadata['theme'] = utils.extract_tags(meta.get('priority_tags', None))
+            metadata['theme'] = extract_tags(meta.get('priority_tags', None))
 
             resource_list = []
             for res in meta['Resources']:
                 if (self.data_types is None or
                    res['name'].lower() in self.data_types):
                     aux = dict()
                     aux['name'] = res.get('name', None)
```

### Comparing `opendatacrawler-1.0.8/opendatacrawler.egg-info/PKG-INFO` & `opendatacrawler-1.0.9/opendatacrawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatacrawler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Crawler for open data portals
 Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor
 Author-email: alberto.berenguer@ua.es
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.8 Summary: Crawler for
+Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.9 Summary: Crawler for
 open data portals Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor Author-email: alberto.berenguer@ua.es License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
```

### Comparing `opendatacrawler-1.0.8/opendatacrawler.egg-info/SOURCES.txt` & `opendatacrawler-1.0.9/opendatacrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.8/setup.py` & `opendatacrawler-1.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="opendatacrawler",
-    version="1.0.8",
+    version="1.0.9",
     description="Crawler for open data portals",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/aberenguerpas/OpenDataCrawler/",
     author="Alberto Berenguer Pastor",
     author_email="alberto.berenguer@ua.es",
     license="MIT",
```

