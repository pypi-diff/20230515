# Comparing `tmp/whackerhero-0.1.0.tar.gz` & `tmp/whackerhero-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whackerhero-0.1.0.tar", last modified: Mon Dec 27 09:48:31 2021, max compression
+gzip compressed data, was "whackerhero-0.1.1.tar", last modified: Mon May 15 18:59:47 2023, max compression
```

## Comparing `whackerhero-0.1.0.tar` & `whackerhero-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alex      (1000) users      (100)        0 2021-12-27 09:48:31.100330 whackerhero-0.1.0/
--rw-r--r--   0 alex      (1000) users      (100)    35149 2021-12-26 21:41:03.000000 whackerhero-0.1.0/LICENSE.txt
--rw-r--r--   0 alex      (1000) users      (100)     3035 2021-12-27 09:48:31.100330 whackerhero-0.1.0/PKG-INFO
--rw-r--r--   0 alex      (1000) users      (100)     2092 2021-12-27 09:47:00.000000 whackerhero-0.1.0/README.md
--rw-r--r--   0 alex      (1000) users      (100)      104 2021-12-26 21:41:03.000000 whackerhero-0.1.0/pyproject.toml
--rw-r--r--   0 alex      (1000) users      (100)     1092 2021-12-27 09:48:31.100330 whackerhero-0.1.0/setup.cfg
-drwxr-xr-x   0 alex      (1000) users      (100)        0 2021-12-27 09:48:31.100330 whackerhero-0.1.0/src/
-drwxr-xr-x   0 alex      (1000) users      (100)        0 2021-12-27 09:48:31.100330 whackerhero-0.1.0/src/whackerhero.egg-info/
--rw-r--r--   0 alex      (1000) users      (100)     3035 2021-12-27 09:48:31.000000 whackerhero-0.1.0/src/whackerhero.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) users      (100)      301 2021-12-27 09:48:31.000000 whackerhero-0.1.0/src/whackerhero.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) users      (100)        1 2021-12-27 09:48:31.000000 whackerhero-0.1.0/src/whackerhero.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) users      (100)      100 2021-12-27 09:48:31.000000 whackerhero-0.1.0/src/whackerhero.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) users      (100)       33 2021-12-27 09:48:31.000000 whackerhero-0.1.0/src/whackerhero.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) users      (100)       12 2021-12-27 09:48:31.000000 whackerhero-0.1.0/src/whackerhero.egg-info/top_level.txt
--rwxr-xr-x   0 alex      (1000) users      (100)    18742 2021-12-26 23:05:34.000000 whackerhero-0.1.0/src/whackerhero.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:59:47.084537 whackerhero-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 18:59:38.000000 whackerhero-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-15 18:59:47.084537 whackerhero-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-15 18:59:38.000000 whackerhero-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 18:59:38.000000 whackerhero-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-15 18:59:47.084537 whackerhero-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:59:47.084537 whackerhero-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:59:47.084537 whackerhero-0.1.1/src/whackerhero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-15 18:59:47.000000 whackerhero-0.1.1/src/whackerhero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-15 18:59:47.000000 whackerhero-0.1.1/src/whackerhero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:59:47.000000 whackerhero-0.1.1/src/whackerhero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 18:59:47.000000 whackerhero-0.1.1/src/whackerhero.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 18:59:47.000000 whackerhero-0.1.1/src/whackerhero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 18:59:47.000000 whackerhero-0.1.1/src/whackerhero.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18810 2023-05-15 18:59:38.000000 whackerhero-0.1.1/src/whackerhero.py
```

### Comparing `whackerhero-0.1.0/LICENSE.txt` & `whackerhero-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `whackerhero-0.1.0/PKG-INFO` & `whackerhero-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: whackerhero
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate Boomwhacker play-along videos from MIDI files
 Home-page: https://github.com/allejok96/whackerhero
 Author: allejok96
-License: UNKNOWN
 Keywords: boomwhacker video generator midi piano-roll
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -67,9 +65,7 @@
 1. Write notes in sync with the music. What you hear is what you'll see.
    If you make all notes the same short length, things will look less cluttered in the final video.
 1. Export to a midi file.
 1. Run `whackerhero`
 1. Select the midi file and the music video.
 1. Check the `test` box and press start.
 1. If everything looks good, uncheck `test` and run again.
-
-
```

### Comparing `whackerhero-0.1.0/README.md` & `whackerhero-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `whackerhero-0.1.0/setup.cfg` & `whackerhero-0.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = whackerhero
-version = 0.1.0
+version = attr: whackerhero.VERSION
 author = allejok96
 description = Generate Boomwhacker play-along videos from MIDI files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allejok96/whackerhero
 keywords = boomwhacker video generator midi piano-roll
 classifiers =
```

### Comparing `whackerhero-0.1.0/src/whackerhero.egg-info/PKG-INFO` & `whackerhero-0.1.1/src/whackerhero.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: whackerhero
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate Boomwhacker play-along videos from MIDI files
 Home-page: https://github.com/allejok96/whackerhero
 Author: allejok96
-License: UNKNOWN
 Keywords: boomwhacker video generator midi piano-roll
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -67,9 +65,7 @@
 1. Write notes in sync with the music. What you hear is what you'll see.
    If you make all notes the same short length, things will look less cluttered in the final video.
 1. Export to a midi file.
 1. Run `whackerhero`
 1. Select the midi file and the music video.
 1. Check the `test` box and press start.
 1. If everything looks good, uncheck `test` and run again.
-
-
```

### Comparing `whackerhero-0.1.0/src/whackerhero.py` & `whackerhero-0.1.1/src/whackerhero.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 import numpy as np
 from mido import MidiFile
 from moviepy.editor import AudioFileClip, VideoFileClip, VideoClip, CompositeVideoClip, ImageClip
 from moviepy.video.io.ffmpeg_tools import ffmpeg_resize
 from proglog import TqdmProgressBarLogger
 
+VERSION='0.1.1'
+
 BOTTOM_MARGIN = 0.2  # of screen height
 END_TIME = 4  # sec
 FONTS = 'arial.ttf', 'DejaVuSans.ttf', 'LiberationSans-Regular.ttf'
 FONT_HEIGHT = 0.3  # of bottom area
 HIT_EFFECT_COLOR = (255, 255, 255)  # white
 HIT_EFFECT_TIME = 1  # sec
 HIT_LINE_COLOR = (255, 255, 255)  # white
@@ -185,23 +187,23 @@
         pressed_keys = {}  # {key: start_sec}
         self.notes: list[Note] = []
 
         # Iterates all midi messages in the order they were recorded
         for msg in midi:
             # Time is reported as seconds since last message
             total_sec += msg.time
-            # Remember when a key is pressed down
-            if msg.type == 'note_on':
-                if msg.note not in pressed_keys:
-                    pressed_keys[msg.note] = total_sec
             # Save a note when a key is released
-            if msg.type == 'note_off':
+            if msg.type == 'note_off' or (msg.type == 'note_on' and msg.velocity == 0):
                 if msg.note in pressed_keys:
                     self.notes.append(Note(key=msg.note, start=pressed_keys[msg.note], stop=total_sec))
                     del pressed_keys[msg.note]
+            # Remember when a key is pressed down
+            elif msg.type == 'note_on':
+                if msg.note not in pressed_keys:
+                    pressed_keys[msg.note] = total_sec
 
         # All keys that will be displayed
         self.used_keys = sorted(set(note.key for note in self.notes))
 
         self.colors = [Color.fromhex(colorcode) for colorcode in KEYS.values()]
 
         # Common measurements
```

