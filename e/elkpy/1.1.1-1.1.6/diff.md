# Comparing `tmp/elkpy-1.1.1.tar.gz` & `tmp/elkpy-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkpy-1.1.1.tar", last modified: Fri Apr 14 14:09:56 2023, max compression
+gzip compressed data, was "elkpy-1.1.6.tar", last modified: Mon May 15 14:50:26 2023, max compression
```

## Comparing `elkpy-1.1.1.tar` & `elkpy-1.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-14 14:09:56.864838 elkpy-1.1.1/
--rw-r--r--   0 max        (501) staff       (20)    35148 2023-03-30 13:19:14.000000 elkpy-1.1.1/COPYING
--rw-r--r--   0 max        (501) staff       (20)    35128 2023-03-30 13:19:14.000000 elkpy-1.1.1/LICENSE
--rw-r--r--   0 max        (501) staff       (20)     5142 2023-04-14 14:09:56.864956 elkpy-1.1.1/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     4447 2023-03-30 13:19:14.000000 elkpy-1.1.1/README.md
--rw-r--r--   0 max        (501) staff       (20)      694 2023-04-14 14:07:40.000000 elkpy-1.1.1/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)      330 2023-04-14 14:09:56.865267 elkpy-1.1.1/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)       69 2023-03-30 13:19:14.000000 elkpy-1.1.1/setup.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-14 14:09:56.858639 elkpy-1.1.1/src/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-14 14:09:56.864071 elkpy-1.1.1/src/elkpy/
--rw-r--r--   0 max        (501) staff       (20)        0 2023-03-30 13:21:26.000000 elkpy-1.1.1/src/elkpy/__init__.py
--rw-r--r--   0 max        (501) staff       (20)    19388 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/audiographcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     9934 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/audioroutingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    16365 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/cvgatecontroller.py
--rw-r--r--   0 max        (501) staff       (20)     1989 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/grpc_gen.py
--rw-r--r--   0 max        (501) staff       (20)     8021 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/keyboardcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    19656 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/midicontroller.py
--rw-r--r--   0 max        (501) staff       (20)    16178 2023-04-14 14:06:32.000000 elkpy-1.1.1/src/elkpy/notificationcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     5032 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/osccontroller.py
--rw-r--r--   0 max        (501) staff       (20)    15841 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/parametercontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6506 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/programcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     3056 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/sessioncontroller.py
--rw-r--r--   0 max        (501) staff       (20)    22973 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/sushi_info_types.py
--rw-r--r--   0 max        (501) staff       (20)     6191 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/sushicontroller.py
--rw-r--r--   0 max        (501) staff       (20)     2143 2023-04-13 14:13:40.000000 elkpy-1.1.1/src/elkpy/sushierrors.py
--rw-r--r--   0 max        (501) staff       (20)     9701 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/sushiprocessor.py
--rw-r--r--   0 max        (501) staff       (20)     3024 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/systemcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6641 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/timingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     7011 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/transportcontroller.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-14 14:09:56.864731 elkpy-1.1.1/src/elkpy.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     5142 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      790 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)        9 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)        6 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-15 14:50:26.035057 elkpy-1.1.6/
+-rw-r--r--   0 max        (501) staff       (20)    35148 2023-03-30 13:19:14.000000 elkpy-1.1.6/COPYING
+-rw-r--r--   0 max        (501) staff       (20)    35128 2023-03-30 13:19:14.000000 elkpy-1.1.6/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-15 14:50:26.035155 elkpy-1.1.6/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     4447 2023-03-30 13:19:14.000000 elkpy-1.1.6/README.md
+-rw-r--r--   0 max        (501) staff       (20)      757 2023-05-15 14:48:54.000000 elkpy-1.1.6/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)      368 2023-05-15 14:50:26.035419 elkpy-1.1.6/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)       69 2023-03-30 13:19:14.000000 elkpy-1.1.6/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-15 14:50:26.029260 elkpy-1.1.6/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-15 14:50:26.034355 elkpy-1.1.6/src/elkpy/
+-rw-r--r--   0 max        (501) staff       (20)        0 2023-03-30 13:21:26.000000 elkpy-1.1.6/src/elkpy/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)    19397 2023-05-15 12:31:59.000000 elkpy-1.1.6/src/elkpy/audiographcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     9934 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/audioroutingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    16365 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/cvgatecontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     1989 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/grpc_gen.py
+-rw-r--r--   0 max        (501) staff       (20)     8021 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/keyboardcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    19656 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/midicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    16178 2023-04-14 14:06:32.000000 elkpy-1.1.6/src/elkpy/notificationcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     5032 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/osccontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    15841 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/parametercontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6506 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/programcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     3056 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/sessioncontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    22973 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/sushi_info_types.py
+-rw-r--r--   0 max        (501) staff       (20)     6191 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/sushicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     2143 2023-04-13 14:13:40.000000 elkpy-1.1.6/src/elkpy/sushierrors.py
+-rw-r--r--   0 max        (501) staff       (20)     9701 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/sushiprocessor.py
+-rw-r--r--   0 max        (501) staff       (20)     3024 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/systemcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6641 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/timingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     7011 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/transportcontroller.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-15 14:50:26.034948 elkpy-1.1.6/src/elkpy.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      790 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       29 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)        6 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/top_level.txt
```

### Comparing `elkpy-1.1.1/COPYING` & `elkpy-1.1.6/COPYING`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/LICENSE` & `elkpy-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/PKG-INFO` & `elkpy-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.1.1
+Version: 1.1.6
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elkpy-1.1.1/README.md` & `elkpy-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/pyproject.toml` & `elkpy-1.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
-requires = ["setuptools>=59.5.0"]
+requires = ["setuptools>=59.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elkpy"
-version = "1.1.1"
+version = "1.1.6"
 authors = [
   { name="Maxime Gendebien", email="max@elk.audio" },
   { name="Ruben Svensson", email="ruben@elk.audio" },
 ]
 description = "A basic controller for sushi using gRPC"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
 ]
+dependencies = ['protobuf', 'grpcio', 'grpcio-tools']
 [project.urls]
 "Homepage" = "https://github.com/elkaudio/elkpy"
 "Bug Tracker" = "https://github.com/elkaudio/elkpy/issues"
```

