# Comparing `tmp/hellomodule2-1.0.tar.gz` & `tmp/hellomodule2-2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hellomodule2-1.0.tar", last modified: Mon May 15 16:21:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

