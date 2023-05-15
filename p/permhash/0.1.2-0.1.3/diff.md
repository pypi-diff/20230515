# Comparing `tmp/permhash-0.1.2-py3-none-any.whl.zip` & `tmp/permhash-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15094 bytes, number of entries: 15
+Zip file size: 15128 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 19:45 permhash/__init__.py
 -rw-r--r--  2.0 unx     3107 b- defN 23-May-02 18:27 permhash/functions.py
 -rw-r--r--  2.0 unx    11541 b- defN 23-May-03 15:29 permhash/helpers.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-02 18:28 permhash/scripts/__init__.py
 -rw-r--r--  2.0 unx     1900 b- defN 23-May-02 18:55 permhash/scripts/cli.py
 -rw-r--r--  2.0 unx     1037 b- defN 23-May-02 18:29 permhash/scripts/cli_permhash_apk.py
 -rw-r--r--  2.0 unx     1055 b- defN 23-May-02 18:30 permhash/scripts/cli_permhash_apk_manifest.py
 -rw-r--r--  2.0 unx     1038 b- defN 23-May-02 18:29 permhash/scripts/cli_permhash_crx.py
 -rw-r--r--  2.0 unx     1055 b- defN 23-May-02 18:29 permhash/scripts/cli_permhash_crx_manifest.py
--rw-r--r--  2.0 unx    11358 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3400 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1268 b- defN 23-May-15 12:52 permhash-0.1.2.dist-info/RECORD
-15 files, 36915 bytes uncompressed, 12976 bytes compressed:  64.8%
+-rw-r--r--  2.0 unx    11358 b- defN 23-May-15 12:54 permhash-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3465 b- defN 23-May-15 12:54 permhash-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 12:54 permhash-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-May-15 12:54 permhash-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-15 12:54 permhash-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1268 b- defN 23-May-15 12:54 permhash-0.1.3.dist-info/RECORD
+15 files, 36980 bytes uncompressed, 13010 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: permhash/scripts/cli_permhash_crx.py
 Comment: 
 
 Filename: permhash/scripts/cli_permhash_crx_manifest.py
 Comment: 
 
-Filename: permhash-0.1.2.dist-info/LICENSE
+Filename: permhash-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: permhash-0.1.2.dist-info/METADATA
+Filename: permhash-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: permhash-0.1.2.dist-info/WHEEL
+Filename: permhash-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: permhash-0.1.2.dist-info/entry_points.txt
+Filename: permhash-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: permhash-0.1.2.dist-info/top_level.txt
+Filename: permhash-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: permhash-0.1.2.dist-info/RECORD
+Filename: permhash-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `permhash-0.1.2.dist-info/LICENSE` & `permhash-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `permhash-0.1.2.dist-info/METADATA` & `permhash-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permhash
-Version: 0.1.2
+Version: 0.1.3
 Summary: Permhash calculator
 Author: jaredscottwilson
 License: Google
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: androguard (>=3.3.5)
 Requires-Dist: python-magic (>=0.4.27)
@@ -98,14 +98,14 @@
 permhash --type apk --path '[PATH TO APK File]'
 permhash --type apk_manifest --path '[PATH TO APK Manifest Files]'
 ```
 
 
 # Further Information
 ## Permhash
-[Permhash Blog](https://www.mandiant.com/resources/blog/)
+Review the [Mandiant Permhash Blog](https://www.mandiant.com/resources/blog/permhash-no-curls-necessary) for more details.
 
 ## Discussion
 The [Permhash Google Group](https://groups.google.com/g/permhash) can be used to facilitate discussion.
 
 # Disclaimer
 This is not an officially supported Google product.
```

## Comparing `permhash-0.1.2.dist-info/RECORD` & `permhash-0.1.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 permhash/helpers.py,sha256=xVKHwopOx0OCK7ICBkOyw9XzZYZrKeXWeXeKWqY2zbg,11541
 permhash/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 permhash/scripts/cli.py,sha256=iDoO-eH4RDbFSfjWGKb__Sye3EDlu9iV2b0ZKg_uf-o,1900
 permhash/scripts/cli_permhash_apk.py,sha256=HuP9uzuznve8HwKdrZtgrixNQlVxMBD9nJe4UZCpmnA,1037
 permhash/scripts/cli_permhash_apk_manifest.py,sha256=VWn0yfJCCO5A3Nr_JCS5cHijiX-M2FFcnEEviGLQG7Q,1055
 permhash/scripts/cli_permhash_crx.py,sha256=2OYs5lz_XpV00PO9LhXkclY7H4jvOQCZIqlF3ugTzwk,1038
 permhash/scripts/cli_permhash_crx_manifest.py,sha256=s2Og5GVBY-9F8L2G6YgSPuG10c7F2uU_ET5WkirxRTQ,1055
-permhash-0.1.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-permhash-0.1.2.dist-info/METADATA,sha256=jIJq58R7crJUfLgWfj2TrlZZpVFFjpUIZrcOTF4brPY,3400
-permhash-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-permhash-0.1.2.dist-info/entry_points.txt,sha256=9G1dFXQGQMLBhcBTgKUejgk-NQabwJb_rnaNZpB5Sns,55
-permhash-0.1.2.dist-info/top_level.txt,sha256=2BTb0jwxoz1xoMPQuNIJdkpy2XQKMysgG3C_zH05XsU,9
-permhash-0.1.2.dist-info/RECORD,,
+permhash-0.1.3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+permhash-0.1.3.dist-info/METADATA,sha256=Uqzb1jub6YxsbNivRrVLCzGeYVbzp0w0ToUNV71betg,3465
+permhash-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+permhash-0.1.3.dist-info/entry_points.txt,sha256=9G1dFXQGQMLBhcBTgKUejgk-NQabwJb_rnaNZpB5Sns,55
+permhash-0.1.3.dist-info/top_level.txt,sha256=2BTb0jwxoz1xoMPQuNIJdkpy2XQKMysgG3C_zH05XsU,9
+permhash-0.1.3.dist-info/RECORD,,
```

