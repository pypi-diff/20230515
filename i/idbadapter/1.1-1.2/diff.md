# Comparing `tmp/idbadapter-1.1.tar.gz` & `tmp/idbadapter-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.1.tar", last modified: Fri May  5 13:34:12 2023, max compression
+gzip compressed data, was "idbadapter-1.2.tar", last modified: Mon May 15 10:45:54 2023, max compression
```

## Comparing `idbadapter-1.1.tar` & `idbadapter-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:34:12.482477 idbadapter-1.1/
--rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.1/LICENSE
--rw-rw-rw-   0        0        0      695 2023-05-05 13:34:12.482477 idbadapter-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 13:34:12.469478 idbadapter-1.1/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-02 13:48:21.000000 idbadapter-1.1/idbadapter/__init__.py
--rw-rw-rw-   0        0        0     5820 2023-05-05 13:07:31.000000 idbadapter-1.1/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:34:12.481480 idbadapter-1.1/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      695 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 13:34:12.484477 idbadapter-1.1/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-05-05 13:34:09.000000 idbadapter-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:45:54.086416 idbadapter-1.2/
+-rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.2/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-05-15 10:45:54.086416 idbadapter-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:45:54.074418 idbadapter-1.2/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.2/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0     6086 2023-05-15 10:36:39.000000 idbadapter-1.2/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:45:54.084416 idbadapter-1.2/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-05-15 10:45:53.000000 idbadapter-1.2/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-15 10:45:54.000000 idbadapter-1.2/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 10:45:53.000000 idbadapter-1.2/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-15 10:45:53.000000 idbadapter-1.2/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 10:45:53.000000 idbadapter-1.2/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 10:45:54.087416 idbadapter-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-05-15 10:44:01.000000 idbadapter-1.2/setup.py
```

### Comparing `idbadapter-1.1/LICENSE` & `idbadapter-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.1/PKG-INFO` & `idbadapter-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.1
+Version: 1.2
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.1/idbadapter/schedule_loader.py` & `idbadapter-1.2/idbadapter/schedule_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,48 +49,52 @@
     def from_names(self, works: list[str], resources: list[str] = [], ceil_limit: int = 1_000):
         """method for getting schedules by works names list
 
         Args:
             work_name_list (list[str]): lists of basic works names 
             ceil_limit (int, optional): limit of records in one dataframe. Defaults to 1_000.
         """
-        if len(works) == 0:
+        if len(works) == 0 and len(resources) == 0:
             raise Exception("Empty works list")
         self.ceil_limit = ceil_limit
         self.works_list = self._get_works_ids_by_names(works)
         self.resource_list = self._get_resource_ids_by_names(resources)
         
         self.objects = list({*self._get_objects_by_resource(), *self._get_objects_by_works()})
         
         return self
            
     def _get_works_ids_by_names(self, work_name_list):
         data = json.dumps(work_name_list)
         response = self.session.post(urllib.parse.urljoin(self.url, "work/get_basic_works_ids"), data=data)
-
+        if "detail" in response.json(): 
+            return []
         return response.json()
     
     def _get_resource_ids_by_names(self, resource_names_list):
+        if len(resource_names_list) == 0:
+            return []
         data = json.dumps(resource_names_list)
-        response = self.session.post(urllib.parse.urljoin(self.url, "resource/get_basic_resouce_ids"), data=data)
-        
+        response = self.session.post(urllib.parse.urljoin(self.url, "resource/get_basic_resource_ids"), data=data)
+        if "detail" in response.json():
+            return []
         return response.json()
     
     def _get_objects_by_resource(self):
         if len(self.resource_list) == 0:
             return []
         data = json.dumps(self.resource_list)
         response = self.session.post(urllib.parse.urljoin(self.url, "resource/schedule_ids"), data=data)
-
         return response.json()
     
     def _get_objects_by_works(self):
+        if len(self.works_list) == 0:
+            return []
         data = json.dumps(self.works_list)
         response = self.session.post(urllib.parse.urljoin(self.url, "work/schedule_ids"), data=data)
-
         return response.json()
    
     def __iter__(self):
         return SchedulesIterator(self.objects, self.session, self.url, self.ceil_limit)
 
 
 class SchedulesIterator:
```

### Comparing `idbadapter-1.1/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.2/idbadapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.1
+Version: 1.2
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.1/setup.py` & `idbadapter-1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 
 version = '1.1'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.1',
+      version='1.2',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

