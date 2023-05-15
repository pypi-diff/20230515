# Comparing `tmp/pyqrack-1.9.3.tar.gz` & `tmp/pyqrack-1.9.4-py3-none-manylinux_2_35_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqrack-1.9.3.tar", last modified: Sun May 14 13:46:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

