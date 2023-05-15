# Comparing `tmp/convert_videos-2.8.6.tar.gz` & `tmp/convert_videos-2.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert_videos-2.8.6.tar", max compression
+gzip compressed data, was "convert_videos-2.8.7.tar", max compression
```

## Comparing `convert_videos-2.8.6.tar` & `convert_videos-2.8.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-05-06 13:21:43.305393 convert_videos-2.8.6/LICENSE.md
--rw-r--r--   0        0        0     4316 2023-05-06 13:21:43.305393 convert_videos-2.8.6/README.md
--rwxr-xr-x   0        0        0      195 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/__init__.py
--rw-r--r--   0        0        0     4431 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/cli.py
--rw-r--r--   0        0        0      219 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/colour.py
--rw-r--r--   0        0        0     2399 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/ffmpeg_converter.py
--rw-r--r--   0        0        0     2196 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/processor.py
--rw-r--r--   0        0        0     4045 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/settings.py
--rw-r--r--   0        0        0     4520 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/video_processor.py
--rw-r--r--   0        0        0      836 2023-05-06 13:21:43.309393 convert_videos-2.8.6/pyproject.toml
--rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 convert_videos-2.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-15 12:46:29.487639 convert_videos-2.8.7/LICENSE.md
+-rw-r--r--   0        0        0     4316 2023-05-15 12:46:29.487639 convert_videos-2.8.7/README.md
+-rwxr-xr-x   0        0        0      195 2023-05-15 12:46:29.487639 convert_videos-2.8.7/convert_videos/__init__.py
+-rw-r--r--   0        0        0     4360 2023-05-15 12:46:29.487639 convert_videos-2.8.7/convert_videos/cli.py
+-rw-r--r--   0        0        0      219 2023-05-15 12:46:29.487639 convert_videos-2.8.7/convert_videos/colour.py
+-rw-r--r--   0        0        0     2399 2023-05-15 12:46:29.487639 convert_videos-2.8.7/convert_videos/ffmpeg_converter.py
+-rw-r--r--   0        0        0     2196 2023-05-15 12:46:29.487639 convert_videos-2.8.7/convert_videos/processor.py
+-rw-r--r--   0        0        0     4045 2023-05-15 12:46:29.487639 convert_videos-2.8.7/convert_videos/settings.py
+-rw-r--r--   0        0        0     4514 2023-05-15 12:46:29.487639 convert_videos-2.8.7/convert_videos/video_processor.py
+-rw-r--r--   0        0        0      836 2023-05-15 12:46:29.487639 convert_videos-2.8.7/pyproject.toml
+-rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 convert_videos-2.8.7/PKG-INFO
```

### Comparing `convert_videos-2.8.6/LICENSE.md` & `convert_videos-2.8.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.6/README.md` & `convert_videos-2.8.7/README.md`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.6/convert_videos/cli.py` & `convert_videos-2.8.7/convert_videos/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,22 +68,19 @@
     dry_run,
     encoder,
     audio_language,
     subtitle_language,
 ):
     configure_logger(verbose)
 
-    print(subtitle_language)
     video_settings = VideoSettings(
         codec=Codec(video_codec), quality=quality, preset=preset, width=width, encoder=encoder, subtitle_language=subtitle_language
     )
     audio_settings = AudioSettings(codec=Codec(audio_codec), channels=audio_channels, bitrate=audio_bitrate, language=audio_language)
 
-    print(video_settings.codec.__dict__)
-
     results = []
     for directory in directories:
         results += Processor(
             directory=directory,
             force=force,
             video_settings=video_settings,
             audio_settings=audio_settings,
```

### Comparing `convert_videos-2.8.6/convert_videos/ffmpeg_converter.py` & `convert_videos-2.8.7/convert_videos/ffmpeg_converter.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.6/convert_videos/processor.py` & `convert_videos-2.8.7/convert_videos/processor.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.6/convert_videos/settings.py` & `convert_videos-2.8.7/convert_videos/settings.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.6/convert_videos/video_processor.py` & `convert_videos-2.8.7/convert_videos/video_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,25 +23,28 @@
     # The file would be converted, if we weren't running in dry-run mode
     WOULD_CONVERT = auto()
 
     # If a file is already converted with renaming
     # (e.g. appending the output codec) and this is that converted file
     ALREADY_PROCESSED = auto()
 
-    # Force can override already in desired format, but not if both original and converted files already exist
-    FORCE_CONVERTED = auto()
-
     # The file is already using the target format, can be overridden with --force
     IN_DESIRED_FORMAT = auto()
 
     FAILED = auto()
 
     def __str__(self):
         return titlecase(lowercase(self.name))
 
+    def colour(self):
+        c = "green"
+        if self == Status.FAILED:
+            c = "red"
+        return colour(c, str(self))
+
 
 @dataclass
 class VideoProcessor:
     video: Video
     video_settings: VideoSettings
     audio_settings: AudioSettings
     container: str
```

### Comparing `convert_videos-2.8.6/pyproject.toml` & `convert_videos-2.8.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convert_videos"
-version = "2.8.6"
+version = "2.8.7"
 description = "This tool allows bulk conversion of videos using ffmpeg"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `convert_videos-2.8.6/PKG-INFO` & `convert_videos-2.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-videos
-Version: 2.8.6
+Version: 2.8.7
 Summary: This tool allows bulk conversion of videos using ffmpeg
 License: MIT
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

