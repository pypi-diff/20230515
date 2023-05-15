# Comparing `tmp/ecida-0.0.7.tar.gz` & `tmp/ecida-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecida-0.0.7.tar", last modified: Sun May 14 22:18:40 2023, max compression
+gzip compressed data, was "ecida-0.0.8.tar", last modified: Mon May 15 15:39:09 2023, max compression
```

## Comparing `ecida-0.0.7.tar` & `ecida-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-14 22:18:40.073035 ecida-0.0.7/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     6929 2023-05-14 22:17:10.000000 ecida-0.0.7/Ecida.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-14 22:18:40.073035 ecida-0.0.7/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-05-13 22:19:01.000000 ecida-0.0.7/README.md
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-14 22:18:40.073035 ecida-0.0.7/ecida.egg-info/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      185 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/SOURCES.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/dependency_links.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/requires.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/top_level.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-14 22:18:40.073035 ecida-0.0.7/setup.cfg
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-14 22:18:28.000000 ecida-0.0.7/setup.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     1048 2023-05-14 22:17:36.000000 ecida-0.0.7/test_Ecida.py
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-15 15:39:09.847196 ecida-0.0.8/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     6928 2023-05-15 15:38:20.000000 ecida-0.0.8/Ecida.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-15 15:39:09.843196 ecida-0.0.8/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-05-13 22:19:01.000000 ecida-0.0.8/README.md
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-15 15:39:09.843196 ecida-0.0.8/ecida.egg-info/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-15 15:39:09.000000 ecida-0.0.8/ecida.egg-info/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      185 2023-05-15 15:39:09.000000 ecida-0.0.8/ecida.egg-info/SOURCES.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-15 15:39:09.000000 ecida-0.0.8/ecida.egg-info/dependency_links.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-15 15:39:09.000000 ecida-0.0.8/ecida.egg-info/requires.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-15 15:39:09.000000 ecida-0.0.8/ecida.egg-info/top_level.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-15 15:39:09.847196 ecida-0.0.8/setup.cfg
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-15 15:38:55.000000 ecida-0.0.8/setup.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     1048 2023-05-14 22:17:36.000000 ecida-0.0.8/test_Ecida.py
```

### Comparing `ecida-0.0.7/Ecida.py` & `ecida-0.0.8/Ecida.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,18 +165,19 @@
             for key, value in self._outputs.items() :
                 if value == "directory":
                     continue
                 topicName = os.environ[self._topics_envVars[key]]
                 self._topics_names[key] = topicName
             
             self._initialized = True
-        else:
-            for output in self._outputs:
-                if output in self._directories:
-                    create_directory(self._directories[output]["localPath"])
+        
+        #ALWYAS
+        for output in self._outputs:
+            if output in self._directories:
+                create_directory(self._directories[output]["localPath"])
 
             
   
     def push(self, output_channel: str, message) -> bool:
         if self._deployed:
             if output_channel in self._outputs:
                 self._producer.send(self._topics_names[output_channel], value= str(message).encode("utf-8"))
```

### Comparing `ecida-0.0.7/PKG-INFO` & `ecida-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.7
+Version: 0.0.8
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.7/ecida.egg-info/PKG-INFO` & `ecida-0.0.8/ecida.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.7
+Version: 0.0.8
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.7/setup.py` & `ecida-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
    long_description = fh.read()
    
 setuptools.setup(
    name='ecida',
-   version='0.0.7',
+   version='0.0.8',
    author="Mostafa Hadadian",
    author_email="m.hadadian@rug.nl",
    description="The ECiDA-python to make things easier",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://gitlab.com/ecida",
    packages=["."] or setuptools.find_packages(),
```

### Comparing `ecida-0.0.7/test_Ecida.py` & `ecida-0.0.8/test_Ecida.py`

 * *Files identical despite different names*

