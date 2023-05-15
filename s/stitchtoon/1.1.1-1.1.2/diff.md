# Comparing `tmp/stitchtoon-1.1.1.tar.gz` & `tmp/stitchtoon-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stitchtoon-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "stitchtoon-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `stitchtoon-1.1.1.tar` & `stitchtoon-1.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      431 2023-05-07 16:26:35.000000 stitchtoon-1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      131 2023-05-15 03:14:37.433657 stitchtoon-1.1.1/.gitignore
--rw-r--r--   0        0        0     1091 2023-05-15 03:14:37.433657 stitchtoon-1.1.1/LICENSE
--rw-r--r--   0        0        0      603 2023-04-26 07:52:39.000000 stitchtoon-1.1.1/Makefile
--rw-r--r--   0        0        0      376 2023-05-15 03:14:37.434656 stitchtoon-1.1.1/Pipfile
--rw-r--r--   0        0        0    36902 2023-04-28 10:37:12.000000 stitchtoon-1.1.1/Pipfile.lock
--rw-r--r--   0        0        0     3099 2023-05-15 03:14:37.434656 stitchtoon-1.1.1/README.md
--rw-r--r--   0        0        0       98 2023-05-11 11:01:07.250980 stitchtoon-1.1.1/TODO
--rw-r--r--   0        0        0      128 2023-05-15 03:14:37.436654 stitchtoon-1.1.1/pre-commit.sh
--rw-r--r--   0        0        0     1234 2023-05-15 03:27:37.039760 stitchtoon-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      613 2023-05-15 03:14:37.437654 stitchtoon-1.1.1/requirements.txt
--rw-r--r--   0        0        0      817 2023-05-15 03:14:37.440158 stitchtoon-1.1.1/setup.cfg
--rw-r--r--   0        0        0      125 2023-05-15 03:14:37.437654 stitchtoon-1.1.1/setup.py
--rw-r--r--   0        0        0     1883 2023-05-15 03:21:20.328929 stitchtoon-1.1.1/src/stitchtoon/__init__.py
--rw-r--r--   0        0        0     6364 2023-05-15 03:14:37.439653 stitchtoon-1.1.1/src/stitchtoon/__main__.py
--rw-r--r--   0        0        0      224 2023-05-15 03:14:37.442169 stitchtoon-1.1.1/src/stitchtoon/detectors/__init__.py
--rw-r--r--   0        0        0      832 2023-05-15 03:14:37.441164 stitchtoon-1.1.1/src/stitchtoon/detectors/direct_slicing.py
--rw-r--r--   0        0        0     2189 2023-05-15 03:14:37.443168 stitchtoon-1.1.1/src/stitchtoon/detectors/pixel_comparison.py
--rw-r--r--   0        0        0      537 2023-05-15 03:14:37.442169 stitchtoon-1.1.1/src/stitchtoon/detectors/selector.py
--rw-r--r--   0        0        0      457 2023-05-15 03:14:37.443168 stitchtoon-1.1.1/src/stitchtoon/services/__init__.py
--rw-r--r--   0        0        0     1629 2023-05-15 03:14:37.446165 stitchtoon-1.1.1/src/stitchtoon/services/global_logger.py
--rw-r--r--   0        0        0     2298 2023-05-15 03:14:37.445166 stitchtoon-1.1.1/src/stitchtoon/services/image_directory.py
--rw-r--r--   0        0        0     3564 2023-05-15 03:14:37.445166 stitchtoon-1.1.1/src/stitchtoon/services/image_handler.py
--rw-r--r--   0        0        0     4385 2023-05-15 03:14:37.448165 stitchtoon-1.1.1/src/stitchtoon/services/image_manipulator.py
--rw-r--r--   0        0        0      773 2023-05-15 03:14:37.448165 stitchtoon-1.1.1/src/stitchtoon/services/postprocess_runner.py
--rw-r--r--   0        0        0     8672 2023-05-15 03:14:37.448165 stitchtoon-1.1.1/src/stitchtoon/services/process.py
--rw-r--r--   0        0        0     1009 2023-05-07 16:10:22.000000 stitchtoon-1.1.1/src/stitchtoon/services/progressbar.py
--rw-r--r--   0        0        0     3148 2023-05-15 03:14:37.449671 stitchtoon-1.1.1/src/stitchtoon/services/scanner.py
--rw-r--r--   0        0        0        0 2023-05-15 03:14:37.449671 stitchtoon-1.1.1/src/stitchtoon/utils/__init__.py
--rw-r--r--   0        0        0     1267 2023-05-15 03:14:37.450700 stitchtoon-1.1.1/src/stitchtoon/utils/constants.py
--rw-r--r--   0        0        0      144 2023-05-15 03:14:37.451704 stitchtoon-1.1.1/src/stitchtoon/utils/errors.py
--rw-r--r--   0        0        0      470 2023-05-15 03:14:37.452703 stitchtoon-1.1.1/src/stitchtoon/utils/funcs.py
--rw-r--r--   0        0        0      867 2023-05-15 03:14:37.452703 stitchtoon-1.1.1/stitchtoon.spec
--rw-r--r--   0        0        0        0 2023-04-26 07:52:39.000000 stitchtoon-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0   138180 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/01.jpeg
--rw-r--r--   0        0        0  1726886 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/01.webp
--rw-r--r--   0        0        0   141943 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/02.jpeg
--rw-r--r--   0        0        0   123745 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/03.jpeg
--rw-r--r--   0        0        0   142053 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/data/04.jpeg
--rw-r--r--   0        0        0     1117 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/test_manipulator.py
--rw-r--r--   0        0        0     1101 2023-05-07 16:35:32.000000 stitchtoon-1.1.1/tests/test/test_scan.py
--rw-r--r--   0        0        0      284 2023-04-28 22:41:33.000000 stitchtoon-1.1.1/tox.ini
--rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 stitchtoon-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      431 2023-05-07 16:26:35.000000 stitchtoon-1.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      131 2023-05-15 05:57:41.297529 stitchtoon-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1091 2023-05-15 05:57:41.297529 stitchtoon-1.1.2/LICENSE
+-rw-r--r--   0        0        0      603 2023-04-26 07:52:39.000000 stitchtoon-1.1.2/Makefile
+-rw-r--r--   0        0        0      376 2023-05-15 05:57:41.297529 stitchtoon-1.1.2/Pipfile
+-rw-r--r--   0        0        0    36902 2023-04-28 10:37:12.000000 stitchtoon-1.1.2/Pipfile.lock
+-rw-r--r--   0        0        0     3099 2023-05-15 05:57:41.298529 stitchtoon-1.1.2/README.md
+-rw-r--r--   0        0        0       98 2023-05-11 11:01:07.250980 stitchtoon-1.1.2/TODO
+-rw-r--r--   0        0        0      128 2023-05-15 05:57:41.299527 stitchtoon-1.1.2/pre-commit.sh
+-rw-r--r--   0        0        0     1234 2023-05-15 05:54:55.399524 stitchtoon-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      613 2023-05-15 05:57:41.300526 stitchtoon-1.1.2/requirements.txt
+-rw-r--r--   0        0        0      817 2023-05-15 05:57:41.299527 stitchtoon-1.1.2/setup.cfg
+-rw-r--r--   0        0        0      125 2023-05-15 05:57:41.300526 stitchtoon-1.1.2/setup.py
+-rw-r--r--   0        0        0     1883 2023-05-15 06:01:23.849355 stitchtoon-1.1.2/src/stitchtoon/__init__.py
+-rw-r--r--   0        0        0     6364 2023-05-15 05:57:41.302526 stitchtoon-1.1.2/src/stitchtoon/__main__.py
+-rw-r--r--   0        0        0      224 2023-05-15 05:57:41.302526 stitchtoon-1.1.2/src/stitchtoon/detectors/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-15 05:57:41.302526 stitchtoon-1.1.2/src/stitchtoon/detectors/direct_slicing.py
+-rw-r--r--   0        0        0     2189 2023-05-15 05:57:41.303525 stitchtoon-1.1.2/src/stitchtoon/detectors/pixel_comparison.py
+-rw-r--r--   0        0        0      537 2023-05-15 05:57:41.304525 stitchtoon-1.1.2/src/stitchtoon/detectors/selector.py
+-rw-r--r--   0        0        0      457 2023-05-15 05:57:41.304525 stitchtoon-1.1.2/src/stitchtoon/services/__init__.py
+-rw-r--r--   0        0        0     1690 2023-05-15 05:17:33.638749 stitchtoon-1.1.2/src/stitchtoon/services/global_logger.py
+-rw-r--r--   0        0        0     2298 2023-05-15 05:57:41.305523 stitchtoon-1.1.2/src/stitchtoon/services/image_directory.py
+-rw-r--r--   0        0        0     3564 2023-05-15 05:57:41.305523 stitchtoon-1.1.2/src/stitchtoon/services/image_handler.py
+-rw-r--r--   0        0        0     4454 2023-05-15 05:42:27.284509 stitchtoon-1.1.2/src/stitchtoon/services/image_manipulator.py
+-rw-r--r--   0        0        0      773 2023-05-15 05:57:41.306523 stitchtoon-1.1.2/src/stitchtoon/services/postprocess_runner.py
+-rw-r--r--   0        0        0     8672 2023-05-15 05:57:41.307522 stitchtoon-1.1.2/src/stitchtoon/services/process.py
+-rw-r--r--   0        0        0     1009 2023-05-07 16:10:22.000000 stitchtoon-1.1.2/src/stitchtoon/services/progressbar.py
+-rw-r--r--   0        0        0     3148 2023-05-15 05:57:41.307522 stitchtoon-1.1.2/src/stitchtoon/services/scanner.py
+-rw-r--r--   0        0        0        0 2023-05-15 05:57:41.306523 stitchtoon-1.1.2/src/stitchtoon/utils/__init__.py
+-rw-r--r--   0        0        0     1275 2023-05-15 05:47:18.302075 stitchtoon-1.1.2/src/stitchtoon/utils/constants.py
+-rw-r--r--   0        0        0      144 2023-05-15 05:57:41.309521 stitchtoon-1.1.2/src/stitchtoon/utils/errors.py
+-rw-r--r--   0        0        0      470 2023-05-15 05:57:41.309521 stitchtoon-1.1.2/src/stitchtoon/utils/funcs.py
+-rw-r--r--   0        0        0      867 2023-05-15 05:57:41.309521 stitchtoon-1.1.2/stitchtoon.spec
+-rw-r--r--   0        0        0        0 2023-04-26 07:52:39.000000 stitchtoon-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0   138180 2023-05-07 16:35:32.000000 stitchtoon-1.1.2/tests/test/data/01.jpeg
+-rw-r--r--   0        0        0  1726886 2023-05-07 16:35:32.000000 stitchtoon-1.1.2/tests/test/data/01.webp
+-rw-r--r--   0        0        0   141943 2023-05-07 16:35:32.000000 stitchtoon-1.1.2/tests/test/data/02.jpeg
+-rw-r--r--   0        0        0   123745 2023-05-07 16:35:32.000000 stitchtoon-1.1.2/tests/test/data/03.jpeg
+-rw-r--r--   0        0        0   142053 2023-05-07 16:35:32.000000 stitchtoon-1.1.2/tests/test/data/04.jpeg
+-rw-r--r--   0        0        0     1117 2023-05-07 16:35:32.000000 stitchtoon-1.1.2/tests/test/test_manipulator.py
+-rw-r--r--   0        0        0     1101 2023-05-07 16:35:32.000000 stitchtoon-1.1.2/tests/test/test_scan.py
+-rw-r--r--   0        0        0      284 2023-04-28 22:41:33.000000 stitchtoon-1.1.2/tox.ini
+-rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 stitchtoon-1.1.2/PKG-INFO
```

### Comparing `stitchtoon-1.1.1/LICENSE` & `stitchtoon-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/Makefile` & `stitchtoon-1.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/Pipfile.lock` & `stitchtoon-1.1.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/README.md` & `stitchtoon-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/pyproject.toml` & `stitchtoon-1.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stitchtoon"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Beshr Alghalil", email="beshrghalil@protonmail.com" },
 ]
 description = "A powerful program for stitching and cutting webtoons/manhwa/manhua raws."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["manga", "webtoon", "stitch", "slice", "combin"]
