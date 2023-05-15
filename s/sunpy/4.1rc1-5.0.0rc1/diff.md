# Comparing `tmp/sunpy-4.1rc1.tar.gz` & `tmp/sunpy-5.0.0rc1-cp39-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunpy-4.1rc1.tar", last modified: Fri Nov  4 18:24:17 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

