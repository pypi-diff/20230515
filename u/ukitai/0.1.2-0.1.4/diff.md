# Comparing `tmp/ukitai-0.1.2.tar.gz` & `tmp/ukitai-0.1.4.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukitai-0.1.2.tar", last modified: Wed May 19 07:41:34 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

