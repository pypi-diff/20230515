# Comparing `tmp/TACTUS-data-1.1.1.tar.gz` & `tmp/TACTUS-data-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TACTUS-data-1.1.1.tar", last modified: Mon May 15 14:30:38 2023, max compression
+gzip compressed data, was "TACTUS-data-1.1.2.tar", last modified: Mon May 15 20:30:54 2023, max compression
```

## Comparing `TACTUS-data-1.1.1.tar` & `TACTUS-data-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 14:30:38.858780 TACTUS-data-1.1.1/
--rw-rw-rw-   0        0        0     4033 2023-05-15 14:30:38.858780 TACTUS-data-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3619 2023-05-15 14:23:02.000000 TACTUS-data-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 14:30:38.640046 TACTUS-data-1.1.1/TACTUS_data.egg-info/
--rw-rw-rw-   0        0        0     4033 2023-05-15 14:30:38.000000 TACTUS-data-1.1.1/TACTUS_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-05-15 14:30:38.000000 TACTUS-data-1.1.1/TACTUS_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 14:30:38.000000 TACTUS-data-1.1.1/TACTUS_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-05-15 14:30:38.000000 TACTUS-data-1.1.1/TACTUS_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-05-15 14:30:38.000000 TACTUS-data-1.1.1/TACTUS_data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      734 2023-05-15 14:29:58.000000 TACTUS-data-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 14:30:38.862494 TACTUS-data-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 14:30:38.653206 TACTUS-data-1.1.1/tactus_data/
--rw-rw-rw-   0        0        0      449 2023-05-15 13:01:27.000000 TACTUS-data-1.1.1/tactus_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:30:38.677245 TACTUS-data-1.1.1/tactus_data/datasets/
--rw-rw-rw-   0        0        0        0 2023-05-14 12:26:44.000000 TACTUS-data-1.1.1/tactus_data/datasets/__init__.py
--rw-rw-rw-   0        0        0     5192 2023-05-07 12:54:31.000000 TACTUS-data-1.1.1/tactus_data/datasets/dataset.py
--rw-rw-rw-   0        0        0     4654 2023-04-23 13:21:41.000000 TACTUS-data-1.1.1/tactus_data/datasets/ut_interaction.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:30:38.825900 TACTUS-data-1.1.1/tactus_data/utils/
--rw-rw-rw-   0        0        0        0 2023-03-14 09:55:08.000000 TACTUS-data-1.1.1/tactus_data/utils/__init__.py
--rw-rw-rw-   0        0        0     9207 2023-04-22 06:51:13.000000 TACTUS-data-1.1.1/tactus_data/utils/data_augment.py
--rw-rw-rw-   0        0        0     2269 2023-05-13 16:34:39.000000 TACTUS-data-1.1.1/tactus_data/utils/retracker.py
--rw-rw-rw-   0        0        0    15447 2023-05-13 13:44:06.000000 TACTUS-data-1.1.1/tactus_data/utils/skeleton.py
--rw-rw-rw-   0        0        0     4408 2023-05-14 14:13:25.000000 TACTUS-data-1.1.1/tactus_data/utils/skeletonrollingwindow.py
--rw-rw-rw-   0        0        0     9338 2023-05-13 16:39:06.000000 TACTUS-data-1.1.1/tactus_data/utils/thread_videocapture.py
--rw-rw-rw-   0        0        0     4092 2023-05-14 14:45:35.000000 TACTUS-data-1.1.1/tactus_data/utils/visualisation.py
--rw-rw-rw-   0        0        0     1399 2023-05-13 16:45:52.000000 TACTUS-data-1.1.1/tactus_data/utils/yolov7.py
--rw-rw-rw-   0        0        0    11761 2023-05-13 16:44:58.000000 TACTUS-data-1.1.1/tactus_data/utils/yolov8.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:30:38.850495 TACTUS-data-1.1.1/test/
--rw-rw-rw-   0        0        0     2654 2023-05-03 09:05:29.000000 TACTUS-data-1.1.1/test/test_skeletonization.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:30:54.585423 TACTUS-data-1.1.2/
+-rw-rw-rw-   0        0        0     4033 2023-05-15 20:30:54.584422 TACTUS-data-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3619 2023-05-15 16:10:43.000000 TACTUS-data-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 20:30:54.421848 TACTUS-data-1.1.2/TACTUS_data.egg-info/
+-rw-rw-rw-   0        0        0     4033 2023-05-15 20:30:54.000000 TACTUS-data-1.1.2/TACTUS_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-05-15 20:30:54.000000 TACTUS-data-1.1.2/TACTUS_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 20:30:54.000000 TACTUS-data-1.1.2/TACTUS_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-05-15 20:30:54.000000 TACTUS-data-1.1.2/TACTUS_data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-05-15 20:30:54.000000 TACTUS-data-1.1.2/TACTUS_data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      756 2023-05-15 20:29:50.000000 TACTUS-data-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 20:30:54.586410 TACTUS-data-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 20:30:54.430863 TACTUS-data-1.1.2/tactus_data/
+-rw-rw-rw-   0        0        0      449 2023-05-15 16:10:43.000000 TACTUS-data-1.1.2/tactus_data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:30:54.471377 TACTUS-data-1.1.2/tactus_data/datasets/
+-rw-rw-rw-   0        0        0        0 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/datasets/__init__.py
+-rw-rw-rw-   0        0        0     5192 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/datasets/dataset.py
+-rw-rw-rw-   0        0        0     4654 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/datasets/ut_interaction.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:30:54.570398 TACTUS-data-1.1.2/tactus_data/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-14 09:55:08.000000 TACTUS-data-1.1.2/tactus_data/utils/__init__.py
+-rw-rw-rw-   0        0        0     9207 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/utils/data_augment.py
+-rw-rw-rw-   0        0        0     2269 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/utils/retracker.py
+-rw-rw-rw-   0        0        0    15447 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/utils/skeleton.py
+-rw-rw-rw-   0        0        0     4408 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/utils/skeletonrollingwindow.py
+-rw-rw-rw-   0        0        0     9338 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/utils/thread_videocapture.py
+-rw-rw-rw-   0        0        0     4092 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/utils/visualisation.py
+-rw-rw-rw-   0        0        0     1399 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/utils/yolov7.py
+-rw-rw-rw-   0        0        0    11761 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/tactus_data/utils/yolov8.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:30:54.579410 TACTUS-data-1.1.2/test/
+-rw-rw-rw-   0        0        0     2654 2023-05-15 16:10:39.000000 TACTUS-data-1.1.2/test/test_skeletonization.py
```

### Comparing `TACTUS-data-1.1.1/PKG-INFO` & `TACTUS-data-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TACTUS-data
-Version: 1.1.1
+Version: 1.1.2
 Summary: Threatening activities classification toward users' security
 Project-URL: repository, https://github.com/Cranfield-GDP3/TACTUS-data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `TACTUS-data-1.1.1/README.md` & `TACTUS-data-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/TACTUS_data.egg-info/PKG-INFO` & `TACTUS-data-1.1.2/TACTUS_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TACTUS-data