### Comparing `elkpy-1.1.1/src/elkpy/audiographcontroller.py` & `elkpy-1.1.6/src/elkpy/audiographcontroller.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,16 +392,16 @@
                                   str, processor_type: info_types.PluginType, track_id: int,
                                   before_processor: int, add_to_back: bool) -> None:
         """
         Create a new processor on an existing track.
 
         Parameters:
             name (str): The name to assign the processor. Must be unique.
-            uid (str): The uid of an internal sushi processor or the URI of an LV2 processor. Not applicable for vst2 or vst3.
-            path (str): The path to the processor library. Only for vst2 or vst3 processors.
+            uid (str): The uid of an internal Sushi processor. Not applicable for vst2, vst3 and lv2.
+            path (str): The path to the processor library (for vst2 or vst3 processors) or the URI of an installed lv2 plugin.
             processor_type (info_type.PluginType): The type of processor to create.
             track_id (int): The id of the track to add the processor to.
             before_processor (int): Which existing processor to create the new processor in front of.
             add_to_back (bool): Set to true to add the processor to the back of the processing chain on the track.
         """
         try:
             self._stub.CreateProcessorOnTrack(self._sushi_proto.CreateProcessorRequest(
```

### Comparing `elkpy-1.1.1/src/elkpy/audioroutingcontroller.py` & `elkpy-1.1.6/src/elkpy/audioroutingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/cvgatecontroller.py` & `elkpy-1.1.6/src/elkpy/cvgatecontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/grpc_gen.py` & `elkpy-1.1.6/src/elkpy/grpc_gen.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/keyboardcontroller.py` & `elkpy-1.1.6/src/elkpy/keyboardcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/midicontroller.py` & `elkpy-1.1.6/src/elkpy/midicontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/notificationcontroller.py` & `elkpy-1.1.6/src/elkpy/notificationcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/osccontroller.py` & `elkpy-1.1.6/src/elkpy/osccontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/parametercontroller.py` & `elkpy-1.1.6/src/elkpy/parametercontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/programcontroller.py` & `elkpy-1.1.6/src/elkpy/programcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/sessioncontroller.py` & `elkpy-1.1.6/src/elkpy/sessioncontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/sushi_info_types.py` & `elkpy-1.1.6/src/elkpy/sushi_info_types.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/sushicontroller.py` & `elkpy-1.1.6/src/elkpy/sushicontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/sushierrors.py` & `elkpy-1.1.6/src/elkpy/sushierrors.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/sushiprocessor.py` & `elkpy-1.1.6/src/elkpy/sushiprocessor.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/systemcontroller.py` & `elkpy-1.1.6/src/elkpy/systemcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/timingcontroller.py` & `elkpy-1.1.6/src/elkpy/timingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy/transportcontroller.py` & `elkpy-1.1.6/src/elkpy/transportcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.1/src/elkpy.egg-info/PKG-INFO` & `elkpy-1.1.6/src/elkpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.1.1
+Version: 1.1.6
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elkpy-1.1.1/src/elkpy.egg-info/SOURCES.txt` & `elkpy-1.1.6/src/elkpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

