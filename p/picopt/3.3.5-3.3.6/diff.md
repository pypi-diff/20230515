# Comparing `tmp/picopt-3.3.5.tar.gz` & `tmp/picopt-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopt-3.3.5.tar", max compression
+gzip compressed data, was "picopt-3.3.6.tar", max compression
```

## Comparing `picopt-3.3.5.tar` & `picopt-3.3.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     7482 2023-05-13 22:37:07.993212 picopt-3.3.5/README.md
--rw-r--r--   0        0        0       64 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/__init__.py
--rw-r--r--   0        0        0     7124 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/cli.py
--rw-r--r--   0        0        0    14506 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/config.py
--rw-r--r--   0        0        0      286 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/config_default.yaml
--rw-r--r--   0        0        0      457 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/configurable.py
--rw-r--r--   0        0        0      501 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/data.py
--rw-r--r--   0        0        0       25 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/handlers/__init__.py
--rw-r--r--   0        0        0     3478 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/handlers/container.py
--rw-r--r--   0        0        0     5508 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/handlers/factory.py
--rw-r--r--   0        0        0     1360 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/handlers/gif.py
--rw-r--r--   0        0        0     6071 2023-05-13 22:37:07.997212 picopt-3.3.5/picopt/handlers/handler.py
--rw-r--r--   0        0        0     2988 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/handlers/image.py
--rw-r--r--   0        0        0     1875 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/handlers/jpeg.py
--rw-r--r--   0        0        0     1902 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/handlers/png.py
--rw-r--r--   0        0        0     4299 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/handlers/webp.py
--rw-r--r--   0        0        0     4468 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/handlers/webp_animated.py
--rw-r--r--   0        0        0     4047 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/handlers/zip.py
--rw-r--r--   0        0        0     2276 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/old_timestamps.py
--rw-r--r--   0        0        0       22 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/pillow/__init__.py
--rw-r--r--   0        0        0      777 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/pillow/header.py
--rwxr-xr-x   0        0        0     1052 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/pillow/png_bit_depth.py
--rwxr-xr-x   0        0        0      996 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/pillow/webp_lossless.py
--rw-r--r--   0        0        0     2599 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/stats.py
--rw-r--r--   0        0        0    15817 2023-05-13 22:37:08.001213 picopt-3.3.5/picopt/walk.py
--rw-r--r--   0        0        0     4173 2023-05-13 22:37:08.001213 picopt-3.3.5/pyproject.toml
--rw-r--r--   0        0        0      560 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/__init__.py
--rw-r--r--   0        0        0       22 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/integration/__init__.py
--rw-r--r--   0        0        0     2813 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/integration/test_containers.py
--rw-r--r--   0        0        0     4447 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/integration/test_images_dir.py
--rw-r--r--   0        0        0     2454 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/integration/test_old_timestamps.py
--rw-r--r--   0        0        0     1140 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/integration/test_one_container.py
--rw-r--r--   0        0        0     5084 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/integration/test_timestamps.py
--rw-r--r--   0        0        0   292448 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/test_files/containers/igp-twss.epub
--rw-r--r--   0        0        0    93725 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/test_files/containers/test_cbr.cbr
--rw-r--r--   0        0        0    93408 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/test_files/containers/test_cbz.cbz
--rw-r--r--   0        0        0    93675 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/test_files/containers/test_rar.rar
--rw-r--r--   0        0        0     2974 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/test_files/containers/test_zip.zip
--rw-r--r--   0        0        0    93676 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/test_files/images/07themecamplist.pdf
--rw-r--r--   0        0        0    59640 2023-05-13 22:37:08.001213 picopt-3.3.5/tests/test_files/images/eight.tif
--rw-r--r--   0        0        0   230578 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/mri.tif
--rw-r--r--   0        0        0    16383 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_animated_gif.gif
--rw-r--r--   0        0        0    63435 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_animated_png.png
--rw-r--r--   0        0        0    13610 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_animated_webp.webp
--rw-r--r--   0        0        0   141430 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_bmp.bmp
--rw-r--r--   0        0        0   138952 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_gif.gif
--rw-r--r--   0        0        0    97373 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_jpg.jpg
--rw-r--r--   0        0        0     7967 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_png.png
--rw-r--r--   0        0        0     3435 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_png_16rgba.png
--rw-r--r--   0        0        0    27661 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_pnm.pnm
--rw-r--r--   0        0        0    22664 2023-05-13 22:37:08.005213 picopt-3.3.5/tests/test_files/images/test_pre-optimized_jpg.jpg
--rw-r--r--   0        0        0   256572 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/images/test_pre-optimized_png.png
--rw-r--r--   0        0        0        6 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/images/test_txt.txt
--rw-r--r--   0        0        0     5334 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/images/test_webp_lossless.webp
--rw-r--r--   0        0        0     8914 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/images/test_webp_lossless_pre-optimized.webp
--rw-r--r--   0        0        0     2764 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/images/test_webp_lossy.webp
--rw-r--r--   0        0        0     1508 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/images/test_webp_lossy_pre-optimized.webp
--rw-r--r--   0        0        0        3 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/invalid/test_invalid_cbr.cbr
--rw-r--r--   0        0        0        3 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/invalid/test_invalid_cbz.cbz
--rw-r--r--   0        0        0        0 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/invalid/test_invalid_gif.gif
--rw-r--r--   0        0        0        0 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/invalid/test_invalid_jpg.jpg
--rw-r--r--   0        0        0        0 2023-05-13 22:37:08.009214 picopt-3.3.5/tests/test_files/invalid/test_invalid_png.png
--rw-r--r--   0        0        0   879952 2023-05-13 22:37:08.013214 picopt-3.3.5/tests/test_files/invalid/test_mpeg.mpeg
--rw-r--r--   0        0        0       80 2023-05-13 22:37:08.013214 picopt-3.3.5/tests/test_files/invalid/test_rar.rar
--rw-r--r--   0        0        0      167 2023-05-13 22:37:08.013214 picopt-3.3.5/tests/test_files/invalid/test_zip.zip
--rw-r--r--   0        0        0       18 2023-05-13 22:37:08.013214 picopt-3.3.5/tests/unit/__init__.py
--rw-r--r--   0        0        0     1923 2023-05-13 22:37:08.013214 picopt-3.3.5/tests/unit/test_cli.py
--rw-r--r--   0        0        0      871 2023-05-13 22:37:08.013214 picopt-3.3.5/tests/unit/test_png_bit_depth.py
--rw-r--r--   0        0        0     9059 1970-01-01 00:00:00.000000 picopt-3.3.5/PKG-INFO
+-rw-r--r--   0        0        0     7482 2023-05-14 22:59:15.318081 picopt-3.3.6/README.md
+-rw-r--r--   0        0        0       64 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/__init__.py
+-rw-r--r--   0        0        0     7120 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/cli.py
+-rw-r--r--   0        0        0    14510 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/config.py
+-rw-r--r--   0        0        0      286 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/config_default.yaml
+-rw-r--r--   0        0        0      457 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/configurable.py
+-rw-r--r--   0        0        0      501 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/data.py
+-rw-r--r--   0        0        0       25 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/__init__.py
+-rw-r--r--   0        0        0     3478 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/container.py
+-rw-r--r--   0        0        0     5528 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/factory.py
+-rw-r--r--   0        0        0     1360 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/gif.py
+-rw-r--r--   0        0        0     6071 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/handler.py
+-rw-r--r--   0        0        0     2988 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/image.py
+-rw-r--r--   0        0        0     1875 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/jpeg.py
+-rw-r--r--   0        0        0     1902 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/png.py
+-rw-r--r--   0        0        0     4299 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/webp.py
+-rw-r--r--   0        0        0     4468 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/webp_animated.py
+-rw-r--r--   0        0        0     4818 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/handlers/zip.py
+-rw-r--r--   0        0        0     2276 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/old_timestamps.py
+-rw-r--r--   0        0        0       22 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/pillow/__init__.py
+-rw-r--r--   0        0        0      777 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/pillow/header.py
+-rwxr-xr-x   0        0        0     1052 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/pillow/png_bit_depth.py
+-rwxr-xr-x   0        0        0      996 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/pillow/webp_lossless.py
+-rw-r--r--   0        0        0     2596 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/stats.py
+-rw-r--r--   0        0        0    15809 2023-05-14 22:59:15.326082 picopt-3.3.6/picopt/walk.py
+-rw-r--r--   0        0        0     4210 2023-05-14 22:59:15.326082 picopt-3.3.6/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2813 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/integration/test_containers.py
+-rw-r--r--   0        0        0     4447 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/integration/test_images_dir.py
+-rw-r--r--   0        0        0     2454 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/integration/test_old_timestamps.py
+-rw-r--r--   0        0        0     1140 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/integration/test_one_container.py
+-rw-r--r--   0        0        0     5084 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/integration/test_timestamps.py
+-rw-r--r--   0        0        0   292448 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/test_files/containers/igp-twss.epub
+-rw-r--r--   0        0        0    93725 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/test_files/containers/test_cbr.cbr
+-rw-r--r--   0        0        0    93408 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/test_files/containers/test_cbz.cbz
+-rw-r--r--   0        0        0    93675 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/test_files/containers/test_rar.rar
+-rw-r--r--   0        0        0     2974 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/test_files/containers/test_zip.zip
+-rw-r--r--   0        0        0    93676 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/test_files/images/07themecamplist.pdf
+-rw-r--r--   0        0        0    59640 2023-05-14 22:59:15.326082 picopt-3.3.6/tests/test_files/images/eight.tif
+-rw-r--r--   0        0        0   230578 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/mri.tif
+-rw-r--r--   0        0        0    16383 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_animated_gif.gif
+-rw-r--r--   0        0        0    63435 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_animated_png.png
+-rw-r--r--   0        0        0    13610 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_animated_webp.webp
+-rw-r--r--   0        0        0   141430 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_bmp.bmp
+-rw-r--r--   0        0        0   138952 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_gif.gif
+-rw-r--r--   0        0        0    97373 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_jpg.jpg
+-rw-r--r--   0        0        0     7967 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_png.png
+-rw-r--r--   0        0        0     3435 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_png_16rgba.png
+-rw-r--r--   0        0        0    27661 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_pnm.pnm
+-rw-r--r--   0        0        0    22664 2023-05-14 22:59:15.330082 picopt-3.3.6/tests/test_files/images/test_pre-optimized_jpg.jpg
+-rw-r--r--   0        0        0   256572 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/images/test_pre-optimized_png.png
+-rw-r--r--   0        0        0        6 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/images/test_txt.txt
+-rw-r--r--   0        0        0     5334 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/images/test_webp_lossless.webp
+-rw-r--r--   0        0        0     8914 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/images/test_webp_lossless_pre-optimized.webp
+-rw-r--r--   0        0        0     2764 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/images/test_webp_lossy.webp
+-rw-r--r--   0        0        0     1508 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/images/test_webp_lossy_pre-optimized.webp
+-rw-r--r--   0        0        0        3 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/invalid/test_invalid_cbr.cbr
+-rw-r--r--   0        0        0        3 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/invalid/test_invalid_cbz.cbz
+-rw-r--r--   0        0        0        0 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/invalid/test_invalid_gif.gif
+-rw-r--r--   0        0        0        0 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/invalid/test_invalid_jpg.jpg
+-rw-r--r--   0        0        0        0 2023-05-14 22:59:15.334082 picopt-3.3.6/tests/test_files/invalid/test_invalid_png.png
+-rw-r--r--   0        0        0   879952 2023-05-14 22:59:15.338082 picopt-3.3.6/tests/test_files/invalid/test_mpeg.mpeg
+-rw-r--r--   0        0        0       80 2023-05-14 22:59:15.338082 picopt-3.3.6/tests/test_files/invalid/test_rar.rar
+-rw-r--r--   0        0        0      167 2023-05-14 22:59:15.338082 picopt-3.3.6/tests/test_files/invalid/test_zip.zip
+-rw-r--r--   0        0        0       18 2023-05-14 22:59:15.338082 picopt-3.3.6/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1923 2023-05-14 22:59:15.338082 picopt-3.3.6/tests/unit/test_cli.py
+-rw-r--r--   0        0        0      871 2023-05-14 22:59:15.338082 picopt-3.3.6/tests/unit/test_png_bit_depth.py
+-rw-r--r--   0        0        0     9109 1970-01-01 00:00:00.000000 picopt-3.3.6/PKG-INFO
```

### Comparing `picopt-3.3.5/README.md` & `picopt-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/cli.py` & `picopt-3.3.6/picopt/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from termcolor import colored, cprint
 
 from picopt import PROGRAM_NAME, walk
 from picopt.config import ALL_FORMAT_STRS, DEFAULT_HANDLERS, get_config
 from picopt.handlers.png import Png
 from picopt.handlers.webp import WebP
