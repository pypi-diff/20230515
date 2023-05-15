# Comparing `tmp/pydivsufsort-0.0.8.tar.gz` & `tmp/pydivsufsort-0.0.9-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivsufsort-0.0.8.tar", last modified: Sat May 13 15:53:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

