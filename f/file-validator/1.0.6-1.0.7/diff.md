# Comparing `tmp/file_validator-1.0.6.tar.gz` & `tmp/file_validator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Progamming Project\file-validator\dist\.tmp-vh05ocbu\file_validator-1.0.6.tar", last modified: Sun May 14 22:38:34 2023, max compression
+gzip compressed data, was "F:\Progamming Project\file-validator\dist\.tmp-88umq59z\file_validator-1.0.7.tar", last modified: Mon May 15 12:15:45 2023, max compression
```

## Comparing `file_validator-1.0.6.tar` & `file_validator-1.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.796372 file_validator-1.0.6/
--rw-rw-rw-   0        0        0      115 2023-03-23 16:55:55.000000 file_validator-1.0.6/AUTHORS.md
--rw-rw-rw-   0        0        0     2474 2023-03-23 16:55:55.000000 file_validator-1.0.6/CONTRIBUTING.md
--rw-rw-rw-   0        0        0      162 2023-03-23 16:55:55.000000 file_validator-1.0.6/HISTORY.md
--rw-rw-rw-   0        0        0     1091 2023-03-23 16:55:55.000000 file_validator-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      310 2023-03-23 16:55:55.000000 file_validator-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     8148 2023-05-14 22:38:34.797362 file_validator-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     6289 2023-05-14 21:22:48.000000 file_validator-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.767360 file_validator-1.0.6/file_validator/
--rw-rw-rw-   0        0        0      136 2023-05-14 22:19:37.000000 file_validator-1.0.6/file_validator/__init__.py
--rw-rw-rw-   0        0        0     2765 2023-03-30 15:19:51.000000 file_validator-1.0.6/file_validator/constants.py
--rw-rw-rw-   0        0        0     3978 2023-03-30 15:19:51.000000 file_validator-1.0.6/file_validator/exceptions.py
--rw-rw-rw-   0        0        0      807 2023-05-14 21:22:48.000000 file_validator-1.0.6/file_validator/forms.py
--rw-rw-rw-   0        0        0    12995 2023-05-14 22:32:47.000000 file_validator-1.0.6/file_validator/models.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.675359 file_validator-1.0.6/file_validator/templates/
-drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.782368 file_validator-1.0.6/file_validator/templates/file_validator/
--rw-rw-rw-   0        0        0      127 2023-03-23 16:55:55.000000 file_validator-1.0.6/file_validator/templates/file_validator/file_input_widget.html
--rw-rw-rw-   0        0        0     4204 2023-05-14 21:22:48.000000 file_validator-1.0.6/file_validator/utils.py
--rw-rw-rw-   0        0        0    16723 2023-05-14 21:22:48.000000 file_validator-1.0.6/file_validator/validators.py
--rw-rw-rw-   0        0        0      214 2023-05-14 21:22:48.000000 file_validator-1.0.6/file_validator/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.779378 file_validator-1.0.6/file_validator.egg-info/
--rw-rw-rw-   0        0        0     8148 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      206 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      846 2023-05-14 22:38:34.798359 file_validator-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2774 2023-05-14 22:19:37.000000 file_validator-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:15:45.569163 file_validator-1.0.7/
+-rw-rw-rw-   0        0        0      115 2023-03-23 16:55:55.000000 file_validator-1.0.7/AUTHORS.md
+-rw-rw-rw-   0        0        0     2474 2023-03-23 16:55:55.000000 file_validator-1.0.7/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0      162 2023-03-23 16:55:55.000000 file_validator-1.0.7/HISTORY.md
+-rw-rw-rw-   0        0        0     1091 2023-03-23 16:55:55.000000 file_validator-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      310 2023-03-23 16:55:55.000000 file_validator-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     8172 2023-05-15 12:15:45.569163 file_validator-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6289 2023-05-14 21:22:48.000000 file_validator-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 12:15:45.559162 file_validator-1.0.7/file_validator/
+-rw-rw-rw-   0        0        0      136 2023-05-15 12:14:30.000000 file_validator-1.0.7/file_validator/__init__.py
+-rw-rw-rw-   0        0        0     2765 2023-03-30 15:19:51.000000 file_validator-1.0.7/file_validator/constants.py
+-rw-rw-rw-   0        0        0     3978 2023-03-30 15:19:51.000000 file_validator-1.0.7/file_validator/exceptions.py
+-rw-rw-rw-   0        0        0      807 2023-05-14 21:22:48.000000 file_validator-1.0.7/file_validator/forms.py
+-rw-rw-rw-   0        0        0    12995 2023-05-14 22:32:47.000000 file_validator-1.0.7/file_validator/models.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:15:45.437160 file_validator-1.0.7/file_validator/templates/
+drwxrwxrwx   0        0        0        0 2023-05-15 12:15:45.568163 file_validator-1.0.7/file_validator/templates/file_validator/
+-rw-rw-rw-   0        0        0      127 2023-03-23 16:55:55.000000 file_validator-1.0.7/file_validator/templates/file_validator/file_input_widget.html
+-rw-rw-rw-   0        0        0     4204 2023-05-14 21:22:48.000000 file_validator-1.0.7/file_validator/utils.py
+-rw-rw-rw-   0        0        0    16723 2023-05-14 21:22:48.000000 file_validator-1.0.7/file_validator/validators.py
+-rw-rw-rw-   0        0        0      214 2023-05-14 21:22:48.000000 file_validator-1.0.7/file_validator/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:15:45.567166 file_validator-1.0.7/file_validator.egg-info/
+-rw-rw-rw-   0        0        0     8172 2023-05-15 12:15:45.000000 file_validator-1.0.7/file_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-05-15 12:15:45.000000 file_validator-1.0.7/file_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 12:15:45.000000 file_validator-1.0.7/file_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-15 12:15:45.000000 file_validator-1.0.7/file_validator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 12:15:45.000000 file_validator-1.0.7/file_validator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      223 2023-05-15 12:15:45.000000 file_validator-1.0.7/file_validator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-15 12:15:45.000000 file_validator-1.0.7/file_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      846 2023-05-15 12:15:45.570162 file_validator-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2832 2023-05-15 12:14:31.000000 file_validator-1.0.7/setup.py
```

### Comparing `file_validator-1.0.6/CONTRIBUTING.md` & `file_validator-1.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/LICENSE` & `file_validator-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/PKG-INFO` & `file_validator-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_validator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python validation library to validate files using type, mime, extension, magic numbers and size ✅
 Home-page: https://github.com/file-validator/file-validator
 Author: Reza Shakeri
 Author-email: rzashakeri@outlook.com
 License: MIT license
 Project-URL: Documentation, https://file-validator.github.io/
 Project-URL: Homepage, https://github.com/file-validator
