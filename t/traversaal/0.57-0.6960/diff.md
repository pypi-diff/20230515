# Comparing `tmp/traversaal-0.57-py3-none-any.whl.zip` & `tmp/traversaal-0.6960-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2653 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1059 b- defN 23-May-14 16:51 traversaal-0.57.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1893 b- defN 23-May-14 16:51 traversaal-0.57.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-14 16:51 traversaal-0.57.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-14 16:51 traversaal-0.57.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      399 b- defN 23-May-14 16:51 traversaal-0.57.dist-info/RECORD
-5 files, 3444 bytes uncompressed, 1905 bytes compressed:  44.7%
+Zip file size: 2866 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     1059 b- defN 23-May-14 21:48 traversaal-0.6960.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-14 21:48 traversaal-0.6960.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 21:48 traversaal-0.6960.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-14 21:48 traversaal-0.6960.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      409 b- defN 23-May-14 21:48 traversaal-0.6960.dist-info/RECORD
+5 files, 3829 bytes uncompressed, 2098 bytes compressed:  45.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: traversaal-0.57.dist-info/LICENSE.txt
+Filename: traversaal-0.6960.dist-info/LICENSE.txt
 Comment: 
 
-Filename: traversaal-0.57.dist-info/METADATA
+Filename: traversaal-0.6960.dist-info/METADATA
 Comment: 
 
-Filename: traversaal-0.57.dist-info/WHEEL
+Filename: traversaal-0.6960.dist-info/WHEEL
 Comment: 
 
-Filename: traversaal-0.57.dist-info/top_level.txt
+Filename: traversaal-0.6960.dist-info/top_level.txt
 Comment: 
 
-Filename: traversaal-0.57.dist-info/RECORD
+Filename: traversaal-0.6960.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `traversaal-0.57.dist-info/LICENSE.txt` & `traversaal-0.6960.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `traversaal-0.57.dist-info/METADATA` & `traversaal-0.6960.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: traversaal
-Version: 0.57
+Version: 0.6960
 Summary: A semantic search package for hotel data
 Home-page: https://github.com/hamzafarooq
 Author: Traversaal
 Author-email: hello@traversaal.com
 License: MIT
+Keywords: Transformer Networks BERT XLNet sentence embedding PyTorch NLP deep learning
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: torch
-Requires-Dist: transformers
-Requires-Dist: flask
-Requires-Dist: openai
-Requires-Dist: langchain
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: nltk
 
 ## Traversaal
 
 Traversaal is a Python package that provides a simple semantic search functionality for hotel data. It leverages large language models such as BERT to encode hotel descriptions and reviews, allowing users to perform semantic search queries and retrieve relevant results based on the provided search query.
 
 ## Features
```

