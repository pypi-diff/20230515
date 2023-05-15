# Comparing `tmp/excel-dates-0.1.1.tar.gz` & `tmp/excel_dates-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-dates-0.1.1.tar", last modified: Mon Nov 29 20:30:12 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

