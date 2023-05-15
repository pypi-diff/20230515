# Comparing `tmp/dearwatson-0.7.2.tar.gz` & `tmp/dearwatson-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.7.2.tar", last modified: Mon May 15 07:54:01 2023, max compression
+gzip compressed data, was "dearwatson-0.7.3.tar", last modified: Mon May 15 16:16:55 2023, max compression
```

## Comparing `dearwatson-0.7.2.tar` & `dearwatson-0.7.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:54:01.136803 dearwatson-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-15 07:53:43.000000 dearwatson-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 07:53:43.000000 dearwatson-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-15 07:54:01.136803 dearwatson-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-15 07:53:43.000000 dearwatson-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:54:01.132803 dearwatson-0.7.2/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-15 07:54:00.000000 dearwatson-0.7.2/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-15 07:54:01.000000 dearwatson-0.7.2/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:54:00.000000 dearwatson-0.7.2/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-15 07:54:00.000000 dearwatson-0.7.2/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 07:54:00.000000 dearwatson-0.7.2/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:54:01.136803 dearwatson-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-15 07:53:44.000000 dearwatson-0.7.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 07:53:44.000000 dearwatson-0.7.2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:54:01.132803 dearwatson-0.7.2/watson/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 07:53:44.000000 dearwatson-0.7.2/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 07:53:44.000000 dearwatson-0.7.2/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:54:01.132803 dearwatson-0.7.2/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-15 07:53:44.000000 dearwatson-0.7.2/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 07:53:44.000000 dearwatson-0.7.2/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-15 07:53:44.000000 dearwatson-0.7.2/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-15 07:53:44.000000 dearwatson-0.7.2/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:54:01.128802 dearwatson-0.7.2/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:54:01.132803 dearwatson-0.7.2/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-05-15 07:53:44.000000 dearwatson-0.7.2/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-05-15 07:53:44.000000 dearwatson-0.7.2/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:54:01.136803 dearwatson-0.7.2/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:53:45.000000 dearwatson-0.7.2/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-15 07:53:45.000000 dearwatson-0.7.2/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:54:01.136803 dearwatson-0.7.2/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:53:46.000000 dearwatson-0.7.2/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-15 07:53:46.000000 dearwatson-0.7.2/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-15 07:53:46.000000 dearwatson-0.7.2/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)   105984 2023-05-15 07:53:45.000000 dearwatson-0.7.2/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.719729 dearwatson-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-15 16:16:43.000000 dearwatson-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 16:16:43.000000 dearwatson-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-15 16:16:55.719729 dearwatson-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-15 16:16:43.000000 dearwatson-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.715728 dearwatson-0.7.3/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:16:55.719729 dearwatson-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-15 16:16:43.000000 dearwatson-0.7.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 16:16:43.000000 dearwatson-0.7.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.715728 dearwatson-0.7.3/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.715728 dearwatson-0.7.3/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.711728 dearwatson-0.7.3/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.719729 dearwatson-0.7.3/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.719729 dearwatson-0.7.3/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:44.000000 dearwatson-0.7.3/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-15 16:16:44.000000 dearwatson-0.7.3/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.719729 dearwatson-0.7.3/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:16:45.000000 dearwatson-0.7.3/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-15 16:16:45.000000 dearwatson-0.7.3/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-15 16:16:45.000000 dearwatson-0.7.3/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107144 2023-05-15 16:16:44.000000 dearwatson-0.7.3/watson/watson.py
```

### Comparing `dearwatson-0.7.2/LICENSE` & `dearwatson-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/PKG-INFO` & `dearwatson-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.2
+Version: 0.7.3
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.2/README.md` & `dearwatson-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/dearwatson.egg-info/PKG-INFO` & `dearwatson-0.7.3/dearwatson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.2
+Version: 0.7.3
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.2/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.7.3/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/setup.py` & `dearwatson-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.7.2"
+version = "0.7.3"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
```

### Comparing `dearwatson-0.7.2/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.7.3/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/watson/neighbours.py` & `dearwatson-0.7.3/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/watson/report.py` & `dearwatson-0.7.3/watson/report.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/watson/resources/images/sherlock3.png` & `dearwatson-0.7.3/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/watson/resources/images/watson.png` & `dearwatson-0.7.3/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/watson/tests/test_watson.py` & `dearwatson-0.7.3/watson/tests/test_watson.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.7.3/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.7.3/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.2/watson/watson.py` & `dearwatson-0.7.3/watson/watson.py`

 * *Files 1% similar despite different names*

```diff
@@ -660,29 +660,52 @@
         snrs = {}
         for index, cadence in enumerate(cadences):
             lc = None
             found_sectors = []
             axs[index].set_title(mission_prefix + " " + str(id) + " " + str(found_sectors) + ": " + cadence)
             if mission == lcbuilder.constants.MISSION_TESS and cadence == 'long':
                 author = "TESS-SPOC"
