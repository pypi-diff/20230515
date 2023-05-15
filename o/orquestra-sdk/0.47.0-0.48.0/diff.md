# Comparing `tmp/orquestra-sdk-0.47.0.tar.gz` & `tmp/orquestra_sdk-0.48.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orquestra-sdk-0.47.0.tar", last modified: Fri Apr 28 13:27:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

