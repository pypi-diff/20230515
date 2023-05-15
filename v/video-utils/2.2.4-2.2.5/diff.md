# Comparing `tmp/video_utils-2.2.4.tar.gz` & `tmp/video_utils-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_utils-2.2.4.tar", max compression
+gzip compressed data, was "video_utils-2.2.5.tar", max compression
```

## Comparing `video_utils-2.2.4.tar` & `video_utils-2.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-05-06 13:10:07.403968 video_utils-2.2.4/LICENSE.md
--rw-r--r--   0        0        0      917 2023-05-06 13:10:07.403968 video_utils-2.2.4/README.md
--rw-r--r--   0        0        0      726 2023-05-06 13:10:07.403968 video_utils-2.2.4/pyproject.toml
--rw-r--r--   0        0        0      166 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/__init__.py
--rw-r--r--   0        0        0     1626 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/codec.py
--rw-r--r--   0        0        0      258 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/colour.py
--rw-r--r--   0        0        0     5181 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/fileMap.py
--rw-r--r--   0        0        0      868 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/parse_episode.py
--rw-r--r--   0        0        0     1549 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/validators.py
--rw-r--r--   0        0        0     2649 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/video.py
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 video_utils-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-15 13:34:03.040912 video_utils-2.2.5/LICENSE.md
+-rw-r--r--   0        0        0      917 2023-05-15 13:34:03.040912 video_utils-2.2.5/README.md
+-rw-r--r--   0        0        0      726 2023-05-15 13:34:03.040912 video_utils-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/__init__.py
+-rw-r--r--   0        0        0     1627 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/codec.py
+-rw-r--r--   0        0        0      259 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/colour.py
+-rw-r--r--   0        0        0     5355 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/fileMap.py
+-rw-r--r--   0        0        0      868 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/parse_episode.py
+-rw-r--r--   0        0        0     1549 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/validators.py
+-rw-r--r--   0        0        0     2649 2023-05-15 13:34:03.044912 video_utils-2.2.5/video_utils/video.py
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 video_utils-2.2.5/PKG-INFO
```

### Comparing `video_utils-2.2.4/LICENSE.md` & `video_utils-2.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.4/README.md` & `video_utils-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.4/pyproject.toml` & `video_utils-2.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "video_utils"
-version = "2.2.4"
+version = "2.2.5"
 description = "This library is used for lots of shared functionality around parsing TV shows and movies"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `video_utils-2.2.4/video_utils/codec.py` & `video_utils-2.2.5/video_utils/codec.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 
     def get_ffmpeg_name(self, encoder="software"):
         if self._ffmpeg_name:
             return self._ffmpeg_name
         try:
             return self._data["ffmpeg_names"][encoder]
         except:
-            return None
+            return None
```

### Comparing `video_utils-2.2.4/video_utils/fileMap.py` & `video_utils-2.2.5/video_utils/fileMap.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 from .validators import Filter
 from .video import Video
 
 log = logging.getLogger(__name__)
 
 
 class FileMap:
-    def __init__(self, directory, update=True, use_cache=True):
+    def __init__(self, directory, update=True, use_cache=True, progress_bar=True):
         """
         update and use_cache values are only honoured on object initialization
         """
         self.directory = directory
         self._update = update
         self._use_cache = use_cache
+        self._progress_bar = progress_bar
         self.contents = {}
         self._validate_settings(update=self.update, use_cache=self.use_cache)
 
     @property
     def directory(self):
         return self._directory
 
@@ -74,15 +75,15 @@
             self._prune_missing_files()
         for dir_path, dir_names, file_names in self._file_tree():
             log.info(colour("green", "Working in directory: %s" % dir_path))
 
             video_files = filter.only_videos(file_names)
             log.debug("Total videos in %s: %s" % (dir_path, len(video_files)))
 
-            if log.level > logging.INFO:
+            if self._progress_bar:
                 video_files = tqdm(video_files)
 
             for video_file in video_files:
                 self._update_video(dir_path, video_file)
 
     def _update_video(self, dir_path, video_name):
         if dir_path not in self.contents:
@@ -109,23 +110,27 @@
             file_tree = os.walk(self.directory, followlinks=True)
         return file_tree
 
     def _prune_missing_files(self):
         log.info(colour("blue", "Checking for missing/deleted files..."))
         # Can't mutate the original while we iterate through it
         contents_copy = deepcopy(self.contents)
-        if log.level > logging.INFO:
-            contents_copy = tqdm(contents_copy)
         for dir_path in contents_copy:
+            log.info(colour("blue", f"Processing directory {dir_path}"))
+
             if not path.exists(dir_path):
                 log.debug("Removing %s from cache" % dir_path)
                 del self.contents[dir_path]
                 continue
 
-            for video in contents_copy[dir_path]:
+            sub_directory = contents_copy[dir_path]
+            if self._progress_bar:
+                sub_directory = tqdm(sub_directory)
+
+            for video in sub_directory:
                 if not path.exists(video.full_path):
                     log.debug("Removing %s from cache" % video.full_path)
                     self.contents[dir_path].remove(video)
 
 
 class _FileMapStorage:
     def __init__(self, directory):
```

### Comparing `video_utils-2.2.4/video_utils/parse_episode.py` & `video_utils-2.2.5/video_utils/parse_episode.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.4/video_utils/validators.py` & `video_utils-2.2.5/video_utils/validators.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.4/video_utils/video.py` & `video_utils-2.2.5/video_utils/video.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.4/PKG-INFO` & `video_utils-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-utils
-Version: 2.2.4
+Version: 2.2.5
 Summary: This library is used for lots of shared functionality around parsing TV shows and movies
 License: MIT
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

