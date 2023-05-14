# Comparing `tmp/mef_tools-1.1.0.tar.gz` & `tmp/mef_tools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mef_tools-1.1.0.tar", last modified: Thu Oct 15 18:32:38 2020, max compression
+gzip compressed data, was "dist/mef_tools-1.2.0.tar", last modified: Sun May 14 23:01:51 2023, max compression
```

## Comparing `mef_tools-1.1.0.tar` & `mef_tools-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-15 18:32:38.000000 mef_tools-1.1.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      967 2020-10-15 18:32:38.000000 mef_tools-1.1.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-15 18:32:38.000000 mef_tools-1.1.0/mef_tools/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    27635 2020-10-15 18:32:08.000000 mef_tools-1.1.0/mef_tools/io.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-15 18:32:38.000000 mef_tools-1.1.0/mef_tools/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12355 2020-10-15 18:32:08.000000 mef_tools-1.1.0/mef_tools/test/test_io.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-15 18:32:08.000000 mef_tools-1.1.0/mef_tools/test/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      460 2020-10-15 18:32:08.000000 mef_tools-1.1.0/mef_tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1949 2020-10-15 18:32:08.000000 mef_tools-1.1.0/mef_tools/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      269 2020-10-15 18:32:08.000000 mef_tools-1.1.0/mef_tools/server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-10-15 18:32:38.000000 mef_tools-1.1.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-15 18:32:38.000000 mef_tools-1.1.0/mef_tools.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      967 2020-10-15 18:32:38.000000 mef_tools-1.1.0/mef_tools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-15 18:32:38.000000 mef_tools-1.1.0/mef_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2020-10-15 18:32:38.000000 mef_tools-1.1.0/mef_tools.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      314 2020-10-15 18:32:38.000000 mef_tools-1.1.0/mef_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-10-15 18:32:38.000000 mef_tools-1.1.0/mef_tools.egg-info/requires.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6812 2020-10-15 18:32:08.000000 mef_tools-1.1.0/README.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2000 2020-10-15 18:32:08.000000 mef_tools-1.1.0/setup.py
+drwxrwxr-x   0 lambda2   (1000) lambda2   (1000)        0 2023-05-14 23:01:51.000000 mef_tools-1.2.0/
+drwxrwxr-x   0 lambda2   (1000) lambda2   (1000)        0 2023-05-14 23:01:51.000000 mef_tools-1.2.0/mef_tools/
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)     1949 2022-03-04 16:47:53.000000 mef_tools-1.2.0/mef_tools/client.py
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)      401 2023-05-14 22:45:07.000000 mef_tools-1.2.0/mef_tools/__init__.py
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)    43231 2023-05-14 22:37:16.000000 mef_tools-1.2.0/mef_tools/io.py
+drwxrwxr-x   0 lambda2   (1000) lambda2   (1000)        0 2023-05-14 23:01:51.000000 mef_tools-1.2.0/mef_tools/test/
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)        0 2022-03-04 16:47:53.000000 mef_tools-1.2.0/mef_tools/test/__init__.py
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)    12447 2023-05-14 22:45:14.000000 mef_tools-1.2.0/mef_tools/test/test_io.py
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)      269 2022-03-04 16:47:53.000000 mef_tools-1.2.0/mef_tools/server.py
+drwxrwxr-x   0 lambda2   (1000) lambda2   (1000)        0 2023-05-14 23:01:51.000000 mef_tools-1.2.0/mef_tools.egg-info/
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)        1 2023-05-14 23:01:51.000000 mef_tools-1.2.0/mef_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)       56 2023-05-14 23:01:51.000000 mef_tools-1.2.0/mef_tools.egg-info/requires.txt
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)      322 2023-05-14 23:01:51.000000 mef_tools-1.2.0/mef_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)       10 2023-05-14 23:01:51.000000 mef_tools-1.2.0/mef_tools.egg-info/top_level.txt
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)     1035 2023-05-14 23:01:51.000000 mef_tools-1.2.0/mef_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)       38 2023-05-14 23:01:51.000000 mef_tools-1.2.0/setup.cfg
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)     2015 2023-05-14 22:45:07.000000 mef_tools-1.2.0/setup.py
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)     7206 2023-05-14 23:00:58.000000 mef_tools-1.2.0/README.rst
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)    11358 2022-03-04 16:47:53.000000 mef_tools-1.2.0/LICENSE
+-rw-rw-r--   0 lambda2   (1000) lambda2   (1000)     1035 2023-05-14 23:01:51.000000 mef_tools-1.2.0/PKG-INFO
```

### Comparing `mef_tools-1.1.0/PKG-INFO` & `mef_tools-1.2.0/mef_tools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-Metadata-Version: 1.2
-Name: mef_tools
-Version: 1.1.0
-Summary: Advanced tools for handling MEF file format using pymef - python wrapper.
-Home-page: https://github.com/xmival00/MEF_Tools
+Metadata-Version: 2.1
+Name: mef-tools
+Version: 1.2.0
+Summary: Tools for handling Multiscale Eleptrophysiology Format (MEF3) using pymef library.
+Home-page: https://github.com/mselair/MEF_Tools
 Author: Filip Mivalt
 Author-email: mivalt.filip@mayo.edu
 License: Apache
-Description: Advanced tools for handling MEF file format using pymef - python wrapper. MefWriter and MefReader are high-level API tools containing all headers required for writing a mef file.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.6
+License-File: LICENSE
+
+MefWriter and MefReader are high-level API tools containing all headers required for convenient MEF3 file writing and reading.
+
```

### Comparing `mef_tools-1.1.0/mef_tools/test/test_io.py` & `mef_tools-1.2.0/mef_tools/test/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,17 @@
         duration = [10025462] * len(starts)
         new_annotations = pd.DataFrame(data={'time': starts2, 'text': text2, 'type': types,'duration':duration})
         self.mef_writer.write_annotations(new_annotations, channel=channel)
 
         annot_list = self.mef_writer._read_annotation_record(channel=channel)
         read_annotations = pd.DataFrame(annot_list)
         read_annotations = read_annotations[cols]
-        total_annots = new_annotations.append(note_annotations, ignore_index=True)
+
+        # total_annots = new_annotations.append(note_annotations, ignore_index=True)
+        total_annots = pd.concat([new_annotations, note_annotations], ignore_index=True)
 
         pd.testing.assert_frame_equal(read_annotations, total_annots)
 
 
 class TestMefReader(TestCase):
     def setUp(self):
         session_name = 'test_session'
```

### Comparing `mef_tools-1.1.0/mef_tools/client.py` & `mef_tools-1.2.0/mef_tools/client.py`

 * *Files identical despite different names*

### Comparing `mef_tools-1.1.0/mef_tools.egg-info/PKG-INFO` & `mef_tools-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-Metadata-Version: 1.2
-Name: mef-tools
-Version: 1.1.0
-Summary: Advanced tools for handling MEF file format using pymef - python wrapper.
-Home-page: https://github.com/xmival00/MEF_Tools
+Metadata-Version: 2.1
+Name: mef_tools
+Version: 1.2.0
+Summary: Tools for handling Multiscale Eleptrophysiology Format (MEF3) using pymef library.
+Home-page: https://github.com/mselair/MEF_Tools
 Author: Filip Mivalt
 Author-email: mivalt.filip@mayo.edu
 License: Apache
-Description: Advanced tools for handling MEF file format using pymef - python wrapper. MefWriter and MefReader are high-level API tools containing all headers required for writing a mef file.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.6
+License-File: LICENSE
+
+MefWriter and MefReader are high-level API tools containing all headers required for convenient MEF3 file writing and reading.
+
```