-from picopt.handlers.zip import CBZ, Zip
+from picopt.handlers.zip import CBR, Rar
 
 DEFAULT_FORMAT_STRS = frozenset(
     [handler_cls.OUTPUT_FORMAT_STR for handler_cls in DEFAULT_HANDLERS]
 )
 EXTRA_FORMAT_STRS = ALL_FORMAT_STRS - DEFAULT_FORMAT_STRS
 FORMAT_DELIMETER = ","
 try:
@@ -103,16 +103,16 @@
     parser.add_argument(
         "-c",
         "--convert-to",
         action=SplitArgsAction,
         dest="convert_to",
         help="A list of formats to convert to. Lossless images may convert to"
         f" {Png.OUTPUT_FORMAT_STR} or {WebP.OUTPUT_FORMAT_STR}."
-        f" {Zip.INPUT_FORMAT_STR_RAR} archives"
-        f" may convert to {Zip.OUTPUT_FORMAT_STR} or {CBZ.OUTPUT_FORMAT_STR}."
+        f" {Rar.INPUT_FORMAT_STR} archives"
+        f" may convert to {Rar.OUTPUT_FORMAT_STR} or {CBR.OUTPUT_FORMAT_STR}."
         " By default formats are not converted to other formats.",
     )
     parser.add_argument(
         "-S",
         "--no-symlinks",
         action="store_false",
         dest="symlinks",
```

### Comparing `picopt-3.3.5/picopt/config.py` & `picopt-3.3.6/picopt/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     TIFF_FILE_FORMAT,
     TIFF_FORMAT_STR,
 )
 from picopt.handlers.jpeg import Jpeg
 from picopt.handlers.png import Png
 from picopt.handlers.webp import Gif2WebP, WebPLossless, WebPLossy
 from picopt.handlers.webp_animated import WebPAnimatedLossless, WebPAnimatedLossy
