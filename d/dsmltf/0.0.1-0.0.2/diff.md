# Comparing `tmp/DSMLTF-0.0.1.tar.gz` & `tmp/dsmltf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DSMLTF-0.0.1.tar", last modified: Sun May 14 07:34:23 2023, max compression
+gzip compressed data, was "dist/dsmltf-0.0.2.tar", last modified: Mon May 15 19:33:18 2023, max compression
```

## Comparing `DSMLTF-0.0.1.tar` & `dsmltf-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/
--rw-r--r--   0 sergejzuev   (501) staff       (20)      695 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      177 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/SOURCES.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/dependency_links.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)       17 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/requires.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/top_level.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)      695 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      284 2023-05-14 06:17:21.000000 DSMLTF-0.0.1/README.md
--rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/setup.cfg
--rw-r--r--   0 sergejzuev   (501) staff       (20)      611 2023-05-14 07:34:11.000000 DSMLTF-0.0.1/setup.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-15 19:33:18.000000 dsmltf-0.0.2/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      695 2023-05-15 19:33:18.000000 dsmltf-0.0.2/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      284 2023-05-14 06:17:21.000000 dsmltf-0.0.2/README.md
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-15 19:33:18.000000 dsmltf-0.0.2/dsmltf/
+-rwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-14 06:09:45.000000 dsmltf-0.0.2/dsmltf/__init__.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    33332 2023-05-15 19:12:42.000000 dsmltf-0.0.2/dsmltf/main.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-15 19:33:18.000000 dsmltf-0.0.2/dsmltf.egg-info/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      695 2023-05-15 19:33:18.000000 dsmltf-0.0.2/dsmltf.egg-info/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      182 2023-05-15 19:33:18.000000 dsmltf-0.0.2/dsmltf.egg-info/SOURCES.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-15 19:33:18.000000 dsmltf-0.0.2/dsmltf.egg-info/dependency_links.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        7 2023-05-15 19:33:18.000000 dsmltf-0.0.2/dsmltf.egg-info/top_level.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-05-15 19:33:18.000000 dsmltf-0.0.2/setup.cfg
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      623 2023-05-15 19:31:25.000000 dsmltf-0.0.2/setup.py
```

### Comparing `DSMLTF-0.0.1/DSMLTF.egg-info/PKG-INFO` & `dsmltf-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: DSMLTF
-Version: 0.0.1
+Name: dsmltf
+Version: 0.0.2
 Summary: A set of functions to study Data Science
 Home-page: UNKNOWN
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 License: UNKNOWN
 Description: The dsmltf (Data Science and Machine Learning Training Functions) contains 
         a set of functions to be used for educational purposes during study the  
         Data Science course. Most of functions are described in the textbook 
         available from the author by request on email shoukhov@mail.ru.
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `DSMLTF-0.0.1/PKG-INFO` & `dsmltf-0.0.2/dsmltf.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: DSMLTF
-Version: 0.0.1
+Name: dsmltf
+Version: 0.0.2
 Summary: A set of functions to study Data Science
 Home-page: UNKNOWN
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 License: UNKNOWN
 Description: The dsmltf (Data Science and Machine Learning Training Functions) contains 
         a set of functions to be used for educational purposes during study the  
         Data Science course. Most of functions are described in the textbook 
         available from the author by request on email shoukhov@mail.ru.
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `DSMLTF-0.0.1/setup.py` & `dsmltf-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from setuptools import setup
+import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
-requirements = ["requests<=2.21.0"]
+#requirements = ["requests<=2.21.0"]
 
-setup(name="DSMLTF",
-	version="0.0.1",
+setuptools.setup(name="dsmltf",
+	version="0.0.2",
 	author="Sergei Zuev",
 	author_email="shoukhov@mail.ru",
 	description="A set of functions to study Data Science",
+	packages=setuptools.find_packages(),
 	long_description=long_description,
 	long_description_content_type="text/markdown",
-	install_requires=requirements,
 	classifiers=[
-		"Programming Language :: Python :: 3.8",
+		"Programming Language :: Python :: 3.7",
 		"Operating System :: OS Independent",
 	],
 	python_requires='>=3.6',
 )
 
-#packages=find_packages(),
-#"License :: OSI Approved :: GNU", (in classifiers)
+#"License :: OSI Approved :: GNU", (in classifiers)
+#install_requires=requirements,
```

