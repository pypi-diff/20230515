# Comparing `tmp/sar_handler-0.1.7.tar.gz` & `tmp/sar_handler-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sar_handler-0.1.7.tar", last modified: Thu Apr 27 13:14:43 2023, max compression
+gzip compressed data, was "sar_handler-0.1.8.tar", last modified: Mon May 15 17:44:39 2023, max compression
```

## Comparing `sar_handler-0.1.7.tar` & `sar_handler-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:14:43.614758 sar_handler-0.1.7/
--rw-rw-rw-   0        0        0     1057 2023-04-27 11:30:14.000000 sar_handler-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      511 2023-04-27 13:14:43.613759 sar_handler-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-27 10:58:50.000000 sar_handler-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 13:14:43.602761 sar_handler-0.1.7/sar_handler/
--rw-rw-rw-   0        0        0        0 2023-04-27 13:10:57.000000 sar_handler-0.1.7/sar_handler/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-04-27 12:20:24.000000 sar_handler-0.1.7/sar_handler/assistive_funcs.py
--rw-rw-rw-   0        0        0      918 2022-10-11 07:49:15.000000 sar_handler-0.1.7/sar_handler/check_validity_of_values.py
--rw-rw-rw-   0        0        0     4381 2023-03-01 10:44:04.000000 sar_handler-0.1.7/sar_handler/csv_dataloader.py
--rw-rw-rw-   0        0        0     9324 2023-04-27 12:20:58.000000 sar_handler-0.1.7/sar_handler/dataset_creator.py
--rw-rw-rw-   0        0        0    10185 2023-04-27 10:17:07.000000 sar_handler-0.1.7/sar_handler/fastaniso.py
--rw-rw-rw-   0        0        0     3445 2023-02-26 12:09:17.000000 sar_handler-0.1.7/sar_handler/image_processing.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:14:43.612759 sar_handler-0.1.7/sar_handler.egg-info/
--rw-rw-rw-   0        0        0      511 2023-04-27 13:14:43.000000 sar_handler-0.1.7/sar_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-04-27 13:14:43.000000 sar_handler-0.1.7/sar_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:14:43.000000 sar_handler-0.1.7/sar_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-27 13:14:43.000000 sar_handler-0.1.7/sar_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 13:14:43.000000 sar_handler-0.1.7/sar_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 13:14:43.614758 sar_handler-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1118 2023-04-27 13:12:00.000000 sar_handler-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:44:39.868747 sar_handler-0.1.8/
+-rw-rw-rw-   0        0        0     1057 2023-04-27 11:30:14.000000 sar_handler-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      512 2023-05-15 17:44:39.845938 sar_handler-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-15 17:40:02.000000 sar_handler-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 17:44:39.797255 sar_handler-0.1.8/sar_handler/
+-rw-rw-rw-   0        0        0        0 2023-04-27 13:10:57.000000 sar_handler-0.1.8/sar_handler/__init__.py
+-rw-rw-rw-   0        0        0     4352 2023-05-15 17:39:39.000000 sar_handler-0.1.8/sar_handler/assistive_funcs.py
+-rw-rw-rw-   0        0        0      918 2022-10-11 07:49:15.000000 sar_handler-0.1.8/sar_handler/check_validity_of_values.py
+-rw-rw-rw-   0        0        0     4381 2023-03-01 10:44:04.000000 sar_handler-0.1.8/sar_handler/csv_dataloader.py
+-rw-rw-rw-   0        0        0     9324 2023-04-27 12:20:58.000000 sar_handler-0.1.8/sar_handler/dataset_creator.py
+-rw-rw-rw-   0        0        0    10185 2023-04-27 10:17:07.000000 sar_handler-0.1.8/sar_handler/fastaniso.py
+-rw-rw-rw-   0        0        0     3445 2023-02-26 12:09:17.000000 sar_handler-0.1.8/sar_handler/image_processing.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:44:39.844935 sar_handler-0.1.8/sar_handler.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-05-15 17:44:39.000000 sar_handler-0.1.8/sar_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-05-15 17:44:39.000000 sar_handler-0.1.8/sar_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 17:44:39.000000 sar_handler-0.1.8/sar_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-15 17:44:39.000000 sar_handler-0.1.8/sar_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-15 17:44:39.000000 sar_handler-0.1.8/sar_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 17:44:39.868747 sar_handler-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-05-15 17:44:06.000000 sar_handler-0.1.8/setup.py
```

### Comparing `sar_handler-0.1.7/LICENSE` & `sar_handler-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.7/sar_handler/assistive_funcs.py` & `sar_handler-0.1.8/sar_handler/assistive_funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,17 @@
             res = model(res).to("cpu")
             if classifier:
                 res = res.argmax(axis=-1)
             out_image[y] = np.squeeze(np.array(res))
 
         if not classifier and normalize_data:
             out_image *= 255
-        out = np.where(out_image >= 255, 255, out_image)
+        if not classifier:
+            out = np.where(out_image >= 255, 255, out_image)
+            out = np.where(out_image < 0, 0, out)
         out = out.astype(np.uint8)
         out = Image.fromarray(out)
         out.save(out_path)
 
 
 def check_ssim(filtered_images, genuine_images, image_name, print_metric=False) -> None:
     filtered_img = np.array(ImageOps.grayscale(Image.open(filtered_images / image_name)))
```

### Comparing `sar_handler-0.1.7/sar_handler/check_validity_of_values.py` & `sar_handler-0.1.8/sar_handler/check_validity_of_values.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.7/sar_handler/csv_dataloader.py` & `sar_handler-0.1.8/sar_handler/csv_dataloader.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.7/sar_handler/dataset_creator.py` & `sar_handler-0.1.8/sar_handler/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.7/sar_handler/fastaniso.py` & `sar_handler-0.1.8/sar_handler/fastaniso.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.7/sar_handler/image_processing.py` & `sar_handler-0.1.8/sar_handler/image_processing.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.7/setup.py` & `sar_handler-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 from datetime import datetime
 
 
-version = '0.1.7'
-changes = "src dir removed"
+version = '0.1.8'
+changes = "bug with regression normalized fixed"
 
 SHIFT = "=" * 30
 date = datetime.now()
 changes = f"\n{SHIFT}\n{date} | {version}\n{changes}\n"
 
 if __name__ == "__main__":
     with open("./CHANGELOG.txt", "a") as f:
```

