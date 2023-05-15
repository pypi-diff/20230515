# Comparing `tmp/threedi-scenario-downloader-0.9.tar.gz` & `tmp/threedi-scenario-downloader-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/threedi-scenario-downloader-0.9.tar", last modified: Wed May 22 09:15:01 2019, max compression
+gzip compressed data, was "threedi-scenario-downloader-1.0.tar", last modified: Mon May 15 08:33:00 2023, max compression
```

## Comparing `threedi-scenario-downloader-0.9.tar` & `threedi-scenario-downloader-1.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-22 09:15:01.000000 threedi-scenario-downloader-0.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)      203 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6354 2019-05-22 09:15:01.000000 threedi-scenario-downloader-0.9/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-22 09:15:01.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6354 2019-05-22 09:15:00.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-22 09:15:00.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-05-22 09:15:00.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-22 09:15:00.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2019-05-22 09:15:00.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2019-05-22 09:15:00.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      130 2019-05-22 09:15:01.000000 threedi-scenario-downloader-0.9/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-22 09:15:01.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17168 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader/downloader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-22 09:15:01.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4987 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader/tests/test_downloader_manual.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-22 09:15:01.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader/tests/testdata/
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader/tests/testdata/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2622 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader/tests/test_downloader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/threedi_scenario_downloader/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3606 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      974 2019-05-22 09:13:19.000000 threedi-scenario-downloader-0.9/setup.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.304116 threedi-scenario-downloader-1.0/
+-rw-r--r--   0 reinout    (501) staff       (20)     2371 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/CHANGES.rst
+-rw-r--r--   0 reinout    (501) staff       (20)     1111 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/LICENSE
+-rw-r--r--   0 reinout    (501) staff       (20)      203 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/MANIFEST.in
+-rw-r--r--   0 reinout    (501) staff       (20)     6466 2023-05-15 08:33:00.304167 threedi-scenario-downloader-1.0/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)     3698 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/README.rst
+-rw-r--r--   0 reinout    (501) staff       (20)      159 2023-05-15 08:33:00.304352 threedi-scenario-downloader-1.0/setup.cfg
+-rw-r--r--   0 reinout    (501) staff       (20)      974 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/setup.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.302578 threedi-scenario-downloader-1.0/threedi_scenario_downloader/
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)    27513 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/downloader.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.303767 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     1379 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_batch.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2070 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_downloader.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4819 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_downloader_manual.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.304008 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/testdata/
+-rw-r--r--   0 reinout    (501) staff       (20)       31 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/testdata/README.rst
+-rw-r--r--   0 reinout    (501) staff       (20)      366 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/testdata/batch.csv
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.303327 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/
+-rw-r--r--   0 reinout    (501) staff       (20)     6466 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)      761 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/not-zip-safe
+-rw-r--r--   0 reinout    (501) staff       (20)       67 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/requires.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       28 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `threedi-scenario-downloader-0.9/threedi_scenario_downloader.egg-info/SOURCES.txt` & `threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 CHANGES.rst
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 threedi_scenario_downloader/__init__.py
 threedi_scenario_downloader/downloader.py
 threedi_scenario_downloader.egg-info/PKG-INFO
 threedi_scenario_downloader.egg-info/SOURCES.txt
 threedi_scenario_downloader.egg-info/dependency_links.txt
 threedi_scenario_downloader.egg-info/not-zip-safe
 threedi_scenario_downloader.egg-info/requires.txt
 threedi_scenario_downloader.egg-info/top_level.txt
 threedi_scenario_downloader/tests/__init__.py
+threedi_scenario_downloader/tests/test_batch.py
 threedi_scenario_downloader/tests/test_downloader.py
 threedi_scenario_downloader/tests/test_downloader_manual.py
-threedi_scenario_downloader/tests/testdata/README.rst
+threedi_scenario_downloader/tests/testdata/README.rst
+threedi_scenario_downloader/tests/testdata/batch.csv
```