+                lcs = lightkurve.search_lightcurve(
+                    mission_prefix + " " + str(id),
+                    mission=mission,
+                    sector=sectors,
+                    campaign=sectors,
+                    quarter=sectors,
+                    author=author,
+                    cadence=cadence
+                ).download_all(download_dir=os.path.expanduser('~') + '/' + LIGHTKURVE_CACHE_DIR)
             elif mission == lcbuilder.constants.MISSION_TESS and cadence != 'long':
                 author = "SPOC"
+                lcs = lightkurve.search_lightcurve(
+                    mission_prefix + " " + str(id),
+                    mission=mission,
+                    sector=sectors,
+                    campaign=sectors,
+                    quarter=sectors,
+                    author=author,
+                    cadence=cadence
+                ).download_all(download_dir=os.path.expanduser('~') + '/' + LIGHTKURVE_CACHE_DIR)
             elif mission == lcbuilder.constants.MISSION_KEPLER:
                 author = "Kepler"
+                lcs = lightkurve.search_lightcurve(
+                    mission_prefix + " " + str(id),
+                    mission=mission,
+                    quarter=sectors,
+                    author=author,
+                    cadence=cadence
+                ).download_all(download_dir=os.path.expanduser('~') + '/' + LIGHTKURVE_CACHE_DIR)
             elif mission == lcbuilder.constants.MISSION_K2:
                 author = "K2"
-            lcs = lightkurve.search_lightcurve(
-                mission_prefix + " " + str(id),
-                mission=mission,
-                sector=sectors,
-                campaign=sectors,
-                quarter=sectors,
-                author=author,
-                cadence=cadence
-            ).download_all(download_dir=os.path.expanduser('~') + '/' + LIGHTKURVE_CACHE_DIR)
+                lcs = lightkurve.search_lightcurve(
+                    mission_prefix + " " + str(id),
+                    mission=mission,
+                    campaign=sectors,
+                    author=author,
+                    cadence=cadence
+                ).download_all(download_dir=os.path.expanduser('~') + '/' + LIGHTKURVE_CACHE_DIR)
             if lcs is None:
                 continue
             matching_objects = []
             for i in range(0, len(lcs.data)):
                 if lcs.data[i].label == mission_prefix + " " + str(id):
                     if lc is None:
                         lc = lcs.data[i].normalize()
@@ -1114,17 +1137,17 @@
         source_offset_bls_ra_err = np.nanstd(np.array(source_offsets_bls)[:, 0])
         source_offset_bls_dec_err = np.nanstd(np.array(source_offsets_bls)[:, 1])
         offset_ra = np.mean([source_offset_bls_ra, source_offset_diggimg_ra])
         offset_dec = np.mean([source_offset_bls_dec, source_offset_diggimg_dec])
         offset_ra_err = 1/2 * np.sqrt(source_offset_bls_ra_err ** 2 + source_offset_diggimg_ra_err ** 2)
         offset_dec_err = 1/2 * np.sqrt(source_offset_bls_dec_err ** 2 + source_offset_diggimg_dec_err ** 2)
         if np.isnan(offset_ra_err) or offset_ra_err == 0.0:
-            offset_ra_err = np.nanstd([source_offset_bls_ra, source_offset_diggimg_ra])
+            offset_ra_err = 3 * np.nanstd([source_offset_bls_ra, source_offset_diggimg_ra])
         if np.isnan(offset_dec_err) or offset_dec_err == 0.0:
-            offset_dec_err = np.nanstd([source_offset_bls_dec, source_offset_diggimg_dec])
+            offset_dec_err = 3 * np.nanstd([source_offset_bls_dec, source_offset_diggimg_dec])
         offsets_df = pd.DataFrame(columns=['name', 'ra', 'dec', 'ra_err', 'dec_err'])
         offsets_df.append({'name': 'diff_img', 'ra': source_offset_diggimg_ra, 'dec': source_offset_diggimg_dec,
                            'ra_err': source_offset_diggimg_ra_err, 'dec_err': source_offset_diggimg_dec_err}, ignore_index=True)
         offsets_df.append({'name': 'px_bls', 'ra': source_offset_bls_ra, 'dec': source_offset_bls_dec,
                            'ra_err': source_offset_bls_ra_err, 'dec_err': source_offset_bls_dec_err}, ignore_index=True)
         offsets_df.append({'name': 'mean', 'ra': offset_ra, 'dec': offset_dec,
                            'ra_err': offset_ra_err, 'dec_err': offset_dec_err}, ignore_index=True)
```

