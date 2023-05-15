# Comparing `tmp/unitranscode-0.3.3.tar.gz` & `tmp/unitranscode-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitranscode-0.3.3.tar", last modified: Fri May  5 08:31:23 2023, max compression
+gzip compressed data, was "unitranscode-0.4.0.tar", last modified: Mon May 15 03:37:41 2023, max compression
```

## Comparing `unitranscode-0.3.3.tar` & `unitranscode-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-05 08:31:23.014281 unitranscode-0.3.3/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.3.3/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-05-05 08:31:23.014281 unitranscode-0.3.3/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.3.3/README.md
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-05 08:31:23.014281 unitranscode-0.3.3/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      717 2023-05-05 08:30:58.000000 unitranscode-0.3.3/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-05 08:31:23.010281 unitranscode-0.3.3/tests/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1138 2023-04-28 03:34:33.000000 unitranscode-0.3.3/tests/test_transcoder.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-05 08:31:23.010281 unitranscode-0.3.3/unitranscode/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.3.3/unitranscode/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3661 2023-04-28 03:37:11.000000 unitranscode-0.3.3/unitranscode/custom_types.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    25714 2023-05-05 08:20:48.000000 unitranscode-0.3.3/unitranscode/transcoder.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-05-01 05:12:02.000000 unitranscode-0.3.3/unitranscode/utils.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-05 08:31:23.014281 unitranscode-0.3.3/unitranscode.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/top_level.txt
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-15 03:37:41.915683 unitranscode-0.4.0/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.4.0/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-05-15 03:37:41.915683 unitranscode-0.4.0/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.4.0/README.md
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-15 03:37:41.915683 unitranscode-0.4.0/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      717 2023-05-15 03:37:18.000000 unitranscode-0.4.0/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-15 03:37:41.915683 unitranscode-0.4.0/tests/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1525 2023-05-15 03:36:36.000000 unitranscode-0.4.0/tests/test_transcoder.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-15 03:37:41.915683 unitranscode-0.4.0/unitranscode/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.4.0/unitranscode/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     3661 2023-04-28 03:37:11.000000 unitranscode-0.4.0/unitranscode/custom_types.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    26830 2023-05-15 03:34:49.000000 unitranscode-0.4.0/unitranscode/transcoder.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-05-01 05:12:02.000000 unitranscode-0.4.0/unitranscode/utils.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-15 03:37:41.915683 unitranscode-0.4.0/unitranscode.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-05-15 03:37:41.000000 unitranscode-0.4.0/unitranscode.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-05-15 03:37:41.000000 unitranscode-0.4.0/unitranscode.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-15 03:37:41.000000 unitranscode-0.4.0/unitranscode.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-05-15 03:37:41.000000 unitranscode-0.4.0/unitranscode.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-05-15 03:37:41.000000 unitranscode-0.4.0/unitranscode.egg-info/top_level.txt
```

### Comparing `unitranscode-0.3.3/LICENSE` & `unitranscode-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.3/PKG-INFO` & `unitranscode-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.3.3
+Version: 0.4.0
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
+License: UNKNOWN
 Keywords: unitranscode
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `unitranscode-0.3.3/README.md` & `unitranscode-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.3/setup.py` & `unitranscode-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='unitranscode',
-    version='0.3.3',
+    version='0.4.0',
     description='Universal transcoding library',
     url='https://github.com/MatthewScholefield/unitranscode',
     author='Matthew D. Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `unitranscode-0.3.3/tests/test_transcoder.py` & `unitranscode-0.4.0/tests/test_transcoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,7 +31,20 @@
     out_files = transcoder.extract_cuts(
         in_file, cuts, str(temp_folder.joinpath('out-%d.wav'))
     )
 
     assert transcoder.info(out_files[0]).duration_s == pytest.approx(1.0)
     assert transcoder.info(out_files[1]).duration_s == pytest.approx(1.5)
     assert transcoder.info(out_files[2]).duration_s == pytest.approx(3.0)