-from picopt.handlers.zip import CBZ, EPub, Zip
+from picopt.handlers.zip import CBR, CBZ, EPub, Rar, Zip
 
 _PNG_CONVERTABLE_FILE_FORMATS = CONVERTABLE_FILE_FORMATS | frozenset(
     [Gif.OUTPUT_FILE_FORMAT]
 )
 _WEBP_CONVERTABLE_FILE_FORMATS = _PNG_CONVERTABLE_FILE_FORMATS | frozenset(
     [Png.OUTPUT_FILE_FORMAT]
 )
@@ -57,25 +57,27 @@
         Png.OUTPUT_FORMAT_STR,
         WebPLossless.OUTPUT_FORMAT_STR,
         Zip.OUTPUT_FORMAT_STR,
         CBZ.OUTPUT_FORMAT_STR,
     )
 )
 CONTAINER_CONVERTABLE_FORMAT_STRS = frozenset(
-    (Zip.INPUT_FORMAT_STR_RAR, CBZ.INPUT_FORMAT_STR_RAR)
+    (Rar.INPUT_FORMAT_STR, CBR.INPUT_FORMAT_STR)
 )
 DEFAULT_HANDLERS = (Gif, AnimatedGif, Jpeg, Png, WebPLossy, WebPLossless)
 HANDLERS = frozenset(
     [
         *DEFAULT_HANDLERS,
         Gif2WebP,
         WebPAnimatedLossy,
         WebPAnimatedLossless,
         Zip,
+        Rar,
         CBZ,
+        CBR,
         EPub,
     ]
 )
 ALL_FORMAT_STRS: frozenset[str] = (
     frozenset([cls.OUTPUT_FORMAT_STR for cls in HANDLERS])
     | CONVERTABLE_FORMAT_STRS
     | frozenset([TIFF_FORMAT_STR])
@@ -177,16 +179,16 @@
     WebPLossless.OUTPUT_FILE_FORMAT: FileFormatHandlers(native=WebPLossless),
     WebPAnimatedLossy.OUTPUT_FILE_FORMAT: FileFormatHandlers(native=WebPAnimatedLossy),
     WebPAnimatedLossless.OUTPUT_FILE_FORMAT: FileFormatHandlers(
         native=WebPAnimatedLossless
     ),
     Zip.OUTPUT_FILE_FORMAT: FileFormatHandlers(native=Zip),
     CBZ.OUTPUT_FILE_FORMAT: FileFormatHandlers(native=CBZ),
-    Zip.INPUT_FILE_FORMAT_RAR: FileFormatHandlers(convert=Zip),
-    CBZ.INPUT_FILE_FORMAT_RAR: FileFormatHandlers(convert=CBZ),
+    Rar.INPUT_FILE_FORMAT: FileFormatHandlers(convert=Rar),
+    CBR.INPUT_FILE_FORMAT: FileFormatHandlers(convert=CBR),
     EPub.OUTPUT_FILE_FORMAT: FileFormatHandlers(native=EPub),
     TIFF_FILE_FORMAT: FileFormatHandlers(convert=(WebPLossless, Png)),
     TIFF_ANIMATED_FILE_FORMAT: FileFormatHandlers(convert=WebPAnimatedLossless),
     PNG_ANIMATED_FILE_FORMAT: FileFormatHandlers(convert=WebPAnimatedLossless),
 }
 MODE_EXECUTABLE = stat.S_IXUSR ^ stat.S_IXGRP ^ stat.S_IXOTH
 
