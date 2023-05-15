# Comparing `tmp/themis_imager_readfile-1.1.1.tar.gz` & `tmp/themis_imager_readfile-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themis_imager_readfile-1.1.1.tar", max compression
+gzip compressed data, was "themis_imager_readfile-1.1.2.tar", max compression
```

## Comparing `themis_imager_readfile-1.1.1.tar` & `themis_imager_readfile-1.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.1.1/LICENSE
--rw-r--r--   0        0        0     2475 2023-05-04 21:32:07.373602 themis_imager_readfile-1.1.1/README.md
--rw-r--r--   0        0        0      666 2023-05-05 13:23:43.203365 themis_imager_readfile-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       49 2023-05-05 13:23:43.230366 themis_imager_readfile-1.1.1/themis_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8458 2021-11-17 16:36:55.000000 themis_imager_readfile-1.1.1/themis_imager_readfile/_themis.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 themis_imager_readfile-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2763 2023-05-15 18:17:56.997619 themis_imager_readfile-1.1.2/README.md
+-rw-r--r--   0        0        0      666 2023-05-15 18:09:11.715955 themis_imager_readfile-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-05-15 18:09:11.747955 themis_imager_readfile-1.1.2/themis_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8501 2023-05-15 18:10:02.283981 themis_imager_readfile-1.1.2/themis_imager_readfile/_themis.py
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 themis_imager_readfile-1.1.2/PKG-INFO
```

### Comparing `themis_imager_readfile-1.1.1/LICENSE` & `themis_imager_readfile-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.1.1/README.md` & `themis_imager_readfile-1.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import themis_imager_readfile`
 
+**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
+
 ### Read a single file
 
 ```python
 >>> import themis_imager_readfile
 >>> filename = "path/to/data/2020/01/01/atha_themis02/ut06/20200101_0600_atha_themis02_full.pgm.gz"
 >>> img, meta, problematic_files = themis_imager_readfile.read(filename)
 ```
```

### Comparing `themis_imager_readfile-1.1.1/pyproject.toml` & `themis_imager_readfile-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "themis-imager-readfile"
-version = "1.1.1"
+version = "1.1.2"
 description = "Read functions for THEMIS ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `themis_imager_readfile-1.1.1/themis_imager_readfile/_themis.py` & `themis_imager_readfile-1.1.2/themis_imager_readfile/_themis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Author: Lukas Vollmerhaus
 # Date: 2020-10-16
 
 import gzip
 import bz2
 import numpy as np
 import signal
-from multiprocessing import Pool
+import multiprocessing
 
 # globals
 THEMIS_IMAGE_SIZE_BYTES = 131072
 THEMIS_DT = np.dtype("uint16")
 THEMIS_DT = THEMIS_DT.newbyteorder('>')  # force big endian byte ordering
 THEMIS_EXPECTED_MINUTE_NUM_FRAMES = 20
 
@@ -23,16 +23,17 @@
     :param workers: number of worker processes to spawn, defaults to 1
     :type workers: int, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
     # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
+    multiprocessing.freeze_support()
     original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    pool = Pool(processes=workers)
+    pool = multiprocessing.Pool(processes=workers)
     signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
 
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
     # call readfile function, run each iteration with a single input file from file_list
```

### Comparing `themis_imager_readfile-1.1.1/PKG-INFO` & `themis_imager_readfile-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themis-imager-readfile
-Version: 1.1.1
+Version: 1.1.2
 Summary: Read functions for THEMIS ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/themis-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,16 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import themis_imager_readfile`
 
+**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
+
 ### Read a single file
 
 ```python
 >>> import themis_imager_readfile
 >>> filename = "path/to/data/2020/01/01/atha_themis02/ut06/20200101_0600_atha_themis02_full.pgm.gz"
 >>> img, meta, problematic_files = themis_imager_readfile.read(filename)
 ```
```

