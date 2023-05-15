# Comparing `tmp/smartdns-3.5.1.tar.gz` & `tmp/smartdns-3.6.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdns-3.5.1.tar", last modified: Mon Nov 15 05:47:01 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