```

### Comparing `stitchtoon-1.1.1/requirements.txt` & `stitchtoon-1.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/setup.cfg` & `stitchtoon-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/__init__.py` & `stitchtoon-1.1.2/src/stitchtoon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         except (OSError, subprocess.CalledProcessError, AttributeError):
             version_string = version_string.format(__version__)
     return version_string
 
 
 # Information
 __license__ = "MIT"
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 __release__ = False
 __author__ = __maintainer__ = "Beshr Ghalil"
 __email__ = "beshrghalil@porotonmail.com"
 
 # Constants
 stitchtoon = os.path.dirname(__file__)
 DEFAULT_PAGER = "less"
```

### Comparing `stitchtoon-1.1.1/src/stitchtoon/__main__.py` & `stitchtoon-1.1.2/src/stitchtoon/__main__.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/detectors/direct_slicing.py` & `stitchtoon-1.1.2/src/stitchtoon/detectors/direct_slicing.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/detectors/pixel_comparison.py` & `stitchtoon-1.1.2/src/stitchtoon/detectors/pixel_comparison.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/detectors/selector.py` & `stitchtoon-1.1.2/src/stitchtoon/detectors/selector.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/services/global_logger.py` & `stitchtoon-1.1.2/src/stitchtoon/services/global_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     logger.setLevel(log_level)
     log_format = "%(name)s:%(levelname)s:%(asctime)s:%(message)s"
     logging.basicConfig(format=log_format)
     if isinstance(filename, str):
         current_date = datetime.now()
         filename = current_date.strftime(filename)
         handler = logging.FileHandler(filename, mode="w")