@@ -284,23 +286,23 @@
         convertable_format_strs
     )
     return format_strs
 
 
 def _update_formats_zip(format_strs, convert_handlers):
     """Update formats if converting to zip."""
-    format_strs |= {Zip.INPUT_FORMAT_STR_RAR}
-    convert_handlers[Zip] = {Zip.INPUT_FILE_FORMAT_RAR}
+    format_strs |= {Rar.INPUT_FORMAT_STR}
+    convert_handlers[Rar] = {Rar.INPUT_FILE_FORMAT}
     return format_strs
 
 
 def _update_formats_cbz(format_strs, convert_handlers):
     """Update formats if converting to cbz."""
-    format_strs |= {CBZ.INPUT_FORMAT_STR_RAR}
-    convert_handlers[CBZ] = {CBZ.INPUT_FILE_FORMAT_RAR}
+    format_strs |= {CBR.INPUT_FORMAT_STR}
+    convert_handlers[CBR] = {CBR.INPUT_FILE_FORMAT}
     return format_strs
 
 
 def _update_formats(config: Configuration) -> dict:
     formats = _config_formats_list_to_set(config, "formats")
     if "extra_formats" in config[PROGRAM_NAME]["computed"]:
         extra_formats = _config_formats_list_to_set(
@@ -312,17 +314,17 @@
     convert_to = _config_formats_list_to_set(config, "convert_to")
     config[PROGRAM_NAME]["convert_to"].set(sorted(convert_to))
     convert_handlers: dict[type[Handler], set[FileFormat]] = {}
     if Png.OUTPUT_FORMAT_STR in convert_to:
         formats = _update_formats_png(formats, convert_handlers, config)
     if WebPLossless.OUTPUT_FORMAT_STR in convert_to:
         formats = _update_formats_webp_lossless(formats, convert_handlers, config)
-    if Zip.OUTPUT_FORMAT_STR in convert_to:
+    if Rar.OUTPUT_FORMAT_STR in convert_to:
         formats = _update_formats_zip(formats, convert_handlers)
-    if CBZ.OUTPUT_FORMAT_STR in convert_to:
+    if CBR.OUTPUT_FORMAT_STR in convert_to:
         formats = _update_formats_cbz(formats, convert_handlers)
     config[PROGRAM_NAME]["formats"].set(sorted(formats))
 
     return convert_handlers
 
 
 def _create_format_handler_map(config: Configuration, convert_handlers: dict) -> None:
```

### Comparing `picopt-3.3.5/picopt/handlers/container.py` & `picopt-3.3.6/picopt/handlers/container.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/handlers/factory.py` & `picopt-3.3.6/picopt/handlers/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from picopt.config import WEBP_CONVERTABLE_FORMAT_STRS
 from picopt.data import PathInfo
 from picopt.handlers.container import ContainerHandler
 from picopt.handlers.handler import FileFormat, Handler, Metadata
 from picopt.handlers.image import TIFF_FORMAT_STR
 from picopt.handlers.webp import WebPLossless
-from picopt.handlers.zip import CBZ, EPub, Zip
+from picopt.handlers.zip import CBR, CBZ, EPub, Rar, Zip
 from picopt.pillow.webp_lossless import is_lossless
 
 _ALWAYS_LOSSLESS_FORMAT_STRS = WEBP_CONVERTABLE_FORMAT_STRS - {TIFF_FORMAT_STR}
-_CONTAINER_HANDLERS: tuple[type[ContainerHandler], ...] = (CBZ, Zip, EPub)
+_CONTAINER_HANDLERS: tuple[type[ContainerHandler], ...] = (CBZ, Zip, CBR, Rar, EPub)
 
 
 def _is_lossless(image_format: str, path: Path, info: dict) -> bool:
     """Determine if image format is lossless."""
     if image_format in _ALWAYS_LOSSLESS_FORMAT_STRS:
         lossless = True
     elif image_format == WebPLossless.OUTPUT_FORMAT_STR:
```

### Comparing `picopt-3.3.5/picopt/handlers/gif.py` & `picopt-3.3.6/picopt/handlers/gif.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/handlers/handler.py` & `picopt-3.3.6/picopt/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/handlers/image.py` & `picopt-3.3.6/picopt/handlers/image.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/handlers/jpeg.py` & `picopt-3.3.6/picopt/handlers/jpeg.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/handlers/png.py` & `picopt-3.3.6/picopt/handlers/png.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/handlers/webp.py` & `picopt-3.3.6/picopt/handlers/webp.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/handlers/webp_animated.py` & `picopt-3.3.6/picopt/handlers/webp_animated.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/handlers/zip.py` & `picopt-3.3.6/picopt/handlers/zip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 """Handler for zip files."""
 import os
 from pathlib import Path
-from typing import Optional, Union
-from zipfile import ZIP_DEFLATED, ZipFile, is_zipfile
+from typing import Optional
 
 from PIL import Image, UnidentifiedImageError
 from rarfile import RarFile, is_rarfile
 from termcolor import cprint
+from zipfile_deflate64 import ZIP_DEFLATED, ZipFile, is_zipfile
 
 from picopt.handlers.container import ContainerHandler
 from picopt.handlers.handler import FileFormat
 
 
 class Zip(ContainerHandler):
     """Ziplike container."""
 
     OUTPUT_FORMAT_STR: str = "ZIP"
     OUTPUT_FILE_FORMAT: FileFormat = FileFormat(OUTPUT_FORMAT_STR)
-    INPUT_FORMAT_STR_RAR: str = "RAR"
-    INPUT_FILE_FORMAT_RAR: FileFormat = FileFormat(INPUT_FORMAT_STR_RAR)
-    RAR_SUFFIX: str = "." + INPUT_FORMAT_STR_RAR.lower()
-    PROGRAMS: dict[str, Optional[str]] = {ContainerHandler.INTERNAL: None}
+    PROGRAMS: dict[str, Optional[str]] = {
+        ContainerHandler.INTERNAL: None,
+    }
 
     @classmethod
     def identify_format(cls, path: Path) -> Optional[FileFormat]:
         """Return the format if this handler can handle this path."""
         file_format = None
         suffix = path.suffix.lower()
         if is_zipfile(path) and suffix == cls.get_default_suffix():
             file_format = cls.OUTPUT_FILE_FORMAT
-        elif is_rarfile(path) and suffix == cls.RAR_SUFFIX:
-            file_format = cls.INPUT_FILE_FORMAT_RAR
         return file_format
 
-    def _get_archive(self) -> Union[ZipFile, RarFile]:
+    def _get_archive(self) -> ZipFile:
         """Use the zipfile builtin for this archive."""
         if is_zipfile(self.original_path):
             archive = ZipFile(self.original_path, "r")
-        elif is_rarfile(self.original_path):
-            archive = RarFile(self.original_path, "r")
         else:
             msg = f"Unknown archive type: {self.original_path}"
             raise ValueError(msg)
         return archive
 
-    def _set_comment(self, comment: Union[str, bytes, None]) -> None:
+    def _set_comment(self, comment: Optional[bytes]) -> None:
         """Set the comment from the archive."""
-        if type(comment) is str:
-            self.comment = comment.encode()
-        elif type(comment) is bytes:
+        if comment:
             self.comment = comment
 
     def unpack_into(self) -> None:
         """Uncompress archive."""
         with self._get_archive() as archive:
             archive.extractall(self.tmp_container_dir)
             self._set_comment(archive.comment)
@@ -87,22 +80,61 @@
                     compress_type = None if self._is_image(full_path) else ZIP_DEFLATED
                     archive_path = full_path.relative_to(self.tmp_container_dir)
                     new_zf.write(full_path, archive_path, compress_type)
             if self.comment:
                 new_zf.comment = self.comment
 
 
+class Rar(Zip):
+    """RAR Container."""
+
+    INPUT_FORMAT_STR: str = "RAR"
+    INPUT_FILE_FORMAT: FileFormat = FileFormat(INPUT_FORMAT_STR)
+    INPUT_SUFFIX: str = "." + INPUT_FORMAT_STR.lower()
+    PROGRAMS: dict[str, Optional[str]] = Zip.init_programs(("unrar",))
+
+    @classmethod
+    def identify_format(cls, path: Path) -> Optional[FileFormat]:
+        """Return the format if this handler can handle this path."""
+        file_format = None
+        suffix = path.suffix.lower()
+        if is_rarfile(path) and suffix == cls.INPUT_SUFFIX:
+            file_format = cls.INPUT_FILE_FORMAT
+        return file_format
+
+    def _get_archive(self) -> RarFile:
+        """Use the zipfile builtin for this archive."""
+        if is_rarfile(self.original_path):
+            archive = RarFile(self.original_path)
+        else:
+            msg = f"Unknown archive type: {self.original_path}"
+            raise ValueError(msg)
+        return archive
+
+    def _set_comment(self, comment: Optional[str]) -> None:
+        """Set the comment from the archive."""
+        if comment:
+            self.comment = comment.encode()
+
+
 class CBZ(Zip):
     """CBZ Container."""
 
     OUTPUT_FORMAT_STR: str = "CBZ"
     OUTPUT_FILE_FORMAT: FileFormat = FileFormat(OUTPUT_FORMAT_STR)
-    INPUT_FORMAT_STR_RAR: str = "CBR"
-    INPUT_FILE_FORMAT_RAR: FileFormat = FileFormat(INPUT_FORMAT_STR_RAR)
-    RAR_SUFFIX: str = "." + INPUT_FORMAT_STR_RAR.lower()
+
+
+class CBR(Rar):
+    """CBR Container."""
+
+    INPUT_FORMAT_STR: str = "CBR"
+    INPUT_FILE_FORMAT: FileFormat = FileFormat(INPUT_FORMAT_STR)
+    INPUT_SUFFIX: str = "." + INPUT_FORMAT_STR.lower()
+    OUTPUT_FORMAT_STR: str = "CBZ"
+    OUTPUT_FILE_FORMAT: FileFormat = FileFormat(OUTPUT_FORMAT_STR)
 
 
 class EPub(Zip):
     """Epub Container."""
 
     OUTPUT_FORMAT_STR: str = "EPUB"
     OUTPUT_FILE_FORMAT: FileFormat = FileFormat(OUTPUT_FORMAT_STR)
```

### Comparing `picopt-3.3.5/picopt/old_timestamps.py` & `picopt-3.3.6/picopt/old_timestamps.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/pillow/header.py` & `picopt-3.3.6/picopt/pillow/header.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/pillow/png_bit_depth.py` & `picopt-3.3.6/picopt/pillow/png_bit_depth.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/pillow/webp_lossless.py` & `picopt-3.3.6/picopt/pillow/webp_lossless.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/picopt/stats.py` & `picopt-3.3.6/picopt/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 cmd = " ".join(self.exc.cmd)
                 report += f"\n{self._TAB}command: {cmd}"
             if self.exc.stdout:
                 report += f"\n{self._TAB}stdout: {self.exc.stdout}"
             if self.exc.stderr:
                 report += f"\n{self._TAB}stderr: {self.exc.stderr}"
         else:
-            report += f"\n{self._TAB}{str(self.exc)}"
+            report += f"\n{self._TAB}{self.exc!s}"
         return report
 
     def report(self) -> None:
         """Record the percent saved & print it."""
         attrs = []
         if self.exc:
             report = self._report_error()
```

### Comparing `picopt-3.3.5/picopt/walk.py` & `picopt-3.3.6/picopt/walk.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from picopt.data import PathInfo, ReportInfo
 from picopt.handlers.container import ContainerHandler
 from picopt.handlers.factory import create_handler
 from picopt.handlers.handler import Handler
 from picopt.handlers.image import ImageHandler
 from picopt.handlers.png import Png
 from picopt.handlers.webp import WebP
-from picopt.handlers.zip import CBZ, Zip
+from picopt.handlers.zip import CBR, Rar
 from picopt.old_timestamps import OLD_TIMESTAMPS_NAME, OldTimestamps
 from picopt.stats import ReportStats, Totals
 
 
 class Walk(Configurable):
     """Walk object for storing state of a walk run."""
 
@@ -55,18 +55,18 @@
                 self._convert_message(
                     self._config.computed.convertable_formats.webp, WebP
                 )
             elif Png.OUTPUT_FORMAT_STR in self._config.convert_to:
                 self._convert_message(
                     self._config.computed.convertable_formats.png, Png
                 )
-            if Zip.OUTPUT_FORMAT_STR in self._config.convert_to:
-                self._convert_message(frozenset([Zip.INPUT_FORMAT_STR_RAR]), Zip)
-            if CBZ.OUTPUT_FORMAT_STR in self._config.convert_to:
-                self._convert_message(frozenset([CBZ.INPUT_FORMAT_STR_RAR]), CBZ)
+            if Rar.OUTPUT_FORMAT_STR in self._config.convert_to:
+                self._convert_message(frozenset([Rar.INPUT_FORMAT_STR]), Rar)
+            if CBR.OUTPUT_FORMAT_STR in self._config.convert_to:
+                self._convert_message(frozenset([CBR.INPUT_FORMAT_STR]), CBR)
         if self._config.after is not None:
             after = time.ctime(self._config.after)
             cprint(f"Optimizing after {after}")
 
     def _init_run_timestamps(self) -> None:
         """Init timestamps."""
         config = GrovestampsConfig(
```

### Comparing `picopt-3.3.5/pyproject.toml` & `picopt-3.3.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = ["poetry.core.masonry.api"]
 
 [tool.poetry]
 name = "picopt"
-version = "3.3.5"
+version = "3.3.6"
 description = "A multi format lossless image optimizer that uses external tools"
 license = "GPL-3.0-only"
 authors = ["AJ Slater <aj@slater.net>"]
 readme = "README.md"
 homepage = "https://github.com/ajslater/picopt"
 documentation = "https://github.com/ajslater/picopt"
 keywords = ["image", "png", "jpg", "cbz", "cbr"]
@@ -32,26 +32,27 @@
 humanize = "^4.0.0"
 python-dateutil = "^2.8"
 rarfile = "^4.0"
 "ruamel.yaml" = "^0.17.16"
 termcolor = "^2.0.1"
 treestamps = "^0.4.3"
 Pillow = "^9.0"
+zipfile-deflate64 = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 codespell = "^2.1.0"
 coverage = { extras = ["toml"], version = "^7.0" }
 neovim = "^0.3.1"
 pyright = "^1.1.237"
 pytest = "^7.0.0"
 pytest-cov = "^4.0"
 pytest-gitignore = "^1.3"
 radon = { version = "^6.0.1", extras = ["toml"] }
-ruff = "^0.0.265"
+ruff = ">=0.0.265,<0.1.0"
 types-python-dateutil = "^2.8.0"
 vulture = "^2.1"
 
 [tool.poetry.scripts]
 picopt = "picopt.cli:main"
 
 [tool.poetry.urls]
```

### Comparing `picopt-3.3.5/tests/__init__.py` & `picopt-3.3.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/integration/test_containers.py` & `picopt-3.3.6/tests/integration/test_containers.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/integration/test_images_dir.py` & `picopt-3.3.6/tests/integration/test_images_dir.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/integration/test_old_timestamps.py` & `picopt-3.3.6/tests/integration/test_old_timestamps.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/integration/test_one_container.py` & `picopt-3.3.6/tests/integration/test_one_container.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/integration/test_timestamps.py` & `picopt-3.3.6/tests/integration/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/containers/igp-twss.epub` & `picopt-3.3.6/tests/test_files/containers/igp-twss.epub`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/containers/test_cbr.cbr` & `picopt-3.3.6/tests/test_files/containers/test_cbr.cbr`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/containers/test_cbz.cbz` & `picopt-3.3.6/tests/test_files/containers/test_cbz.cbz`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/containers/test_rar.rar` & `picopt-3.3.6/tests/test_files/containers/test_rar.rar`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/containers/test_zip.zip` & `picopt-3.3.6/tests/test_files/containers/test_zip.zip`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/07themecamplist.pdf` & `picopt-3.3.6/tests/test_files/images/07themecamplist.pdf`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/eight.tif` & `picopt-3.3.6/tests/test_files/images/eight.tif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/mri.tif` & `picopt-3.3.6/tests/test_files/images/mri.tif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_animated_gif.gif` & `picopt-3.3.6/tests/test_files/images/test_animated_gif.gif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_animated_png.png` & `picopt-3.3.6/tests/test_files/images/test_animated_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_animated_webp.webp` & `picopt-3.3.6/tests/test_files/images/test_animated_webp.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_bmp.bmp` & `picopt-3.3.6/tests/test_files/images/test_bmp.bmp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_gif.gif` & `picopt-3.3.6/tests/test_files/images/test_gif.gif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_jpg.jpg` & `picopt-3.3.6/tests/test_files/images/test_jpg.jpg`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_png.png` & `picopt-3.3.6/tests/test_files/images/test_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_png_16rgba.png` & `picopt-3.3.6/tests/test_files/images/test_png_16rgba.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_pnm.pnm` & `picopt-3.3.6/tests/test_files/images/test_pnm.pnm`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_pre-optimized_jpg.jpg` & `picopt-3.3.6/tests/test_files/images/test_pre-optimized_jpg.jpg`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_pre-optimized_png.png` & `picopt-3.3.6/tests/test_files/images/test_pre-optimized_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_webp_lossless.webp` & `picopt-3.3.6/tests/test_files/images/test_webp_lossless.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_webp_lossless_pre-optimized.webp` & `picopt-3.3.6/tests/test_files/images/test_webp_lossless_pre-optimized.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_webp_lossy.webp` & `picopt-3.3.6/tests/test_files/images/test_webp_lossy.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/images/test_webp_lossy_pre-optimized.webp` & `picopt-3.3.6/tests/test_files/images/test_webp_lossy_pre-optimized.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/test_files/invalid/test_mpeg.mpeg` & `picopt-3.3.6/tests/test_files/invalid/test_mpeg.mpeg`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/unit/test_cli.py` & `picopt-3.3.6/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/tests/unit/test_png_bit_depth.py` & `picopt-3.3.6/tests/unit/test_png_bit_depth.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.5/PKG-INFO` & `picopt-3.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picopt
-Version: 3.3.5
+Version: 3.3.6
 Summary: A multi format lossless image optimizer that uses external tools
 Home-page: https://github.com/ajslater/picopt
 License: GPL-3.0-only
 Keywords: image,png,jpg,cbz,cbr
 Author: AJ Slater
 Author-email: aj@slater.net
 Requires-Python: >=3.9,<4.0
@@ -26,14 +26,15 @@
 Requires-Dist: confuse (>=2.0.0,<3.0.0)
 Requires-Dist: humanize (>=4.0.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8,<3.0)
 Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: ruamel.yaml (>=0.17.16,<0.18.0)
 Requires-Dist: termcolor (>=2.0.1,<3.0.0)
 Requires-Dist: treestamps (>=0.4.3,<0.5.0)
+Requires-Dist: zipfile-deflate64 (>=0.2.0,<0.3.0)
 Project-URL: Documentation, https://github.com/ajslater/picopt
 Project-URL: Issues, https://github.com/ajslater/picopt/issues
 Project-URL: Source, https://github.com/ajslater/picopt
 Description-Content-Type: text/markdown
 
 # picopt
```

