# Comparing `tmp/permhash-0.1.1-py3-none-any.whl.zip` & `tmp/permhash-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15166 bytes, number of entries: 15
+Zip file size: 15094 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 19:45 permhash/__init__.py
 -rw-r--r--  2.0 unx     3107 b- defN 23-May-02 18:27 permhash/functions.py
 -rw-r--r--  2.0 unx    11541 b- defN 23-May-03 15:29 permhash/helpers.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-02 18:28 permhash/scripts/__init__.py
 -rw-r--r--  2.0 unx     1900 b- defN 23-May-02 18:55 permhash/scripts/cli.py
 -rw-r--r--  2.0 unx     1037 b- defN 23-May-02 18:29 permhash/scripts/cli_permhash_apk.py
 -rw-r--r--  2.0 unx     1055 b- defN 23-May-02 18:30 permhash/scripts/cli_permhash_apk_manifest.py
 -rw-r--r--  2.0 unx     1038 b- defN 23-May-02 18:29 permhash/scripts/cli_permhash_crx.py
 -rw-r--r--  2.0 unx     1055 b- defN 23-May-02 18:29 permhash/scripts/cli_permhash_crx_manifest.py
--rw-r--r--  2.0 unx    11358 b- defN 23-May-15 12:50 permhash-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3763 b- defN 23-May-15 12:50 permhash-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 12:50 permhash-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-15 12:50 permhash-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-15 12:50 permhash-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1268 b- defN 23-May-15 12:50 permhash-0.1.1.dist-info/RECORD
-15 files, 37278 bytes uncompressed, 13048 bytes compressed:  65.0%
+-rw-r--r--  2.0 unx    11358 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3400 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1268 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/RECORD
+15 files, 36915 bytes uncompressed, 12976 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: permhash/scripts/cli_permhash_crx.py
 Comment: 
 
 Filename: permhash/scripts/cli_permhash_crx_manifest.py
 Comment: 
 
-Filename: permhash-0.1.1.dist-info/LICENSE
+Filename: permhash-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: permhash-0.1.1.dist-info/METADATA
+Filename: permhash-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: permhash-0.1.1.dist-info/WHEEL
+Filename: permhash-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: permhash-0.1.1.dist-info/entry_points.txt
+Filename: permhash-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: permhash-0.1.1.dist-info/top_level.txt
+Filename: permhash-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: permhash-0.1.1.dist-info/RECORD
+Filename: permhash-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `permhash-0.1.1.dist-info/LICENSE` & `permhash-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `permhash-0.1.1.dist-info/METADATA` & `permhash-0.1.2.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 Metadata-Version: 2.1
 Name: permhash
-Version: 0.1.1
+Version: 0.1.2
 Summary: Permhash calculator
 Author: jaredscottwilson
 License: Google
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: androguard (>=3.3.5)
 Requires-Dist: python-magic (>=0.4.27)
 Requires-Dist: bs4 (>=0.0.1)
 
-![permhash]https://github.com/google/permhash/blob/master/docs/images/logo.png)
-
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/permhash)](https://pypi.org/project/permhash)
-[![Last release](https://img.shields.io/github/v/release/google/permhash)](https://github.com/google/permhash/releases)
-[![Downloads](https://img.shields.io/github/downloads/google/permhash/total)](https://github.com/google/permhash/releases)
-[![License](https://img.shields.io/badge/license-Apache--2.0-green.svg)](LICENSE.txt)
+<img src="https://github.com/google/permhash/blob/59d2c35765cf3b97ce310a3708e1cc8aa839a5a5/docs/images/permhash.jpg" align="center" width="20%" height="20%">
 
 Permhash is an extensible framework to hash the declared permissions applied to Chromium-based browser extensions and APKs allowing for clustering, hunting, and pivoting similar to import hashing and rich header hashing.
 
 Permhash is currently capable of running on four types of files, but is extensible beyond this:
 1. An Android Package (APK) file.
 2. A Chromium-based Extension file (CRX).
 3. An AXML Android Manifest file found at the root directory within APKs.
```

## Comparing `permhash-0.1.1.dist-info/RECORD` & `permhash-0.1.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 permhash/helpers.py,sha256=xVKHwopOx0OCK7ICBkOyw9XzZYZrKeXWeXeKWqY2zbg,11541
 permhash/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 permhash/scripts/cli.py,sha256=iDoO-eH4RDbFSfjWGKb__Sye3EDlu9iV2b0ZKg_uf-o,1900
 permhash/scripts/cli_permhash_apk.py,sha256=HuP9uzuznve8HwKdrZtgrixNQlVxMBD9nJe4UZCpmnA,1037
 permhash/scripts/cli_permhash_apk_manifest.py,sha256=VWn0yfJCCO5A3Nr_JCS5cHijiX-M2FFcnEEviGLQG7Q,1055
 permhash/scripts/cli_permhash_crx.py,sha256=2OYs5lz_XpV00PO9LhXkclY7H4jvOQCZIqlF3ugTzwk,1038
 permhash/scripts/cli_permhash_crx_manifest.py,sha256=s2Og5GVBY-9F8L2G6YgSPuG10c7F2uU_ET5WkirxRTQ,1055
-permhash-0.1.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-permhash-0.1.1.dist-info/METADATA,sha256=W0SqmpAgkQVyCMMfP7YU7s7w-6aR4HrWagzH9LRvaRc,3763
-permhash-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-permhash-0.1.1.dist-info/entry_points.txt,sha256=9G1dFXQGQMLBhcBTgKUejgk-NQabwJb_rnaNZpB5Sns,55
-permhash-0.1.1.dist-info/top_level.txt,sha256=2BTb0jwxoz1xoMPQuNIJdkpy2XQKMysgG3C_zH05XsU,9
-permhash-0.1.1.dist-info/RECORD,,
+permhash-0.1.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+permhash-0.1.2.dist-info/METADATA,sha256=jIJq58R7crJUfLgWfj2TrlZZpVFFjpUIZrcOTF4brPY,3400
+permhash-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+permhash-0.1.2.dist-info/entry_points.txt,sha256=9G1dFXQGQMLBhcBTgKUejgk-NQabwJb_rnaNZpB5Sns,55
+permhash-0.1.2.dist-info/top_level.txt,sha256=2BTb0jwxoz1xoMPQuNIJdkpy2XQKMysgG3C_zH05XsU,9
+permhash-0.1.2.dist-info/RECORD,,
```