+
+
+def test_transcode_wav(example_20s_wav_file: Path, temp_folder: Path):
+    transcoder = Transcoder()
+    out_file = transcoder.transcode(
+        str(example_20s_wav_file),
+        str(temp_folder.joinpath('output.wav')),
+        audio_codec='pcm_s16le',
+    )
+    assert (
+        transcoder.info(example_20s_wav_file).duration_s
+        == transcoder.info(out_file).duration_s
+    )
```

### Comparing `unitranscode-0.3.3/unitranscode/custom_types.py` & `unitranscode-0.4.0/unitranscode/custom_types.py`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.3/unitranscode/transcoder.py` & `unitranscode-0.4.0/unitranscode/transcoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -381,20 +381,21 @@
         self,
         input: Union[str, List[str]],
         output: str,
         channels: Optional[int] = None,
         sample_rate: Optional[int] = None,
         audio_index: int = None,
         video_index: int = None,
+        audio_codec: str = None,
         mix_down=True,
         extra_args: list = None,
         on_progress: ProgressHandler = None,
         audiogram_op: Union[AudiogramOp, dict] = None,
         op: FfmpegOperation = None,
-    ):
+    ) -> str:
         op = op or self.op()
         op.input_files = [input] if isinstance(input, str) else list(input)
         infos = op.input_files_info
         args = []
         for i in op.input_files:
             args.extend(['-i', i])
         if audiogram_op:
@@ -482,24 +483,31 @@
                     '-map',
                     '[outv]:v',
                     '-map',
                     '0:a',
                 ]
             )
 
-        if not did_mix:
-            audio_infos = [
-                infos[i].audio_stream
-                for i in audio_indices
-                if infos[i].audio_stream_maybe
-            ]
-            if not audio_infos:
-                raise UnitranscodeFormatError(
-                    'Input does not have any audio channels!'
-                )
+        audio_infos = [
+            infos[i].audio_stream
+            for i in audio_indices
+            if infos[i].audio_stream_maybe
+        ]
+        if not audio_infos:
+            raise UnitranscodeFormatError(
+                'Input does not have any audio channels!'
+            )
+
+        if audio_codec:
+            if not did_mix and audio_infos[0]['codec_name'] == audio_codec:
+                args.extend(['-c:a', 'copy'])
+            else:
+                args.extend(['-c:a', audio_codec])
+
+        if not did_mix and not audio_codec:
             audio_info = audio_infos[0]
             incompatible = False
             if (
                 sample_rate is not None
                 and audio_info['sample_rate'] != sample_rate
             ):
                 incompatible = True
@@ -580,24 +588,49 @@
         in_file: str,
         cuts: List[Tuple[float, float]],
         output_file: str,
         on_progress: ProgressHandler = None,
         op: FfmpegOperation = None,
     ) -> str:
         op = op or self.op()
-        filter_str = '+'.join(
-            f'between(t,{start},{end})' for start, end in cuts
+        info = self.info(in_file)
+        has_video = bool(info.video_stream_maybe)
+        has_audio = bool(info.audio_stream_maybe)
+        filter_cmds = []
+        stream_names = []
+        for i, (lt, rt) in enumerate(cuts):
+            cmd = ''
+            name = ''
+            if has_video:
+                cmd += f'[0:v]trim={lt}:{rt},setpts=PTS-STARTPTS[v{i}];'
+                name += f'[v{i}]'
+            if has_audio:
+                cmd += f'[0:a]atrim={lt}:{rt},asetpts=PTS-STARTPTS[a{i}];'
+                name += f'[a{i}]'
+            filter_cmds.append(cmd)
+            stream_names.append(name)
+        video_output = '[v]' * has_video
+        audio_output = '[a]' * has_audio
+        complex_filter = (
+            ''.join(filter_cmds)
+            + ''.join(stream_names)
+            + f'concat=n={str(len(stream_names))}'
+            + f':v={[0, 1][has_video]}:a={[0, 1][has_audio]}'
+            + video_output
+            + audio_output
         )
 
         self.ffmpeg(
             *('-i', in_file),
-            *('-vf', f"select='{filter_str}',setpts=N/FRAME_RATE/TB"),
-            *('-af', f"aselect='{filter_str}',asetpts=N/SR/TB"),
+            *('-filter_complex', complex_filter),
+            *('-map', video_output) * has_video,
+            *('-map', audio_output) * has_audio,
+            '-shortest',
             output_file,
-            duration_s=self.info(in_file).duration_s if on_progress else None,
+            duration_s=sum(b - a for a, b in cuts),
             on_progress=on_progress,
             op=op,
         )
         return output_file
 
     @staticmethod
     def _format_duration(dur: float) -> str:
```

### Comparing `unitranscode-0.3.3/unitranscode.egg-info/PKG-INFO` & `unitranscode-0.4.0/unitranscode.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.3.3
+Version: 0.4.0
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
+License: UNKNOWN
 Keywords: unitranscode
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
+
+UNKNOWN
+
```