### Comparing `threedi-scenario-downloader-0.9/threedi_scenario_downloader/tests/test_downloader_manual.py` & `threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_downloader_manual.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,152 @@
 # -*- coding: utf-8 -*-
 """Tests for downloader.py"""
 from threedi_scenario_downloader import downloader
 import configparser
 import os
 
+SCENARIO_UUID = "4d3c9b6d-58d0-43cd-a850-8e6c2982d14f"
+SCENARIO_NAME = "threedi-scenario-download-testmodel-EV"
+MODEL_UUID = "e5c91df19ad33337d82e8cd83edb1196b7b39d3d"
+DEPTH_MAX_UUID = "c3c4dd31-8a15-4a9e-aefa-97d0cb13cbcc"
+DEPTH_UUID = "921540af-57aa-4a74-8788-6d8f1c8b518b"
 
-def test_set_headers():
+
+def test_api_key():
     config = configparser.ConfigParser()
     config.read("threedi_scenario_downloader/tests/testdata/realconfig.ini")
-    downloader.set_headers(
-        config["credentials"]["username"], config["credentials"]["password"]
+    downloader.set_api_key(config["credentials"]["api_key"])
+
+    assert (downloader.get_api_key() is not None) and (
+        downloader.get_api_key() == config["credentials"]["api_key"]
     )
 
 
 def test_download_maximum_waterdepth_raster():
     downloader.download_maximum_waterdepth_raster(
-        "06c38953-31ec-4f6d-ae1f-ccdf31a348ae",
+        SCENARIO_UUID,
         "EPSG:28992",
         resolution=1000,
-        bounds=None,
+        bbox=None,
         pathname="threedi_scenario_downloader/tests/testdata/max_waterdepth.tif",
     )
     assert os.path.isfile(
         "threedi_scenario_downloader/tests/testdata/max_waterdepth.tif"
     )
 
 
 def test_download_waterdepth_raster():
     downloader.download_waterdepth_raster(
-        "06c38953-31ec-4f6d-ae1f-ccdf31a348ae",
+        SCENARIO_UUID,
         "EPSG:28992",
         1000,
         "2018-06-02T06:00:00Z",
-        None,
-        "threedi_scenario_downloader/tests/testdata/waterdepth.tif",
+        bbox=None,
+        pathname="threedi_scenario_downloader/tests/testdata/waterdepth.tif",
     )
     assert os.path.isfile("threedi_scenario_downloader/tests/testdata/waterdepth.tif")
 
 
-def test_get_netcdf_link():
-    url = downloader.get_netcdf_link("06c38953-31ec-4f6d-ae1f-ccdf31a348ae")
-    assert url == "https://demo.lizard.net/api/v3/scenario-results/52331/results_3di.nc"
+def test_download_waterdepth_raster_reprojected_bounds():
+    bbox = {"east": 115000, "west": 114000, "north": 561000, "south": 560000}
+    downloader.download_waterdepth_raster(
+        SCENARIO_UUID,
+        "EPSG:28992",
+        1000,
+        "2018-06-02T06:00:00Z",
+        bbox=bbox,
+        pathname="threedi_scenario_downloader/tests/testdata/waterdepth_reprojected.tif",
+    )
+    assert os.path.isfile(
+        "threedi_scenario_downloader/tests/testdata/waterdepth_reprojected.tif"
+    )
 
 
 def test_download_raw_results():
     downloader.download_raw_results(
-        "06c38953-31ec-4f6d-ae1f-ccdf31a348ae",
-        "threedi_scenario_downloader/tests/testdata/test.nc",
+        SCENARIO_UUID, "threedi_scenario_downloader/tests/testdata/test.nc"
     )
     assert os.path.isfile("threedi_scenario_downloader/tests/testdata/test.nc")
 
 
 def test_download_grid_administration():
     downloader.download_grid_administration(
-        "06c38953-31ec-4f6d-ae1f-ccdf31a348ae",
-        "threedi_scenario_downloader/tests/testdata/test.h5",
+        SCENARIO_UUID, "threedi_scenario_downloader/tests/testdata/test.h5"
     )
     assert os.path.isfile("threedi_scenario_downloader/tests/testdata/test.h5")
 
 
-def test_clear_inbox():
-    result = downloader.clear_inbox()
-    assert result
-
-
 def test_get_attachment_links():
-    scenario = downloader.find_scenarios_by_name("lizardapitest")[0]
+    scenario = downloader.find_scenarios_by_name(SCENARIO_NAME)[0]
     links = downloader.get_attachment_links(scenario)
     assert links is not None
 
 
 def test_rasters_in_scenario():
-    scenario = downloader.find_scenarios_by_name("lizardapitest")[0]
+    scenario = downloader.find_scenarios_by_name(SCENARIO_NAME)[0]
     static_rasters, temporal_rasters = downloader.rasters_in_scenario(scenario)
     assert static_rasters is not None and temporal_rasters is not None
 
 
-def test_get_raster_link():
-    raster = downloader.get_raster(
-        "06c38953-31ec-4f6d-ae1f-ccdf31a348ae", "depth-max-dtri"
-    )
-    download_url = downloader.get_raster_link(
-        raster, "EPSG:4326", 10, bounds=None, time=None
+def test_get_raster_download_link():
+    raster = downloader.get_raster(SCENARIO_UUID, "depth-max-dtri")
+    scenario_instance = downloader.get_scenario_instance(SCENARIO_UUID)
+    download_url = downloader.get_raster_download_link(
+        raster, scenario_instance, 10, "EPSG:4326", bbox=None, time=None
     )
     assert download_url is not None
 
 
-# def test_get_static_rasters_links():
-#    scenario = downloader.find_scenarios_by_name("lizardapitest")[0]
-#    static_rasters, _ = downloader.rasters_in_scenario(scenario)
-#    static_rasters = [x for x in static_rasters if x["spatial_bounds"]]
-#    static_rasters_urls = downloader.get_static_rasters_links(
-#        static_rasters, "EPSG:4326", 1000, bounds=None, time=None
-#    )
-#    assert isinstance(static_rasters_urls, dict)
-
-
-# def test_get_temporal_raster_links():
-#    scenario = downloader.find_scenarios_by_name("lizardapitest")[0]
-#    _, temporal_rasters = downloader.rasters_in_scenario(scenario)
-#    temporal_rasters = [x for x in temporal_rasters if x["spatial_bounds"]]
-#    temporal_raster = temporal_rasters[0]
-#
-#    temporal_raster_urls = downloader.get_temporal_raster_links(
-#        temporal_raster, "EPSG:4326", 1000, bounds=None, interval_hours=None
-#    )
-#    assert isinstance(temporal_raster_urls, dict) and len(temporal_raster_urls) > 1
-
-
-# def test_get_temporal_rasters_links():
-#    scenario = downloader.find_scenarios_by_name("lizardapitest")[0]
-#    _, temporal_rasters = downloader.rasters_in_scenario(scenario)
-#    temporal_rasters = [x for x in temporal_rasters if x["spatial_bounds"]]
-#    temporal_rasters_urls = downloader.get_temporal_rasters_links(
-#        temporal_rasters, "EPSG:4326", 1000, bounds=None, interval_hours=None
-#    )
-#    assert isinstance(temporal_rasters_urls, dict)
+def test_download_raster():
+    file_path = "threedi_scenario_downloader/tests/testdata/max_wd.tif"
+
+    downloader.download_raster(
+        SCENARIO_UUID,
+        "depth-max-dtri",
+        "EPSG:4326",
+        10,
+        bbox=None,
+        time=None,
+        pathname=file_path,
+    )
+    assert os.path.isfile(file_path)
+
+
+def test_download_raster_batch():
+    scenario_uuids = [SCENARIO_UUID, SCENARIO_UUID]
+
+    file_paths = [
+        "threedi_scenario_downloader/tests/testdata/max_wd_batch_1.tif",
+        "threedi_scenario_downloader/tests/testdata/max_wd_batch_2.tif",
+    ]
+
+    downloader.download_raster(
+        scenario_uuids,
+        "depth-max-dtri",
+        "EPSG:4326",
+        10,
+        bbox=None,
+        time=None,
+        pathname=file_paths,
+    )
+
+    for file_path in file_paths:
+        assert os.path.isfile(file_path)
 
 
 def test_get_raster_timesteps():
-    raster = downloader.get_raster("06c38953-31ec-4f6d-ae1f-ccdf31a348ae", "s1-dtri")
+    raster = downloader.get_raster(SCENARIO_UUID, "s1-dtri")
     timesteps = downloader.get_raster_timesteps(raster, interval_hours=None)
     assert isinstance(timesteps, list) and all(
         isinstance(step, str) for step in timesteps
     )
 
 
 def test_get_raster_from_json():
-    scenario = downloader.find_scenarios_by_model_slug(
-        "005a58d09538e4e4cdbe48f2f3f22aeb89330ae4"
-    )[0]
-    raster = downloader.get_raster_from_json(scenario, "depth-max-dtri")
-    assert raster["uuid"] == "4ef95627-e370-4eba-a5bc-bed661a3101a"
+    scenario_json = downloader.find_scenarios_by_model_slug(MODEL_UUID)[0]
+    raster = downloader.get_raster_from_json(scenario_json, "depth-max-dtri")
+    assert raster["uuid"] == DEPTH_MAX_UUID
 
 
 def test_request_json_from_url():
-    url = (
-        "https://demo.lizard.net/api/v3/scenarios/06c38953-31ec-4f6d-ae1f-ccdf31a348ae/"
-    )
+    url = "https://demo.lizard.net/api/v4/scenarios/{}/".format(SCENARIO_UUID)
     assert isinstance(downloader.request_json_from_url(url, params=None), dict)
```

### Comparing `threedi-scenario-downloader-0.9/README.rst` & `threedi-scenario-downloader-1.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -9,87 +9,97 @@
 - Download raw results.
 - Download logging.
 - Download maximum waterdepth (non-temporal raster).
 - Download waterdepth (temporal raster, supply timestamp for snapshot).
 - Find all scenarios model slug or scenario name.
 
 Examples
-========================================
+--------
+
 Start importing the package::
-  
-  $ from threedi_scenario_downloader import downloader as dl
 
-Set headers for authentication to the Lizard API::
-  
-  $ dl.set_headers("your_username","your_password")
+  >>> from threedi_scenario_downloader import downloader as dl
+
+Set the API key for authentication to the Lizard API (you can get an API key
+here: <your portal>.lizard.net/management/#/personal_api_keys)::
+
+  >>> dl.set_api_key("INSERT YOUR API KEY HERE")
+
+Find scenarios based on a model slug (unique model identifier) or scenario
+name. Returns last 10 matching results unless told otherwise::
 
-Find scenarios based on a model slug (unique model identifier) or scenario name. Returns last 10 matching results unless told otherwise::
+  >>> scenarios = dl.find_scenarios_by_model_slug("enter your model_uuid", limit=10)
 
-  $ scenarios = dl.find_scenarios_by_model_slug("enter your model_uuid",limit=10)
-  
 or::
 
-  $ scenarios = dl.find_scenarios_by_name("my_first_scenario",limit=100)
+  >>> scenarios = dl.find_scenarios_by_name("my_first_scenario", limit=100)
 
-Do you want to download the raw 3Di-results (.nc and .h5 files) of a specific scenario? Use the following methods::
+or if you have too many similarly-named scenarios, do a case-sensitive exact
+search::
 
-  $ dl.download_raw_results("scenario_uuid")
-  $ dl.download_grid_administration("scenario_uuid")
+  >>> scenarios = dl.find_scenarios_by_exact_name("my_first_scenario", limit=100)
 
+Do you want to download the raw 3Di-results (.nc and .h5 files) of a specific
+scenario? Use the following methods::
+
+  >>> dl.download_raw_results("scenario_uuid")
+  >>> dl.download_grid_administration("scenario_uuid")
 
 or::
 
-  $ dl.download_raw_results("scenario_uuid",pathname="save_under_different_name.nc")
-  $ dl.download_grid_administration("scenario_uuid",pathname="save_under_different_name.h5")
+  >>> dl.download_raw_results("scenario_uuid",pathname="save_under_different_name.nc")
+  >>> dl.download_grid_administration("scenario_uuid",pathname="save_under_different_name.h5")
 
-Downloading (temporal) rasters of specific scenarios can be done using the following methods::
+Downloading (temporal) rasters of specific scenarios can be done using the
+following methods::
 
-  $ dl.download_maximum_waterdepth_raster("scenario_uuid","EPSG:28992",10) 
+  >>> dl.download_maximum_waterdepth_raster("scenario_uuid","EPSG:28992",10)
   #download the full extent of the maximum waterdepth of the given scenario_uuid with a 10 meter resolution in the RD New/Amersfoort projection (EPSG:28992)
-  
-  $ dl.download_waterdepth_raster("scenario_uuid","EPSG:28992",10,"2019-01-01T02:00") 
+
+  >>> dl.download_waterdepth_raster("scenario_uuid","EPSG:28992",10,"2019-01-01T02:00")
   #download the full extend of the waterdepth at the supplied timestamp given scenario_uuid, on 10 meter resolution in the RD New/Amersfoort projection (EPSG:28992)
 
-The raster download methods creates a task for the API. Depending on the size and resolution it takes some time for the raster to be prepared. These methods will keep on checking if the raster is ready to be downloaded.
-When a raster is ready to be downloaded a message in the Lizard portal is created as well. If you want to delete these messages (due to bulk downloading for example), use the following method::
+The raster download methods creates a task for the API. Depending on the size
+and resolution it takes some time for the raster to be prepared. These methods
+will keep on checking if the raster is ready to be downloaded.  When a raster
+is ready to be downloaded a message in the Lizard portal is created as
+well. If you want to delete these messages (due to bulk downloading for
+example), use the following method::
+
+  >>> dl.clear_inbox()
 
-  $dl.clear_inbox()
 
 Installation
 ------------
 
 We can be installed with::
 
   $ pip install threedi-scenario-downloader
 
 
 Development installation of this project itself
 -----------------------------------------------
 
-We're installed with `pipenv <https://docs.pipenv.org/>`_, a handy wrapper
-around pip and virtualenv. Install that first with ``pip install
-pipenv``. Then run::
+We're installed with regular pip and virtualenv. Create a virtualenv and call pip::
 
-  $ PIPENV_VENV_IN_PROJECT=1 pipenv --three
-  $ pipenv install --dev
+  $ python3 -m venv .
+  $ bin/pip install -r requirements.txt
 
 In order to get nicely formatted python files without having to spend manual
 work on it, run the following command periodically::
 
-  $ pipenv run black threedi_scenario_downloader
+  $ bin/black threedi_scenario_downloader
 
 Run the tests regularly. This also checks with pyflakes, black and it reports
 coverage. Pure luxury::
 
-  $ pipenv run pytest
+  $ bin/pytest
 
-The tests are also run automatically `on travis-ci
-<https://travis-ci.com/nens/threedi-scenario-downloader>`_, you'll see it in
-the pull requests. There's also `coverage reporting
-<https://coveralls.io/github/nens/threedi-scenario-downloader>`_ on
-coveralls.io.
+The tests **used** to run on travis-ci.org, but we don't use that service
+anymore. Also, new releases were automatically added to pypi there. For now,
+contact Reinout when you need a new release.
 
 If you need a new dependency (like `requests`), add it in `setup.py` in
 `install_requires`. Afterwards, run install again to actuall install your
 dependency::
 
-  $ pipenv install --dev
+  $ bin/pip install -r requirements.txt
```

### Comparing `threedi-scenario-downloader-0.9/setup.py` & `threedi-scenario-downloader-1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.9"
+version = "1.0"
 long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read()])
 install_requires = ["requests"]
 tests_require = ["pytest", "mock", "pytest-cov", "pytest-flakes", "pytest-black"]
 setup(
     name="threedi-scenario-downloader",
     version=version,
     description="Tools for downloading results for 3Di scenarios",
```