@@ -26,14 +26,15 @@
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: django
 License-File: LICENSE
 License-File: AUTHORS.md
 
 <pre style="position: relative;color: black;">0000-0010:  89 50 4e 47-0d 0a 1a 0a-00 00 00 0d-49 48 44 52  .PNG.... ....IHDR
 0000-0020:  00 00 04 7b-00 00 04 dc-08 06 00 00-00 14 48 89  ...{.... ......H.
 0000-0030:  b8 00 00 20-00 49 44 41-54 78 9c ec-dd dd 6f 9b  .....IDA Tx....o.
 0000-0040:  e7 79 c7 f1-4b 22 25 ca-2c d9 06 89-e2 84 69 d2  .y..K"%. ,.....i.
```

### Comparing `file_validator-1.0.6/README.md` & `file_validator-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/file_validator/constants.py` & `file_validator-1.0.7/file_validator/constants.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/file_validator/exceptions.py` & `file_validator-1.0.7/file_validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/file_validator/forms.py` & `file_validator-1.0.7/file_validator/forms.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/file_validator/models.py` & `file_validator-1.0.7/file_validator/models.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/file_validator/utils.py` & `file_validator-1.0.7/file_validator/utils.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/file_validator/validators.py` & `file_validator-1.0.7/file_validator/validators.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/file_validator.egg-info/PKG-INFO` & `file_validator-1.0.7/file_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-validator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python validation library to validate files using type, mime, extension, magic numbers and size ✅
 Home-page: https://github.com/file-validator/file-validator
 Author: Reza Shakeri
 Author-email: rzashakeri@outlook.com
 License: MIT license
 Project-URL: Documentation, https://file-validator.github.io/
 Project-URL: Homepage, https://github.com/file-validator
@@ -26,14 +26,15 @@
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: django
 License-File: LICENSE
 License-File: AUTHORS.md
 
 <pre style="position: relative;color: black;">0000-0010:  89 50 4e 47-0d 0a 1a 0a-00 00 00 0d-49 48 44 52  .PNG.... ....IHDR
 0000-0020:  00 00 04 7b-00 00 04 dc-08 06 00 00-00 14 48 89  ...{.... ......H.
 0000-0030:  b8 00 00 20-00 49 44 41-54 78 9c ec-dd dd 6f 9b  .....IDA Tx....o.
 0000-0040:  e7 79 c7 f1-4b 22 25 ca-2c d9 06 89-e2 84 69 d2  .y..K"%. ,.....i.
```

### Comparing `file_validator-1.0.6/file_validator.egg-info/SOURCES.txt` & `file_validator-1.0.7/file_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.6/setup.cfg` & `file_validator-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.6
+current_version = 1.0.7
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `file_validator-1.0.6/setup.py` & `file_validator-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     "using type, mime, extension, magic numbers and size ✅",
     entry_points={
         "console_scripts": [
             "file_validator=file_validator.cli:main",
         ],
     },
     install_requires=requirements,
+    extras_require={
+        "django": ["django"],
+    },
     license="MIT license",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords=[
         "file_validator",
         "file",
@@ -66,15 +69,15 @@
         "django",
     ],
     name="file_validator",
     packages=find_packages(include=["file_validator", "file_validator.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/file-validator/file-validator",
-    version="1.0.6",
+    version="1.0.7",
     zip_safe=False,
     project_urls={
         "Documentation": "https://file-validator.github.io/",
         "Homepage": "https://github.com/file-validator",
         "Issue tracker": "https://github.com/file-validator/file-validator/issues",
         "Release notes": "https://github.com/file-validator/file-validator/releases",
         "Source": "https://github.com/file-validator/file-validator",
```

