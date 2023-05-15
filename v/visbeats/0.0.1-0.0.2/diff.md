# Comparing `tmp/visbeats-0.0.1.tar.gz` & `tmp/visbeats-0.0.2-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visbeats-0.0.1.tar", last modified: Mon May 15 15:38:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