+        handler.setFormatter(logging.Formatter(log_format))
         logger.addHandler(handler)
 
     logger.debug("Logger Initialized")
     # Removes the pil logging from polluting the Debug Level.
     pil_logger = logging.getLogger("PIL")
     pil_logger.setLevel(logging.INFO)
     return logger
```

### Comparing `stitchtoon-1.1.1/src/stitchtoon/services/image_directory.py` & `stitchtoon-1.1.2/src/stitchtoon/services/image_directory.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/services/image_handler.py` & `stitchtoon-1.1.2/src/stitchtoon/services/image_handler.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/services/image_manipulator.py` & `stitchtoon-1.1.2/src/stitchtoon/services/image_manipulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,16 @@
         """
 
         max_width = combined_img.width
         img_objs = []
         for index in range(1, len(slice_locations)):
             upper_limit = slice_locations[index - 1]
             lower_limit = slice_locations[index]
+            if lower_limit < upper_limit:
+                continue
             slice_boundaries = (0, upper_limit, max_width, lower_limit)
             try:
                 img_slice = combined_img.pil.crop(slice_boundaries)
             except ValueError:
                 raise SizeLimitError("Images to small to slice")
             img = combined_img.copy()
             img.pil = img_slice
```

### Comparing `stitchtoon-1.1.1/src/stitchtoon/services/postprocess_runner.py` & `stitchtoon-1.1.2/src/stitchtoon/services/postprocess_runner.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/services/process.py` & `stitchtoon-1.1.2/src/stitchtoon/services/process.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/services/progressbar.py` & `stitchtoon-1.1.2/src/stitchtoon/services/progressbar.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/services/scanner.py` & `stitchtoon-1.1.2/src/stitchtoon/services/scanner.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/src/stitchtoon/utils/constants.py` & `stitchtoon-1.1.2/src/stitchtoon/utils/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "webp": 16_383,
     "png": 300_000,
     "psd": 30_000,
     "psb": 300_000,
 }
 
 PHOTOSHOP_FILE_TYPES = ("psd", "psb")
-SUPPORTS_TRANSPARENCY = ("png", "psd", "psb")
+SUPPORTS_TRANSPARENCY = ("png", "webp", "psd", "psb")
 
 
 # Static Enums
 class WIDTH_ENFORCEMENT(Enum):
     NONE = "none"
     AUTO = "auto"
     FIXED = "fixed"
```

### Comparing `stitchtoon-1.1.1/stitchtoon.spec` & `stitchtoon-1.1.2/stitchtoon.spec`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/tests/test/data/01.jpeg` & `stitchtoon-1.1.2/tests/test/data/01.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/tests/test/data/01.webp` & `stitchtoon-1.1.2/tests/test/data/01.webp`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/tests/test/data/02.jpeg` & `stitchtoon-1.1.2/tests/test/data/02.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/tests/test/data/03.jpeg` & `stitchtoon-1.1.2/tests/test/data/03.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/tests/test/data/04.jpeg` & `stitchtoon-1.1.2/tests/test/data/04.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/tests/test/test_manipulator.py` & `stitchtoon-1.1.2/tests/test/test_manipulator.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/tests/test/test_scan.py` & `stitchtoon-1.1.2/tests/test/test_scan.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.1.1/PKG-INFO` & `stitchtoon-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stitchtoon
-Version: 1.1.1
+Version: 1.1.2
 Summary: A powerful program for stitching and cutting webtoons/manhwa/manhua raws.
 Keywords: manga,webtoon,stitch,slice,combin
 Author-email: Beshr Alghalil <beshrghalil@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stitchtoon Version: 1.1.1 Summary: A powerful
+Metadata-Version: 2.1 Name: stitchtoon Version: 1.1.2 Summary: A powerful
 program for stitching and cutting webtoons/manhwa/manhua raws. Keywords:
 manga,webtoon,stitch,slice,combin Author-email: Beshr Alghalil
 protonmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Dist: psd_tools Requires-Dist: natsort Requires-Dist: pillow Requires-
 Dist: progress Requires-Dist: black ; extra == "dev" Requires-Dist: flake8 ;
```

