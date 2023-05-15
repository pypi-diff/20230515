# Comparing `tmp/ecida-0.0.6.tar.gz` & `tmp/ecida-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecida-0.0.6.tar", last modified: Sun May 14 11:03:53 2023, max compression
+gzip compressed data, was "ecida-0.0.7.tar", last modified: Sun May 14 22:18:40 2023, max compression
```

## Comparing `ecida-0.0.6.tar` & `ecida-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-14 11:03:53.169649 ecida-0.0.6/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     6169 2023-05-14 10:58:13.000000 ecida-0.0.6/Ecida.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-14 11:03:53.169649 ecida-0.0.6/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-05-13 22:19:01.000000 ecida-0.0.6/README.md
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-14 11:03:53.169649 ecida-0.0.6/ecida.egg-info/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      171 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/SOURCES.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/dependency_links.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/requires.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/top_level.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-14 11:03:53.169649 ecida-0.0.6/setup.cfg
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-14 10:58:49.000000 ecida-0.0.6/setup.py
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-14 22:18:40.073035 ecida-0.0.7/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     6929 2023-05-14 22:17:10.000000 ecida-0.0.7/Ecida.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-14 22:18:40.073035 ecida-0.0.7/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-05-13 22:19:01.000000 ecida-0.0.7/README.md
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-14 22:18:40.073035 ecida-0.0.7/ecida.egg-info/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      185 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/SOURCES.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/dependency_links.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/requires.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-14 22:18:40.000000 ecida-0.0.7/ecida.egg-info/top_level.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-14 22:18:40.073035 ecida-0.0.7/setup.cfg
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-14 22:18:28.000000 ecida-0.0.7/setup.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     1048 2023-05-14 22:17:36.000000 ecida-0.0.7/test_Ecida.py
```

### Comparing `ecida-0.0.6/Ecida.py` & `ecida-0.0.7/Ecida.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,33 @@
     flag_value = os.getenv("ECIDA_DEPLOY", "").lower()
     return flag_value == "true"
 
 def now():
     return "[" + datetime.now().strftime("%Y-%m-%d %H:%M:%S") + "]"
 
 
+def convert_to_dns_name(string):
+    # Convert the string to lowercase
+    string = string.lower()
+    
+    # Replace non-alphanumeric characters with hyphens
+    string = ''.join('-' if not c.isalnum() else c for c in string)
+    
+    # Remove leading and trailing hyphens
+    string = string.strip('-')
+    
+    # Replace multiple consecutive hyphens with a single hyphen
+    string = '-'.join(filter(None, string.split('-')))
+    
+    # Ensure the resulting string is not empty
+    if not string:
+        raise ValueError("Invalid string: Cannot convert to DNS name.")
+    
+    return string
+
 def create_directory(directory_path):
     if os.path.exists(directory_path):
         print(f"Deleting existing directory: {directory_path}")
         shutil.rmtree(directory_path)
 
     try:
         print(f"Creating directory: {directory_path}")
@@ -78,36 +97,38 @@
         self._topics_envVars[inp] = "KAFKA_TOPIC_"+ inp.upper()
         
     def add_output(self, out: str, type):
         self._outputs[out] = type
         self._topics_envVars[out] = "KAFKA_TOPIC_"+ out.upper()
         
     def add_input_directory(self, inp: str):
+        localPath = convert_to_dns_name(inp)
         self._inputs[inp] = "directory"
         self.directories[inp] = {}
-        self.directories[inp]["localPath"] = inp
+        self.directories[inp]["localPath"] = localPath
         
     def add_output_directory(self, out: str):
+        localPath = convert_to_dns_name(out)
         self._outputs[out] = "directory"
         self.directories[out] = {}
-        self.directories[out]["localPath"] = out
+        self.directories[out]["localPath"] = localPath
         
     def add_input_from_git(self, name: str, git: str, path: str):
         self.add_input_directory(name)
         self.__add_git_to_directory(name, git,path)
     
     def add_output_to_git(self, name: str, git: str, path: str):
         self.add_output_directory(name)
         self.__add_git_to_directory(name, git,path)
         
     def get_path(self, name):
         if self._deployed:
-            return "/"+name
+            return "/"+self.directories[name]["localPath"]
         else:
-            return "./"+name
+            return "./"+self.directories[name]["localPath"]
     
     def __add_git_to_directory(self, name: str, git: str, path: str):
         self._directories[name]["source"] = git
         self._directories[name]["folder"] = path
     
     def to_yaml(self) -> str:
         return str(self._inputs) + "\n" + str(self._outputs)
```

### Comparing `ecida-0.0.6/PKG-INFO` & `ecida-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.6
+Version: 0.0.7
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.6/ecida.egg-info/PKG-INFO` & `ecida-0.0.7/ecida.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.6
+Version: 0.0.7
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.6/setup.py` & `ecida-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
    long_description = fh.read()
    
 setuptools.setup(
    name='ecida',
-   version='0.0.6',
+   version='0.0.7',
    author="Mostafa Hadadian",
    author_email="m.hadadian@rug.nl",
    description="The ECiDA-python to make things easier",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://gitlab.com/ecida",
    packages=["."] or setuptools.find_packages(),
```

