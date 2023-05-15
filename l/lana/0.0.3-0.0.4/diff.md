# Comparing `tmp/lana-0.0.3-cp39-cp39-macosx_10_7_x86_64.whl.zip` & `tmp/lana-0.0.4-cp37-abi3-macosx_10_7_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 229227 bytes, number of entries: 6
--rw-r--r--  4.6 unx      665 b- defN 23-May-15 16:35 lana-0.0.3.dist-info/METADATA
--rw-r--r--  4.6 unx      104 b- defN 23-May-15 16:35 lana-0.0.3.dist-info/WHEEL
--rw-r--r--  4.6 unx     1060 b- defN 23-May-15 16:35 lana-0.0.3.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx       99 b- defN 23-May-15 16:35 lana/__init__.py
--rwxr-xr-x  4.6 unx   592720 b- defN 23-May-15 16:35 lana/lana.cpython-39-darwin.so
--rw-r--r--  4.6 unx      456 b- defN 23-May-15 16:35 lana-0.0.3.dist-info/RECORD
-6 files, 595104 bytes uncompressed, 228409 bytes compressed:  61.6%
+Zip file size: 396295 bytes, number of entries: 6
+-rw-r--r--  4.6 unx      660 b- defN 23-May-15 19:11 lana-0.0.4.dist-info/METADATA
+-rw-r--r--  4.6 unx      104 b- defN 23-May-15 19:11 lana-0.0.4.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1060 b- defN 23-May-15 19:11 lana-0.0.4.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx       99 b- defN 23-May-15 19:11 lana/__init__.py
+-rwxr-xr-x  4.6 unx  1296456 b- defN 23-May-15 19:11 lana/lana.abi3.so
+-rw-r--r--  4.6 unx      444 b- defN 23-May-15 19:11 lana-0.0.4.dist-info/RECORD
+6 files, 1298823 bytes uncompressed, 395503 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: lana-0.0.3.dist-info/METADATA
+Filename: lana-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: lana-0.0.3.dist-info/WHEEL
+Filename: lana-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: lana-0.0.3.dist-info/license_files/LICENSE
+Filename: lana-0.0.4.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: lana/__init__.py
 Comment: 
 
-Filename: lana/lana.cpython-39-darwin.so
+Filename: lana/lana.abi3.so
 Comment: 
 
-Filename: lana-0.0.3.dist-info/RECORD
+Filename: lana-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lana-0.0.3.dist-info/METADATA` & `lana-0.0.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
-Summary: Blazingly fast linear algebra experiment
+Summary: Linear Algebra experimental library
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/marcosalvalaggio/lana
 
 ## Lana
```

## Comparing `lana-0.0.3.dist-info/license_files/LICENSE` & `lana-0.0.4.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

