# Comparing `tmp/recode-0.1.8.tar.gz` & `tmp/recode-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recode-0.1.8.tar", last modified: Thu Jun 24 20:04:46 2021, max compression
+gzip compressed data, was "recode-0.1.9.tar", last modified: Fri Jun 25 14:58:51 2021, max compression
```

## Comparing `recode-0.1.8.tar` & `recode-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:04:46.619754 recode-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-24 20:04:26.000000 recode-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17552 2021-06-24 20:04:46.619754 recode-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12870 2021-06-24 20:04:26.000000 recode-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:04:46.619754 recode-0.1.8/recode/
--rw-r--r--   0 runner    (1001) docker     (121)    12413 2021-06-24 20:04:26.000000 recode-0.1.8/recode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-06-24 20:04:26.000000 recode-0.1.8/recode/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:04:46.619754 recode-0.1.8/recode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17552 2021-06-24 20:04:46.000000 recode-0.1.8/recode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-06-24 20:04:46.000000 recode-0.1.8/recode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 20:04:46.000000 recode-0.1.8/recode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 20:04:46.000000 recode-0.1.8/recode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-24 20:04:46.000000 recode-0.1.8/recode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      538 2021-06-24 20:04:46.623755 recode-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-06-24 20:04:26.000000 recode-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 14:58:51.329856 recode-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-25 14:58:32.000000 recode-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    17778 2021-06-25 14:58:51.329856 recode-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13048 2021-06-25 14:58:32.000000 recode-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 14:58:51.325857 recode-0.1.9/recode/
+-rw-r--r--   0 runner    (1001) docker     (121)    12413 2021-06-25 14:58:32.000000 recode-0.1.9/recode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-06-25 14:58:32.000000 recode-0.1.9/recode/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 14:58:51.329856 recode-0.1.9/recode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    17778 2021-06-25 14:58:51.000000 recode-0.1.9/recode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2021-06-25 14:58:51.000000 recode-0.1.9/recode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-25 14:58:51.000000 recode-0.1.9/recode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-25 14:58:51.000000 recode-0.1.9/recode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-25 14:58:51.000000 recode-0.1.9/recode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2021-06-25 14:58:51.329856 recode-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-06-25 14:58:32.000000 recode-0.1.9/setup.py
```

### Comparing `recode-0.1.8/LICENSE` & `recode-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `recode-0.1.8/PKG-INFO` & `recode-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recode
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools to make codecs for time-series serialization and deserialization.
 Home-page: https://github.com/otosense/recode
 Author: OtoSense
 License: apache-2.0
 Description: 
         # recode
         Make codecs for fixed size structured chunks serialization and deserialization of
@@ -552,9 +552,15 @@
         encoder = ChunkedEncoder(frame_to_chk = specs.frame_to_chk)
         decoder = ChunkedDecoder(chk_to_frame=specs.chk_to_frame)
         b = encoder(frames)
         decoded_frames = list(decoder(b))
         assert decoded_frames == [(1.1,2.2),(3.3,4.4)]
         ```
         
+        # More
+        
+        [Example of recode functionality to read and write audio files](https://github.com/otosense/recode/wiki/Example-of-recode-functionality-to-read-and-write-audio-files)
+        
+        
+        
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `recode-0.1.8/README.md` & `recode-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -544,7 +544,13 @@
 frames, specs = specs_from_frames(frames)
 encoder = ChunkedEncoder(frame_to_chk = specs.frame_to_chk)
 decoder = ChunkedDecoder(chk_to_frame=specs.chk_to_frame)
 b = encoder(frames)
 decoded_frames = list(decoder(b))
 assert decoded_frames == [(1.1,2.2),(3.3,4.4)]
 ```
+
+# More
+
+[Example of recode functionality to read and write audio files](https://github.com/otosense/recode/wiki/Example-of-recode-functionality-to-read-and-write-audio-files)
+
+
```

### Comparing `recode-0.1.8/recode/__init__.py` & `recode-0.1.9/recode/__init__.py`

 * *Files identical despite different names*

### Comparing `recode-0.1.8/recode/util.py` & `recode-0.1.9/recode/util.py`

 * *Files identical despite different names*

### Comparing `recode-0.1.8/recode.egg-info/PKG-INFO` & `recode-0.1.9/recode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recode
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools to make codecs for time-series serialization and deserialization.
 Home-page: https://github.com/otosense/recode
 Author: OtoSense
 License: apache-2.0
 Description: 
         # recode
         Make codecs for fixed size structured chunks serialization and deserialization of
@@ -552,9 +552,15 @@
         encoder = ChunkedEncoder(frame_to_chk = specs.frame_to_chk)
         decoder = ChunkedDecoder(chk_to_frame=specs.chk_to_frame)
         b = encoder(frames)
         decoded_frames = list(decoder(b))
         assert decoded_frames == [(1.1,2.2),(3.3,4.4)]
         ```
         
+        # More
+        
+        [Example of recode functionality to read and write audio files](https://github.com/otosense/recode/wiki/Example-of-recode-functionality-to-read-and-write-audio-files)
+        
+        
+        
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `recode-0.1.8/setup.cfg` & `recode-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = recode
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/otosense/recode
 platforms = any
 description_file = README.md
 root_url = https://github.com/otosense/
 license = apache-2.0
 author = OtoSense
 description = Tools to make codecs for time-series serialization and deserialization.
```