-Version: 1.1.1
+Version: 1.1.2
 Summary: Threatening activities classification toward users' security
 Project-URL: repository, https://github.com/Cranfield-GDP3/TACTUS-data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `TACTUS-data-1.1.1/TACTUS_data.egg-info/SOURCES.txt` & `TACTUS-data-1.1.2/TACTUS_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/pyproject.toml` & `TACTUS-data-1.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "TACTUS-data"
 # PEP 440 - Version Identification and Dependency Specification https://peps.python.org/pep-0440/
-version = "1.1.1"
+version = "1.1.2"
 description = "Threatening activities classification toward users' security"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
 ]
 
 dependencies = [
+    "opencv-python",
     "requests",
     "tactus_deep-sort-realtime",
     "torch",
     "ultralytics",
     "matplotlib",
     "Pillow",
     "numpy",
```

### Comparing `TACTUS-data-1.1.1/tactus_data/datasets/dataset.py` & `TACTUS-data-1.1.2/tactus_data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/tactus_data/datasets/ut_interaction.py` & `TACTUS-data-1.1.2/tactus_data/datasets/ut_interaction.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/tactus_data/utils/data_augment.py` & `TACTUS-data-1.1.2/tactus_data/utils/data_augment.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/tactus_data/utils/retracker.py` & `TACTUS-data-1.1.2/tactus_data/utils/retracker.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/tactus_data/utils/skeleton.py` & `TACTUS-data-1.1.2/tactus_data/utils/skeleton.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/tactus_data/utils/skeletonrollingwindow.py` & `TACTUS-data-1.1.2/tactus_data/utils/skeletonrollingwindow.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/tactus_data/utils/thread_videocapture.py` & `TACTUS-data-1.1.2/tactus_data/utils/thread_videocapture.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/tactus_data/utils/visualisation.py` & `TACTUS-data-1.1.2/tactus_data/utils/visualisation.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/tactus_data/utils/yolov7.py` & `TACTUS-data-1.1.2/tactus_data/utils/yolov7.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/tactus_data/utils/yolov8.py` & `TACTUS-data-1.1.2/tactus_data/utils/yolov8.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.1/test/test_skeletonization.py` & `TACTUS-data-1.1.2/test/test_skeletonization.py`

 * *Files identical despite different names*

